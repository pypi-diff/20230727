# Comparing `tmp/scikeo-0.2.13.tar.gz` & `tmp/scikeo-0.2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikeo-0.2.13.tar", last modified: Mon Jun 26 18:09:08 2023, max compression
+gzip compressed data, was "scikeo-0.2.15.tar", last modified: Thu Jul 27 16:36:32 2023, max compression
```

## Comparing `scikeo-0.2.13.tar` & `scikeo-0.2.15.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 18:09:08.510575 scikeo-0.2.13/
--rw-rw-rw-   0        0        0      613 2023-06-26 18:09:00.000000 scikeo-0.2.13/LICENSE
--rw-rw-rw-   0        0        0      130 2023-06-26 18:09:00.000000 scikeo-0.2.13/MANIFEST.in
--rw-rw-rw-   0        0        0     8708 2023-06-26 18:09:08.510575 scikeo-0.2.13/PKG-INFO
--rw-rw-rw-   0        0        0     7954 2023-06-26 18:09:00.000000 scikeo-0.2.13/README.md
--rw-rw-rw-   0        0        0       62 2023-06-26 18:09:00.000000 scikeo-0.2.13/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 18:09:08.501800 scikeo-0.2.13/scikeo/
--rw-rw-rw-   0        0        0      143 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/__init__.py
--rw-rw-rw-   0        0        0    10900 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/atmosCorr.py
--rw-rw-rw-   0        0        0     5794 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/calkmeans.py
--rw-rw-rw-   0        0        0    19966 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/calmla.py
--rw-rw-rw-   0        0        0     9941 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/deeplearning.py
--rw-rw-rw-   0        0        0     6113 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/fusionrs.py
--rw-rw-rw-   0        0        0     6668 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/linearTrend.py
--rw-rw-rw-   0        0        0    26407 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/mla.py
--rw-rw-rw-   0        0        0     5043 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/pca.py
--rw-rw-rw-   0        0        0     5789 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/plot.py
--rw-rw-rw-   0        0        0    10580 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/process.py
--rw-rw-rw-   0        0        0     1871 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/rkmeans.py
--rw-rw-rw-   0        0        0     3819 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/sma.py
--rw-rw-rw-   0        0        0     5235 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/tassCap.py
--rw-rw-rw-   0        0        0     2068 2023-06-26 18:09:00.000000 scikeo-0.2.13/scikeo/writeRaster.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:09:08.510575 scikeo-0.2.13/scikeo.egg-info/
--rw-rw-rw-   0        0        0     8708 2023-06-26 18:09:08.000000 scikeo-0.2.13/scikeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-06-26 18:09:08.000000 scikeo-0.2.13/scikeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       56 2023-06-26 18:09:08.000000 scikeo-0.2.13/scikeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-26 18:09:08.000000 scikeo-0.2.13/scikeo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-06-26 18:09:08.000000 scikeo-0.2.13/scikeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 18:09:08.000000 scikeo-0.2.13/scikeo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      414 2023-06-26 18:09:08.526886 scikeo-0.2.13/setup.cfg
--rw-rw-rw-   0        0        0     1813 2023-06-26 18:09:00.000000 scikeo-0.2.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:36:32.025515 scikeo-0.2.15/
+-rw-rw-rw-   0        0        0      613 2023-06-26 18:09:00.000000 scikeo-0.2.15/LICENSE
+-rw-rw-rw-   0        0        0      130 2023-06-26 18:09:00.000000 scikeo-0.2.15/MANIFEST.in
+-rw-rw-rw-   0        0        0     8738 2023-07-27 16:36:32.025515 scikeo-0.2.15/PKG-INFO
+-rw-rw-rw-   0        0        0     7984 2023-07-27 16:35:12.000000 scikeo-0.2.15/README.md
+-rw-rw-rw-   0        0        0       62 2023-06-26 18:09:00.000000 scikeo-0.2.15/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 16:36:31.999416 scikeo-0.2.15/scikeo/
+-rw-rw-rw-   0        0        0      143 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/__init__.py
+-rw-rw-rw-   0        0        0    10900 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/atmosCorr.py
+-rw-rw-rw-   0        0        0     5794 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/calkmeans.py
+-rw-rw-rw-   0        0        0    19966 2023-07-27 16:35:12.000000 scikeo-0.2.15/scikeo/calmla.py
+-rw-rw-rw-   0        0        0     9989 2023-07-27 16:35:12.000000 scikeo-0.2.15/scikeo/deeplearning.py
+-rw-rw-rw-   0        0        0     6113 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/fusionrs.py
+-rw-rw-rw-   0        0        0     6668 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/linearTrend.py
+-rw-rw-rw-   0        0        0    26407 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/mla.py
+-rw-rw-rw-   0        0        0     5043 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/pca.py
+-rw-rw-rw-   0        0        0     5789 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/plot.py
+-rw-rw-rw-   0        0        0    12253 2023-07-27 16:35:12.000000 scikeo-0.2.15/scikeo/process.py
+-rw-rw-rw-   0        0        0     1871 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/rkmeans.py
+-rw-rw-rw-   0        0        0     3819 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/sma.py
+-rw-rw-rw-   0        0        0     5235 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/tassCap.py
+-rw-rw-rw-   0        0        0     2068 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/writeRaster.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:36:32.025004 scikeo-0.2.15/scikeo.egg-info/
+-rw-rw-rw-   0        0        0     8738 2023-07-27 16:36:31.000000 scikeo-0.2.15/scikeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-07-27 16:36:31.000000 scikeo-0.2.15/scikeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       56 2023-07-27 16:36:31.000000 scikeo-0.2.15/scikeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-26 18:09:08.000000 scikeo-0.2.15/scikeo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-07-27 16:36:31.000000 scikeo-0.2.15/scikeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 16:36:31.000000 scikeo-0.2.15/scikeo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      414 2023-07-27 16:36:32.027517 scikeo-0.2.15/setup.cfg
+-rw-rw-rw-   0        0        0     1813 2023-07-27 16:35:12.000000 scikeo-0.2.15/setup.py
```

### Comparing `scikeo-0.2.13/LICENSE` & `scikeo-0.2.15/LICENSE`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/PKG-INFO` & `scikeo-0.2.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikeo
-Version: 0.2.13
+Version: 0.2.15
 Summary: Remote Sensing Tools
 Home-page: https://github.com/ytarazona/scikit-eo
 Author: Yonatan Tarazona Coronel
 Author-email: geoyons@gmail.com
 License: Apache Software License 2.0
 Keywords: scikeo
 Classifier: Intended Audience :: Developers
@@ -25,16 +25,17 @@
 [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
 [![License: MIT](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PythonVersion]( https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-green)]()
 [![PyPI version](https://badge.fury.io/py/scikeo.svg)](https://badge.fury.io/py/scikeo)
 [![Youtube](https://img.shields.io/badge/YouTube-Channel-red)]()
 [![Downloads](https://pepy.tech/badge/scikeo)](https://pepy.tech/project/scikeo)
 [![Downloads](https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/docs-passing-brightgreen.svg)]()
+[![tests](https://github.com/ytarazona/scikit-eo/actions/workflows/tests.yml/badge.svg)](https://github.com/ytarazona/scikit-eo/actions/workflows/tests.yml)
+
 
-<img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/scikit-eo_logo.jpg" align="right" width="220"/>
 
 
 <!-- #region -->
 # Introduction
 
 Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are used to monitor a variety of environmental issues such as deforestation, land degradation, land use and land cover change, among others. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users developing Python lines of code. Algorithms for mapping land degradation through a linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, and calibration of machine learning algorithms, among others, are not available yet.
```

### Comparing `scikeo-0.2.13/README.md` & `scikeo-0.2.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
 [![License: MIT](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PythonVersion]( https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-green)]()
 [![PyPI version](https://badge.fury.io/py/scikeo.svg)](https://badge.fury.io/py/scikeo)
 [![Youtube](https://img.shields.io/badge/YouTube-Channel-red)]()
 [![Downloads](https://pepy.tech/badge/scikeo)](https://pepy.tech/project/scikeo)
 [![Downloads](https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/docs-passing-brightgreen.svg)]()
+[![tests](https://github.com/ytarazona/scikit-eo/actions/workflows/tests.yml/badge.svg)](https://github.com/ytarazona/scikit-eo/actions/workflows/tests.yml)
+
 
-<img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/scikit-eo_logo.jpg" align="right" width="220"/>
 
 
 <!-- #region -->
 # Introduction
 
 Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are used to monitor a variety of environmental issues such as deforestation, land degradation, land use and land cover change, among others. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users developing Python lines of code. Algorithms for mapping land degradation through a linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, and calibration of machine learning algorithms, among others, are not available yet.
```

### Comparing `scikeo-0.2.13/scikeo/atmosCorr.py` & `scikeo-0.2.15/scikeo/atmosCorr.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/scikeo/calkmeans.py` & `scikeo-0.2.15/scikeo/calkmeans.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/scikeo/calmla.py` & `scikeo-0.2.15/scikeo/calmla.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,24 +43,24 @@
         self.endm = endmembers
         
         # if it is read by pandas.read_csv()
         if isinstance(self.endm, (pd.core.frame.DataFrame)):
             
             for i in np.arange(self.endm.shape[1]):
                 
-                if all(self.endm.iloc[:,int(i)] < 100) & all(self.endm.iloc[:,int(i)] >= 1): indx = i; break
+                if all(self.endm.iloc[:,int(i)] < 100) & all(self.endm.iloc[:,int(i)] >= 0): indx = i; break
         
         # if the file is .dbf    
         elif isinstance(self.endm, (DBF)): # isinstance() function With Inheritance
             
             self.endm = pd.DataFrame(iter(self.endm))
             
             for i in np.arange(self.endm.shape[1]):
                 
-                if all(self.endm.iloc[:,int(i)] < 100) & all(self.endm.iloc[:,int(i)] >= 1): indx = i; break
+                if all(self.endm.iloc[:,int(i)] < 100) & all(self.endm.iloc[:,int(i)] >= 0): indx = i; break
         
         else:
             raise TypeError('"endm" must be .csv (pandas.core.frame.DataFrame).')
         
         self.indx = indx
```

### Comparing `scikeo-0.2.13/scikeo/deeplearning.py` & `scikeo-0.2.15/scikeo/deeplearning.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,17 @@
         # data in [rows*cols, bands]
         arr = st_reorder.reshape((rows*cols, bands))
 
         # nodata
         #if np.isnan(np.sum(arr)):
             #arr[np.isnan(arr)] = self.nodata
         
+        # dealing with nan
+        key_nan = np.isnan(np.sum(arr[:,0]))
+        
         if key_nan:
             # saving un array for predicted classes
             class_final = arr[:, 0].copy()
             # positions with nan
             posIndx = np.argwhere(~np.isnan(class_final)).flatten()
             # replace np.nan -> 0
             arr[np.isnan(arr)] = 0
@@ -251,10 +254,7 @@
                   'Confusion_Matrix': confusionMatrix,
                   'Classification_Map': class_fullyconnected,
                   'Image': self.image
                  } 
     
         return output
     
-    def CNN():
-        pass
-
```

### Comparing `scikeo-0.2.13/scikeo/fusionrs.py` & `scikeo-0.2.15/scikeo/fusionrs.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/scikeo/linearTrend.py` & `scikeo-0.2.15/scikeo/linearTrend.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/scikeo/mla.py` & `scikeo-0.2.15/scikeo/mla.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/scikeo/pca.py` & `scikeo-0.2.15/scikeo/pca.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/scikeo/plot.py` & `scikeo-0.2.15/scikeo/plot.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/scikeo/process.py` & `scikeo-0.2.15/scikeo/process.py`

 * *Files 12% similar despite different names*

```diff
@@ -167,15 +167,16 @@
     from a sample. This function shows how to obtain a confusion matrix by estimated proportions of area with a confidence
     interval at 95% (1.96).
      
     Parameters:
     
         matrix: confusion matrix or error matrix in numpy.ndarray.
             
-        image_pred: Array with 2d (rows, cols). This array should be the image classified with predicted classes.
+        image_pred: Could be an array with 2d (rows, cols). This array should be the image classified 
+                    with predicted classes. Or, could be a list with number of pixels for each class.
             
         pixel_size: Pixel size of the image classified. By default is 10m of Sentinel-2.
             
         conf: Confidence interval. By default is 95%.
     
     Return:
         
@@ -191,40 +192,61 @@
       doi:https://doi.org/10.1016/j.rse.2014.02.015.
     
     '''
     
     if not isinstance(matrix, (np.ndarray)):
         raise TypeError('"matrix" must be numpy.ndarray with rows and cols.')
         
-    if not isinstance(image_pred, (np.ndarray)):
-        raise TypeError('"image" must be numpy.ndarray with rows and cols.')
-    
-    # xlabel
-    if nodata is None:
-        image_pred = image_pred
-    else:
-        image_pred[image_pred == nodata] = np.nan
+    if isinstance(image_pred, (np.ndarray)):
+        
+        if image_pred.ndim == 2:
+            
+            # xlabel
+            if nodata is None:
+                image_pred = image_pred
+            else:
+                image_pred[image_pred == nodata] = np.nan
         
-    # classes
-    iclass = np.unique(image_pred[~np.isnan(image_pred)])
+            # classes
+            iclass = np.unique(image_pred[~np.isnan(image_pred)])
     
-    # ni
-    ni = np.sum(matrix, axis = 1)
+            # ni
+            ni = np.sum(matrix, axis = 1)
     
-    # number of classes
-    n = matrix.shape[0]
+            # number of classes
+            n = matrix.shape[0]
     
-    pixels = []
+            pixels = []
     
-    for i in iclass:
-        pixels.append((image_pred == i).sum()) #((30**2)/10000) # ha    
+            for i in iclass:
+                pixels.append((image_pred == i).sum()) #((30**2)/10000) # ha    
     
-    wi = (np.array([pixels])/np.array([pixels]).sum()).flatten()
+            wi = (np.array([pixels])/np.array([pixels]).sum()).flatten()
     
-    pixels = np.array(pixels)
+            pixels = np.array(pixels)
+        
+        elif image_pred.ndim == 1:
+            
+            # ni
+            ni = np.sum(matrix, axis = 1)
+    
+            # number of classes
+            n = matrix.shape[0]
+            
+            # classes
+            iclass = np.arange(len(image_pred))
+            
+            # pixels
+            pixels = np.array(image_pred)
+            
+            # pesos
+            wi = (np.array([pixels])/np.array([pixels]).sum()).flatten()
+    
+        else:
+            raise TypeError('"image" must be numpy.ndarray')
     
     # copy of matrix
     matConf = matrix.astype(float).copy()
     
     for i in range(n):
         matConf[i,:] = (matConf[i,:]/ni[i])*wi[i]
     
@@ -275,30 +297,58 @@
     
     # S(A)=1.96*s(p)*A(total) in ha
     SA = conf*np.array(sp)*(np.array(pixels).sum())*(pixel_size**2/10000)
     
     # Area total estimated
     A = total[0:n]*(np.array(pixels).sum())*(pixel_size**2/10000)
     
-    # print info
-    def print_info(matrixCEA, a, b, c, d):
-        print('***** Confusion Matrix by Estimated Proportions of area an uncertainty*****')
-        print('')
-        print('Overall accuracy with 95%')
-        print(f'{oa:.4f} ± {conf_int_oa:.4f}')
-        print('')
-        print('Confusion matrix')
-        print(matrixCEA)
-        print('')
-        print('User´s accuracy with 95%')
-        for i in range(b.shape[0]):
-            print(f'{iclass[i]}: {a[i]:.4f} ± {b[i]:.4f}')
-        print('')
-        print('Estimating area (Ha) and uncertainty with 95%')
-        for i in range(b.shape[0]):
-            print(f'{iclass[i]}: {c[i]:.4f} ± {d[i]:.4f}')
-            
-    return print_info(cm_prop_area, 
-                      ua, 
-                      conf_int_ua, 
-                      A, 
-                      SA)
+    result = {'Overall_accuracy':oa,
+              'CM_estimatedPA':cm_prop_area,
+              'Users_accuracy':ua,
+              'Users_accuracy_95%':conf_int_ua,
+              'Area_total_estimated': A,
+              'Area_at_95%': SA,
+              'conf_int_oa': conf_int_oa}
+    
+    return result
+
+
+def print_info(params):
+    
+    ''' Information: Confusion Matrix by Estimated Proportions of area an uncertainty
+    
+    Parameters:
+    
+        params: ```confintervalML``` result. See the function: https://github.com/ytarazona/scikit-eo/blob/main/scikeo/process.py
+    
+    Return:
+        
+        Information of confusion matrix by proportions of area, overall accuracy, user's accuracy with confidence interval 
+        and estimated area with confidence interval as well.
+        
+    Note:
+        This function was tested using ground-truth values obtained by Olofsson et al. (2014).
+        
+    '''
+    oa = params.get('Overall_accuracy')
+    matrixCEA = params.get('CM_estimatedPA')
+    a = params.get('Users_accuracy')
+    b = params.get('Users_accuracy_95%')
+    c = params.get('Area_total_estimated')
+    d = params.get('Area_at_95%')
+    e = params.get('conf_int_oa')
+    
+    print('***** Confusion Matrix by Estimated Proportions of area an uncertainty*****')
+    print('')
+    print('Overall accuracy with 95%')
+    print(f'{oa:.4f} ± {e:.4f}')
+    print('')
+    print('Confusion matrix')
+    print(matrixCEA)
+    print('')
+    print('User´s accuracy with 95%')
+    for i in range(b.shape[0]):
+        print(f'{iclass[i]}: {a[i]:.4f} ± {b[i]:.4f}')
+    print('')
+    print('Estimating area (Ha) and uncertainty with 95%')
+    for i in range(b.shape[0]):
+        print(f'{iclass[i]}: {c[i]:.4f} ± {d[i]:.4f}')
```

### Comparing `scikeo-0.2.13/scikeo/rkmeans.py` & `scikeo-0.2.15/scikeo/rkmeans.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/scikeo/sma.py` & `scikeo-0.2.15/scikeo/sma.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/scikeo/tassCap.py` & `scikeo-0.2.15/scikeo/tassCap.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/scikeo/writeRaster.py` & `scikeo-0.2.15/scikeo/writeRaster.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/scikeo.egg-info/PKG-INFO` & `scikeo-0.2.15/scikeo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikeo
-Version: 0.2.13
+Version: 0.2.15
 Summary: Remote Sensing Tools
 Home-page: https://github.com/ytarazona/scikit-eo
 Author: Yonatan Tarazona Coronel
 Author-email: geoyons@gmail.com
 License: Apache Software License 2.0
 Keywords: scikeo
 Classifier: Intended Audience :: Developers
@@ -25,16 +25,17 @@
 [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)]()
 [![License: MIT](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PythonVersion]( https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-green)]()
 [![PyPI version](https://badge.fury.io/py/scikeo.svg)](https://badge.fury.io/py/scikeo)
 [![Youtube](https://img.shields.io/badge/YouTube-Channel-red)]()
 [![Downloads](https://pepy.tech/badge/scikeo)](https://pepy.tech/project/scikeo)
 [![Downloads](https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/docs-passing-brightgreen.svg)]()
+[![tests](https://github.com/ytarazona/scikit-eo/actions/workflows/tests.yml/badge.svg)](https://github.com/ytarazona/scikit-eo/actions/workflows/tests.yml)
+
 
-<img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/scikit-eo_logo.jpg" align="right" width="220"/>
 
 
 <!-- #region -->
 # Introduction
 
 Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are used to monitor a variety of environmental issues such as deforestation, land degradation, land use and land cover change, among others. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users developing Python lines of code. Algorithms for mapping land degradation through a linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, and calibration of machine learning algorithms, among others, are not available yet.
```

### Comparing `scikeo-0.2.13/scikeo.egg-info/SOURCES.txt` & `scikeo-0.2.15/scikeo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.13/setup.py` & `scikeo-0.2.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='scikeo',
     name='scikeo',
     packages=find_packages(include=['scikeo', 'scikeo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ytarazona/scikit-eo',
-    version='0.2.13',
+    version='0.2.15',
     zip_safe=False,
 )
```

