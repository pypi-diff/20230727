# Comparing `tmp/intellect_core-0.2.2.tar.gz` & `tmp/intellect_core-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intellect_core-0.2.2.tar", max compression
+gzip compressed data, was "intellect_core-0.2.3.tar", max compression
```

## Comparing `intellect_core-0.2.2.tar` & `intellect_core-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      186 2023-07-04 13:46:17.485985 intellect_core-0.2.2/LICENSE
--rw-r--r--   0        0        0      171 2023-07-04 13:46:17.485985 intellect_core-0.2.2/README.md
--rw-r--r--   0        0        0     5366 2023-07-27 13:43:42.953220 intellect_core-0.2.2/intellect_core/core.py
--rw-r--r--   0        0        0        0 2023-07-04 13:46:17.485985 intellect_core-0.2.2/intellect_core/dto/__init__.py
--rw-r--r--   0        0        0     2592 2023-07-27 13:43:42.945220 intellect_core-0.2.2/intellect_core/dto/dto.py
--rw-r--r--   0        0        0     1023 2023-07-11 08:28:49.676801 intellect_core-0.2.2/intellect_core/handler.py
--rw-r--r--   0        0        0      306 2023-07-27 13:45:43.941287 intellect_core-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-07-04 13:46:17.485985 intellect_core-0.2.3/LICENSE
+-rw-r--r--   0        0        0      171 2023-07-04 13:46:17.485985 intellect_core-0.2.3/README.md
+-rw-r--r--   0        0        0     5380 2023-07-27 14:17:45.361375 intellect_core-0.2.3/intellect_core/core.py
+-rw-r--r--   0        0        0        0 2023-07-04 13:46:17.485985 intellect_core-0.2.3/intellect_core/dto/__init__.py
+-rw-r--r--   0        0        0     3121 2023-07-27 14:50:24.206218 intellect_core-0.2.3/intellect_core/dto/dto.py
+-rw-r--r--   0        0        0     1023 2023-07-11 08:28:49.676801 intellect_core-0.2.3/intellect_core/handler.py
+-rw-r--r--   0        0        0      306 2023-07-27 14:58:44.653584 intellect_core-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.2.3/PKG-INFO
```

### Comparing `intellect_core-0.2.2/intellect_core/core.py` & `intellect_core-0.2.3/intellect_core/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     def _connection(self, session: requests.Session, url: str):
         try:
             response = session.get(url,
                                    verify=self.config.certificate_path if self.config.certificate_path else False)
             if self.log_debug:
                 logger.debug(
-                    f"response: {response.text}")
+                    f"\nURL: {url}\nResponse: {response.text}")
         except requests.exceptions.ConnectionError as e:
             session.close()
             logger.error(f"Intellect connection error: {e}")
 
     def logic(self, object_type: ObjectType,
               command: CoreCommand,
               dto: IntellectVisitDto.Create | IntellectVisitDto.Update | None,
```

### Comparing `intellect_core-0.2.2/intellect_core/dto/dto.py` & `intellect_core-0.2.3/intellect_core/dto/dto.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 from enum import Enum
 
 from pydantic import BaseModel
 
 
 class ResponseMethod(Enum):
     GET = "GET"
@@ -53,14 +54,17 @@
         phone: str | None  # phone
         visit_birthplace: str | None  # place_of_birth
         visit_reg: str | None  # registration
         facility_code: str | None
         level_id: int | None  # access_level
         visit_purpose: str | None
         card: str | None
+        service_photo: str | None = ""
+        expired: str | None = "" # действительна до (datetime.now() + timedelta(days=1)).strftime("%d.%m.%Y %H:%M:%S")
+        begin: str | None = "" # начало действия карты (datetime.now()).strftime("%d.%m.%Y %H:%M:%S")
 
     class Update(BaseModel):
         objid: int
         name: str | None  # second_name
         surname: str | None  # first_name
         patronymic: str | None  # middle_name
         parent_id: int | None  # department_id
@@ -69,29 +73,32 @@
         visit_birthplace: str | None  # place_of_birth
         visit_reg: str | None  # registration
         facility_code: str | None
         level_id: int | None  # access_level
         visit_purpose: str | None
         card: str | None
         temp_card: str | None
+        service_photo: str | None = ""
+        expired: str | None = ""  # действительна до (datetime.now() + timedelta(days=1)).strftime("%d.%m.%Y %H:%M:%S")
+        begin: str | None = ""  # начало действия карты (datetime.now()).strftime("%d.%m.%Y %H:%M:%S")
 
 
 class IntellectDepartmentDto:
     class Create(BaseModel):
         objid: int
         name: str  # unique_name
         schedule_id: str | None = ""
         level_id: str | None = ""
         region_id: str | None = ""
         external_id: str | None = ""
         owner_id: str | None = ""
-        service_photo: str| None = ""
+
 
     class Update(BaseModel):
         schedule_id: str | None = ""
         objid: str | None = ""
         name: str | None = ""
         level_id: str | None = ""
         region_id: str | None = ""
         external_id: str | None = ""
         owner_id: str | None = ""
-        service_photo: str | None = ""
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `intellect_core-0.2.2/intellect_core/handler.py` & `intellect_core-0.2.3/intellect_core/handler.py`

 * *Files identical despite different names*

### Comparing `intellect_core-0.2.2/PKG-INFO` & `intellect_core-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intellect-core
-Version: 0.2.2
+Version: 0.2.3
 Summary: Модуль интеграции с Интеллект
 Author: Mrkorogod
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

