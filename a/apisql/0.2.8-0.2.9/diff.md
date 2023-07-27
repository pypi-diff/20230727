# Comparing `tmp/apisql-0.2.8.tar.gz` & `tmp/apisql-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apisql-0.2.8.tar", last modified: Tue Feb 14 07:29:23 2023, max compression
+gzip compressed data, was "apisql-0.2.9.tar", last modified: Thu Jul 27 09:13:49 2023, max compression
```

## Comparing `apisql-0.2.8.tar` & `apisql-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-02-14 07:29:23.893376 apisql-0.2.8/
--rw-r--r--   0 adam       (501) staff       (20)      123 2021-06-14 07:03:57.000000 apisql-0.2.8/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)      457 2021-06-14 07:11:08.000000 apisql-0.2.8/Makefile
--rw-r--r--   0 adam       (501) staff       (20)     3521 2023-02-14 07:29:23.893591 apisql-0.2.8/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     2397 2021-07-06 12:06:14.000000 apisql-0.2.8/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-02-14 07:29:23.889838 apisql-0.2.8/apisql/
--rw-r--r--   0 adam       (501) staff       (20)        5 2023-02-14 07:27:15.000000 apisql-0.2.8/apisql/VERSION
--rw-r--r--   0 adam       (501) staff       (20)       59 2021-06-14 08:02:53.000000 apisql-0.2.8/apisql/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     5098 2023-02-14 07:27:10.000000 apisql-0.2.8/apisql/blueprint.py
--rw-r--r--   0 adam       (501) staff       (20)     4858 2022-09-07 07:34:48.000000 apisql-0.2.8/apisql/controllers.py
--rw-r--r--   0 adam       (501) staff       (20)      264 2021-06-14 08:03:28.000000 apisql-0.2.8/apisql/logger.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-02-14 07:29:23.893059 apisql-0.2.8/apisql/utils/
--rw-r--r--   0 adam       (501) staff       (20)        0 2021-06-14 07:03:57.000000 apisql-0.2.8/apisql/utils/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     7488 2021-06-14 07:03:57.000000 apisql-0.2.8/apisql/utils/file_maker.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-02-14 07:29:23.892418 apisql-0.2.8/apisql.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)     3521 2023-02-14 07:29:23.000000 apisql-0.2.8/apisql.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      372 2023-02-14 07:29:23.000000 apisql-0.2.8/apisql.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-02-14 07:29:23.000000 apisql-0.2.8/apisql.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2021-06-15 10:13:09.000000 apisql-0.2.8/apisql.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)      156 2023-02-14 07:29:23.000000 apisql-0.2.8/apisql.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)        7 2023-02-14 07:29:23.000000 apisql-0.2.8/apisql.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)       67 2023-02-14 07:29:23.894172 apisql-0.2.8/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     1815 2021-06-15 10:19:05.000000 apisql-0.2.8/setup.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-27 09:13:49.363555 apisql-0.2.9/
+-rw-r--r--   0 adam       (501) staff       (20)     1067 2021-06-14 07:10:44.000000 apisql-0.2.9/LICENSE
+-rw-r--r--   0 adam       (501) staff       (20)      123 2021-06-14 07:03:57.000000 apisql-0.2.9/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)      457 2021-06-14 07:11:08.000000 apisql-0.2.9/Makefile
+-rw-r--r--   0 adam       (501) staff       (20)     3041 2023-07-27 09:13:49.363738 apisql-0.2.9/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     2397 2021-07-06 12:06:14.000000 apisql-0.2.9/README.md
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-27 09:13:49.357478 apisql-0.2.9/apisql/
+-rw-r--r--   0 adam       (501) staff       (20)        5 2023-07-27 08:59:13.000000 apisql-0.2.9/apisql/VERSION
+-rw-r--r--   0 adam       (501) staff       (20)       59 2021-06-14 08:02:53.000000 apisql-0.2.9/apisql/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     5092 2023-07-27 08:58:47.000000 apisql-0.2.9/apisql/blueprint.py
+-rw-r--r--   0 adam       (501) staff       (20)     4858 2022-09-07 07:34:48.000000 apisql-0.2.9/apisql/controllers.py
+-rw-r--r--   0 adam       (501) staff       (20)      264 2021-06-14 08:03:28.000000 apisql-0.2.9/apisql/logger.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-27 09:13:49.362765 apisql-0.2.9/apisql/utils/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2021-06-14 07:03:57.000000 apisql-0.2.9/apisql/utils/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     7488 2021-06-14 07:03:57.000000 apisql-0.2.9/apisql/utils/file_maker.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-27 09:13:49.361737 apisql-0.2.9/apisql.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     3041 2023-07-27 09:13:49.000000 apisql-0.2.9/apisql.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      380 2023-07-27 09:13:49.000000 apisql-0.2.9/apisql.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-27 09:13:49.000000 apisql-0.2.9/apisql.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2021-06-15 10:13:09.000000 apisql-0.2.9/apisql.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)      156 2023-07-27 09:13:49.000000 apisql-0.2.9/apisql.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)        7 2023-07-27 09:13:49.000000 apisql-0.2.9/apisql.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)       67 2023-07-27 09:13:49.364367 apisql-0.2.9/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     1815 2021-06-15 10:19:05.000000 apisql-0.2.9/setup.py
```

### Comparing `apisql-0.2.8/PKG-INFO` & `apisql-0.2.9/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,60 @@
-Metadata-Version: 2.1
-Name: apisql
-Version: 0.2.8
-Summary: A flask blueprint providing a read-lny API for querying RDBMS
-Home-page: https://github.com/dataspot/apisql
-Author: Adam Kariv
-Author-email: adam.kariv@gmail.com
-License: MIT
-Description: # apisql
-        
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/apisql.svg)
-        
-        apisql is a flask blueprint providing an API for read-only access for a DBMS using direct SQL Queries
-        
-        ## endpoints
-        
-        ### `/query`
-        
-        Returns query results in json format.
-        
-        Query parameters that can be send:
-        - **query**: The SQL query to execute on the DB. The query can be provided in plain text or base64 encoded.
-        - **num_rows**: The maximum number of rows to return. If not specified, will return the aount defined in the configuration, the amount defined in the environment variable `APISQL__MAX_ROWS` or 100.
-        - **page_size**: The size of the 'page', when doing paging. By default will use `num_rows` and in any way the page size it won't exceed `num_rows`.
-        - **page**: Which page to fetch, starting from page 0
-        
-        ### `/download`
-        
-        Downloads query results in either csv, xls or xlsx format.
-        
-        Query parameters that can be send:
-        - **query**: The SQL query to execute on the DB. The query can be provided in plain text or base64 encoded.
-        - **format**: Either `csv` or `xlsx`. Defaults to `csv`.
-        - **filename**: The filename for the file to be downloaded, *without the extension*. Defaults to `query-results`.
-        - **headers**: A semicolon separated list of the headers for the output file. Headers should match the field names that appear in the query.
-          Headers may contain one or more modifiers, which appear after a colon. The currently supported modifiers are:
-          - `number`, to convert numeric values to strings
-          - `yesno`, which converts boolean values to "Yes" / "No"
-          - `comma-separated`, which converts arrays of strings to a comma separated list of these strings.
-          Finally, the content for a column may be fetched from a different field in the query output, by specifying the field name after a `<` character.
-        
-          Example:
-          `Fiscal Year:number<fiscal_year;Leap Year:yesno<0;`
-        
-        
-        
-        **Example:**
-        For the following SQL:
-        ```
-        select employee_name as "Employee Name", employee_salary as "Salary", is_manager as "Managerial role?" from employees
-        ```
-        
-        `headers` could be specified as `Employee Name;Managerial role?:yesno;Salary:number`.
-        
-        ## configuration
-        
-        Flask configuration for this blueprint:
-        
-        
-        ```python
-        
-            from apisql import apisql_blueprint
-        
-            app.register_blueprint(
-                apisql_blueprint(connection_string='psql://host/database', max_rows=1000, debug=False),
-                url_prefix='/api/db/'
-            )
-        ```
-Keywords: data
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Provides-Extra: develop
+# apisql
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/apisql.svg)
+
+apisql is a flask blueprint providing an API for read-only access for a DBMS using direct SQL Queries
+
+## endpoints
+
+### `/query`
+
+Returns query results in json format.
+
+Query parameters that can be send:
+- **query**: The SQL query to execute on the DB. The query can be provided in plain text or base64 encoded.
+- **num_rows**: The maximum number of rows to return. If not specified, will return the aount defined in the configuration, the amount defined in the environment variable `APISQL__MAX_ROWS` or 100.
+- **page_size**: The size of the 'page', when doing paging. By default will use `num_rows` and in any way the page size it won't exceed `num_rows`.
+- **page**: Which page to fetch, starting from page 0
+
+### `/download`
+
+Downloads query results in either csv, xls or xlsx format.
+
+Query parameters that can be send:
+- **query**: The SQL query to execute on the DB. The query can be provided in plain text or base64 encoded.
+- **format**: Either `csv` or `xlsx`. Defaults to `csv`.
+- **filename**: The filename for the file to be downloaded, *without the extension*. Defaults to `query-results`.
+- **headers**: A semicolon separated list of the headers for the output file. Headers should match the field names that appear in the query.
+  Headers may contain one or more modifiers, which appear after a colon. The currently supported modifiers are:
+  - `number`, to convert numeric values to strings
+  - `yesno`, which converts boolean values to "Yes" / "No"
+  - `comma-separated`, which converts arrays of strings to a comma separated list of these strings.
+  Finally, the content for a column may be fetched from a different field in the query output, by specifying the field name after a `<` character.
+
+  Example:
+  `Fiscal Year:number<fiscal_year;Leap Year:yesno<0;`
+
+
+
+**Example:**
+For the following SQL:
+```
+select employee_name as "Employee Name", employee_salary as "Salary", is_manager as "Managerial role?" from employees
+```
+
+`headers` could be specified as `Employee Name;Managerial role?:yesno;Salary:number`.
+
+## configuration
+
+Flask configuration for this blueprint:
+
+
+```python
+
+    from apisql import apisql_blueprint
+
+    app.register_blueprint(
+        apisql_blueprint(connection_string='psql://host/database', max_rows=1000, debug=False),
+        url_prefix='/api/db/'
+    )
+```
```

### Comparing `apisql-0.2.8/README.md` & `apisql-0.2.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: apisql
+Version: 0.2.9
+Summary: A flask blueprint providing a read-lny API for querying RDBMS
+Home-page: https://github.com/dataspot/apisql
+Author: Adam Kariv
+Author-email: adam.kariv@gmail.com
+License: MIT
+Keywords: data
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+Provides-Extra: develop
+License-File: LICENSE
+
 # apisql
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/apisql.svg)
 
 apisql is a flask blueprint providing an API for read-only access for a DBMS using direct SQL Queries
 
 ## endpoints
```

### Comparing `apisql-0.2.8/apisql/blueprint.py` & `apisql-0.2.9/apisql/blueprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                             if v is not None:
                                 try:
                                     worksheet.write_number(i, j, float(v))
                                 except ValueError:
                                     worksheet.write(i, j, str(v))
                 finally:
                     workbook.close()
-                return send_file(out.name, mimetype=mime, as_attachment=True, attachment_filename=file_name + '.xlsx')
+                return send_file(out.name, mimetype=mime, as_attachment=True, download_name=file_name + '.xlsx')
 
     def detect_bot(self):
         if request.user_agent.browser in ('google', 'aol', 'baidu', 'bing', 'yahoo'):
             logger.info('Bot detected %s: %s', request.user_agent.string, request.user_agent.browser)
         elif any(x in request.user_agent.string.lower() for x in ('applebot', 'yandexbot', 'petalbot')):
             logger.info('Bot detected %s: %s', request.user_agent.string, request.user_agent.browser)
         else:
```

### Comparing `apisql-0.2.8/apisql/controllers.py` & `apisql-0.2.9/apisql/controllers.py`

 * *Files identical despite different names*

### Comparing `apisql-0.2.8/apisql/utils/file_maker.py` & `apisql-0.2.9/apisql/utils/file_maker.py`

 * *Files identical despite different names*

### Comparing `apisql-0.2.8/apisql.egg-info/PKG-INFO` & `apisql-0.2.9/apisql.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 Metadata-Version: 2.1
 Name: apisql
-Version: 0.2.8
+Version: 0.2.9
 Summary: A flask blueprint providing a read-lny API for querying RDBMS
 Home-page: https://github.com/dataspot/apisql
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
-Description: # apisql
-        
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/apisql.svg)
-        
-        apisql is a flask blueprint providing an API for read-only access for a DBMS using direct SQL Queries
-        
-        ## endpoints
-        
-        ### `/query`
-        
-        Returns query results in json format.
-        
-        Query parameters that can be send:
-        - **query**: The SQL query to execute on the DB. The query can be provided in plain text or base64 encoded.
-        - **num_rows**: The maximum number of rows to return. If not specified, will return the aount defined in the configuration, the amount defined in the environment variable `APISQL__MAX_ROWS` or 100.
-        - **page_size**: The size of the 'page', when doing paging. By default will use `num_rows` and in any way the page size it won't exceed `num_rows`.
-        - **page**: Which page to fetch, starting from page 0
-        
-        ### `/download`
-        
-        Downloads query results in either csv, xls or xlsx format.
-        
-        Query parameters that can be send:
-        - **query**: The SQL query to execute on the DB. The query can be provided in plain text or base64 encoded.
-        - **format**: Either `csv` or `xlsx`. Defaults to `csv`.
-        - **filename**: The filename for the file to be downloaded, *without the extension*. Defaults to `query-results`.
-        - **headers**: A semicolon separated list of the headers for the output file. Headers should match the field names that appear in the query.
-          Headers may contain one or more modifiers, which appear after a colon. The currently supported modifiers are:
-          - `number`, to convert numeric values to strings
-          - `yesno`, which converts boolean values to "Yes" / "No"
-          - `comma-separated`, which converts arrays of strings to a comma separated list of these strings.
-          Finally, the content for a column may be fetched from a different field in the query output, by specifying the field name after a `<` character.
-        
-          Example:
-          `Fiscal Year:number<fiscal_year;Leap Year:yesno<0;`
-        
-        
-        
-        **Example:**
-        For the following SQL:
-        ```
-        select employee_name as "Employee Name", employee_salary as "Salary", is_manager as "Managerial role?" from employees
-        ```
-        
-        `headers` could be specified as `Employee Name;Managerial role?:yesno;Salary:number`.
-        
-        ## configuration
-        
-        Flask configuration for this blueprint:
-        
-        
-        ```python
-        
-            from apisql import apisql_blueprint
-        
-            app.register_blueprint(
-                apisql_blueprint(connection_string='psql://host/database', max_rows=1000, debug=False),
-                url_prefix='/api/db/'
-            )
-        ```
 Keywords: data
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: develop
+License-File: LICENSE
+
+# apisql
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/apisql.svg)
+
+apisql is a flask blueprint providing an API for read-only access for a DBMS using direct SQL Queries
+
+## endpoints
+
+### `/query`
+
+Returns query results in json format.
+
+Query parameters that can be send:
+- **query**: The SQL query to execute on the DB. The query can be provided in plain text or base64 encoded.
+- **num_rows**: The maximum number of rows to return. If not specified, will return the aount defined in the configuration, the amount defined in the environment variable `APISQL__MAX_ROWS` or 100.
+- **page_size**: The size of the 'page', when doing paging. By default will use `num_rows` and in any way the page size it won't exceed `num_rows`.
+- **page**: Which page to fetch, starting from page 0
+
+### `/download`
+
+Downloads query results in either csv, xls or xlsx format.
+
+Query parameters that can be send:
+- **query**: The SQL query to execute on the DB. The query can be provided in plain text or base64 encoded.
+- **format**: Either `csv` or `xlsx`. Defaults to `csv`.
+- **filename**: The filename for the file to be downloaded, *without the extension*. Defaults to `query-results`.
+- **headers**: A semicolon separated list of the headers for the output file. Headers should match the field names that appear in the query.
+  Headers may contain one or more modifiers, which appear after a colon. The currently supported modifiers are:
+  - `number`, to convert numeric values to strings
+  - `yesno`, which converts boolean values to "Yes" / "No"
+  - `comma-separated`, which converts arrays of strings to a comma separated list of these strings.
+  Finally, the content for a column may be fetched from a different field in the query output, by specifying the field name after a `<` character.
+
+  Example:
+  `Fiscal Year:number<fiscal_year;Leap Year:yesno<0;`
+
+
+
+**Example:**
+For the following SQL:
+```
+select employee_name as "Employee Name", employee_salary as "Salary", is_manager as "Managerial role?" from employees
+```
+
+`headers` could be specified as `Employee Name;Managerial role?:yesno;Salary:number`.
+
+## configuration
+
+Flask configuration for this blueprint:
+
+
+```python
+
+    from apisql import apisql_blueprint
+
+    app.register_blueprint(
+        apisql_blueprint(connection_string='psql://host/database', max_rows=1000, debug=False),
+        url_prefix='/api/db/'
+    )
+```
```

### Comparing `apisql-0.2.8/setup.py` & `apisql-0.2.9/setup.py`

 * *Files identical despite different names*

