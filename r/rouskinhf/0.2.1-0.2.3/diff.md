# Comparing `tmp/rouskinhf-0.2.1.tar.gz` & `tmp/rouskinhf-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rouskinhf-0.2.1.tar", last modified: Tue Jul 25 21:35:11 2023, max compression
+gzip compressed data, was "rouskinhf-0.2.3.tar", last modified: Wed Jul 26 22:48:05 2023, max compression
```

## Comparing `rouskinhf-0.2.1.tar` & `rouskinhf-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:35:11.681869 rouskinhf-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-25 21:35:11.681869 rouskinhf-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:35:11.681869 rouskinhf-0.2.1/rouskinhf/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/datafolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/import_dataset_fun.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/info_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/list_datapoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/rnastructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/rouskinhf/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:35:11.681869 rouskinhf-0.2.1/rouskinhf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-25 21:35:11.000000 rouskinhf-0.2.1/rouskinhf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-25 21:35:11.000000 rouskinhf-0.2.1/rouskinhf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:35:11.000000 rouskinhf-0.2.1/rouskinhf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-25 21:35:11.000000 rouskinhf-0.2.1/rouskinhf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 21:35:11.000000 rouskinhf-0.2.1/rouskinhf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:35:11.681869 rouskinhf-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-25 21:34:16.000000 rouskinhf-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:48:05.431418 rouskinhf-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-26 22:48:05.431418 rouskinhf-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:48:05.431418 rouskinhf-0.2.3/rouskinhf/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/rouskinhf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17251 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/rouskinhf/datafolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/rouskinhf/datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/rouskinhf/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/rouskinhf/import_dataset_fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/rouskinhf/info_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/rouskinhf/list_datapoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/rouskinhf/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/rouskinhf/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/rouskinhf/rnastructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/rouskinhf/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:48:05.431418 rouskinhf-0.2.3/rouskinhf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-26 22:48:05.000000 rouskinhf-0.2.3/rouskinhf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-26 22:48:05.000000 rouskinhf-0.2.3/rouskinhf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:48:05.000000 rouskinhf-0.2.3/rouskinhf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-26 22:48:05.000000 rouskinhf-0.2.3/rouskinhf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 22:48:05.000000 rouskinhf-0.2.3/rouskinhf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:48:05.431418 rouskinhf-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-26 22:47:09.000000 rouskinhf-0.2.3/setup.py
```

### Comparing `rouskinhf-0.2.1/LICENSE` & `rouskinhf-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.1/PKG-INFO` & `rouskinhf-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rouskinhf
-Version: 0.2.1
+Version: 0.2.3
 Summary: A library to manipulate data for our DMS prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -52,19 +52,19 @@
 ```bash
 nano env
 ```
 
 Copy paste the following content, and change the values to your own:
 
 ```bash
-HUGGINGFACE_TOKEN="your token here"  # you must change this to your HuggingFace token
-DATA_FOLDER="data/datafolders" # where the datafolder are stored by default, change it if you want to store it somewhere else
-DATA_FOLDER_TESTING="data/input_files_for_testing" # Don't touch this
-RNASTRUCTURE_PATH="/Users/ymdt/src/RNAstructure/exe" # Change this to the path of your RNAstructure executable
-RNASTRUCTURE_TEMP_FOLDER="temp" # You can change this to the path of your RNAstructure temp folder
+export HUGGINGFACE_TOKEN="your token here"  # you must change this to your HuggingFace token
+export DATA_FOLDER="data/datafolders" # where the datafolder are stored by default, change it if you want to store it somewhere else
+export DATA_FOLDER_TESTING="data/input_files_for_testing" # Don't touch this
+export RNASTRUCTURE_PATH="/Users/ymdt/src/RNAstructure/exe" # Change this to the path of your RNAstructure executable
+export RNASTRUCTURE_TEMP_FOLDER="temp" # You can change this to the path of your RNAstructure temp folder
 ```
 
 Then save the file and exit nano.
 
 ### Source the environment
 
 ```bash
```

### Comparing `rouskinhf-0.2.1/README.md` & `rouskinhf-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,19 @@
 ```bash
 nano env
 ```
 
 Copy paste the following content, and change the values to your own:
 
 ```bash
-HUGGINGFACE_TOKEN="your token here"  # you must change this to your HuggingFace token
-DATA_FOLDER="data/datafolders" # where the datafolder are stored by default, change it if you want to store it somewhere else
-DATA_FOLDER_TESTING="data/input_files_for_testing" # Don't touch this
-RNASTRUCTURE_PATH="/Users/ymdt/src/RNAstructure/exe" # Change this to the path of your RNAstructure executable
-RNASTRUCTURE_TEMP_FOLDER="temp" # You can change this to the path of your RNAstructure temp folder
+export HUGGINGFACE_TOKEN="your token here"  # you must change this to your HuggingFace token
+export DATA_FOLDER="data/datafolders" # where the datafolder are stored by default, change it if you want to store it somewhere else
+export DATA_FOLDER_TESTING="data/input_files_for_testing" # Don't touch this
+export RNASTRUCTURE_PATH="/Users/ymdt/src/RNAstructure/exe" # Change this to the path of your RNAstructure executable
+export RNASTRUCTURE_TEMP_FOLDER="temp" # You can change this to the path of your RNAstructure temp folder
 ```
 
 Then save the file and exit nano.
 
 ### Source the environment
 
 ```bash
```

### Comparing `rouskinhf-0.2.1/pyproject.toml` & `rouskinhf-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ['rouskinhf']
 
 [project]
 name =  "rouskinhf"
-version = "0.2.1"
+version = "0.2.3"
 authors = [
     {name = "Yves Martin", email = "yves@martin.yt"},
     {name = "Alberic de Lajarte", email = "albericlajarte@gmail.com"},
 ]
 description = "A library to manipulate data for our DMS prediction models."
 readme = "README.md"
 classifiers = [
```

### Comparing `rouskinhf-0.2.1/rouskinhf/datafolder.py` & `rouskinhf-0.2.3/rouskinhf/datafolder.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self.predict_dms = predict_dms
 
         # move path_in to source folder
         os.makedirs(self.get_source_folder(), exist_ok=True)
         os.system(f'cp -fr {path_in} {self.get_source_folder()}')
 
         # Write info file
-        infoFileWriter(source=source, datafolder=self, predict_dms=predict_dms, predict_structure=predict_dms).write()
+        self.infofile = infoFileWriter(source=source, datafolder=self, predict_dms=predict_dms, predict_structure=predict_dms)
 
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__} @{self.get_main_folder()}"
 
     def _set_name(self, name, path_in):
         if name is None:
@@ -94,18 +94,16 @@
 
         private : bool, optional
             If True, the repo is private. Default is True.
 
         Examples
         --------
 
-        >>> datafolder = DataFolder.from_dreem_output(path_in='data/input_files_for_testing/dreem_output.json')
-        Loaded 13 valid datapoints, filtered out 0 invalid datapoints.
+        >>> datafolder = DataFolder.from_dreem_output(path_in='data/input_files_for_testing/dreem_output.json', verbose=False)
         >>> datafolder.create_repo(exist_ok=True)
-
         """
 
         self.api.create_repo(
             repo_id=ROUSKINLAB+self.name,
             token=HUGGINGFACE_TOKEN,
             exist_ok=exist_ok,
             private=private,
@@ -133,33 +131,22 @@
 
         run_as_future : bool, optional
             If True, the upload is run asynchonously. The state of the upload can be checked with the returned future. See sample code. Default is False.
 
         Examples
         --------
 
-        >>> datafolder = DataFolder.from_dreem_output(path_in='data/input_files_for_testing/dreem_output.json')
-        Loaded 13 valid datapoints, filtered out 0 invalid datapoints.
+        >>> datafolder = DataFolder.from_dreem_output(path_in='data/input_files_for_testing/dreem_output.json', verbose=False)
         >>> datafolder.create_repo(exist_ok=True)
         >>> datafolder.upload_folder('main', 'pytest commit', 'A commit generated by pytest for the upload_folder method')
         >>> future = datafolder.upload_folder(run_as_future=True)
         >>> future.result() # wait for the upload to finish
         'https://huggingface.co/datasets/rouskinlab/dreem_output/tree/main/'
         >>> future.done() # check if the upload is done
         True
-        >>> datafolder = DataFolder.from_ct_folder(path_in='data/input_files_for_testing/ct_files')
-        Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
-        >>> datafolder.create_repo(exist_ok=True)
-        >>> datafolder.upload_folder('main', 'pytest commit', 'A commit generated by pytest for the upload_folder method')
-        >>> future = datafolder.upload_folder(run_as_future=True)
-        >>> datafolder = DataFolder.from_fasta(path_in='data/input_files_for_testing/sequences.fasta')
-        Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
-        >>> datafolder.create_repo(exist_ok=True)
-        >>> datafolder.upload_folder('main', 'pytest commit', 'A commit generated by pytest for the upload_folder method')
-
         """
 
         future = self.api.upload_folder(
             repo_id=ROUSKINLAB+self.name,
             folder_path=self.get_main_folder(),
             repo_type="dataset",
             token=HUGGINGFACE_TOKEN,
@@ -209,30 +196,34 @@
         If True, a progress bar is displayed. Default is True.
 
 
     Examples
     --------
 
     >>> datafolder = DataFolder.from_dreem_output(path_in='data/input_files_for_testing/dreem_output.json', generate_npy=True)
-    Loaded 13 valid datapoints, filtered out 0 invalid datapoints.
+    Over a total of 13 datapoints, there are:
+        - 12 valid datapoints
+        - 1 invalid datapoints (ex: sequence with non-regular characters)
+        - 0 datapoints with the same reference
+        - 0 duplicate sequences with the same structure / dms
+        - 0 duplicate sequences with different structure / dms
     >>> datafolder.name
     'dreem_output'
     >>> print(str(datafolder).split(' ')[0])
     CreateDatafolderFromDreemOutput
     >>> os.path.isfile(datafolder.get_json())
     True
     """
 
-    def __init__(self, path_in, path_out, name, predict_structure, generate_npy, tqdm=True) -> None:
+    def __init__(self, path_in, path_out, name, predict_structure, generate_npy, tqdm=True, verbose=True) -> None:
         super().__init__(path_in, path_out, name, source = 'dreem_output', predict_structure = predict_structure, predict_dms = False)
 
-        self.datapoints = ListofDatapoints.from_dreem_output(path_in, predict_structure = predict_structure, tqdm=tqdm)
-        self.datapoints.filter_duplicates()
+        self.datapoints = ListofDatapoints.from_dreem_output(path_in, predict_structure = predict_structure, tqdm=tqdm, verbose=verbose)
         self.dump_datapoints(generate_npy)
-
+        self.infofile.add_filtering_report(self.datapoints.filtering_report).write()
 
 class CreateDatafolderFromFasta(CreateDatafolderTemplate):
 
     """ Create a datafolder from a fasta file.
 
     Parameters
     ----------
@@ -253,29 +244,33 @@
         If True, the npy files are generated. Default is True.
 
 
     Examples
     --------
 
     >>> datafolder = DataFolder.from_fasta(path_in='data/input_files_for_testing/sequences.fasta', generate_npy=True)
-    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
+    Over a total of 5 datapoints, there are:
+        - 2 valid datapoints
+        - 1 invalid datapoints (ex: sequence with non-regular characters)
+        - 1 datapoints with the same reference
+        - 1 duplicate sequences
     >>> datafolder.name
     'sequences'
     >>> print(str(datafolder).split(' ')[0])
     CreateDatafolderFromFasta
     >>> os.path.isfile(datafolder.get_json())
     True
     """
 
-    def __init__(self, path_in, path_out, name, predict_structure, predict_dms, generate_npy, tqdm) -> None:
+    def __init__(self, path_in, path_out, name, predict_structure, predict_dms, generate_npy, tqdm, verbose=True) -> None:
         super().__init__(path_in, path_out, name, source = 'fasta', predict_structure = predict_structure, predict_dms = predict_dms)
 
-        self.datapoints = ListofDatapoints.from_fasta(path_in, predict_structure = predict_structure, predict_dms = predict_dms, tqdm=tqdm)
-        self.datapoints.filter_duplicates()
+        self.datapoints = ListofDatapoints.from_fasta(path_in, predict_structure = predict_structure, predict_dms = predict_dms, tqdm=tqdm, verbose=verbose)
         self.dump_datapoints(generate_npy)
+        self.infofile.add_filtering_report(self.datapoints.filtering_report).write()
 
 
 
 class CreateDatafolderFromCTfolder(CreateDatafolderTemplate):
 
     """ Create a datafolder from a folder of ct files.
 
@@ -293,35 +288,39 @@
 
     generate_npy : bool, optional
         If True, the npy files are generated. Default is True.
 
     tqdm : bool, optional
         If True, a progress bar is displayed. Default is True.
 
-
     Examples
     --------
 
     >>> datafolder = DataFolder.from_ct_folder(path_in='data/input_files_for_testing/ct_files', generate_npy=True)
-    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
+    Over a total of 5 datapoints, there are:
+        - 1 valid datapoints
+        - 1 invalid datapoints (ex: sequence with non-regular characters)
+        - 0 datapoints with the same reference
+        - 1 duplicate sequences with the same structure / dms
+        - 2 duplicate sequences with different structure / dms
     >>> datafolder.name
     'ct_files'
     >>> print(str(datafolder).split(' ')[0])
     CreateDatafolderFromCTfolder
     >>> os.path.isfile(datafolder.get_json())
     True
     """
 
-    def __init__(self, path_in, path_out, name, predict_dms, generate_npy, tqdm=True) -> None:
+    def __init__(self, path_in, path_out, name, predict_dms, generate_npy, tqdm=True, verbose=True) -> None:
         super().__init__(path_in, path_out, name, source = 'ct', predict_structure = False, predict_dms = predict_dms)
 
         ct_files = [os.path.join(path_in, f) for f in os.listdir(path_in) if f.endswith('.ct') or f.endswith('.txt')]
-        self.datapoints = ListofDatapoints.from_ct(ct_files, predict_dms = predict_dms, tqdm=tqdm)
-        self.datapoints.filter_duplicates()
+        self.datapoints = ListofDatapoints.from_ct(ct_files, predict_dms = predict_dms, tqdm=tqdm, verbose=verbose)
         self.dump_datapoints(generate_npy)
+        self.infofile.add_filtering_report(self.datapoints.filtering_report).write()
 
 
 class LoadDatafolder(DataFolderTemplate):
 
     def __init__(self, name, root) -> None:
         super().__init__(name, root)
 
@@ -342,20 +341,25 @@
         Revision of the datafolder. Default is 'main'.
 
 
     Examples
     --------
 
     >>> datafolder = LoadDatafolderFromHF(name='for_testing', path_out='data/datafolders')
-    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
+    Over a total of 2 datapoints, there are:
+        - 2 valid datapoints
+        - 0 invalid datapoints (ex: sequence with non-regular characters)
+        - 0 datapoints with the same reference
+        - 0 duplicate sequences with the same structure / dms
+        - 0 duplicate sequences with different structure / dms
     >>> datafolder.name
     'for_testing'
     """
 
-    def __init__(self, name, path_out, revision='main', tqdm=True) -> None:
+    def __init__(self, name, path_out, revision='main', tqdm=True, verbose=True) -> None:
         super().__init__(name, path_out)
 
         # Download the datafolder #TODO : check if the datafolder is already downloaded
         snapshot_download(
             repo_id = ROUSKINLAB+self.name,
             repo_type='dataset',
             local_dir=self.get_main_folder(),
@@ -363,15 +367,15 @@
             token=HUGGINGFACE_TOKEN,
             allow_patterns=['info.json', 'data.json']
             )
 
         assert os.path.isdir(self.get_main_folder()), f'No folder found in {self.get_main_folder()}'
         assert os.path.isfile(self.get_json()), f'No json file found in {self.get_main_folder()}'
 
-        self.datapoints = ListofDatapoints.from_json(self.get_json(), tqdm=tqdm)
+        self.datapoints = ListofDatapoints.from_json(self.get_json(), tqdm=tqdm, verbose=verbose)
 
 
 class LoadDatafolderFromLocal(LoadDatafolder):
     """Load a datafolder from local.
 
     Parameters
     ----------
@@ -382,26 +386,31 @@
     path : str
         Path to the folder where the datafolder is saved. Defaut is set in the env variable DATAFOLDER_PATH.
 
     Examples
     --------
 
     >>> datafolder = LoadDatafolderFromLocal(name='for_testing', path='data/datafolders')
-    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
+    Over a total of 2 datapoints, there are:
+        - 2 valid datapoints
+        - 0 invalid datapoints (ex: sequence with non-regular characters)
+        - 0 datapoints with the same reference
+        - 0 duplicate sequences with the same structure / dms
+        - 0 duplicate sequences with different structure / dms
     >>> datafolder.name
     'for_testing'
     """
 
-    def __init__(self, name, path) -> None:
+    def __init__(self, name, path, tqdm=True, verbose=True) -> None:
         super().__init__(name, path)
 
         assert os.path.isdir(self.get_main_folder()), f'No folder found in {self.get_main_folder()}'
         assert os.path.isfile(self.get_json()), f'No json file found in {self.get_main_folder()}'
 
-        self.datapoints = ListofDatapoints.from_json(self.get_json())
+        self.datapoints = ListofDatapoints.from_json(self.get_json(), tqdm=tqdm, verbose=verbose)
 
 class DataFolder:
     """Create a datafolder from a fasta file, a json file or a folder of ct files.
 
     Parameters
     ----------
 
@@ -419,41 +428,31 @@
 
     predict_dms : bool, optional
         If True, the dms is predicted. Default is True.
 
     tqdm : bool, optional
         If True, a progress bar is displayed. Default is True.
 
-    Example
-    -------
+    verbose : bool, optional
+        If True, the filtering report is displayed. Default is True.
 
-    >>> datafolder = DataFolder.from_dreem_output('data/input_files_for_testing/dreem_output.json')
-    Loaded 13 valid datapoints, filtered out 0 invalid datapoints.
-    >>> datafolder = DataFolder.from_fasta('data/input_files_for_testing/sequences.fasta')
-    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
-    >>> datafolder = DataFolder.from_ct_folder('data/input_files_for_testing/ct_files')
-    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
-    >>> datafolder = DataFolder.from_huggingface('for_testing')
-    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
-    >>> datafolder = DataFolder.from_local('for_testing')
-    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
     """
 
-    def from_fasta(path_in, path_out=DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY, tqdm=True)->CreateDatafolderFromFasta:
+    def from_fasta(path_in, path_out=DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY, tqdm=True, verbose=True)->CreateDatafolderFromFasta:
         """Create a datafolder from a fasta file. See CreateDatafolderFromFasta for more details."""
-        return CreateDatafolderFromFasta(path_in, path_out, name, predict_structure, predict_dms, generate_npy, tqdm=tqdm)
+        return CreateDatafolderFromFasta(path_in, path_out, name, predict_structure, predict_dms, generate_npy, tqdm=tqdm, verbose=verbose)
 
-    def from_dreem_output(path_in, path_out=DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, generate_npy = GENERATE_NPY, tqdm=True)->CreateDatafolderFromDreemOutput:
+    def from_dreem_output(path_in, path_out=DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, generate_npy = GENERATE_NPY, tqdm=True, verbose=True)->CreateDatafolderFromDreemOutput:
         """Create a datafolder from a dreem output file. See CreateDatafolderFromDreemOutput for more details."""
-        return CreateDatafolderFromDreemOutput(path_in, path_out, name, predict_structure, generate_npy, tqdm=tqdm)
+        return CreateDatafolderFromDreemOutput(path_in, path_out, name, predict_structure, generate_npy, tqdm=tqdm, verbose= verbose)
 
-    def from_local(name, path=DATA_FOLDER)->LoadDatafolderFromLocal:
+    def from_local(name, path=DATA_FOLDER, tqdm=True, verbose=True)->LoadDatafolderFromLocal:
         """Load a datafolder from local. See LoadDatafolderFromLocal for more details."""
-        return LoadDatafolderFromLocal(name, path)
+        return LoadDatafolderFromLocal(name, path, tqdm=tqdm, verbose=verbose)
 
-    def from_ct_folder(path_in, path_out=DATA_FOLDER, name = None, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY, tqdm=True)->CreateDatafolderFromCTfolder:
+    def from_ct_folder(path_in, path_out=DATA_FOLDER, name = None, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY, tqdm=True, verbose=True)->CreateDatafolderFromCTfolder:
         """Create a datafolder from a folder of ct files. See CreateDatafolderFromCTfolder for more details."""
-        return CreateDatafolderFromCTfolder(path_in, path_out, name, predict_dms, generate_npy, tqdm=tqdm)
+        return CreateDatafolderFromCTfolder(path_in, path_out, name, predict_dms, generate_npy, tqdm=tqdm, verbose= verbose)
 
-    def from_huggingface(name, path_out=DATA_FOLDER, tqdm=True)->LoadDatafolderFromHF:
+    def from_huggingface(name, path_out=DATA_FOLDER, tqdm=True, verbose=True)->LoadDatafolderFromHF:
         """Load a datafolder from HuggingFace. See LoadDatafolderFromHF for more details."""
-        return LoadDatafolderFromHF(name, path_out, tqdm=tqdm)
+        return LoadDatafolderFromHF(name, path_out, tqdm=tqdm, verbose=verbose)
```

### Comparing `rouskinhf-0.2.1/rouskinhf/datapoint.py` & `rouskinhf-0.2.3/rouskinhf/datapoint.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,35 +12,40 @@
     - sequence is a string of A, C, G, U
     - structure is a string of (, ), .
     - dms is a list of floats corresponding to the reactivity of each base in the sequence
     - paired_bases is a list of tuples (i,j) where i and j are paired bases.
 
 
     Example:
-    >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0])
-    >>> print(datapoint)
-    "reference":{"sequence": "AACCGG", "paired_bases": [[1, 4], [0, 5]], "dms": [1.0, 2.0, 3.0]}
-    >>> datapoint = Datapoint(reference='reference', sequence='not a valid sequence', structure='((..))')
-    >>> print(datapoint)
+    >>> print(Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0]))
+    "reference":{"sequence": "AACCGG", "paired_bases": [[0, 5], [1, 4]], "dms": [1.0, 2.0, 3.0]}
+    >>> print(Datapoint(reference='reference', sequence='not a valid sequence', structure='((..))'))
     None
-    >>> datapoint = Datapoint(reference='reference', sequence='NNNNNNN', structure='((..))')
-    >>> print(datapoint)
+    >>> print(Datapoint(reference='reference', sequence='NNNNNNN', structure='((..))'))
+    None
+    >>> print(Datapoint(reference='reference', sequence='AACCGG', paired_bases=[(0, 5), (1, 4)]))
+    "reference":{"sequence": "AACCGG", "paired_bases": [[0, 5], [1, 4]]}
+    >>> print(Datapoint(reference='reference', sequence='AACCGG', paired_bases=[(1, 5), (1, 4)]))
     None
     """
 
     def __new__(cls, *args, **kwargs):
         # Check if the conditions are met before creating the object
         sequence = kwargs.get('sequence', args[0] if len(args) > 0 else None)
         reference = kwargs.get('reference', args[1] if len(args) > 1 else None)
         if sequence is None or reference is None:
             return None
         sequence = standardize_sequence(sequence)
 
         if not sequence_has_regular_characters(sequence) or len(sequence) == 0 or len(reference) == 0:
             return None
+        
+        if 'paired_bases' in kwargs:
+            if not cls._assert_paired_bases(None, kwargs['paired_bases'], sequence):
+                return None
 
         # If conditions are met, create and return the new instance
         instance = super().__new__(cls)
         return instance
 
     def __init__(self, sequence, reference, structure=None, dms=None, paired_bases=None):
         for attr in [sequence, reference]:
@@ -49,43 +54,83 @@
 
         # standardize the sequence
         sequence = standardize_sequence(sequence)
 
         if not sequence_has_regular_characters(sequence):
             raise Exception(f"Sequence {sequence} contains characters other than ACGTUacgtu.")
 
-
         self.reference = reference
         self.sequence = sequence
         self.structure = structure
-        self.paired_bases = paired_bases if paired_bases is not None else self.structure_to_paired_bases(structure) if structure is not None else None
-        self.dms = dms
+        self.paired_bases = self._format_paired_bases(paired_bases) if paired_bases is not None else self._format_paired_bases(self.structure_to_paired_bases(structure)) if structure is not None else None
+        self.dms = self._format_dms(dms) if dms is not None else None
         self.opt_dict = {'paired_bases': self.paired_bases, 'dms': self.dms}
 
+    def _format_paired_bases(self, paired_bases):
+        """Returns a set of tuples.
+        >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0])
+        >>> datapoint._format_paired_bases([[1, 4], [0, 5]])
+        ((0, 5), (1, 4))
+        """
+        return tuple(sorted([tuple(sorted(pair)) for pair in paired_bases])) if paired_bases is not None else None
+    
+    def _assert_paired_bases(self, paired_bases, sequence):
+        """Ensures that the base pairs are 0=<bp<len(sequence) and that that there's maximum one pair per base. 
+        >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0])
+        >>> datapoint._assert_paired_bases([(0, 5), (1, 4)], 'AACCGG')
+        True
+        >>> datapoint._assert_paired_bases([(0, 5), (1, 4), (1, 2)], 'AACCGG')
+        False
+        >>> datapoint._assert_paired_bases([(0, 5), (4, 1), (1, 2)], 'AACCGG')
+        False
+        >>> datapoint._assert_paired_bases([(0, 8), (3, 4), (1, 2)], 'AACCGG')
+        False
+        >>> datapoint._assert_paired_bases(None, 'AACCGG')
+        True
+        """
+        if paired_bases is not None:
+            return all([0 <= pair[0] < len(sequence) and 0 <= pair[1] < len(sequence) and pair[0] != pair[1] for pair in paired_bases]) \
+                and len(set([pair[0] for pair in paired_bases] + [pair[1] for pair in paired_bases])) == len(paired_bases) * 2
+        else:
+            return True
+
+    def _format_dms(self, dms):
+        """returns a tuple
+        >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0])
+        >>> datapoint._format_dms([1.0, 2.0, 3.0])
+        (1.0, 2.0, 3.0)
+        """
+        return tuple(dms) if dms is not None else None
+        
+
     def to_dict(self):
         return self.reference, {'sequence': self.sequence, **{k:v for k,v in self.opt_dict.items() if v is not None}}
 
     def to_flat_dict(self):
         return {'reference': self.reference, 'sequence': self.sequence, **{k:v for k,v in self.opt_dict.items() if v is not None}}
 
+    @classmethod
+    def from_flat_dict(cls, d):
+        return cls(sequence=d['sequence'], reference=d['reference'], **{k:v for k,v in d.items() if k not in ['sequence', 'reference']})
+
     def __str__(self):
         return '"'+self.reference+'"' + ':' + str({"sequence": self.sequence, **{k:v for k,v in self.opt_dict.items() if v is not None}}).replace("'",'"').replace('(','[').replace(')',']').replace('None','null')
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}('{self.reference}', sequence='{self.sequence}', paired_bases={self.paired_bases}, dms={self.dms})"
 
     def structure_to_paired_bases(self, structure):
         """Returns a list of tuples (i,j) where i and j are paired bases."""
-        paired_bases = []
+        paired_bases = set()
         stack = []
         for i, char in enumerate(structure):
             if char == '(':
                 stack.append(i)
             elif char == ')':
-                paired_bases.append((stack.pop(), i))
+                paired_bases.add((stack.pop(), i))
         return paired_bases
 
     def embed_sequence(self):
         """Returns a list of integers corresponding to the sequence.
 
         >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure='((..))', dms=[1.0, 2.0, 3.0])
         >>> datapoint.embed_sequence()
@@ -139,26 +184,25 @@
 
         if sequence_has_regular_characters(sequence):
             return Datapoint(
                 sequence=sequence,
                 reference=reference,
                 structure=RNAstructure_singleton.predictStructure(sequence, dms=mutation_rate) if predict_structure else None,
                 dms=mutation_rate)
-        print('DatapointFactory.from_dreem_output: sequence is not valid "{}"'.format(set(sequence) - set('ACGTUacgtu')))
 
 
     def from_json_line(string):
         """Create a datapoint from a json line. The json line should have the following format:
         "reference": {"sequence": "sequence", "paired_bases": [[1, 2], [3,4]], "dms": [1.0, 2.0, 3.0]}
 
         Example:
         >>> DatapointFactory.from_json_line('"reference": {"sequence": "ACAAGU"}')
         Datapoint('reference', sequence='ACAAGU', paired_bases=None, dms=None)
         >>> DatapointFactory.from_json_line('"reference": {"sequence": "ACAAGU", "paired_bases": [[1, 2], [3, 4]], "dms": [1.0, 2.0, 3.0]}')
-        Datapoint('reference', sequence='ACAAGU', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])
+        Datapoint('reference', sequence='ACAAGU', paired_bases=((1, 2), (3, 4)), dms=(1.0, 2.0, 3.0))
         >>> DatapointFactory.from_json_line('"reference": {"sequence": "something else than ACGTUacgtu", "paired_bases": [[1, 2], [3, 4]], "dms": [1.0, 2.0, 3.0]}')
         """
 
         # process the string into a dictionary
         string= string.strip()[:-1] if string.strip()[-1] == ',' else string.strip()
         string = add_braces_if_no_braces(string)
         d = json.loads(string)
```

### Comparing `rouskinhf-0.2.1/rouskinhf/env.py` & `rouskinhf-0.2.3/rouskinhf/env.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.1/rouskinhf/import_dataset_fun.py` & `rouskinhf-0.2.3/rouskinhf/import_dataset_fun.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,35 +16,30 @@
         Name of the type of data to find the dataset for (structure or DMS).
     force_download : bool
         Whether to force download the dataset from HuggingFace Hub. Defaults to False.
 
     Returns
     -------
 
-    ndarray
-        The dataset with the given name for the given type of data.
+    dict: {str: ndarray}
+        Dictionary with the following keys: 'references', 'sequences', and 'structure' or 'DMS' depending on the data type.
 
     Example
     -------
 
-    >>> import_dataset(name='for_testing', data='structure').keys()
-    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
-    dict_keys(['references', 'sequences', 'structure'])
-    >>> import_dataset(name='for_testing', data='DMS').keys()
-    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
-    dict_keys(['references', 'sequences', 'DMS'])
     >>> import_dataset(name='for_testing', data='structure', force_download=True).keys()
-    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
+    Over a total of 2 datapoints, there are:
+        - 2 valid datapoints
+        - 0 invalid datapoints (ex: sequence with non-regular characters)
+        - 0 datapoints with the same reference
+        - 0 duplicate sequences with the same structure / dms
+        - 0 duplicate sequences with different structure / dms
     dict_keys(['references', 'sequences', 'structure'])
-    >>> import_dataset(name='for_testing', data='DMS', force_download=True).keys()
-    Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
-    dict_keys(['references', 'sequences', 'DMS'])
-
     """
-
+    if data == 'dms': data = 'DMS'
     assert data in ['structure', 'DMS'], "data must be either 'structure' or 'DMS'"
 
     # Get the data folder
     try:
         assert not force_download, "Force download from HuggingFace Hub"
         datafolder = DataFolder.from_local(name=name)
     except:
```

### Comparing `rouskinhf-0.2.1/rouskinhf/info_file.py` & `rouskinhf-0.2.3/rouskinhf/info_file.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,14 +45,19 @@
                     f.write(f"\t{k}: {v}\n")
             f.write(f"\tData types:")
             if self.has_structure:
                 f.write(f"\n\t- structure ({self.info['about structure']})")
             if self.has_dms:
                 f.write(f"\n\t- DMS ({self.info['about DMS']})")
 
+        return self
+    
+    def add_filtering_report(self, filtering_report):
+        self.info['filtering_report'] = filtering_report
+        return self
 
 
 class InfoFileWriterFromDREEMoutput(InfoFileWriterTemplate):
 
     def __init__(self, name, root, path_in, predict_dms, predict_structure) -> None:
         super().__init__(name, root, has_dms=True, has_structure=predict_structure)
 
@@ -60,42 +65,46 @@
         if 'user' in file:
             file['experimenter'] = file.pop('user')
         for k, v in file.items():
             if type(v) != dict:
                 self.info[k] = v
 
         self.info['source'] = "`{}` (DREEM output format)".format(os.path.basename(path_in))
-        self.info['structure'] = STRUCTURE_FROM_RNASTRUCTURE
-        self.info['about structure'] = 'Predicted using RNAstructure and the DMS reactivity data.'
+        if predict_structure:
+            self.info['structure'] = STRUCTURE_FROM_RNASTRUCTURE
+            self.info['about structure'] = 'Predicted using RNAstructure and the DMS reactivity data.'
         self.info['DMS'] = DMS_FROM_SOURCE
         self.info['about DMS'] = 'Measured experimentally using the attached experimental conditions.'
 
 
 class InfoFileWriterFromCT(InfoFileWriterTemplate):
 
     def __init__(self, name, root, path_in, predict_dms, predict_structure) -> None:
         super().__init__(name, root, has_dms=predict_dms, has_structure=True)
 
         self.info['source'] = "`{}` (CT files format)".format(os.path.basename(path_in))
         self.info['structure'] = STRUCTURE_FROM_SOURCE
         self.info['about structure'] = 'Read from source.'
-        self.info['DMS'] = DMS_FROM_RNASTRUCTURE
-        self.info['about DMS'] = 'Predicted using RNAstructure at 310K.'
+        if predict_dms:
+            self.info['DMS'] = DMS_FROM_RNASTRUCTURE
+            self.info['about DMS'] = 'Predicted using RNAstructure at 310K.'
 
 
 class InfoFileWriterFromFasta(InfoFileWriterTemplate):
 
     def __init__(self, name, root, path_in, predict_dms, predict_structure) -> None:
         super().__init__(name, root, has_dms=predict_dms, has_structure=predict_structure)
 
         self.info['source'] = "`{}` (fasta file format)".format(os.path.basename(path_in))
-        self.info['structure'] = STRUCTURE_FROM_RNASTRUCTURE
-        self.info['about structure'] = 'Predicted using RNAstructure at 310K.'
-        self.info['DMS'] = DMS_FROM_RNASTRUCTURE
-        self.info['about DMS'] = 'Predicted using RNAstructure at 310K.'
+        if predict_structure:
+            self.info['structure'] = STRUCTURE_FROM_RNASTRUCTURE
+            self.info['about structure'] = 'Predicted using RNAstructure at 310K.'
+        if predict_dms:
+            self.info['DMS'] = DMS_FROM_RNASTRUCTURE
+            self.info['about DMS'] = 'Predicted using RNAstructure at 310K.'
 
 
 def infoFileWriter(source, datafolder, predict_dms, predict_structure):
 
     if source == 'dreem_output':
         return InfoFileWriterFromDREEMoutput(datafolder.name, datafolder.path_out, datafolder.path_in, predict_dms=predict_dms, predict_structure=predict_structure)
     if source == 'ct':
```

### Comparing `rouskinhf-0.2.1/rouskinhf/list_datapoints.py` & `rouskinhf-0.2.3/rouskinhf/list_datapoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,60 +7,57 @@
 from typing import List, Tuple, Union, Optional
 from .parsers import Fasta, DreemOutput
 import pandas as pd
 from tqdm import tqdm as tqdm_parser
 
 class ListofDatapoints:
 
-    def __init__(self, datapoints, verbose=True):
-        self.datapoints = list(filter(lambda x: x is not None, datapoints))
-        if verbose:
-            print(f"Loaded {len(self.datapoints)} valid datapoints, filtered out {len(datapoints)-len(self.datapoints)} invalid datapoints.")
-
+    def __init__(self, datapoints=[], verbose=True):
+        self.datapoints, self.filtering_report = self.filter_duplicates_and_unvalid(datapoints, verbose)
+        
     def __call__(self) -> List[Datapoint]:
         return self.datapoints
 
     @classmethod
-    def from_fasta(cls, fasta_file, predict_structure, predict_dms, tqdm=True):
+    def from_fasta(cls, fasta_file, predict_structure, predict_dms, tqdm=True, verbose=True):
         """Create a list of datapoint from a fasta file. The structure and dms will be predicted if predict_structure and predict_dms are True."""
         sequences, references = Fasta.parse(fasta_file)
         return cls([DatapointFactory.from_fasta(sequence, reference, predict_structure, predict_dms)
-                    for sequence, reference in tqdm_parser(zip(sequences, references), total=len(sequences), desc='Parsing fasta file', disable=not tqdm)])
+                    for sequence, reference in tqdm_parser(zip(sequences, references), total=len(sequences), desc='Parsing fasta file', disable=not tqdm)], verbose=verbose)
 
     @classmethod
-    def from_ct(cls, ct_files, predict_dms, tqdm=True):
+    def from_ct(cls, ct_files, predict_dms, tqdm=True, verbose=True):
         """Create a list of datapoint from a ct file. The dms will be predicted if predict_dms is True."""
-        return cls([DatapointFactory.from_ct(ct_file, predict_dms) for ct_file in tqdm_parser(ct_files, total=len(ct_files), desc='Parsing ct files', disable=not tqdm)])
+        return cls([DatapointFactory.from_ct(ct_file, predict_dms) for ct_file in tqdm_parser(ct_files, total=len(ct_files), desc='Parsing ct files', disable=not tqdm)], verbose=verbose)
 
     @classmethod
-    def from_dreem_output(cls, dreem_output_file, predict_structure, tqdm):
+    def from_dreem_output(cls, dreem_output_file, predict_structure, tqdm=True, verbose=True):
         """Create a list of datapoint from a dreem output file. The structure and dms will be predicted if predict_structure and predict_dms are True."""
         n_lines = len(list(DreemOutput.parse(dreem_output_file)))
         return cls([DatapointFactory.from_dreem_output(reference, sequence, mutation_rate, predict_structure)
-            for reference, sequence, mutation_rate in tqdm_parser(DreemOutput.parse(dreem_output_file), total=n_lines, desc='Parsing dreem output file', disable=not tqdm)])
+            for reference, sequence, mutation_rate in tqdm_parser(DreemOutput.parse(dreem_output_file), total=n_lines, desc='Parsing dreem output file', disable=not tqdm)], verbose=verbose)
 
     @classmethod
-    def from_json(cls, json_file, tqdm=True):
+    def from_json(cls, json_file, tqdm=True, verbose=True):
         """Create a list of datapoint from a json file."""
         with open(json_file) as f:
-            return cls([DatapointFactory.from_json_line(line) for line in tqdm_parser(f, total=sum(1 for line in open(json_file) if line.strip() not in ['{', '}']), desc='Parsing json file', disable= not tqdm) if line.strip() not in ['{', '}']])
+            return cls([DatapointFactory.from_json_line(line) for line in tqdm_parser(f, total=sum(1 for line in open(json_file) if line.strip() not in ['{', '}']), desc='Parsing json file', disable= not tqdm) if line.strip() not in ['{', '}']], verbose=verbose)
 
 
     def to_base_pairs_npy(self, path):
         """Writes the structure npy file from the list of datapoints.
 
         Args:
             path (str): path to the npy file
 
         Returns:
             np.array: structure matrix of pairs of 0-based indices.
 
         Examples:
-            >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])])
-            Loaded 1 valid datapoints, filtered out 0 invalid datapoints.
+            >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])], verbose=False)
             >>> datapoints.to_base_pairs_npy('temp/base_pairs.npy')
             array([[[1, 2],
                     [3, 4]]], dtype=object)
         """
 
         arr = np.array([np.array(datapoint.paired_bases) for datapoint in self.datapoints], dtype=object)
         np.save(path, arr)
@@ -73,16 +70,15 @@
         Args:
             path (str): path to the npy file
 
         Returns:
             np.array: dms matrix of floats arrays.
 
         Examples:
-            >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])])
-            Loaded 1 valid datapoints, filtered out 0 invalid datapoints.
+            >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])], verbose=False)
             >>> datapoints.to_dms_npy('temp/dms.npy')
             array([[1.0, 2.0, 3.0]], dtype=object)
         """
 
         arr = np.array([datapoint.dms for datapoint in self.datapoints], dtype=object)
         np.save(path, arr)
         return arr
@@ -96,16 +92,15 @@
 
         Returns:
             np.array: int-encoded sequence matrix
 
         Examples:
             >>> from numpy import array
             >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0]),\
-                                               Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])])
-            Loaded 2 valid datapoints, filtered out 0 invalid datapoints.
+                                               Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])], verbose=False)
             >>> assert not (datapoints.to_sequence_npy('temp/sequence.npy') - array([[0, 0, 1 ,1, 2, 2],[0, 0, 1, 1, 2 ,2]], dtype=object)).any(), "The sequence matrix is not correct."
         """
 
         arr = np.array([datapoint.embed_sequence() for datapoint in self.datapoints], dtype=object)
         np.save(path, arr)
         return arr
 
@@ -116,16 +111,15 @@
         Args:
             path (str): path to the npy file
 
         Returns:
             np.array: reference matrix of int-encoded.
 
         Examples:
-            >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])])
-            Loaded 1 valid datapoints, filtered out 0 invalid datapoints.
+            >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])], verbose=False)
             >>> datapoints.to_reference_npy('temp/reference.npy')
             array(['reference'], dtype='<U9')
         """
 
         arr = np.array([datapoint.reference for datapoint in self.datapoints])
         np.save(path, arr)
         return arr
@@ -136,75 +130,108 @@
         os.makedirs(os.path.dirname(path), exist_ok=True)
         with open(path, 'w') as f:
             f.write('{\n')
             for idx, datapoint in enumerate(self.datapoints): # write the datapoints one by one to avoid memory issues
                 f.write(str(datapoint)+ ',\n' if idx != len(self.datapoints)-1 else str(datapoint)+'\n')
             f.write('}\n')
 
-    def to_pandas(self) -> pd.DataFrame:
+    def to_pandas(self, datapoints=None) -> pd.DataFrame:
         """Converts the list of datapoints into a pandas dataframe.
 
         Example:
-            >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])])
-            Loaded 1 valid datapoints, filtered out 0 invalid datapoints.
-            >>> datapoints.to_pandas()
-               reference sequence      paired_bases              dms
-            0  reference   AACCGG  [[1, 2], [3, 4]]  [1.0, 2.0, 3.0]
+        >>> datapoints = ListofDatapoints([Datapoint(reference='reference', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[1.0, 2.0, 3.0])], verbose=False)
+        >>> datapoints.to_pandas()
+           reference sequence      paired_bases              dms
+        0  reference   AACCGG  ((1, 2), (3, 4))  (1.0, 2.0, 3.0)
+        """
+        if datapoints is None: datapoints = self.datapoints
+        return pd.DataFrame([datapoint.to_flat_dict() for datapoint in datapoints])
+    
+    def from_pandas(self, df: pd.DataFrame) -> None:
+        """Converts a pandas dataframe into a list of datapoints.
+
+        Example:
+            >>> df = pd.DataFrame([{'reference': 'reference', 'sequence': 'AACCGG', 'paired_bases': [[1, 2], [3, 4]], 'dms': [1.0, 2.0, 3.0]}])
+            >>> ListofDatapoints(verbose=False).from_pandas(df)
+            [Datapoint('reference', sequence='AACCGG', paired_bases=((1, 2), (3, 4)), dms=(1.0, 2.0, 3.0))]
         """
-        return pd.DataFrame([datapoint.to_flat_dict() for datapoint in self.datapoints])
+        return [Datapoint.from_flat_dict(datapoint_dict) for datapoint_dict in df.to_dict('records')]
 
-    def filter_duplicates(self):
+    def filter_duplicates_and_unvalid(self, datapoints, verbose=True):
         """Filters out duplicate sequences.
         Only keep the first occurence of a sequence if all the other structures are the same.
 
         Examples:
             >>> datapoints = ListofDatapoints([ Datapoint(reference='ref1', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[0,0,0,0,0,0]),\
                                 Datapoint(reference='ref2', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[0,0,0,0,0,0]),\
-                                Datapoint(reference='ref3', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[0,0,0,0,0,0]),\
-                                Datapoint(reference='ref4', sequence='AUGGC', paired_bases=[[1, 2]], dms=[0,0,0,0,0]),\
-                                Datapoint(reference='ref5', sequence='GCCUA', paired_bases=[[0, 4], [2, 3]], dms=[0,0,0,0,0]),\
+                                Datapoint(reference='ref2', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[0,0,0,0,0,0]),\
+                                Datapoint(reference='ref4', sequence='AUGGC', paired_bases=[[1, 2]], dms=[0,0,0,0,1]),\
+                                Datapoint(reference='ref5', sequence='AUGGC', paired_bases=[[0, 4], [2, 3]], dms=[0,0,0,0,0]),\
                                 Datapoint(reference='ref6', sequence='not a regular sequence', paired_bases=[[0, 4]], dms=[0,0,0,0,0]) ])
-            Loaded 5 valid datapoints, filtered out 1 invalid datapoints.
-            >>> datapoints.filter_duplicates()
+            Over a total of 6 datapoints, there are:
+                - 1 valid datapoints
+                - 1 invalid datapoints (ex: sequence with non-regular characters)
+                - 1 datapoints with the same reference
+                - 1 duplicate sequences with the same structure / dms
+                - 2 duplicate sequences with different structure / dms
             >>> datapoints.datapoints
-            [Datapoint('ref1', sequence='AACCGG', paired_bases=[[1, 2], [3, 4]], dms=[0, 0, 0, 0, 0, 0]), Datapoint('ref4', sequence='AUGGC', paired_bases=[[1, 2]], dms=[0, 0, 0, 0, 0]), Datapoint('ref5', sequence='GCCUA', paired_bases=[[0, 4], [2, 3]], dms=[0, 0, 0, 0, 0])]
+            [Datapoint('ref1', sequence='AACCGG', paired_bases=((1, 2), (3, 4)), dms=(0, 0, 0, 0, 0, 0))]
         """
-
-        # Group datapoints by sequence
-        unique_seqs = {}
-        for i, datapoint in enumerate(self.datapoints):
-
-            struct = np.array(datapoint.paired_bases)
-
-            if datapoint.sequence not in unique_seqs.keys():
-                unique_seqs[datapoint.sequence] = ([struct], [i])
-            else:
-                unique_seqs[datapoint.sequence][0].append(struct)
-                unique_seqs[datapoint.sequence][1].append(i)
-
-        # Only keep sequence duplicate that have the same pairing matrix
-        idxs_to_remove = []
-        for seq in unique_seqs.keys():
-            if len(unique_seqs[seq]) > 1:
-                matches = []
-                for i in range(len(unique_seqs[seq][0])):
-                    for j in range(i+1, len(unique_seqs[seq][0])):
-                        matches.append(np.array_equal(unique_seqs[seq][0][i], unique_seqs[seq][0][j]))
-
-                # Remove sequences from dataframe if f1 score is not 1.0, keep only one of the structures otherwise
-                if not np.array(matches).all():
-                    idxs_to_remove += unique_seqs[seq][1]
-                else:
-                    idxs_to_remove += unique_seqs[seq][1][1:]
-
-        idxs_to_keep = list( set(range(len(self.datapoints)))-set(idxs_to_remove) )
-        self.datapoints = [self.datapoints[i] for i in idxs_to_keep]
-
-
-
+        
+        # Remove None datapoints        
+        n_input_datapoints = len(datapoints)
+        datapoints = list(filter(lambda x: x is not None, datapoints))
+        n_unvalid_datapoints = n_input_datapoints - len(datapoints)
+
+        # Convert to pandas
+        df = self.to_pandas(datapoints)
+        
+        # Remove duplicate or conflicting datapoints and keep track of the number of datapoints removed
+        def drop_duplicates(df:pd.DataFrame, **kwargs):
+            len_df_before = len(df)
+            df.drop_duplicates(**kwargs)
+            return len_df_before - len(df)
+
+        
+        # Don't allow multiple sequences with the same reference
+        n_same_ref_datapoints = drop_duplicates(df, subset=['reference'], inplace=True)
+
+        # Keep only one datapoint per sequence and structure
+        if 'paired_bases' in df.columns:
+            n_duplicates_datapoints = drop_duplicates(df, subset=['sequence','paired_bases'], inplace=True, ignore_index=True)
+
+        # Keep only one datapoint per sequence and dms
+        if 'dms' in df.columns:
+            if not 'paired_bases' in df.columns: n_duplicates_datapoints = 0
+            n_duplicates_datapoints += drop_duplicates(df, subset=['sequence','dms'], inplace=True, ignore_index=True)
+        
+        # If there are multiple structures / dms with the same structure, keep none
+        n_same_seq_datapoints = drop_duplicates(df, subset=['sequence'], inplace=True, ignore_index=True, keep='first' if not ('paired_bases' in df.columns or 'dms' in df.columns) else False)
+
+        # Convert back to list of datapoints
+        datapoints = self.from_pandas(df)
+
+        # Write report
+        report = f"""Over a total of {n_input_datapoints} datapoints, there are:
+    - {len(datapoints)} valid datapoints
+    - {n_unvalid_datapoints} invalid datapoints (ex: sequence with non-regular characters)
+    - {n_same_ref_datapoints} datapoints with the same reference"""
+        if 'paired_bases' in df.columns or 'dms' in df.columns:
+            report += f"""
+    - {n_duplicates_datapoints} duplicate sequences with the same structure / dms
+    - {n_same_seq_datapoints} duplicate sequences with different structure / dms"""
+        else:
+            report += f"""
+    - {n_same_seq_datapoints} duplicate sequences"""
+    
+        if verbose: print(report)
+            
+        return datapoints, report
+    
+            
 def base_pairs_into_matrix(base_pairs):
     """Turns a list of base pairs into a matrix of 1s and 0s.
 
     Args:
         base_pairs (list): list of base pairs, where each base pair is a tuple of 0-based two ints.
 
     Returns:
```

### Comparing `rouskinhf-0.2.1/rouskinhf/parsers.py` & `rouskinhf-0.2.3/rouskinhf/parsers.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.1/rouskinhf/path.py` & `rouskinhf-0.2.3/rouskinhf/path.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.1/rouskinhf/rnastructure.py` & `rouskinhf-0.2.3/rouskinhf/rnastructure.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.1/rouskinhf/util.py` & `rouskinhf-0.2.3/rouskinhf/util.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.1/rouskinhf.egg-info/PKG-INFO` & `rouskinhf-0.2.3/rouskinhf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rouskinhf
-Version: 0.2.1
+Version: 0.2.3
 Summary: A library to manipulate data for our DMS prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -52,19 +52,19 @@
 ```bash
 nano env
 ```
 
 Copy paste the following content, and change the values to your own:
 
 ```bash
-HUGGINGFACE_TOKEN="your token here"  # you must change this to your HuggingFace token
-DATA_FOLDER="data/datafolders" # where the datafolder are stored by default, change it if you want to store it somewhere else
-DATA_FOLDER_TESTING="data/input_files_for_testing" # Don't touch this
-RNASTRUCTURE_PATH="/Users/ymdt/src/RNAstructure/exe" # Change this to the path of your RNAstructure executable
-RNASTRUCTURE_TEMP_FOLDER="temp" # You can change this to the path of your RNAstructure temp folder
+export HUGGINGFACE_TOKEN="your token here"  # you must change this to your HuggingFace token
+export DATA_FOLDER="data/datafolders" # where the datafolder are stored by default, change it if you want to store it somewhere else
+export DATA_FOLDER_TESTING="data/input_files_for_testing" # Don't touch this
+export RNASTRUCTURE_PATH="/Users/ymdt/src/RNAstructure/exe" # Change this to the path of your RNAstructure executable
+export RNASTRUCTURE_TEMP_FOLDER="temp" # You can change this to the path of your RNAstructure temp folder
 ```
 
 Then save the file and exit nano.
 
 ### Source the environment
 
 ```bash
```

