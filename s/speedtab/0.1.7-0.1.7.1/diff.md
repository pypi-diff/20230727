# Comparing `tmp/speedtab-0.1.7.tar.gz` & `tmp/speedtab-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.7.tar", max compression
+gzip compressed data, was "speedtab-0.1.7.1.tar", max compression
```

## Comparing `speedtab-0.1.7.tar` & `speedtab-0.1.7.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      565 2023-07-24 16:25:14.147381 speedtab-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      354 2023-07-24 13:24:26.057717 speedtab-0.1.7/speedtab/__init__.py
--rw-r--r--   0        0        0    53658 2023-07-24 16:25:14.106218 speedtab-0.1.7/speedtab/client.py
--rw-r--r--   0        0        0     6520 2023-07-24 13:55:52.073795 speedtab-0.1.7/speedtab/enums.py
--rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.7/speedtab/formats.py
--rw-r--r--   0        0        0      781 2023-07-24 16:25:19.956258 speedtab-0.1.7/setup.py
--rw-r--r--   0        0        0      806 2023-07-24 16:25:19.957268 speedtab-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-07-27 14:35:28.726773 speedtab-0.1.7.1/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-07-24 13:24:26.057717 speedtab-0.1.7.1/speedtab/__init__.py
+-rw-r--r--   0        0        0    53731 2023-07-27 14:36:01.264984 speedtab-0.1.7.1/speedtab/client.py
+-rw-r--r--   0        0        0     6520 2023-07-24 13:55:52.073795 speedtab-0.1.7.1/speedtab/enums.py
+-rw-r--r--   0        0        0     1848 2023-07-21 13:53:11.575405 speedtab-0.1.7.1/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-07-27 14:36:24.456475 speedtab-0.1.7.1/setup.py
+-rw-r--r--   0        0        0      808 2023-07-27 14:36:24.456475 speedtab-0.1.7.1/PKG-INFO
```

### Comparing `speedtab-0.1.7/pyproject.toml` & `speedtab-0.1.7.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.7"
+version = "0.1.7.1"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.7/speedtab/client.py` & `speedtab-0.1.7.1/speedtab/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1139,17 +1139,17 @@
             return self.create_folder(folder_name, current_folder)
         else:
             return None
 
     def delete_file(self, file_id: str):
         self.connect_v3.files().delete(fileId=file_id).execute()
 
-    def move_spreadsheet_to_folder(self, ss: SpreedSheet, real_folder_id: str):
+    def move_spreadsheet_to_folder(self, ss: SpreedSheet, real_folder_id: str, supports_all_drives: bool = True):
         previous_parents = ','.join(self.connect_v3.files().get(fileId=ss.spreadsheet_id, fields='parents').execute().get('parents'))
-        self.connect_v3.files().update(fileId=ss.spreadsheet_id, addParents=real_folder_id,
+        self.connect_v3.files().update(fileId=ss.spreadsheet_id, addParents=real_folder_id, supportsAllDrives=supports_all_drives,
                                        removeParents=previous_parents, fields='id, parents').execute()
 
     def share_spreadsheet_with_domain(self, ss: SpreedSheet, domain: str, role: ShareRole):
         self.connect_v3.permissions().create(**{
             'fileId': ss.spreadsheet_id,
             'body': {
                 'type': 'domain',
```

### Comparing `speedtab-0.1.7/speedtab/enums.py` & `speedtab-0.1.7.1/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.7/speedtab/formats.py` & `speedtab-0.1.7.1/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.7/setup.py` & `speedtab-0.1.7.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.7',
+    'version': '0.1.7.1',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.7/PKG-INFO` & `speedtab-0.1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

