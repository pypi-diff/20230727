# Comparing `tmp/ecallisto_ng-0.2.6.tar.gz` & `tmp/ecallisto_ng-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.2.6.tar", last modified: Wed Jul 26 02:20:40 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.2.7.tar", last modified: Thu Jul 27 15:52:46 2023, max compression
```

## Comparing `ecallisto_ng-0.2.6.tar` & `ecallisto_ng-0.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.6/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3564 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2945 2023-07-19 13:07:49.000000 ecallisto_ng-0.2.6/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      905 2023-07-26 02:20:13.000000 ecallisto_ng-0.2.6/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     9301 2023-07-26 02:08:55.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4680 2023-07-26 02:15:22.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5694 2023-07-26 02:08:55.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3025 2023-07-26 02:08:55.000000 ecallisto_ng-0.2.6/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-26 02:20:40.890290 ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3564 2023-07-26 02:20:40.000000 ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-26 02:20:40.000000 ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-26 02:20:40.000000 ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      137 2023-07-26 02:20:40.000000 ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-26 02:20:40.000000 ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-27 15:52:46.113454 ecallisto_ng-0.2.7/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.7/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4171 2023-07-27 15:52:46.113454 ecallisto_ng-0.2.7/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3552 2023-07-26 02:25:53.000000 ecallisto_ng-0.2.7/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      905 2023-07-27 15:52:05.000000 ecallisto_ng-0.2.7/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-27 15:52:46.113454 ecallisto_ng-0.2.7/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-27 15:52:46.093454 ecallisto_ng-0.2.7/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-27 15:52:46.103454 ecallisto_ng-0.2.7/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.7/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-27 15:52:46.103454 ecallisto_ng-0.2.7/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.7/src/ecallisto_ng/data_fetching/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     9922 2023-07-27 15:50:53.000000 ecallisto_ng-0.2.7/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4680 2023-07-26 02:15:22.000000 ecallisto_ng-0.2.7/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-27 15:52:46.103454 ecallisto_ng-0.2.7/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.7/src/ecallisto_ng/data_processing/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5694 2023-07-26 02:08:55.000000 ecallisto_ng-0.2.7/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-27 15:52:46.113454 ecallisto_ng-0.2.7/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.7/src/ecallisto_ng/plotting/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3025 2023-07-26 02:08:55.000000 ecallisto_ng-0.2.7/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-27 15:52:46.103454 ecallisto_ng-0.2.7/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     4171 2023-07-27 15:52:46.000000 ecallisto_ng-0.2.7/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-27 15:52:46.000000 ecallisto_ng-0.2.7/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-27 15:52:46.000000 ecallisto_ng-0.2.7/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      137 2023-07-27 15:52:46.000000 ecallisto_ng-0.2.7/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-27 15:52:46.000000 ecallisto_ng-0.2.7/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.2.6/LICENSE` & `ecallisto_ng-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.6/PKG-INFO` & `ecallisto_ng-0.2.7/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
-Name: ecallisto_ng
-Version: 0.2.6
+Name: ecallisto-ng
+Version: 0.2.7
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: nb
 Provides-Extra: dev
 License-File: LICENSE
 
 # Ecallisto NG 
-Ecallisto NG is a compact yet effective Python package designed to facilitate seamless interaction with the Ecallisto API. 
-The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto API via the link: [https://v000792.fhnw.ch/api/redoc](https://v000792.fhnw.ch/api/redoc).
+Ecallisto NG is a compact yet effective Python package designed to facilitate seamless interaction with the Ecallisto API (Rest API built with FastAPI). It provides a simple interface to fetch data from the API, as well as some basic data processing and plotting capabilities. Behind the Rest API, there is a TimeScaleDB database, which is a time-series database. Thus, data access by time, with aggregation functions, is fast and possible.
+
+## Background
+The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto Rest API via the link: [https://v000792.fhnw.ch/api/redoc](https://v000792.fhnw.ch/api/redoc).
+Currently, not all data is added to the database. Feel free to reach out if you need data before 2020. 
 
 ## Installation
 To install this package, clone this repository and use pip for installation. Execute the following command in your terminal:
 ```pip install -e .```
 
 ## PyPI
 Ecallisto NG is conveniently available on PyPI as well. To download, visit the following link: [https://pypi.org/project/ecallisto-ng/](https://pypi.org/project/ecallisto-ng/)
 
 ## Example
 Please have a look at the jupyter notebook under `example`. 
 
 ## Usage
-Here's a guide on how to use the different features of Ecallisto NG:
+Here's a guide on how to use the different features of Ecallisto NG. Be aware that data is cached automatically in your working directory under `ecallisto_ng_cache`. Feel free to delete this folder if you want to fetch the data again.
 
 ### Data Fetching
 Fetching data is easy using the `get_data` function, housed under the `ecallisto_ng.data_fetching.get_data` module. Here's an example:
 
 ```python
 from ecallisto_ng.data_fetching.get_data import get_data
```

### Comparing `ecallisto_ng-0.2.6/README.md` & `ecallisto_ng-0.2.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # Ecallisto NG 
-Ecallisto NG is a compact yet effective Python package designed to facilitate seamless interaction with the Ecallisto API. 
-The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto API via the link: [https://v000792.fhnw.ch/api/redoc](https://v000792.fhnw.ch/api/redoc).
+Ecallisto NG is a compact yet effective Python package designed to facilitate seamless interaction with the Ecallisto API (Rest API built with FastAPI). It provides a simple interface to fetch data from the API, as well as some basic data processing and plotting capabilities. Behind the Rest API, there is a TimeScaleDB database, which is a time-series database. Thus, data access by time, with aggregation functions, is fast and possible.
+
+## Background
+The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto Rest API via the link: [https://v000792.fhnw.ch/api/redoc](https://v000792.fhnw.ch/api/redoc).
+Currently, not all data is added to the database. Feel free to reach out if you need data before 2020. 
 
 ## Installation
 To install this package, clone this repository and use pip for installation. Execute the following command in your terminal:
 ```pip install -e .```
 
 ## PyPI
 Ecallisto NG is conveniently available on PyPI as well. To download, visit the following link: [https://pypi.org/project/ecallisto-ng/](https://pypi.org/project/ecallisto-ng/)
 
 ## Example
 Please have a look at the jupyter notebook under `example`. 
 
 ## Usage
-Here's a guide on how to use the different features of Ecallisto NG:
+Here's a guide on how to use the different features of Ecallisto NG. Be aware that data is cached automatically in your working directory under `ecallisto_ng_cache`. Feel free to delete this folder if you want to fetch the data again.
 
 ### Data Fetching
 Fetching data is easy using the `get_data` function, housed under the `ecallisto_ng.data_fetching.get_data` module. Here's an example:
 
 ```python
 from ecallisto_ng.data_fetching.get_data import get_data
```

### Comparing `ecallisto_ng-0.2.6/pyproject.toml` & `ecallisto_ng-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.2.6"
+version = "0.2.7"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.2.6/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.2.7/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+import json
 import os
 import time
 
 import pandas as pd
 import requests
 
 BASE_URL = "https://v000792.fhnw.ch"
-
+DATA_FOLDER = "ecallisto_ng_cache"
 
 def get_data(
     instrument_name,
     start_datetime,
     end_datetime,
     timebucket=None,
     agg_function=None,
-    data_folder="ecallisto_ng_cache",
+    data_folder=DATA_FOLDER,
     verbose=False,
     max_retries=3,
 ):
     """
     Get data from the eCallisto API. See: https://v000792.fhnw.ch/api/redoc
     Of course, this is just a wrapper around the requests.post function.
     Depending on the size, the request can take a while. For example, two
@@ -67,46 +68,50 @@
     file_path = os.path.join(
         data_folder,
         f"{instrument_name}_{start_datetime}_{end_datetime}_{timebucket}_{agg_function}.parquet",
     )
     os.makedirs(data_folder, exist_ok=True)
     if os.path.exists(file_path):
         print(f"Reading data from {file_path}")
-        return pd.read_parquet(file_path)
+        return read_parquet_and_meta_data(file_path)
 
     # Send the request to the API
     response = requests.post(BASE_URL + "/api/data", json=data, timeout=180)
     # Check if the request was successful
     if response.status_code == 200:
         if verbose:
             print(
                 "Data retrieval started successfully. Waiting for file to be ready..."
             )
         # Get the URL for the parquet file
         parquet_url = response.json()["data_parquet_url"]
         json_url = response.json()["info_json_url"]
         file_id = response.json()["file_id"]
+        meta_data_url = response.json()["meta_data_url"]
 
         # Now we can start polling the URL until the parquet file is ready for download
-        n_tries = 0
+        n_tries = 1
         while True:
             try:
                 if verbose:
                     print(f"Trying to download file {file_id}")
                 # Try to download the parquet file
                 file_response = requests.get(BASE_URL + parquet_url)
                 # If the file is available, save it to disk
                 if file_response.status_code == 200:
                     print("File downloaded successfully")
                     with open(file_path, "wb") as f:
                         f.write(file_response.content)
+                    # Download the meta data
+                    meta_data_response = requests.get(BASE_URL + meta_data_url)
+                    with open(file_path.replace(".parquet", ".json"), "w") as f:
+                        f.write(meta_data_response.text)
                     # Check that the file is bigger than 8 bytes (sometimes, the API returns an empty file)
                     if os.path.getsize(file_path) > 8:
-                        # Return the file as a DataFrame
-                        return pd.read_parquet(file_path)
+                        return read_parquet_and_meta_data(file_path)
                     else:
                         # Remove file and try again
                         os.remove(file_path)
                         raise ValueError(
                             f"Error downloading file: {file_response.status_code}. File is empty."
                         )
                 elif file_response.status_code == 204:
@@ -150,14 +155,23 @@
                         f"Error downloading file: {file_response.status_code}. Max retries reached."
                     )
                 time.sleep(3)
     else:
         print(f"Error starting data retrieval: {response.status_code}")
 
 
+def read_parquet_and_meta_data(file_path):
+    meta_data_path = file_path.replace(".parquet", ".json")
+    df = pd.read_parquet(file_path)
+    with open(meta_data_path, "r") as f:
+        meta_data = json.load(f)
+    for key, value in meta_data.items():
+        df.attrs[key] = value
+    return df
+
 # Because of SQL limitation, the names of the tables do not perfectly match the instrument names.
 # This function converts the instrument name to the table name.
 def extract_instrument_name(file_path):
     """
     Because of SQL limitation, the names of the tables do not perfectly match the instrument names.
     This function converts the instrument name to the table name.
```

### Comparing `ecallisto_ng-0.2.6/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.2.7/src/ecallisto_ng/data_fetching/get_information.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.6/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.2.7/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.6/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.2.7/src/ecallisto_ng/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.2.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
-Name: ecallisto-ng
-Version: 0.2.6
+Name: ecallisto_ng
+Version: 0.2.7
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: nb
 Provides-Extra: dev
 License-File: LICENSE
 
 # Ecallisto NG 
-Ecallisto NG is a compact yet effective Python package designed to facilitate seamless interaction with the Ecallisto API. 
-The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto API via the link: [https://v000792.fhnw.ch/api/redoc](https://v000792.fhnw.ch/api/redoc).
+Ecallisto NG is a compact yet effective Python package designed to facilitate seamless interaction with the Ecallisto API (Rest API built with FastAPI). It provides a simple interface to fetch data from the API, as well as some basic data processing and plotting capabilities. Behind the Rest API, there is a TimeScaleDB database, which is a time-series database. Thus, data access by time, with aggregation functions, is fast and possible.
+
+## Background
+The package is constructed in Python 3.9 and utilizes the `requests` library to directly access the Ecallisto Rest API via the link: [https://v000792.fhnw.ch/api/redoc](https://v000792.fhnw.ch/api/redoc).
+Currently, not all data is added to the database. Feel free to reach out if you need data before 2020. 
 
 ## Installation
 To install this package, clone this repository and use pip for installation. Execute the following command in your terminal:
 ```pip install -e .```
 
 ## PyPI
 Ecallisto NG is conveniently available on PyPI as well. To download, visit the following link: [https://pypi.org/project/ecallisto-ng/](https://pypi.org/project/ecallisto-ng/)
 
 ## Example
 Please have a look at the jupyter notebook under `example`. 
 
 ## Usage
-Here's a guide on how to use the different features of Ecallisto NG:
+Here's a guide on how to use the different features of Ecallisto NG. Be aware that data is cached automatically in your working directory under `ecallisto_ng_cache`. Feel free to delete this folder if you want to fetch the data again.
 
 ### Data Fetching
 Fetching data is easy using the `get_data` function, housed under the `ecallisto_ng.data_fetching.get_data` module. Here's an example:
 
 ```python
 from ecallisto_ng.data_fetching.get_data import get_data
```

### Comparing `ecallisto_ng-0.2.6/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.2.7/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

