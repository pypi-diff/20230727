# Comparing `tmp/retakesearch-0.1.12.tar.gz` & `tmp/retakesearch-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-0.1.12.tar", max compression
+gzip compressed data, was "retakesearch-0.1.15.tar", max compression
```

## Comparing `retakesearch-0.1.12.tar` & `retakesearch-0.1.15.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-26 16:07:18.332412 retakesearch-0.1.12/README.md
--rw-r--r--   0        0        0      412 2023-07-26 16:07:39.896618 retakesearch-0.1.12/pyproject.toml
--rw-r--r--   0        0        0      140 2023-07-26 16:07:18.332412 retakesearch-0.1.12/retakesearch/__init__.py
--rw-r--r--   0        0        0     2471 2023-07-26 16:07:18.332412 retakesearch-0.1.12/retakesearch/client.py
--rw-r--r--   0        0        0      159 2023-07-26 16:07:18.332412 retakesearch-0.1.12/retakesearch/search.py
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 retakesearch-0.1.12/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-27 17:31:42.520071 retakesearch-0.1.15/README.md
+-rw-r--r--   0        0        0      412 2023-07-27 17:32:04.096430 retakesearch-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-07-27 17:31:42.520071 retakesearch-0.1.15/retakesearch/__init__.py
+-rw-r--r--   0        0        0     1277 2023-07-27 17:31:42.520071 retakesearch-0.1.15/retakesearch/client.py
+-rw-r--r--   0        0        0     2571 2023-07-27 17:31:42.520071 retakesearch-0.1.15/retakesearch/index.py
+-rw-r--r--   0        0        0      159 2023-07-27 17:31:42.520071 retakesearch-0.1.15/retakesearch/search.py
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 retakesearch-0.1.15/PKG-INFO
```

### Comparing `retakesearch-0.1.12/retakesearch/client.py` & `retakesearch-0.1.15/retakesearch/index.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import httpx
+
 from opensearchpy import Search
 from typing import Any, List
 
 
 class Database:
     def __init__(self, host: str, user: str, password: str, port: int):
         self.host = host
@@ -17,54 +18,57 @@
     ):
         self.name = name
         self.primary_key = primary_key
         self.columns = columns
         self.neural_columns = neural_columns
 
 
-class Client:
-    def __init__(self, api_key: str, url: str):
+class Index:
+    def __init__(self, index_name: str, api_key: str, url: str) -> None:
+        self.index_name = index_name
         self.api_key = api_key
         self.url = url
+
         self.headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
 
-    def index(self, database: Database, table: Table, reindex: bool = False) -> Any:
+    def add_source(self, database: Database, table: Table) -> Any:
         json = {
+            "index_name": self.index_name,
             "source_host": database.host,
             "source_user": database.user,
             "source_password": database.password,
             "source_port": database.port,
             "source_relation": table.name,
             "source_primary_key": table.primary_key,
             "source_columns": table.columns,
             "source_neural_columns": table.neural_columns,
-            "reindex": reindex,
         }
+
         try:
             with httpx.Client(timeout=None) as http:
                 print(
-                    f"Indexing {table.name}. This could take some time if the table is large..."
+                    f"Adding {table.name} to index {self.index_name}. This could take some time if the table is large..."
                 )
                 response = http.post(
-                    f"{self.url}/client/index", headers=self.headers, json=json
+                    f"{self.url}/index/add_source", headers=self.headers, json=json
                 )
                 response.raise_for_status()
                 return response.json()
         except httpx.HTTPStatusError as exc:
             return exc.response.json()
         except Exception as exc:
             return str(exc)
 
-    def search(self, table: str, search: Search) -> Any:
+    def search(self, search: Search) -> Any:
         json = {
-            "dsl": search.to_dict(),
-            "index_name": table,
+            "dsl": search.to_dict(),  # type: ignore
+            "index_name": self.index_name,
         }
         try:
             with httpx.Client(timeout=None) as http:
                 response = http.post(
                     f"{self.url}/index/search", headers=self.headers, json=json
                 )
                 response.raise_for_status()
```

### Comparing `retakesearch-0.1.12/PKG-INFO` & `retakesearch-0.1.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: retakesearch
-Version: 0.1.12
+Version: 0.1.15
 Summary: Open Source Neural Search Engine Python Client
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi (>=2023.7.22,<2024.0.0)
-Requires-Dist: retakesearch-py (>=2.2.0,<3.0.0)
+Requires-Dist: retakesearch-py (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
```

