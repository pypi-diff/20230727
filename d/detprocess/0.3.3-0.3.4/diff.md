# Comparing `tmp/detprocess-0.3.3.tar.gz` & `tmp/detprocess-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detprocess-0.3.3.tar", last modified: Thu Mar  2 00:32:04 2023, max compression
+gzip compressed data, was "detprocess-0.3.4.tar", last modified: Thu Jul 27 00:58:44 2023, max compression
```

## Comparing `detprocess-0.3.3.tar` & `detprocess-0.3.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:32:04.708621 detprocess-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-02 00:31:55.000000 detprocess-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-03-02 00:32:04.708621 detprocess-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-03-02 00:31:55.000000 detprocess-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:32:04.704621 detprocess-0.3.3/detprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-02 00:31:55.000000 detprocess-0.3.3/detprocess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:32:04.708621 detprocess-0.3.3/detprocess/core/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-02 00:31:55.000000 detprocess-0.3.3/detprocess/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14971 2023-03-02 00:31:55.000000 detprocess-0.3.3/detprocess/core/_cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-03-02 00:31:55.000000 detprocess-0.3.3/detprocess/core/_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    27728 2023-03-02 00:31:55.000000 detprocess-0.3.3/detprocess/core/_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:32:04.708621 detprocess-0.3.3/detprocess/io/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-02 00:31:55.000000 detprocess-0.3.3/detprocess/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-02 00:31:55.000000 detprocess-0.3.3/detprocess/io/_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-02 00:31:55.000000 detprocess-0.3.3/detprocess/io/_save.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:32:04.708621 detprocess-0.3.3/detprocess/process/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-02 00:31:55.000000 detprocess-0.3.3/detprocess/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-03-02 00:31:55.000000 detprocess-0.3.3/detprocess/process/_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    39762 2023-03-02 00:31:55.000000 detprocess-0.3.3/detprocess/process/_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    18655 2023-03-02 00:31:55.000000 detprocess-0.3.3/detprocess/process/_processing_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:32:04.708621 detprocess-0.3.3/detprocess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-03-02 00:32:04.000000 detprocess-0.3.3/detprocess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-02 00:32:04.000000 detprocess-0.3.3/detprocess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 00:32:04.000000 detprocess-0.3.3/detprocess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 00:32:04.000000 detprocess-0.3.3/detprocess.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-02 00:32:04.000000 detprocess-0.3.3/detprocess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-02 00:32:04.000000 detprocess-0.3.3/detprocess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-02 00:31:55.000000 detprocess-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 00:32:04.708621 detprocess-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-03-02 00:31:55.000000 detprocess-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:58:44.671497 detprocess-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 00:58:32.000000 detprocess-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-07-27 00:58:44.671497 detprocess-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-07-27 00:58:32.000000 detprocess-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:58:44.667497 detprocess-0.3.4/detprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:58:44.671497 detprocess-0.3.4/detprocess/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24863 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/core/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/core/eventbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/core/filterdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21378 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/core/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19125 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/core/oftrigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/core/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:58:44.671497 detprocess-0.3.4/detprocess/process/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/process/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/process/processing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30278 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/process/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36059 2023-07-27 00:58:32.000000 detprocess-0.3.4/detprocess/process/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:58:44.667497 detprocess-0.3.4/detprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-07-27 00:58:44.000000 detprocess-0.3.4/detprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-27 00:58:44.000000 detprocess-0.3.4/detprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:58:44.000000 detprocess-0.3.4/detprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:58:44.000000 detprocess-0.3.4/detprocess.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-27 00:58:44.000000 detprocess-0.3.4/detprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 00:58:44.000000 detprocess-0.3.4/detprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 00:58:32.000000 detprocess-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:58:44.671497 detprocess-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-27 00:58:32.000000 detprocess-0.3.4/setup.py
```

### Comparing `detprocess-0.3.3/LICENSE` & `detprocess-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `detprocess-0.3.3/PKG-INFO` & `detprocess-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: detprocess
-Version: 0.3.3
+Version: 0.3.4
 Summary: Detector Data Processing Package
 Home-page: https://github.com/spice-herald/detprocess
-Author: Samuel Watkins
-Author-email: samwatkins@berkeley.edu
+Author: Bruno Serfass, Samuel Watkins
+Author-email: serfass@berkeley.edu, samwatkins@berkeley.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #  `detprocess`: Detector processing code for feature extraction
 
 [![PyPI](https://img.shields.io/pypi/v/detprocess)](https://pypi.org/project/detprocess/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
```

### Comparing `detprocess-0.3.3/README.md` & `detprocess-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `detprocess-0.3.3/detprocess/process/_features.py` & `detprocess-0.3.4/detprocess/core/algorithms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import qetpy as qp
+from numpy.fft import fftfreq, fft
 
 
 __all__ = [
     'FeatureExtractors',
 ]
 
 
@@ -686,8 +687,85 @@
         en_abs = np.trapz(p0, dx=1/fs, axis=-1)
 
         retdict = {
             feature_base_name: en_abs,
         }
             
         return retdict
-
+        
+        
+    @staticmethod
+    def psd_amp(of_base=None, trace=None, fs=None,
+               f_lims=[],
+               feature_base_name='psd_amp',
+               **kwargs):
+        """
+        Feature extraction for measuring the average amplitude of a
+        ffted trace in a range of frequencies. Rather than recalculating
+        the fft, this feature references the pre-calculated OF class.
+        The arguments "trace", "template", "psd"
+        (and associated parameters "fs", "nb_samples_pretrigger")
+        should only be used if  not already added in OF base object.
+        Otherwise keep as None        
+        
+        Parameters
+        ----------        
+        of_base : OFBase object, optional
+            OFBase  if it has been instantiated independently
+                   
+        trace : ndarray, optional
+            An ndarray containing the raw data to extract the feature
+            from. It is required if trace not already added in OFbase,
+            otherwise keep it as None
+        
+        fs : float, optional
+            If trace is passed, used to construct fft of trace and fft
+            frequencies array.
+            
+        f_lims : list of list of floats
+            A list of [f_low, f_high]s between which the averaged PSD is
+            calculated. For example, [[45.0, 65.0], [120.0, 130.0]]
+            
+        feature_base_name : str, option
+            output feature base name
+            
+        Returns
+        -------
+        retdict : dict
+            Dictionary containing the various extracted features.   
+                 
+        """
+            
+        if of_base is not None:
+            freqs = of_base._fft_freqs
+            trace_psd = np.abs(of_base._signal_fft)
+            
+        else:
+            trace_length = len(trace[0])
+            df = fs/trace_length
+            freqs = fftfreq(trace_length, 1.0/fs)
+            trace_psd = np.abs(fft(trace, axis=-1)/trace_length/df)
+                          
+        i = 0
+        retdict = {}   
+        while i < len(f_lims):
+            f_low = f_lims[i][0]
+            f_high = f_lims[i][1]
+            
+            #round the frequencies so we can more easily look up what
+            #frequencies to average between
+            freq_spacing = freqs[1] - freqs[0]
+            f_low_mod = freq_spacing * np.ceil(f_low/freq_spacing)
+            f_high_mod = freq_spacing * np.floor(f_high/freq_spacing)
+            
+            #get the indices of where to average the psd
+            f_low_index = np.where(freqs == f_low_mod)[0][0]
+            f_high_index = np.where(freqs == f_high_mod)[0][0]
+            
+            #calculate the average psd in that range
+            av_psd = np.average(trace_psd[f_low_index:f_high_index])
+            
+            # store features
+            retdict[feature_base_name + '_' + str(round(f_low)) + '_' + str(round(f_high))] = av_psd            
+            i += 1
+            
+        return retdict
```

### Comparing `detprocess-0.3.3/detprocess/process/_process.py` & `detprocess-0.3.4/detprocess/process/features.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,54 +11,57 @@
 from pprint import pprint
 from multiprocessing import Pool
 from itertools import repeat
 from datetime import datetime
 import stat
 import time
 import astropy
+from humanfriendly import parse_size
 
-from detprocess.process._features  import FeatureExtractors
-from detprocess.process._processing_data  import ProcessingData
+from detprocess.core.algorithms  import FeatureExtractors
+from detprocess.process.processing_data  import ProcessingData
 import pytesdaq.io as h5io
-
+warnings.filterwarnings('ignore')
 
 
 __all__ = [
-    'Processing'
+    'FeatureProcessing'
 ]
 
 
 
 
-class Processing:
+class FeatureProcessing:
     """
     Class to manage data processing and 
     extract features, dataframe can be saved
     in hdf5 using vaex framework and returned
     as a pandas dataframe (not both)
 
     Multiple nodes can be used if data splitted in 
     different series
 
     """
 
     def __init__(self, raw_path, config_file,
-                 external_file=None, series=None,
+                 series=None,
+                 trigger_dataframe_path=None,
+                 external_file=None,
                  processing_id=None,
                  verbose=True):
         """
         Intialize data processing 
         
         Parameters
         ---------
     
         raw_path : str or list of str 
-           raw data group directory OR full path to HDF5  file 
-           (or list of files). Only a single raw data group 
-           allowed 
+           data group directory containing data OR full path to HDF5  file 
+           (or list of files). Data can be either raw data or 
+           vaex dataframes
             
         config_file : str 
            Full path and file name to the YAML settings for the
            processing.
 
         output_path : str, optional (default=No saved file)
            base directory where output feature file will be saved
@@ -87,36 +90,53 @@
 
 
         Return
         ------
         None
         """
 
+        # processing id
+        self._processing_id = processing_id
+        
         # display
         self._verbose = verbose
 
-        # processing ID 
-        self._processing_id = processing_id
-
-        # extract input file list
-        input_file_dict, input_base_path, group_name = (
-            self._get_file_list(raw_path, series=series)
+        # Raw file list
+        raw_files, raw_path, group_name = (
+            self._get_file_list(raw_path,
+                                series=series)
         )
-
-        if not input_file_dict:
-            raise ValueError('No files were found! Check configuration...')
-
-        self._input_base_path = input_base_path
-        self._series_list = list(input_file_dict.keys())
-                  
+        if not raw_files:
+            raise ValueError('No raw data files were found! '
+                             + 'Check configuration...')
+        self._series_list = list(raw_files.keys())
+        self._input_group_name = group_name
+        
+        # Dataframe file list
+        trigger_files = None
+        trigger_path = None
+        trigger_group_name = None
+        
+        if trigger_dataframe_path is not None:
+            
+            trigger_files, trigger_path, trigger_group_name = (
+                self._get_file_list(trigger_dataframe_path,
+                                    is_raw=False)
+            )
+            if not trigger_files:
+                raise ValueError('No dataframe files were found! '
+                                 + 'Check configuration...')
+            
+            self._series_list = list(trigger_files.keys())
+                    
         # processing configuration
         if not os.path.exists(config_file):
             raise ValueError('Configuration file "' + config_file
                              + '" not found!')
-        available_channels = self._get_channel_list(input_file_dict)
+        available_channels = self._get_channel_list(raw_files)
         config, filter_file, selected_channels = (
             self._read_config(config_file, available_channels)
         )
         self._processing_config = config
         self._selected_channels = selected_channels
         
         # check channels to be processed
@@ -134,166 +154,189 @@
                                  + '" not found!')
             self._external_file = external_file
             if self._verbose:
                 print('INFO: External feature extractor = '
                       + self._external_file)
                 
         # get list of available features and check for duplicate
-        self._algorithm_list, self._ext_algorithm_list = self._extract_algorithm_list()
-
-
+        self._algorithm_list, self._ext_algorithm_list = (
+            self._extract_algorithm_list()
+        )
 
-        # instantiate processing data 
-        self._processing_data = ProcessingData(input_file_dict,
-                                               group_name=group_name,
-                                               filter_file=filter_file,
-                                               verbose=verbose)
+        # instantiate processing data
+        self._processing_data = ProcessingData(
+            raw_path,
+            raw_files,
+            group_name=group_name,
+            trigger_files=trigger_files,
+            trigger_group_name =trigger_group_name,
+            filter_file=filter_file,
+            verbose=verbose)
                                 
 
         
-    def process(self, nevents=-1,
-                save_hdf5=True, output_path=None,
+    def process(self,
+                nevents=-1,
+                lgc_save=False, save_path=None,
+                lgc_output=False, 
                 ncores=1,
-                memory_limit_MB=2000):
+                memory_limit='2GB'):
         
         """
         Process data 
         
         Parameters
         ---------
-
+       
         nevents : int, optional
            number of events to be processed
            if not all events, requires ncores = 1
-           Default: all available (=-1)
-            
-
-        save_hdf5 : bool, optional
+           Default: all available (=-1).
+        
+        lgc_save : bool, optional
            if True, save dataframe in hdf5 files
-           (dataframe not returned)
-           if False, return dataframe (memory limit applies
-           so not all events may be processed)
-           Default: True
+           Default: False
+
+        lgc_output : bool, optional
+           if True, return dataframe 
+           Default: False
 
-        output_path : str, optional
+        save_path : str, optional
            base directory where output group will be saved
            default: same base path as input data
     
         ncores: int, optional
            number of cores that will be used for processing
            default: 1
 
-        memory_limit_MB : float, optionl
-           memory limit per file  in MB
-           (and/or if saved_hdf5=False, max dataframe size)
-        
+        memory_limit : str or float, optional
+           memory limit per file, example '2GB', '2MB'
+           if float, then unit is byte
 
         """
 
-
+             
         # check input
         if (ncores>1 and nevents>-1):
             raise ValueError('ERROR: Multi cores processing only allowed when '
                              + 'processing ALL events!')
-        
+
+        if lgc_output and lgc_save:
+            raise ValueError('ERROR: Unable to save and output datafame '
+                             + 'at the same time. Set either lgc_output '
+                             + 'or lgc_save to False.')
+
         # check number cores allowed
         if ncores>len(self._series_list):
             ncores = len(self._series_list)
             if self._verbose:
                 print('INFO: Changing number cores to '
                       + str(ncores) + ' (maximum allowed)')
-
                 
         # create output directory
         output_group_path = None
+        output_series_num = None
         
-        if save_hdf5:
-            if  output_path is None:
-                output_path  = self._input_base_path
-            
-            output_group_path = self._create_output_directory(
-                output_path,
-                self._processing_data.get_facility()
+        if lgc_save:
+            if  save_path is None:
+                save_path  = self._processing_data.get_raw_path()
+                if '/raw' in save_path:
+                    save_path = save_path.replace('/raw','/processed')
+
+            # add group name
+            if self._input_group_name not in save_path:
+                save_path += '/' + self._input_group_name
+
+                    
+            output_group_path, output_series_num = (
+                self._create_output_directory(
+                    save_path,
+                    self._processing_data.get_facility()
+                )
             )
             
             if self._verbose:
                 print(f'INFO: Processing output group path: {output_group_path}')
 
                 
         # instantiate OF object
         # (-> calculate FFT template/noise, optimum filter)
         if self._verbose:
             print('INFO: Instantiate OF base for each channel!')
         
         self._processing_data.instantiate_OF_base(self._processing_config)
         
-                
+        # convert memory usage in bytes
+        if isinstance(memory_limit, str):
+            memory_limit = parse_size(memory_limit)   
 
         # initialize output
         output_df = None
         
         # case only 1 node used for processing
         if ncores == 1:
-            output_df = self._process(-1,
+            output_df = self._process(1,
                                       self._series_list,
                                       nevents,
-                                      save_hdf5,
+                                      lgc_save,
+                                      lgc_output,
+                                      output_series_num,
                                       output_group_path,
-                                      memory_limit_MB)
+                                      memory_limit)
 
         else:
             
             # split data
             series_list_split = self._split_series(ncores)
             
             # for multi-core processing, we need to decrease the
             # max memory so it fits in RAM
-            memory_limit_MB /= ncores
+            memory_limit /= ncores
 
               
             # lauch pool processing
             if self._verbose:
                 print(f'INFO: Processing with be split between {ncores} cores!')
 
             node_nums = list(range(ncores+1))[1:]
             pool = Pool(processes=ncores)
             output_df_list = pool.starmap(self._process,
                                           zip(node_nums,
                                               series_list_split,
                                               repeat(nevents),
-                                              repeat(save_hdf5),
+                                              repeat(lgc_save),
+                                              repeat(lgc_output),
+                                              repeat(output_series_num),
                                               repeat(output_group_path),
-                                              repeat(memory_limit_MB)))
+                                              repeat(memory_limit)))
             pool.close()
             pool.join()
 
             # concatenate
             output_df = pd.concat(output_df_list)
 
 
 
             
         # processing done
         if self._verbose:
             print('INFO: Feature processing done!') 
                 
         
-        if not save_hdf5:
+        if lgc_output:
             return output_df 
         
-            
-
-        
-
-            
-        
+           
     def _process(self, node_num,
                  series_list, nevents,
-                 save_hdf5, output_group_path,
-                 memory_limit_MB):
+                 lgc_save,
+                 lgc_output,
+                 output_series_num,
+                 output_group_path,
+                 memory_limit):
         """
         Process data
         
         Parameters
         ---------
 
         node_num :  int
@@ -303,30 +346,30 @@
           list of series name to be processed
 
         nevents : int, optional
            number of events to be processed
            if not all events, requires ncores = 1
            Default: all available (=-1)
         
-        save_hdf5 : bool, optional
+        lgc_save : bool, optional
            if True, save dataframe in hdf5 files
            (dataframe not returned)
            if False, return dataframe (memory limit applies
            so not all events may be processed)
            Default: True
 
-        output_path : str, optional
+        save_path : str, optional
            base directory where output feature file will be saved
            default: same base path as input data
     
         ncores: int, optional
            number of cores that will be used for processing
            default: 1
 
-        memory_limit_MB : float, optionl
+        memory_limit : float, optionl
            memory limit per file 
            (and/or if return_df=True, max dataframe size)
    
         """
 
         # node string (for display)
         node_num_str = str()
@@ -336,148 +379,146 @@
 
         # feature extractors
         FE = FeatureExtractors
         FE_ext = None
         if self._external_file is not None:
             FE_ext = self._load_external_extractors(self._external_file)
 
-            
-        # intialize event counter
-        # (only used to check maximum
-        # numberof events
-        event_counter = 0
 
 
-        # initialize output data frame
+        # output file name base
+        output_base_file = None
+        if lgc_save:
+            
+            file_prefix = 'feature'
+            if self._processing_id is not None:
+                file_prefix = self._processing_id + '_feature'
+            series_name = h5io.extract_series_name(
+                int(output_series_num+node_num)
+            )
+                    
+            output_base_file = (output_group_path
+                                + '/' + file_prefix
+                                + '_' + series_name)
+
+                
+        # intialize counters
+        dump_counter = 0
+        event_counter = 0
+
+        # initialize data frame
         feature_df = pd.DataFrame()
             
         # loop series
         for series in series_list:
 
-
             if self._verbose:
                 print('INFO' + node_num_str
                       + ': starting processing series '
                       + series)
 
             
             # set file list
             self._processing_data.set_series(series)
 
-            # output file name base (if saving data)
-            output_base_file = None
-            if save_hdf5:
-                
-                file_prefix = 'feature'
-                if self._processing_id is not None:
-                    file_prefix = self._processing_id + '_feature'
-                       
-                output_base_file = (output_group_path
-                                    + '/' + file_prefix
-                                    + '_' + series)
-
-       
-            # initialize dump counter
-            dump_couter = 1
-                        
             # loop events
             do_stop = False
             while (not do_stop):
 
                 # -----------------------
                 # Check number events
                 # and memory usage
                 # -----------------------
 
                 nevents_limit_reached = (nevents>0 and event_counter>=nevents)
                 
                 # flag memory limit reached
-                memory_usage_MB = feature_df.memory_usage(deep=True).sum()/1e6
-                memory_limit_reached =  memory_usage_MB  >= memory_limit_MB
+                memory_usage = feature_df.memory_usage(deep=True).sum()
+                memory_limit_reached =  memory_usage  >= memory_limit
                 
 
                 # display
                 if self._verbose:
-                    
                     if (event_counter%500==0 and event_counter!=0):
                         print('INFO' + node_num_str
                               + ': Local number of events = '
                               + str(event_counter)
-                              + ' (memory = ' + str(memory_usage_MB) + ' MB)')
+                              + ' (memory = ' + str(memory_usage/1e6) + ' MB)')
                         
                 # -----------------------
                 # Read next event
                 # -----------------------
 
                 success = self._processing_data.read_next_event(
                     channels=self._selected_channels
                 )
-                
+
+                # end of file
                 if not success:
                     do_stop = True
 
             
                 # -----------------------
                 # save file if needed
                 # -----------------------
                 
                 # now let's handle case we need to stop
-                # or memory/nb events limit reached
+                # memory/nb events limit reached
+                
                 if (do_stop
                     or nevents_limit_reached
                     or memory_limit_reached):
                     
                     # save file if needed
-                    if save_hdf5:
+                    if lgc_save:
                         
                         # build hdf5 file name
-                        dump_str = '_F'
-                        for ii in range(0,4-len(str(dump_couter))):
-                            dump_str += '0'
-                        dump_str += str(dump_couter)
+                        dump_str = str(dump_counter)
+                        dump_str ='_F' + dump_str.zfill(4)
                         file_name =  output_base_file +  dump_str + '.hdf5'
                     
                         # convert to vaex
                         feature_vx = vx.from_pandas(feature_df,
-                                                    copy_index=True)
+                                                    copy_index=False)
 
 
                         # export
                         feature_vx.export_hdf5(file_name,
                                                mode='w')
                         
                         # increment dump
-                        dump_couter += 1
+                        dump_counter += 1
+                        if not do_stop and self._verbose:
+                            print('INFO' + node_num_str
+                                  + ': Incrementing dump number')
 
-                        # reset dataframe
+                        # initialize
                         del feature_df
                         feature_df = pd.DataFrame()
 
-
+                        
                     # case maximum number of events reached
                     # -> processing done!
                     if nevents_limit_reached:
-                        print('INFO' + node_num_str + ': Requested nb events reached. '
-                                      + 'Stopping processing!')
+                        if self._verbose:
+                            print('INFO' + node_num_str
+                                  + ': Requested nb events reached. '
+                                  + 'Stopping processing!')
                         return feature_df
 
                     # case memory limit reached and not saving file
                     # -> processing done
-                    if memory_limit_reached:
-                        print('INFO' + node_num_str + ': Memory limit reached!')
-                        if save_hdf5:
-                            print('INFO' + node_num_str + ': Starting a new  dump for series '
-                                  + series)
-                        else:
-                            if success:
-                                print('WARNING' + node_num_str + ': Stopping procssing. '
-                                      +' Not all events have been processed!')
-                            return feature_df
-
-
+                    # case memory limit reached
+                    # -> processing needs to stop!
+                    if lgc_output and memory_limit_reached:
+                        raise ValueError(
+                            'ERROR: memory limit reached! '
+                            + 'Change memory limit or only save hdf5 files '
+                            +'(lgc_save=True AND lgc_output=False) '
+                        )
 
 
                 # Now let's stop or increment event counter....
                 if do_stop:
                     break
                 else:
                     event_counter += 1
@@ -488,15 +529,15 @@
                 # -----------------------
 
                 # initialize event features dictionary
                 event_features = dict()
 
                 # update signal trace in OF base objects
                 # -> calculate FFTs, etc.
-                self._processing_data.update_signal_OF()
+                self._processing_data.update_signal_OF(self._processing_config)
 
               
                 # Processing id   
                 event_features.update(
                     {'processing_id': self._processing_id}
                 )
 
@@ -519,38 +560,62 @@
                 for channel, algorithms in self._processing_config.items():
 
                                         
                     # check channel has any parameters
                     if not isinstance(algorithms, dict):
                         continue
 
-
                     # check if feature channel name
                     # is changed by user
                     feature_channel = channel
-                    if 'feature_channel' in algorithms:
+                    if 'feature_channel' in algorithms.keys():
                         feature_channel = algorithms['feature_channel']
+
+                    # number of samples
+                    nb_samples = self._processing_data.get_nb_samples()
+                    if 'nb_samples' in algorithms.keys():
+                        nb_samples = algorithms['nb_samples']
+                    nb_pretrigger_samples = (
+                        self._processing_data.get_nb_samples_pretrigger()
+                    )
+                    if 'nb_pretrigger_samples' in algorithms.keys():
+                        nb_pretrigger_samples = algorithms['nb_pretrigger_samples']
+                    
                         
                     # loop algorithms to extact features
                     for algorithm, algorithm_params in algorithms.items():
 
 
                         # skip if "feature_channel"
                         if algorithm=='feature_channel':
                             continue
+
+                        # skip if nb samples
+                        if (algorithm=='nb_samples'
+                            or  algorithm=='nb_pretrigger_samples'):
+                            continue
                         
                         # skip if algorithm disable
                         if not algorithm_params['run']:
                             continue
                         
                         # check if derived algorithm
                         base_algorithm = algorithm
-                        if 'base_algorithm' in algorithm_params:
+                        if 'base_algorithm' in algorithm_params.keys():
                             base_algorithm = algorithm_params['base_algorithm']
 
+
+                        # check if different number of samples
+                        if 'nb_samples' in algorithm_params.keys():
+                            nb_samples = algorithms['nb_samples']
+                        if 'nb_pretrigger_samples' in algorithm_params.keys():
+                            nb_pretrigger_samples = (
+                                algorithms['nb_pretrigger_samples']
+                            )
+                                                  
                      
                         # get feature extractor
                         extractor = None
                         if base_algorithm in self._algorithm_list:
                             extractor = getattr(FE, base_algorithm)
                         elif base_algorithm in self._ext_algorithm_list:
                             extractor = getattr(FE_ext, base_algorithm)
@@ -565,63 +630,66 @@
                         # add parameter if needed
                         kwargs = {key: value
                                   for (key, value) in algorithm_params.items()
                                   if key!='run'}
 
                         # add various parameters that may be needed
                         # by the algoithm
-                        kwargs['fs'] = self._processing_data.get_sample_rate()
-                        kwargs['nb_samples_pretrigger'] = (
-                            self._processing_data.get_nb_samples_pretrigger()-1
+                        kwargs['fs'] = (
+                            self._processing_data.get_sample_rate()
                         )
-                        kwargs['nb_samples'] = self._processing_data.get_nb_samples()
+                        kwargs['nb_samples_pretrigger'] = nb_pretrigger_samples-1
+                        kwargs['nb_samples'] = nb_samples
                         
                         kwargs['window_min_index'], kwargs['window_max_index'] = (
                             self._get_window_indices(**kwargs)
                         )
 
                         # base feature name = algorithm name
                         kwargs['feature_base_name'] = algorithm
                         
                         # calculate features and get output dictionary 
                         extracted_features = dict()
                         
                         # For OF algorithms, get OB base object
-                        OF_base = self._processing_data.get_OF_base(channel,
-                                                                    algorithm)
+                        OF_base = self._processing_data.get_OF_base(
+                            channel, algorithm)
+                        
                         if OF_base is not None:
                             extracted_features = extractor(OF_base, **kwargs)
                         else:
-                            trace = self._processing_data.get_channel_trace(channel)
+                            trace = self._processing_data.get_channel_trace(
+                                channel,
+                                nb_samples=nb_samples,
+                                nb_pretrigger_samples=nb_pretrigger_samples
+                            )
                             extracted_features = extractor(trace, **kwargs)
 
                                                         
                         # append channel name and save in data frame
                         for feature_base_name in extracted_features:
                             feature_name = f'{feature_base_name}_{feature_channel}'
                             event_features.update(
                                 {feature_name: extracted_features[feature_base_name]}
                             )
 
-
-
-
                 # done processing event!
                 # append event dictionary to dataframe
                 feature_df = feature_df.append(event_features,
                                                ignore_index=True)
            
         # return features
         return feature_df
        
 
 
         
         
-    def _get_file_list(self, file_path, series=None):
+    def _get_file_list(self, file_path, is_raw=True,
+                       series=None):
         """
         Get file list from path. Return as a dictionary
         with key=series and value=list of files
 
         Parameters
         ----------
 
@@ -642,24 +710,26 @@
         base_path :  str
            base path of the raw data
 
         group_name : str
            group name of raw data
 
         """
-        
-        # loop file path
-        if not isinstance(file_path, list):
-            file_path = [file_path]
 
+        # convert file_path to list 
+        if isinstance(file_path, str):
+            file_path = [file_path]
+            
+            
         # initialize
         file_list = list()
         base_path = None
         group_name = None
 
+
         # loop files 
         for a_path in file_path:
 
                    
             # case path is a directory
             if os.path.isdir(a_path):
 
@@ -712,52 +782,75 @@
                                  + '" does not exist!')
             
         if not file_list:
             raise ValueError('ERROR: No raw input data found. Check arguments!')
 
         # sort
         file_list.sort()
+
+
+        
       
-        # get list of series
+        # convert to series dictionary so can be easily split
+        # in multiple cores
+        
         series_dict = dict()
         h5reader = h5io.H5Reader()
         series_name = None
         file_counter = 0
+        
         for file_name in file_list:
 
             # skip if filter file
             if 'filter' in file_name:
                 continue
+
+            # skip didv
+            if 'didv' in file_name:
+                continue
             
             # append file if series already in dictionary
             if (series_name is not None
                 and series_name in file_name
                 and series_name in series_dict.keys()):
 
                 if file_name not in series_dict[series_name]:
                     series_dict[series_name].append(file_name)
                     file_counter += 1
                 continue
             
             # get metadata
-            metadata = h5reader.get_metadata(file_name)
-            series_name = h5io.extract_series_name(metadata['series_num'])
+            if is_raw:
+                metadata = h5reader.get_metadata(file_name)
+                series_name = h5io.extract_series_name(metadata['series_num'])
+            else:
+                series_name =str(Path(file_name).name)
+                sep_start = series_name.find('_I')
+                sep_end = series_name.find('_F')
+                series_name = series_name[sep_start+1:sep_end]
+
+                
             if series_name not in series_dict.keys():
                 series_dict[series_name] = list()
 
             # append
             if file_name not in series_dict[series_name]:
                 series_dict[series_name].append(file_name)
                 file_counter += 1
                 
 
         if self._verbose:
+            msg = ' raw data file(s) with '
+            if not is_raw:
+                msg = ' dataframe file(s) with '
+                
             print('INFO: Found total of '
                   + str(file_counter)
-                  + ' files from ' + str(len(series_dict.keys()))
+                  + msg
+                  + str(len(series_dict.keys()))
                   + ' different series number!')
 
       
         return series_dict, base_path, group_name
 
 
 
@@ -840,14 +933,18 @@
             raise ValueError('Unable to read processing configuration!')
 
 
         # Let's check for unallowed duplication
         key_list = list()
         key_list_duplicate = list()
         for key in yaml_dict.keys():
+            
+            if key=='trigger' or key=='filter':
+                continue
+            
             if ',' in key:
                 key_split = key.split(',')
                 for key_sep in key_split:
                     if key_sep in key_list:
                         key_list_duplicate.append(key_sep)
                     else:
                         key_list.append(key_sep)
@@ -877,15 +974,18 @@
         # loop config to load individual channels
         for key in yaml_dict.keys():
                      
             # skip "all" and "filter_file"
             # (already taking into account)
             if (key=='filter_file' or key=='all'):
                 continue
-
+            
+            # skip trigger or filter
+            if key=='trigger' or key=='filter':
+                continue
             
             # check if key contains a comma 
             # -> need to split 
             key_split = list()
             if ',' in key:
                 key_split = key.split(',')
             else:
@@ -930,21 +1030,23 @@
             chans = list()
             if ',' in key:
                 chans = key.split(',')
             elif '|' in key:
                 chans = key.split('|')
             elif '+' in key:
                 chans = key.split('+')
+                # elif '-' in key:
+                # chans = key.split('-')
             elif key != 'filter_file':
                 chans.append(key)
                 
             for chan in chans:
                 if chan not in available_channels:
                     raise ValueError('Channel "' + chan
-                                     + '" do not exist in '
+                                     + '" does not exist in '
                                      + 'raw data! Check yaml file!')
                 else:
                     channel_list_temp.append(chan)
 
         # make list unique
         for chan in available_channels:
             if chan in channel_list_temp:
@@ -976,14 +1078,16 @@
         """
 
         now = datetime.now()
         series_day = now.strftime('%Y') +  now.strftime('%m') + now.strftime('%d') 
         series_time = now.strftime('%H') + now.strftime('%M')
         series_name = ('I' + str(facility) +'_D' + series_day + '_T'
                        + series_time + now.strftime('%S'))
+
+        series_num = h5io.extract_series_num(series_name)
         
         # prefix
         prefix = 'feature'
         if self._processing_id is not None:
             prefix = self._processing_id + '_feature'
         output_dir = base_path + '/' + prefix + '_' + series_name
         
@@ -991,15 +1095,15 @@
         if not os.path.isdir(output_dir):
             try:
                 os.makedirs(output_dir)
                 os.chmod(output_dir, stat.S_IRWXG | stat.S_IRWXU | stat.S_IROTH | stat.S_IXOTH)
             except OSError:
                 raise ValueError('\nERROR: Unable to create directory "'+ output_dir  + '"!\n')
                 
-        return output_dir
+        return output_dir, series_num
         
 
 
 
     
     def _extract_algorithm_list(self):
         """
@@ -1224,7 +1328,9 @@
             raise ValueError('ERROR window calculation: '
                              + 'max index smaller than min!'
                              + 'Check configuration!')
 
         
 
         return min_index, max_index
+        
+
```

### Comparing `detprocess-0.3.3/detprocess/process/_processing_data.py` & `detprocess-0.3.4/detprocess/core/oftrigger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,719 +1,534 @@
 import numpy as np
-import pandas as pd
-import qetpy as qp
-import sys
-from pprint import pprint
-import pytesdaq.io as h5io
+import os
+from math import log10, floor
+import math
+import array
+from scipy.signal import correlate
+from scipy.fft import ifft, fft, next_fast_len
+import vaex as vx
 
 
 
-__all__ = [
-    'ProcessingData'
-]
+__all__ = ['OptimumFilterTrigger']
 
 
-class ProcessingData:
+def _getchangeslessthanthresh(x, threshold):
     """
-    Class to manage data used for processing,
-    in particular  
-      - raw data filew, event traces and metadata
-      - filter file data
-      - optimal filter objects containing template/PSD FFTs, etc.
+    Helper function that returns a list of the start and ending indices
+    of the ranges of inputted values that change by less than the
+    specified threshold value.
+
+    Parameters
+    ----------
+    x : ndarray
+        1-dimensional of values.
+    threshold : int
+        Value to detect the different ranges of vals that change by
+        less than this threshold value.
+
+    Returns
+    -------
+    ranges : ndarray
+        List of tuples that each store the start and ending index of
+        each range. For example, vals[ranges[0][0]:ranges[0][1]] gives
+        the first section of values that change by less than the
+        specified threshold.
+    vals : ndarray
+        The corresponding starting and ending values for each range in
+        x.
 
     """
 
-    def __init__(self, input_files, group_name=None,
-                 filter_file=None, verbose=True):
-        """
-        Intialize data processing 
-        
-        Parameters
-        -----------
+    diff = x[1:]-x[:-1]
+    a = diff>threshold
+    inds = np.where(a)[0]+1
 
-        input_files : list
-           list of raw data files to be processed
+    start_inds = np.zeros(len(inds)+1, dtype = int)
+    start_inds[1:] = inds
 
-        group_name : str, optional
-           raw data group name
-           default: None
-
-        filter_file : str, optional
-          full path to filter file
-          default: None
-
-        verbose :  bool, optional 
-          if True, display info
-           Default: True
-    
-        """
+    end_inds = np.zeros(len(inds)+1, dtype = int)
+    end_inds[-1] = len(x)
+    end_inds[:-1] = inds
 
-        # verbose
-        self._verbose = verbose
+    ranges = np.array(list(zip(start_inds,end_inds)))
 
-        # input files
-        self._input_file_dict = input_files
+    if len(x)!=0:
+        vals = np.array([(x[st], x[end-1]) for (st, end) in ranges])
+    else:
+        vals = np.array([])
 
-        # group_name
-        self._group_name = group_name
-        
-        # filter data
-        self._filter_data = None
-        if filter_file is not None:
-            filter_inst = h5io.FilterH5IO(filter_file)
-            self._filter_data = filter_inst.load()
-            if self._verbose:
-                print('INFO: Filter file '
-                      + filter_file
-                      + ' has been successfully loaded!')
-                
-        
-        # initialize OF containers
-        self._OF_base_objs = dict()
-        self._OF_algorithms = dict()
-        
-        # initialize raw data reader
-        self._h5 = h5io.H5Reader()
+    return ranges, vals
 
-        # initialize event traces and metadata 
-        self._event_traces  = None
-        self._event_info = None
 
-        # get ADC and file info
-        self._data_info = self._extract_data_info()
-      
+class OptimumFilterTrigger:
+    """
+    Class for applying a time-domain optimum filter to a long trace,
+    which can be thought of as an FIR filter.
 
+    Attributes
+    ----------
+    phi : ndarray 
+        The optimum filter in time-domain, equal to the inverse FT of
+        (FT of the template/power spectral density of noise)
+    norm : float
+        The normalization of the optimal amplitude.
+    fs : float
+        The sample rate of the data (Hz).
+    traces : ndarray
+        Trace(s) to be filtered, assumed to be an ndarray of
+        shape 1D or 2D = (# of channels, # of trace bins). Should
+        be in units of Amps.
+    template : ndarray
+        The template that will be used for the Optimum Filter.
+    noisepsd : ndarray
+        The two-sided noise PSD that will be used to create the Optimum
+        Filter.
+    filtered_trace : ndarray 
+        The result of the FIR filter on each of the traces.
+    resolution : float
+        The expected energy resolution in Amps given by the template
+        and the noisepsd, calculated from the Optimum Filter.
 
-    @property
-    def verbose(self):
-        return self._verbose
 
-                
+    """
+
+    def __init__(self, trigger_channel,
+                 fs, template, noisepsd,
+                 pretrigger_samples,
+                 template_ttl=None):
+        """
+        Initialization of the FIR filter.
+       
+        ----------
+        trigger_channel : str or list of str
+            the channel name (s) of the trigger. In case of NxM trigger, 
+            it can be a list of channels
+        fs : float
+            The sample rate of the data (Hz)
+        template : ndarray
+            The pulse template(s) to be used when creating the optimum
+            filter (assumed to be normalized)
+            For single pulse trigger: 1D array or 2D array [1, samples]
+            For NxM trigger: 2D array [channel, samples] 
+        noisepsd : ndarray
+            The two-sided power spectral density in units of A^2/Hz
+         template_ttl : NoneType, ndarray, optional
+            The template for the trigger channel pulse. If left as
+            None, then the trigger channel will not be analyzed.
         
-    def instantiate_OF_base(self, processing_config, channel=None):
         """
-        Instantiate QETpy OF base class, perform pre-calculations 
-        such as FFT, etc
 
-        Parameters
-        ----------
-        
-        processing_config : dict
-         disctionary with processing user config (loaded
-         from yaml file)
+        # save internal variable
+        self._fs = fs
+        self._template = template
+        self._noisepsd = noisepsd
+        self._trigger_channel = trigger_channel
+        self._pretrigger_samples = pretrigger_samples
+        self._nb_samples = self._template.shape[-1]
+        self._posttrigger_samples = self._nb_samples - self._pretrigger_samples
+
+        # trigger index shift if pretrigger not midpoint
+        self._trigger_index_shift = self._pretrigger_samples - self._nb_samples//2
+        
+        # check array shapes
+        #if isinstance(trigger_channel, str):   
+        #    trigger_channel = [trigger_channel]
+
+        # intitialize trigger data
+        # dictionary 
+        self._trigger_data = None
+  
+        
+        # calculate the time-domain optimum filter
+        phi_freq = fft(self._template) / self._noisepsd
+        phi_freq[0] = 0 #ensure we do not use DC information
+        self._phi = ifft(phi_freq).real
 
-        channel : str. optional
-          channel name
-          Default: all channels from config
         
-        """
-
-        # check if filter file data available
-        if self._filter_data is None:
-            if self._verbose:
-                print('INFO: No filter file available. Skipping '
-                      + ' OF instantiation!')
-    
+        # calculate the normalization of the optimum filter
+        self._norm = np.dot(self._phi, self._template)
         
-        # check channel
-        if (channel is not None
-            and channel not in processing_config.keys()):
-            raise ValueError('No channel ' + channel
-                             + ' found in configuration file!')
-        
-        
-        # loop channels
-        for chan, chan_config in processing_config.items():
-
-            # skip if filter file
-            if (chan == 'filter_file'
-                or not isinstance(chan_config, dict)):
-                continue
-
-            # skip if not selected channel
-            if (channel is not None
-                and channel != chan):
-                continue
-
-            
-            # loop configuration and get list of templates
-            for alg, alg_config in chan_config.items():
-
-                if alg.find('of1x')==-1:
-                    continue
-                
-                # psd
-                psd_tag = 'default'
-                if 'psd_tag' in alg_config.keys():
-                    psd_tag = alg_config['psd_tag']
-
-                # check if OF already instantiated
-                if chan not in self._OF_base_objs.keys():
-                    self._OF_base_objs[chan] = dict()
+        # calculate the expected energy resolution
+        self._resolution = 1/(np.dot(self._phi, self._template)/self._fs)**0.5
 
-                # instantiate
-                if psd_tag not in self._OF_base_objs[chan].keys():
-                    
-                    # get psd
-                    psd, psd_fs = self.get_psd(chan, psd_tag)
-                    
-                    # coupling
-                    coupling = 'AC'
-                    if 'coupling' in alg_config.keys():
-                        coupling = alg_config['coupling']
-                        
-                        
-                    # check sample rate
-                    sample_rate = self.get_sample_rate()
-                    if (psd_fs is not None
-                        and  (psd_fs != sample_rate)):
-                        raise ValueError('Sample rate for PSD is '
-                                         + 'inconsistent with data!')
-                       
-
-                    # get pretrigger samples
-                    pretrigger_samples = self.get_nb_samples_pretrigger()
-
-
-                    # instantiate
-                    self._OF_base_objs[chan][psd_tag] = qp.OFBase(
-                        sample_rate,
-                        pretrigger_samples=pretrigger_samples,
-                        channel_name=chan
-                    )
-
-
-                    # set psd
-                    self._OF_base_objs[chan][psd_tag].set_psd(
-                        psd,
-                        coupling=coupling,
-                        psd_tag=psd_tag)
-                        
-                                                
-
-                # check if there are template tag(s)
-                tag_list = list()
-                for key in alg_config.keys():
-                    if key.find('template_tag')!=-1:
-                        tag_list.append(
-                            alg_config[key]
-                        )
-
-                if not tag_list:
-                    tag_list = ['default']
-
-                integralnorm=False
-                if 'integralnorm' in alg_config.keys():
-                    integralnorm = alg_config['integralnorm']
-                        
-                for tag in tag_list:
-                    template_list = self._OF_base_objs[chan][psd_tag].template_tags()
-                    if tag not in template_list:
-                        # get template from filter file
-                        template = self.get_template(chan, tag)
-
-                        #  add
-                        self._OF_base_objs[chan][psd_tag].add_template(
-                            template,
-                            template_tag=tag,
-                            integralnorm=integralnorm
-                        )
                             
-                        
-                # save algorithm name and psd/signal tag
-                if chan not in self._OF_algorithms:
-                    self._OF_algorithms[chan] = dict()
-                self._OF_algorithms[chan][alg] = psd_tag
-
-            # calculate phi
-            if chan in self._OF_base_objs.keys():
-                for tag in self._OF_base_objs[chan].keys():
-                    self._OF_base_objs[chan][tag].calc_phi()
-                        
-    def get_OF_base(self, channel, alg_name):
-        """
-        Get OF object 
-
-        Parameters
-        ----------
-
-        channel : str
-          channel name 
-
-        alg_name : str
-          algorithm name 
-
-        Return
-        ------
-        
-        OF : object 
-          optiomal filter base instance
+        # TTL template and norm
+        self._template_ttl = template_ttl
+        self._norm_ttl = None
+        if template_ttl is not None:
+            self._norm_ttl = np.dot(template_ttl, template_ttl)
+    
 
+    def get_filtered_trace(self):
         """
-        
-        OF = None
-
-        # get OF base
-        tag = str()
-        if (channel in self._OF_algorithms.keys()
-            and alg_name in self._OF_algorithms[channel].keys()):
-
-            tag = self._OF_algorithms[channel][alg_name]
-
-            OF = self._OF_base_objs[channel][tag]
-
-        return OF
-
-        
-                
-                    
-    def get_template(self, channel, tag=None):
+        Get current filtered trace
         """
-        Get template from filter file
-        
-        Parameters
-        ----------
-
-        channel : str
-          channel name 
 
-
-        tag : str
-          tag/ID of the template
-          Default: None
-
-        Return
-        ------
-
-        template : ndarray
-          array with template values
+        return self._filtered_trace
 
 
+    def get_filtered_trace_ttl(self):
+        """
+        Get current filtered trace
         """
-        
-        # check if channel in filter_file
-        if channel not in self._filter_data:
-            raise ValueError('No channel ' + channel
-                             + ' found in filter file!')
-
-        # check if template in filter file
-        template_name = 'template'
-        if tag is not None and tag != 'default':
-            template_name += '_' + tag
-
-        if template_name not in self._filter_data[channel]:
-            raise ValueError('No parameter "' + template_name
-                             + '" found in filter file!'
-                             + ' for channel ' + channel)
 
-        return self._filter_data[channel][template_name].values
+        return self._filtered_trace_ttl
 
 
     
-    def get_psd(self, channel, tag=None):
+    def get_trigger_data(self):
         """
-        Get psd from filter file
-
-          
-        Parameters
-        ----------
-
-        channel : str
-          channel name 
-
-
-        tag : str
-          tag/ID of the PSD
-          Default: None
-
-        Return
-        ------
-
-        psd : ndarray
-          array with psd values
-
-        freq : ndarray
-          array with psd frequencies
-
-
+        Get current filtered trace
         """
-        
-        # check if channel in filter_file
-        if channel not in self._filter_data:
-            raise ValueError('No channel ' + channel
-                             + ' found in filter file!')
 
-        # check if psd in filter file
-        psd_name = 'psd'
-        if tag is not None and tag != 'default':
-            psd_name += '_' + tag
+        return self._trigger_data
 
-        
-
-        if psd_name not in self._filter_data[channel]:
-            raise ValueError('No parameter "' + psd_name
-                             + '" found in filter file!'
-                             + ' for channel ' + channel)
-
-        # FIXME add fs
-        return self._filter_data[channel][psd_name].values, None
-    
-
-
-    def set_series(self, series):
+    def get_trigger_data_df(self):
         """
-        Set file list for a specific 
-        series
-
-        Parameters
-        ----------
-
-        series : str
-          series name
-
-        Return
-        ------
-        None
-
+        Get current filtered trace
         """
+        df = None
+        if self._trigger_data is not None:
+            df = vx.from_dict(
+                self._trigger_data[self._trigger_channel]
+            )
+        return df
+           
 
-        file_list = self._input_file_dict[series]
-        
-        # Set files
-        self._h5.set_files(file_list)
-        
-    
-        
-    def read_next_event(self, channels=None):
+    def get_phi(self):
         """
-        Read next event
+        Get optimal filter 
+        in time domain
         """
 
-        self._event_traces, self._event_info = self._h5.read_next_event(
-            detector_chans=channels,
-            adctoamp=True,
-            include_metadata=True
-        )    
+        return self._phi
 
-
-        # if end of file, traces will be empty
-        if self._event_traces.size != 0:
-            return True
-        else:
-            return False
-        
-
-    def update_signal_OF(self):
+    
+    def get_norm(self):
+        """
+        Get normalization
         """
-        Update OF base object with traces
 
-        Parameters
-        ---------
-        None
+        return self._norm
 
-        Return
-        ------
-        None
 
+    def get_resolution(self):
         """
-        
-        # loop OF and update traces
-        for channel, channel_dict in self._OF_base_objs.items():
-            trace = self.get_channel_trace(channel)
-            for tag, OF_base in channel_dict.items():
-                OF_base.update_signal(trace)
-                
-                
-
-    def get_event_admin(self):
+        Get resolution
         """
-        Get event admin info
-
-        Parameters
-        ---------
-        None
-
-        Return
-        ------
-        admin_dict : dict
-          dictionnary with various admin and trigger variables
+        return self._resolution
+    
 
+            
+    def update_trace(self, trace=None, filtered_trace=None,
+                     filtered_trace_ttl=None):
         """
+        Method to apply the FIR filter the inputted traces with
+        specified times.
 
-        admin_dict = dict()
-
-        if self._event_info is None:
-            return admin_dict
-        
-        # fill dictionary
-        admin_dict['event_number'] = np.int64(self._event_info['event_num'])
-        admin_dict['event_index'] = np.int32(self._event_info['event_index'])
-        admin_dict['dump_number'] = np.int16(self._event_info['dump_num'])
-        admin_dict['series_number'] = np.int64(self._event_info['series_num'])
-        admin_dict['event_id'] = np.int32(self._event_info['event_id'])
-        admin_dict['event_time'] = self._event_info['event_time']
-        admin_dict['run_type'] = np.int16(self._event_info['run_type'])
+        Parameters
+        ----------
 
-        if self._group_name is not None:
-            admin_dict['group_name'] = self._group_name
-        else:
-            admin_dict['group_name'] = np.nan
+        trace : ndarray, optional
+            trigger channel trace(s) to be filtered
+            units: Amps, should be positive going
+            For single pulse trigger: 1D array or 2D array [1, samples]
+            For NxM trigger: 2D array [channel, samples] 
+            Default: None (required "filtered_trace")
+           
+        filtered_trace : ndarray, optional
+            OF filtered trigger channel trace(s)
+            units: Amps
+            For single pulse trigger: 1D array or 2D array [1, samples]
+            For NxM trigger: 2D array [channel, samples] 
+
+        filtered_trace_ttl: ndarray, optional
+            OF filtered trigger channel trace(s) with TTL template
+            units: Amps
+            1D array or 2D array [#channels, #samples]
+            For single pulse channel: #channels=1
+        """
+
+        # check input
+        if trace is None and filtered_trace is None:
+            raise ValueError(
+                'ERROR: "trace" or "filtered_trace required!'
+            )
+
+
+        # check dimension trace here
+        # FIXME
+
+        # update the traces, times, and ttl attributes
+        self._raw_trace = trace
+        self._filtered_trace = filtered_trace
+                  
+        # filter trace 
+        if self._filtered_trace is None:
+            self._filtered_trace = correlate(trace,
+                                             self._phi,
+                                             mode='same',
+                                             method='fft')/self._norm
             
-        # trigger info
-        if 'trigger_type' in self._event_info:
-            admin_dict['trigger_type'] = np.int16(self._event_info['trigger_type'])
-        else:
-            data_mode =  self._event_info['data_mode']
-            data_modes = ['cont', 'trig-ext', 'rand', 'threshold']
-            if  data_mode  in data_modes:
-                admin_dict['trigger_type'] = data_modes.index(data_mode)+1
-            else:
-                admin_dict['trigger_type'] = np.nan
         
-        if  'trigger_amplitude' in self._event_info:
-            admin_dict['trigger_amplitude'] = self._event_info['trigger_amplitude']
-        else:
-            admin_dict['trigger_amplitude'] = np.nan
+        # set the filtered values to zero near the edges,
+        # so as not to use the padded values in the analysis
+        cut_len =  self._phi.shape[-1]
+        self._filtered_trace[:cut_len] = 0.0
+        self._filtered_trace[-(cut_len)
+                             +(cut_len+1)%2:] = 0.0
+        
+        # filtered with ttl template
+        self._filtered_trace_ttl = filtered_trace_ttl
+        if self._template_ttl is not None:
+            self._filtered_trace_ttl = correlate(
+                trace,
+                self._template_ttl,
+                mode="same",
+                method='fft')/self._norm_ttl      
+
+            self._filtered_trace_ttl[:cut_len] = 0.0
+            self._filtered_trace_ttl[-(cut_len)
+                                     + (cut_len+1)%2:] = 0.0
+         
+            
+            
 
-        if  'trigger_time' in self._event_info:
-            admin_dict['trigger_time'] = self._event_info['trigger_time']
+            
+    def find_triggers(self, thresh, thresh_ttl=None,
+                      pileup_window_msec=None, pileup_window_samples=None,
+                      positive_pulses=True):
+        """
+        Method to detect events in the traces with an optimum amplitude
+        greater than the specified threshold. Note that this may return
+        duplicate events, so care should be taken in post-processing to
+        get rid of such events.
+
+        Parameters
+        ----------
+        thresh : float
+            The number of standard deviations of the energy resolution
+            to use as the threshold for which events will be detected
+            as a pulse.
+        thresh_ttl : NoneType, float, optional
+            The threshold value (in units of the ttl channel) such
+            that any amplitudes higher than this will be detected as
+            ttl trigger event. If left as None, then only the pulses
+            are analyzed.
+
+
+        pileup_window_msec : float, optional
+
+        pileup_window_samples : int, optional
+        
+        positive_pulses : boolean, optional
+            Boolean flag for which direction the pulses go in the
+            traces. If they go in the positive direction, then this
+            should be set to True. If they go in the negative
+            direction, then this should be set to False. Default is
+            True.
+
+        """
+
+        # check filtered trace
+        if self._filtered_trace is None:
+            raise ValueError('ERROR: Filter trace not available. '
+                             + ' Use "update_trace" first!')
+        
+        
+        # intialize dictionary with list of
+        # variables
+        trigger_data = {
+            'trigger_amplitude':list(),
+            'trigger_time': list(),
+            'trigger_index': list(),
+            'trigger_pileup_window': list(),
+            'trigger_threshold_sigma': list(),
+            'trigger_type': list()}
+        
+        # Extra parameters if TTL trigger used
+        if (self._filtered_trace_ttl is not None
+            and thresh_ttl is not None):
+            trigger_data.update(
+                {'trigger_time_ttl': list(),
+                 'trigger_index_ttl': list(),
+                 'trigger_amplitude_ttl': list(),
+                 'trigger_time_pulse': list(),
+                 'trigger_index_pulse': list(),
+                 'trigger_amplitude_pulse': list()}
+            )
+               
+        # merge window
+        pileup_window = 0
+        if pileup_window_msec is not None:
+            pileup_window = int(pileup_window_msec*self._fs/1000)
+        elif pileup_window_samples is not None:
+            pileup_window = pileup_window_samples
+            
+                
+        # find where the filtered trace has an optimum amplitude
+        # greater than the specified amplitude
+        if positive_pulses:
+            triggers_mask = self._filtered_trace>thresh*self._resolution
         else:
-            admin_dict['trigger_time'] = np.nan 
-
-
-        return admin_dict
-
-
-
-    def get_channel_settings(self, channel):
-        """
-        Get channel settings dictionary
-
-        Parameters
-        ---------
+            triggers_mask = self._filtered_trace<-thresh*self._resolution
+            
+        triggers = np.where(triggers_mask)[0]
         
-        channel : str
-           channel can be a single channel
-           or sum of channels "chan1+chan2"
-           or multiple channels "chan1|chan2"     
+        # check if any left over detected triggers are within
+        # the specified pulse_range from each other
+        trigger_ranges, trigger_vals = _getchangeslessthanthresh(
+            triggers, pileup_window)
         
-
-        Return
-        ------
-        settings_dict : dict
-          dictionnary with various detector settings variable
-
-        """
-
-        # initialize output
-        settings_dict = dict()
-
-
-        # check info filled
-        if (self._event_info is None or
-            'detector_config' not in self._event_info):
-            return admin_dict
-
+        # set the trigger type to pulses
+        rangetypes = np.zeros((len(trigger_ranges), 3), dtype=bool)
+        rangetypes[:,1] = True
         
-        # channel list 
-        channels = list()  
-        if '+' in channel:
-            channels = channel.split('+')
-        elif '|' in channel:
-            channels = channel.split('|')
-        else:
-            channels = [channel]
 
-        # fill dictionary
-        for chan in channels:
-            settings_dict['tes_bias_' + chan] =  (
-                self._event_info['detector_config'][chan]['tes_bias'])
-            settings_dict['output_gain_' + chan] =  (
-                self._event_info['detector_config'][chan]['output_gain'])
+        # TTL trigger
+        if (self._filtered_trace_ttl is not None
+            and thresh_ttl is not None):
             
-        return settings_dict
-
-     
-                
-    def get_channel_trace(self, channel):
-        """
-        Get trace (s)
-
-        Parameters
-        ----------
-
-        channel : str
-           channel can be a single channel
-           or sum of channels "chan1+chan2"
-           or multiple channels "chan1|chan2"     
-   
-        Return:
-        -------
-        array : ndarray
-          array with trace values
-
-        """
-
-        array = []
-
-        #  get channels for case + or | used 
-        channels = list()
+            # make a boolean mask of the ranges of the events in the trace
+            # from the pulse triggering
+            pulse_mask = np.zeros(self._filtered_trace.shape, dtype=bool)
+            for evt_range in trigger_ranges:
+                if evt_range[1]>evt_range[0]:
+                    trigger_inds = triggers[evt_range[0]:evt_range[1]]
+                    pulse_mask[trigger_inds] = True
+                    
+            # find where the ttl trigger has an optimum amplitude
+            # greater than the specified threshold
+            triggers_mask_ttl = self._filtered_trace_ttl>thresh_ttl
+
+            # get the mask of the total events, taking the
+            # or of the pulse and ttl trigger events
+            tot_mask = np.logical_or(triggers_mask_ttl, pulse_mask)
+            triggers = np.where(tot_mask)[0]
+            trigger_ranges, trigger_vals = _getchangeslessthanthresh(
+                triggers,  pileup_window)
             
-        if '+' in channel:
-            channels = channel.split('+')
-        elif '|' in channel:
-            channels = channel.split('|')
-        else:
-            channels = [channel]
-
-        # get indicies
-        trace_indices = list()
-        for chan in channels:
-            trace_indices.append(self._event_info['detector_chans'].index(chan))
-
-        if not trace_indices:
-            raise ValueError('Unable to get event  traces for '
-                             + channel)
-
-        # build array
-        if '+' in channel:
-            array = np.sum(self._event_traces[trace_indices,:],
-                           axis = 0)
-        elif '|' in channel:
-            array =  self._event_traces[trace_indices,:]
-        else:
-            array =  self._event_traces[trace_indices[0],:]
-
-        return array
-
-    def get_facility(self):
-        """
-        Function to extract facility # from
-        metadata
-
-        Parameters
-        ----------
-        None
-
-        Return
-        ------
-
-        facility : int
-         facility number    
-
-        """
-        facility = None
-        if 'facility' in self._data_info.keys():
-            facility = self._data_info['facility']
-
-        return facility
-
-    def get_sample_rate(self):
-        """
-        Function to extract sample rate from
-        metadata
-
-        Parameters
-        ----------
-        None
-
-        Return
-        ------
-
-        sample_rate : float
-         ADC sample rate used to take data 
-
-
-        """
-        sample_rate = None
-        if 'sample_rate' in self._data_info.keys():
-            sample_rate = self._data_info['sample_rate']
-
-        return sample_rate
-    
-    def get_nb_samples(self):
-        """
-        Function to extract number of samples information 
-        from metadata
-
-        Parameters
-        ----------
-        None
-
-        Return
-        ------
-
-        nb_samples : int
-         number of samples of the traces
-
-        """
-        nb_samples = None
-        if 'nb_samples' in self._data_info.keys():
-             nb_samples = self._data_info['nb_samples']
-
-        return nb_samples
-
-    
-    def get_nb_samples_pretrigger(self):
-        """
-        Function to extract number of pretrigger samples 
-        information  from metadata
-
-        Parameters
-        ----------
-        None
-
-        Return
-        ------
-
-        nb_samples : int
-         number of pretrigger samples
-
-
-
-        """
-        nb_samples_pretrigger = None
-        if 'nb_samples_pretrigger' in self._data_info.keys():
-             nb_samples_pretrigger = self._data_info['nb_samples_pretrigger']
+            tot_types = np.zeros(len(tot_mask), dtype=int)
+            tot_types[triggers_mask] = 1
+            tot_types[triggers_mask_ttl] = 2
+            
+            # given the ranges, determine the trigger type based on if
+            # the total ranges overlap with
+            # the pulse events and/or the ttl trigger events
+            rangetypes = np.zeros((len(trigger_ranges), 3), dtype=bool)
+            for ival, vals in enumerate(trigger_vals):
+                if np.any(tot_types[vals[0]:vals[1]]==1):
+                    rangetypes[ival, 1] = True
+                if np.any(tot_types[vals[0]:vals[1]]==2):
+                    rangetypes[ival, 2] = True
 
-        return nb_samples_pretrigger
 
+                    
+        # for each range with changes less than the merge_windw
+        # keep only the bin with the largest amplitude
+        for irange, evt_range in enumerate(trigger_ranges):
+                
+            if evt_range[1]>evt_range[0]:
 
-    
-    def _extract_data_info(self):
-        """
-        Function to extract all metadata
-        from raw data
+                evt_inds = triggers[evt_range[0]:evt_range[1]]
 
-        Parameters
-        ----------
-        None
+                # find index maximum amplitude
+                evt_ind = None
+                if positive_pulses:
+                    evt_ind = evt_inds[np.argmax(self._filtered_trace[evt_inds])]
+                else:
+                    evt_ind = evt_inds[np.argmin(self._filtered_trace[evt_inds])]
 
-        Return
-        ------
+                evt_ind_shift = evt_ind + self._trigger_index_shift
 
-        data_info : dict
-         dictionary with ADC/data information
+                    
+                # Case TTL is used
+                if (self._filtered_trace_ttl is not None
+                    and thresh_ttl is not None):
+
+                    # TTL index
+                    ttl_ind = evt_inds[np.argmax(self._filtered_trace_ttl[evt_inds])]
+                    ttl_ind_shift = ttl_ind + self._trigger_index_shift
+                        
+                    # case trigger TTL -> primary
+                    if rangetypes[irange][2]:
 
+                        # primary = TTL
+                        trigger_data['trigger_index'].extend([ttl_ind_shift])
+                        trigger_data['trigger_time'].extend([ttl_ind_shift/self._fs])
+                        trigger_data['trigger_amplitude'].extend(
+                            [self._filtered_trace[ttl_ind]])
+                        trigger_data['trigger_type'].extend([5])
 
-        """
+                        
+                        # TTL                    
+                        trigger_data['trigger_index_ttl'].extend([ttl_ind_shift])
+                        trigger_data['trigger_time_ttl'].extend([ttl_ind_shift/self._fs])
+                        trigger_data['trigger_amplitude_ttl'].extend(
+                            [self._filtered_trace_ttl[ttl_ind]])
+                        
+                        # pulse
+                        if rangetypes[irange][1]:
+                            # pulse also triggered
+                            trigger_data['trigger_index_pulse'].extend([evt_ind_shift])
+                            trigger_data['trigger_time_pulse'].extend([evt_ind_shift/self._fs])
+                            trigger_data['trigger_amplitude_pulse'].extend(
+                                [self._filtered_trace[evt_ind]])
+                        else:
+                            # no trigger
+                            trigger_data['trigger_index_pulse'].extend([np.nan])
+                            trigger_data['trigger_time_pulse'].extend([np.nan])
+                            trigger_data['trigger_amplitude_pulse'].extend([np.nan])
+
+                    # case only pulse triggered
+                    else:
+                        # primary = pulse
+                        trigger_data['trigger_index'].extend([evt_ind_shift])
+                        trigger_data['trigger_time'].extend([evt_ind_shift/self._fs])
+                        trigger_data['trigger_amplitude'].extend(
+                            [self._filtered_trace[evt_ind]])
+                        trigger_data['trigger_type'].extend([4])
 
-        data_info = None
+                        
+                        # pulse also triggered
+                        trigger_data['trigger_index_pulse'].extend([evt_ind_shift])
+                        trigger_data['trigger_time_pulse'].extend([evt_ind_shift/self._fs])
+                        trigger_data['trigger_amplitude_pulse'].extend(
+                            [self._filtered_trace[evt_ind]])
+                        
+                        #ttl
+                        trigger_data['trigger_index_ttl'].extend([np.nan])
+                        trigger_data['trigger_time_ttl'].extend([np.nan])
+                        trigger_data['trigger_amplitude_ttl'].extend([np.nan])
+
+                # Case no TTL
+                else:
+                    trigger_data['trigger_index'].extend([evt_ind_shift])
+                    trigger_data['trigger_time'].extend([evt_ind_shift/self._fs])
+                    trigger_data['trigger_amplitude'].extend([self._filtered_trace[evt_ind]])
+                    trigger_data['trigger_type'].extend([4])
+                    
+                # extra parameter both TTL and pulse threshold
+                trigger_data['trigger_threshold_sigma'].extend([thresh])
+                trigger_data['trigger_pileup_window'].extend([pileup_window])
+
+
+        # duplicate key channel name
+        self._trigger_data = dict()
+        self._trigger_data[self._trigger_channel] = trigger_data.copy()
+        
+        for key, val in trigger_data.items():
+            newkey = key + '_' + self._trigger_channel
+            self._trigger_data[self._trigger_channel][newkey] = val
+
+        #  add channels
+        nb_events = len(trigger_data['trigger_index'])
+        chan_list = list()
+        if nb_events>0:
+            chan_list = [self._trigger_channel]*nb_events
+        self._trigger_data[self._trigger_channel]['trigger_channel'] = chan_list
+                        
+        
+        
+        
         
-        if not self._input_file_dict:
-            raise ValueError('No file available to get sample rate!')
-
-        for series, files in self._input_file_dict.items():
-            metadata = self._h5.get_metadata(file_name=files[0],
-                                             include_dataset_metadata=False)
-
-            adc_name = metadata['adc_list'][0]
-            data_info = metadata['groups'][adc_name]
-            data_info['comment'] = metadata['comment']
-            data_info['facility'] = metadata['facility']
-            data_info['run_purpose'] = metadata['run_purpose']
-            break
-
-        if data_info is None:
-            raise ValueError('ERROR: No ADC info in file. Something wrong...')
-
-        return data_info
```

### Comparing `detprocess-0.3.3/detprocess.egg-info/PKG-INFO` & `detprocess-0.3.4/detprocess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: detprocess
-Version: 0.3.3
+Version: 0.3.4
 Summary: Detector Data Processing Package
 Home-page: https://github.com/spice-herald/detprocess
-Author: Samuel Watkins
-Author-email: samwatkins@berkeley.edu
+Author: Bruno Serfass, Samuel Watkins
+Author-email: serfass@berkeley.edu, samwatkins@berkeley.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #  `detprocess`: Detector processing code for feature extraction
 
 [![PyPI](https://img.shields.io/pypi/v/detprocess)](https://pypi.org/project/detprocess/) [![Python 3.6](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
```

### Comparing `detprocess-0.3.3/setup.py` & `detprocess-0.3.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,33 +32,35 @@
                     # Die if path in CLEAN_FILES is absolute + outside this directory
                     raise ValueError("%s is not a path inside %s" % (path, here))
                 print('removing %s' % os.path.relpath(path))
                 shutil.rmtree(path)
 
 setup(
     name="detprocess",
-    version="0.3.3",
+    version="0.3.4",
     description="Detector Data Processing Package",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Samuel Watkins",
-    author_email="samwatkins@berkeley.edu",
+    author="Bruno Serfass, Samuel Watkins",
+    author_email="serfass@berkeley.edu, samwatkins@berkeley.edu",
     url="https://github.com/spice-herald/detprocess",
     license_files = ('LICENSE', ),
     packages=find_packages(), 
     zip_safe=False,
     cmdclass={
         'clean': CleanCommand,
     },
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
         'pyyaml',
-        'qetpy>=1.6.2',
+        'qetpy>=1.6.3',
         'pandas',
-        'pytesdaq>=0.2.8',
+        'pytesdaq>=0.3.3',
         'scikit-image',
         'iminuit>=2',
         'seaborn',
+        'humanfriendly',
+        'vaex',
     ],
 )
```

