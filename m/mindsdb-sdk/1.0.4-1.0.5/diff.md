# Comparing `tmp/mindsdb_sdk-1.0.4.tar.gz` & `tmp/mindsdb_sdk-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mindsdb_sdk-1.0.4.tar", last modified: Thu Jun  8 11:15:48 2023, max compression
+gzip compressed data, was "dist/mindsdb_sdk-1.0.5.tar", last modified: Thu Jul 27 14:30:08 2023, max compression
```

## Comparing `mindsdb_sdk-1.0.4.tar` & `mindsdb_sdk-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:15:48.000000 mindsdb_sdk-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-06-08 11:15:48.000000 mindsdb_sdk-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:15:48.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/connect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:15:48.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/connectors/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/mindsdb_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:15:48.000000 mindsdb_sdk-1.0.4/mindsdb_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-06-08 11:15:47.000000 mindsdb_sdk-1.0.4/mindsdb_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-08 11:15:48.000000 mindsdb_sdk-1.0.4/mindsdb_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:15:47.000000 mindsdb_sdk-1.0.4/mindsdb_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-08 11:15:47.000000 mindsdb_sdk-1.0.4/mindsdb_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 11:15:47.000000 mindsdb_sdk-1.0.4/mindsdb_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:15:48.000000 mindsdb_sdk-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-08 11:15:27.000000 mindsdb_sdk-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:08.000000 mindsdb_sdk-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-27 14:30:08.000000 mindsdb_sdk-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:08.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      407 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/connect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:08.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/connectors/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/mindsdb_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:08.000000 mindsdb_sdk-1.0.5/mindsdb_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-27 14:30:08.000000 mindsdb_sdk-1.0.5/mindsdb_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-27 14:30:08.000000 mindsdb_sdk-1.0.5/mindsdb_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:30:08.000000 mindsdb_sdk-1.0.5/mindsdb_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-27 14:30:08.000000 mindsdb_sdk-1.0.5/mindsdb_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 14:30:08.000000 mindsdb_sdk-1.0.5/mindsdb_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:30:08.000000 mindsdb_sdk-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-27 14:29:58.000000 mindsdb_sdk-1.0.5/setup.py
```

### Comparing `mindsdb_sdk-1.0.4/PKG-INFO` & `mindsdb_sdk-1.0.5/mindsdb_sdk.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,177 +1,146 @@
 Metadata-Version: 2.1
-Name: mindsdb_sdk
-Version: 1.0.4
+Name: mindsdb-sdk
+Version: 1.0.5
 Summary: MindsDB Python SDK, provides an SDK to use a remote mindsdb instance
 Home-page: https://github.com/mindsdb/mindsdb_python_sdk
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb-sdk/
 Description: # Python MindsDB SDK
-        It enables you to connect to a MindsDB server from python using HTTP API.
         
-        ## Install
+        The Python MindsDB SDK allows you to connect to a MindsDB server from Python using the HTTP API.
+        
+        ## Installation
+        
         ```
         pip install mindsdb_sdk
         ```
         
         ## Example
         
-        Connect:
-        ```python
-        import mindsdb_sdk
+        ### Connecting to the MindsDB server
+        
+        You can establish a connection to the MindsDB server using the SDK. Here are some examples:
         
-        # Connect to local server 
+        #### Connect to a local MindsDB server
         
+        ```python
+        import mindsdb_sdk
         server = mindsdb_sdk.connect()
         server = mindsdb_sdk.connect('http://127.0.0.1:47334')
+        ```
         
-        # Connect to cloud server
+        #### Connect to the MindsDB Cloud
         
+        ```python
+        import mindsdb_sdk
         server = mindsdb_sdk.connect(email='a@b.com', password='-')
         server = mindsdb_sdk.connect('https://cloud.mindsdb.com', login='a@b.com', password='-')
+        ```
         
-        # Connect to MindsDB Pro
+        ####  Connect to a MindsDB Pro server
         
+        ```python
+        import mindsdb_sdk
         server = mindsdb_sdk.connect('http://<YOUR_INSTANCE_IP>', login='a@b.com', password='-', is_managed=True)
-        
         ```
         
-        Base usage:
-        ```python
+        ## Basic usage
         
-        # database
+        Once connected to the server, you can perform various operations. Here are some examples:
+        
+        ```python
+        # Get a list of databases
         databases = server.list_databases()
         
-        database = databases[0] # Database type object
+        # Get a specific database
+        database = databases[0]  # Database type object
         
-        # sql query
+        # Perform an SQL query
         query = database.query('select * from table1')
         print(query.fetch())
         
-        # create table
+        # Create a table
         table = database.create_table('table2', query)
         
-        
-        # project
+        # Get a project
         project = server.get_project('proj')
         
-        # sql query
+        # Perform an SQL query within a project
         query = project.query('select * from database.table join model1')
         
-        # create view
-        view = project.create_view(
-              'btc_view',
-               query=query
-        )
+        # Create a view
+        view = project.create_view('view1', query=query)
         
-        # get view
+        # Get a list of views
         views = project.list_views()
         view = views[0]
         df = view.fetch()
         
-        # get model
+        # Get a list of models
         models = project.list_models()
         model = models[0]
         
-        # using model
+        # Use a model for prediction
         result_df = model.predict(df)
         result_df = model.predict(query)
         
-        # create model
+        # Create a model
+        timeseries_options = {
+            'order': 'date',
+            'window': 5,
+            'horizon': 1
+        }
         model = project.create_model(
-              'rentals_model',
-              predict='price',
-              query=query,
+            'rentals_model',
+            predict='price',
+            query=query,
+            timeseries_options=timeseries_options
         )
         
         ```
         
-        More examples in [Google colab notebook](
+        You can find more examples in this [Google colab notebook](
         https://colab.research.google.com/drive/1QouwAR3saFb9ffthrIs1LSH5COzyQa11#scrollTo=k6IbwsKRPQCR
         )
         
-        ## API documentation
-        
-        Api documentation can be found in: 
-        https://mindsdb.github.io/mindsdb_python_sdk/
-        
+        ## API Documentation
         
-        **Generating api docs:**
+        The API documentation for the MindsDB SDK can be found at https://mindsdb.github.io/mindsdb_python_sdk/. You can generate the API documentation locally by following these steps:
         
-        Locally:
+        ### Generating API docs locally:
         
         ```commandline
         cd docs
-        
         pip install -r requirements.txt
-        
         make html
         ```
         
+        The online documentation is automatically updated by pushing changes to the docs branch.
         
-        **Online documentation** is updated by pushing in `docs` branch
         
+        ## Testing
         
-        
-        ## How to test
-        `
-        It runs all tests for components 
+        To run all the tests for the components, use the following command:
         
         ```bash
         env PYTHONPATH=./ pytest
         ```
         
-        ## How to Connect From a Python File
-        
-        Create a file in your python project's root directory to store the connection details:
-        
-        `server.py` 
-        
-        Add the connection arguments with **your MindsDB credentials** to `server.py`:
-        
-        ```python
-        import mindsdb_sdk
-        
-        server = mindsdb_sdk.connect()
-        server = mindsdb_sdk.connect('http://127.0.0.1:47334')
-        
-        server = mindsdb_sdk.connect(email='your_mindsdb_email', password='your_mindsdb_password')
-        server = mindsdb_sdk.connect('https://cloud.mindsdb.com', email='your_mindsdb_email', password='your_mindsdb_password')
-        ```
+        ## Contributing
         
-        Open your terminal and type:
+        We welcome contributions to the MindsDB SDK. If you'd like to contribute, please refer to the contribution guidelines for more information.
         
-        `python server.py` 
+        ## License
         
-        ### Testing the Connection
+        The MindsDB SDK is licensed under the MIT License. Feel free to use and modify it according to your needs
         
-        Add test queries to `server.py` with `print()` statements to confirm the connection:
-        
-        ```python
-        import mindsdb_sdk #import the mindsdb_sdk package
-        
-        server = mindsdb_sdk.connect()
-        server = mindsdb_sdk.connect('http://127.0.0.1:47334')
-        
-        #  Input your MindsDB Cloud Credentials below to connect to MindsDB Cloud
-        server = mindsdb_sdk.connect(email='your_mindsdb_email', password='your_mindsdb_password')
-        server = mindsdb_sdk.connect('https://cloud.mindsdb.com', email='your_mindsdb_email', password='your_mindsdb_password') # Connect to MindsDB server in the cloud
-        
-        databases = server.list_databases()
-        
-        database = databases[1] # Database type object
-        
-        query = database.query('select * from files.test_data')
-        print(database)
-        ```
         
-        To see a full example, checkout:
-        `server.py`
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mindsdb_sdk-1.0.4/mindsdb_sdk/connect.py` & `mindsdb_sdk-1.0.5/mindsdb_sdk/connect.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-1.0.4/mindsdb_sdk/connectors/rest_api.py` & `mindsdb_sdk-1.0.5/mindsdb_sdk/connectors/rest_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from functools import wraps
+import io
 
 import requests
 import pandas as pd
 
+from .. import __about__
 
 def _try_relogin(fnc):
     @wraps(fnc)
     def wrapper(self, *args, **kwargs):
         try:
             return fnc(self, *args, **kwargs)
         except requests.HTTPError as e:
@@ -34,14 +36,16 @@
 
         self.url = url
         self.username = login
         self.password = password
         self.is_managed = is_managed
         self.session = requests.Session()
 
+        self.session.headers['User-Agent'] = f'python-sdk/{__about__.__version__}'
+
         if login is not None:
             self.login()
 
     def login(self):
         managed_endpoint = '/api/login'
         cloud_endpoint = '/cloud/login'
 
@@ -110,7 +114,29 @@
 
     @_try_relogin
     def objects_tree(self, item=''):
         r = self.session.get(self.url + f'/api/tree/{item}')
         _raise_for_status(r)
 
         return pd.DataFrame(r.json())
+
+    @_try_relogin
+    def upload_file(self, name: str, df: pd.DataFrame):
+
+        # convert to file
+        fd = io.BytesIO()
+        df.to_csv(fd)
+        fd.seek(0)
+
+        url = self.url + f'/api/files/{name}'
+        r = self.session.put(
+            url,
+            data={
+                'source': name,
+                'name': name,
+                'source_type': 'file',
+            },
+            files={
+                'file': fd,
+            }
+        )
+        _raise_for_status(r)
```

### Comparing `mindsdb_sdk-1.0.4/mindsdb_sdk/database.py` & `mindsdb_sdk-1.0.5/mindsdb_sdk/database.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from typing import List
+from typing import List, Union
 
-from mindsdb_sql.parser.ast import Identifier
+import pandas as pd
+
+from mindsdb_sql.parser.ast import Identifier, DropTables
 
 from mindsdb_sdk.query import Query, Table
 
 
 class Database:
     """
     Allows to work with database (datasource): to use tables and make raw queries
@@ -38,14 +40,23 @@
 
     >>> table = database.create_table('table2', query)
 
     From other table
 
     >>> table2 = database.create_table('table2', table)
 
+    Uploading file
+
+    >>> db = server.get_database('files')
+    >>> db.create_table('filename', dataframe)
+
+  ` Droping table
+
+    >>> database.drop_table('table2')
+
     """
 
     def __init__(self, server, name):
         self.server = server
         self.name = name
         self.api = server.api
 
@@ -85,15 +96,15 @@
 
         if name not in self._list_tables():
             if '.' not in name:
                 # fixme: schemas not visible in 'show tables'
                 raise AttributeError("Table doesn't exist")
         return Table(self, name)
 
-    def create_table(self, name: str, query: Query, replace: bool = False) -> Table:
+    def create_table(self, name: str, query: Union[pd.DataFrame, Query], replace: bool = False) -> Table:
         """
         Create new table and return it.
 
         On mindsdb server it executes command:
         `insert into a (select ...)`
 
         or if replace is True
@@ -103,14 +114,20 @@
 
         :param name: name of table
         :param query: Query object
         :param replace: if true,
         :return: Table object
         """
 
+        if isinstance(query, pd.DataFrame) and self.name == 'files':
+            # now it is only possible for file uploading
+            self.api.upload_file(name, query)
+
+            return Table(self, name)
+
         if not isinstance(query, Query):
             raise NotImplementedError
 
         # # query can be in different database: wrap to NativeQuery
         # ast_query = CreateTable(
         #     name=Identifier(name),
         #     is_replace=is_replace,
@@ -133,7 +150,20 @@
 
         self.api.sql_query(
             f'create{replace_str} table {table.to_string()} ({query.sql})',
             database=query.database
         )
 
         return Table(self, name)
+
+    def drop_table(self, name: str):
+        """
+        Delete table
+
+        :param name: name of table
+        """
+        ast_query = DropTables(
+            tables=[
+                Identifier(parts=[name])
+            ]
+        )
+        self.api.sql_query(ast_query.to_string(), database=self.name)
```

### Comparing `mindsdb_sdk-1.0.4/mindsdb_sdk/model.py` & `mindsdb_sdk-1.0.5/mindsdb_sdk/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def _get_identifier(self):
         parts = [self.project.name, self.name]
         if self.version is not None:
             parts.append(str(self.version))
         return Identifier(parts=parts)
 
-    def predict(self, data: Union[pd.DataFrame, Query], params: dict = None) -> pd.DataFrame:
+    def predict(self, data: Union[pd.DataFrame, Query, dict], params: dict = None) -> pd.DataFrame:
         """
         Make prediction using model
 
         if data is dataframe it uses /model/predict http method and sends dataframe over it
         if data is select query with one table it replaces table to jon table and predictor
         and sends query over sql/query http method
 
@@ -97,14 +97,18 @@
                 )
             )
             if params is not None:
                 ast_query.using = params
             # execute in query's database
             return self.project.api.sql_query(ast_query.to_string(), database=data.database)
 
+        elif isinstance(data, dict):
+            data = pd.DataFrame([data])
+            return self.project.api.model_predict(self.project.name, self.name, data,
+                                                  params=params, version=self.version)
         elif isinstance(data, pd.DataFrame):
             return self.project.api.model_predict(self.project.name, self.name, data,
                                                   params=params, version=self.version)
         else:
             raise ValueError('Unknown input')
 
     def get_status(self) -> str:
```

### Comparing `mindsdb_sdk-1.0.4/mindsdb_sdk/project.py` & `mindsdb_sdk-1.0.5/mindsdb_sdk/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,18 @@
     Usng model
 
     Dataframe on input
 
     >>> result_df = model.predict(df_rental)
     >>> result_df = model.predict(df_rental, params={'a': 'q'})
 
+    Dict on input
+
+    >>> result_df = model.predict({'n_rooms': 2})
+
     Deferred query on input
 
     >>> result_df = model.predict(query, params={'': ''})
 
     Time series prediction
 
     >>> query = database.query('select * from table1 where type="house" and saledate>latest')
@@ -387,14 +391,20 @@
             name=Identifier(name),
             query_str=query,
             integration_name=database,
             targets=targets,
         )
 
         if timeseries_options is not None:
+            # check ts options
+            allowed_keys = ['group', 'order', 'window', 'horizon']
+            for key in timeseries_options.keys():
+                if key not in allowed_keys:
+                    raise AttributeError(f"Unexpected time series option: {key}")
+
             if 'group' in timeseries_options:
                 group = timeseries_options['group']
                 if not isinstance(group, list):
                     group = [group]
                 ast_query.group_by = [Identifier(i) for i in group]
             if 'order' in timeseries_options:
                 ast_query.order_by = [Identifier(timeseries_options['order'])]
```

### Comparing `mindsdb_sdk-1.0.4/mindsdb_sdk/query.py` & `mindsdb_sdk-1.0.5/mindsdb_sdk/query.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-1.0.4/mindsdb_sdk/server.py` & `mindsdb_sdk-1.0.5/mindsdb_sdk/server.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-1.0.4/mindsdb_sdk.egg-info/PKG-INFO` & `mindsdb_sdk-1.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,177 +1,146 @@
 Metadata-Version: 2.1
-Name: mindsdb-sdk
-Version: 1.0.4
+Name: mindsdb_sdk
+Version: 1.0.5
 Summary: MindsDB Python SDK, provides an SDK to use a remote mindsdb instance
 Home-page: https://github.com/mindsdb/mindsdb_python_sdk
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb-sdk/
 Description: # Python MindsDB SDK
-        It enables you to connect to a MindsDB server from python using HTTP API.
         
-        ## Install
+        The Python MindsDB SDK allows you to connect to a MindsDB server from Python using the HTTP API.
+        
+        ## Installation
+        
         ```
         pip install mindsdb_sdk
         ```
         
         ## Example
         
-        Connect:
-        ```python
-        import mindsdb_sdk
+        ### Connecting to the MindsDB server
+        
+        You can establish a connection to the MindsDB server using the SDK. Here are some examples:
         
-        # Connect to local server 
+        #### Connect to a local MindsDB server
         
+        ```python
+        import mindsdb_sdk
         server = mindsdb_sdk.connect()
         server = mindsdb_sdk.connect('http://127.0.0.1:47334')
+        ```
         
-        # Connect to cloud server
+        #### Connect to the MindsDB Cloud
         
+        ```python
+        import mindsdb_sdk
         server = mindsdb_sdk.connect(email='a@b.com', password='-')
         server = mindsdb_sdk.connect('https://cloud.mindsdb.com', login='a@b.com', password='-')
+        ```
         
-        # Connect to MindsDB Pro
+        ####  Connect to a MindsDB Pro server
         
+        ```python
+        import mindsdb_sdk
         server = mindsdb_sdk.connect('http://<YOUR_INSTANCE_IP>', login='a@b.com', password='-', is_managed=True)
-        
         ```
         
-        Base usage:
-        ```python
+        ## Basic usage
         
-        # database
+        Once connected to the server, you can perform various operations. Here are some examples:
+        
+        ```python
+        # Get a list of databases
         databases = server.list_databases()
         
-        database = databases[0] # Database type object
+        # Get a specific database
+        database = databases[0]  # Database type object
         
-        # sql query
+        # Perform an SQL query
         query = database.query('select * from table1')
         print(query.fetch())
         
-        # create table
+        # Create a table
         table = database.create_table('table2', query)
         
-        
-        # project
+        # Get a project
         project = server.get_project('proj')
         
-        # sql query
+        # Perform an SQL query within a project
         query = project.query('select * from database.table join model1')
         
-        # create view
-        view = project.create_view(
-              'btc_view',
-               query=query
-        )
+        # Create a view
+        view = project.create_view('view1', query=query)
         
-        # get view
+        # Get a list of views
         views = project.list_views()
         view = views[0]
         df = view.fetch()
         
-        # get model
+        # Get a list of models
         models = project.list_models()
         model = models[0]
         
-        # using model
+        # Use a model for prediction
         result_df = model.predict(df)
         result_df = model.predict(query)
         
-        # create model
+        # Create a model
+        timeseries_options = {
+            'order': 'date',
+            'window': 5,
+            'horizon': 1
+        }
         model = project.create_model(
-              'rentals_model',
-              predict='price',
-              query=query,
+            'rentals_model',
+            predict='price',
+            query=query,
+            timeseries_options=timeseries_options
         )
         
         ```
         
-        More examples in [Google colab notebook](
+        You can find more examples in this [Google colab notebook](
         https://colab.research.google.com/drive/1QouwAR3saFb9ffthrIs1LSH5COzyQa11#scrollTo=k6IbwsKRPQCR
         )
         
-        ## API documentation
-        
-        Api documentation can be found in: 
-        https://mindsdb.github.io/mindsdb_python_sdk/
-        
+        ## API Documentation
         
-        **Generating api docs:**
+        The API documentation for the MindsDB SDK can be found at https://mindsdb.github.io/mindsdb_python_sdk/. You can generate the API documentation locally by following these steps:
         
-        Locally:
+        ### Generating API docs locally:
         
         ```commandline
         cd docs
-        
         pip install -r requirements.txt
-        
         make html
         ```
         
+        The online documentation is automatically updated by pushing changes to the docs branch.
         
-        **Online documentation** is updated by pushing in `docs` branch
         
+        ## Testing
         
-        
-        ## How to test
-        `
-        It runs all tests for components 
+        To run all the tests for the components, use the following command:
         
         ```bash
         env PYTHONPATH=./ pytest
         ```
         
-        ## How to Connect From a Python File
-        
-        Create a file in your python project's root directory to store the connection details:
-        
-        `server.py` 
-        
-        Add the connection arguments with **your MindsDB credentials** to `server.py`:
-        
-        ```python
-        import mindsdb_sdk
-        
-        server = mindsdb_sdk.connect()
-        server = mindsdb_sdk.connect('http://127.0.0.1:47334')
-        
-        server = mindsdb_sdk.connect(email='your_mindsdb_email', password='your_mindsdb_password')
-        server = mindsdb_sdk.connect('https://cloud.mindsdb.com', email='your_mindsdb_email', password='your_mindsdb_password')
-        ```
+        ## Contributing
         
-        Open your terminal and type:
+        We welcome contributions to the MindsDB SDK. If you'd like to contribute, please refer to the contribution guidelines for more information.
         
-        `python server.py` 
+        ## License
         
-        ### Testing the Connection
+        The MindsDB SDK is licensed under the MIT License. Feel free to use and modify it according to your needs
         
-        Add test queries to `server.py` with `print()` statements to confirm the connection:
-        
-        ```python
-        import mindsdb_sdk #import the mindsdb_sdk package
-        
-        server = mindsdb_sdk.connect()
-        server = mindsdb_sdk.connect('http://127.0.0.1:47334')
-        
-        #  Input your MindsDB Cloud Credentials below to connect to MindsDB Cloud
-        server = mindsdb_sdk.connect(email='your_mindsdb_email', password='your_mindsdb_password')
-        server = mindsdb_sdk.connect('https://cloud.mindsdb.com', email='your_mindsdb_email', password='your_mindsdb_password') # Connect to MindsDB server in the cloud
-        
-        databases = server.list_databases()
-        
-        database = databases[1] # Database type object
-        
-        query = database.query('select * from files.test_data')
-        print(database)
-        ```
         
-        To see a full example, checkout:
-        `server.py`
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `mindsdb_sdk-1.0.4/setup.py` & `mindsdb_sdk-1.0.5/setup.py`

 * *Files identical despite different names*

