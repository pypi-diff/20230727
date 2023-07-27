# Comparing `tmp/FastXlsToCsv-1.0.0.tar.gz` & `tmp/FastXlsToCsv-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastXlsToCsv-1.0.0.tar", last modified: Mon Jul 24 20:39:10 2023, max compression
+gzip compressed data, was "FastXlsToCsv-1.2.1.tar", last modified: Thu Jul 27 20:13:19 2023, max compression
```

## Comparing `FastXlsToCsv-1.0.0.tar` & `FastXlsToCsv-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 20:39:10.525823 FastXlsToCsv-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-07-24 20:39:10.506803 FastXlsToCsv-1.0.0/FastXlsToCsv/
--rw-rw-rw-   0        0        0     3381 2023-07-24 20:34:19.000000 FastXlsToCsv-1.0.0/FastXlsToCsv/XlsConverter.py
--rw-rw-rw-   0        0        0     1145 2023-07-24 20:34:19.000000 FastXlsToCsv-1.0.0/FastXlsToCsv/_XlsToCsvExceptions.py
--rw-rw-rw-   0        0        0      187 2023-07-24 20:34:19.000000 FastXlsToCsv-1.0.0/FastXlsToCsv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 20:39:10.522757 FastXlsToCsv-1.0.0/FastXlsToCsv.egg-info/
--rw-rw-rw-   0        0        0     1380 2023-07-24 20:39:10.000000 FastXlsToCsv-1.0.0/FastXlsToCsv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-24 20:39:10.000000 FastXlsToCsv-1.0.0/FastXlsToCsv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 20:39:10.000000 FastXlsToCsv-1.0.0/FastXlsToCsv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-24 20:39:10.000000 FastXlsToCsv-1.0.0/FastXlsToCsv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1105 2023-07-24 20:34:19.000000 FastXlsToCsv-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1380 2023-07-24 20:39:10.525170 FastXlsToCsv-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      905 2023-07-24 20:34:19.000000 FastXlsToCsv-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 20:39:10.525823 FastXlsToCsv-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      778 2023-07-24 20:34:19.000000 FastXlsToCsv-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:13:19.344746 FastXlsToCsv-1.2.1/
+drwxrwxrwx   0        0        0        0 2023-07-27 20:13:19.333449 FastXlsToCsv-1.2.1/FastXlsToCsv/
+-rw-rw-rw-   0        0        0     3381 2023-07-27 20:08:09.000000 FastXlsToCsv-1.2.1/FastXlsToCsv/XlConverter.py
+-rw-rw-rw-   0        0        0     1145 2023-07-24 20:34:19.000000 FastXlsToCsv-1.2.1/FastXlsToCsv/_XlsToCsvExceptions.py
+-rw-rw-rw-   0        0        0      184 2023-07-27 20:08:09.000000 FastXlsToCsv-1.2.1/FastXlsToCsv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:13:19.343741 FastXlsToCsv-1.2.1/FastXlsToCsv.egg-info/
+-rw-rw-rw-   0        0        0     1751 2023-07-27 20:13:19.000000 FastXlsToCsv-1.2.1/FastXlsToCsv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-07-27 20:13:19.000000 FastXlsToCsv-1.2.1/FastXlsToCsv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 20:13:19.000000 FastXlsToCsv-1.2.1/FastXlsToCsv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-27 20:13:19.000000 FastXlsToCsv-1.2.1/FastXlsToCsv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1105 2023-07-24 20:34:19.000000 FastXlsToCsv-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1751 2023-07-27 20:13:19.344746 FastXlsToCsv-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2023-07-24 21:06:59.000000 FastXlsToCsv-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 20:13:19.344746 FastXlsToCsv-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-07-27 20:11:58.000000 FastXlsToCsv-1.2.1/setup.py
```

### Comparing `FastXlsToCsv-1.0.0/FastXlsToCsv/XlsConverter.py` & `FastXlsToCsv-1.2.1/FastXlsToCsv/XlConverter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-## XlsConverter Module from FastXlsToCsv v.1.0.0
+## XlsConverter Module from FastXlsToCsv v.1.2.1
 #### Made by:
 William Norland, 2023, https://github.com/willayy
 ### Requirements:
 You have Excel installed on your computer, only tested with Microsoft Excel 2016.
 ### How to use?:
 Call methods convertXlFile() and convertXlDir() from this module to convert excel files to csv,
 ### Github
```

### Comparing `FastXlsToCsv-1.0.0/FastXlsToCsv/_XlsToCsvExceptions.py` & `FastXlsToCsv-1.2.1/FastXlsToCsv/_XlsToCsvExceptions.py`

 * *Files identical despite different names*

### Comparing `FastXlsToCsv-1.0.0/FastXlsToCsv.egg-info/PKG-INFO` & `FastXlsToCsv-1.2.1/FastXlsToCsv.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,62 @@
 Metadata-Version: 2.1
 Name: FastXlsToCsv
-Version: 1.0.0
+Version: 1.2.1
 Summary: A fast way to convert .xls and .xlsx to csv with vbs
 Home-page: https://github.com/willayy/FastXlsToCsv
 Author: William Norland
 Author-email: williamnorland@gmail.com
 License: MIT
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
-# FastXlsToCsv
-### Made by William Norland, 2023
-
-Fast way to convert large .xls/.xlsx files to CSV by saving them via a vbs and running the vbs with windows script host.
-
-## Dependencies
-* Excel (Only tested on excel 2016) and .
+FastXlsToCsv
+--------------
+*Made by William Norland, 2023*
+
+Fast way to convert large .xls/.xlsx files to CSV by saving them via a vbs running via windows script host.
+
+Dependencies
+=============
+* Excel (Only tested on excel 2016)
 * Windows operating system (Only tested on Windows 10).
 * Only tested on Python 3.11, should probably work on any python that has os and subprocess.
 * Windows script host (Exists on pretty much every windows ever).
 
-## Usage
-### Import
-![Screenshot (52)](https://github.com/willayy/FastXlsToCsv/assets/117913560/4ff08183-e8db-4c71-941e-e9864462c9f3)
-### Use
-```python
-input = r"c:\Users\someone\Desktop\ExcelFiles\excelFileThatWantsTobeCsv.xlsx"
-output =  r"c:\Users\someone\Desktop\FolderForExportedCsvs"
-XlsConverter.convertXlsFileToCsv(input, output)
-```
 
-## License
-Relased under the MIT License, check FastXlsToCsv/LICENSE for more information.
+Usage
+==========
+==========
+Install
+==========
+
+pip install FastXlsToCsv
+
+==========
+Import
+==========
+
+from FastXlToCsv import XlsConverter
+
+======
+Use
+======
 
+| inputFile: str = r"c:\\Users\\someone\\Desktop\\ExcelFiles\\excelFileThatWantsTobeCsv.xlsx"
+
+| inputDir: str = r"c:\Users\\someone\\Desktop\\ExcelFiles"
+
+| outputDir: str =  r"c:\\Users\\someone\\Desktop\\FolderForExportedCsvs"
+
+| XlsConverter.convertXlFileToCsv(inputFile, output)
+
+| XlsConverter.convertXlDir(inputDir, output)
+
+License
+=========
+Relased under the MIT License, check FastXlsToCsv/LICENSE for more information.
```

### Comparing `FastXlsToCsv-1.0.0/LICENSE` & `FastXlsToCsv-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FastXlsToCsv-1.0.0/PKG-INFO` & `FastXlsToCsv-1.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,62 @@
 Metadata-Version: 2.1
 Name: FastXlsToCsv
-Version: 1.0.0
+Version: 1.2.1
 Summary: A fast way to convert .xls and .xlsx to csv with vbs
 Home-page: https://github.com/willayy/FastXlsToCsv
 Author: William Norland
 Author-email: williamnorland@gmail.com
 License: MIT
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 
-# FastXlsToCsv
-### Made by William Norland, 2023
-
-Fast way to convert large .xls/.xlsx files to CSV by saving them via a vbs and running the vbs with windows script host.
-
-## Dependencies
-* Excel (Only tested on excel 2016) and .
+FastXlsToCsv
+--------------
+*Made by William Norland, 2023*
+
+Fast way to convert large .xls/.xlsx files to CSV by saving them via a vbs running via windows script host.
+
+Dependencies
+=============
+* Excel (Only tested on excel 2016)
 * Windows operating system (Only tested on Windows 10).
 * Only tested on Python 3.11, should probably work on any python that has os and subprocess.
 * Windows script host (Exists on pretty much every windows ever).
 
-## Usage
-### Import
-![Screenshot (52)](https://github.com/willayy/FastXlsToCsv/assets/117913560/4ff08183-e8db-4c71-941e-e9864462c9f3)
-### Use
-```python
-input = r"c:\Users\someone\Desktop\ExcelFiles\excelFileThatWantsTobeCsv.xlsx"
-output =  r"c:\Users\someone\Desktop\FolderForExportedCsvs"
-XlsConverter.convertXlsFileToCsv(input, output)
-```
 
-## License
-Relased under the MIT License, check FastXlsToCsv/LICENSE for more information.
+Usage
+==========
+==========
+Install
+==========
+
+pip install FastXlsToCsv
+
+==========
+Import
+==========
+
+from FastXlToCsv import XlsConverter
+
+======
+Use
+======
 
+| inputFile: str = r"c:\\Users\\someone\\Desktop\\ExcelFiles\\excelFileThatWantsTobeCsv.xlsx"
+
+| inputDir: str = r"c:\Users\\someone\\Desktop\\ExcelFiles"
+
+| outputDir: str =  r"c:\\Users\\someone\\Desktop\\FolderForExportedCsvs"
+
+| XlsConverter.convertXlFileToCsv(inputFile, output)
+
+| XlsConverter.convertXlDir(inputDir, output)
+
+License
+=========
+Relased under the MIT License, check FastXlsToCsv/LICENSE for more information.
```

### Comparing `FastXlsToCsv-1.0.0/README.md` & `FastXlsToCsv-1.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # FastXlsToCsv
 ### Made by William Norland, 2023
 
-Fast way to convert large .xls/.xlsx files to CSV by saving them via a vbs and running the vbs with windows script host.
+Fast way to convert large .xls/.xlsx files to CSV by saving them via a vbs running via windows script host.
 
 ## Dependencies
 * Excel (Only tested on excel 2016) and .
 * Windows operating system (Only tested on Windows 10).
 * Only tested on Python 3.11, should probably work on any python that has os and subprocess.
 * Windows script host (Exists on pretty much every windows ever).
 
 ## Usage
+### Install
+![Screenshot (1)](https://github.com/willayy/FastXlsToCsv/assets/117913560/f3d7e81d-346b-49d3-8992-e8c948f8162d)
 ### Import
 ![Screenshot (52)](https://github.com/willayy/FastXlsToCsv/assets/117913560/4ff08183-e8db-4c71-941e-e9864462c9f3)
 ### Use
 ```python
-input = r"c:\Users\someone\Desktop\ExcelFiles\excelFileThatWantsTobeCsv.xlsx"
-output =  r"c:\Users\someone\Desktop\FolderForExportedCsvs"
-XlsConverter.convertXlsFileToCsv(input, output)
+inputFile: str = r"c:\Users\someone\Desktop\ExcelFiles\excelFileThatWantsTobeCsv.xlsx"
+inputDir: str = r"c:\Users\someone\Desktop\ExcelFiles"
+outputDir: str =  r"c:\Users\someone\Desktop\FolderForExportedCsvs"
+XlsConverter.convertXlFileToCsv(inputFile, output)
+XlsConverter.convertXlDir(inputDir, output)
 ```
 
 ## License
 Relased under the MIT License, check FastXlsToCsv/LICENSE for more information.
```

