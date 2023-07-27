# Comparing `tmp/tableau_sql_parser-0.1.0.tar.gz` & `tmp/tableau_sql_parser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau_sql_parser-0.1.0.tar", max compression
+gzip compressed data, was "tableau_sql_parser-0.1.1.tar", max compression
```

## Comparing `tableau_sql_parser-0.1.0.tar` & `tableau_sql_parser-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-07-05 12:46:03.789910 tableau_sql_parser-0.1.0/LICENSE
--rw-r--r--   0        0        0      501 2023-07-27 10:00:00.379451 tableau_sql_parser-0.1.0/README.md
--rw-r--r--   0        0        0      644 2023-07-27 12:22:03.079404 tableau_sql_parser-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-18 08:05:42.168626 tableau_sql_parser-0.1.0/tableau_sql_parser/__init__.py
--rw-r--r--   0        0        0     1041 2023-07-27 10:04:22.156074 tableau_sql_parser-0.1.0/tableau_sql_parser/cli.py
--rw-r--r--   0        0        0     1348 2023-07-27 10:02:02.950615 tableau_sql_parser-0.1.0/tableau_sql_parser/output_formatting.py
--rw-r--r--   0        0        0     2818 2023-07-27 10:02:03.026929 tableau_sql_parser-0.1.0/tableau_sql_parser/recursive_search.py
--rw-r--r--   0        0        0     3329 2023-07-27 10:04:22.147731 tableau_sql_parser-0.1.0/tableau_sql_parser/tableau_workbook.py
--rw-r--r--   0        0        0     1816 2023-07-27 10:06:39.723014 tableau_sql_parser-0.1.0/tableau_sql_parser/utils.py
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 tableau_sql_parser-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-05 12:46:03.789910 tableau_sql_parser-0.1.1/LICENSE
+-rw-r--r--   0        0        0      393 2023-07-27 12:34:24.594246 tableau_sql_parser-0.1.1/README.md
+-rw-r--r--   0        0        0      644 2023-07-27 16:12:12.353914 tableau_sql_parser-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-18 08:05:42.168626 tableau_sql_parser-0.1.1/tableau_sql_parser/__init__.py
+-rw-r--r--   0        0        0     1060 2023-07-27 12:36:47.049148 tableau_sql_parser-0.1.1/tableau_sql_parser/cli.py
+-rw-r--r--   0        0        0     1348 2023-07-27 10:02:02.950615 tableau_sql_parser-0.1.1/tableau_sql_parser/output_formatting.py
+-rw-r--r--   0        0        0     2818 2023-07-27 10:02:03.026929 tableau_sql_parser-0.1.1/tableau_sql_parser/recursive_search.py
+-rw-r--r--   0        0        0     3329 2023-07-27 10:04:22.147731 tableau_sql_parser-0.1.1/tableau_sql_parser/tableau_workbook.py
+-rw-r--r--   0        0        0     1816 2023-07-27 10:06:39.723014 tableau_sql_parser-0.1.1/tableau_sql_parser/utils.py
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 tableau_sql_parser-0.1.1/PKG-INFO
```

### Comparing `tableau_sql_parser-0.1.0/LICENSE` & `tableau_sql_parser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau_sql_parser-0.1.0/pyproject.toml` & `tableau_sql_parser-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tableau-sql-parser"
-version = "0.1.0"
+version = "0.1.1"
 description = "A tool for parsing Tableau custom SQL queries and extracting useful information"
 authors = ["florian-drouet <50357200+florian-drouet@users.noreply.github.com>"]
 license = "LICENSE"
 readme = "README.md"
 packages = [{include = "tableau_sql_parser"}]
 
 [tool.poetry.scripts]
```

### Comparing `tableau_sql_parser-0.1.0/tableau_sql_parser/cli.py` & `tableau_sql_parser-0.1.1/tableau_sql_parser/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import click
-from utils import generate_report
 
 from tableau_sql_parser.tableau_workbook import TableauWorkbook
+from tableau_sql_parser.utils import generate_report
 
 
 @click.command()
 @click.option(
     "-f",
     "--file-to-parse",
     required=True,
```

### Comparing `tableau_sql_parser-0.1.0/tableau_sql_parser/output_formatting.py` & `tableau_sql_parser-0.1.1/tableau_sql_parser/output_formatting.py`

 * *Files identical despite different names*

### Comparing `tableau_sql_parser-0.1.0/tableau_sql_parser/recursive_search.py` & `tableau_sql_parser-0.1.1/tableau_sql_parser/recursive_search.py`

 * *Files identical despite different names*

### Comparing `tableau_sql_parser-0.1.0/tableau_sql_parser/tableau_workbook.py` & `tableau_sql_parser-0.1.1/tableau_sql_parser/tableau_workbook.py`

 * *Files identical despite different names*

### Comparing `tableau_sql_parser-0.1.0/tableau_sql_parser/utils.py` & `tableau_sql_parser-0.1.1/tableau_sql_parser/utils.py`

 * *Files identical despite different names*

