# Comparing `tmp/exergenics-etl-1.5.3.tar.gz` & `tmp/exergenics-etl-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.5.3.tar", last modified: Thu Jun 29 23:21:18 2023, max compression
+gzip compressed data, was "exergenics-etl-1.6.0.tar", last modified: Thu Jul 27 00:19:47 2023, max compression
```

## Comparing `exergenics-etl-1.5.3.tar` & `exergenics-etl-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:18.488448 exergenics-etl-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 23:21:18.488448 exergenics-etl-1.5.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:18.484449 exergenics-etl-1.5.3/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:18.484449 exergenics-etl-1.5.3/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:18.488448 exergenics-etl-1.5.3/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57393 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/src/exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:18.488448 exergenics-etl-1.5.3/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    42150 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/test/test_exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-29 23:21:14.000000 exergenics-etl-1.5.3/app/exergenics_etl/test/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:21:18.488448 exergenics-etl-1.5.3/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-29 23:21:18.000000 exergenics-etl-1.5.3/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-29 23:21:18.000000 exergenics-etl-1.5.3/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:21:18.000000 exergenics-etl-1.5.3/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-29 23:21:18.000000 exergenics-etl-1.5.3/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 23:21:18.000000 exergenics-etl-1.5.3/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 23:21:18.488448 exergenics-etl-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-29 23:21:17.000000 exergenics-etl-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/src/exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43240 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/test/test_exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-27 00:19:44.000000 exergenics-etl-1.6.0/app/exergenics_etl/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-27 00:19:47.000000 exergenics-etl-1.6.0/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-27 00:19:47.000000 exergenics-etl-1.6.0/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:19:47.000000 exergenics-etl-1.6.0/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-27 00:19:47.000000 exergenics-etl-1.6.0/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 00:19:47.000000 exergenics-etl-1.6.0/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:19:47.774743 exergenics-etl-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-27 00:19:46.000000 exergenics-etl-1.6.0/setup.py
```

### Comparing `exergenics-etl-1.5.3/LICENSE` & `exergenics-etl-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.5.3/app/exergenics_etl/__init__.py` & `exergenics-etl-1.6.0/app/exergenics_etl/__init__.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.5.3/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.6.0/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 1% similar despite different names*

```diff
@@ -955,14 +955,33 @@
         else:
             errorMessage = f"Cannot find the position of year in timestamps."
             self.logger.error(errorMessage)
             raise EtlError(errorMessage)
 
         return
 
+    def _find_month_wording(self, datestring: str) -> list:
+        """Find any month name or abbreviation in date string 
+        and return them as a list of names.
+
+        Args:
+            datestring (str): Input datetime string to identify month wording.
+
+        Returns:
+            list: Identified list of month wording (could be empty).
+        """
+        month_names = r"January|February|March|April|May|June|July|August|September|October|November|December"
+        month_abbrs = r"Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec"
+
+        pattern = rf"\b(?:{month_names}|{month_abbrs})\b"
+        matches = re.findall(pattern, datestring, re.IGNORECASE)
+
+        return matches
+
+
     def _find_day_position(self, dtSeries: pd.Series) -> int:
         """Find 50 timestamps with day > 12 as test cases and
         find the position of day.
 
         Args:
             dtSeries (pd.Series): Panda Series containing timestamp strings
 
@@ -984,16 +1003,16 @@
 
             # PARSE the selected timestamp with a magic datetime parser
             # dtObjectTest = parser.parse(dtTest)
             dtObjectTest = dateparser.parse(str(dtTest))
 
             day = dtObjectTest.day
 
-            # Don't use timestamps with day <= 12
-            if day <= 12:
+            # Don't use timestamps with day <= 12 and no month wording found
+            if day <= 12 and not self._find_month_wording(dtTest):
                 continue
             else:
                 day = str(day)
 
             # SPLIT the corresponding datetime string into chunks of strings by delimiters into a list
             dateParts = self.delim.split(str(dtTest))
```

### Comparing `exergenics-etl-1.5.3/app/exergenics_etl/src/logger.py` & `exergenics-etl-1.6.0/app/exergenics_etl/src/logger.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.5.3/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.6.0/app/exergenics_etl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.5.3/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.6.0/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files 2% similar despite different names*

```diff
@@ -502,14 +502,22 @@
         dtSeries = pd.read_csv(
             f"{TEST_DATA_DIR}/timestamps_ampm.csv", header=None)[0]
         my_dtFinalFormat = '%d/%m/%Y %I:%M %p'
         my_dtObjects = pd.to_datetime(dtSeries, format=my_dtFinalFormat)
         return dtSeries, my_dtObjects
 
     @pytest.fixture(scope='class')
+    def my_test_case_month_name_parsing(self):
+        dtSeries = pd.read_csv(
+            f"{TEST_DATA_DIR}/timestamps_monthName.csv", header=None)[0]
+        my_dtFinalFormat = '%B %d, %Y %I:%M:%S %p'
+        my_dtObjects = pd.to_datetime(dtSeries, format=my_dtFinalFormat)
+        return dtSeries, my_dtObjects
+
+    @pytest.fixture(scope='class')
     def my_test_case_time_zone_parsing(self):
         dtSeries = pd.read_csv(
             f"{TEST_DATA_DIR}/timestamps_timeZones_1.csv", header=None)[0]  # TODO
         expected_output = pd.read_csv(
             f"{TEST_DATA_DIR}/timestamps_timeZones_expectedOutput_1.csv", header=None)[0]
         return dtSeries, expected_output
 
@@ -606,14 +614,21 @@
     def test_parse_for_ampm(self, my_datetimeParser, my_test_case_ampm_parsing, my_non_unix_timestamp_flag):
         dtSeries, my_dtObjects = my_test_case_ampm_parsing
         assert my_datetimeParser.dtFinalFormat is None
         dtObjects = my_datetimeParser.parse(dtSeries, my_non_unix_timestamp_flag)
         assert my_datetimeParser.dtFinalFormat is not None
         assert dtObjects.equals(my_dtObjects)
 
+    def test_parse_for_month_name(self, my_datetimeParser, my_test_case_month_name_parsing, my_non_unix_timestamp_flag):
+        dtSeries, my_dtObjects = my_test_case_month_name_parsing
+        assert my_datetimeParser.dtFinalFormat is None
+        dtObjects = my_datetimeParser.parse(dtSeries, my_non_unix_timestamp_flag)
+        assert my_datetimeParser.dtFinalFormat is not None
+        assert dtObjects.equals(my_dtObjects)
+
     def test_checkTimeZone_for_timestamps_with_time_zones(self, my_datetimeParser, my_test_case_time_zone_parsing, my_non_unix_timestamp_flag):
         dtSeries, expected_output = my_test_case_time_zone_parsing
         dtObjects = my_datetimeParser.parse(dtSeries, my_non_unix_timestamp_flag)
         assert my_datetimeParser.containsTimeZone
 
     def test_find_day_position_when_timestamps_inadequate(self, my_datetimeParser):
         myTestDtSeries = pd.read_csv(
@@ -626,14 +641,21 @@
         myTestDtSeries = pd.read_csv(
             f"{TEST_DATA_DIR}/timestamps_findDayPosition_2.csv", header=None)[0]
         positionDay = my_datetimeParser._find_day_position(
             myTestDtSeries)  # TODO
         my_expected_day_position_2 = 2
         assert positionDay == my_expected_day_position_2
 
+    def test_find_day_position_when_month_name_exist(self, my_datetimeParser):
+        myTestDtSeries = pd.read_csv(
+            f"{TEST_DATA_DIR}/timestamps_monthName.csv", header=None)[0]
+        positionDay = my_datetimeParser._find_day_position(
+            myTestDtSeries)
+        assert positionDay == 2
+
     def test_removeTimeZone_for_timestamps_with_time_zones(self, my_datetimeParser, my_test_case_for_removing_time_zone_from_timestamps_with_time_zones):
         myDatetimeParts, myFormatCodeList, expectedFormatCodeList = my_test_case_for_removing_time_zone_from_timestamps_with_time_zones
         newFormatCodeList = my_datetimeParser._check_and_remove_time_zone(
             myDatetimeParts, myFormatCodeList)
         assert newFormatCodeList == expectedFormatCodeList
 
     def test_removeTimeZone_for_timestamps_without_time_zones(self, my_datetimeParser, my_test_case_for_removing_time_zone_from_timestamps_without_time_zones):
```

### Comparing `exergenics-etl-1.5.3/app/exergenics_etl.egg-info/SOURCES.txt` & `exergenics-etl-1.6.0/app/exergenics_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.5.3/setup.py` & `exergenics-etl-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.5.3",
+    version="v1.6.0",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```

