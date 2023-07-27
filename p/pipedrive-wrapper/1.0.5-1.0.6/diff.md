# Comparing `tmp/pipedrive-wrapper-1.0.5.tar.gz` & `tmp/pipedrive-wrapper-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipedrive-wrapper-1.0.5.tar", last modified: Sat Jul 22 15:53:38 2023, max compression
+gzip compressed data, was "pipedrive-wrapper-1.0.6.tar", last modified: Thu Jul 27 21:26:47 2023, max compression
```

## Comparing `pipedrive-wrapper-1.0.5.tar` & `pipedrive-wrapper-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 15:53:38.842350 pipedrive-wrapper-1.0.5/
--rw-rw-rw-   0        0        0     1092 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      705 2023-07-22 15:53:38.842350 pipedrive-wrapper-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       65 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 15:53:38.814249 pipedrive-wrapper-1.0.5/pipedrive/
--rw-rw-rw-   0        0        0        0 2023-05-07 15:48:01.000000 pipedrive-wrapper-1.0.5/pipedrive/__init__.py
--rw-rw-rw-   0        0        0     3628 2023-07-16 14:41:55.000000 pipedrive-wrapper-1.0.5/pipedrive/activity.py
--rw-rw-rw-   0        0        0     2993 2023-07-22 15:22:11.000000 pipedrive-wrapper-1.0.5/pipedrive/client.py
--rw-rw-rw-   0        0        0     6459 2023-07-22 15:16:43.000000 pipedrive-wrapper-1.0.5/pipedrive/deal.py
--rw-rw-rw-   0        0        0     1323 2023-07-22 15:38:22.000000 pipedrive-wrapper-1.0.5/pipedrive/deal_field.py
--rw-rw-rw-   0        0        0      855 2023-06-06 19:39:27.000000 pipedrive-wrapper-1.0.5/pipedrive/exceptions.py
--rw-rw-rw-   0        0        0     5541 2023-07-16 14:42:13.000000 pipedrive-wrapper-1.0.5/pipedrive/person.py
--rw-rw-rw-   0        0        0     3319 2023-06-06 19:04:08.000000 pipedrive-wrapper-1.0.5/pipedrive/util.py
-drwxrwxrwx   0        0        0        0 2023-07-22 15:53:38.841352 pipedrive-wrapper-1.0.5/pipedrive_wrapper.egg-info/
--rw-rw-rw-   0        0        0      705 2023-07-22 15:53:38.000000 pipedrive-wrapper-1.0.5/pipedrive_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-22 15:53:38.000000 pipedrive-wrapper-1.0.5/pipedrive_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 15:53:38.000000 pipedrive-wrapper-1.0.5/pipedrive_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-22 15:53:38.000000 pipedrive-wrapper-1.0.5/pipedrive_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-22 15:53:38.000000 pipedrive-wrapper-1.0.5/pipedrive_wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 15:53:38.842350 pipedrive-wrapper-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-07-22 15:53:24.000000 pipedrive-wrapper-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:26:47.819090 pipedrive-wrapper-1.0.6/
+-rw-rw-rw-   0        0        0     1092 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      705 2023-07-27 21:26:47.819090 pipedrive-wrapper-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2023-05-07 15:23:08.000000 pipedrive-wrapper-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 21:26:47.813088 pipedrive-wrapper-1.0.6/pipedrive/
+-rw-rw-rw-   0        0        0        0 2023-05-07 15:48:01.000000 pipedrive-wrapper-1.0.6/pipedrive/__init__.py
+-rw-rw-rw-   0        0        0     3904 2023-07-27 20:00:05.000000 pipedrive-wrapper-1.0.6/pipedrive/activity.py
+-rw-rw-rw-   0        0        0     4242 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.6/pipedrive/client.py
+-rw-rw-rw-   0        0        0     6504 2023-07-27 19:52:36.000000 pipedrive-wrapper-1.0.6/pipedrive/deal.py
+-rw-rw-rw-   0        0        0     1321 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.6/pipedrive/deal_field.py
+-rw-rw-rw-   0        0        0      855 2023-06-06 19:39:27.000000 pipedrive-wrapper-1.0.6/pipedrive/exceptions.py
+-rw-rw-rw-   0        0        0     5537 2023-07-26 14:59:47.000000 pipedrive-wrapper-1.0.6/pipedrive/person.py
+-rw-rw-rw-   0        0        0     3319 2023-06-06 19:04:08.000000 pipedrive-wrapper-1.0.6/pipedrive/util.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:26:47.818088 pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/
+-rw-rw-rw-   0        0        0      705 2023-07-27 21:26:47.000000 pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-07-27 21:26:47.000000 pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 21:26:47.000000 pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 21:26:47.000000 pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 21:26:47.000000 pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 21:26:47.819090 pipedrive-wrapper-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-07-27 21:15:20.000000 pipedrive-wrapper-1.0.6/setup.py
```

### Comparing `pipedrive-wrapper-1.0.5/LICENSE` & `pipedrive-wrapper-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.5/PKG-INFO` & `pipedrive-wrapper-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipedrive-wrapper
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python wrapper for the Pipedrive API
 Home-page: https://github.com/ppcantidio/pipedrive.py
 Author: Pedro Cantidio
 Author-email: ppcantidio@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pipedrive-wrapper-1.0.5/pipedrive/activity.py` & `pipedrive-wrapper-1.0.6/pipedrive/activity.py`

 * *Files 9% similar despite different names*

```diff
@@ -85,8 +85,17 @@
             "user_id": user_id,
             # "participants": participants,
             # "busy_flag": busy_flag,
             # "attendees": attendees,
             # "done": done,
         }
 
+        return self._client.post(url_context, payload)
+
+    def update_acitity(self, activity_id: int, done: bool = False):
+        url_context = f"/activities/{activity_id}"
+
+        payload = {}
+        if done is not None:
+            payload['done'] = int(done)
+
         return self._client._post(url_context, payload)
```

### Comparing `pipedrive-wrapper-1.0.5/pipedrive/client.py` & `pipedrive-wrapper-1.0.6/pipedrive/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,92 @@
 import requests
 
 from .activity import Activity
 from .deal import Deal
 from .deal_field import DealField
 from .exceptions import BadRequest, Forbidden, InternalServerError, NotFound, TooManyRequests, Unauthorized
 from .person import Person
+import logging
+from logging import Logger
 
 
 class Client:
-    def __init__(self, token: str) -> None:
+    def __init__(self, token: str, logger: Logger = logging) -> None:
+        self.extra_log = None
         self.base_url = "https://api.pipedrive.com/v1"
         self.token = token
         self.headers = {"Accept": "application/json"}
         self.activity = Activity(self)
         self.person = Person(self)
         self.deal = Deal(self)
         self.deal_field = DealField(self)
+        self.logger = logger
 
-    def _post(self, url_context: str, body: dict):
+    def post(self, url_context: str, body: dict):
         url_to_request = self.__generate_url_to_request(url_context)
 
+        self.extra_log = {'request_url': url_to_request, 'http_method': 'POST'}
+
         body = self.__check_values_of_dict(body)
 
         response = requests.post(
             url=url_to_request,
             headers=self.headers,
             json=body,
         )
 
+        extra_log_body_content = self.extra_log.copy()
+        extra_log_body_content['body'] = body
+        self.logger.debug('Body content at extras', extra=extra_log_body_content)
+
+        self.logger.info('Sending request', extra=self.extra_log)
+
         self.__raise_for_status(response)
 
         result = self.__parse_response(response)
 
         return result.get("data")
 
-    def _put(self, url_context: str, body: dict):
+    def put(self, url_context: str, body: dict):
         url_to_request = self.__generate_url_to_request(url_context)
 
+        self.extra_log = {'request_url': url_to_request, 'http_method': 'PUT'}
+
         body = self.__check_values_of_dict(body)
 
+        self.logger.info('Sending request', extra=self.extra_log)
+
+        extra_log_body_content = self.extra_log.copy()
+        extra_log_body_content['body'] = body
+        self.logger.debug('Body content at extras', extra=extra_log_body_content)
+
         response = requests.put(
             url=url_to_request,
             headers=self.headers,
             json=body,
         )
 
         self.__raise_for_status(response)
 
         result = self.__parse_response(response)
 
         return result.get("data")
 
-    def _get(self, url_context: str, params: dict = None):
+    def get(self, url_context: str, params: dict = None):
         url_to_request = self.__generate_url_to_request(url_context)
 
+        self.extra_log = {'request_url': url_to_request, 'http_method': 'GET'}
+
         if isinstance(params, dict):
             params = self.__check_values_of_dict(params)
 
+        self.extra_log['query_params'] = params
+
+        self.logger.info('Sending request', extra=self.extra_log)
+
         response = requests.get(
             url=url_to_request,
             headers=self.headers,
             params=params,
         )
 
         self.__raise_for_status(response)
@@ -77,18 +103,22 @@
         return response.json()
 
     def __check_values_of_dict(self, params: dict):
         return {key: value for key, value in params.items() if value is not None}
 
     def __raise_for_status(self, response: requests.Response):
         status_code = response.status_code
+        self.extra_log['http_status_code'] = status_code
 
         if 300 > status_code >= 200:
+            self.logger.info('Successful request', extra=self.extra_log)
             return
 
+        self.logger.error(f'Error when performing request, see extra for details', extra=self.extra_log)
+
         if status_code == 400:
             raise BadRequest()
 
         if status_code == 401:
             raise Unauthorized()
 
         if status_code == 403:
```

### Comparing `pipedrive-wrapper-1.0.5/pipedrive/deal.py` & `pipedrive-wrapper-1.0.6/pipedrive/deal.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             "lost_reason": lost_reason,
             "visible_to": visible_to,
             "add_time": add_time,
         }
 
         payload.update(personalized_fields)
 
-        result = self.client._post(url_context=url, body=payload)
+        result = self.client.post(url_context=url, body=payload)
 
         return result
 
     def update_deal(
         self,
         deal_id: int,
         title: str = None,
@@ -87,16 +87,14 @@
         expected_close_date: str = None,
         probability: int = None,
         lost_reason: str = None,
         visible_to: str = None,
         add_time: str = None,
     ):
         url_context = f"/deals/{deal_id}"
-        url_to_request = self.client._generate_url_to_request(url_context)
-        headers = self.client._generate_headers()
 
         payload = {
             "title": title,
             "value": value,
             "currency": currency,
             "user_id": user_id,
             "person_id": person_id,
@@ -111,15 +109,15 @@
             "add_time": add_time,
         }
 
         for key, value in payload:
             if value is None:
                 del payload[key]
 
-        result = self.client._put(url=url_to_request, headers=headers, body=payload)
+        result = self.client.put(url_context=url_context,  body=payload)
 
         return result
 
     def get_deal_by_id(self, deal_id: int):
         """
         Retrieve a deal by its ID.
 
@@ -131,15 +129,15 @@
 
         Raises:
             Exception: If there is an error while retrieving the deal.
 
         """
         url_context = f"/deals/{deal_id}"
 
-        return self.client._get(url_context)
+        return self.client.get(url_context)
 
     def search_deals(
         self,
         term: str,
         exact_match: bool = True,
         person_id: int = None,
         organization_id: int = None,
@@ -174,10 +172,17 @@
             "organization_id": organization_id,
             "status": status,
             "include_fields": include_fields,
             "start": start,
             "limit": limit,
         }
 
-        result = self.client._get(url_context=url, params=params)
+        result = self.client.get(url_context=url, params=params)
+
+        return result
+
+    def get_activities_associated_with_deal(self, deal_id):
+        url = f'/deals/{deal_id}/activities'
+
+        result = self.client.get(url_context=url)
 
         return result
```

### Comparing `pipedrive-wrapper-1.0.5/pipedrive/deal_field.py` & `pipedrive-wrapper-1.0.6/pipedrive/deal_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
         Raises:
             Exception: If there is an error while retrieving the deal.
 
         """
         url_context = f"/dealsFields/{deal_field_id}"
 
-        return self.client._get(url_context)
+        return self.client.get(url_context)
 
     def get_all_deal_fields(self):
         url_context = f"/dealFields"
 
-        return self.client._get(url_context)
+        return self.client.get(url_context)
 
     def get_deal_field_by_key(self, deal_field_key: str):
         all_deal_fields = self.get_all_deal_fields()
 
         for deal_field in all_deal_fields:
             if deal_field.get("key") == deal_field_key:
                 return deal_field
```

### Comparing `pipedrive-wrapper-1.0.5/pipedrive/exceptions.py` & `pipedrive-wrapper-1.0.6/pipedrive/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.5/pipedrive/person.py` & `pipedrive-wrapper-1.0.6/pipedrive/person.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             "phone": [{"value": phone}],
             "owner_id": owner_id,
             "org_id": org_id,
             "visible_to": visible_to,
             "marketing_status": marketing_status,
         }
 
-        return self.client._post(url_context, body)
+        return self.client.post(url_context, body)
 
     def search_person(
         self,
         term: str,
         fields: str = None,
         exact_match: bool = False,
         organization_id: int = None,
@@ -84,15 +84,15 @@
             "exact_match": exact_match,
             "organization_id": organization_id,
             "include_fields": include_fields,
             "start": start,
             "limit": limit,
         }
 
-        return self.client._get(url_context, params)
+        return self.client.get(url_context, params)
 
     def get_person_by_id(self, person_id: int):
         """
         Retrieve a person by their ID.
 
         Args:
             person_id (int): The ID of the person to retrieve.
@@ -102,15 +102,15 @@
 
         Raises:
             Exception: If there is an error while retrieving the person.
 
         """
         url_context = f"/persons/{person_id}"
 
-        return self.client._get(url_context)
+        return self.client.get(url_context)
 
     def update_person(
         self,
         person_id: int,
         name: str = None,
         owner_id: int = None,
         org_id: int = None,
@@ -160,8 +160,8 @@
             "email": email,
             "phone": phone,
             "visible_to": visible_to,
             "marketing_status": marketing_status,
             "add_time": add_time,
         }
 
-        return self.client._put(url_context, payload)
+        return self.client.put(url_context, payload)
```

### Comparing `pipedrive-wrapper-1.0.5/pipedrive/util.py` & `pipedrive-wrapper-1.0.6/pipedrive/util.py`

 * *Files identical despite different names*

### Comparing `pipedrive-wrapper-1.0.5/pipedrive_wrapper.egg-info/PKG-INFO` & `pipedrive-wrapper-1.0.6/pipedrive_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipedrive-wrapper
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python wrapper for the Pipedrive API
 Home-page: https://github.com/ppcantidio/pipedrive.py
 Author: Pedro Cantidio
 Author-email: ppcantidio@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pipedrive-wrapper-1.0.5/setup.py` & `pipedrive-wrapper-1.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="pipedrive-wrapper",
-    version="1.0.5",
+    version="1.0.6",
     author="Pedro Cantidio",
     author_email="ppcantidio@gmail.com",
     description="A Python wrapper for the Pipedrive API",
     long_description="A Python wrapper that simplifies interaction with the Pipedrive API",
     url="https://github.com/ppcantidio/pipedrive.py",
     packages=find_packages(exclude=["tests"]),
     classifiers=[
```

