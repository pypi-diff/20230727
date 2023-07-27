# Comparing `tmp/FM15_bfr2geojson-0.0.3.tar.gz` & `tmp/FM15_bfr2geojson-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FM15_bfr2geojson-0.0.3.tar", last modified: Wed Jul 26 22:48:35 2023, max compression
+gzip compressed data, was "FM15_bfr2geojson-0.0.4.tar", last modified: Thu Jul 27 17:59:27 2023, max compression
```

## Comparing `FM15_bfr2geojson-0.0.3.tar` & `FM15_bfr2geojson-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-26 22:48:35.353071 FM15_bfr2geojson-0.0.3/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      523 2023-07-26 22:48:35.352071 FM15_bfr2geojson-0.0.3/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       18 2023-07-25 16:39:55.000000 FM15_bfr2geojson-0.0.3/README.md
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      657 2023-07-26 22:48:05.000000 FM15_bfr2geojson-0.0.3/pyproject.toml
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-07-26 22:48:35.353071 FM15_bfr2geojson-0.0.3/setup.cfg
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-26 22:48:35.351071 FM15_bfr2geojson-0.0.3/src/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-26 22:48:35.351071 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    29382 2023-07-26 22:47:54.000000 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson/__init__.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-26 22:48:35.352071 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson.egg-info/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      523 2023-07-26 22:48:35.000000 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson.egg-info/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      233 2023-07-26 22:48:35.000000 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson.egg-info/SOURCES.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-07-26 22:48:35.000000 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson.egg-info/dependency_links.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       17 2023-07-26 22:48:35.000000 FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson.egg-info/top_level.txt
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-27 17:59:27.904609 FM15_bfr2geojson-0.0.4/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      523 2023-07-27 17:59:27.903609 FM15_bfr2geojson-0.0.4/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       18 2023-07-25 16:39:55.000000 FM15_bfr2geojson-0.0.4/README.md
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      657 2023-07-27 17:58:16.000000 FM15_bfr2geojson-0.0.4/pyproject.toml
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-07-27 17:59:27.904609 FM15_bfr2geojson-0.0.4/setup.cfg
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-27 17:59:27.902609 FM15_bfr2geojson-0.0.4/src/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-27 17:59:27.902609 FM15_bfr2geojson-0.0.4/src/FM15_bfr2geojson/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    29576 2023-07-27 17:57:59.000000 FM15_bfr2geojson-0.0.4/src/FM15_bfr2geojson/__init__.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-27 17:59:27.903609 FM15_bfr2geojson-0.0.4/src/FM15_bfr2geojson.egg-info/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      523 2023-07-27 17:59:27.000000 FM15_bfr2geojson-0.0.4/src/FM15_bfr2geojson.egg-info/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      233 2023-07-27 17:59:27.000000 FM15_bfr2geojson-0.0.4/src/FM15_bfr2geojson.egg-info/SOURCES.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-07-27 17:59:27.000000 FM15_bfr2geojson-0.0.4/src/FM15_bfr2geojson.egg-info/dependency_links.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       17 2023-07-27 17:59:27.000000 FM15_bfr2geojson-0.0.4/src/FM15_bfr2geojson.egg-info/top_level.txt
```

### Comparing `FM15_bfr2geojson-0.0.3/PKG-INFO` & `FM15_bfr2geojson-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FM15_bfr2geojson
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for converting FM15(METAR) bufr encoded messages to geojson
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `FM15_bfr2geojson-0.0.3/pyproject.toml` & `FM15_bfr2geojson-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FM15_bfr2geojson"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Alexander Thompson", email="alexander.thompson@noaa.gov" },
 ]
 description = "Package for converting FM15(METAR) bufr encoded messages to geojson"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson/__init__.py` & `FM15_bfr2geojson-0.0.4/src/FM15_bfr2geojson/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,23 +249,26 @@
         if "latitude" not in self.qualifiers["05"]:
             LOGGER.warning("Invalid location in BUFR message, no latitude")
             LOGGER.warning(self.qualifiers["05"])
             LOGGER.warning("latitude set to None")
             latitude = None
         else:
             latitude = deepcopy(self.qualifiers["05"]["latitude"])
+            latitude = round(latitude["value"],
+                             latitude["attributes"]["scale"])
 
         # now get longitude
         if "longitude" not in self.qualifiers["06"]:
             LOGGER.warning("Invalid location in BUFR message, no longitude")
             LOGGER.warning(self.qualifiers["06"])
             LOGGER.warning("longitude set to None")
             longitude = None
         else:
             longitude = self.qualifiers["06"]["longitude"]
+            longitude = round(longitude["value"], longitude["attributes"]["scale"])
 
         # now station elevation
         if "height_of_station" in self.qualifiers["07"]:  # noqa
             elevation = self.qualifiers["07"]["height_of_station"]  # noqa
             elevation = round(elevation["value"], elevation["attributes"]["scale"])  # noqa
         else:
             elevation = None
```

### Comparing `FM15_bfr2geojson-0.0.3/src/FM15_bfr2geojson.egg-info/PKG-INFO` & `FM15_bfr2geojson-0.0.4/src/FM15_bfr2geojson.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FM15-bfr2geojson
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for converting FM15(METAR) bufr encoded messages to geojson
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

