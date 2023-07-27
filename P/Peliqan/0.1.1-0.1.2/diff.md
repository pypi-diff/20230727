# Comparing `tmp/Peliqan-0.1.1.tar.gz` & `tmp/Peliqan-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Peliqan-0.1.1.tar", last modified: Wed Jul 26 07:00:06 2023, max compression
+gzip compressed data, was "Peliqan-0.1.2.tar", last modified: Thu Jul 27 13:12:20 2023, max compression
```

## Comparing `Peliqan-0.1.1.tar` & `Peliqan-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-26 07:00:06.422699 Peliqan-0.1.1/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-26 07:00:06.422554 Peliqan-0.1.1/PKG-INFO
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-26 07:00:06.421940 Peliqan-0.1.1/Peliqan.egg-info/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-26 07:00:06.000000 Peliqan-0.1.1/Peliqan.egg-info/PKG-INFO
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      192 2023-07-26 07:00:06.000000 Peliqan-0.1.1/Peliqan.egg-info/SOURCES.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2023-07-26 07:00:06.000000 Peliqan-0.1.1/Peliqan.egg-info/dependency_links.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2023-07-26 07:00:06.000000 Peliqan-0.1.1/Peliqan.egg-info/requires.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2023-07-26 07:00:06.000000 Peliqan-0.1.1/Peliqan.egg-info/top_level.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-07-14 07:23:16.000000 Peliqan-0.1.1/README.md
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-26 07:00:06.422267 Peliqan-0.1.1/peliqan/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    37222 2023-07-26 06:45:43.000000 Peliqan-0.1.1/peliqan/__init__.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2023-07-26 07:00:06.422792 Peliqan-0.1.1/setup.cfg
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1335 2023-07-25 13:32:11.000000 Peliqan-0.1.1/setup.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-27 13:12:20.620772 Peliqan-0.1.2/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-27 13:12:20.620634 Peliqan-0.1.2/PKG-INFO
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-27 13:12:20.620336 Peliqan-0.1.2/Peliqan.egg-info/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2023-07-27 13:12:20.000000 Peliqan-0.1.2/Peliqan.egg-info/PKG-INFO
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      192 2023-07-27 13:12:20.000000 Peliqan-0.1.2/Peliqan.egg-info/SOURCES.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2023-07-27 13:12:20.000000 Peliqan-0.1.2/Peliqan.egg-info/dependency_links.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2023-07-27 13:12:20.000000 Peliqan-0.1.2/Peliqan.egg-info/requires.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2023-07-27 13:12:20.000000 Peliqan-0.1.2/Peliqan.egg-info/top_level.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-07-27 13:05:47.000000 Peliqan-0.1.2/README.md
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2023-07-27 13:12:20.620439 Peliqan-0.1.2/peliqan/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    38718 2023-07-27 13:10:58.000000 Peliqan-0.1.2/peliqan/__init__.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2023-07-27 13:12:20.620811 Peliqan-0.1.2/setup.cfg
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1335 2023-07-27 13:05:47.000000 Peliqan-0.1.2/setup.py
```

### Comparing `Peliqan-0.1.1/PKG-INFO` & `Peliqan-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-0.1.1/Peliqan.egg-info/PKG-INFO` & `Peliqan-0.1.2/Peliqan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-0.1.1/README.md` & `Peliqan-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `Peliqan-0.1.1/peliqan/__init__.py` & `Peliqan-0.1.2/peliqan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __author__ = 'Peliqan.io'
 __credits__ = 'Peliqan.io'
 
 # import necessary modules
 import logging
 
 import pandas
@@ -70,14 +70,26 @@
             error_message = f"Server responded with status code {response.status_code}"
             if response_dict:
                 error_message += f" and error details \n{response_dict}"
             raise PeliqanClientException(error_message)
 
         return response_dict
 
+    def args_to_kwargs(self, args, kwargs):
+        """
+        Used in writeback functions add(), update() etc. to allow using both a dict argument or keyword arguments:
+        pq.add("contact", name='John', city='NY') or
+        pq.add("contact", contact_obj)
+        """
+        for arg in args:
+            if type(arg) != dict:
+                raise PeliqanClientException("Only arguments of type dict and kwargs are accepted")
+            kwargs.update(**arg)
+        return kwargs
+
 
 class WritebackClient(BaseClient):
     def __init__(self, connection, jwt, backend_url):
         super(WritebackClient, self).__init__(jwt, backend_url)
         self.connection = connection
 
     def request_endpoint_via_proxy(self, object_name, action, **kwargs):
@@ -96,35 +108,45 @@
         response_dict = self.request_endpoint_via_proxy(object_name, 'get', **kwargs)
         if "detail" in response_dict:
             return response_dict["detail"]
         else:
             return response_dict
 
     def findone(self, object_name, **kwargs):
-        if "searchfield" not in kwargs or "searchterm" not in kwargs:
-            raise PeliqanClientException(f"Parameters searchfield and searchfield are required for function 'findone'.")
+        if "searchterm" not in kwargs:
+            raise PeliqanClientException(f"Parameter searchterm is required and searchfield is sometimes required for function 'findone'.")
         response_dict = self.request_endpoint_via_proxy(object_name, 'findone', **kwargs)
         if "detail" in response_dict:
-            return response_dict["detail"]
+            detail = response_dict["detail"]
+            if not isinstance(detail, dict): # replace empty string response "" (if no record found) with {}
+                detail = {}
+            return detail
         else:
             return response_dict
 
     def list(self, object_name, **kwargs):
         response_dict = self.request_endpoint_via_proxy(object_name, 'list', **kwargs)
         return response_dict
 
-    def add(self, object_name, **kwargs):
+    def add(self, object_name, *args, **kwargs):
+        kwargs = self.args_to_kwargs(args, kwargs) # allow using both keyword arguments or a dict as argument: pq.add("contact", name='John', city='NY') or pq.add("contact", contact_obj)
         response_dict = self.request_endpoint_via_proxy(object_name, 'add', **kwargs)
         return response_dict
 
-    def update(self, object_name, **kwargs):
+    def update(self, object_name, *args, **kwargs):
+        kwargs = self.args_to_kwargs(args, kwargs) # allow using both keyword arguments or a dict as argument: pq.update("contact", name='John', city='NY') or pq.update("contact", contact_obj)
         response_dict = self.request_endpoint_via_proxy(object_name, 'update', **kwargs)
         return response_dict
 
-    def upsert(self, object_name, **kwargs):
+    def upsert(self, object_name, *args, **kwargs):
+        kwargs = self.args_to_kwargs(args, kwargs) # allow using both keyword arguments or a dict as argument: pq.update("contact", name='John', city='NY') or pq.update("contact", contact_obj)
+        if "searchterm" not in kwargs:
+            raise PeliqanClientException(f"Parameter searchterm is required and searchfield is sometimes required for function 'upsert'.")
+        if "searchfield" not in kwargs:
+            kwargs["searchfield"] = None
         response_dict_findone = self.request_endpoint_via_proxy(object_name, 'findone',
                                                                 searchfield=kwargs["searchfield"],
                                                                 searchterm=kwargs["searchterm"])
         kwargs.pop('searchfield', None)
         kwargs.pop('searchterm', None)
         if "detail" in response_dict_findone and "id" in response_dict_findone["detail"]:
             kwargs["id"] = response_dict_findone["detail"]["id"]
```

### Comparing `Peliqan-0.1.1/setup.py` & `Peliqan-0.1.2/setup.py`

 * *Files identical despite different names*

