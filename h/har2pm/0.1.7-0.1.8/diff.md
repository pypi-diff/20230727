# Comparing `tmp/har2pm-0.1.7.tar.gz` & `tmp/har2pm-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "har2pm-0.1.7.tar", max compression
+gzip compressed data, was "har2pm-0.1.8.tar", max compression
```

## Comparing `har2pm-0.1.7.tar` & `har2pm-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       50 2023-07-14 10:20:04.533135 har2pm-0.1.7/har2pm/__init__.py
--rw-r--r--   0        0        0     1106 2023-07-17 03:34:06.940299 har2pm-0.1.7/har2pm/cli.py
--rw-r--r--   0        0        0     3723 2023-07-18 03:33:17.277795 har2pm-0.1.7/har2pm/common.py
--rw-r--r--   0        0        0     1851 2023-07-17 03:34:06.940299 har2pm-0.1.7/har2pm/har2postman.py
--rw-r--r--   0        0        0     1083 2023-07-14 10:20:04.532132 har2pm-0.1.7/LICENSE
--rw-r--r--   0        0        0      689 2023-07-18 03:33:43.534800 har2pm-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      604 2023-07-14 10:20:04.532132 har2pm-0.1.7/README.md
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 har2pm-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-07-14 10:20:04.533135 har2pm-0.1.8/har2pm/__init__.py
+-rw-r--r--   0        0        0     1106 2023-07-17 03:34:06.940299 har2pm-0.1.8/har2pm/cli.py
+-rw-r--r--   0        0        0     3723 2023-07-18 03:33:17.277795 har2pm-0.1.8/har2pm/common.py
+-rw-r--r--   0        0        0     1950 2023-07-27 02:36:24.900740 har2pm-0.1.8/har2pm/har2postman.py
+-rw-r--r--   0        0        0     1083 2023-07-14 10:20:04.532132 har2pm-0.1.8/LICENSE
+-rw-r--r--   0        0        0      689 2023-07-27 02:36:34.615759 har2pm-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      604 2023-07-14 10:20:04.532132 har2pm-0.1.8/README.md
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 har2pm-0.1.8/PKG-INFO
```

### Comparing `har2pm-0.1.7/har2pm/cli.py` & `har2pm-0.1.8/har2pm/cli.py`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.7/har2pm/common.py` & `har2pm-0.1.8/har2pm/common.py`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.7/har2pm/har2postman.py` & `har2pm-0.1.8/har2pm/har2postman.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,18 @@
 
         if request['method'] == 'POST':
             postman_request['body'] = convert_body(request)
 
         # 处理 headers
         postman_request['header'] = convert_headers(request['headers'])
 
-        self.postman_collection['item'].append({'name': request['url'], 'request': postman_request})
+        post_data = {'name': request['url'], 'request': postman_request}
+
+        if post_data not in self.postman_collection['item']:
+            self.postman_collection['item'].append(post_data)
 
     def run(self, generate_file=True):
         logging.info(f'read {self.har_path}')
 
         data = load_har(self.har_path)
         requests = jmespath.search('log.entries[].request', data)
```

### Comparing `har2pm-0.1.7/LICENSE` & `har2pm-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.7/pyproject.toml` & `har2pm-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "har2pm"
-version = "0.1.7"
+version = "0.1.8"
 description = "Convert HAR(HTTP Archive) to Postman Collection"
 authors = ["ysansan"]
 license = "MIT"
 homepage = "https://github.com/whitexie/Har2Postman"
 repository = "https://github.com/whitexie/Har2Postman"
 keywords = ["har", "postman"]
 readme = "README.md"
```

### Comparing `har2pm-0.1.7/README.md` & `har2pm-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `har2pm-0.1.7/PKG-INFO` & `har2pm-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: har2pm
-Version: 0.1.7
+Version: 0.1.8
 Summary: Convert HAR(HTTP Archive) to Postman Collection
 Home-page: https://github.com/whitexie/Har2Postman
 License: MIT
 Keywords: har,postman
 Author: ysansan
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

