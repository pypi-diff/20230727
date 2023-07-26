# Comparing `tmp/FM15_bfr2geojson-0.0.2.tar.gz` & `tmp/FM15_bfr2geojson-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FM15_bfr2geojson-0.0.2.tar", last modified: Tue Jul 25 21:52:59 2023, max compression
+gzip compressed data, was "FM15_bfr2geojson-0.0.3.tar", last modified: Wed Jul 26 22:48:35 2023, max compression
```

## Comparing `FM15_bfr2geojson-0.0.2.tar` & `FM15_bfr2geojson-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 21:52:59.230810 FM15_bfr2geojson-0.0.2/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      523 2023-07-25 21:52:59.229810 FM15_bfr2geojson-0.0.2/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       18 2023-07-25 16:39:55.000000 FM15_bfr2geojson-0.0.2/README.md
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      657 2023-07-25 21:51:51.000000 FM15_bfr2geojson-0.0.2/pyproject.toml
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-07-25 21:52:59.230810 FM15_bfr2geojson-0.0.2/setup.cfg
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 21:52:59.228809 FM15_bfr2geojson-0.0.2/src/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 21:52:59.228809 FM15_bfr2geojson-0.0.2/src/FM15_bfr2geojson/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    29367 2023-07-25 17:34:01.000000 FM15_bfr2geojson-0.0.2/src/FM15_bfr2geojson/__init__.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-25 21:52:59.229810 FM15_bfr2geojson-0.0.2/src/FM15_bfr2geojson.egg-info/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      523 2023-07-25 21:52:59.000000 FM15_bfr2geojson-0.0.2/src/FM15_bfr2geojson.egg-info/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      233 2023-07-25 21:52:59.000000 FM15_bfr2geojson-0.0.2/src/FM15_bfr2geojson.egg-info/SOURCES.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-07-25 21:52:59.000000 FM15_bfr2geojson-0.0.2/src/FM15_bfr2geojson.egg-info/dependency_links.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       17 2023-07-25 21:52:59.000000 FM15_bfr2geojson-0.0.2/src/FM15_bfr2geojson.egg-info/top_level.txt
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-26 22:48:35.353071 FM15_bfr2geojson-0.0.3/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      523 2023-07-26 22:48:35.352071 FM15_bfr2geojson-0.0.3/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       18 2023-07-25 16:39:55.000000 FM15_bfr2geojson-0.0.3/README.md
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      657 2023-07-26 22:48:05.000000 FM15_bfr2geojson-0.0.3/pyproject.toml
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-07-26 22:48:35.353071 FM15_bfr2geojson-0.0.3/setup.cfg
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-26 22:48:35.351071 FM15_bfr2geojson-0.0.3/src/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-26 22:48:35.351071 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    29382 2023-07-26 22:47:54.000000 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson/__init__.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-26 22:48:35.352071 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson.egg-info/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      523 2023-07-26 22:48:35.000000 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson.egg-info/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      233 2023-07-26 22:48:35.000000 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson.egg-info/SOURCES.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-07-26 22:48:35.000000 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson.egg-info/dependency_links.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       17 2023-07-26 22:48:35.000000 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson.egg-info/top_level.txt
```

### Comparing `FM15_bfr2geojson-0.0.2/PKG-INFO` & `FM15_bfr2geojson-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FM15_bfr2geojson
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for converting FM15(METAR) bufr encoded messages to geojson
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `FM15_bfr2geojson-0.0.2/pyproject.toml` & `FM15_bfr2geojson-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FM15_bfr2geojson"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Alexander Thompson", email="alexander.thompson@noaa.gov" },
 ]
 description = "Package for converting FM15(METAR) bufr encoded messages to geojson"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `FM15_bfr2geojson-0.0.2/src/FM15_bfr2geojson/__init__.py` & `FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
         """
 
         # see https://library.wmo.int/doc_num.php?explnum_id=11021
         # page 19 for allocation of WSI if not set
         # check to see what identification we have
             
         if "icao_location_indicator" in self.qualifiers["01"]:
-            icao = self.qualifiers["01"]["icao_location_indicator"]
+            icao = self.qualifiers["01"]["icao_location_indicator"]["description"]
             return {
                 "icao": icao,
                 "type": "icao_location_identifier"
             }
 
         # flag if we do not have WSI
         LOGGER.debug(self.qualifiers["01"])
```

### Comparing `FM15_bfr2geojson-0.0.2/src/FM15_bfr2geojson.egg-info/PKG-INFO` & `FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FM15-bfr2geojson
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for converting FM15(METAR) bufr encoded messages to geojson
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

