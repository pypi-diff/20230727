# Comparing `tmp/intellect_core-0.2.1.tar.gz` & `tmp/intellect_core-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intellect_core-0.2.1.tar", max compression
+gzip compressed data, was "intellect_core-0.2.2.tar", max compression
```

## Comparing `intellect_core-0.2.1.tar` & `intellect_core-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      186 2023-07-04 13:46:17.485985 intellect_core-0.2.1/LICENSE
--rw-r--r--   0        0        0      171 2023-07-04 13:46:17.485985 intellect_core-0.2.1/README.md
--rw-r--r--   0        0        0     5340 2023-07-24 15:03:14.421323 intellect_core-0.2.1/intellect_core/core.py
--rw-r--r--   0        0        0        0 2023-07-04 13:46:17.485985 intellect_core-0.2.1/intellect_core/dto/__init__.py
--rw-r--r--   0        0        0     2515 2023-07-24 13:16:58.644497 intellect_core-0.2.1/intellect_core/dto/dto.py
--rw-r--r--   0        0        0     1023 2023-07-11 08:28:49.676801 intellect_core-0.2.1/intellect_core/handler.py
--rw-r--r--   0        0        0      306 2023-07-24 15:04:51.681126 intellect_core-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-07-04 13:46:17.485985 intellect_core-0.2.2/LICENSE
+-rw-r--r--   0        0        0      171 2023-07-04 13:46:17.485985 intellect_core-0.2.2/README.md
+-rw-r--r--   0        0        0     5366 2023-07-27 13:43:42.953220 intellect_core-0.2.2/intellect_core/core.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:46:17.485985 intellect_core-0.2.2/intellect_core/dto/__init__.py
+-rw-r--r--   0        0        0     2592 2023-07-27 13:43:42.945220 intellect_core-0.2.2/intellect_core/dto/dto.py
+-rw-r--r--   0        0        0     1023 2023-07-11 08:28:49.676801 intellect_core-0.2.2/intellect_core/handler.py
+-rw-r--r--   0        0        0      306 2023-07-27 13:45:43.941287 intellect_core-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.2.2/PKG-INFO
```

### Comparing `intellect_core-0.2.1/intellect_core/core.py` & `intellect_core-0.2.2/intellect_core/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 class Intellect:
     log_debug: bool = False
     config: IntellectConfigDto
     autarization_info: AutarizationInfo | None
     expire_token_date: str
 
-
     def init(self, intellect_config: IntellectConfigDto):
         self.config = intellect_config
 
     def _get_url(self, object_type: ObjectType, command: CoreCommand,
                  dto: IntellectVisitDto.Create | IntellectVisitDto.Update | None,
                  objid: int | None) -> str:
         url = ""
@@ -35,30 +34,31 @@
             return url[0:-1]
         else:
             url = url + f"objid<{objid}>"
             return url
 
     def autarization(self):
         session = requests.Session()
+
         try:
             if not self.config.https:
                 url = f"http://{self.config.host_user}:{self.config.host_password}@{self.config.intellect_host}:{self.config.intellect_port}/token?expires_in={self.config.token_expires}"
                 response = session.get(url)
             if self.config.https:
                 url = f"https://{self.config.intellect_host}/token?expires_in={self.config.token_expires}"
                 response = requests.get(url,
                                         verify=self.config.certificate_path if self.config.certificate_path else False)
+
                 if response.status_code != 200:
-                    logger.warning(f"\nIntellect server error:  \nCode: {response.status_code}\nReason: {response.reason}\nHeaders: {response.headers}\nResponse text: {response.text}")
+                    logger.warning(
+                        f"\nIntellect server error:  \nCode: {response.status_code}\nReason: {response.reason}\nHeaders: {response.headers}\nResponse text: {response.text}")
                     return
 
             string = "{" + (response.text).replace("\n", ",")[2:-2] + "}"
-
             self.autarization_info = AutarizationInfo(**json.loads(string))
-
             self.expire_token_date = datetime.now() + timedelta(
                 seconds=self.autarization_info.expires_in)
 
             if self.log_debug:
                 logger.debug(
                     f"response: {response.text}")
 
@@ -67,15 +67,15 @@
             logger.warning(f"Intellect connection error: {e}\n"
                            f"Next try in {self.expire_token_date + timedelta(minutes=self.config.retry_to_connection_in_minute)}")
             session.close()
         except ValidationError as ex:
             logger.debug(response.status_code)
             self.expire_token_date = datetime.now()
             logger.warning(f"Intellect connection error: validation error: {ex}\n"
-                         f"Next try in {self.expire_token_date + timedelta(minutes=self.config.retry_to_connection_in_minute)}")
+                           f"Next try in {self.expire_token_date + timedelta(minutes=self.config.retry_to_connection_in_minute)}")
             session.close()
         return
 
     def _connection(self, session: requests.Session, url: str):
         try:
             response = session.get(url,
                                    verify=self.config.certificate_path if self.config.certificate_path else False)
```

### Comparing `intellect_core-0.2.1/intellect_core/dto/dto.py` & `intellect_core-0.2.2/intellect_core/dto/dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,16 +80,18 @@
         objid: int
         name: str  # unique_name
         schedule_id: str | None = ""
         level_id: str | None = ""
         region_id: str | None = ""
         external_id: str | None = ""
         owner_id: str | None = ""
+        service_photo: str| None = ""
 
     class Update(BaseModel):
         schedule_id: str | None = ""
         objid: str | None = ""
         name: str | None = ""
         level_id: str | None = ""
         region_id: str | None = ""
         external_id: str | None = ""
         owner_id: str | None = ""
+        service_photo: str | None = ""
```

### Comparing `intellect_core-0.2.1/intellect_core/handler.py` & `intellect_core-0.2.2/intellect_core/handler.py`

 * *Files identical despite different names*

### Comparing `intellect_core-0.2.1/PKG-INFO` & `intellect_core-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intellect-core
-Version: 0.2.1
+Version: 0.2.2
 Summary: Модуль интеграции с Интеллект
 Author: Mrkorogod
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

