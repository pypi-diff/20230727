# Comparing `tmp/filelistener-1.0.2.tar.gz` & `tmp/filelistener-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filelistener-1.0.2.tar", last modified: Tue Jul 25 18:29:36 2023, max compression
+gzip compressed data, was "filelistener-1.0.3.tar", last modified: Thu Jul 27 05:11:17 2023, max compression
```

## Comparing `filelistener-1.0.2.tar` & `filelistener-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 18:29:36.428695 filelistener-1.0.2/
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 18:29:36.417344 filelistener-1.0.2/Content/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:49:10.000000 filelistener-1.0.2/Content/__init__.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     6429 2023-07-25 18:27:52.000000 filelistener-1.0.2/Content/duplicate_content.py
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 18:29:36.419778 filelistener-1.0.2/Content/modules/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:10:47.000000 filelistener-1.0.2/Content/modules/__init__.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     1563 2023-07-21 04:19:28.000000 filelistener-1.0.2/Content/modules/duplicate_zip_files.py
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-25 18:29:36.426759 filelistener-1.0.2/PKG-INFO
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      421 2023-07-25 17:46:19.000000 filelistener-1.0.2/README.md
-drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-25 18:29:36.425536 filelistener-1.0.2/filelistener.egg-info/
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-25 18:29:36.000000 filelistener-1.0.2/filelistener.egg-info/PKG-INFO
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      352 2023-07-25 18:29:36.000000 filelistener-1.0.2/filelistener.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        1 2023-07-25 18:29:36.000000 filelistener-1.0.2/filelistener.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       58 2023-07-25 18:29:36.000000 filelistener-1.0.2/filelistener.egg-info/entry_points.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        9 2023-07-25 18:29:36.000000 filelistener-1.0.2/filelistener.egg-info/requires.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        8 2023-07-25 18:29:36.000000 filelistener-1.0.2/filelistener.egg-info/top_level.txt
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       38 2023-07-25 18:29:36.429147 filelistener-1.0.2/setup.cfg
--rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      496 2023-07-25 18:29:32.000000 filelistener-1.0.2/setup.py
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:11:17.906144 filelistener-1.0.3/
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:11:17.891856 filelistener-1.0.3/Content/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     8054 2023-07-27 05:02:56.000000 filelistener-1.0.3/Content/duplicate_content.py
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:11:17.895515 filelistener-1.0.3/Content/modules/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-21 04:10:47.000000 filelistener-1.0.3/Content/modules/__init__.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)     1453 2023-07-27 05:09:32.000000 filelistener-1.0.3/Content/modules/duplicate_zip_files.py
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-27 05:11:17.903031 filelistener-1.0.3/PKG-INFO
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      500 2023-07-27 05:06:29.000000 filelistener-1.0.3/README.md
+drwxr-xr-x   0 rishabhsplayarea   (501) staff       (20)        0 2023-07-27 05:11:17.901993 filelistener-1.0.3/filelistener.egg-info/
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      231 2023-07-27 05:11:17.000000 filelistener-1.0.3/filelistener.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      332 2023-07-27 05:11:17.000000 filelistener-1.0.3/filelistener.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        1 2023-07-27 05:11:17.000000 filelistener-1.0.3/filelistener.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       58 2023-07-27 05:11:17.000000 filelistener-1.0.3/filelistener.egg-info/entry_points.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        9 2023-07-27 05:11:17.000000 filelistener-1.0.3/filelistener.egg-info/requires.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)        1 2023-07-27 05:11:17.000000 filelistener-1.0.3/filelistener.egg-info/top_level.txt
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)       38 2023-07-27 05:11:17.906459 filelistener-1.0.3/setup.cfg
+-rw-r--r--   0 rishabhsplayarea   (501) staff       (20)      496 2023-07-27 05:10:41.000000 filelistener-1.0.3/setup.py
```

### Comparing `filelistener-1.0.2/Content/duplicate_content.py` & `filelistener-1.0.3/Content/duplicate_content.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import argparse
 import platform
 import subprocess
 from collections import defaultdict
-from Content.modules.duplicate_zip_files import print_duplicate_zip_files
+from modules.duplicate_zip_files import check_single_zip_for_duplicates
 
 
 def get_file_hash(file_path):
     """Calculate the MD5 hash of a file.
 
     Args:
         file_path (str): The path to the file.
@@ -88,28 +88,55 @@
             if len(file_paths) > 1:
                 print(f"Duplicate files with hash {file_hash}:")
                 for file_path in file_paths:
                     print(file_path)
                 print()
 
     return duplicate_files
+
+def print_duplicate_zip_files(folder_path, calculate_sizes):
+    """Print duplicate files in zip archives in the specified folder."""
+    # Traverse through the folder and its subdirectories
+    for root, dirs, files in os.walk(folder_path):
+        for file_name in files:
+            file_path = os.path.join(root, file_name)
+
+            if file_name.endswith('.zip'):
+                duplicate_file_paths = check_single_zip_for_duplicates(file_path)
+                if duplicate_file_paths:
+                    print(f"Duplicate files in {file_name}:")
+                    for duplicate_file_path in duplicate_file_paths:
+                        print(duplicate_file_path)
+                    print()
+                else:
+                    print(f"No duplicates in {file_name}")
+                    print()
+
+        for subfolder in dirs:
+            subfolder_path = os.path.join(root, subfolder)
+            check_files_in_folder(subfolder_path, calculate_sizes)  # Recursive call to check files in nested folder
+
     
 def main():
     parser = argparse.ArgumentParser(description='Check for duplicate files in a folder.')
     parser.add_argument('-f', '--folder', required=True, help='Path to the folder')
     parser.add_argument('-d', '--delete', action='store_true', help='Flag to enable deletion of duplicates')
+    parser.add_argument('-o', '--output', help='Output file path to save the duplicates in TSV format')
+
     args = parser.parse_args()
 
     folder_path = args.folder
     enable_delete = args.delete
+    output_file = args.output
+    calculate_sizes = True  # Set calculate_sizes to True by default
 
     duplicate_files = check_files_in_folder(folder_path)
 
     # After checking for duplicate files in the folder, print duplicate zip files
-    print_duplicate_zip_files(folder_path)
+    print_duplicate_zip_files(folder_path, calculate_sizes)
 
     found_duplicates = False
     duplicates_to_print = set()
     for size, hash_dict in duplicate_files.items():
         for file_hash, file_info_list in hash_dict.items():
             if file_hash == 'file_paths':
                 continue
@@ -144,11 +171,18 @@
                 print("\033[32mDeletion canceled. Duplicates are still available.\033[0m")
         else:
             print("\033[32mDuplicates are still available.\033[0m")
 
     if enable_delete and not found_duplicates:
         print("\033[33mNo duplicates found. Nothing to delete.\033[0m")
 
+        # Save duplicates info to the output file in TSV format if provided
+    if output_file and duplicates_to_print:
+        with open(output_file, 'w') as f:
+            f.write("Name\tAbsolute Path\n")
+            for file_name in sorted(duplicates_to_print):
+                file_path = os.path.join(folder_path, file_name)
+                f.write(f"{file_name}\t{file_path}\n")
+
 
 if __name__ == '__main__':
     main()
-
```

