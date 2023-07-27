# Comparing `tmp/rcs_common-0.2.4.tar.gz` & `tmp/rcs_common-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcs_common-0.2.4.tar", last modified: Thu Jul 27 11:55:26 2023, max compression
+gzip compressed data, was "rcs_common-0.2.5.tar", last modified: Thu Jul 27 12:04:34 2023, max compression
```

## Comparing `rcs_common-0.2.4.tar` & `rcs_common-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:55:26.537927 rcs_common-0.2.4/
--rw-rw-rw-   0        0        0      201 2023-07-27 11:55:26.536519 rcs_common-0.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 11:55:26.525555 rcs_common-0.2.4/common/
--rw-rw-rw-   0        0        0      513 2023-07-23 08:33:13.000000 rcs_common-0.2.4/common/MCPutil.py
--rw-rw-rw-   0        0        0    13871 2023-07-23 08:22:40.000000 rcs_common-0.2.4/common/TGtypes.py
--rw-rw-rw-   0        0        0        0 2023-07-23 08:22:40.000000 rcs_common-0.2.4/common/__init__.py
--rw-rw-rw-   0        0        0    14213 2023-07-23 08:22:52.000000 rcs_common-0.2.4/common/azutils.py
--rw-rw-rw-   0        0        0     9249 2023-07-23 08:31:10.000000 rcs_common-0.2.4/common/common_def.py
--rw-rw-rw-   0        0        0    18144 2023-07-25 11:34:31.000000 rcs_common-0.2.4/common/common_types.py
--rw-rw-rw-   0        0        0     2665 2023-07-23 08:22:40.000000 rcs_common-0.2.4/common/filter_utils.py
--rw-rw-rw-   0        0        0     3330 2023-07-23 08:22:40.000000 rcs_common-0.2.4/common/geoutils.py
--rw-rw-rw-   0        0        0      610 2023-07-23 08:22:40.000000 rcs_common-0.2.4/common/getip.py
--rw-rw-rw-   0        0        0    12411 2023-07-23 08:32:02.000000 rcs_common-0.2.4/common/mcpop.py
--rw-rw-rw-   0        0        0    22792 2023-07-23 08:33:57.000000 rcs_common-0.2.4/common/mcpre.py
--rw-rw-rw-   0        0        0    56061 2023-07-25 08:52:49.000000 rcs_common-0.2.4/common/v2_1def.py
--rw-rw-rw-   0        0        0    20146 2023-07-25 13:18:56.000000 rcs_common-0.2.4/common/volume_4D_Converter.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:55:26.535516 rcs_common-0.2.4/rcs_common.egg-info/
--rw-rw-rw-   0        0        0      201 2023-07-27 11:55:26.000000 rcs_common-0.2.4/rcs_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-07-27 11:55:26.000000 rcs_common-0.2.4/rcs_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       30 2023-07-27 11:55:26.000000 rcs_common-0.2.4/rcs_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      249 2023-07-27 11:55:26.000000 rcs_common-0.2.4/rcs_common.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 11:55:26.000000 rcs_common-0.2.4/rcs_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 11:55:26.538947 rcs_common-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-07-27 11:55:08.000000 rcs_common-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:04:34.297902 rcs_common-0.2.5/
+-rw-rw-rw-   0        0        0      201 2023-07-27 12:04:34.296890 rcs_common-0.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 12:04:34.285821 rcs_common-0.2.5/common/
+-rw-rw-rw-   0        0        0      513 2023-07-23 08:33:13.000000 rcs_common-0.2.5/common/MCPutil.py
+-rw-rw-rw-   0        0        0    13871 2023-07-23 08:22:40.000000 rcs_common-0.2.5/common/TGtypes.py
+-rw-rw-rw-   0        0        0        0 2023-07-23 08:22:40.000000 rcs_common-0.2.5/common/__init__.py
+-rw-rw-rw-   0        0        0    14213 2023-07-23 08:22:52.000000 rcs_common-0.2.5/common/azutils.py
+-rw-rw-rw-   0        0        0     9249 2023-07-23 08:31:10.000000 rcs_common-0.2.5/common/common_def.py
+-rw-rw-rw-   0        0        0    18144 2023-07-25 11:34:31.000000 rcs_common-0.2.5/common/common_types.py
+-rw-rw-rw-   0        0        0     2665 2023-07-23 08:22:40.000000 rcs_common-0.2.5/common/filter_utils.py
+-rw-rw-rw-   0        0        0     3330 2023-07-23 08:22:40.000000 rcs_common-0.2.5/common/geoutils.py
+-rw-rw-rw-   0        0        0      610 2023-07-23 08:22:40.000000 rcs_common-0.2.5/common/getip.py
+-rw-rw-rw-   0        0        0    12411 2023-07-23 08:32:02.000000 rcs_common-0.2.5/common/mcpop.py
+-rw-rw-rw-   0        0        0    22792 2023-07-23 08:33:57.000000 rcs_common-0.2.5/common/mcpre.py
+-rw-rw-rw-   0        0        0    56061 2023-07-25 08:52:49.000000 rcs_common-0.2.5/common/v2_1def.py
+-rw-rw-rw-   0        0        0    20146 2023-07-25 13:18:56.000000 rcs_common-0.2.5/common/volume_4D_Converter.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:04:34.294872 rcs_common-0.2.5/rcs_common.egg-info/
+-rw-rw-rw-   0        0        0      201 2023-07-27 12:04:34.000000 rcs_common-0.2.5/rcs_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-07-27 12:04:34.000000 rcs_common-0.2.5/rcs_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      100 2023-07-27 12:04:34.000000 rcs_common-0.2.5/rcs_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      249 2023-07-27 12:04:34.000000 rcs_common-0.2.5/rcs_common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 12:04:34.000000 rcs_common-0.2.5/rcs_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 12:04:34.297902 rcs_common-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      870 2023-07-27 12:04:28.000000 rcs_common-0.2.5/setup.py
```

### Comparing `rcs_common-0.2.4/common/MCPutil.py` & `rcs_common-0.2.5/common/MCPutil.py`

 * *Files identical despite different names*

### Comparing `rcs_common-0.2.4/common/TGtypes.py` & `rcs_common-0.2.5/common/TGtypes.py`

 * *Files identical despite different names*

### Comparing `rcs_common-0.2.4/common/azutils.py` & `rcs_common-0.2.5/common/azutils.py`

 * *Files identical despite different names*

### Comparing `rcs_common-0.2.4/common/common_def.py` & `rcs_common-0.2.5/common/common_def.py`

 * *Files identical despite different names*

### Comparing `rcs_common-0.2.4/common/common_types.py` & `rcs_common-0.2.5/common/common_types.py`

 * *Files identical despite different names*

### Comparing `rcs_common-0.2.4/common/filter_utils.py` & `rcs_common-0.2.5/common/filter_utils.py`

 * *Files identical despite different names*

### Comparing `rcs_common-0.2.4/common/geoutils.py` & `rcs_common-0.2.5/common/geoutils.py`

 * *Files identical despite different names*

### Comparing `rcs_common-0.2.4/common/getip.py` & `rcs_common-0.2.5/common/getip.py`

 * *Files identical despite different names*

### Comparing `rcs_common-0.2.4/common/mcpop.py` & `rcs_common-0.2.5/common/mcpop.py`

 * *Files identical despite different names*

### Comparing `rcs_common-0.2.4/common/mcpre.py` & `rcs_common-0.2.5/common/mcpre.py`

 * *Files identical despite different names*

### Comparing `rcs_common-0.2.4/common/v2_1def.py` & `rcs_common-0.2.5/common/v2_1def.py`

 * *Files identical despite different names*

### Comparing `rcs_common-0.2.4/common/volume_4D_Converter.py` & `rcs_common-0.2.5/common/volume_4D_Converter.py`

 * *Files identical despite different names*

### Comparing `rcs_common-0.2.4/setup.py` & `rcs_common-0.2.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import setuptools
 setuptools.setup(
     name='rcs_common',
-    version='0.2.4',
+    version='0.2.5',
     description='Common directory of Airwayz Dev',
     url='https://bitbucket.org/airwayzdev/common',
     # project_urls = {
     #     "Bug Tracker": "https://bitbucket.org/airwayzdev/common/issues"
     # },
     packages=['common'],
-
     install_requires=['awz-server-api-test','awz_client_api_test','swagger-ui-bundle==0.0.9','clickclick','jsonschema','inflection','openapi-spec-validator==0.6.0',\
                     'numpy','pandas>=1.5.2',\
                     'python_dateutil>=2.8.2','pytz>=2022.6','requests>=2.28.1',\
                     'rtree>=1.0.1','scipy>=1.11.1',\
                     'Shapely>=1.8.5.post1'],
                     
-    dependency_links=['https://test.pypi.org/simple/'])
+    dependency_links=['https://test.pypi.org/simple/ awz-server-api-test','https://test.pypi.org/simple/ awz-client-api-test'])
```

