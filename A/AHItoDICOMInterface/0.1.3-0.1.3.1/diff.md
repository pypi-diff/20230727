# Comparing `tmp/AHItoDICOMInterface-0.1.3.tar.gz` & `tmp/AHItoDICOMInterface-0.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AHItoDICOMInterface-0.1.3.tar", last modified: Wed Jul 26 16:07:44 2023, max compression
+gzip compressed data, was "AHItoDICOMInterface-0.1.3.1.tar", last modified: Thu Jul 27 18:33:35 2023, max compression
```

## Comparing `AHItoDICOMInterface-0.1.3.tar` & `AHItoDICOMInterface-0.1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 16:07:44.183371 AHItoDICOMInterface-0.1.3/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 16:07:44.183371 AHItoDICOMInterface-0.1.3/AHItoDICOMInterface/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-07-26 01:11:03.000000 AHItoDICOMInterface-0.1.3/AHItoDICOMInterface/AHIClientFactory.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6389 2023-07-26 01:11:03.000000 AHItoDICOMInterface-0.1.3/AHItoDICOMInterface/AHIDataDICOMizer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3288 2023-07-26 01:11:03.000000 AHItoDICOMInterface-0.1.3/AHItoDICOMInterface/AHIFrameFetcher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16435 2023-07-26 15:56:39.000000 AHItoDICOMInterface-0.1.3/AHItoDICOMInterface/AHItoDICOM.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      168 2023-07-26 14:34:05.000000 AHItoDICOMInterface-0.1.3/AHItoDICOMInterface/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 16:07:44.183371 AHItoDICOMInterface-0.1.3/AHItoDICOMInterface.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-07-26 16:07:44.000000 AHItoDICOMInterface-0.1.3/AHItoDICOMInterface.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      432 2023-07-26 16:07:44.000000 AHItoDICOMInterface-0.1.3/AHItoDICOMInterface.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-26 16:07:44.000000 AHItoDICOMInterface-0.1.3/AHItoDICOMInterface.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-07-26 16:07:44.000000 AHItoDICOMInterface-0.1.3/AHItoDICOMInterface.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-26 16:07:44.000000 AHItoDICOMInterface-0.1.3/AHItoDICOMInterface.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10142 2023-05-02 22:59:53.000000 AHItoDICOMInterface-0.1.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-05-02 22:59:53.000000 AHItoDICOMInterface-0.1.3/NOTICE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      829 2023-07-26 16:07:44.183371 AHItoDICOMInterface-0.1.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5772 2023-07-26 00:39:46.000000 AHItoDICOMInterface-0.1.3/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-26 16:07:44.183371 AHItoDICOMInterface-0.1.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1180 2023-07-26 16:07:38.000000 AHItoDICOMInterface-0.1.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 18:33:35.010922 AHItoDICOMInterface-0.1.3.1/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 18:33:35.006922 AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-07-26 01:11:03.000000 AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface/AHIClientFactory.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6459 2023-07-27 18:10:07.000000 AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface/AHIDataDICOMizer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3242 2023-07-27 18:12:38.000000 AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface/AHIFrameFetcher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16742 2023-07-27 18:17:52.000000 AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface/AHItoDICOM.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      168 2023-07-27 18:28:25.000000 AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 18:33:35.010922 AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      831 2023-07-27 18:33:34.000000 AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      432 2023-07-27 18:33:34.000000 AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-27 18:33:34.000000 AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-07-27 18:33:34.000000 AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-27 18:33:34.000000 AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10142 2023-05-02 22:59:53.000000 AHItoDICOMInterface-0.1.3.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-05-02 22:59:53.000000 AHItoDICOMInterface-0.1.3.1/NOTICE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      831 2023-07-27 18:33:35.010922 AHItoDICOMInterface-0.1.3.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6498 2023-07-26 18:47:51.000000 AHItoDICOMInterface-0.1.3.1/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-27 18:33:35.010922 AHItoDICOMInterface-0.1.3.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1182 2023-07-27 18:33:23.000000 AHItoDICOMInterface-0.1.3.1/setup.py
```

### Comparing `AHItoDICOMInterface-0.1.3/AHItoDICOMInterface/AHIClientFactory.py` & `AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface/AHIClientFactory.py`

 * *Files identical despite different names*

### Comparing `AHItoDICOMInterface-0.1.3/AHItoDICOMInterface/AHIDataDICOMizer.py` & `AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface/AHIDataDICOMizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 
     ds = Dataset()
     InstanceId  = None
     thread_running = None
     AHI_metadata = None 
     process = None
     status = None
+    logger = None
 
 
     def __init__(self, InstanceId, AHI_metadata) -> None:
+        self.logger = logging.getLogger(__name__)
         self.InstanceId = InstanceId
         self.DICOMizeJobs = Queue()
         self.DICOMizeJobsCompleted = Queue()
         self.AHI_metadata = AHI_metadata
         manager = Manager()
         self.thread_running = manager.Value('i', 1)
         self.status = manager.Value(c_char_p, "idle")
@@ -37,15 +39,15 @@
         self.process.start()
 
 
 
 
     def AddDICOMizeJob(self,FetchJob):
             self.DICOMizeJobs.put(FetchJob)
-            #logging.debug("[AHIDataDICOMizer][AddDICOMizeJob]["+self.InstanceId+"] - DICOMize Job added "+str(FetchJob)+".")
+            self.logger.debug("[{__name__}][AddDICOMizeJob]["+self.InstanceId+"] - DICOMize Job added "+str(FetchJob)+".")
 
     def ProcessJobs(self , DICOMizeJobs , DICOMizeJobsCompleted , status , thread_running , InstanceId):      
         while(bool(thread_running.value)):
             if not DICOMizeJobs.empty():
                 status.value ="busy"
                 try:
                     ImageFrame = DICOMizeJobs.get(block=False)
@@ -69,21 +71,21 @@
                     if (pixels is not None):
                         self.ds.PixelData = pixels.tobytes()
                     vrlist.clear()
                     DICOMizeJobsCompleted.put(self.ds)
                 except Exception as DICOMizeError:
                     print("ERROR")
                     DICOMizeJobsCompleted.put(None)
-                    logging.error(f"[AHIDataDICOMizer][{str(self.InstanceId)}] - {DICOMizeError}")
+                    self.logger.error(f"[{__name__}][{str(self.InstanceId)}] - {DICOMizeError}")
             else:
                 status.value = 'idle'    
                 sleep(0.1)
-            logging.debug(f" DICOMizer Process {InstanceId} : {status.value}")
+            self.logger.debug(f" DICOMizer Process {InstanceId} : {status.value}")
         status.value ="stopped"
-        logging.debug(f" DICOMizer Process {InstanceId} : {status.value}")
+        self.logger.debug(f" DICOMizer Process {InstanceId} : {status.value}")
 
     def getFramesDICOMized(self):
         if not self.DICOMizeJobsCompleted.empty():
             obj = self.DICOMizeJobsCompleted.get()
             return obj
         else:
             return None
@@ -91,15 +93,15 @@
     def getDataset(self):
         return self.ds
 
         
     def getDICOMVRs(self,taglevel, vrlist):
         for theKey in taglevel:
             vrlist.append( [ theKey , taglevel[theKey] ])
-            #logging.debug(f"[AHIDataDICOMizer][getDICOMVRs] - List of private tags VRs: {vrlist}\r\n")
+            self.logger.debug(f"[{__name__}][getDICOMVRs] - List of private tags VRs: {vrlist}\r\n")
 
 
 
     def getTags(self,tagLevel, ds , vrlist):    
         for theKey in tagLevel:
             try:
                 try:
@@ -108,15 +110,15 @@
                     tagvr = None
                     for vr in vrlist:
                         if theKey == vr[0]:
                             tagvr = vr[1]
                 datavalue=tagLevel[theKey]
                 #print(f"{theKey} : {datavalue}")
                 if(tagvr == 'SQ'):
-                    #logging.debug(f"{theKey} : {tagLevel[theKey]} , {vrlist}")
+                    #self.logger.debug(f"{theKey} : {tagLevel[theKey]} , {vrlist}")
                     seqs = []
                     for underSeq in tagLevel[theKey]:
                         seqds = Dataset()
                         self.getTags(underSeq, seqds, vrlist)
                         seqs.append(seqds)
                     datavalue = Sequence(seqs)
                     continue
@@ -136,13 +138,13 @@
                 data_element = DataElement(theKey , tagvr , datavalue )
                 if data_element.tag.group != 2:
                     try:
                         ds.add(data_element) 
                     except:
                         continue
             except Exception as err:
-                logging.warning(f"[AHIDataDICOMizer][getTags] - {err}")
+                self.logger.warning(f"[{__name__}][getTags] - {err}")
                 continue
 
     def Dispose(self):
         self.thread_running.value = 0
         self.process.kill()
```

### Comparing `AHItoDICOMInterface-0.1.3/AHItoDICOMInterface/AHIFrameFetcher.py` & `AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface/AHIFrameFetcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,32 +21,32 @@
     InstanceId= None
     client = None
     thread_running = True
     process = None
     aws_access_key = None
     aws_secret_key = None
     AHI_endpoint = None
+    logger = None
 
     def __init__(self, InstanceId , aws_access_key , aws_secret_key , AHI_endpoint = None , ahi_client = None):
+        self.logger = logging.getLogger(__name__)
         self.InstanceId = InstanceId
         self.FetchJobs = Queue()
         self.FetchJobsCompleted = Queue()
         self.FetchJobsInError = Queue()
         self.aws_secret_key = aws_access_key
         self.aws_secret_key = aws_secret_key
         self.AHI_endpoint = AHI_endpoint
         self.ahi_client = ahi_client
         self.process = Process(target = self.ProcessJobs , args=(self.FetchJobs,self.FetchJobsCompleted, self.FetchJobsInError ,  self.aws_access_key , self.aws_secret_key , self.AHI_endpoint , self.ahi_client))
         self.process.start()
    
     def AddFetchJob(self,FetchJob):
             self.FetchJobs.put(FetchJob)
-            #print(f"[FrameFetcher][{self.InstanceId}] Job entry added")
-            #print(FetchJob)
-            #logging.debug("[AHIFrameFetcher][AddFetchJob]["+self.InstanceId+"] - Fetch Job added "+str(FetchJob)+".")
+            self.logger.debug("[{__name__}]["+self.InstanceId+"] - Fetch Job added "+str(FetchJob)+".")
 
     def ProcessJobs(self,FetchJobs : Queue, FetchJobsCompleted : Queue , FetchJobsInError : Queue ,   aws_access_key : str = None , aws_secret_key : str = None , AHI_endpoint : str = None , ahi_client = None):  
         if ahi_client is None: 
             ahi_client = AHIClientFactory( aws_access_key= aws_access_key , aws_secret_key=aws_secret_key ,  aws_accendpoint_url=AHI_endpoint )
         while(self.thread_running):
             if not FetchJobs.empty():
                 try:
@@ -77,14 +77,14 @@
                 imageFrameInformation= {'imageFrameId' :imageFrameId})
             b = io.BytesIO()
             b.write(res['imageFrameBlob'].read())
             b.seek(0)
             d = decode(b)
             return d
         except Exception as e:
-            logging.error("[AHIFramefetcher] - Frame could not be decoded.")
-            logging.error(e)
+            self.logger.error("[{__name__}] - Frame could not be decoded.")
+            self.logger.error(e)
             return None
     
     def Dispose(self):
         self.thread_running = False
         self.process.kill()
```

### Comparing `AHItoDICOMInterface-0.1.3/AHItoDICOMInterface/AHItoDICOM.py` & `AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface/AHItoDICOM.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,25 +34,27 @@
     FrameDICOMizerPoolManager = None
     DICOMizedFrames = None
     CountToDICOMize = 0
     still_processing = False
     aws_access_key = None
     aws_secret_key = None
     AHI_endpoint = None
+    logger = None
 
     def __init__(self, aws_access_key : str =  None, aws_secret_key : str = None , AHI_endpoint : str = None , fetcher_process_count : int = None , dicomizer_process_count : int = None ) -> None:
         """
         Helper class constructor.
 
         :param aws_access_key: Optional IAM user access key.
         :param aws_secret_key: Optional IAM user secret key.
         :param AHI_endpoint: Optional AHI endpoint URL. Only useful to AWS employees.
         :param fetcher_process_count: Optional number of processes to use for fetching frames. Will default to CPU count x 8
         :param dicomizer_process_count: Optional number of processes to use for DICOMizing frames.Will default to CPU count.
         """ 
+        self.logger = logging.getLogger(__name__)
         self.ImageFrames = collections.deque()
         self.frameToDICOMize = collections.deque()
         self.DICOMizedFrames = collections.deque()
         self.aws_access_key = aws_access_key
         self.aws_secret_key =  aws_secret_key
         self.AHI_endpoint = AHI_endpoint
         if fetcher_process_count is None:
@@ -60,15 +62,15 @@
         else:
             self.fetcherProcessCount = fetcher_process_count
         if dicomizer_process_count is None:
             self.DICOMizerProcessCount = int(os.cpu_count())
         else:
             self.DICOMizerProcessCount = dicomizer_process_count
         
-        logging.debug(f"[AHItoDICOM] - Fetcher process count : {self.fetcherProcessCount} , DICOMizer process count : {self.DICOMizerProcessCount}")
+        self.logger.debug(f"[{__name__}] - Fetcher process count : {self.fetcherProcessCount} , DICOMizer process count : {self.DICOMizerProcessCount}")
         #mp.set_start_method('fork')
         
     def DICOMizeByStudyInstanceUID(self, datastore_id : str = None , study_instance_uid : str = None):
         """
         DICOMizeByStudyInstanceUID(datastore_id : str = None , study_instance_uid : str = None).
 
         :param datastore_id: The datastoreId containtaining the DICOM Study.
@@ -88,15 +90,15 @@
             ]
         }
         client = AHIClientFactory(self.aws_access_key ,  self.aws_secret_key , self.AHI_endpoint )
         search_result = client.search_image_sets(datastoreId=datastore_id, searchCriteria = search_criteria) ### in theory we should check if a continuation token is returned and loop until we have all the results...
         instances = []
         for imageset in search_result["imageSetsMetadataSummaries"]:
             current_imageset = imageset["imageSetId"]
-            print(current_imageset)
+            self.logger.debug(f"[{__name__}] - Exporting {current_imageset} instances in memory.")
             instances += self.DICOMizeImageSet(datastore_id=datastore_id , image_set_id=current_imageset)
 
         return instances
 
     def DICOMizeImageSet(self, datastore_id : str = None , image_set_id : str = None):
         """
         DICOMizeImageSet(datastore_id : str = None , image_set_id : str = None).
@@ -115,15 +117,15 @@
         if AHI_metadata is None:
             return None
         #threads init for Frame fetching and DICOM encapsulation
         self._initFetchAndDICOMizeProcesses(AHI_metadata=AHI_metadata )
         series = self.getSeriesList(AHI_metadata , image_set_id)[0]
         self.ImageFrames.extendleft(self.getImageFrames(datastore_id, image_set_id , AHI_metadata , series["SeriesInstanceUID"])) 
         ImageFrameCount = len(self.ImageFrames) 
-        logging.debug(f"[DICOMize] - Importing {ImageFrameCount} instances in memory.")
+        self.logger.debug(f"[{__name__}] - Importing {ImageFrameCount} instances in memory.")
         self.CountToDICOMize = ImageFrameCount
         self.FrameDICOMizerPoolManager.start()
         
         #Assigning jobs to the Frame fetching thread pool.
         threadId = 0
         while(len(self.ImageFrames)> 0):
             self.frameFetcherThreadList[threadId].AddFetchJob(self.ImageFrames.popleft())
@@ -135,33 +137,33 @@
                 #logging.debug(f"Done {FrameFetchedCount}/{ImageFrameCount}")
                 for x in range(self.fetcherProcessCount):
                     entry=self.frameFetcherThreadList[x].getFramesFetched()
                     if entry is not None:
                         FrameFetchedCount+=1
                         self.frameToDICOMize.append(entry)  
                 sleep(0.01)
-        logging.debug("All frames Fetched and submitted to the DICOMizer queue") 
+        self.logger.debug("All frames Fetched and submitted to the DICOMizer queue") 
         for x in range(self.fetcherProcessCount):
-            logging.debug(f"[DICOMize] - Disposing frame fetcher thread # {x}")
+            self.logger.debug(f"[{__name__}] - Disposing frame fetcher thread # {x}")
             self.frameFetcherThreadList[x].Dispose()
-            logging.debug(f"[DICOMize] - frame fetcher thread # {x} disposed.")
+            self.logger.debug(f"[{__name__}] - frame fetcher thread # {x} disposed.")
         while(self.still_processing  == True):
-            logging.debug("[DICOMize] - Still processing DICOMizing...")
+            self.logger.debug(f"[{__name__}] - Still processing DICOMizing...")
             sleep(0.1)
 
         returnlist = list(self.DICOMizedFrames)
         returnlist.sort( key= self.getInstanceNumberInDICOM)
         return returnlist
 
 
 
 
     def AssignDICOMizeJob(self):
         #this function rounds robin accross all the dicomizer threads, until all the images are actually dicomized.
-        logging.debug(f"[AssignDICOMizeJob] - DICOMizer Thread Assigner started.")
+        self.logger.debug(f"[AssignDICOMizeJob] - DICOMizer Thread Assigner started.")
         keep_running = True
 
 
         while( keep_running):
             while( len(self.frameToDICOMize) > 0):
                 threadId = 0
                 self.frameDICOMizerThreadList[threadId].AddDICOMizeJob(self.frameToDICOMize.popleft())
@@ -173,37 +175,37 @@
                 while( not self.frameDICOMizerThreadList[x].DICOMizeJobsCompleted.empty()):
                     self.DICOMizedFrames.append(self.frameDICOMizerThreadList[x].getFramesDICOMized())
             dc = len(self.DICOMizedFrames)
             #print(dc)
 
             if(len(self.DICOMizedFrames)  == self.CountToDICOMize):
                 keep_running = False
-                logging.debug(f"DICOMized count : {dc}")
+                self.logger.debug(f"[{__name__}] - DICOMized count : {dc}")
                 for x in range(self.DICOMizerProcessCount):
-                    logging.debug(f"[DICOMize] - Disposing DICOMizer thread # {x}")
+                    self.logger.debug(f"[{__name__}] - Disposing DICOMizer thread # {x}")
                     self.frameDICOMizerThreadList[x].Dispose()
-                    logging.debug(f"[DICOMize] - DICOMizer thread # {x} Disposed.")
+                    self.logger.debug(f"[{__name__}] - DICOMizer thread # {x} Disposed.")
                 self.still_processing = False
             else:
                 sleep(0.05)
 
-        logging.debug(f"[AssignDICOMizeJob] - DICOMizer Thread Assigner finished.")        
+        self.logger.debug(f"[AssignDICOMizeJob] - DICOMizer Thread Assigner finished.")        
 
     def getImageFrames(self, datastoreId, studyId , AHI_metadata , seriesUid) -> collections.deque:
         instancesList = []
         for instances in AHI_metadata["Study"]["Series"][seriesUid]["Instances"]:
             if len(AHI_metadata["Study"]["Series"][seriesUid]["Instances"][instances]["ImageFrames"]) < 1:
                 print("Skipping the following instances because they do not contain ImageFrames: " + instances)
                 continue
             try:        
                 frameId = AHI_metadata["Study"]["Series"][seriesUid]["Instances"][instances]["ImageFrames"][0]["ID"]
                 InstanceNumber = AHI_metadata["Study"]["Series"][seriesUid]["Instances"][instances]["DICOM"]["InstanceNumber"]
                 instancesList.append( { "datastoreId" : datastoreId, "studyId" : studyId , "frameId" : frameId , "SeriesUID" : seriesUid , "SOPInstanceUID" : instances,  "InstanceNumber" : InstanceNumber , "PixelData" : None})
-            except Exception as e: # The code above failes for 
-                print(e)
+            except Exception as AHIErr: # The code above failes for 
+                self.logger.error(f"[{__name__}] - {AHIErr}")
         instancesList.sort(key=self.getInstanceNumber)
         return collections.deque(instancesList)
 
     def getSeriesList(self, AHI_metadata , image_set_id : str):
         ###07/25/2023 - awsjpleger :  this function is from a time when there could be multiple series withing a single ImageSetId. Still works with new AHI metadata, but should be refactored.
         seriesList = []
         for series in AHI_metadata["Study"]["Series"]:
@@ -234,15 +236,15 @@
             if client is None:
                 client = AHIClientFactory(self.aws_access_key ,  self.aws_secret_key , self.AHI_endpoint )
             AHI_study_metadata = client.get_image_set_metadata(datastoreId=datastore_id , imageSetId=imageset_id)
             json_study_metadata = gzip.decompress(AHI_study_metadata["imageSetMetadataBlob"].read())
             json_study_metadata = json.loads(json_study_metadata)  
             return json_study_metadata
         except Exception as AHIErr :
-            logging.error(AHIErr)
+            self.logger.error(f"[{__name__}] - {AHIErr}")
             return None
     
     def getImageSetToSeriesUIDMap(self, datastore_id : str, study_instance_uid : str ):
         """
         getImageSetToSeriesUIDMap(datastore_id : str = None , study_instance_uid : str).
 
         :param datastore_id: The datastoreId containtaining the DICOM Study.
@@ -293,33 +295,33 @@
             image_2d_scaled = (np.maximum(image_2d,0) / image_2d.max()) * 255.0
             image_2d_scaled = np.uint8(image_2d_scaled)
             if 'PhotometricInterpretation' in ds and ds.PhotometricInterpretation == "MONOCHROME1":
                 image_2d_scaled = np.max(image_2d_scaled) - image_2d_scaled
             img = Image.fromarray(image_2d_scaled)
             img.save(destination, 'png')
         except Exception as err:
-            logging.error(f"[saveAsPngPIL] - {err}")
+            self.logger.error(f"[{__name__}][saveAsPngPIL] - {err}")
             return False
         return True
 
     # def getSeries(self, datastore_id : str = None , image_set_id : str = None):
     #     AHI_metadata = self.getMetadata(datastore_id, image_set_id, self.AHIclient)
     #     seriesList = self.getSeriesList(AHI_metadata=AHI_metadata)
     #     return seriesList  
 
     def _initFetchAndDICOMizeProcesses(self, AHI_metadata):
         self.frameDICOMizerThreadList = []
         self.frameDICOMizerThreadList = []
         self.frameFetcherThreadList.clear()
         self.frameDICOMizerThreadList.clear()
         for x in range(self.fetcherProcessCount): 
-            #logging.debug("[DICOMize] - Spawning AHIFrameFetcher thread # "+str(x))
+            self.logger.debug("[DICOMize] - Spawning AHIFrameFetcher thread # "+str(x))
             self.frameFetcherThreadList.append(AHIFrameFetcher(str(x), self.aws_access_key , self.aws_access_key , self.AHI_endpoint  )) 
         for x in range(self.DICOMizerProcessCount):
-            #logging.debug("[DICOMize] - Spawning AHIDICOMizer thread # "+str(x))
+            self.logger.debug("[DICOMize] - Spawning AHIDICOMizer thread # "+str(x))
             self.frameDICOMizerThreadList.append(AHIDataDICOMizer(str(x) , AHI_metadata )) 
     
     def saveAsDICOM(self, ds : pydicom.Dataset , destination : str = './out' ) -> bool:
         """
         saveAsDICOM(ds : pydicom.Dataset , destination : str).
         Saves a DICOM Part10 file for the DICOM object to the specified destination.
 
@@ -327,10 +329,10 @@
         :param destination: the folder path where to save the DICOM file to. The file name will be the SOPInstanceUID of the DICOM object suffixed by '.dcm'.
         """ 
         try:
             os.makedirs( destination  , exist_ok=True)
             filename = os.path.join( destination , ds["SOPInstanceUID"].value)
             ds.save_as(f"{filename}.dcm", write_like_original=False)
         except Exception as err:
-            logging.error(f"[saveAsDICOM] - {err}")
+            self.logger.error(f"[{__name__}][saveAsDICOM] - {err}")
             return False
         return True
```

### Comparing `AHItoDICOMInterface-0.1.3/AHItoDICOMInterface.egg-info/PKG-INFO` & `AHItoDICOMInterface-0.1.3.1/AHItoDICOMInterface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AHItoDICOMInterface
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: A package to simply export DICOM data from AWS HealthImaging in your application memory or the file system.
 Home-page: https://github.com/aws-samples/healthlake-imaging-to-dicom-python-module
 Author: JP Leger
 Author-email: jpleger@amazon.com
 License: MIT-0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `AHItoDICOMInterface-0.1.3/LICENSE` & `AHItoDICOMInterface-0.1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AHItoDICOMInterface-0.1.3/PKG-INFO` & `AHItoDICOMInterface-0.1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AHItoDICOMInterface
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: A package to simply export DICOM data from AWS HealthImaging in your application memory or the file system.
 Home-page: https://github.com/aws-samples/healthlake-imaging-to-dicom-python-module
 Author: JP Leger
 Author-email: jpleger@amazon.com
 License: MIT-0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `AHItoDICOMInterface-0.1.3/README.md` & `AHItoDICOMInterface-0.1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -60,8 +60,30 @@
 81bfc6aa3416912056e95188ab74870b
 DICOMizing by ImageSetID
 222 DICOMized in 3.3336379528045654.
 Exporting images of the ImageSet in png format.
 Exporting images of the ImageSet in DICOM P10 format.
 ```
 After the example code has returned the file system now contains folders named with the `StudyInstanceUID` of the imageSet exported within the `out` folder. This fodler prefixed with `dcm_` holds the DICOM P10 files for the imageSet. The folder prefixed with `png_` holds PNG image representations of the imageSet. 
+
+## Using this module in Amazon SageMaker
+
+This package can be used in Amazn SageMaker by adding the following code to the SageMaker notebook instance 2 first cells:
+
+### Cell 1
+
+```python
+#Install the python packages
+%%sh
+pip install --upgrade pip --quiet
+pip install boto3 botocore awscliv2 AHItoDICOMInterface --upgrade --quiet
+
 ```
+
+### Cell 2
+
+```python
+#Restart the Kernel to take the new versions of awscliv2 in account.
+import IPython
+IPython.Application.instance().kernel.do_shutdown(True) #automatically restarts kernel
+```
+An example of a SageMaker Jupyter notebook using this module is available in the `example` folder of this repository : [jupyter-sagemaker-example.ipynb](./example/jupyter-sagemaker-example.ipynb)
```

### Comparing `AHItoDICOMInterface-0.1.3/setup.py` & `AHItoDICOMInterface-0.1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup
 
 setup(
     name='AHItoDICOMInterface',
-    version='0.1.3',    
+    version='0.1.3.1',    
     description='A package to simply export DICOM data from AWS HealthImaging in your application memory or the file system.',
     url='https://github.com/aws-samples/healthlake-imaging-to-dicom-python-module',
     long_description='More details about the project and features can be found on the project\'s GitHub page.',
     author='JP Leger',
     author_email='jpleger@amazon.com',
     license='MIT-0',
     packages=['AHItoDICOMInterface'],
     install_requires=[  'boto3',
                         'pydicom',
-                        'pylibjpeg-openjpeg>=1.3.0',
+                        'pylibjpeg-openjpeg>=1.3.1',
                         'numpy',
                         'pillow ',                 
                       ],
 
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
```

