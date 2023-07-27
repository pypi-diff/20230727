# Comparing `tmp/excellentman-1.0.0.tar.gz` & `tmp/excellentman-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excellentman-1.0.0.tar", last modified: Tue Sep 27 12:51:44 2022, max compression
+gzip compressed data, was "excellentman-1.1.0.tar", last modified: Thu Jul 27 19:13:18 2023, max compression
```

## Comparing `excellentman-1.0.0.tar` & `excellentman-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2022-09-27 12:51:44.287044 excellentman-1.0.0/
--rw-r--r--   0 alec       (501) staff       (20)     3428 2022-09-27 12:51:44.286889 excellentman-1.0.0/PKG-INFO
--rw-r--r--   0 alec       (501) staff       (20)     2520 2022-09-27 12:51:26.000000 excellentman-1.0.0/README.md
--rw-r--r--   0 alec       (501) staff       (20)       38 2022-09-27 12:51:44.287098 excellentman-1.0.0/setup.cfg
--rw-r--r--   0 alec       (501) staff       (20)     1322 2022-09-27 12:51:26.000000 excellentman-1.0.0/setup.py
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2022-09-27 12:51:44.285717 excellentman-1.0.0/src/
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2022-09-27 12:51:44.286672 excellentman-1.0.0/src/excellentman.egg-info/
--rw-r--r--   0 alec       (501) staff       (20)     3428 2022-09-27 12:51:44.000000 excellentman-1.0.0/src/excellentman.egg-info/PKG-INFO
--rw-r--r--   0 alec       (501) staff       (20)      280 2022-09-27 12:51:44.000000 excellentman-1.0.0/src/excellentman.egg-info/SOURCES.txt
--rw-r--r--   0 alec       (501) staff       (20)        1 2022-09-27 12:51:44.000000 excellentman-1.0.0/src/excellentman.egg-info/dependency_links.txt
--rw-r--r--   0 alec       (501) staff       (20)       52 2022-09-27 12:51:44.000000 excellentman-1.0.0/src/excellentman.egg-info/entry_points.txt
--rw-r--r--   0 alec       (501) staff       (20)        9 2022-09-27 12:51:44.000000 excellentman-1.0.0/src/excellentman.egg-info/requires.txt
--rw-r--r--   0 alec       (501) staff       (20)       13 2022-09-27 12:51:44.000000 excellentman-1.0.0/src/excellentman.egg-info/top_level.txt
--rw-r--r--   0 alec       (501) staff       (20)     3662 2022-09-27 12:51:26.000000 excellentman-1.0.0/src/excellentman.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-07-27 19:13:18.432570 excellentman-1.1.0/
+-rw-r--r--   0 alec       (501) staff       (20)     3096 2023-07-27 19:13:18.432394 excellentman-1.1.0/PKG-INFO
+-rw-r--r--   0 alec       (501) staff       (20)     2679 2023-07-27 19:13:09.000000 excellentman-1.1.0/README.md
+-rw-r--r--   0 alec       (501) staff       (20)       38 2023-07-27 19:13:18.432624 excellentman-1.1.0/setup.cfg
+-rw-r--r--   0 alec       (501) staff       (20)     1322 2023-07-27 19:13:09.000000 excellentman-1.1.0/setup.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-07-27 19:13:18.431053 excellentman-1.1.0/src/
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2023-07-27 19:13:18.432164 excellentman-1.1.0/src/excellentman.egg-info/
+-rw-r--r--   0 alec       (501) staff       (20)     3096 2023-07-27 19:13:18.000000 excellentman-1.1.0/src/excellentman.egg-info/PKG-INFO
+-rw-r--r--   0 alec       (501) staff       (20)      280 2023-07-27 19:13:18.000000 excellentman-1.1.0/src/excellentman.egg-info/SOURCES.txt
+-rw-r--r--   0 alec       (501) staff       (20)        1 2023-07-27 19:13:18.000000 excellentman-1.1.0/src/excellentman.egg-info/dependency_links.txt
+-rw-r--r--   0 alec       (501) staff       (20)       52 2023-07-27 19:13:18.000000 excellentman-1.1.0/src/excellentman.egg-info/entry_points.txt
+-rw-r--r--   0 alec       (501) staff       (20)        9 2023-07-27 19:13:18.000000 excellentman-1.1.0/src/excellentman.egg-info/requires.txt
+-rw-r--r--   0 alec       (501) staff       (20)       13 2023-07-27 19:13:18.000000 excellentman-1.1.0/src/excellentman.egg-info/top_level.txt
+-rw-r--r--   0 alec       (501) staff       (20)     5156 2023-07-27 19:13:09.000000 excellentman-1.1.0/src/excellentman.py
```

### Comparing `excellentman-1.0.0/PKG-INFO` & `excellentman-1.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,62 @@
-Metadata-Version: 2.1
-Name: excellentman
-Version: 1.0.0
-Summary: A tool for running Newman with parameters from an Excel file
-Home-page: UNKNOWN
-Author: Alec and Lindsay
-License: UNKNOWN
-Description: # excellentman
-        An experimental repo for probably writing tools to execute parameterized newman runs from data in spreadsheets
-        
-        ## Install Newman
-        
-        1. Download and install [Node.js](https://nodejs.org/en/download/current/).
-        2. Then, run the command `npm install -g newman` in your CLI.
-        3. Install the HTML reporter `npm install -g newman-reporter-htmlextra`
-        
-        ## Installing
-        
-        `pip install -i https://test.pypi.org/simple/ excellentman==0.9.0`
-        
-        ## Usage
-        
-        `excellentman <EXCEL_FILE> <JSON_COLLECTION> <ENVIRONMENT_FILE>`
-        
-        Where:
-         - *EXCEL_FILE*: is a an excel file where each worksheet contains parameters to be passed into the postman requests
-         - *JSON_COLLECTION*: collection of requests, either a URL, or downloaded from postman
-         - *ENVIRONMENT_FILE*: an exported Postman environments file
-        
-        ## Example
-        
-        We've included example data for querying https://www.thecocktaildb.com, in the `examples` directory.
-        
-         - `examples/Cocktails.postman_collection.json` - A postman collection for querying the cocktail database
-         - `examples/Cocktails.xlsx` - An excel file with multiple worksheets for different types of cocktails
-         - `examples/Production Cocktails.postman_environment.json` - An environment file for parameterizing the requests
-        
-        You can run this:
-        
-        `excellentman examples/Cocktails.xlsx examples/Cocktails.postman_collection.json "examples/Production Cocktails.postman_environment.json"`
-        
-        ### Custom Field Handling
-        
-        If you have data in your spreadsheet that needs to be transformed before it gets sent to the API you're working with, you can provide a python file of transformation functions, as in `examples/custom_formats.py`.
-        
-        We include a trivial example that lowercases the drink names, which you can demonstrate by running:
-        
-        `excellentman examples/Cocktails.xlsx examples/Cocktails.postman_collection.json "examples/Production Cocktails.postman_environment.json" --custom_formats=examples/custom_formats.py`
-        
-        ### Custom Report Formatting
-        
-        This tool use `newman-reporter-htmlextra` to provide an HTML report of the results. You can customize the template used for this report, and pass it in as follows:
-        
-        `excellentman examples/Cocktails.xlsx examples/Cocktails.postman_collection.json "examples/Production Cocktails.postman_environment.json" --custom_template=examples/example_reporter_template.hbs`
-        
-        ## Publishing a new version
-        
-        Update the version in setup.py.
-        
-        Build the version to publish
-        
-        `python3 setup.py sdist bdist_wheel`
-        
-        Publish to testpypi (for now)
-        
-        `python3 -m twine upload --repository testpypi dist/*`
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+# excellentman
+An experimental repo for probably writing tools to execute parameterized newman runs from data in spreadsheets
+
+## Install Newman
+
+1. Download and install [Node.js](https://nodejs.org/en/download/current/).
+2. Then, run the command `npm install -g newman` in your CLI.
+3. Install the HTML reporter `npm install -g newman-reporter-htmlextra`
+4. Install the xunit reporter, run command `npm install -g newman-reporter-xunit`
+
+## Installing
+
+`pip install excellentman`
+
+## Usage
+
+`excellentman <EXCEL_FILE> <JSON_COLLECTION> <ENVIRONMENT_FILE>`
+
+Where:
+ - *EXCEL_FILE*: is a an excel file where each worksheet contains parameters to be passed into the postman requests
+ - *JSON_COLLECTION*: collection of requests, either a URL, or downloaded from postman
+ - *ENVIRONMENT_FILE*: an exported Postman environments file
+
+## Example
+
+We've included example data for querying https://www.thecocktaildb.com, in the `examples` directory.
+
+ - `examples/Cocktails.postman_collection.json` - A postman collection for querying the cocktail database
+ - `examples/Cocktails.xlsx` - An excel file with multiple worksheets for different types of cocktails
+ - `examples/Production Cocktails.postman_environment.json` - An environment file for parameterizing the requests
+
+You can run this:
+
+`excellentman examples/Cocktails.xlsx examples/Cocktails.postman_collection.json "examples/Production Cocktails.postman_environment.json"`
+
+### Custom Field Handling
+
+If you have data in your spreadsheet that needs to be transformed before it gets sent to the API you're working with, you can provide a python file of transformation functions, as in `examples/custom_formats.py`.
+
+We include a trivial example that lowercases the drink names, which you can demonstrate by running:
+
+`excellentman examples/Cocktails.xlsx examples/Cocktails.postman_collection.json "examples/Production Cocktails.postman_environment.json" --custom_formats=examples/custom_formats.py`
+
+### Custom Report Formatting
+
+This tool uses `newman-reporter-htmlextra` to provide an HTML report of the results and can also support `newman-reporter-xunit` to provide an XML report file. You can customize the template used for this report, and pass it in as follows:
+
+`excellentman examples/Cocktails.xlsx examples/Cocktails.postman_collection.json "examples/Production Cocktails.postman_environment.json" --custom_template=examples/example_reporter_template.hbs --xunit_file=xunit_reporter_example.xml`
+
+
+## Publishing a new version
+
+Update the version in setup.py.
+
+Build the version to publish
+
+`python3 setup.py sdist bdist_wheel`
+
+Publish to testpypi (for now)
+
+`python3 -m twine upload --repository testpypi dist/*`
+
```

### Comparing `excellentman-1.0.0/README.md` & `excellentman-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,34 @@
+Metadata-Version: 2.1
+Name: excellentman
+Version: 1.1.0
+Summary: A tool for running Newman with parameters from an Excel file
+Home-page: UNKNOWN
+Author: Alec and Lindsay
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # excellentman
 An experimental repo for probably writing tools to execute parameterized newman runs from data in spreadsheets
 
 ## Install Newman
 
 1. Download and install [Node.js](https://nodejs.org/en/download/current/).
 2. Then, run the command `npm install -g newman` in your CLI.
 3. Install the HTML reporter `npm install -g newman-reporter-htmlextra`
+4. Install the xunit reporter, run command `npm install -g newman-reporter-xunit`
 
 ## Installing
 
-`pip install -i https://test.pypi.org/simple/ excellentman==0.9.0`
+`pip install excellentman`
 
 ## Usage
 
 `excellentman <EXCEL_FILE> <JSON_COLLECTION> <ENVIRONMENT_FILE>`
 
 Where:
  - *EXCEL_FILE*: is a an excel file where each worksheet contains parameters to be passed into the postman requests
@@ -38,23 +53,26 @@
 
 We include a trivial example that lowercases the drink names, which you can demonstrate by running:
 
 `excellentman examples/Cocktails.xlsx examples/Cocktails.postman_collection.json "examples/Production Cocktails.postman_environment.json" --custom_formats=examples/custom_formats.py`
 
 ### Custom Report Formatting
 
-This tool use `newman-reporter-htmlextra` to provide an HTML report of the results. You can customize the template used for this report, and pass it in as follows:
+This tool uses `newman-reporter-htmlextra` to provide an HTML report of the results and can also support `newman-reporter-xunit` to provide an XML report file. You can customize the template used for this report, and pass it in as follows:
+
+`excellentman examples/Cocktails.xlsx examples/Cocktails.postman_collection.json "examples/Production Cocktails.postman_environment.json" --custom_template=examples/example_reporter_template.hbs --xunit_file=xunit_reporter_example.xml`
 
-`excellentman examples/Cocktails.xlsx examples/Cocktails.postman_collection.json "examples/Production Cocktails.postman_environment.json" --custom_template=examples/example_reporter_template.hbs`
 
 ## Publishing a new version
 
 Update the version in setup.py.
 
 Build the version to publish
 
 `python3 setup.py sdist bdist_wheel`
 
 Publish to testpypi (for now)
 
 `python3 -m twine upload --repository testpypi dist/*`
 
+
+
```

### Comparing `excellentman-1.0.0/setup.py` & `excellentman-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="excellentman",                     # This is the name of the package
-    version="1.0.0",                        
+    version="1.1.0",                        
     author="Alec and Lindsay",                     # Full name of the author
     description="A tool for running Newman with parameters from an Excel file",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

