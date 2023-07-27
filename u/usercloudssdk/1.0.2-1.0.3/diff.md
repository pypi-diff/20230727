# Comparing `tmp/usercloudssdk-1.0.2.tar.gz` & `tmp/usercloudssdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usercloudssdk-1.0.2.tar", last modified: Thu Jul 27 13:40:15 2023, max compression
+gzip compressed data, was "usercloudssdk-1.0.3.tar", last modified: Thu Jul 27 19:01:05 2023, max compression
```

## Comparing `usercloudssdk-1.0.2.tar` & `usercloudssdk-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 13:40:15.431465 usercloudssdk-1.0.2/
--rw-r--r--   0 jwang      (501) staff       (20)     1103 2023-07-27 00:46:25.000000 usercloudssdk-1.0.2/LICENSE
--rw-r--r--   0 jwang      (501) staff       (20)     1507 2023-07-27 13:40:15.431352 usercloudssdk-1.0.2/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)       12 2023-07-27 00:40:23.000000 usercloudssdk-1.0.2/README.md
--rw-r--r--   0 jwang      (501) staff       (20)      380 2023-07-27 13:39:01.000000 usercloudssdk-1.0.2/pyproject.toml
--rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-27 13:40:15.431499 usercloudssdk-1.0.2/setup.cfg
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 13:40:15.428290 usercloudssdk-1.0.2/src/
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 13:40:15.430628 usercloudssdk-1.0.2/src/usercloudssdk/
--rw-r--r--   0 jwang      (501) staff       (20)        0 2023-06-13 16:36:00.000000 usercloudssdk-1.0.2/src/usercloudssdk/__init__.py
--rw-r--r--   0 jwang      (501) staff       (20)    17689 2023-07-27 13:23:56.000000 usercloudssdk-1.0.2/src/usercloudssdk/client.py
--rw-r--r--   0 jwang      (501) staff       (20)      636 2023-06-30 17:46:25.000000 usercloudssdk-1.0.2/src/usercloudssdk/constants.py
--rw-r--r--   0 jwang      (501) staff       (20)    14342 2023-07-27 13:23:37.000000 usercloudssdk-1.0.2/src/usercloudssdk/models.py
--rw-r--r--   0 jwang      (501) staff       (20)      790 2023-07-27 13:34:23.000000 usercloudssdk-1.0.2/src/usercloudssdk/policies.py
--rw-r--r--   0 jwang      (501) staff       (20)     6377 2023-07-27 13:28:09.000000 usercloudssdk-1.0.2/src/usercloudssdk/tokenizer_sample.py
--rw-r--r--   0 jwang      (501) staff       (20)      405 2023-06-13 16:36:00.000000 usercloudssdk-1.0.2/src/usercloudssdk/ucjson.py
--rw-r--r--   0 jwang      (501) staff       (20)    11159 2023-07-27 13:36:23.000000 usercloudssdk-1.0.2/src/usercloudssdk/userstore_sample.py
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 13:40:15.431204 usercloudssdk-1.0.2/src/usercloudssdk.egg-info/
--rw-r--r--   0 jwang      (501) staff       (20)     1507 2023-07-27 13:40:15.000000 usercloudssdk-1.0.2/src/usercloudssdk.egg-info/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)      447 2023-07-27 13:40:15.000000 usercloudssdk-1.0.2/src/usercloudssdk.egg-info/SOURCES.txt
--rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-27 13:40:15.000000 usercloudssdk-1.0.2/src/usercloudssdk.egg-info/dependency_links.txt
--rw-r--r--   0 jwang      (501) staff       (20)       14 2023-07-27 13:40:15.000000 usercloudssdk-1.0.2/src/usercloudssdk.egg-info/top_level.txt
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 19:01:05.584837 usercloudssdk-1.0.3/
+-rw-r--r--   0 jwang      (501) staff       (20)     1103 2023-07-27 17:28:09.000000 usercloudssdk-1.0.3/LICENSE
+-rw-r--r--   0 jwang      (501) staff       (20)     1507 2023-07-27 19:01:05.584720 usercloudssdk-1.0.3/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)       12 2023-07-27 00:40:23.000000 usercloudssdk-1.0.3/README.md
+-rw-r--r--   0 jwang      (501) staff       (20)      634 2023-07-27 19:00:20.000000 usercloudssdk-1.0.3/pyproject.toml
+-rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-27 19:01:05.584873 usercloudssdk-1.0.3/setup.cfg
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 19:01:05.581624 usercloudssdk-1.0.3/src/
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 19:01:05.583876 usercloudssdk-1.0.3/src/usercloudssdk/
+-rw-r--r--   0 jwang      (501) staff       (20)        0 2023-07-27 13:43:32.000000 usercloudssdk-1.0.3/src/usercloudssdk/__init__.py
+-rw-r--r--   0 jwang      (501) staff       (20)    17780 2023-07-27 17:19:10.000000 usercloudssdk-1.0.3/src/usercloudssdk/client.py
+-rw-r--r--   0 jwang      (501) staff       (20)      636 2023-07-27 13:43:32.000000 usercloudssdk-1.0.3/src/usercloudssdk/constants.py
+-rw-r--r--   0 jwang      (501) staff       (20)    14342 2023-07-27 17:19:10.000000 usercloudssdk-1.0.3/src/usercloudssdk/models.py
+-rw-r--r--   0 jwang      (501) staff       (20)      790 2023-07-27 17:19:10.000000 usercloudssdk-1.0.3/src/usercloudssdk/policies.py
+-rw-r--r--   0 jwang      (501) staff       (20)     6377 2023-07-27 17:19:10.000000 usercloudssdk-1.0.3/src/usercloudssdk/tokenizer_sample.py
+-rw-r--r--   0 jwang      (501) staff       (20)      405 2023-07-27 13:43:32.000000 usercloudssdk-1.0.3/src/usercloudssdk/ucjson.py
+-rw-r--r--   0 jwang      (501) staff       (20)    11159 2023-07-27 17:19:10.000000 usercloudssdk-1.0.3/src/usercloudssdk/userstore_sample.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 19:01:05.584581 usercloudssdk-1.0.3/src/usercloudssdk.egg-info/
+-rw-r--r--   0 jwang      (501) staff       (20)     1507 2023-07-27 19:01:05.000000 usercloudssdk-1.0.3/src/usercloudssdk.egg-info/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)      487 2023-07-27 19:01:05.000000 usercloudssdk-1.0.3/src/usercloudssdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-27 19:01:05.000000 usercloudssdk-1.0.3/src/usercloudssdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jwang      (501) staff       (20)      166 2023-07-27 19:01:05.000000 usercloudssdk-1.0.3/src/usercloudssdk.egg-info/requires.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       14 2023-07-27 19:01:05.000000 usercloudssdk-1.0.3/src/usercloudssdk.egg-info/top_level.txt
```

### Comparing `usercloudssdk-1.0.2/LICENSE` & `usercloudssdk-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.2/PKG-INFO` & `usercloudssdk-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usercloudssdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python SDK for UserClouds
 Author-email: Real Python <info@realpython.com>
 License: The MIT License
         
         Copyright (c) 2021- UserClouds, Inc. (https://userclouds.com)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `usercloudssdk-1.0.2/src/usercloudssdk/client.py` & `usercloudssdk-1.0.3/src/usercloudssdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,18 +77,15 @@
             params["limit"] = limit
         if starting_after is not None:
             params["starting_after"] = f"id:{str(starting_after)}"
         if email is not None:
             params["email"] = email
         params["version"] = "2"
         j = self._get("/authn/users", params=params)
-        if email is None:
-            users = [UserResponse.from_json(ur) for ur in j["data"]]
-        else:
-            users = [UserResponse.from_json(ur) for ur in j]
+        users = [UserResponse.from_json(ur) for ur in j["data"]]
         return users
 
     def GetUser(self, id: uuid.UUID) -> UserResponse:
         j = self._get(f"/authn/users/{str(id)}")
         return UserResponse.from_json(j)
 
     def UpdateUser(self, id: uuid.UUID, profile: dict) -> UserResponse:
@@ -119,21 +116,25 @@
     def DeleteColumn(self, id: uuid.UUID) -> str:
         return self._delete(f"/userstore/config/columns/{str(id)}")
 
     def GetColumn(self, id: uuid.UUID) -> Column:
         j = self._get(f"/userstore/config/columns/{str(id)}")
         return Column.from_json(j)
 
-    def ListColumns(self) -> list[Column]:
-        j = self._get("/userstore/config/columns")
-
-        columns = []
-        for c in j:
-            columns.append(Column.from_json(c))
-
+    def ListColumns(
+        self, limit: int = 0, starting_after: uuid.UUID = None
+    ) -> list[Column]:
+        params = {}
+        if limit > 0:
+            params["limit"] = limit
+        if starting_after is not None:
+            params["starting_after"] = f"id:{str(starting_after)}"
+        params["version"] = "2"
+        j = self._get("/userstore/config/columns", params=params)
+        columns = [Column.from_json(c) for c in j["data"]]
         return columns
 
     def UpdateColumn(self, column: Column) -> Column:
         body = {"column": column.__dict__}
 
         j = self._put(f"/userstore/config/columns/{column.id}", data=ucjson.dumps(body))
         return Column.from_json(j)
@@ -337,19 +338,15 @@
 
     def GetAccessor(self, id: uuid.UUID) -> Accessor:
         j = self._get(f"/userstore/config/accessors/{str(id)}")
         return Accessor.from_json(j)
 
     def ListAccessors(self) -> list[Accessor]:
         j = self._get("/userstore/config/accessors")
-
-        accessors = []
-        for a in j:
-            accessors.append(Accessor.from_json(a))
-
+        accessors = [Accessor.from_json(a) for a in j["data"]]
         return accessors
 
     def UpdateAccessor(self, accessor: Accessor) -> Accessor:
         body = {"accessor": accessor.__dict__}
 
         j = self._put(
             f"/userstore/config/accessors/{accessor.id}",
@@ -388,19 +385,15 @@
 
     def GetMutator(self, id: uuid.UUID) -> Mutator:
         j = self._get(f"/userstore/config/mutators/{str(id)}")
         return Mutator.from_json(j)
 
     def ListMutators(self) -> list[Mutator]:
         j = self._get("/userstore/config/mutators")
-
-        mutators = []
-        for a in j:
-            mutators.append(Mutator.from_json(a))
-
+        mutators = [Mutator.from_json(m) for m in j["data"]]
         return mutators
 
     def UpdateMutator(self, mutator: Mutator) -> Mutator:
         body = {"mutator": mutator.__dict__}
 
         j = self._put(
             f"/userstore/config/mutators/{mutator.id}",
```

### Comparing `usercloudssdk-1.0.2/src/usercloudssdk/constants.py` & `usercloudssdk-1.0.3/src/usercloudssdk/constants.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.2/src/usercloudssdk/models.py` & `usercloudssdk-1.0.3/src/usercloudssdk/models.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.2/src/usercloudssdk/policies.py` & `usercloudssdk-1.0.3/src/usercloudssdk/policies.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.2/src/usercloudssdk/tokenizer_sample.py` & `usercloudssdk-1.0.3/src/usercloudssdk/tokenizer_sample.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.2/src/usercloudssdk/userstore_sample.py` & `usercloudssdk-1.0.3/src/usercloudssdk/userstore_sample.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.2/src/usercloudssdk.egg-info/PKG-INFO` & `usercloudssdk-1.0.3/src/usercloudssdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usercloudssdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python SDK for UserClouds
 Author-email: Real Python <info@realpython.com>
 License: The MIT License
         
         Copyright (c) 2021- UserClouds, Inc. (https://userclouds.com)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

