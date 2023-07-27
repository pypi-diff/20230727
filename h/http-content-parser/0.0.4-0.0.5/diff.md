# Comparing `tmp/http_content_parser-0.0.4.tar.gz` & `tmp/http_content_parser-0.0.5.tar.gz`

## Comparing `http_content_parser-0.0.4.tar` & `http_content_parser-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/src/http_content_parser/__init__.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/src/http_content_parser/curl_parser.py
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/src/http_content_parser/generate_api_file.py
--rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/src/http_content_parser/openapi_parser.py
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/src/http_content_parser/param_util.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/src/http_content_parser/postman_parser.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/src/http_content_parser/req_data.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/src/http_content_parser/swagger2_parser.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/LICENSE
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/README.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 http_content_parser-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/src/http_content_parser/__init__.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/src/http_content_parser/curl_parser.py
+-rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/src/http_content_parser/generate_api_file.py
+-rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/src/http_content_parser/openapi_parser.py
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/src/http_content_parser/param_util.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/src/http_content_parser/postman_parser.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/src/http_content_parser/req_data.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/src/http_content_parser/swagger2_parser.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/LICENSE
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 http_content_parser-0.0.5/PKG-INFO
```

### Comparing `http_content_parser-0.0.4/src/http_content_parser/curl_parser.py` & `http_content_parser-0.0.5/src/http_content_parser/curl_parser.py`

 * *Files identical despite different names*

### Comparing `http_content_parser-0.0.4/src/http_content_parser/generate_api_file.py` & `http_content_parser-0.0.5/src/http_content_parser/generate_api_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,34 +26,63 @@
             req_data.method = api_info['method'].lower()
             req_data.temp_api_label = self.convert_swagger2_path(
                 api_info['path'].split('/'), '_').replace('{', '').replace('}', '') + "_" + api_info['method'].lower()
             self.write_api_content_to_yaml(yaml_file, req_data)
         # remove duplicate key
         self.remove_duplicate_key_for_yaml(yaml_file)
 
+    # def produce_api_yaml_for_curl2(self, curl_file, yaml_file, curl_filter=None):
+    #     curl_parser = CurlParser()
+    #     with open(curl_file, 'rt') as f:
+    #         lines = f.readlines()
+    #         line_num_array = curl_parser.get_curl_line_num_scope(lines=lines)
+    #         for r in line_num_array:
+    #             res_dict = curl_parser.split_curl_to_struct(
+    #                 lines, r[0], r[1], curl_filter)
+    #             template = ReqData(dd=res_dict)
+    #             split_url = curl_parser.split_url(template.original_url, '_')
+    #             template.temp_api_label = self.replace_api_label_chars(
+    #                 split_url['url_path']) + template.method
+    #             template.header = json.dumps(template.header)
+    #             template.query_param = json.dumps(split_url['url_params'])
+    #             split_url_origin = curl_parser.split_url(
+    #                 template.original_url, '/')
+    #             template.path = split_url_origin['url_path'][:-1]
+    #             self.write_api_content_to_yaml(yaml_file, template)
+    #     # remove duplicate key
+    #     self.remove_duplicate_key_for_yaml(yaml_file)
+
     def produce_api_yaml_for_curl(self, curl_file, yaml_file, curl_filter=None):
+        payload_list = self.convert_curl_data_to_model(
+            curl_file_path=curl_file, curl_filter=curl_filter)
+        for payload in payload_list:
+            self.write_api_content_to_yaml(yaml_file, payload)
+        # remove duplicate key
+        self.remove_duplicate_key_for_yaml(yaml_file)
+
+    def convert_curl_data_to_model(self, curl_file_path, curl_filter=None) -> list[ReqData]:
         curl_parser = CurlParser()
-        with open(curl_file, 'rt') as f:
+        payload_list = []
+        with open(curl_file_path, 'rt') as f:
             lines = f.readlines()
             line_num_array = curl_parser.get_curl_line_num_scope(lines=lines)
             for r in line_num_array:
                 res_dict = curl_parser.split_curl_to_struct(
                     lines, r[0], r[1], curl_filter)
                 template = ReqData(dd=res_dict)
                 split_url = curl_parser.split_url(template.original_url, '_')
                 template.temp_api_label = self.replace_api_label_chars(
                     split_url['url_path']) + template.method
                 template.header = json.dumps(template.header)
                 template.query_param = json.dumps(split_url['url_params'])
                 split_url_origin = curl_parser.split_url(
                     template.original_url, '/')
                 template.path = split_url_origin['url_path'][:-1]
-                self.write_api_content_to_yaml(yaml_file, template)
-        # remove duplicate key
-        self.remove_duplicate_key_for_yaml(yaml_file)
+                payload_list.append(template)
+        return payload_list
 
     def produce_api_yaml_for_swagger2(self, swagger2_dict, yaml_file):
         swagger_parser = Swagger2Parser(swagger2_dict)
         api_dict = swagger_parser.get_swagger_api_info()
         if not api_dict:
             print('check your swagger json')
             return
```

### Comparing `http_content_parser-0.0.4/src/http_content_parser/openapi_parser.py` & `http_content_parser-0.0.5/src/http_content_parser/openapi_parser.py`

 * *Files identical despite different names*

### Comparing `http_content_parser-0.0.4/src/http_content_parser/param_util.py` & `http_content_parser-0.0.5/src/http_content_parser/param_util.py`

 * *Files identical despite different names*

### Comparing `http_content_parser-0.0.4/src/http_content_parser/postman_parser.py` & `http_content_parser-0.0.5/src/http_content_parser/postman_parser.py`

 * *Files identical despite different names*

### Comparing `http_content_parser-0.0.4/src/http_content_parser/req_data.py` & `http_content_parser-0.0.5/src/http_content_parser/req_data.py`

 * *Files identical despite different names*

### Comparing `http_content_parser-0.0.4/src/http_content_parser/swagger2_parser.py` & `http_content_parser-0.0.5/src/http_content_parser/swagger2_parser.py`

 * *Files identical despite different names*

### Comparing `http_content_parser-0.0.4/LICENSE` & `http_content_parser-0.0.5/LICENSE`

 * *Files identical despite different names*

