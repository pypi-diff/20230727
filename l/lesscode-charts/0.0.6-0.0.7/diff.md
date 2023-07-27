# Comparing `tmp/lesscode_charts-0.0.6.tar.gz` & `tmp/lesscode_charts-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_charts-0.0.6.tar", last modified: Tue Jul  4 08:45:23 2023, max compression
+gzip compressed data, was "dist/lesscode_charts-0.0.7.tar", last modified: Thu Jul 27 02:33:05 2023, max compression
```

## Comparing `lesscode_charts-0.0.6.tar` & `lesscode_charts-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/
--rw-r--r--   0 baai       (501) staff       (20)      397 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)       61 2023-05-19 12:52:02.000000 lesscode_charts-0.0.6/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:23.000000 lesscode_charts-0.0.6/lesscode_charts/__init__.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts/utils/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:19:20.000000 lesscode_charts-0.0.6/lesscode_charts/utils/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     1238 2023-05-19 08:41:53.000000 lesscode_charts-0.0.6/lesscode_charts/utils/common_utils.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts/v1/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:49.000000 lesscode_charts-0.0.6/lesscode_charts/v1/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)      582 2023-05-19 07:43:47.000000 lesscode_charts-0.0.6/lesscode_charts/v1/forest_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     3459 2023-06-05 09:16:34.000000 lesscode_charts-0.0.6/lesscode_charts/v1/histogram_chart.py
--rw-r--r--   0 baai       (501) staff       (20)      848 2023-05-19 07:29:21.000000 lesscode_charts-0.0.6/lesscode_charts/v1/k_line_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1444 2023-07-04 08:44:48.000000 lesscode_charts-0.0.6/lesscode_charts/v1/pie_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1143 2023-07-04 08:44:48.000000 lesscode_charts-0.0.6/lesscode_charts/v1/pyramid_chart.py
--rw-r--r--   0 baai       (501) staff       (20)      814 2023-05-19 07:29:21.000000 lesscode_charts-0.0.6/lesscode_charts/v1/radar_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     1870 2023-05-31 11:03:04.000000 lesscode_charts-0.0.6/lesscode_charts/v1/sankey_chart.py
--rw-r--r--   0 baai       (501) staff       (20)     3088 2023-05-19 02:50:25.000000 lesscode_charts-0.0.6/lesscode_charts/v1/table_chart.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-07-04 08:45:12.000000 lesscode_charts-0.0.6/lesscode_charts/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)      397 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      611 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       16 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/lesscode_charts.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-07-04 08:45:23.000000 lesscode_charts-0.0.6/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1223 2023-05-19 09:42:06.000000 lesscode_charts-0.0.6/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-27 02:33:05.000000 lesscode_charts-0.0.7/
+-rw-r--r--   0 baai       (501) staff       (20)      397 2023-07-27 02:33:05.000000 lesscode_charts-0.0.7/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       61 2023-05-19 12:52:02.000000 lesscode_charts-0.0.7/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-27 02:33:05.000000 lesscode_charts-0.0.7/lesscode_charts/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:23.000000 lesscode_charts-0.0.7/lesscode_charts/__init__.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-27 02:33:05.000000 lesscode_charts-0.0.7/lesscode_charts/utils/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:19:20.000000 lesscode_charts-0.0.7/lesscode_charts/utils/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     1238 2023-05-19 08:41:53.000000 lesscode_charts-0.0.7/lesscode_charts/utils/common_utils.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-27 02:33:05.000000 lesscode_charts-0.0.7/lesscode_charts/v1/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-05-19 01:13:49.000000 lesscode_charts-0.0.7/lesscode_charts/v1/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)      582 2023-05-19 07:43:47.000000 lesscode_charts-0.0.7/lesscode_charts/v1/forest_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     3459 2023-06-05 09:16:34.000000 lesscode_charts-0.0.7/lesscode_charts/v1/histogram_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)      848 2023-05-19 07:29:21.000000 lesscode_charts-0.0.7/lesscode_charts/v1/k_line_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1444 2023-07-04 08:44:48.000000 lesscode_charts-0.0.7/lesscode_charts/v1/pie_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1143 2023-07-04 08:44:48.000000 lesscode_charts-0.0.7/lesscode_charts/v1/pyramid_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)      814 2023-05-19 07:29:21.000000 lesscode_charts-0.0.7/lesscode_charts/v1/radar_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     1870 2023-05-31 11:03:04.000000 lesscode_charts-0.0.7/lesscode_charts/v1/sankey_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)     3125 2023-07-27 02:32:26.000000 lesscode_charts-0.0.7/lesscode_charts/v1/table_chart.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-07-27 02:32:26.000000 lesscode_charts-0.0.7/lesscode_charts/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-27 02:33:05.000000 lesscode_charts-0.0.7/lesscode_charts.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      397 2023-07-27 02:33:05.000000 lesscode_charts-0.0.7/lesscode_charts.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      611 2023-07-27 02:33:05.000000 lesscode_charts-0.0.7/lesscode_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-07-27 02:33:05.000000 lesscode_charts-0.0.7/lesscode_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       16 2023-07-27 02:33:05.000000 lesscode_charts-0.0.7/lesscode_charts.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-07-27 02:33:05.000000 lesscode_charts-0.0.7/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1223 2023-05-19 09:42:06.000000 lesscode_charts-0.0.7/setup.py
```

### Comparing `lesscode_charts-0.0.6/lesscode_charts/utils/common_utils.py` & `lesscode_charts-0.0.7/lesscode_charts/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.6/lesscode_charts/v1/forest_chart.py` & `lesscode_charts-0.0.7/lesscode_charts/v1/forest_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.6/lesscode_charts/v1/histogram_chart.py` & `lesscode_charts-0.0.7/lesscode_charts/v1/histogram_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.6/lesscode_charts/v1/k_line_chart.py` & `lesscode_charts-0.0.7/lesscode_charts/v1/k_line_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.6/lesscode_charts/v1/pie_chart.py` & `lesscode_charts-0.0.7/lesscode_charts/v1/pie_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.6/lesscode_charts/v1/pyramid_chart.py` & `lesscode_charts-0.0.7/lesscode_charts/v1/pyramid_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.6/lesscode_charts/v1/radar_chart.py` & `lesscode_charts-0.0.7/lesscode_charts/v1/radar_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.6/lesscode_charts/v1/sankey_chart.py` & `lesscode_charts-0.0.7/lesscode_charts/v1/sankey_chart.py`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.6/lesscode_charts/v1/table_chart.py` & `lesscode_charts-0.0.7/lesscode_charts/v1/table_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,12 +63,13 @@
                 result["dataSource"].append(data_item)
                 index_start += 1
         else:
             if index_enable:
                 for item in data:
                     item[index_key] = index_start + 1
                     result["dataSource"].append(item)
+                    index_start += 1
             else:
                 result["dataSource"] = data
         result["total"] = total
 
         return result
```

### Comparing `lesscode_charts-0.0.6/lesscode_charts.egg-info/SOURCES.txt` & `lesscode_charts-0.0.7/lesscode_charts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesscode_charts-0.0.6/setup.py` & `lesscode_charts-0.0.7/setup.py`

 * *Files identical despite different names*

