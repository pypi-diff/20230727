# Comparing `tmp/tableau_utilities-2.0.62.tar.gz` & `tmp/tableau_utilities-2.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau_utilities-2.0.62.tar", last modified: Tue Jul 25 18:34:00 2023, max compression
+gzip compressed data, was "tableau_utilities-2.0.63.tar", last modified: Thu Jul 27 17:52:26 2023, max compression
```

## Comparing `tableau_utilities-2.0.62.tar` & `tableau_utilities-2.0.63.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.835278 tableau_utilities-2.0.62/
--rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.0.62/LICENSE
--rw-r--r--   0 justin     (502) staff       (20)     8421 2023-07-25 18:34:00.834964 tableau_utilities-2.0.62/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     8116 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/README.md
--rw-r--r--   0 justin     (502) staff       (20)       38 2023-07-25 18:34:00.835397 tableau_utilities-2.0.62/setup.cfg
--rw-r--r--   0 justin     (502) staff       (20)     1108 2023-07-25 18:33:34.000000 tableau_utilities-2.0.62/setup.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.814806 tableau_utilities-2.0.62/tableau_utilities/
--rw-r--r--   0 justin     (502) staff       (20)      272 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2441 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/fetch_all_cols.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.822366 tableau_utilities-2.0.62/tableau_utilities/general/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/general/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/general/cli_styling.py
--rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/general/config_column_persona.py
--rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/general/funcs.py
--rw-r--r--   0 justin     (502) staff       (20)     2874 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripted_testing.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.829404 tableau_utilities-2.0.62/tableau_utilities/scripts/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    23247 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/cli.py
--rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/csv_config.py
--rw-r--r--   0 justin     (502) staff       (20)     7863 2023-07-25 18:33:34.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/datasource.py
--rw-r--r--   0 justin     (502) staff       (20)    13151 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/gen_config.py
--rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/merge_config.py
--rw-r--r--   0 justin     (502) staff       (20)     1867 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/server_info.py
--rw-r--r--   0 justin     (502) staff       (20)     4531 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/scripts/server_operate.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.831492 tableau_utilities-2.0.62/tableau_utilities/tableau_file/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/tableau_file/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    12316 2023-07-18 22:10:49.000000 tableau_utilities-2.0.62/tableau_utilities/tableau_file/tableau_file.py
--rw-r--r--   0 justin     (502) staff       (20)    37752 2023-07-25 18:33:34.000000 tableau_utilities-2.0.62/tableau_utilities/tableau_file/tableau_file_objects.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.834051 tableau_utilities-2.0.62/tableau_utilities/tableau_server/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/tableau_server/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    31778 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/tableau_server/tableau_server.py
--rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.0.62/tableau_utilities/tableau_server/tableau_server_objects.py
--rw-r--r--   0 justin     (502) staff       (20)    10765 2023-07-10 18:39:33.000000 tableau_utilities-2.0.62/tableau_utilities/test_tableau_utilities.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-25 18:34:00.818767 tableau_utilities-2.0.62/tableau_utilities.egg-info/
--rw-r--r--   0 justin     (502) staff       (20)     8421 2023-07-25 18:34:00.000000 tableau_utilities-2.0.62/tableau_utilities.egg-info/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     1205 2023-07-25 18:34:00.000000 tableau_utilities-2.0.62/tableau_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 justin     (502) staff       (20)        1 2023-07-25 18:34:00.000000 tableau_utilities-2.0.62/tableau_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 justin     (502) staff       (20)       73 2023-07-25 18:34:00.000000 tableau_utilities-2.0.62/tableau_utilities.egg-info/entry_points.txt
--rw-r--r--   0 justin     (502) staff       (20)      112 2023-07-25 18:34:00.000000 tableau_utilities-2.0.62/tableau_utilities.egg-info/requires.txt
--rw-r--r--   0 justin     (502) staff       (20)       18 2023-07-25 18:34:00.000000 tableau_utilities-2.0.62/tableau_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-27 17:52:26.579574 tableau_utilities-2.0.63/
+-rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.0.63/LICENSE
+-rw-r--r--   0 justin     (502) staff       (20)     8421 2023-07-27 17:52:26.579002 tableau_utilities-2.0.63/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     8116 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/README.md
+-rw-r--r--   0 justin     (502) staff       (20)       38 2023-07-27 17:52:26.579753 tableau_utilities-2.0.63/setup.cfg
+-rw-r--r--   0 justin     (502) staff       (20)     1108 2023-07-27 17:51:54.000000 tableau_utilities-2.0.63/setup.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-27 17:52:26.560172 tableau_utilities-2.0.63/tableau_utilities/
+-rw-r--r--   0 justin     (502) staff       (20)      272 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2441 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/fetch_all_cols.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-27 17:52:26.565697 tableau_utilities-2.0.63/tableau_utilities/general/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/general/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/general/cli_styling.py
+-rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/general/config_column_persona.py
+-rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/general/funcs.py
+-rw-r--r--   0 justin     (502) staff       (20)     2874 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/scripted_testing.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-27 17:52:26.571642 tableau_utilities-2.0.63/tableau_utilities/scripts/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/scripts/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    23247 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/scripts/cli.py
+-rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/scripts/csv_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     7863 2023-07-25 18:33:34.000000 tableau_utilities-2.0.63/tableau_utilities/scripts/datasource.py
+-rw-r--r--   0 justin     (502) staff       (20)    13151 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/scripts/gen_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/scripts/merge_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     1867 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/scripts/server_info.py
+-rw-r--r--   0 justin     (502) staff       (20)     4531 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/scripts/server_operate.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-27 17:52:26.574275 tableau_utilities-2.0.63/tableau_utilities/tableau_file/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/tableau_file/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    13627 2023-07-27 17:51:54.000000 tableau_utilities-2.0.63/tableau_utilities/tableau_file/tableau_file.py
+-rw-r--r--   0 justin     (502) staff       (20)    37752 2023-07-25 18:33:34.000000 tableau_utilities-2.0.63/tableau_utilities/tableau_file/tableau_file_objects.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-27 17:52:26.577700 tableau_utilities-2.0.63/tableau_utilities/tableau_server/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/tableau_server/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    31778 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/tableau_server/tableau_server.py
+-rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.0.63/tableau_utilities/tableau_server/tableau_server_objects.py
+-rw-r--r--   0 justin     (502) staff       (20)    10765 2023-07-10 18:39:33.000000 tableau_utilities-2.0.63/tableau_utilities/test_tableau_utilities.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2023-07-27 17:52:26.563597 tableau_utilities-2.0.63/tableau_utilities.egg-info/
+-rw-r--r--   0 justin     (502) staff       (20)     8421 2023-07-27 17:52:26.000000 tableau_utilities-2.0.63/tableau_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     1205 2023-07-27 17:52:26.000000 tableau_utilities-2.0.63/tableau_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 justin     (502) staff       (20)        1 2023-07-27 17:52:26.000000 tableau_utilities-2.0.63/tableau_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 justin     (502) staff       (20)       73 2023-07-27 17:52:26.000000 tableau_utilities-2.0.63/tableau_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 justin     (502) staff       (20)      112 2023-07-27 17:52:26.000000 tableau_utilities-2.0.63/tableau_utilities.egg-info/requires.txt
+-rw-r--r--   0 justin     (502) staff       (20)       18 2023-07-27 17:52:26.000000 tableau_utilities-2.0.63/tableau_utilities.egg-info/top_level.txt
```

### Comparing `tableau_utilities-2.0.62/LICENSE` & `tableau_utilities-2.0.63/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/PKG-INFO` & `tableau_utilities-2.0.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau_utilities
-Version: 2.0.62
+Version: 2.0.63
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tableau_utilities-2.0.62/README.md` & `tableau_utilities-2.0.63/README.md`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/setup.py` & `tableau_utilities-2.0.63/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     author_email="justin.grilli@gmail.com",
     license='MIT',
     url='http://pypi.python.org/pypi/tableau-utilities/',
     description='Utility for maintaining Tableau objects',
     long_description=readme,
     long_description_content_type='text/markdown',
     name="tableau_utilities",
-    version="2.0.62",
+    version="2.0.63",
     packages=[
         'tableau_utilities',
         'tableau_utilities.general',
         'tableau_utilities.tableau_file',
         'tableau_utilities.tableau_server',
         'tableau_utilities.scripts'
     ],
```

### Comparing `tableau_utilities-2.0.62/tableau_utilities/fetch_all_cols.py` & `tableau_utilities-2.0.63/tableau_utilities/fetch_all_cols.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/general/cli_styling.py` & `tableau_utilities-2.0.63/tableau_utilities/general/cli_styling.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/general/config_column_persona.py` & `tableau_utilities-2.0.63/tableau_utilities/general/config_column_persona.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/general/funcs.py` & `tableau_utilities-2.0.63/tableau_utilities/general/funcs.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/scripted_testing.py` & `tableau_utilities-2.0.63/tableau_utilities/scripted_testing.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/scripts/cli.py` & `tableau_utilities-2.0.63/tableau_utilities/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/scripts/csv_config.py` & `tableau_utilities-2.0.63/tableau_utilities/scripts/csv_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/scripts/datasource.py` & `tableau_utilities-2.0.63/tableau_utilities/scripts/datasource.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/scripts/gen_config.py` & `tableau_utilities-2.0.63/tableau_utilities/scripts/gen_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/scripts/merge_config.py` & `tableau_utilities-2.0.63/tableau_utilities/scripts/merge_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/scripts/server_info.py` & `tableau_utilities-2.0.63/tableau_utilities/scripts/server_info.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/scripts/server_operate.py` & `tableau_utilities-2.0.63/tableau_utilities/scripts/server_operate.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/tableau_file/tableau_file.py` & `tableau_utilities-2.0.63/tableau_utilities/tableau_file/tableau_file.py`

 * *Files 18% similar despite different names*

```diff
@@ -201,14 +201,15 @@
         """
         # Add Column
         if column not in self.columns:
             self.columns.add(column)
         # Update the Column
         else:
             self.columns.update(column)
+
         # Add Folder / FolderItem for the column, if folder_name was provided
         if folder_name:
             # Remove the column's folder-item for preview folder, if it will be moved to a new folder
             current_folder = [f for f in self.folders_common.folder if f.folder_item.get(column.name)]
             if current_folder and current_folder[0].name != folder_name:
                 current_folder[0].folder_item.delete(column.name)
                 self.folders_common.folder.update(current_folder[0])
@@ -216,33 +217,62 @@
             folder = self.folders_common.folder.get(folder_name)
             folder_item = tfo.FolderItem(name=column.name)
             if folder and folder_item not in folder.folder_item:
                 folder.folder_item.append(folder_item)
                 self.folders_common.folder.update(folder)
             elif not folder:
                 self.folders_common.folder.add(tfo.Folder(name=folder_name, folder_item=[folder_item]))
+
         # If a remote_name was provided, and the column is not a Tableau Calculation - enforce metadata
-        if remote_name and not column.calculation:
-            # Update MetadataRecords
-            datasource_record = self.connection.metadata_records.get(remote_name)
-            datasource_record.local_name = column.name
-            self.connection.metadata_records.update(datasource_record)
-            extract_record = self.extract.connection.metadata_records.get(remote_name) if self.extract else None
-            if extract_record:
-                extract_record.local_name = column.name
-                self.extract.connection.metadata_records.update(extract_record)
-            # Update MappingCols
-            if column.name not in self.connection.cols:
-                self.connection.cols.append(
-                    tfo.MappingCol(key=column.name, value=f'{datasource_record.parent_name}.[{remote_name}]')
-                )
-            if extract_record and column.name not in self.extract.connection.cols:
-                self.extract.connection.cols.append(
-                    tfo.MappingCol(key=column.name, value=f'{extract_record.parent_name}.[{remote_name}]')
-                )
+        if not remote_name or column.calculation:
+            return None
+
+        # Update Connection MetadataRecords & MappingCols
+        connection_record = self.connection.metadata_records.get(remote_name)
+        if not connection_record:
+            raise TableauFileError(f'Remote name provided is not in the metadata of the connection: {remote_name}')
+        connection_record.local_name = column.name
+        self.connection.metadata_records.update(connection_record)
+        # Update Connection MappingCols
+        if column.name not in self.connection.cols:
+            # Delete existing mapping for the remote_name
+            existing_mapped_remote_col = None
+            for col in self.connection.cols:
+                col_remote_name = col.value.split('.')[0][1:-1]
+                if col_remote_name == remote_name:
+                    existing_mapped_remote_col = col
+            if existing_mapped_remote_col:
+                self.connection.cols.delete(existing_mapped_remote_col)
+            # Add Connection MappingCol
+            self.connection.cols.append(
+                tfo.MappingCol(key=column.name, value=f'{connection_record.parent_name}.[{remote_name}]')
+            )
+
+        # Update Extract MetadataRecords & MappingCols
+        if not self.extract:
+            return None
+        extract_record = self.extract.connection.metadata_records.get(remote_name)
+        if not extract_record:
+            raise TableauFileError(f'Remote name provided is not in the metadata of the extract: {remote_name}')
+        extract_record.local_name = column.name
+        self.extract.connection.metadata_records.update(extract_record)
+        # Update Extract MappingCols
+        if column.name not in self.extract.connection.cols:
+            # Delete existing mapping for the remote_name
+            existing_mapped_remote_col = None
+            for col in self.extract.connection.cols:
+                col_remote_name = col.value.split('.')[0][1:-1]
+                if col_remote_name == remote_name:
+                    existing_mapped_remote_col = col
+            if existing_mapped_remote_col:
+                self.extract.connection.cols.delete(existing_mapped_remote_col)
+            # Add Extract MappingCol
+            self.extract.connection.cols.append(
+                tfo.MappingCol(key=column.name, value=f'{extract_record.parent_name}.[{remote_name}]')
+            )
 
     def save(self):
         """ Save all changes made to each section of the Datasource """
         parent = self._root.find('.')
         ending_index = -1
         for section in self.sections():
             if not section:
```

### Comparing `tableau_utilities-2.0.62/tableau_utilities/tableau_file/tableau_file_objects.py` & `tableau_utilities-2.0.63/tableau_utilities/tableau_file/tableau_file_objects.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/tableau_server/tableau_server.py` & `tableau_utilities-2.0.63/tableau_utilities/tableau_server/tableau_server.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/tableau_server/tableau_server_objects.py` & `tableau_utilities-2.0.63/tableau_utilities/tableau_server/tableau_server_objects.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities/test_tableau_utilities.py` & `tableau_utilities-2.0.63/tableau_utilities/test_tableau_utilities.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.0.62/tableau_utilities.egg-info/PKG-INFO` & `tableau_utilities-2.0.63/tableau_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableau-utilities
-Version: 2.0.62
+Version: 2.0.63
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tableau_utilities-2.0.62/tableau_utilities.egg-info/SOURCES.txt` & `tableau_utilities-2.0.63/tableau_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

