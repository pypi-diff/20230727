# Comparing `tmp/mypyllant-0.3.3.tar.gz` & `tmp/mypyllant-0.4.0.tar.gz`

## Comparing `mypyllant-0.3.3.tar` & `mypyllant-0.4.0.tar`

### file list

```diff
@@ -1,43 +1,37 @@
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.3.3/logo.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.3.3/requirements-dev.txt
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.3.3/run_pytest.sh
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.3.3/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    17950 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/api.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2782 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/export.py
--rw-r--r--   0        0        0     8610 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/py.typed
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/sample.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/__init__.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/conftest.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/find_countries.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/generate_test_data.py
--rw-r--r--   0        0        0     7808 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/test_api.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/test_countries.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/test_export.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/test_generate_test_data.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/test_sample.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/update_sample.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/claims.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/connection_status.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/control_identifier.json
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/current_system.json
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/device_buckets.json
--rw-r--r--   0        0        0     9669 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/system.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/time_zone.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
--rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.3.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.3.3/LICENSE
--rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 mypyllant-0.3.3/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 mypyllant-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.4.0/logo.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.4.0/requirements-dev.txt
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.4.0/run_pytest.sh
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.4.0/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    19167 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/api.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2782 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/export.py
+-rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/py.typed
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/__init__.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/conftest.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/find_countries.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/generate_test_data.py
+-rw-r--r--   0        0        0     7808 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/test_api.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/test_countries.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/test_export.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/test_sample.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/update_sample.py
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/utils.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/firmware_update_required.json
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 mypyllant-0.4.0/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 mypyllant-0.4.0/PKG-INFO
```

### Comparing `mypyllant-0.3.3/.pre-commit-config.yaml` & `mypyllant-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/logo.png` & `mypyllant-0.4.0/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/.github/workflows/build-test.yaml` & `mypyllant-0.4.0/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/src/myPyllant/api.py` & `mypyllant-0.4.0/src/myPyllant/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -229,15 +229,18 @@
         async with self.aiohttp_session.get(
             f"{API_URL_BASE}/claims", headers=self.get_authorized_headers()
         ) as claims_resp:
             for claim_json in await claims_resp.json():
                 yield Claim(**dict_to_snake_case(claim_json))
 
     async def get_systems(
-        self, include_timezone=False, include_connection_status=False
+        self,
+        include_timezone=False,
+        include_connection_status=False,
+        include_firmware_update_required=False,
     ) -> AsyncIterator[System]:
         logger.debug(
             f"Getting systems with include_timezone={include_timezone}"
             f" and include_connection_status={include_connection_status}"
         )
         claims = self.get_claims()
         async for claim in claims:
@@ -263,14 +266,19 @@
                 claim=claim,
                 timezone=await self.get_time_zone(claim.system_id)
                 if include_timezone
                 else None,
                 connected=await self.get_connection_status(claim.system_id)
                 if include_connection_status
                 else None,
+                firmware_update_required=await self.get_firmware_update_required(
+                    claim.system_id
+                )
+                if include_firmware_update_required
+                else None,
                 current_system=dict_to_snake_case(current_system_json),
                 **dict_to_snake_case(system_json),
             )
             yield system
 
     async def get_data_by_device(
         self,
@@ -355,14 +363,32 @@
                 json={
                     "desiredRoomTemperatureSetpoint": temperature,
                     "duration": duration_hours if duration_hours else default_duration,
                 },
                 headers=self.get_authorized_headers(),
             )
 
+    async def set_manual_mode_setpoint(
+        self,
+        zone: Zone,
+        temperature: float,
+        setpoint_type: str = "HEATING",
+    ):
+        logger.debug(f"Setting manual mode setpoint for {zone.name}")
+        url = f"{API_URL_BASE}/systems/{zone.system_id}/tli/zones/{zone.index}/manual-mode-setpoint"
+        payload = {
+            "setpoint": temperature,
+            "type": setpoint_type,
+        }
+        return await self.aiohttp_session.patch(
+            url,
+            json=payload,
+            headers=self.get_authorized_headers(),
+        )
+
     async def cancel_quick_veto_zone_temperature(self, zone: Zone):
         url = f"{API_URL_BASE}/systems/{zone.system_id}/zones/{zone.index}/quickVeto"
         return await self.aiohttp_session.delete(
             url, headers=self.get_authorized_headers()
         )
 
     async def set_set_back_temperature(self, zone: Zone, temperature: float):
@@ -474,7 +500,15 @@
         )
         try:
             tz = (await response.json())["timeZone"]
             return gettz(tz)
         except KeyError:
             logger.warning("Couldn't get timezone from API")
             return None
+
+    async def get_firmware_update_required(self, system: System | str) -> bool:
+        url = f"{API_URL_BASE}/firmware-update-required/{self.get_system_id(system)}"
+        response = await self.aiohttp_session.get(
+            url,
+            headers=self.get_authorized_headers(),
+        )
+        return (await response.json())["firmwareUpdateRequired"]
```

### Comparing `mypyllant-0.3.3/src/myPyllant/const.py` & `mypyllant-0.4.0/src/myPyllant/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,9 +52,14 @@
         "poland": "Poland",
         "portugal": "Portugal",
         "romania": "Romania",
         "slovakia": "Slovakia",
         "spain": "Spain",
     },
 }
+MANUAL_SETPOINT_TYPES = {
+    "HEATING": "Heating",
+    "COOLING": "Cooling",
+}
+DEFAULT_MANUAL_SETPOINT_TYPE = "HEATING"
 DEFAULT_QUICK_VETO_DURATION = 3
 DEFAULT_CONTROL_IDENTIFIER = "tli"
```

### Comparing `mypyllant-0.3.3/src/myPyllant/export.py` & `mypyllant-0.4.0/src/myPyllant/export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/src/myPyllant/models.py` & `mypyllant-0.4.0/src/myPyllant/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
     properties: dict
     configuration: dict
     zones: list[Zone] = []
     circuits: list[Circuit] = []
     domestic_hot_water: list[DomesticHotWater] = []
     devices: list["Device"] = []
     timezone: datetime.tzinfo | None
+    firmware_update_required: bool | None
     connected: bool | None
 
     def __init__(self, **data: Any) -> None:
         if "claim" in data and "id" not in data:
             data["id"] = data["claim"].system_id
         super().__init__(**data)
         logger.debug(f"Creating related models from state: {data}")
```

### Comparing `mypyllant-0.3.3/src/myPyllant/sample.py` & `mypyllant-0.4.0/src/myPyllant/sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/src/myPyllant/utils.py` & `mypyllant-0.4.0/src/myPyllant/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/src/myPyllant/tests/find_countries.py` & `mypyllant-0.4.0/src/myPyllant/tests/find_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/src/myPyllant/tests/generate_test_data.py` & `mypyllant-0.4.0/src/myPyllant/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/src/myPyllant/tests/test_api.py` & `mypyllant-0.4.0/src/myPyllant/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/src/myPyllant/tests/test_countries.py` & `mypyllant-0.4.0/src/myPyllant/tests/test_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/src/myPyllant/tests/test_export.py` & `mypyllant-0.4.0/src/myPyllant/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/src/myPyllant/tests/test_generate_test_data.py` & `mypyllant-0.4.0/src/myPyllant/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/src/myPyllant/tests/update_sample.py` & `mypyllant-0.4.0/src/myPyllant/tests/update_sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/src/myPyllant/tests/utils.py` & `mypyllant-0.4.0/src/myPyllant/tests/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -137,14 +137,20 @@
                 )
                 self.get(
                     re.compile(r".*meta-info/connection-status"),
                     status=200,
                     payload=self.test_data["connection_status"],
                     repeat=True,
                 )
+                self.get(
+                    re.compile(r".*firmware-update-required.*"),
+                    status=200,
+                    payload=self.test_data["firmware_update_required"],
+                    repeat=True,
+                )
             return self
 
     return _mypyllant_aioresponses
 
 
 async def _mocked_api(*args, **kwargs) -> MyPyllantAPI:
     api = MyPyllantAPI("test@example.com", "test", "germany", "vaillant")
```

### Comparing `mypyllant-0.3.3/src/myPyllant/tests/json/030f109526faf40c523f7ac79f8a0d7e368b2938/device_buckets.json` & `mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6850198412698413%*

 * *Differences: {"'data'": "{0: {'startDate': '2023-07-24T00:00:00Z', 'endDate': '2023-07-24T01:00:00Z', 'value': "*

 * *           "68.965515}, 1: {'startDate': '2023-07-24T01:00:00Z', 'endDate': "*

 * *           "'2023-07-24T02:00:00Z', 'value': 68.965515}, 2: {'startDate': '2023-07-24T02:00:00Z', "*

 * *           "'endDate': '2023-07-24T03:00:00Z', 'value': 68.965515}, 3: {'startDate': "*

 * *           "'2023-07-24T03:00:00Z', 'endDate': '2023-07-24T04:00:00Z', 'value': 68.965515}, 4: "*

 * *           "{'startDate': '2023-07-24T04:00:00Z',  […]*

```diff
@@ -1,129 +1,130 @@
 {
     "data": [
         {
-            "endDate": "2023-04-23T01:00:00Z",
-            "startDate": "2023-04-23T00:00:00Z",
-            "value": 0.0
+            "endDate": "2023-07-24T01:00:00Z",
+            "startDate": "2023-07-24T00:00:00Z",
+            "value": 68.965515
         },
         {
-            "endDate": "2023-04-23T02:00:00Z",
-            "startDate": "2023-04-23T01:00:00Z",
-            "value": 0.0
+            "endDate": "2023-07-24T02:00:00Z",
+            "startDate": "2023-07-24T01:00:00Z",
+            "value": 68.965515
         },
         {
-            "endDate": "2023-04-23T03:00:00Z",
-            "startDate": "2023-04-23T02:00:00Z",
-            "value": 0.0
+            "endDate": "2023-07-24T03:00:00Z",
+            "startDate": "2023-07-24T02:00:00Z",
+            "value": 68.965515
         },
         {
-            "endDate": "2023-04-23T04:00:00Z",
-            "startDate": "2023-04-23T03:00:00Z",
-            "value": 0.0
+            "endDate": "2023-07-24T04:00:00Z",
+            "startDate": "2023-07-24T03:00:00Z",
+            "value": 68.965515
         },
         {
-            "endDate": "2023-04-23T05:00:00Z",
-            "startDate": "2023-04-23T04:00:00Z",
-            "value": 0.0
+            "endDate": "2023-07-24T05:00:00Z",
+            "startDate": "2023-07-24T04:00:00Z",
+            "value": 68.965515
         },
         {
-            "endDate": "2023-04-23T06:00:00Z",
-            "startDate": "2023-04-23T05:00:00Z",
-            "value": 135.5625
+            "endDate": "2023-07-24T06:00:00Z",
+            "startDate": "2023-07-24T05:00:00Z",
+            "value": 346.0309
         },
         {
-            "endDate": "2023-04-23T07:00:00Z",
-            "startDate": "2023-04-23T06:00:00Z",
-            "value": 1135.5625
+            "endDate": "2023-07-24T07:00:00Z",
+            "startDate": "2023-07-24T06:00:00Z",
+            "value": 702.4173
         },
         {
-            "endDate": "2023-04-23T08:00:00Z",
-            "startDate": "2023-04-23T07:00:00Z",
-            "value": 1728.875
+            "endDate": "2023-07-24T08:00:00Z",
+            "startDate": "2023-07-24T07:00:00Z",
+            "value": 0.0
         },
         {
-            "endDate": "2023-04-23T09:00:00Z",
-            "startDate": "2023-04-23T08:00:00Z",
+            "endDate": "2023-07-24T09:00:00Z",
+            "startDate": "2023-07-24T08:00:00Z",
             "value": 0.0
         },
         {
-            "endDate": "2023-04-23T10:00:00Z",
-            "startDate": "2023-04-23T09:00:00Z",
+            "endDate": "2023-07-24T10:00:00Z",
+            "startDate": "2023-07-24T09:00:00Z",
             "value": 0.0
         },
         {
-            "endDate": "2023-04-23T11:00:00Z",
-            "startDate": "2023-04-23T10:00:00Z",
+            "endDate": "2023-07-24T11:00:00Z",
+            "startDate": "2023-07-24T10:00:00Z",
             "value": 0.0
         },
         {
-            "endDate": "2023-04-23T12:00:00Z",
-            "startDate": "2023-04-23T11:00:00Z",
+            "endDate": "2023-07-24T12:00:00Z",
+            "startDate": "2023-07-24T11:00:00Z",
             "value": 0.0
         },
         {
-            "endDate": "2023-04-23T13:00:00Z",
-            "startDate": "2023-04-23T12:00:00Z",
-            "value": 0.0
+            "endDate": "2023-07-24T13:00:00Z",
+            "startDate": "2023-07-24T12:00:00Z",
+            "value": 297.69507
         },
         {
-            "endDate": "2023-04-23T14:00:00Z",
-            "startDate": "2023-04-23T13:00:00Z",
-            "value": 135.5625
+            "endDate": "2023-07-24T14:00:00Z",
+            "startDate": "2023-07-24T13:00:00Z",
+            "value": 702.3049
         },
         {
-            "endDate": "2023-04-23T15:00:00Z",
-            "startDate": "2023-04-23T14:00:00Z",
-            "value": 864.4375
+            "endDate": "2023-07-24T15:00:00Z",
+            "startDate": "2023-07-24T14:00:00Z",
+            "value": 0.0
         },
         {
-            "endDate": "2023-04-23T16:00:00Z",
-            "startDate": "2023-04-23T15:00:00Z",
+            "endDate": "2023-07-24T16:00:00Z",
+            "startDate": "2023-07-24T15:00:00Z",
             "value": 0.0
         },
         {
-            "endDate": "2023-04-23T17:00:00Z",
-            "startDate": "2023-04-23T16:00:00Z",
+            "endDate": "2023-07-24T17:00:00Z",
+            "startDate": "2023-07-24T16:00:00Z",
             "value": 0.0
         },
         {
-            "endDate": "2023-04-23T18:00:00Z",
-            "startDate": "2023-04-23T17:00:00Z",
+            "endDate": "2023-07-24T18:00:00Z",
+            "startDate": "2023-07-24T17:00:00Z",
             "value": 0.0
         },
         {
-            "endDate": "2023-04-23T19:00:00Z",
-            "startDate": "2023-04-23T18:00:00Z",
+            "endDate": "2023-07-24T19:00:00Z",
+            "startDate": "2023-07-24T18:00:00Z",
             "value": 0.0
         },
         {
-            "endDate": "2023-04-23T20:00:00Z",
-            "startDate": "2023-04-23T19:00:00Z",
+            "endDate": "2023-07-24T20:00:00Z",
+            "startDate": "2023-07-24T19:00:00Z",
             "value": 0.0
         },
         {
-            "endDate": "2023-04-23T21:00:00Z",
-            "startDate": "2023-04-23T20:00:00Z",
+            "endDate": "2023-07-24T21:00:00Z",
+            "startDate": "2023-07-24T20:00:00Z",
             "value": 0.0
         },
         {
-            "endDate": "2023-04-23T22:00:00Z",
-            "startDate": "2023-04-23T21:00:00Z",
+            "endDate": "2023-07-24T22:00:00Z",
+            "startDate": "2023-07-24T21:00:00Z",
             "value": 0.0
         },
         {
-            "endDate": "2023-04-23T23:00:00Z",
-            "startDate": "2023-04-23T22:00:00Z",
+            "endDate": "2023-07-24T23:00:00Z",
+            "startDate": "2023-07-24T22:00:00Z",
             "value": 0.0
         },
         {
-            "endDate": "2023-04-24T00:00:00Z",
-            "startDate": "2023-04-23T23:00:00Z",
+            "endDate": "2023-07-25T00:00:00Z",
+            "startDate": "2023-07-24T23:00:00Z",
             "value": 0.0
         }
     ],
-    "endDate": "2023-04-24T00:00:00Z",
+    "endDate": "2023-07-25T00:00:00Z",
     "energyType": "CONSUMED_ELECTRICAL_ENERGY",
     "operationMode": "DOMESTIC_HOT_WATER",
     "resolution": "HOUR",
-    "startDate": "2023-04-23T00:00:00Z"
+    "startDate": "2023-07-24T00:00:00Z",
+    "totalConsumption": 2393.276
 }
```

### Comparing `mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json` & `mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json` & `mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/.gitignore` & `mypyllant-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/LICENSE` & `mypyllant-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/README.md` & `mypyllant-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -123,18 +123,35 @@
 Copy the resulting dictionary into [src/myPyllant/const.py](src/myPyllant/const.py)
 
 ### Contributing Test Data
 
 Because the myVAILLANT API isn't documented, you can help the development of this library by contributing test data:
 
 ```shell
+python3 -m myPyllant.tests.generate_test_data -h
 python3 -m myPyllant.tests.generate_test_data username password country brand
 ```
 
-Create a fork of this repository and create a PR with the newly created folder in `src/myPyllant/tests/json`.
+This creates a new folder with JSON values from the API in `src/myPyllant/tests/json`.
+Check the timestamp on the folders, if you're unsure which one is yours.
+
+You can then either create a PR with the newly created folder, or zip it and attach it to an issue.
+
+### Reverse Engineering API requests of the myVAILLANT app
+
+You'll need an Android device and a computer with ADB on the same network.
+
+1. Run mitmproxy, for example in Docker: `docker run --rm -it -v ~/.mitmproxy:/home/mitmproxy/.mitmproxy -p 0.0.0.0:8080:8080 -p 127.0.0.1:8081:8081 mitmproxy/mitmproxy mitmweb --web-host 0.0.0.0`
+2. In the WIFI connection settings of your Android device, set a manual proxy to the IP of the computer running mitmproxy on port 8080, with an exception for `identity.vaillant-group.com` (which opens in your browser and uses HSTS)
+3. Visit http://mitm.it/ on your Android device, download the CA cert & install it through the settings app
+4. Install ADB and connect your Android device to USB in debug mode
+5. Look for the myVAILLANT APK and download it
+6. Run https://github.com/mitmproxy/android-unpinner on the APK and wait for it to launch the modified app on your Android device with ADB
+7. You should see all API calls in mitmproxy's web interface on http://127.0.0.1:8081 now. If you can't log in because of a certificate error, make sure you added the exception to the proxy settings.
+   If you can log in, but the app reports an error, the unpinning didn't work. You can try https://github.com/NVISOsecurity/MagiskTrustUserCertson if you have a rooted Android device
 
 ## Notes
 
 * Auth is loosely based on https://github.com/TA2k/ioBroker.vaillant
 * Most API endpoints are reverse-engineered from the myVaillant app, using https://github.com/mitmproxy/mitmproxy
 * Setting weekly time tables for heating and domestic hot water is still missing
 * There is a home assistant component based on this library here: https://github.com/signalkraft/mypyllant-component
```

### Comparing `mypyllant-0.3.3/pyproject.toml` & `mypyllant-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.3.3/PKG-INFO` & `mypyllant-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.3.3
+Version: 0.4.0
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -139,18 +139,35 @@
 Copy the resulting dictionary into [src/myPyllant/const.py](src/myPyllant/const.py)
 
 ### Contributing Test Data
 
 Because the myVAILLANT API isn't documented, you can help the development of this library by contributing test data:
 
 ```shell
+python3 -m myPyllant.tests.generate_test_data -h
 python3 -m myPyllant.tests.generate_test_data username password country brand
 ```
 
-Create a fork of this repository and create a PR with the newly created folder in `src/myPyllant/tests/json`.
+This creates a new folder with JSON values from the API in `src/myPyllant/tests/json`.
+Check the timestamp on the folders, if you're unsure which one is yours.
+
+You can then either create a PR with the newly created folder, or zip it and attach it to an issue.
+
+### Reverse Engineering API requests of the myVAILLANT app
+
+You'll need an Android device and a computer with ADB on the same network.
+
+1. Run mitmproxy, for example in Docker: `docker run --rm -it -v ~/.mitmproxy:/home/mitmproxy/.mitmproxy -p 0.0.0.0:8080:8080 -p 127.0.0.1:8081:8081 mitmproxy/mitmproxy mitmweb --web-host 0.0.0.0`
+2. In the WIFI connection settings of your Android device, set a manual proxy to the IP of the computer running mitmproxy on port 8080, with an exception for `identity.vaillant-group.com` (which opens in your browser and uses HSTS)
+3. Visit http://mitm.it/ on your Android device, download the CA cert & install it through the settings app
+4. Install ADB and connect your Android device to USB in debug mode
+5. Look for the myVAILLANT APK and download it
+6. Run https://github.com/mitmproxy/android-unpinner on the APK and wait for it to launch the modified app on your Android device with ADB
+7. You should see all API calls in mitmproxy's web interface on http://127.0.0.1:8081 now. If you can't log in because of a certificate error, make sure you added the exception to the proxy settings.
+   If you can log in, but the app reports an error, the unpinning didn't work. You can try https://github.com/NVISOsecurity/MagiskTrustUserCertson if you have a rooted Android device
 
 ## Notes
 
 * Auth is loosely based on https://github.com/TA2k/ioBroker.vaillant
 * Most API endpoints are reverse-engineered from the myVaillant app, using https://github.com/mitmproxy/mitmproxy
 * Setting weekly time tables for heating and domestic hot water is still missing
 * There is a home assistant component based on this library here: https://github.com/signalkraft/mypyllant-component
```

