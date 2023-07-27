# Comparing `tmp/database_testing_tools-1.0.1.tar.gz` & `tmp/database_testing_tools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_testing_tools-1.0.1.tar", max compression
+gzip compressed data, was "database_testing_tools-1.0.2.tar", max compression
```

## Comparing `database_testing_tools-1.0.1.tar` & `database_testing_tools-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3846 2023-07-26 12:03:41.752716 database_testing_tools-1.0.1/README.md
--rw-r--r--   0        0        0    40943 2023-07-26 12:03:41.752716 database_testing_tools-1.0.1/database_testing_tools/__init__.py
--rw-r--r--   0        0        0     3982 2023-07-26 12:03:41.752716 database_testing_tools-1.0.1/database_testing_tools/utils.py
--rw-r--r--   0        0        0     1067 2023-07-26 12:03:41.756716 database_testing_tools-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 database_testing_tools-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3832 2023-07-27 09:20:13.023036 database_testing_tools-1.0.2/README.md
+-rw-r--r--   0        0        0    40943 2023-07-27 09:20:13.023036 database_testing_tools-1.0.2/database_testing_tools/__init__.py
+-rw-r--r--   0        0        0     3975 2023-07-27 09:20:13.023036 database_testing_tools-1.0.2/database_testing_tools/utils.py
+-rw-r--r--   0        0        0     1067 2023-07-27 09:20:13.023036 database_testing_tools-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 database_testing_tools-1.0.2/PKG-INFO
```

### Comparing `database_testing_tools-1.0.1/README.md` & `database_testing_tools-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,8 +47,8 @@
 query_engine = DuckDbEngine(conn)
 tester = Tester(query_engine=query_engine)
 database = "some_database"
 
 tester.check_all_tables_return_data(db_name=database)
 ```
 
-Alternative database engines should follow a similar pattern to the DuckDB engine - an initialiser that includes the database connection object, and an implementation of the `run_query` function that runs a given SQL query and returns the result as a pandas dataframe. As the built-in tests use [the Presto SQL dialect](https://prestodb.io/docs/current/index.html), it is recommended to transpile the SQL with [sqlglot](https://sqlglot.com/sqlglot.html) to ensure the tests are executed correctly.
+Alternative database engines should follow a similar pattern to the DuckDB engine - an initialiser that includes the database connection object, and an implementation of the `run_query` function that runs a given SQL query and returns the result as a pandas dataframe. As the built-in tests use [the Trino SQL dialect](https://trino.io/docs/current/), it is recommended to transpile the SQL with [sqlglot](https://sqlglot.com/sqlglot.html) to ensure the tests are executed correctly.
```

### Comparing `database_testing_tools-1.0.1/database_testing_tools/__init__.py` & `database_testing_tools-1.0.2/database_testing_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `database_testing_tools-1.0.1/database_testing_tools/utils.py` & `database_testing_tools-1.0.2/database_testing_tools/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class BaseQueryEngine(ABC):
     @abstractmethod
     def run_query(self, sql):
         """
         Returns a dataframe by executing a query with the specified database engine.
         The queries written in the package were designed to work with Amazon Athena,
-        which uses the Presto SQL dialect, so other implementations need to include
+        which uses the Trino SQL dialect, so other implementations need to include
         a transpile step with sqlglot in order to run correctly.
         """
         pass
 
     def get_tables(self, db_name: str) -> List[str]:
         """ Returns a list of all tables in database """
         query = (
@@ -40,19 +40,19 @@
 
 class DuckDbEngine(BaseQueryEngine):
     def __init__(self, conn: DuckDBPyConnection):
         self.conn = conn
 
     def run_query(self, sql, **kwargs):
         """
-        Transpiles the given SQL from presto to duckdb,
+        Transpiles the given SQL from Trino to duckdb,
         then runs the query and returns as a dataframe
         """
-        query = sqlglot.transpile(sql, read="presto", write="duckdb")[0]
-        return self.conn.execute(query).df()
+        query = sqlglot.transpile(sql, read="trino", write="duckdb")[0]
+        return self.conn.sql(query).df()
 
 
 def write_hidden_notebook_cells(in_path: str, outpath: str = None) -> str:
     """Iterate through code cells and set the metadata of the cell to hidden
     for commuter if the cell starts with "# meta.hide-input" or is tagged as
     "hide-input". Tag names are taken from jupyterbook tag notation.
     Writes the editted notebook to a specified outpath
```

### Comparing `database_testing_tools-1.0.1/pyproject.toml` & `database_testing_tools-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "database-testing-tools"
-version = "1.0.1"
+version = "1.0.2"
 description = "A package to test our databases"
 authors = ["Thomas Hirsch <thomas.hirsch@digital.justice.gov.uk>",
            "Stephen Bias <stephen.bias@digital.justice.gov.uk>",
            "Tapan Perkins <tapan.perkins@digital.justice.gov.uk>",
            "Matt Laverty <matthew.laverty@justice.gov.uk>",
            "Karik Isichei <karik.isichei@digital.justice.gov.uk>",
            "George Kelly <george.kelly@digital.justice.gov.uk>",
@@ -15,15 +15,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4"
 altair = "^4.1"
 pydbtools = "^5.2"
 dataengineeringutils3 = "^1.4"
 papermill = "^2.3.3"
-duckdb = "^0.4.0"
+duckdb = "^0.8.0"
 arrow-pd-parser = "^1.3.1"
 mojap-metadata = "^1.10.0"
 sqlglot = "^4.3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.1"
 flake8 = "^3.8.3"
```

### Comparing `database_testing_tools-1.0.1/PKG-INFO` & `database_testing_tools-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: database-testing-tools
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package to test our databases
 Home-page: https://github.com/moj-analytical-services/database-testing-tools
 Author: Thomas Hirsch
 Author-email: thomas.hirsch@digital.justice.gov.uk
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: altair (>=4.1,<5.0)
 Requires-Dist: arrow-pd-parser (>=1.3.1,<2.0.0)
 Requires-Dist: dataengineeringutils3 (>=1.4,<2.0)
-Requires-Dist: duckdb (>=0.4.0,<0.5.0)
+Requires-Dist: duckdb (>=0.8.0,<0.9.0)
 Requires-Dist: mojap-metadata (>=1.10.0,<2.0.0)
 Requires-Dist: papermill (>=2.3.3,<3.0.0)
 Requires-Dist: pydbtools (>=5.2,<6.0)
 Requires-Dist: sqlglot (>=4.3.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # database-testing-tools
@@ -70,8 +70,8 @@
 query_engine = DuckDbEngine(conn)
 tester = Tester(query_engine=query_engine)
 database = "some_database"
 
 tester.check_all_tables_return_data(db_name=database)
 ```
 
-Alternative database engines should follow a similar pattern to the DuckDB engine - an initialiser that includes the database connection object, and an implementation of the `run_query` function that runs a given SQL query and returns the result as a pandas dataframe. As the built-in tests use [the Presto SQL dialect](https://prestodb.io/docs/current/index.html), it is recommended to transpile the SQL with [sqlglot](https://sqlglot.com/sqlglot.html) to ensure the tests are executed correctly.
+Alternative database engines should follow a similar pattern to the DuckDB engine - an initialiser that includes the database connection object, and an implementation of the `run_query` function that runs a given SQL query and returns the result as a pandas dataframe. As the built-in tests use [the Trino SQL dialect](https://trino.io/docs/current/), it is recommended to transpile the SQL with [sqlglot](https://sqlglot.com/sqlglot.html) to ensure the tests are executed correctly.
```

