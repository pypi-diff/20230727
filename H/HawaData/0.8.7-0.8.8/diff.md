# Comparing `tmp/HawaData-0.8.7.tar.gz` & `tmp/HawaData-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.8.7.tar", last modified: Thu Jul 27 02:47:00 2023, max compression
+gzip compressed data, was "HawaData-0.8.8.tar", last modified: Thu Jul 27 02:50:31 2023, max compression
```

## Comparing `HawaData-0.8.7.tar` & `HawaData-0.8.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:47:00.981382 HawaData-0.8.7/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:47:00.968532 HawaData-0.8.7/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3484 2023-07-27 02:47:00.000000 HawaData-0.8.7/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-27 02:47:00.000000 HawaData-0.8.7/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-27 02:47:00.000000 HawaData-0.8.7/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-27 02:47:00.000000 HawaData-0.8.7/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3484 2023-07-27 02:47:00.981023 HawaData-0.8.7/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.8.7/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:47:00.969225 HawaData-0.8.7/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.8.7/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:47:00.971887 HawaData-0.8.7/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.8.7/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2807 2023-07-27 02:46:27.000000 HawaData-0.8.7/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      522 2023-07-24 09:22:05.000000 HawaData-0.8.7/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.8.7/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.8.7/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:47:00.973626 HawaData-0.8.7/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.8.7/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    17172 2023-07-27 02:46:27.000000 HawaData-0.8.7/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     6455 2023-07-26 15:07:30.000000 HawaData-0.8.7/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.8.7/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.8.7/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:47:00.978150 HawaData-0.8.7/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.8.7/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.8.7/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.8.7/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.8.7/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.8.7/hawa/data/province.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.8.7/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.8.7/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:47:00.979571 HawaData-0.8.7/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.8.7/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28951 2023-07-24 04:31:22.000000 HawaData-0.8.7/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.8.7/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-27 02:47:00.981485 HawaData-0.8.7/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.8.7/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:47:00.980255 HawaData-0.8.7/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.8.7/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:50:31.775715 HawaData-0.8.8/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:50:31.765183 HawaData-0.8.8/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3496 2023-07-27 02:50:31.000000 HawaData-0.8.8/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-27 02:50:31.000000 HawaData-0.8.8/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-27 02:50:31.000000 HawaData-0.8.8/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-27 02:50:31.000000 HawaData-0.8.8/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3496 2023-07-27 02:50:31.775331 HawaData-0.8.8/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.8.8/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:50:31.766007 HawaData-0.8.8/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.8.8/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:50:31.767956 HawaData-0.8.8/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.8.8/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2807 2023-07-27 02:46:27.000000 HawaData-0.8.8/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      522 2023-07-24 09:22:05.000000 HawaData-0.8.8/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.8.8/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.8.8/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:50:31.770075 HawaData-0.8.8/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.8.8/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    17081 2023-07-27 02:50:20.000000 HawaData-0.8.8/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     6455 2023-07-26 15:07:30.000000 HawaData-0.8.8/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.8.8/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.8.8/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:50:31.773182 HawaData-0.8.8/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.8.8/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.8.8/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.8.8/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.8.8/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.8.8/hawa/data/province.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.8.8/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.8.8/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:50:31.774361 HawaData-0.8.8/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.8.8/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28951 2023-07-24 04:31:22.000000 HawaData-0.8.8/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.8.8/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-27 02:50:31.775838 HawaData-0.8.8/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.8.8/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 02:50:31.774765 HawaData-0.8.8/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.8.8/test/test_query.py
```

### Comparing `HawaData-0.8.7/HawaData.egg-info/PKG-INFO` & `HawaData-0.8.8/HawaData.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.8.7
+Version: 0.8.8
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -118,7 +118,8 @@
 - 0.8.0 sort dim field
 - 0.8.1 sort dim field
 - 0.8.2 add global precision
 - 0.8.3 add global precision in func
 - 0.8.4 fix extra dim/field
 - 0.8.5 load less data
 - 0.8.7 add mongo params
+- 0.8.8 fix
```

### Comparing `HawaData-0.8.7/HawaData.egg-info/SOURCES.txt` & `HawaData-0.8.8/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/PKG-INFO` & `HawaData-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.8.7
+Version: 0.8.8
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -118,7 +118,8 @@
 - 0.8.0 sort dim field
 - 0.8.1 sort dim field
 - 0.8.2 add global precision
 - 0.8.3 add global precision in func
 - 0.8.4 fix extra dim/field
 - 0.8.5 load less data
 - 0.8.7 add mongo params
+- 0.8.8 fix
```

### Comparing `HawaData-0.8.7/README.md` & `HawaData-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/hawa/base/db.py` & `HawaData-0.8.8/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/hawa/base/decos.py` & `HawaData-0.8.8/hawa/base/decos.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/hawa/base/init.py` & `HawaData-0.8.8/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/hawa/common/data.py` & `HawaData-0.8.8/hawa/common/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,16 +91,14 @@
             self._to_build_helper()
 
             # 计算数据
             count_functions = [i for i in dir(self) if i.startswith('_to_count_')]
             for func in count_functions:
                 getattr(self, func)()
 
-            t3 = time.perf_counter()
-            print(f"count data cost: {t3 - t2:.2f}s")
         else:
             self.load_less_data()
             self._to_build_helper()
 
     def _to_init_a_meta_unit(self):
         self.meta_unit = self.query.query_unit(self.meta_unit_type, str(self.meta_unit_id))
```

### Comparing `HawaData-0.8.7/hawa/common/query.py` & `HawaData-0.8.8/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/hawa/common/utils.py` & `HawaData-0.8.8/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/hawa/config.py` & `HawaData-0.8.8/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/hawa/data/klass.py` & `HawaData-0.8.8/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/hawa/data/province.py` & `HawaData-0.8.8/hawa/data/province.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/hawa/data/school.py` & `HawaData-0.8.8/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/hawa/data/student.py` & `HawaData-0.8.8/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/hawa/paper/health.py` & `HawaData-0.8.8/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/hawa/paper/mht.py` & `HawaData-0.8.8/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/setup.py` & `HawaData-0.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.7/test/test_query.py` & `HawaData-0.8.8/test/test_query.py`

 * *Files identical despite different names*

