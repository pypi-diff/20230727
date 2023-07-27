# Comparing `tmp/knockapi-0.5.2.tar.gz` & `tmp/knockapi-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knockapi-0.5.2.tar", last modified: Fri Feb 17 18:08:06 2023, max compression
+gzip compressed data, was "knockapi-0.5.6.tar", last modified: Thu Jul 27 20:37:22 2023, max compression
```

## Comparing `knockapi-0.5.2.tar` & `knockapi-0.5.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 18:08:06.157512 knockapi-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2023-02-17 18:07:57.000000 knockapi-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     3801 2023-02-17 18:08:06.157512 knockapi-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2869 2023-02-17 18:07:57.000000 knockapi-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 18:08:06.153512 knockapi-0.5.2/knockapi/
--rw-r--r--   0 runner    (1001) docker     (116)       67 2023-02-17 18:07:57.000000 knockapi-0.5.2/knockapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3414 2023-02-17 18:07:57.000000 knockapi-0.5.2/knockapi/client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 18:08:06.157512 knockapi-0.5.2/knockapi/resources/
--rw-r--r--   0 runner    (1001) docker     (116)      227 2023-02-17 18:07:57.000000 knockapi-0.5.2/knockapi/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      400 2023-02-17 18:07:57.000000 knockapi-0.5.2/knockapi/resources/bulk_operations.py
--rw-r--r--   0 runner    (1001) docker     (116)     2003 2023-02-17 18:07:57.000000 knockapi-0.5.2/knockapi/resources/messages.py
--rw-r--r--   0 runner    (1001) docker     (116)    12543 2023-02-17 18:07:57.000000 knockapi-0.5.2/knockapi/resources/objects.py
--rw-r--r--   0 runner    (1001) docker     (116)     3182 2023-02-17 18:07:57.000000 knockapi-0.5.2/knockapi/resources/preferences.py
--rw-r--r--   0 runner    (1001) docker     (116)       84 2023-02-17 18:07:57.000000 knockapi-0.5.2/knockapi/resources/service.py
--rw-r--r--   0 runner    (1001) docker     (116)     1386 2023-02-17 18:07:57.000000 knockapi-0.5.2/knockapi/resources/tenants.py
--rw-r--r--   0 runner    (1001) docker     (116)    12246 2023-02-17 18:07:57.000000 knockapi-0.5.2/knockapi/resources/users.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2023-02-17 18:07:57.000000 knockapi-0.5.2/knockapi/resources/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 18:08:06.153512 knockapi-0.5.2/knockapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3801 2023-02-17 18:08:06.000000 knockapi-0.5.2/knockapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      537 2023-02-17 18:08:06.000000 knockapi-0.5.2/knockapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-17 18:08:06.000000 knockapi-0.5.2/knockapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       29 2023-02-17 18:08:06.000000 knockapi-0.5.2/knockapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2023-02-17 18:08:06.000000 knockapi-0.5.2/knockapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-17 18:08:06.157512 knockapi-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1273 2023-02-17 18:07:57.000000 knockapi-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-17 18:08:06.157512 knockapi-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      892 2023-02-17 18:07:57.000000 knockapi-0.5.2/tests/test_tenants_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:37:22.559435 knockapi-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-27 20:37:12.000000 knockapi-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-27 20:37:22.559435 knockapi-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-27 20:37:12.000000 knockapi-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:37:22.555435 knockapi-0.5.6/knockapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 20:37:12.000000 knockapi-0.5.6/knockapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-27 20:37:12.000000 knockapi-0.5.6/knockapi/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:37:22.559435 knockapi-0.5.6/knockapi/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-27 20:37:12.000000 knockapi-0.5.6/knockapi/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-27 20:37:12.000000 knockapi-0.5.6/knockapi/resources/bulk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-27 20:37:12.000000 knockapi-0.5.6/knockapi/resources/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-07-27 20:37:12.000000 knockapi-0.5.6/knockapi/resources/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-27 20:37:12.000000 knockapi-0.5.6/knockapi/resources/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-27 20:37:12.000000 knockapi-0.5.6/knockapi/resources/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-27 20:37:12.000000 knockapi-0.5.6/knockapi/resources/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-07-27 20:37:12.000000 knockapi-0.5.6/knockapi/resources/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-27 20:37:12.000000 knockapi-0.5.6/knockapi/resources/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:37:22.555435 knockapi-0.5.6/knockapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-27 20:37:22.000000 knockapi-0.5.6/knockapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-27 20:37:22.000000 knockapi-0.5.6/knockapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:37:22.000000 knockapi-0.5.6/knockapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 20:37:22.000000 knockapi-0.5.6/knockapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 20:37:22.000000 knockapi-0.5.6/knockapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:37:22.559435 knockapi-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-27 20:37:12.000000 knockapi-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:37:22.559435 knockapi-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-27 20:37:12.000000 knockapi-0.5.6/tests/test_tenants_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-27 20:37:12.000000 knockapi-0.5.6/tests/test_workflows_class.py
```

### Comparing `knockapi-0.5.2/LICENSE` & `knockapi-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `knockapi-0.5.2/PKG-INFO` & `knockapi-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knockapi
-Version: 0.5.2
+Version: 0.5.6
 Summary: Client library for the Knock API
 Home-page: https://github.com/knocklabs/knock-python
 Author: Knock Labs, Inc.
 Author-email: support@knock.app
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `knockapi-0.5.2/README.md` & `knockapi-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `knockapi-0.5.2/knockapi/client.py` & `knockapi-0.5.6/knockapi/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import requests
 from json.decoder import JSONDecodeError
 
-__version__ = '0.5.2'
+__version__ = '0.5.6'
 
 
 class Connection(object):
     def __init__(self, api_key, host='https://api.knock.app'):
         self.api_key = api_key
         self.host = host
         self.client_version = __version__
         self.headers = {
             'Authorization': 'Bearer {}'.format(self.api_key),
             'User-Agent': 'Knock Python - {}'.format(self.client_version)
         }
 
-    def request(self, method, endpoint, payload=None):
+    def request(self, method, endpoint, payload=None, options={}):
         url = '{}/v1{}'.format(self.host, endpoint)
 
+        extra_headers = {}
+        if (method in ["post", "put"]) and options.get('idempotency_key') is not None:
+            extra_headers['Idempotency-Key'] = options.get('idempotency_key')
+
         r = requests.request(
             method,
             url,
             params=payload if method == 'get' else None,
             json=payload if method != 'get' else None,
-            headers=self.headers,
+            headers={**self.headers, **extra_headers}
         )
 
         # If we got a successful response, then attempt to deserialize as JSON
         if r.ok:
             try:
                 return r.json()
             except JSONDecodeError:
@@ -84,15 +88,16 @@
     def notify(
             self,
             key,
             recipients,
             data={},
             actor=None,
             cancellation_key=None,
-            tenant=None):
+            tenant=None,
+            options={}):
         """
         Triggers a workflow.
 
         Args:
             key (str): The key of the workflow to invoke.
 
             actor (str | dict[str, Any]): An optional reference for who/what performed the action. This can be A) a user
@@ -104,18 +109,23 @@
 
             data (dict): Any data to be passed to the notify call.
 
             tenant (str): An optional identifier for the tenant that the notifications belong to.
 
             cancellation_key (str): A key used to cancel this notify.
 
+            options (dict): An optional dictionary of options to pass to the request.
+            Can include:
+            - idempotency_key (str): An optional key that, if passed, will ensure that the same call is not made twice.
+
         Returns:
             dict: Response from Knock.
         """
         # Note: this is essentially a delegated method
         return self.workflows.trigger(
             key=key,
             recipients=recipients,
             data=data,
             actor=actor,
             cancellation_key=cancellation_key,
-            tenant=tenant)
+            tenant=tenant,
+            options=options)
```

### Comparing `knockapi-0.5.2/knockapi/resources/messages.py` & `knockapi-0.5.6/knockapi/resources/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import json
 from .service import Service
 
+
 class Messages(Service):
     def list(self, options=None):
         """
         Gets a paginated list of Message records
 
         Args:
             options (dict): An optional set of filtering options to pass to the query
 
         Returns:
             dict: a paginated list of Message records
         """
         endpoint = '/messages'
 
-        if options and options['trigger_data']:
+        if options and options.get('trigger_data'):
             options['trigger_data'] = json.dumps(options['trigger_data'])
 
         return self.client.request('get', endpoint, payload=options)
 
     def get(self, id):
         """
         Get a message by its id
@@ -53,15 +54,15 @@
             id: The message ID
 
         Returns:
             dict: paginated Activity response from Knock.
         """
         endpoint = '/messages/{}/activities'.format(id)
 
-        if options and options['trigger_data']:
+        if options and options.get('trigger_data'):
             options['trigger_data'] = json.dumps(options['trigger_data'])
 
         return self.client.request('get', endpoint, options)
 
     def get_events(self, id, options=None):
         """
         Get a message's events by its id
```

### Comparing `knockapi-0.5.2/knockapi/resources/objects.py` & `knockapi-0.5.6/knockapi/resources/objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,31 @@
 
         Returns:
             dict: A Knock Object
         """
         endpoint = '/objects/{}/{}'.format(collection, id)
         return self.client.request('get', endpoint)
 
+    def list(self, collection, options={}):
+        """
+        Returns objects in collection for the provided environment
+
+        Args:
+            collection (str): The collection the object belongs to
+            options (dict): An optional set of filtering options to pass to the query. These are:
+                - page_size: specify size of the page to be returned by the api. (max limit: 50)
+                - after:  after cursor for pagination
+                - before: before cursor for pagination
+
+        Returns:
+            dict: Paginated Knock Object response.
+        """
+        endpoint = '/objects/{}'.format(collection)
+        return self.client.request('get', endpoint, payload=options)
+
     # NOTE: This is `set_object` as `set` is a reserved keyword
     def set_object(self, collection, id, data={}):
         """
         Returns an object in a collection with the id given.
 
         Args:
             collection (str): The collection the object belongs to
@@ -148,20 +165,43 @@
             options (dict): An optional set of filtering options to pass to the query
 
         Returns:
             dict: Paginated Message response.
         """
         endpoint = '/objects/{}/{}/messages'.format(collection, id)
 
-        if options and options['trigger_data']:
+        if options and options.get('trigger_data'):
             options['trigger_data'] = json.dumps(options['trigger_data'])
 
         return self.client.request('get', endpoint, payload=options)
 
     ##
+    # Schedules
+    ##
+
+    def get_schedules(self, collection, id, options=None):
+        """
+        Get an objects's schedules
+
+        Args:
+            collection (str): The collection the object belongs to
+            id (str): The id of the object in the collection
+            options (dict): An optional set of filtering options to pass to the query. These are:
+                - page_size: specify size of the page to be returned by the api. (max limit: 50)
+                - after:  after cursor for pagination
+                - before: before cursor for pagination
+                - tenant: tenant_id to filter schedules with
+
+        Returns:
+            dict: Paginated Schedule response.
+        """
+        endpoint = '/objects/{}/{}/schedules'.format(collection, id)
+        return self.client.request('get', endpoint, payload=options)
+
+    ##
     # Preferences
     ##
 
     def get_all_preferences(self, collection, id):
         """
         Get an objects full set of preferences
 
@@ -384,7 +424,82 @@
         endpoint = '/objects/{}/{}/preferences/{}/categories/{}'.format(
             collection, id, preference_set_id, key)
 
         params = setting if isinstance(setting, dict) else {
             'subscribed': setting}
 
         return self.client.request('put', endpoint, payload=params)
+
+    ##
+    # Subscriptions
+    ##
+
+    def list_subscriptions(self, collection, id, options={}):
+        """
+        Returns subscriptions for an object
+
+        Args:
+            collection (str): The collection the object belongs to
+            id (str): The id of the object
+            options (dict): An optional set of filtering options to pass to the query. These are:
+                - page_size: specify size of the page to be returned by the api. (max limit: 50)
+                - after:  after cursor for pagination
+                - before: before cursor for pagination
+
+        Returns:
+            dict: Paginated Subscription response.
+        """
+        endpoint = '/objects/{}/{}/subscriptions'.format(collection, id)
+        return self.client.request('get', endpoint, payload=options)
+
+    def get_subscriptions(self, collection, id, options={}):
+        """
+        Returns subscriptions for an object as a recipient
+
+        Args:
+            collection (str): The collection the object belongs to
+            id (str): The id of the object
+            options (dict): An optional set of filtering options to pass to the query. These are:
+                - page_size: specify size of the page to be returned by the api. (max limit: 50)
+                - after:  after cursor for pagination
+                - before: before cursor for pagination
+
+        Returns:
+            dict: Paginated Subscription response.
+        """
+
+        options['mode'] = 'recipient'
+        endpoint = '/objects/{}/{}/subscriptions'.format(collection, id)
+        return self.client.request('get', endpoint, payload=options)
+
+    def add_subscriptions(self, collection, id, recipients, properties={}):
+        """
+        Creates or update subscription for recipients to Object
+
+        Args:
+            collection (str): The collection the object belongs to
+            id (str): The id of the object
+            recipients(list): List of recipients to be subscribed to object
+            properties (dict): Properties to be set on the subscription
+
+        Returns:
+            list: List of Subscription response.
+        """
+
+        endpoint = '/objects/{}/{}/subscriptions'.format(collection, id)
+        return self.client.request('post', endpoint, payload={'recipients': recipients, 'properties': properties})
+
+    def delete_subscriptions(self, collection, id, recipients):
+        """
+        Delete subscription to object for recipients
+
+        Args:
+            collection (str): The collection the object belongs to
+            id (str): The id of the object
+            recipients(list): List of recipients for subscriptions to be deleted
+
+        Returns:
+            list: List of Subscription response.
+        """
+
+        endpoint = '/objects/{}/{}/subscriptions'.format(collection, id)
+        return self.client.request('delete', endpoint, payload={'recipients': recipients})
```

### Comparing `knockapi-0.5.2/knockapi/resources/preferences.py` & `knockapi-0.5.6/knockapi/resources/preferences.py`

 * *Files identical despite different names*

### Comparing `knockapi-0.5.2/knockapi/resources/tenants.py` & `knockapi-0.5.6/knockapi/resources/tenants.py`

 * *Files identical despite different names*

### Comparing `knockapi-0.5.2/knockapi/resources/users.py` & `knockapi-0.5.6/knockapi/resources/users.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,30 @@
 
         Returns:
             dict: User response from Knock.
         """
         endpoint = '/users/{}'.format(id)
         return self.client.request('get', endpoint)
 
+    def list(self, options={}):
+        """
+        List users for the environment
+
+        Args:
+            options (dict): An optional set of filtering options to pass to the query. These are:
+                - page_size: specify size of the page to be returned by the api. (max limit: 50)
+                - after:  after cursor for pagination
+                - before: before cursor for pagination
+
+        Returns:
+            dict: Paginated User response.
+        """
+        endpoint = '/users'
+        return self.client.request('get', endpoint, payload=options)
+
     def identify(self, id, data={}):
         """
         Identify a user, upserting them
 
         Args:
             id (str): The user ID
             data (dict): Other properties to put on the user
@@ -89,15 +105,15 @@
             options (dict): An optional set of feed options to pass to the query
 
         Returns
             dict: A Knock feed response
         """
         endpoint = '/users/{}/feeds/{}'.format(user_id, channel_id)
 
-        if options and options['trigger_data']:
+        if options and options.get('trigger_data'):
             options['trigger_data'] = json.dumps(options['trigger_data'])
 
         return self.client.request('get', endpoint, payload=options)
 
     def merge(self, user_id, from_user_id):
         """
         Merges the user specified with `from_user_id` into the user specified with `user_id`.
@@ -399,7 +415,50 @@
             options (dict): An optional set of filtering options to pass to the query
 
         Returns:
             dict: Paginated Message response.
         """
         endpoint = '/users/{}/messages'.format(id)
         return self.client.request('get', endpoint, payload=options)
+
+    ##
+    # Schedules
+    ##
+
+    def get_schedules(self, id, options=None):
+        """
+        Get user's schedules
+
+        Args:
+            id (str): The user ID
+            options (dict): An optional set of filtering options to pass to the query. These are:
+                - page_size: specify size of the page to be returned by the api. (max limit: 50)
+                - after:  after cursor for pagination
+                - before: before cursor for pagination
+                - tenant: tenant_id to filter schedules with
+
+        Returns:
+            dict: Paginated Schedule response.
+        """
+        endpoint = '/users/{}/schedules'.format(id)
+        return self.client.request('get', endpoint, payload=options)
+
+    ##
+    # Subscriptions
+    ##
+
+    def get_subscriptions(self, id, options=None):
+        """
+        Get user's subscriptions
+
+        Args:
+            id (str): The user ID
+            options (dict): An optional set of filtering options to pass to the query. These are:
+                - page_size: specify size of the page to be returned by the api. (max limit: 50)
+                - after:  after cursor for pagination
+                - before: before cursor for pagination
+
+        Returns:
+            dict: Paginated Subscription response.
+        """
+        endpoint = '/users/{}/subscriptions'.format(id)
+        return self.client.request('get', endpoint, payload=options)
```

### Comparing `knockapi-0.5.2/knockapi.egg-info/PKG-INFO` & `knockapi-0.5.6/knockapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knockapi
-Version: 0.5.2
+Version: 0.5.6
 Summary: Client library for the Knock API
 Home-page: https://github.com/knocklabs/knock-python
 Author: Knock Labs, Inc.
 Author-email: support@knock.app
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `knockapi-0.5.2/knockapi.egg-info/SOURCES.txt` & `knockapi-0.5.6/knockapi.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 knockapi/resources/messages.py
 knockapi/resources/objects.py
 knockapi/resources/preferences.py
 knockapi/resources/service.py
 knockapi/resources/tenants.py
 knockapi/resources/users.py
 knockapi/resources/workflows.py
-tests/test_tenants_class.py
+tests/test_tenants_class.py
+tests/test_workflows_class.py
```

### Comparing `knockapi-0.5.2/setup.py` & `knockapi-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-version = '0.5.2'
+version = '0.5.6'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='knockapi',
     version=version,
```

### Comparing `knockapi-0.5.2/tests/test_tenants_class.py` & `knockapi-0.5.6/tests/test_tenants_class.py`

 * *Files identical despite different names*

