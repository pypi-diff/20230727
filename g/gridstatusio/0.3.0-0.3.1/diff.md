# Comparing `tmp/gridstatusio-0.3.0.tar.gz` & `tmp/gridstatusio-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-_7vu499n/gridstatusio-0.3.0.tar", last modified: Fri Jul 21 19:54:13 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-miq3ax9h/gridstatusio-0.3.1.tar", last modified: Thu Jul 27 18:03:18 2023, max compression
```

## Comparing `gridstatusio-0.3.0.tar` & `gridstatusio-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1461 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3293 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      883 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio/
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/gridstatusio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9887 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/gridstatusio/gs_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/gridstatusio/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5334 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/gridstatusio/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/gridstatusio/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3293 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/gridstatusio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2319 2023-07-21 19:53:58.000000 gridstatusio-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 19:54:13.000000 gridstatusio-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      883 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/gridstatusio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10649 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/gridstatusio/gs_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/gridstatusio/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/gridstatusio/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/gridstatusio/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/gridstatusio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2319 2023-07-27 18:02:59.000000 gridstatusio-0.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 18:03:18.000000 gridstatusio-0.3.1/setup.cfg
```

### Comparing `gridstatusio-0.3.0/LICENSE` & `gridstatusio-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.3.0/PKG-INFO` & `gridstatusio-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `gridstatusio-0.3.0/README.md` & `gridstatusio-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gridstatusio-0.3.0/gridstatusio/gs_client.py` & `gridstatusio-0.3.1/gridstatusio/gs_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 import io
 import time
 
 import gridstatus
 import pandas as pd
 import requests
 from tabulate import tabulate
-from termcolor import colored, cprint
+from termcolor import colored
 
 from gridstatusio import __version__
 
 
+def log(msg, verbose, level="info", end="\n"):
+    """Print a message if verbose matches the level"""
+    if verbose is True:
+        verbose = "info"
+
+    # if verbose is debug, print everything
+    if verbose == "debug":
+        print(msg, end=end)
+    elif verbose == "info" and level == "info":
+        print(msg, end=end)
+
+
 class GridStatusClient:
     def __init__(self, api_key=None, host="https://api.gridstatus.io/v1"):
         """Create a GridStatus.io API client
 
         Parameters:
             api_key (str): The API key to use for authentication.
             If not provided, the GRIDSTATUS_API_KEY environment variable will be used.
@@ -44,17 +56,16 @@
         headers = {
             "x-api-key": self.api_key,
             # set client and version
             "x-client": "gridstatusio-python",
             "x-client-version": __version__,
         }
 
-        if verbose:
-            print(f"GET {url}")
-            print(f"Params: {params}")
+        log(f"\nGET {url}", verbose=verbose, level="debug")
+        log(f"Params: {params}", verbose=verbose, level="debug")
         response = requests.get(url, params=params, headers=headers)
 
         if response.status_code != 200:
             raise Exception(f"Error {response.status_code}: {response.text}")
 
         return response
 
@@ -125,16 +136,19 @@
                         )
 
                     more_info_url = (
                         f"https://www.gridstatus.io/datasets/{dataset['id']}"
                     )
                     dataset_table.append(["More Info", more_info_url])
 
-                    print(tabulate(dataset_table, headers=headers, tablefmt="pretty"))
-                    print("\n")
+                    log(
+                        tabulate(dataset_table, headers=headers, tablefmt="pretty"),
+                        True,
+                    )
+                    log("\n", True)
 
         if return_list:
             return matched_datasets
 
     def get_dataset(
         self,
         dataset,
@@ -143,15 +157,15 @@
         columns=None,
         filter_column=None,
         filter_value=None,
         filter_operator="=",
         limit=10000,
         max_rows=None,
         tz=None,
-        verbose=False,
+        verbose=True,
     ):
         """Get a dataset from GridStatus.io API
 
         Parameters:
             dataset (str): The name of the dataset to fetch
             start (str): The start time of the data to fetch. If not provided,
                 defaults to the earliest available time for the dataset.
@@ -166,16 +180,17 @@
                 Defaults to "=". Possible values are "=",
                 "!=", ">", "<", ">=", "<=", "in".
             limit (int): The maximum number of rows to fetch at time.
                 Defaults to 10000.
             max_rows (int): The maximum number of rows to fetch.
                 Defaults to None, which fetches all rows that match the request.
             tz (str): The timezone to convert utc timestamps to. Defaults to UTC.
-            verbose (bool): If set to True, prints out the number
-                of rows fetched and the time taken to fetch them.
+            verbose (bool): If set to True or "info", prints additional information.
+                If set to "debug", prints more additional debug information. If
+                set to False, no additional information is printed. Defaults to True.
 
         Returns:
             pd.DataFrame: The dataset as a pandas dataframe
         """
         if tz is None:
             tz = "UTC"
 
@@ -209,45 +224,56 @@
                 params["filter_column"] = filter_column
                 params["filter_value"] = filter_value
                 params["filter_operator"] = filter_operator
 
             if columns is not None:
                 params["columns"] = ",".join(columns)
 
+            # Log the fetching message
+            log(f"Fetching Page {page}...", verbose, end="")
+
             response = self.get(url, params=params, verbose=verbose)
 
             df = pd.read_csv(io.StringIO(response.text))
             dfs.append(df)
 
             has_next_page = response.headers["x-has-next-page"] == "true"
             response_time = time.time() - start_time
             total_time += response_time
             avg_time_per_page = total_time / page
 
-            print(
-                f"\rFetching page {page}: Time for last page: \
-                    {round(response_time, 2)} seconds | "
-                f"Average time per page: {round(avg_time_per_page, 2)} seconds",
-                end="",
-            )
+            # Update the fetching message with the done message
+            if page == 1:
+                log(
+                    f"Done in {round(response_time, 2)} seconds. ",
+                    verbose,
+                )
+
+            else:
+                log(
+                    f"Done in {round(response_time, 2)} seconds. "
+                    f"Total time: {round(total_time, 2)}s. "
+                    f"Avg per page: {round(avg_time_per_page, 2)}s",
+                    verbose,
+                )
+
             page += 1
+
             # time.sleep(
             #     0.1
             # )  # Add a small delay to ensure the output is updated correctly
 
-        print()  # Add a newline for cleaner output
+        log("", verbose=verbose)  # Add a newline for cleaner output
 
         df = pd.concat(dfs).reset_index(drop=True)
 
         # Print the additional information
-        cprint(f"\nTotal number of rows: {len(df)}", "cyan")
-        cprint(f"Total Time: {round(total_time, 2)} seconds", "cyan")
-        cprint(
-            f"Average time per page: {round(total_time / (page - 1), 2)} seconds",
-            "cyan",
+        log(
+            f"Total number of rows: {len(df)}",
+            verbose=verbose,
         )
 
         # convert to datetime for any columns that end in _utc
         # or are of type object
         for col in df.columns:
             if df[col].dtype == "object" or col.endswith("_utc"):
                 try:
```

### Comparing `gridstatusio-0.3.0/gridstatusio/tests/test_api.py` & `gridstatusio-0.3.1/gridstatusio/tests/test_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -196,7 +196,65 @@
         filter_operator="=",
         max_rows=max_rows,
         verbose=True,
     )
 
     _check_dataframe(df)
     assert df["curtailment_mw"].unique() == [numeric_value]
+
+
+def test_get_dataset_verbose(capsys):
+    # make sure nothing print to stdout
+    client.get_dataset(
+        dataset="isone_fuel_mix",
+        start="2023-01-01",
+        end="2023-01-05",
+        max_rows=1,
+        verbose=False,
+    )
+
+    captured = capsys.readouterr()
+    assert captured.out == ""
+
+    # test debug
+    client.get_dataset(
+        dataset="isone_fuel_mix",
+        start="2023-01-01",
+        end="2023-01-05",
+        max_rows=1,
+        verbose="debug",
+    )
+
+    captured = capsys.readouterr()
+    assert captured.out != ""
+    # make sure the params are printed
+    assert "Done in" in captured.out
+    assert "Params: {" in captured.out
+
+    # make sure something prints to stdout
+    # but not the params
+    client.get_dataset(
+        dataset="isone_fuel_mix",
+        start="2023-01-01",
+        end="2023-01-05",
+        max_rows=1,
+        verbose=True,
+    )
+
+    captured = capsys.readouterr()
+    assert captured.out != ""
+    assert "Done in" in captured.out
+    assert "Params: {" not in captured.out
+
+    # same as verbose=True
+    client.get_dataset(
+        dataset="isone_fuel_mix",
+        start="2023-01-01",
+        end="2023-01-05",
+        max_rows=1,
+        verbose="info",
+    )
+
+    captured = capsys.readouterr()
+    assert captured.out != ""
+    assert "Done in" in captured.out
+    assert "Params: {" not in captured.out
```

### Comparing `gridstatusio-0.3.0/gridstatusio.egg-info/PKG-INFO` & `gridstatusio-0.3.1/gridstatusio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridstatusio
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python Client for GridStatus.io API
 Author-email: Max Kanter <kmax12@gmail.com>
 Maintainer-email: Max Kanter <kmax12@gmail.com>
 License: Copyright 2022 James Max Kanter
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
```

### Comparing `gridstatusio-0.3.0/pyproject.toml` & `gridstatusio-0.3.1/pyproject.toml`

 * *Files identical despite different names*

