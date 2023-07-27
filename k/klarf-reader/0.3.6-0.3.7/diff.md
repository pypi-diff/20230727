# Comparing `tmp/klarf-reader-0.3.6.tar.gz` & `tmp/klarf-reader-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klarf-reader-0.3.6.tar", last modified: Wed Jul 26 14:48:59 2023, max compression
+gzip compressed data, was "klarf-reader-0.3.7.tar", last modified: Thu Jul 27 09:13:30 2023, max compression
```

## Comparing `klarf-reader-0.3.6.tar` & `klarf-reader-0.3.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 14:48:59.013451 klarf-reader-0.3.6/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.3.6/LICENSE.txt
--rw-rw-rw-   0        0        0      569 2023-07-26 14:48:59.010454 klarf-reader-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 14:48:58.965584 klarf-reader-0.3.6/klarf_reader/
--rw-rw-rw-   0        0        0     1060 2023-06-27 07:08:50.000000 klarf-reader-0.3.6/klarf_reader/klarf.py
-drwxrwxrwx   0        0        0        0 2023-07-26 14:48:58.992879 klarf-reader-0.3.6/klarf_reader/models/
--rw-rw-rw-   0        0        0     2472 2023-06-27 08:18:10.000000 klarf-reader-0.3.6/klarf_reader/models/klarf_content.py
-drwxrwxrwx   0        0        0        0 2023-07-26 14:48:58.997879 klarf-reader-0.3.6/klarf_reader/readers/
--rw-rw-rw-   0        0        0    14081 2023-07-26 14:47:02.000000 klarf-reader-0.3.6/klarf_reader/readers/klarf_file_reader.py
-drwxrwxrwx   0        0        0        0 2023-07-26 14:48:59.001597 klarf-reader-0.3.6/klarf_reader/utils/
--rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.3.6/klarf_reader/utils/klarf_convert.py
-drwxrwxrwx   0        0        0        0 2023-07-26 14:48:58.988159 klarf-reader-0.3.6/klarf_reader.egg-info/
--rw-rw-rw-   0        0        0      569 2023-07-26 14:48:58.000000 klarf-reader-0.3.6/klarf_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-07-26 14:48:58.000000 klarf-reader-0.3.6/klarf_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 14:48:58.000000 klarf-reader-0.3.6/klarf_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-26 14:48:58.000000 klarf-reader-0.3.6/klarf_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-26 14:48:58.000000 klarf-reader-0.3.6/klarf_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 14:48:59.014217 klarf-reader-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-07-26 14:47:36.000000 klarf-reader-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 14:48:59.005601 klarf-reader-0.3.6/tests/
--rw-rw-rw-   0        0        0     4195 2023-06-27 07:43:51.000000 klarf-reader-0.3.6/tests/test_klarf.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.987871 klarf-reader-0.3.7/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      569 2023-07-27 09:13:30.986871 klarf-reader-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.949345 klarf-reader-0.3.7/klarf_reader/
+-rw-rw-rw-   0        0        0     1218 2023-07-27 09:09:59.000000 klarf-reader-0.3.7/klarf_reader/klarf.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.970981 klarf-reader-0.3.7/klarf_reader/models/
+-rw-rw-rw-   0        0        0     2559 2023-07-27 09:12:12.000000 klarf-reader-0.3.7/klarf_reader/models/klarf_content.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.975308 klarf-reader-0.3.7/klarf_reader/readers/
+-rw-rw-rw-   0        0        0    14231 2023-07-27 09:11:10.000000 klarf-reader-0.3.7/klarf_reader/readers/klarf_file_reader.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.980366 klarf-reader-0.3.7/klarf_reader/utils/
+-rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.3.7/klarf_reader/utils/klarf_convert.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.968969 klarf-reader-0.3.7/klarf_reader.egg-info/
+-rw-rw-rw-   0        0        0      569 2023-07-27 09:13:30.000000 klarf-reader-0.3.7/klarf_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-07-27 09:13:30.000000 klarf-reader-0.3.7/klarf_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 09:13:30.000000 klarf-reader-0.3.7/klarf_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-27 09:13:30.000000 klarf-reader-0.3.7/klarf_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-27 09:13:30.000000 klarf-reader-0.3.7/klarf_reader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 09:13:30.988445 klarf-reader-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-07-27 09:12:25.000000 klarf-reader-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:13:30.983855 klarf-reader-0.3.7/tests/
+-rw-rw-rw-   0        0        0     4195 2023-06-27 07:43:51.000000 klarf-reader-0.3.7/tests/test_klarf.py
```

### Comparing `klarf-reader-0.3.6/LICENSE.txt` & `klarf-reader-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.6/PKG-INFO` & `klarf-reader-0.3.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.3.6
+Version: 0.3.7
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.6.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.7.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.3.6/README.md` & `klarf-reader-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.6/klarf_reader/klarf.py` & `klarf-reader-0.3.7/klarf_reader/klarf.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,28 +8,32 @@
 
 class Klarf:
     @staticmethod
     def load_from_file(
         filepath: Path,
         custom_columns_wafer: List[str] = None,
         custom_columns_defect: List[str] = None,
+        parse_summary: bool = True,
     ) -> KlarfContent:
         return Klarf.load_from_file_with_raw_content(
             filepath=filepath,
             custom_columns_wafer=custom_columns_wafer,
             custom_columns_defect=custom_columns_defect,
+            parse_summary=parse_summary,
         )[0]
 
     @staticmethod
     def load_from_file_with_raw_content(
         filepath: Path,
         custom_columns_wafer: List[str] = None,
         custom_columns_defect: List[str] = None,
+        parse_summary: bool = True,
     ) -> Tuple[KlarfContent, List[str]]:
         return klarf_file_reader.readKlarf(
             klarf=filepath,
             custom_columns_wafer=custom_columns_wafer,
             custom_columns_defect=custom_columns_defect,
+            parse_summary=parse_summary,
         )
 
     def __repr__(self):
         print(self.__dict__)
```

### Comparing `klarf-reader-0.3.6/klarf_reader/models/klarf_content.py` & `klarf-reader-0.3.7/klarf_reader/models/klarf_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,19 @@
     number_of_defects: int = None
     number_of_dies: int = None
     number_of_def_dies: int = None
 
     percent_of_def_die: float = None
 
     def __post_init__(self):
-        self.percent_of_def_die = float(self.number_of_def_dies / self.number_of_dies)
+        self.percent_of_def_die = (
+            float(self.number_of_def_dies / self.number_of_dies)
+            if self.number_of_dies != 0
+            else 0
+        )
 
 
 @dataclass
 class Test:
     id: int
     area: float
```

### Comparing `klarf-reader-0.3.6/klarf_reader/readers/klarf_file_reader.py` & `klarf-reader-0.3.7/klarf_reader/readers/klarf_file_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 ACCEPTED_KLARF_VERSIONS = [1.2]
 
 
 def readKlarf(
     klarf: Path,
     custom_columns_wafer: List[str] = None,
     custom_columns_defect: List[str] = None,
+    parse_summary: bool = True,
 ) -> Tuple[KlarfContent, List[str]]:
     """this function open, read and parse a klarf file
 
     Args:
         klarf (Path): the path of the klarf file
 
     Returns:
@@ -42,21 +43,23 @@
     with open(klarf, "r") as f:
         raw_content = f.readlines()
 
     return convert_raw_to_klarf_content(
         raw_content=raw_content,
         custom_columns_wafer=custom_columns_wafer,
         custom_columns_defect=custom_columns_defect,
+        parse_summary=parse_summary,
     )
 
 
 def convert_raw_to_klarf_content(
     raw_content: List[str],
     custom_columns_wafer: List[str] = None,
     custom_columns_defect: List[str] = None,
+    parse_summary: bool = True,
 ) -> Tuple[KlarfContent, List[str]]:
 
     RAW_DEFECT_COLUMNS = [
         "DEFECTID",
         "XREL",
         "YREL",
         "XINDEX",
@@ -308,16 +311,18 @@
                         tests=tests.copy(),
                         custom_attribute=custom_columns_wafer_dict,
                     )
                 )
 
                 tests.clear()
 
-        if line.lstrip().lower().startswith("summarylist") and not (
-            line.rstrip().endswith(";")
+        if (
+            parse_summary
+            and line.lstrip().lower().startswith("summarylist")
+            and not (line.rstrip().endswith(";"))
         ):
             next_line_has_numb = True
             continue
 
         if next_line_has_numb and line.startswith(" "):
             next_line_has_numb = False
             linewithoutSpace = re.sub("\s+", " ", line).strip()
```

### Comparing `klarf-reader-0.3.6/klarf_reader/utils/klarf_convert.py` & `klarf-reader-0.3.7/klarf_reader/utils/klarf_convert.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.6/klarf_reader.egg-info/PKG-INFO` & `klarf-reader-0.3.7/klarf_reader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.3.6
+Version: 0.3.7
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.6.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.7.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.3.6/setup.py` & `klarf-reader-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.6"
+version = "0.3.7"
 
 setup(
     name="klarf-reader",
     version=version,
     packages=[
         "klarf_reader",
         "klarf_reader.models",
```

### Comparing `klarf-reader-0.3.6/tests/test_klarf.py` & `klarf-reader-0.3.7/tests/test_klarf.py`

 * *Files identical despite different names*

