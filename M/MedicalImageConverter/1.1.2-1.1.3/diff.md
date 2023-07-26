# Comparing `tmp/MedicalImageConverter-1.1.2.tar.gz` & `tmp/MedicalImageConverter-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MedicalImageConverter-1.1.2.tar", last modified: Sun Jul 23 20:36:47 2023, max compression
+gzip compressed data, was "MedicalImageConverter-1.1.3.tar", last modified: Wed Jul 26 23:19:28 2023, max compression
```

## Comparing `MedicalImageConverter-1.1.2.tar` & `MedicalImageConverter-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 20:36:47.958167 MedicalImageConverter-1.1.2/
--rw-rw-rw-   0        0        0    35821 2023-07-22 22:51:40.000000 MedicalImageConverter-1.1.2/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-07-23 20:36:47.915709 MedicalImageConverter-1.1.2/MedicalImageConverter/
--rw-rw-rw-   0        0        0      102 2023-07-23 20:35:17.000000 MedicalImageConverter-1.1.2/MedicalImageConverter/__init__.py
--rw-rw-rw-   0        0        0      682 2023-07-23 17:43:51.000000 MedicalImageConverter-1.1.2/MedicalImageConverter/memory.py
--rw-rw-rw-   0        0        0     1281 2023-07-23 17:43:46.000000 MedicalImageConverter-1.1.2/MedicalImageConverter/parsar.py
--rw-rw-rw-   0        0        0    22985 2023-07-23 17:43:58.000000 MedicalImageConverter-1.1.2/MedicalImageConverter/reader.py
-drwxrwxrwx   0        0        0        0 2023-07-23 20:36:47.958167 MedicalImageConverter-1.1.2/MedicalImageConverter.egg-info/
--rw-rw-rw-   0        0        0     4828 2023-07-23 20:36:47.000000 MedicalImageConverter-1.1.2/MedicalImageConverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-23 20:36:47.000000 MedicalImageConverter-1.1.2/MedicalImageConverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 20:36:47.000000 MedicalImageConverter-1.1.2/MedicalImageConverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-23 20:36:47.000000 MedicalImageConverter-1.1.2/MedicalImageConverter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4828 2023-07-23 20:36:47.965752 MedicalImageConverter-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4339 2023-07-23 00:28:45.000000 MedicalImageConverter-1.1.2/README.md
--rw-rw-rw-   0        0        0       97 2023-07-23 20:12:24.000000 MedicalImageConverter-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      594 2023-07-23 20:36:47.969566 MedicalImageConverter-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 23:19:28.870419 MedicalImageConverter-1.1.3/
+-rw-rw-rw-   0        0        0    35821 2023-07-22 22:51:40.000000 MedicalImageConverter-1.1.3/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 23:19:28.820082 MedicalImageConverter-1.1.3/MedicalImageConverter/
+-rw-rw-rw-   0        0        0      102 2023-07-23 20:35:17.000000 MedicalImageConverter-1.1.3/MedicalImageConverter/__init__.py
+-rw-rw-rw-   0        0        0      690 2023-07-26 23:11:11.000000 MedicalImageConverter-1.1.3/MedicalImageConverter/memory.py
+-rw-rw-rw-   0        0        0     1283 2023-07-26 23:12:09.000000 MedicalImageConverter-1.1.3/MedicalImageConverter/parsar.py
+-rw-rw-rw-   0        0        0    24131 2023-07-26 23:10:52.000000 MedicalImageConverter-1.1.3/MedicalImageConverter/reader.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:19:28.863791 MedicalImageConverter-1.1.3/MedicalImageConverter.egg-info/
+-rw-rw-rw-   0        0        0     4828 2023-07-26 23:19:28.000000 MedicalImageConverter-1.1.3/MedicalImageConverter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-07-26 23:19:28.000000 MedicalImageConverter-1.1.3/MedicalImageConverter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 23:19:28.000000 MedicalImageConverter-1.1.3/MedicalImageConverter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 23:19:28.000000 MedicalImageConverter-1.1.3/MedicalImageConverter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4828 2023-07-26 23:19:28.874058 MedicalImageConverter-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4339 2023-07-23 00:28:45.000000 MedicalImageConverter-1.1.3/README.md
+-rw-rw-rw-   0        0        0       97 2023-07-23 20:12:24.000000 MedicalImageConverter-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      594 2023-07-26 23:19:28.876348 MedicalImageConverter-1.1.3/setup.cfg
```

### Comparing `MedicalImageConverter-1.1.2/LICENSE.txt` & `MedicalImageConverter-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MedicalImageConverter-1.1.2/MedicalImageConverter/memory.py` & `MedicalImageConverter-1.1.3/MedicalImageConverter/memory.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import psutil
 
 
 def check_memory(file_dictionary):
     dicom_size = 0
     for file in file_dictionary['Dicom']:
         dicom_size = dicom_size + os.path.getsize(file)
-
+        
     raw_size = 0
     for file in file_dictionary['Raw']:
         raw_size = raw_size + os.path.getsize(file)
 
     stl_size = 0
     for file in file_dictionary['Stl']:
         stl_size = stl_size + os.path.getsize(file)
```

### Comparing `MedicalImageConverter-1.1.2/MedicalImageConverter/parsar.py` & `MedicalImageConverter-1.1.3/MedicalImageConverter/parsar.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     raw_files = []
     stl_files = []
 
     for root, dirs, files in os.walk(path):
         if files:
             for name in files:
                 filepath = os.path.join(root, name)
+
                 if filepath not in exclude_files:
                     filename, file_extension = os.path.splitext(filepath)
 
                     if file_extension == '.dcm':
                         dicom_files.append(filepath)
 
                     elif file_extension == '.mhd':
```

### Comparing `MedicalImageConverter-1.1.2/MedicalImageConverter/reader.py` & `MedicalImageConverter-1.1.3/MedicalImageConverter/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 import time
 from multiprocessing import Pool
 
 import cv2
 import numpy as np
 import pandas as pd
 import pydicom as dicom
+import SimpleITK as sitk
 
 
 def multi_process_dicom(path):
     """
     Uses pydicom to read in dicom files.
 
     Parameters
@@ -70,19 +71,20 @@
         self.ds_images = []
         self.ds_dictionary = dict.fromkeys(['CT', 'MR', 'PT', 'US', 'DX', 'MG', 'NM', 'XA', 'CR', 'RTSTRUCT'])
         self.rt_df = pd.DataFrame(columns=['FilePath', 'SeriesInstanceUID', 'RoiSOP', 'RoiNames'])
 
         keep_tags = ['FilePath', 'SOPInstanceUID', 'PatientID', 'PatientName', 'Modality',
                      'SeriesDescription', 'SeriesDate', 'SeriesTime', 'SeriesInstanceUID', 'SeriesNumber',
                      'AcquisitionNumber', 'SliceThickness', 'PixelSpacing', 'Rows', 'Columns', 'ImagePositionPatient',
-                     'Slices', 'DefaultWindow']
+                     'Slices', 'DefaultWindow', 'FullWindow']
         self.image_info = pd.DataFrame(columns=keep_tags)
         self.image_data = []
 
-        self.roi_info = pd.DataFrame(columns=['FilePath', 'RoiNames', 'PhysicalCoordinates', 'ArrayCoordinates'])
+        self.roi_info = pd.DataFrame(columns=['FilePath', 'RoiNames', 'PhysicalCoordinates', 'ArrayCoordinates',
+                                              'Volume', 'COM'])
         self.roi_data = []
 
     def add_dicom_extension(self):
         """
         Will add .dcm extension to any file inside self.dicom_files that doesn't have an extension
         Returns
         -------
@@ -293,17 +295,14 @@
                             center = image[0].WindowCenter
                             width = image[0].WindowWidth
                             if not isinstance(center, float):
                                 center = center[0]
                             if not isinstance(width, float):
                                 width = width[0]
                             self.image_info.at[ii, t] = [int(center), int(np.round(width/2))]
-
-                    elif image[0].Modality == 'PT':
-                        self.image_info.at[ii, t] = [8000, 8000]
                     elif image[0].Modality == 'US':
                         self.image_info.at[ii, t] = [128, 128]
                     else:
                         self.image_info.at[ii, t] = None
 
                 else:
                     if t in image[0]:
@@ -354,14 +353,18 @@
 
             image_hold = np.asarray(image_slices)
             if len(image_hold.shape) > 3:
                 self.image_data.append(image_hold[0])
             else:
                 self.image_data.append(image_hold)
 
+            image_min = np.min(self.image_data[-1])
+            image_max = np.max(self.image_data[-1])
+            self.image_info.at[ii, 'FullWindow'] = [image_min, image_max]
+
     def create_masks(self):
         """
         existing_image_info is required if the users only loads a RTSTRUCT file, because to make the mask the spacing
         and origin from the CT is needed.
 
         It is pretty gross after that. For a given ROI each contour is read-in, an empty full sized image array is
         created. Using cv2 the contours are converted to a binary slice, then all the slices are combined. To save
@@ -388,14 +391,16 @@
                             float(info.at[ii, 'ImagePositionPatient'][1]),
                             float(info.at[ii, 'ImagePositionPatient'][2])]
 
             rows = int(info.at[ii, 'Rows'])
             columns = int(info.at[ii, 'Columns'])
             slices = len(self.ds_images[ii])
 
+            mask_com = []
+            mask_volume = []
             mask_reduced = []
             roi_filepaths, roi_names = [], []
             physical_coordinates, array_coordinates = [], []
             for jj in range(len(self.rt_df.index)):
                 if img_series == self.rt_df.at[jj, 'SeriesInstanceUID'] and self.rt_df.at[jj, 'RoiSOP'][0] in img_sop:
                     roi_sequence = self.ds_dictionary['RTSTRUCT'][jj].ROIContourSequence
                     for kk, sequence in enumerate(roi_sequence):
@@ -443,28 +448,42 @@
                                 physical_coordinates.append([(region[0]*spacing_array[2]) + corner_array[2],
                                                              (region[2]*spacing_array[1]) + corner_array[1],
                                                              (region[4]*spacing_array[0]) + corner_array[0]])
                                 array_coordinates.append([[region[0], region[1]],
                                                           [region[2], region[3]],
                                                           [region[4], region[5]]])
 
+                                new_mask_sitk = sitk.GetImageFromArray(new_mask)
+                                new_mask_sitk.SetSpacing(spacing_array)
+                                new_mask_sitk.SetOrigin(physical_coordinates[-1])
+
+                                label_statistic = sitk.LabelShapeStatisticsImageFilter()
+                                label_statistic.Execute(new_mask_sitk)
+                                mask_com.append(np.round(label_statistic.GetCentroid(1), 2))
+
+                                volume = np.sum(new_mask) * spacing_array[0] * spacing_array[1] * spacing_array[2]
+                                mask_volume.append(np.round(volume/(10*10*10), 2))
                                 mask_reduced.append(new_mask)
 
             if len(mask_reduced) > 0:
                 self.roi_data.append(mask_reduced)
                 self.roi_info.at[ii, 'FilePath'] = roi_filepaths
                 self.roi_info.at[ii, 'RoiNames'] = roi_names
                 self.roi_info.at[ii, 'PhysicalCoordinates'] = physical_coordinates
                 self.roi_info.at[ii, 'ArrayCoordinates'] = array_coordinates
+                self.roi_info.at[ii, 'Volume'] = mask_volume
+                self.roi_info.at[ii, 'COM'] = mask_com
             else:
                 self.roi_data.append(mask_reduced)
                 self.roi_info.at[ii, 'FilePath'] = None
                 self.roi_info.at[ii, 'RoiNames'] = None
                 self.roi_info.at[ii, 'PhysicalCoordinates'] = None
                 self.roi_info.at[ii, 'ArrayCoordinates'] = None
+                self.roi_info.at[ii, 'Volume'] = None
+                self.roi_info.at[ii, 'COM'] = None
 
     def get_image_info(self):
         return self.image_info
 
     def get_image_data(self):
         return self.image_data
```

### Comparing `MedicalImageConverter-1.1.2/MedicalImageConverter.egg-info/PKG-INFO` & `MedicalImageConverter-1.1.3/MedicalImageConverter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedicalImageConverter
-Version: 1.1.2
+Version: 1.1.3
 Summary: Reads in medical images and converts them into numpy arrays.
 Home-page: https://github.com/caleb-oconnor/MedicalImageConverter
 Author: Caleb OConnor
 Author-email: csoconnor@mdanderson.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.7
```

### Comparing `MedicalImageConverter-1.1.2/PKG-INFO` & `MedicalImageConverter-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedicalImageConverter
-Version: 1.1.2
+Version: 1.1.3
 Summary: Reads in medical images and converts them into numpy arrays.
 Home-page: https://github.com/caleb-oconnor/MedicalImageConverter
 Author: Caleb OConnor
 Author-email: csoconnor@mdanderson.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.7
```

### Comparing `MedicalImageConverter-1.1.2/README.md` & `MedicalImageConverter-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `MedicalImageConverter-1.1.2/setup.cfg` & `MedicalImageConverter-1.1.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204d 6564 6963 616c 496d 6167 6543   = MedicalImageC
 00000020: 6f6e 7665 7274 6572 0d0a 7665 7273 696f  onverter..versio
-00000030: 6e20 3d20 312e 312e 320d 0a61 7574 686f  n = 1.1.2..autho
+00000030: 6e20 3d20 312e 312e 330d 0a61 7574 686f  n = 1.1.3..autho
 00000040: 7220 3d20 4361 6c65 6220 4f43 6f6e 6e6f  r = Caleb OConno
 00000050: 720d 0a61 7574 686f 725f 656d 6169 6c20  r..author_email 
 00000060: 3d20 6373 6f63 6f6e 6e6f 7240 6d64 616e  = csoconnor@mdan
 00000070: 6465 7273 6f6e 2e6f 7267 0d0a 6465 7363  derson.org..desc
 00000080: 7269 7074 696f 6e20 3d20 5265 6164 7320  ription = Reads 
 00000090: 696e 206d 6564 6963 616c 2069 6d61 6765  in medical image
 000000a0: 7320 616e 6420 636f 6e76 6572 7473 2074  s and converts t
```

