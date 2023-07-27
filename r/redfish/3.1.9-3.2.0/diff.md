# Comparing `tmp/redfish-3.1.9.tar.gz` & `tmp/redfish-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish-3.1.9.tar", last modified: Fri Jan 13 20:48:06 2023, max compression
+gzip compressed data, was "redfish-3.2.0.tar", last modified: Thu Jul 27 14:57:56 2023, max compression
```

## Comparing `redfish-3.1.9.tar` & `redfish-3.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:48:06.328169 redfish-3.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-01-13 20:47:55.000000 redfish-3.1.9/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-01-13 20:47:55.000000 redfish-3.1.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-01-13 20:48:06.328169 redfish-3.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-01-13 20:47:55.000000 redfish-3.1.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 20:48:06.328169 redfish-3.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-01-13 20:48:03.000000 redfish-3.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:48:06.324169 redfish-3.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:48:06.328169 redfish-3.1.9/src/redfish/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-01-13 20:48:03.000000 redfish-3.1.9/src/redfish/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:48:06.328169 redfish-3.1.9/src/redfish/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-01-13 20:47:55.000000 redfish-3.1.9/src/redfish/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-01-13 20:47:55.000000 redfish-3.1.9/src/redfish/discovery/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:48:06.328169 redfish-3.1.9/src/redfish/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-13 20:47:55.000000 redfish-3.1.9/src/redfish/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40917 2023-01-13 20:47:55.000000 redfish-3.1.9/src/redfish/rest/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:48:06.328169 redfish-3.1.9/src/redfish/ris/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-13 20:47:55.000000 redfish-3.1.9/src/redfish/ris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-01-13 20:47:55.000000 redfish-3.1.9/src/redfish/ris/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21139 2023-01-13 20:47:55.000000 redfish-3.1.9/src/redfish/ris/ris.py
--rw-r--r--   0 runner    (1001) docker     (123)    67530 2023-01-13 20:47:55.000000 redfish-3.1.9/src/redfish/ris/rmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-01-13 20:47:55.000000 redfish-3.1.9/src/redfish/ris/rmc_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-01-13 20:47:55.000000 redfish-3.1.9/src/redfish/ris/sharedtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:48:06.328169 redfish-3.1.9/src/redfish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-01-13 20:48:06.000000 redfish-3.1.9/src/redfish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-01-13 20:48:06.000000 redfish-3.1.9/src/redfish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 20:48:06.000000 redfish-3.1.9/src/redfish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-13 20:48:06.000000 redfish-3.1.9/src/redfish.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-13 20:48:06.000000 redfish-3.1.9/src/redfish.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.884111 redfish-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-27 14:57:38.000000 redfish-3.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-27 14:57:38.000000 redfish-3.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-07-27 14:57:56.884111 redfish-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-07-27 14:57:38.000000 redfish-3.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:57:56.884111 redfish-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-27 14:57:49.000000 redfish-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.880110 redfish-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.880110 redfish-3.2.0/src/redfish/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-27 14:57:49.000000 redfish-3.2.0/src/redfish/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.880110 redfish-3.2.0/src/redfish/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/discovery/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.880110 redfish-3.2.0/src/redfish/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42047 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/rest/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.884111 redfish-3.2.0/src/redfish/ris/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/ris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/ris/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21137 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/ris/ris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67528 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/ris/rmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23633 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/ris/rmc_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/ris/sharedtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.880110 redfish-3.2.0/src/redfish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-07-27 14:57:56.000000 redfish-3.2.0/src/redfish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-27 14:57:56.000000 redfish-3.2.0/src/redfish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:57:56.000000 redfish-3.2.0/src/redfish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-27 14:57:56.000000 redfish-3.2.0/src/redfish.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 14:57:56.000000 redfish-3.2.0/src/redfish.egg-info/top_level.txt
```

### Comparing `redfish-3.1.9/AUTHORS.md` & `redfish-3.2.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `redfish-3.1.9/LICENSE.md` & `redfish-3.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish-3.1.9/PKG-INFO` & `redfish-3.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish
-Version: 3.1.9
+Version: 3.2.0
 Summary: Redfish Python Library
 Home-page: https://github.com/DMTF/python-redfish-library
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -18,15 +18,15 @@
 ======================
 
 .. image:: https://img.shields.io/pypi/v/redfish.svg?maxAge=2592000
     :target: https://pypi.python.org/pypi/redfish
 .. image:: https://img.shields.io/github/release/DMTF/python-redfish-library.svg?maxAge=2592000
     :target: https://github.com/DMTF/python-redfish-library/releases
 .. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-    :target: https://raw.githubusercontent.com/DMTF/python-redfish-library/master/LICENSE
+    :target: https://raw.githubusercontent.com/DMTF/python-redfish-library/main/LICENSE
 .. image:: https://img.shields.io/pypi/pyversions/redfish.svg?maxAge=2592000
     :target: https://pypi.python.org/pypi/redfish
 
 .. contents:: :depth: 1
 
 Description
 -----------
@@ -86,15 +86,15 @@
 * ``default_prefix``: The path to the Redfish service root.  This is only used for initial connection and authentication with the service.  The default value is ``/redfish/v1/``.
 * ``sessionkey``: The session key to use with subsequent requests.  This can be used to bypass the login step.  The default value is ``None``.
 * ``cafile``: The file path to the CA certificate that issued the Redfish service's certificate.  The default value is ``None``.
 * ``timeout``: The number of seconds to wait for a response before closing the connection.  The default value is ``None``.
 * ``max_retry``: The number of retries to perform an operation before giving up.  The default value is ``10``.
 * ``proxies``: A dictionary containing protocol to proxy URL mappings.  The default value is ``None``.  See `Using proxies`_.
 
-To crete a Redfish object, call the ``redfish_client`` method:
+To create a Redfish object, call the ``redfish_client`` method:
 
 .. code-block:: python
 
     REDFISH_OBJ = redfish.redfish_client(base_url=login_host, username=login_account, \
                           password=login_password, default_prefix='/redfish/v1/')
 
 Login to the service
@@ -109,42 +109,80 @@
 
     REDFISH_OBJ.login(auth="session")
 
 Perform a GET operation
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 A simple GET operation can be performed to obtain the data present in any valid path.
-An example of GET operation on the path "/redfish/v1/systems/1" is shown below:
+An example of GET operation on the path "/redfish/v1/Systems/1" is shown below:
 
 .. code-block:: python
 
-    response = REDFISH_OBJ.get("/redfish/v1/systems/1", None)
+    response = REDFISH_OBJ.get("/redfish/v1/Systems/1")
 
 Perform a POST operation
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 A POST operation can be performed to create a resource or perform an action.
-An example of a POST operation on the path "/redfish/v1/systems/1/Actions/ComputerSystem.Reset" is shown below:
+An example of a POST operation on the path "/redfish/v1/Systems/1/Actions/ComputerSystem.Reset" is shown below:
 
 .. code-block:: python
 
     body = {"ResetType": "GracefulShutdown"}
-    response = REDFISH_OBJ.post("/redfish/v1/systems/1/Actions/ComputerSystem.Reset", body=body)
+    response = REDFISH_OBJ.post("/redfish/v1/Systems/1/Actions/ComputerSystem.Reset", body=body)
+
+Notes about HTTP methods and arguments
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The previous sections showed example GET and POST requests.  The following is a list of the different methods supported:
+
+* ``get``: Performs an HTTP GET operation to retrieve a resource from a URI.
+* ``head``: Performs an HTTP HEAD operation to retrieve response headers from a URI, but no body.
+* ``post``: Performs an HTTP POST operation to perform an action or create a new resource.
+* ``put``: Performs an HTTP PUT operation to replace an existing resource.
+* ``patch``: Performs an HTTP PATCH operation to update an existing resource.
+* ``delete``: Performs an HTTP DELETE operation to remove a resource.
+
+Each of the previous methods allows for the following arguments:
+
+* ``path``: **Required**.  String.  The URI in which to invoke the operation.
+
+  - Example: ``"/redfish/v1/Systems/1"``
+
+* ``args``: Dictionary.  Query parameters to supply with the request.
+
+  - The key-value pairs in the dictionary are the query parameter name and the query parameter value to supply.
+  - Example: ``{"$select": "Reading,Status"}``
+
+* ``body``: Dictionary, List, Bytes, or String.  The request body to provide with the request.
+
+  - Not supported for ``get``, ``head``, or ``delete`` methods.
+  - The data type supplied will dictate the encoding.
+  - A dictionary is the most common usage, which results in a JSON body.
+  - Example: ``{"ResetType": "GracefulShutdown"}``
+  - A list is used to supply multipart forms, which is useful for multipart HTTP push updates.
+  - Bytes is used to supply an octet stream.
+  - A string is used to supply an unstructed body, which may be used in some OEM cases.
+
+* ``headers``: Dictionary.  Additional HTTP headers to supply with the request.
+
+  - The key-value pairs in the dictionary are the HTTP header name and the HTTP header value to supply.
+  - Example: ``{"If-Match": etag_value}``
 
 Working with tasks
 ~~~~~~~~~~~~~~~~~~
 
-A POST and PATCH operations may result in a task, describing an operation with a duration greater than the span of a single request.
+POST, PATCH, PUT, and DELETE operations may result in a task, describing an operation with a duration greater than the span of a single request.
 The action message object that ``is_processing`` will return a task that can be accessed reviewed when polled with monitor.
 An example of a POST operation with a possible task is shown below.
 
 .. code-block:: python
 
     body = {"ResetType": "GracefulShutdown"}
-    response = REDFISH_OBJ.post("/redfish/v1/systems/1/Actions/ComputerSystem.Reset", body=body)
+    response = REDFISH_OBJ.post("/redfish/v1/Systems/1/Actions/ComputerSystem.Reset", body=body)
     if(response.is_processing):
         task = response.monitor(context)
 
         while(task.is_processing):
             retry_time = task.retry_after
             task_status = task.dict['TaskState']
             time.sleep(retry_time if retry_time else 5)
@@ -218,8 +256,8 @@
 5. Click "Run workflow"
 
 Copyright and License
 ---------------------
 
 Copyright Notice:
 Copyright 2016-2022 DMTF. All rights reserved.
-License: BSD 3-Clause License. For full text see link: `https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md <https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md>`_
+License: BSD 3-Clause License. For full text see link: `https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md <https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md>`_
```

### Comparing `redfish-3.1.9/README.rst` & `redfish-3.2.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ======================
 
 .. image:: https://img.shields.io/pypi/v/redfish.svg?maxAge=2592000
     :target: https://pypi.python.org/pypi/redfish
 .. image:: https://img.shields.io/github/release/DMTF/python-redfish-library.svg?maxAge=2592000
     :target: https://github.com/DMTF/python-redfish-library/releases
 .. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-    :target: https://raw.githubusercontent.com/DMTF/python-redfish-library/master/LICENSE
+    :target: https://raw.githubusercontent.com/DMTF/python-redfish-library/main/LICENSE
 .. image:: https://img.shields.io/pypi/pyversions/redfish.svg?maxAge=2592000
     :target: https://pypi.python.org/pypi/redfish
 
 .. contents:: :depth: 1
 
 Description
 -----------
@@ -70,15 +70,15 @@
 * ``default_prefix``: The path to the Redfish service root.  This is only used for initial connection and authentication with the service.  The default value is ``/redfish/v1/``.
 * ``sessionkey``: The session key to use with subsequent requests.  This can be used to bypass the login step.  The default value is ``None``.
 * ``cafile``: The file path to the CA certificate that issued the Redfish service's certificate.  The default value is ``None``.
 * ``timeout``: The number of seconds to wait for a response before closing the connection.  The default value is ``None``.
 * ``max_retry``: The number of retries to perform an operation before giving up.  The default value is ``10``.
 * ``proxies``: A dictionary containing protocol to proxy URL mappings.  The default value is ``None``.  See `Using proxies`_.
 
-To crete a Redfish object, call the ``redfish_client`` method:
+To create a Redfish object, call the ``redfish_client`` method:
 
 .. code-block:: python
 
     REDFISH_OBJ = redfish.redfish_client(base_url=login_host, username=login_account, \
                           password=login_password, default_prefix='/redfish/v1/')
 
 Login to the service
@@ -93,42 +93,80 @@
 
     REDFISH_OBJ.login(auth="session")
 
 Perform a GET operation
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 A simple GET operation can be performed to obtain the data present in any valid path.
-An example of GET operation on the path "/redfish/v1/systems/1" is shown below:
+An example of GET operation on the path "/redfish/v1/Systems/1" is shown below:
 
 .. code-block:: python
 
-    response = REDFISH_OBJ.get("/redfish/v1/systems/1", None)
+    response = REDFISH_OBJ.get("/redfish/v1/Systems/1")
 
 Perform a POST operation
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 A POST operation can be performed to create a resource or perform an action.
-An example of a POST operation on the path "/redfish/v1/systems/1/Actions/ComputerSystem.Reset" is shown below:
+An example of a POST operation on the path "/redfish/v1/Systems/1/Actions/ComputerSystem.Reset" is shown below:
 
 .. code-block:: python
 
     body = {"ResetType": "GracefulShutdown"}
-    response = REDFISH_OBJ.post("/redfish/v1/systems/1/Actions/ComputerSystem.Reset", body=body)
+    response = REDFISH_OBJ.post("/redfish/v1/Systems/1/Actions/ComputerSystem.Reset", body=body)
+
+Notes about HTTP methods and arguments
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The previous sections showed example GET and POST requests.  The following is a list of the different methods supported:
+
+* ``get``: Performs an HTTP GET operation to retrieve a resource from a URI.
+* ``head``: Performs an HTTP HEAD operation to retrieve response headers from a URI, but no body.
+* ``post``: Performs an HTTP POST operation to perform an action or create a new resource.
+* ``put``: Performs an HTTP PUT operation to replace an existing resource.
+* ``patch``: Performs an HTTP PATCH operation to update an existing resource.
+* ``delete``: Performs an HTTP DELETE operation to remove a resource.
+
+Each of the previous methods allows for the following arguments:
+
+* ``path``: **Required**.  String.  The URI in which to invoke the operation.
+
+  - Example: ``"/redfish/v1/Systems/1"``
+
+* ``args``: Dictionary.  Query parameters to supply with the request.
+
+  - The key-value pairs in the dictionary are the query parameter name and the query parameter value to supply.
+  - Example: ``{"$select": "Reading,Status"}``
+
+* ``body``: Dictionary, List, Bytes, or String.  The request body to provide with the request.
+
+  - Not supported for ``get``, ``head``, or ``delete`` methods.
+  - The data type supplied will dictate the encoding.
+  - A dictionary is the most common usage, which results in a JSON body.
+  - Example: ``{"ResetType": "GracefulShutdown"}``
+  - A list is used to supply multipart forms, which is useful for multipart HTTP push updates.
+  - Bytes is used to supply an octet stream.
+  - A string is used to supply an unstructed body, which may be used in some OEM cases.
+
+* ``headers``: Dictionary.  Additional HTTP headers to supply with the request.
+
+  - The key-value pairs in the dictionary are the HTTP header name and the HTTP header value to supply.
+  - Example: ``{"If-Match": etag_value}``
 
 Working with tasks
 ~~~~~~~~~~~~~~~~~~
 
-A POST and PATCH operations may result in a task, describing an operation with a duration greater than the span of a single request.
+POST, PATCH, PUT, and DELETE operations may result in a task, describing an operation with a duration greater than the span of a single request.
 The action message object that ``is_processing`` will return a task that can be accessed reviewed when polled with monitor.
 An example of a POST operation with a possible task is shown below.
 
 .. code-block:: python
 
     body = {"ResetType": "GracefulShutdown"}
-    response = REDFISH_OBJ.post("/redfish/v1/systems/1/Actions/ComputerSystem.Reset", body=body)
+    response = REDFISH_OBJ.post("/redfish/v1/Systems/1/Actions/ComputerSystem.Reset", body=body)
     if(response.is_processing):
         task = response.monitor(context)
 
         while(task.is_processing):
             retry_time = task.retry_after
             task_status = task.dict['TaskState']
             time.sleep(retry_time if retry_time else 5)
@@ -202,8 +240,8 @@
 5. Click "Run workflow"
 
 Copyright and License
 ---------------------
 
 Copyright Notice:
 Copyright 2016-2022 DMTF. All rights reserved.
-License: BSD 3-Clause License. For full text see link: `https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md <https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md>`_
+License: BSD 3-Clause License. For full text see link: `https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md <https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md>`_
```

### Comparing `redfish-3.1.9/setup.py` & `redfish-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright Notice:
 # Copyright 2016-2021 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md
+# https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md
 
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='redfish',
-      version='3.1.9',
+      version='3.2.0',
       description='Redfish Python Library',
       long_description=long_description,
       long_description_content_type='text/x-rst',
       author = 'DMTF, https://www.dmtf.org/standards/feedback',
       license='BSD 3-clause "New" or "Revised License"',
       classifiers=[
           'Development Status :: 5 - Production/Stable',
```

### Comparing `redfish-3.1.9/src/redfish/__init__.py` & `redfish-3.2.0/src/redfish/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright Notice:
 # Copyright 2016-2021 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md
+# https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md
 
 """ Redfish restful library """
 
 __all__ = ['rest', 'ris', 'discovery']
-__version__ = "3.1.9"
+__version__ = "3.2.0"
 
 from redfish.rest.v1 import redfish_client
 from redfish.rest.v1 import AuthMethod
 from redfish.discovery.discovery import discover_ssdp
 import logging
 
 def redfish_logger(file_name, log_format, log_level=logging.ERROR):
```

### Comparing `redfish-3.1.9/src/redfish/discovery/discovery.py` & `redfish-3.2.0/src/redfish/discovery/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2016-2021 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md
+# https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md
 
 # -*- coding: utf-8 -*-
 """Discovers Redfish services"""
 
 import http.client
 import re
 import socket
@@ -78,15 +78,15 @@
 
     # Initialize the multicast data
     msearch_str = (
         "M-SEARCH * HTTP/1.1\r\n"
         "Host: {}:{}\r\n"
         'Man: "ssdp:discover"\r\n'
         "ST: urn:dmtf-org:service:redfish-rest:1\r\n"
-        "MX: {}\r\n"
+        "MX: {}\r\n\r\n"
     ).format(mcast_ip, port, response_time)
     socket.setdefaulttimeout(response_time + 2)
 
     # Set up the socket and send the request
     sock = socket.socket(af_type, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
     sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
     sock.setsockopt(socket.IPPROTO_IP, socket.IP_MULTICAST_TTL, ttl)
@@ -95,15 +95,15 @@
     if iface:
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_BINDTODEVICE, str(iface+"\0").encode("utf-8"))
     sock.sendto(bytearray(msearch_str, "utf-8"), mcast_connection)
 
     # On the same socket, wait for responses
     discovered_services = {}
     pattern = re.compile(
-        "^uuid:([a-f0-9\-]*)::urn:dmtf-org:service:redfish-rest:1(:\d)?$") # noqa
+        "^uuid:([a-f0-9\-]*)::urn:dmtf-org:service:redfish-rest:1(:\d+)?$") # noqa
     while True:
         try:
             response = http.client.HTTPResponse(FakeSocket(sock.recv(1024)))
             response.begin()
             uuid_search = pattern.search(response.getheader("USN").lower())
             if uuid_search:
                 discovered_services[uuid_search.group(1)] = response.getheader(
```

### Comparing `redfish-3.1.9/src/redfish/rest/v1.py` & `redfish-3.2.0/src/redfish/rest/v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2016-2021 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md
+# https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md
 
 # -*- coding: utf-8 -*-
 """Helper module for working with REST technology."""
 
 #---------Imports---------
 
 import sys
@@ -606,106 +606,106 @@
 
         self.root = RisObject.parse(root_data)
         self.root_resp = resp
 
     def get(self, path, args=None, headers=None):
         """Perform a GET request
 
-        :param path: the URL path.
-        :type path: str.
-        :param args: the arguments to get.
-        :type args: dict.
-        :param headers: dict of headers to be appended.
-        :type headers: dict.
+        :param path: The URI to access
+        :type path: str
+        :param args: The query parameters to provide with the request
+        :type args: dict, optional
+        :param headers: Additional HTTP headers to provide in the request
+        :type headers: dict, optional
         :returns: returns a rest request with method 'Get'
 
         """
         try:
             return self._rest_request(path, method='GET', args=args,
                                                                 headers=headers)
         except ValueError:
             str = "Service responded with invalid JSON at URI {}".format(path)
             LOGGER.error(str)
             raise JsonDecodingError(str) from None
 
     def head(self, path, args=None, headers=None):
         """Perform a HEAD request
 
-        :param path: the URL path.
-        :type path: str.
-        :param args: the arguments to get.
-        :type args: dict.
-        :param headers: dict of headers to be appended.
-        :type headers: dict.
+        :param path: The URI to access
+        :type path: str
+        :param args: The query parameters to provide with the request
+        :type args: dict, optional
+        :param headers: Additional HTTP headers to provide in the request
+        :type headers: dict, optional
         :returns: returns a rest request with method 'Head'
 
         """
         return self._rest_request(path, method='HEAD', args=args,
                                                                 headers=headers)
 
     def post(self, path, args=None, body=None, headers=None):
         """Perform a POST request
 
-        :param path: the URL path.
-        :type path: str.
-        :param args: the arguments to post.
-        :type args: dict.
-        :param body: the body to the sent.
-        :type body: str.
-        :param headers: dict of headers to be appended.
-        :type headers: dict.
+        :param path: The URI to access
+        :type path: str
+        :param args: The query parameters to provide with the request
+        :type args: dict, optional
+        :param body: The request body to provide; use a dict for a JSON body, list for multipart forms, bytes for an octet stream, or str for an unstructured request
+        :type body: dict or list or bytes or str, optional
+        :param headers: Additional HTTP headers to provide in the request
+        :type headers: dict, optional
         :returns: returns a rest request with method 'Post'
 
         """
         return self._rest_request(path, method='POST', args=args, body=body,
                                                                 headers=headers)
 
     def put(self, path, args=None, body=None, headers=None):
         """Perform a PUT request
 
-        :param path: the URL path.
-        :type path: str.
-        :param args: the arguments to put.
-        :type args: dict.
-        :param body: the body to the sent.
-        :type body: str.
-        :param headers: dict of headers to be appended.
-        :type headers: dict.
+        :param path: The URI to access
+        :type path: str
+        :param args: The query parameters to provide with the request
+        :type args: dict, optional
+        :param body: The request body to provide; use a dict for a JSON body, list for multipart forms, bytes for an octet stream, or str for an unstructured request
+        :type body: dict or list or bytes or str, optional
+        :param headers: Additional HTTP headers to provide in the request
+        :type headers: dict, optional
         :returns: returns a rest request with method 'Put'
 
         """
         return self._rest_request(path, method='PUT', args=args, body=body,
                                                                 headers=headers)
 
     def patch(self, path, args=None, body=None, headers=None):
-        """Perform a PUT request
+        """Perform a PATCH request
 
-        :param path: the URL path.
-        :type path: str.
-        :param args: the arguments to patch.
-        :type args: dict.
-        :param body: the body to the sent.
-        :type body: str.
-        :param headers: dict of headers to be appended.
-        :type headers: dict.
+        :param path: The URI to access
+        :type path: str
+        :param args: The query parameters to provide with the request
+        :type args: dict, optional
+        :param body: The request body to provide; use a dict for a JSON body, list for multipart forms, bytes for an octet stream, or str for an unstructured request
+        :type body: dict or list or bytes or str, optional
+        :param headers: Additional HTTP headers to provide in the request
+        :type headers: dict, optional
         :returns: returns a rest request with method 'Patch'
 
         """
         return self._rest_request(path, method='PATCH', args=args, body=body,
                                                                 headers=headers)
 
     def delete(self, path, args=None, headers=None):
         """Perform a DELETE request
 
-        :param path: the URL path.
-        :type path: str.
-        :param args: the arguments to delete.
-        :type args: dict.
-        :param headers: dict of headers to be appended.
-        :type headers: dict.
+        :param path: The URI to access
+        :type path: str
+        :param args: The query parameters to provide with the request
+        :type args: dict, optional
+        :param headers: Additional HTTP headers to provide in the request
+        :type headers: dict, optional
         :returns: returns a rest request with method 'Delete'
 
         """
         return self._rest_request(path, method='DELETE', args=args,
                                                                 headers=headers)
 
     def _get_req_headers(self, headers=None):
@@ -729,26 +729,26 @@
 
         return headers
 
     def _rest_request(self, path, method='GET', args=None, body=None,
                       headers=None, allow_redirects=True):
         """Rest request main function
 
-        :param path: path within tree
+        :param path: The URI to access
         :type path: str
-        :param method: method to be implemented
-        :type method: str
-        :param args: the arguments for method
-        :type args: dict
-        :param body: body payload for the rest call
-        :type body: dict
-        :param headers: provide additional headers
-        :type headers: dict
-        :param allow_redirects: controls whether redirects are followed
-        :type allow_redirects: bool
+        :param method: The HTTP method to invoke on the URI; GET if not provided
+        :type method: str, optional
+        :param args: The query parameters to provide with the request
+        :type args: dict, optional
+        :param body: The request body to provide; use a dict for a JSON body, list for multipart forms, bytes for an octet stream, or str for an unstructured request
+        :type body: dict or list or bytes or str, optional
+        :param headers: Additional HTTP headers to provide in the request
+        :type headers: dict, optional
+        :param allow_redirects: Controls whether redirects are followed
+        :type allow_redirects: bool, optional
         :returns: returns a RestResponse object
 
         """
         headers = self._get_req_headers(headers)
         reqpath = path.replace('//', '/')
 
         if body is not None:
```

### Comparing `redfish-3.1.9/src/redfish/ris/__init__.py` & `redfish-3.2.0/src/redfish/ris/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2016-2021 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md
+# https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md
 
 # -*- coding: utf-8 -*-
 """
 RIS implementation
 """
 
 from .sharedtypes import (
```

### Comparing `redfish-3.1.9/src/redfish/ris/config.py` & `redfish-3.2.0/src/redfish/ris/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2016-2021 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md
+# https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md
 
 # -*- coding: utf-8 -*-
 """Module for working with global configuration options."""
 
 #---------Imports---------
 
 import os
```

### Comparing `redfish-3.1.9/src/redfish/ris/ris.py` & `redfish-3.2.0/src/redfish/ris/ris.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2016-2021 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md
+# https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md
 
 # -*- coding: utf-8 -*-
 """RIS implementation"""
 
 # ---------Imports---------
 
 import abc
```

### Comparing `redfish-3.1.9/src/redfish/ris/rmc.py` & `redfish-3.2.0/src/redfish/ris/rmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2016-2021 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md
+# https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md
 
 # -*- coding: utf-8 -*-
 """RMC implementation """
 
 #---------Imports---------
 import os
 import re
```

### Comparing `redfish-3.1.9/src/redfish/ris/rmc_helper.py` & `redfish-3.2.0/src/redfish/ris/rmc_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2016-2021 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md
+# https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md
 
 # -*- coding: utf-8 -*-
 """RMC helper implementation"""
 
 #---------Imports---------
 
 import os
```

### Comparing `redfish-3.1.9/src/redfish/ris/sharedtypes.py` & `redfish-3.2.0/src/redfish/ris/sharedtypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright Notice:
 # Copyright 2016-2021 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
-# https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md
+# https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md
 
 # -*- coding: utf-8 -*-
 """ Shared types used in this module """
 
 #---------Imports---------
 
 import logging
```

### Comparing `redfish-3.1.9/src/redfish.egg-info/PKG-INFO` & `redfish-3.2.0/src/redfish.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish
-Version: 3.1.9
+Version: 3.2.0
 Summary: Redfish Python Library
 Home-page: https://github.com/DMTF/python-redfish-library
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -18,15 +18,15 @@
 ======================
 
 .. image:: https://img.shields.io/pypi/v/redfish.svg?maxAge=2592000
     :target: https://pypi.python.org/pypi/redfish
 .. image:: https://img.shields.io/github/release/DMTF/python-redfish-library.svg?maxAge=2592000
     :target: https://github.com/DMTF/python-redfish-library/releases
 .. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-    :target: https://raw.githubusercontent.com/DMTF/python-redfish-library/master/LICENSE
+    :target: https://raw.githubusercontent.com/DMTF/python-redfish-library/main/LICENSE
 .. image:: https://img.shields.io/pypi/pyversions/redfish.svg?maxAge=2592000
     :target: https://pypi.python.org/pypi/redfish
 
 .. contents:: :depth: 1
 
 Description
 -----------
@@ -86,15 +86,15 @@
 * ``default_prefix``: The path to the Redfish service root.  This is only used for initial connection and authentication with the service.  The default value is ``/redfish/v1/``.
 * ``sessionkey``: The session key to use with subsequent requests.  This can be used to bypass the login step.  The default value is ``None``.
 * ``cafile``: The file path to the CA certificate that issued the Redfish service's certificate.  The default value is ``None``.
 * ``timeout``: The number of seconds to wait for a response before closing the connection.  The default value is ``None``.
 * ``max_retry``: The number of retries to perform an operation before giving up.  The default value is ``10``.
 * ``proxies``: A dictionary containing protocol to proxy URL mappings.  The default value is ``None``.  See `Using proxies`_.
 
-To crete a Redfish object, call the ``redfish_client`` method:
+To create a Redfish object, call the ``redfish_client`` method:
 
 .. code-block:: python
 
     REDFISH_OBJ = redfish.redfish_client(base_url=login_host, username=login_account, \
                           password=login_password, default_prefix='/redfish/v1/')
 
 Login to the service
@@ -109,42 +109,80 @@
 
     REDFISH_OBJ.login(auth="session")
 
 Perform a GET operation
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 A simple GET operation can be performed to obtain the data present in any valid path.
-An example of GET operation on the path "/redfish/v1/systems/1" is shown below:
+An example of GET operation on the path "/redfish/v1/Systems/1" is shown below:
 
 .. code-block:: python
 
-    response = REDFISH_OBJ.get("/redfish/v1/systems/1", None)
+    response = REDFISH_OBJ.get("/redfish/v1/Systems/1")
 
 Perform a POST operation
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 A POST operation can be performed to create a resource or perform an action.
-An example of a POST operation on the path "/redfish/v1/systems/1/Actions/ComputerSystem.Reset" is shown below:
+An example of a POST operation on the path "/redfish/v1/Systems/1/Actions/ComputerSystem.Reset" is shown below:
 
 .. code-block:: python
 
     body = {"ResetType": "GracefulShutdown"}
-    response = REDFISH_OBJ.post("/redfish/v1/systems/1/Actions/ComputerSystem.Reset", body=body)
+    response = REDFISH_OBJ.post("/redfish/v1/Systems/1/Actions/ComputerSystem.Reset", body=body)
+
+Notes about HTTP methods and arguments
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The previous sections showed example GET and POST requests.  The following is a list of the different methods supported:
+
+* ``get``: Performs an HTTP GET operation to retrieve a resource from a URI.
+* ``head``: Performs an HTTP HEAD operation to retrieve response headers from a URI, but no body.
+* ``post``: Performs an HTTP POST operation to perform an action or create a new resource.
+* ``put``: Performs an HTTP PUT operation to replace an existing resource.
+* ``patch``: Performs an HTTP PATCH operation to update an existing resource.
+* ``delete``: Performs an HTTP DELETE operation to remove a resource.
+
+Each of the previous methods allows for the following arguments:
+
+* ``path``: **Required**.  String.  The URI in which to invoke the operation.
+
+  - Example: ``"/redfish/v1/Systems/1"``
+
+* ``args``: Dictionary.  Query parameters to supply with the request.
+
+  - The key-value pairs in the dictionary are the query parameter name and the query parameter value to supply.
+  - Example: ``{"$select": "Reading,Status"}``
+
+* ``body``: Dictionary, List, Bytes, or String.  The request body to provide with the request.
+
+  - Not supported for ``get``, ``head``, or ``delete`` methods.
+  - The data type supplied will dictate the encoding.
+  - A dictionary is the most common usage, which results in a JSON body.
+  - Example: ``{"ResetType": "GracefulShutdown"}``
+  - A list is used to supply multipart forms, which is useful for multipart HTTP push updates.
+  - Bytes is used to supply an octet stream.
+  - A string is used to supply an unstructed body, which may be used in some OEM cases.
+
+* ``headers``: Dictionary.  Additional HTTP headers to supply with the request.
+
+  - The key-value pairs in the dictionary are the HTTP header name and the HTTP header value to supply.
+  - Example: ``{"If-Match": etag_value}``
 
 Working with tasks
 ~~~~~~~~~~~~~~~~~~
 
-A POST and PATCH operations may result in a task, describing an operation with a duration greater than the span of a single request.
+POST, PATCH, PUT, and DELETE operations may result in a task, describing an operation with a duration greater than the span of a single request.
 The action message object that ``is_processing`` will return a task that can be accessed reviewed when polled with monitor.
 An example of a POST operation with a possible task is shown below.
 
 .. code-block:: python
 
     body = {"ResetType": "GracefulShutdown"}
-    response = REDFISH_OBJ.post("/redfish/v1/systems/1/Actions/ComputerSystem.Reset", body=body)
+    response = REDFISH_OBJ.post("/redfish/v1/Systems/1/Actions/ComputerSystem.Reset", body=body)
     if(response.is_processing):
         task = response.monitor(context)
 
         while(task.is_processing):
             retry_time = task.retry_after
             task_status = task.dict['TaskState']
             time.sleep(retry_time if retry_time else 5)
@@ -218,8 +256,8 @@
 5. Click "Run workflow"
 
 Copyright and License
 ---------------------
 
 Copyright Notice:
 Copyright 2016-2022 DMTF. All rights reserved.
-License: BSD 3-Clause License. For full text see link: `https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md <https://github.com/DMTF/python-redfish-library/blob/master/LICENSE.md>`_
+License: BSD 3-Clause License. For full text see link: `https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md <https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md>`_
```

### Comparing `redfish-3.1.9/src/redfish.egg-info/SOURCES.txt` & `redfish-3.2.0/src/redfish.egg-info/SOURCES.txt`

 * *Files identical despite different names*

