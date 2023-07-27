# Comparing `tmp/falconz-2.0.0.tar.gz` & `tmp/falconz-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falconz-2.0.0.tar", last modified: Thu Jul 27 08:40:43 2023, max compression
+gzip compressed data, was "falconz-2.0.1.tar", last modified: Thu Jul 27 08:46:58 2023, max compression
```

## Comparing `falconz-2.0.0.tar` & `falconz-2.0.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 08:40:43.957790 falconz-2.0.0/
--rw-rw-r--   0 lalith    (1000) lalith    (1000)    35149 2023-04-13 18:52:14.000000 falconz-2.0.0/LICENSE
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     1745 2023-07-27 08:40:43.957790 falconz-2.0.0/PKG-INFO
--rw-rw-r--   0 lalith    (1000) lalith    (1000)    13478 2023-07-24 13:59:38.000000 falconz-2.0.0/README.md
-drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 08:40:43.957790 falconz-2.0.0/falconz/
--rw-rw-r--   0 lalith    (1000) lalith    (1000)      129 2023-07-24 14:25:30.000000 falconz-2.0.0/falconz/__init__.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     1503 2023-07-24 14:45:10.000000 falconz-2.0.0/falconz/constants.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     2781 2023-07-24 14:45:10.000000 falconz-2.0.0/falconz/display.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     4178 2023-07-24 14:11:52.000000 falconz-2.0.0/falconz/download.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     5437 2023-07-25 09:35:07.000000 falconz-2.0.0/falconz/falconz.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     4260 2023-07-24 14:13:23.000000 falconz-2.0.0/falconz/file_utilities.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     7640 2023-07-24 14:16:10.000000 falconz-2.0.0/falconz/image_conversion.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     7229 2023-07-27 08:40:14.000000 falconz-2.0.0/falconz/image_processing.py
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     1669 2023-07-24 14:12:34.000000 falconz-2.0.0/falconz/resources.py
-drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 08:40:43.957790 falconz-2.0.0/falconz.egg-info/
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     1745 2023-07-27 08:40:43.000000 falconz-2.0.0/falconz.egg-info/PKG-INFO
--rw-rw-r--   0 lalith    (1000) lalith    (1000)      416 2023-07-27 08:40:43.000000 falconz-2.0.0/falconz.egg-info/SOURCES.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)        1 2023-07-27 08:40:43.000000 falconz-2.0.0/falconz.egg-info/dependency_links.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)       50 2023-07-27 08:40:43.000000 falconz-2.0.0/falconz.egg-info/entry_points.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)      241 2023-07-27 08:40:43.000000 falconz-2.0.0/falconz.egg-info/requires.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)        8 2023-07-27 08:40:43.000000 falconz-2.0.0/falconz.egg-info/top_level.txt
--rw-rw-r--   0 lalith    (1000) lalith    (1000)       38 2023-07-27 08:40:43.957790 falconz-2.0.0/setup.cfg
--rw-rw-r--   0 lalith    (1000) lalith    (1000)     2654 2023-07-24 14:26:24.000000 falconz-2.0.0/setup.py
+drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 08:46:58.788508 falconz-2.0.1/
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)    35149 2023-04-13 18:52:14.000000 falconz-2.0.1/LICENSE
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     1745 2023-07-27 08:46:58.788508 falconz-2.0.1/PKG-INFO
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)    13478 2023-07-24 13:59:38.000000 falconz-2.0.1/README.md
+drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 08:46:58.788508 falconz-2.0.1/falconz/
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      129 2023-07-24 14:25:30.000000 falconz-2.0.1/falconz/__init__.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     1503 2023-07-24 14:45:10.000000 falconz-2.0.1/falconz/constants.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     2781 2023-07-24 14:45:10.000000 falconz-2.0.1/falconz/display.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     4178 2023-07-24 14:11:52.000000 falconz-2.0.1/falconz/download.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     5437 2023-07-25 09:35:07.000000 falconz-2.0.1/falconz/falconz.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     4260 2023-07-24 14:13:23.000000 falconz-2.0.1/falconz/file_utilities.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     9000 2023-07-27 08:45:54.000000 falconz-2.0.1/falconz/image_conversion.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)    10481 2023-07-27 08:44:11.000000 falconz-2.0.1/falconz/image_processing.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      687 2023-07-27 08:42:24.000000 falconz-2.0.1/falconz/input_validation.py
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     1669 2023-07-24 14:12:34.000000 falconz-2.0.1/falconz/resources.py
+drwxrwxr-x   0 lalith    (1000) lalith    (1000)        0 2023-07-27 08:46:58.788508 falconz-2.0.1/falconz.egg-info/
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     1745 2023-07-27 08:46:58.000000 falconz-2.0.1/falconz.egg-info/PKG-INFO
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      444 2023-07-27 08:46:58.000000 falconz-2.0.1/falconz.egg-info/SOURCES.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)        1 2023-07-27 08:46:58.000000 falconz-2.0.1/falconz.egg-info/dependency_links.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)       50 2023-07-27 08:46:58.000000 falconz-2.0.1/falconz.egg-info/entry_points.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)      241 2023-07-27 08:46:58.000000 falconz-2.0.1/falconz.egg-info/requires.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)        8 2023-07-27 08:46:58.000000 falconz-2.0.1/falconz.egg-info/top_level.txt
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)       38 2023-07-27 08:46:58.788508 falconz-2.0.1/setup.cfg
+-rw-rw-r--   0 lalith    (1000) lalith    (1000)     2654 2023-07-27 08:46:55.000000 falconz-2.0.1/setup.py
```

### Comparing `falconz-2.0.0/LICENSE` & `falconz-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `falconz-2.0.0/PKG-INFO` & `falconz-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falconz
-Version: 2.0.0
+Version: 2.0.1
 Summary: FalconZ: A streamlined Python package for PET motion correction.
 Home-page: https://github.com/QIMP-Team/FALCON
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: PET motion correction,diffeomorphic imaging,image processing
 Platform: UNKNOWN
```

### Comparing `falconz-2.0.0/README.md` & `falconz-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `falconz-2.0.0/falconz/constants.py` & `falconz-2.0.1/falconz/constants.py`

 * *Files identical despite different names*

### Comparing `falconz-2.0.0/falconz/display.py` & `falconz-2.0.1/falconz/display.py`

 * *Files identical despite different names*

### Comparing `falconz-2.0.0/falconz/download.py` & `falconz-2.0.1/falconz/download.py`

 * *Files identical despite different names*

### Comparing `falconz-2.0.0/falconz/falconz.py` & `falconz-2.0.1/falconz/falconz.py`

 * *Files identical despite different names*

### Comparing `falconz-2.0.0/falconz/file_utilities.py` & `falconz-2.0.1/falconz/file_utilities.py`

 * *Files identical despite different names*

### Comparing `falconz-2.0.0/falconz/image_conversion.py` & `falconz-2.0.1/falconz/image_conversion.py`

 * *Files 10% similar despite different names*

```diff
@@ -193,8 +193,39 @@
                 # create the new filename
                 new_filename = f"{modality}_{filename}"
 
                 # rename the file
                 os.rename(os.path.join(nifti_dir, filename), os.path.join(nifti_dir, new_filename))
 
                 # delete the old name from the dictionary
-                del dicom_info[filename]
+                del dicom_info[filename]
+
+
+def split4d(nifti_file: str, out_dir: str) -> None:
+    """Split a 4D NIFTI file into 3D NIFTI files using nibabel
+    :param nifti_file: 4D NIFTI file to split
+    :param out_dir: Directory to save the split NIFTI files
+    """
+    logging.info(f"Splitting {nifti_file} into 3D nifti files")
+    spinner = Halo(text=f"Splitting {nifti_file} into 3D nifti files", spinner='dots')
+    spinner.start()
+    split_nifti_files = nib.funcs.four_to_three(nib.funcs.squeeze_image(nib.load(nifti_file)))
+    i = 0
+    for file in split_nifti_files:
+        nib.save(file, os.path.join(out_dir, 'vol' + str(i).zfill(4) + '.nii.gz'))
+        i += 1
+    logging.info(f"Splitting done and split files are saved in {out_dir}")
+    spinner.succeed()
+
+
+def merge3d(nifti_dir: str, wild_card: str, nifti_outfile: str) -> None:
+    """
+    Merge 3D NIFTI files into a 4D NIFTI file using nibabel
+    :param nifti_dir: Directory containing the 3D NIFTI files
+    :param wild_card: Wildcard to use to find the 3D NIFTI files
+    :param nifti_outfile: User-defined output file name for the 4D NIFTI file
+    """
+    logging.info(f"Merging 3D nifti files in {nifti_dir} with wildcard {wild_card}")
+    files_to_merge = fop.get_files(nifti_dir, wild_card)
+    nib.save(nib.funcs.concat_images(files_to_merge, False), nifti_outfile)
+    os.chdir(nifti_dir)
+    logging.info("Done")
```

### Comparing `falconz-2.0.0/falconz/resources.py` & `falconz-2.0.1/falconz/resources.py`

 * *Files identical despite different names*

### Comparing `falconz-2.0.0/falconz.egg-info/PKG-INFO` & `falconz-2.0.1/falconz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falconz
-Version: 2.0.0
+Version: 2.0.1
 Summary: FalconZ: A streamlined Python package for PET motion correction.
 Home-page: https://github.com/QIMP-Team/FALCON
 Author: Lalith Kumar Shiyam Sundar
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: PET motion correction,diffeomorphic imaging,image processing
 Platform: UNKNOWN
```

### Comparing `falconz-2.0.0/setup.py` & `falconz-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falconz',
-    version='2.0.0',
+    version='2.0.1',
     author='Lalith Kumar Shiyam Sundar',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='FalconZ: A streamlined Python package for PET motion correction.',
     python_requires='>=3.9',
     long_description='FalconZ is a robust and comprehensive Python package that offers a simplified approach to PET ('
                      'Positron Emission Tomography) motion correction. The software is equipped to handle both head '
                      'and total-body scans, ensuring high-accuracy results in diverse settings. Built around the '
```

