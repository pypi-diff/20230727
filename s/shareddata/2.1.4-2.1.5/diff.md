# Comparing `tmp/shareddata-2.1.4.tar.gz` & `tmp/shareddata-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.1.4.tar", last modified: Thu Jul 27 09:07:31 2023, max compression
+gzip compressed data, was "shareddata-2.1.5.tar", last modified: Thu Jul 27 17:39:10 2023, max compression
```

## Comparing `shareddata-2.1.4.tar` & `shareddata-2.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-27 09:07:31.819846 shareddata-2.1.4/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.1.4/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-27 09:07:31.819846 shareddata-2.1.4/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.1.4/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.1.4/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-27 09:07:31.819846 shareddata-2.1.4/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-27 09:07:31.815846 shareddata-2.1.4/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-27 09:07:31.819846 shareddata-2.1.4/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1515 2023-06-24 22:46:48.000000 shareddata-2.1.4/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4738 2023-06-24 22:46:48.000000 shareddata-2.1.4/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1232 2023-06-24 22:46:48.000000 shareddata-2.1.4/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11268 2023-06-24 22:46:48.000000 shareddata-2.1.4/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.1.4/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5061 2023-06-24 22:46:48.000000 shareddata-2.1.4/src/SharedData/SeriesLib.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5759 2023-07-18 17:51:31.000000 shareddata-2.1.4/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.1.4/src/SharedData/SharedDataAWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.1.4/src/SharedData/SharedDataAWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1822 2023-07-23 19:20:04.000000 shareddata-2.1.4/src/SharedData/SharedDataFeeder.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10857 2023-06-25 15:34:09.000000 shareddata-2.1.4/src/SharedData/SharedDataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    15137 2023-07-24 01:42:34.000000 shareddata-2.1.4/src/SharedData/SharedDataPeriod.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3399 2023-07-22 06:17:01.000000 shareddata-2.1.4/src/SharedData/SharedDataRealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2468 2023-06-24 22:46:48.000000 shareddata-2.1.4/src/SharedData/SharedDataRealTimeProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28760 2023-07-27 08:45:10.000000 shareddata-2.1.4/src/SharedData/SharedDataTable.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8776 2023-07-08 20:02:34.000000 shareddata-2.1.4/src/SharedData/SharedDataTableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.1.4/src/SharedData/SharedDataTableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    21114 2023-07-24 01:30:39.000000 shareddata-2.1.4/src/SharedData/SharedDataTimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9036 2023-07-07 13:16:24.000000 shareddata-2.1.4/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-18 16:46:01.000000 shareddata-2.1.4/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.1.4/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-27 09:07:31.819846 shareddata-2.1.4/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-27 09:07:31.000000 shareddata-2.1.4/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      928 2023-07-27 09:07:31.000000 shareddata-2.1.4/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-27 09:07:31.000000 shareddata-2.1.4/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-27 09:07:31.000000 shareddata-2.1.4/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-27 09:07:31.000000 shareddata-2.1.4/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-27 17:39:10.717709 shareddata-2.1.5/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.1.5/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-27 17:39:10.717709 shareddata-2.1.5/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.1.5/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.1.5/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-27 17:39:10.717709 shareddata-2.1.5/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-27 17:39:10.713709 shareddata-2.1.5/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-27 17:39:10.717709 shareddata-2.1.5/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1515 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4738 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1232 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11268 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.1.5/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5061 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/SeriesLib.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5759 2023-07-18 17:51:31.000000 shareddata-2.1.5/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.1.5/src/SharedData/SharedDataAWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/SharedDataAWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1817 2023-07-27 16:58:00.000000 shareddata-2.1.5/src/SharedData/SharedDataFeeder.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10857 2023-06-25 15:34:09.000000 shareddata-2.1.5/src/SharedData/SharedDataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    15118 2023-07-27 17:37:34.000000 shareddata-2.1.5/src/SharedData/SharedDataPeriod.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3399 2023-07-22 06:17:01.000000 shareddata-2.1.5/src/SharedData/SharedDataRealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2468 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/SharedDataRealTimeProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28760 2023-07-27 08:45:10.000000 shareddata-2.1.5/src/SharedData/SharedDataTable.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8776 2023-07-08 20:02:34.000000 shareddata-2.1.5/src/SharedData/SharedDataTableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.1.5/src/SharedData/SharedDataTableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    21375 2023-07-27 17:31:32.000000 shareddata-2.1.5/src/SharedData/SharedDataTimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9036 2023-07-07 13:16:24.000000 shareddata-2.1.5/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-18 16:46:01.000000 shareddata-2.1.5/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-27 17:39:10.717709 shareddata-2.1.5/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-27 17:39:10.000000 shareddata-2.1.5/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      928 2023-07-27 17:39:10.000000 shareddata-2.1.5/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-27 17:39:10.000000 shareddata-2.1.5/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-27 17:39:10.000000 shareddata-2.1.5/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-27 17:39:10.000000 shareddata-2.1.5/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.1.4/LICENSE` & `shareddata-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/PKG-INFO` & `shareddata-2.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.1.4
+Version: 2.1.5
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.1.4/README.md` & `shareddata-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/setup.cfg` & `shareddata-2.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 2.1.4
+version = 2.1.5
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-2.1.4/src/SharedData/Defaults.py` & `shareddata-2.1.5/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/Logger.py` & `shareddata-2.1.5/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.1.5/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/Metadata.py` & `shareddata-2.1.5/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/MultiProc.py` & `shareddata-2.1.5/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/SeriesLib.py` & `shareddata-2.1.5/src/SharedData/SeriesLib.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/SharedData.py` & `shareddata-2.1.5/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/SharedDataAWSKinesis.py` & `shareddata-2.1.5/src/SharedData/SharedDataAWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/SharedDataAWSS3.py` & `shareddata-2.1.5/src/SharedData/SharedDataAWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/SharedDataFeeder.py` & `shareddata-2.1.5/src/SharedData/SharedDataFeeder.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(self, sharedData, feeder):
         self.feeder = feeder
         self.sharedData = sharedData    
         self.database = sharedData.database        
         
         # DATA DICTIONARY
         # data[period][tag]
-        self.data = {}     
+        self.data = {}
     
     def __setitem__(self, dataset, value):
         if not dataset in self.data.keys():
             if (dataset in SharedDataFeeder.dense_datasets.keys()):
                 period = dataset
                 self.data[period] = value
             else:
```

### Comparing `shareddata-2.1.4/src/SharedData/SharedDataFrame.py` & `shareddata-2.1.5/src/SharedData/SharedDataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/SharedDataPeriod.py` & `shareddata-2.1.5/src/SharedData/SharedDataPeriod.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os,io,hashlib,gzip,shutil
+import os,io,hashlib,gzip,shutil,time
 import pandas as pd
 import numpy as np
 from datetime import datetime, timedelta
 from pathlib import Path
 from pandas.tseries.offsets import BDay
 from threading import Thread
 
@@ -37,23 +37,24 @@
             self.default_startDate = pd.Timestamp('1990-01-01')
         elif self.period=='M1':
             self.periodSeconds = 60
             self.default_startDate = pd.Timestamp('2010-01-01')
         self.getContinousTimeIndex(self.default_startDate)
         self.loaded = False
 
-        
     def load(self):
         # read if not loaded
         shdatalist = self.sharedData.list()   
         path, shm_name = self.get_path()
         idx = [shm_name in str(s) for s in shdatalist.index]
         if not np.any(idx):
             self.read()
-
+        else:
+            #map
+            self.map(shm_name,shdatalist.index[idx])
 
     def __setitem__(self, tag, df):
         if not tag in self.tags.keys():
             if isinstance(tag, pd.Timestamp):
                 self.tags[tag] = SharedDataFrame(self, tag, df)
             else:
                 self.tags[tag] = SharedDataTimeSeries(self, tag, df)
@@ -61,15 +62,15 @@
             data = self.tags[tag].data
             iidx = df.index.intersection(data.index)
             icol = df.columns.intersection(data.columns)
             data.loc[iidx, icol] = df.loc[iidx, icol].copy()
 
     def __getitem__(self, tag):     
         if not self.loaded:
-            self.load()   
+            self.load()
             self.loaded=True
         if not tag in self.tags.keys():
             if isinstance(tag, pd.Timestamp):
                 df = SharedDataFrame(self, tag)
                 if not df.data.empty:
                     self.tags[tag] = df
                 else:
@@ -121,38 +122,14 @@
             nsec = (_timeidx - startDate).astype(np.int64)
             periods = (nsec/(10**9)/self.periodSeconds).astype(np.int64)
             self.ctimeidx[startDate] = np.empty(max(periods)+1)
             self.ctimeidx[startDate][:] = np.nan
             self.ctimeidx[startDate][periods.values] = np.arange(len(periods))        
         return self.ctimeidx[startDate]
 
-    def get(self, tag):
-        if isinstance(tag, pd.Timestamp):
-            df = SharedDataFrame(self, tag, malloc=False)
-            return df.data
-        else:  
-            return pd.DataFrame([]) 
-    
-    def exists(self, tag):
-        if isinstance(tag, pd.Timestamp):            
-            path = Path(os.environ['DATABASE_FOLDER'])
-            path = path / self.sharedData.user
-            path = path / self.sharedData.database
-            path = path / self.sharedDataFeeder.feeder
-            path = path / self.period       
-            fpath = path / (tag.strftime('%Y%m%d%H%M')+'.npy')            
-            return fpath.is_file()
-        else:
-            return False 
- 
-    def create_timeseries(self,tag,startDate,columns,overwrite=False):
-        self.tags[tag] = SharedDataTimeSeries(\
-            self,tag,startDate=startDate,columns=columns,overwrite=overwrite)
-        return self.tags[tag].data
-
     def get_path(self):        
         shm_name = self.sharedData.user + '/' + self.sharedData.database + '/' \
             + self.sharedDataFeeder.feeder + '/' + self.period
         if os.name=='posix':
             shm_name = shm_name.replace('/','\\')
 
         path = Path(os.environ['DATABASE_FOLDER'])
@@ -162,15 +139,29 @@
         path = path / self.period
         path = Path(str(path).replace('\\','/'))
         if self.sharedData.save_local:
             if not os.path.isdir(path.parent):
                 os.makedirs(path.parent)
         return path , shm_name
 
+    #CREATE
+    def create_timeseries(self,tag,startDate,columns,overwrite=False):
+        self.tags[tag] = SharedDataTimeSeries(\
+            self,tag,startDate=startDate,columns=columns,overwrite=overwrite)
+        return self.tags[tag].data
+
+    # READ
+    def map(self,shm_name,shm_name_list):
+        for shm in shm_name_list:
+            tag = shm.replace(shm_name,'')[1:]
+            self.tags[tag] = SharedDataTimeSeries(self, tag = tag)            
+
+
     def read(self):
+        tini = time.time()
         datasize = 1
         path, shm_name= self.get_path()
         headpath = str(path)+'_head.bin'
         tailpath = str(path)+'_tail.bin'        
         head_io = None
         tail_io = None
         if self.sharedData.s3read:
@@ -205,23 +196,30 @@
                 head_io = open(str(headpath),'rb')            
             
         if (tail_io is None) & (self.sharedData.save_local):
             if os.path.isfile(str(tailpath)):
                 tail_io = open(str(tailpath),'rb')
 
         if not head_io is None:
-            self.read_io(head_io,headpath)
+            datasize += self.read_io(head_io,headpath)
 
         if not tail_io is None:
-            self.read_io(tail_io,tailpath)
+            datasize += self.read_io(tail_io,tailpath)
+
+        te = time.time()-tini+0.000001   
+        datasize = datasize/(1024*1024)
+        Logger.log.debug('read %s/%s %.2fMB in %.2fs %.2fMBps ' % \
+            (self.sharedDataFeeder,self.period,datasize,te,datasize/te))
 
     def read_io(self,io_obj,path):
+        datasize = 0        
         #read
         io_obj.seek(0)
         io_data = io_obj.read()
+        datasize = len(io_data)
         _m = hashlib.md5(io_data[:-24]).digest()
         m = io_data[-16:]
         if (m!=_m):
             Logger.log.error('Timeseries read_head() file %s corrupted!' % (path))
             raise Exception('Timeseries read_head() %s corrupted!' % (path))
         io_obj.seek(0)
         separator = np.frombuffer(io_obj.read(8),dtype=np.int64)[0]        
@@ -245,14 +243,17 @@
                 data = self.tags[_tag].data
                 iidx = df.index.intersection(data.index)
                 icol = df.columns.intersection(data.columns)
                 data.loc[iidx, icol] = df.loc[iidx, icol].copy()
             separator = np.frombuffer(io_obj.read(8),dtype=np.int64)[0]
         io_obj.close()
 
+        return datasize
+
+    # WRITE
     def write(self,startDate=None):
         path , shm_name= self.get_path()                
         mtime = datetime.now().timestamp()
         partdate = pd.Timestamp(datetime(datetime.now().year,1,1))
         firstdate = pd.Timestamp('1970-01-01')
         if not startDate is None:
             firstdate = startDate
```

### Comparing `shareddata-2.1.4/src/SharedData/SharedDataRealTime.py` & `shareddata-2.1.5/src/SharedData/SharedDataRealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/SharedDataRealTimeProcess.py` & `shareddata-2.1.5/src/SharedData/SharedDataRealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/SharedDataTable.py` & `shareddata-2.1.5/src/SharedData/SharedDataTable.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/SharedDataTableIndex.py` & `shareddata-2.1.5/src/SharedData/SharedDataTableIndex.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/SharedDataTableIndexJit.py` & `shareddata-2.1.5/src/SharedData/SharedDataTableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/SharedDataTimeSeries.py` & `shareddata-2.1.5/src/SharedData/SharedDataTimeSeries.py`

 * *Files 22% similar despite different names*

```diff
@@ -62,29 +62,28 @@
                     self.columns = value.columns  
                     self.malloc_create()
                     sidx = np.array([self.get_loc_symbol(s) for s in self.columns])
                     ts = value.index.values.astype(np.int64)/10**9 #seconds
                     tidx = self.get_loc_timestamp(ts)
                     self.setValuesJit(self.data.values,tidx,sidx,value.values)
 
-                elif (value is None):                    
-                    # read & allocate data
-                    tini = time.time()
-                    datasize = self.read()
-                    datasize /= (1024*1024)
-                    te = time.time()-tini+0.000001                    
-                    Logger.log.debug('read %s/%s %.2fMB in %.2fs %.2fMBps ' % \
-                        (self.feeder,self.tag,datasize,te,datasize/te))
+                elif (value is None):
+                    Logger.log.error('Tag %s/%s not mapped!' % (self.feeder,self.tag))
+                    # # read & allocate data
+                    # tini = time.time()
+                    # datasize = self.read()
+                    # datasize /= (1024*1024)
+                    # te = time.time()-tini+0.000001                    
+                    # Logger.log.debug('read %s/%s %.2fMB in %.2fs %.2fMBps ' % \
+                    #     (self.feeder,self.tag,datasize,te,datasize/te))
                     
             elif (self.create_map == 'map'):
                 # map existing shared memory
                 self.malloc_map()
-                if (not value is None):
-                    Logger.log.warning('Tag %s exists in memory setting values '\
-                                       'but index and columns may differ!' % tag)
+                if (not value is None):                    
                     iidx = value.index.intersection(self.data.index)
                     icol = value.columns.intersection(self.data.columns)
                     self.data.loc[iidx,icol] = value.loc[iidx,icol].copy()
         except Exception as e:
             path, shm_name = self.get_path()
             Logger.log.error('Error initalizing %s!\n%s' % (shm_name,str(e)))
             self.free()
@@ -193,201 +192,201 @@
                         copy=False)
         
             return True
         except Exception as e:
             Logger.log.error('Failed to malloc_map\n%s' % str(e))
             return False
 
-    # READ
-    def read(self):           
-        datasize = 1
-        path, shm_name = self.get_path()
-        headpath = path / (self.tag+'_head.bin')
-        tailpath = path / (self.tag+'_tail.bin')   
-        head_io = None
-        tail_io = None
-        if self.sharedData.s3read:
-            force_download= (not self.sharedData.save_local)
-            
-            [head_io_gzip, head_local_mtime, head_remote_mtime] = \
-                S3Download(str(headpath),str(headpath)+'.gzip',force_download)
-            if not head_io_gzip is None:
-                head_io = io.BytesIO()
-                head_io_gzip.seek(0)
-                with gzip.GzipFile(fileobj=head_io_gzip, mode='rb') as gz:
-                    shutil.copyfileobj(gz,head_io)
-                if self.sharedData.save_local:
-                    SharedDataTimeSeries.write_file(head_io,headpath,mtime=head_remote_mtime)
-                    UpdateModTime(headpath,head_remote_mtime)
+    # # READ
+    # def read(self):           
+    #     datasize = 1
+    #     path, shm_name = self.get_path()
+    #     headpath = path / (self.tag+'_head.bin')
+    #     tailpath = path / (self.tag+'_tail.bin')   
+    #     head_io = None
+    #     tail_io = None
+    #     if self.sharedData.s3read:
+    #         force_download= (not self.sharedData.save_local)
+            
+    #         [head_io_gzip, head_local_mtime, head_remote_mtime] = \
+    #             S3Download(str(headpath),str(headpath)+'.gzip',force_download)
+    #         if not head_io_gzip is None:
+    #             head_io = io.BytesIO()
+    #             head_io_gzip.seek(0)
+    #             with gzip.GzipFile(fileobj=head_io_gzip, mode='rb') as gz:
+    #                 shutil.copyfileobj(gz,head_io)
+    #             if self.sharedData.save_local:
+    #                 SharedDataTimeSeries.write_file(head_io,headpath,mtime=head_remote_mtime)
+    #                 UpdateModTime(headpath,head_remote_mtime)
                     
             
-            [tail_io_gzip, tail_local_mtime, tail_remote_mtime] = \
-                S3Download(str(tailpath),str(tailpath)+'.gzip',force_download)
-            if not tail_io_gzip is None:
-                tail_io = io.BytesIO()
-                tail_io_gzip.seek(0)
-                with gzip.GzipFile(fileobj=tail_io_gzip, mode='rb') as gz:
-                    shutil.copyfileobj(gz,tail_io)
-                if self.sharedData.save_local:
-                    SharedDataTimeSeries.write_file(tail_io,tailpath,mtime=tail_remote_mtime)
-                    UpdateModTime(tailpath,tail_remote_mtime)
+    #         [tail_io_gzip, tail_local_mtime, tail_remote_mtime] = \
+    #             S3Download(str(tailpath),str(tailpath)+'.gzip',force_download)
+    #         if not tail_io_gzip is None:
+    #             tail_io = io.BytesIO()
+    #             tail_io_gzip.seek(0)
+    #             with gzip.GzipFile(fileobj=tail_io_gzip, mode='rb') as gz:
+    #                 shutil.copyfileobj(gz,tail_io)
+    #             if self.sharedData.save_local:
+    #                 SharedDataTimeSeries.write_file(tail_io,tailpath,mtime=tail_remote_mtime)
+    #                 UpdateModTime(tailpath,tail_remote_mtime)
         
-        if (head_io is None) & (self.sharedData.save_local):
-            # read local
-            if os.path.isfile(str(headpath)):
-                head_io = open(str(headpath),'rb')
-            
-        if (tail_io is None) & (self.sharedData.save_local):
-            if os.path.isfile(str(tailpath)):
-                tail_io = open(str(tailpath),'rb')
+    #     if (head_io is None) & (self.sharedData.save_local):
+    #         # read local
+    #         if os.path.isfile(str(headpath)):
+    #             head_io = open(str(headpath),'rb')
+            
+    #     if (tail_io is None) & (self.sharedData.save_local):
+    #         if os.path.isfile(str(tailpath)):
+    #             tail_io = open(str(tailpath),'rb')
         
-        self.startDate = None
-        self.columns = pd.Index([])
-        # read index, columns        
-        if not head_io is None:
-            head_io.seek(0)
-            [index,columns] = self.read_header(head_io)
-            self.columns = self.columns.union(columns)
-            self.startDate = pd.Timestamp(index.values[0])
-
-        if not tail_io is None:
-            tail_io.seek(0)
-            [index,columns] = self.read_header(tail_io)
-            self.columns = self.columns.union(columns)            
-            if self.startDate==None:
-                self.startDate = pd.Timestamp(index.values[0])
+    #     self.startDate = None
+    #     self.columns = pd.Index([])
+    #     # read index, columns        
+    #     if not head_io is None:
+    #         head_io.seek(0)
+    #         [index,columns] = self.read_header(head_io)
+    #         self.columns = self.columns.union(columns)
+    #         self.startDate = pd.Timestamp(index.values[0])
+
+    #     if not tail_io is None:
+    #         tail_io.seek(0)
+    #         [index,columns] = self.read_header(tail_io)
+    #         self.columns = self.columns.union(columns)            
+    #         if self.startDate==None:
+    #             self.startDate = pd.Timestamp(index.values[0])
         
-        if not self.startDate is None:
-            self.malloc_create()
-            # read data
-            if not head_io is None:
-                head_io.seek(0)                
-                datasize+=self.read_data(head_io,headpath)                
-                head_io.close()
-
-            if not tail_io is None:
-                tail_io.seek(0)                
-                datasize+=self.read_data(tail_io,tailpath)
-                tail_io.close()
+    #     if not self.startDate is None:
+    #         self.malloc_create()
+    #         # read data
+    #         if not head_io is None:
+    #             head_io.seek(0)                
+    #             datasize+=self.read_data(head_io,headpath)                
+    #             head_io.close()
+
+    #         if not tail_io is None:
+    #             tail_io.seek(0)                
+    #             datasize+=self.read_data(tail_io,tailpath)
+    #             tail_io.close()
         
-        return datasize
+    #     return datasize
 
-    def read_header(self,data_io):
-        _header = np.frombuffer(data_io.read(40),dtype=np.int64)
-        _idx_b = data_io.read(int(_header[2]))
-        _idx = pd.to_datetime(np.frombuffer(_idx_b,dtype=np.int64))
-        _colscsv_b = data_io.read(int(_header[3]))
-        _colscsv = _colscsv_b.decode(encoding='UTF-8',errors='ignore')
-        _cols = _colscsv.split(',')
-        return [_idx,_cols]
-
-    def read_data(self,data_io,path):
-        _header = np.frombuffer(data_io.read(40),dtype=np.int64)
-        _idx_b = data_io.read(int(_header[2]))
-        _idx = pd.to_datetime(np.frombuffer(_idx_b,dtype=np.int64))
-        _colscsv_b = data_io.read(int(_header[3]))
-        _colscsv = _colscsv_b.decode(encoding='UTF-8',errors='ignore')
-        _cols = _colscsv.split(',')
-        _data = np.frombuffer(data_io.read(int(_header[4])),dtype=np.float64).reshape((_header[0],_header[1]))
-        #calculate hash
-        _m = hashlib.md5(_idx_b)
-        _m.update(_colscsv_b)
-        _m.update(_data)
-        _md5hash_b = _m.digest()
-        __md5hash_b = data_io.read(16)
-        if not _md5hash_b==__md5hash_b:
-            raise Exception('Timeseries file corrupted!\n%s' % (path))
-        sidx = np.array([self.get_loc_symbol(s) for s in _cols])
-        ts = _idx.values.astype(np.int64)/10**9 #seconds
-        tidx = self.get_loc_timestamp(ts)
-        self.setValuesJit(self.data.values,tidx,sidx,_data)
-        data_io.close()
-        return _header[4]
+    # def read_header(self,data_io):
+    #     _header = np.frombuffer(data_io.read(40),dtype=np.int64)
+    #     _idx_b = data_io.read(int(_header[2]))
+    #     _idx = pd.to_datetime(np.frombuffer(_idx_b,dtype=np.int64))
+    #     _colscsv_b = data_io.read(int(_header[3]))
+    #     _colscsv = _colscsv_b.decode(encoding='UTF-8',errors='ignore')
+    #     _cols = _colscsv.split(',')
+    #     return [_idx,_cols]
+
+    # def read_data(self,data_io,path):
+    #     _header = np.frombuffer(data_io.read(40),dtype=np.int64)
+    #     _idx_b = data_io.read(int(_header[2]))
+    #     _idx = pd.to_datetime(np.frombuffer(_idx_b,dtype=np.int64))
+    #     _colscsv_b = data_io.read(int(_header[3]))
+    #     _colscsv = _colscsv_b.decode(encoding='UTF-8',errors='ignore')
+    #     _cols = _colscsv.split(',')
+    #     _data = np.frombuffer(data_io.read(int(_header[4])),dtype=np.float64).reshape((_header[0],_header[1]))
+    #     #calculate hash
+    #     _m = hashlib.md5(_idx_b)
+    #     _m.update(_colscsv_b)
+    #     _m.update(_data)
+    #     _md5hash_b = _m.digest()
+    #     __md5hash_b = data_io.read(16)
+    #     if not _md5hash_b==__md5hash_b:
+    #         raise Exception('Timeseries file corrupted!\n%s' % (path))
+    #     sidx = np.array([self.get_loc_symbol(s) for s in _cols])
+    #     ts = _idx.values.astype(np.int64)/10**9 #seconds
+    #     tidx = self.get_loc_timestamp(ts)
+    #     self.setValuesJit(self.data.values,tidx,sidx,_data)
+    #     data_io.close()
+    #     return _header[4]
  
-    # WRITE
-    def write(self, startDate=None):
-        firstdate = self.data.first_valid_index()
-        if not startDate is None:
-            firstdate = startDate
+    # # WRITE
+    # def write(self, startDate=None):
+    #     firstdate = self.data.first_valid_index()
+    #     if not startDate is None:
+    #         firstdate = startDate
         
-        path, shm_name = self.get_path()
+    #     path, shm_name = self.get_path()
         
-        partdate = pd.Timestamp(datetime(datetime.now().year,1,1))
-        threads = []
+    #     partdate = pd.Timestamp(datetime(datetime.now().year,1,1))
+    #     threads = []
 
-        mtime = datetime.now().timestamp()        
-        if firstdate<partdate:
-            # write head
-            threads = [*threads , \
-                Thread(target=SharedDataTimeSeries.write_timeseries_df,\
-                    args=(self,self.data.loc[:partdate], str(path / (self.tag+'_head.bin')), mtime) )]
-        # write tail
-        threads = [*threads , \
-                Thread(target=SharedDataTimeSeries.write_timeseries_df,\
-                    args=(self,self.data.loc[partdate:], str(path / (self.tag+'_tail.bin')), mtime) )]
+    #     mtime = datetime.now().timestamp()        
+    #     if firstdate<partdate:
+    #         # write head
+    #         threads = [*threads , \
+    #             Thread(target=SharedDataTimeSeries.write_timeseries_df,\
+    #                 args=(self,self.data.loc[:partdate], str(path / (self.tag+'_head.bin')), mtime) )]
+    #     # write tail
+    #     threads = [*threads , \
+    #             Thread(target=SharedDataTimeSeries.write_timeseries_df,\
+    #                 args=(self,self.data.loc[partdate:], str(path / (self.tag+'_tail.bin')), mtime) )]
 
-        for i in range(len(threads)):
-            threads[i].start()
+    #     for i in range(len(threads)):
+    #         threads[i].start()
 
-        for i in range(len(threads)):
-            threads[i].join()
+    #     for i in range(len(threads)):
+    #         threads[i].join()
         
-    def write_timeseries_df(self,df,tag_path,mtime):
-        ts_io = SharedDataTimeSeries.create_timeseries_io(df)        
-        threads=[]
-        if self.sharedData.s3write:
-            ts_io.seek(0)
-            gzip_io = io.BytesIO()
-            with gzip.GzipFile(fileobj=gzip_io, mode='wb', compresslevel=1) as gz:
-                shutil.copyfileobj(ts_io, gz)
-
-            threads = [*threads , \
-                Thread(target=S3Upload,args=(gzip_io, tag_path+'.gzip', mtime) )]
-
-        if self.sharedData.save_local:
-            threads = [*threads , \
-                Thread(target=SharedDataTimeSeries.write_file, args=(ts_io, tag_path, mtime) )]
+    # def write_timeseries_df(self,df,tag_path,mtime):
+    #     ts_io = SharedDataTimeSeries.create_timeseries_io(df)        
+    #     threads=[]
+    #     if self.sharedData.s3write:
+    #         ts_io.seek(0)
+    #         gzip_io = io.BytesIO()
+    #         with gzip.GzipFile(fileobj=gzip_io, mode='wb', compresslevel=1) as gz:
+    #             shutil.copyfileobj(ts_io, gz)
+
+    #         threads = [*threads , \
+    #             Thread(target=S3Upload,args=(gzip_io, tag_path+'.gzip', mtime) )]
+
+    #     if self.sharedData.save_local:
+    #         threads = [*threads , \
+    #             Thread(target=SharedDataTimeSeries.write_file, args=(ts_io, tag_path, mtime) )]
                             
-        for i in range(len(threads)):
-            threads[i].start()
+    #     for i in range(len(threads)):
+    #         threads[i].start()
 
-        for i in range(len(threads)):
-            threads[i].join()
+    #     for i in range(len(threads)):
+    #         threads[i].join()
 
-    def create_timeseries_io(df):
-        df = df.dropna(how='all',axis=0)
-        r, c = df.shape
-        idx = (df.index.astype(np.int64))
-        idx_b = idx.values.tobytes()
-        cols = df.columns.values
-        colscsv = ','.join(cols)
-        colscsv_b = str.encode(colscsv,encoding='UTF-8',errors='ignore')
-        nbidx = len(idx_b)
-        nbcols = len(colscsv_b)
-        data = np.ascontiguousarray(df.values.astype(np.float64))
-        header = np.array([r,c,nbidx,nbcols,r*c*8]).astype(np.int64)
-        #calculate hash
-        m = hashlib.md5(idx_b)
-        m.update(colscsv_b)
-        m.update(data)
-        md5hash_b = m.digest()
-        # allocate memory
-        io_obj = io.BytesIO()
-        io_obj.write(header)
-        io_obj.write(idx_b)
-        io_obj.write(colscsv_b)
-        io_obj.write(data)
-        io_obj.write(md5hash_b)
-        return io_obj
-
-    def write_file(io_obj,path,mtime):
-        with open(path, 'wb') as f:
-            f.write(io_obj.getbuffer())
-            f.flush()
-        os.utime(path, (mtime, mtime))
+    # def create_timeseries_io(df):
+    #     df = df.dropna(how='all',axis=0)
+    #     r, c = df.shape
+    #     idx = (df.index.astype(np.int64))
+    #     idx_b = idx.values.tobytes()
+    #     cols = df.columns.values
+    #     colscsv = ','.join(cols)
+    #     colscsv_b = str.encode(colscsv,encoding='UTF-8',errors='ignore')
+    #     nbidx = len(idx_b)
+    #     nbcols = len(colscsv_b)
+    #     data = np.ascontiguousarray(df.values.astype(np.float64))
+    #     header = np.array([r,c,nbidx,nbcols,r*c*8]).astype(np.int64)
+    #     #calculate hash
+    #     m = hashlib.md5(idx_b)
+    #     m.update(colscsv_b)
+    #     m.update(data)
+    #     md5hash_b = m.digest()
+    #     # allocate memory
+    #     io_obj = io.BytesIO()
+    #     io_obj.write(header)
+    #     io_obj.write(idx_b)
+    #     io_obj.write(colscsv_b)
+    #     io_obj.write(data)
+    #     io_obj.write(md5hash_b)
+    #     return io_obj
+
+    # def write_file(io_obj,path,mtime):
+    #     with open(path, 'wb') as f:
+    #         f.write(io_obj.getbuffer())
+    #         f.flush()
+    #     os.utime(path, (mtime, mtime))
 
     # MESSAGES
     def broadcast(self,idx,col):
         SharedDataRealTime.broadcast(
             self.sharedData,
             self.feeder,
             self.period,
```

### Comparing `shareddata-2.1.4/src/SharedData/SharedNumpy.py` & `shareddata-2.1.5/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/SharedData/Utils.py` & `shareddata-2.1.5/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.4/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.1.5/src/shareddata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.1.4
+Version: 2.1.5
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.1.4/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.1.5/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

