# Comparing `tmp/min_max_heap-1.0.0.tar.gz` & `tmp/min_max_heap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "min_max_heap-1.0.0.tar", last modified: Tue Jul 25 05:18:57 2023, max compression
+gzip compressed data, was "min_max_heap-1.0.1.tar", last modified: Thu Jul 27 08:35:31 2023, max compression
```

## Comparing `min_max_heap-1.0.0.tar` & `min_max_heap-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yuan      (1000) yuan      (1000)        0 2023-07-25 05:18:57.225360 min_max_heap-1.0.0/
--rw-r--r--   0 yuan      (1000) yuan      (1000)     1066 2023-07-17 03:08:17.000000 min_max_heap-1.0.0/LICENSE
--rw-r--r--   0 yuan      (1000) yuan      (1000)      965 2023-07-25 05:18:57.225360 min_max_heap-1.0.0/PKG-INFO
--rw-r--r--   0 yuan      (1000) yuan      (1000)      302 2023-07-25 04:26:50.000000 min_max_heap-1.0.0/README.md
-drwxr-xr-x   0 yuan      (1000) yuan      (1000)        0 2023-07-25 05:18:57.225360 min_max_heap-1.0.0/min_max_heap.egg-info/
--rw-r--r--   0 yuan      (1000) yuan      (1000)      965 2023-07-25 05:18:57.000000 min_max_heap-1.0.0/min_max_heap.egg-info/PKG-INFO
--rw-r--r--   0 yuan      (1000) yuan      (1000)      219 2023-07-25 05:18:57.000000 min_max_heap-1.0.0/min_max_heap.egg-info/SOURCES.txt
--rw-r--r--   0 yuan      (1000) yuan      (1000)        1 2023-07-25 05:18:57.000000 min_max_heap-1.0.0/min_max_heap.egg-info/dependency_links.txt
--rw-r--r--   0 yuan      (1000) yuan      (1000)       13 2023-07-25 05:18:57.000000 min_max_heap-1.0.0/min_max_heap.egg-info/top_level.txt
--rw-r--r--   0 yuan      (1000) yuan      (1000)       38 2023-07-25 05:18:57.225360 min_max_heap-1.0.0/setup.cfg
--rw-r--r--   0 yuan      (1000) yuan      (1000)      886 2023-07-25 04:46:47.000000 min_max_heap-1.0.0/setup.py
-drwxr-xr-x   0 yuan      (1000) yuan      (1000)        0 2023-07-25 05:18:57.225360 min_max_heap-1.0.0/src/
--rw-r--r--   0 yuan      (1000) yuan      (1000)      257 2023-07-25 04:19:57.000000 min_max_heap-1.0.0/src/__init__.py
--rw-r--r--   0 yuan      (1000) yuan      (1000)      644 2023-07-25 04:19:38.000000 min_max_heap-1.0.0/src/min_max_heap.py
--rw-r--r--   0 yuan      (1000) yuan      (1000)     2957 2023-07-25 04:25:39.000000 min_max_heap-1.0.0/src/utils.py
+drwxr-xr-x   0 yuan      (1000) yuan      (1000)        0 2023-07-27 08:35:31.439614 min_max_heap-1.0.1/
+-rw-r--r--   0 yuan      (1000) yuan      (1000)     1066 2023-07-17 03:08:17.000000 min_max_heap-1.0.1/LICENSE
+-rw-r--r--   0 yuan      (1000) yuan      (1000)      966 2023-07-27 08:35:31.439614 min_max_heap-1.0.1/PKG-INFO
+-rw-r--r--   0 yuan      (1000) yuan      (1000)      303 2023-07-27 08:31:48.000000 min_max_heap-1.0.1/README.md
+drwxr-xr-x   0 yuan      (1000) yuan      (1000)        0 2023-07-27 08:35:31.439614 min_max_heap-1.0.1/min_max_heap.egg-info/
+-rw-r--r--   0 yuan      (1000) yuan      (1000)      966 2023-07-27 08:35:31.000000 min_max_heap-1.0.1/min_max_heap.egg-info/PKG-INFO
+-rw-r--r--   0 yuan      (1000) yuan      (1000)      219 2023-07-27 08:35:31.000000 min_max_heap-1.0.1/min_max_heap.egg-info/SOURCES.txt
+-rw-r--r--   0 yuan      (1000) yuan      (1000)        1 2023-07-27 08:35:31.000000 min_max_heap-1.0.1/min_max_heap.egg-info/dependency_links.txt
+-rw-r--r--   0 yuan      (1000) yuan      (1000)       13 2023-07-27 08:35:31.000000 min_max_heap-1.0.1/min_max_heap.egg-info/top_level.txt
+-rw-r--r--   0 yuan      (1000) yuan      (1000)       38 2023-07-27 08:35:31.439614 min_max_heap-1.0.1/setup.cfg
+-rw-r--r--   0 yuan      (1000) yuan      (1000)      886 2023-07-27 08:34:30.000000 min_max_heap-1.0.1/setup.py
+drwxr-xr-x   0 yuan      (1000) yuan      (1000)        0 2023-07-27 08:35:31.439614 min_max_heap-1.0.1/src/
+-rw-r--r--   0 yuan      (1000) yuan      (1000)      257 2023-07-25 04:19:57.000000 min_max_heap-1.0.1/src/__init__.py
+-rw-r--r--   0 yuan      (1000) yuan      (1000)      644 2023-07-25 04:19:38.000000 min_max_heap-1.0.1/src/min_max_heap.py
+-rw-r--r--   0 yuan      (1000) yuan      (1000)     2957 2023-07-27 08:29:51.000000 min_max_heap-1.0.1/src/utils.py
```

### Comparing `min_max_heap-1.0.0/LICENSE` & `min_max_heap-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `min_max_heap-1.0.0/PKG-INFO` & `min_max_heap-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: min_max_heap
-Version: 1.0.0
+Version: 1.0.1
 Summary: A implementation of MinMaxHeap with Python language.
 Home-page: https://github.com/hfi/min-max-heap
 Author: Yuan Yang
 Author-email: i@yangyuan.me
 License: The MIT License (MIT)
 Platform: Any
 Classifier: Programming Language :: Python
@@ -34,7 +34,8 @@
 for i in range(50):
     assert heap.pop_min() == i
     assert heap.pop_max() == 99 - i
 
 assert heap.is_empty()
 ```
 
+
```

### Comparing `min_max_heap-1.0.0/min_max_heap.egg-info/PKG-INFO` & `min_max_heap-1.0.1/min_max_heap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: min-max-heap
-Version: 1.0.0
+Version: 1.0.1
 Summary: A implementation of MinMaxHeap with Python language.
 Home-page: https://github.com/hfi/min-max-heap
 Author: Yuan Yang
 Author-email: i@yangyuan.me
 License: The MIT License (MIT)
 Platform: Any
 Classifier: Programming Language :: Python
@@ -34,7 +34,8 @@
 for i in range(50):
     assert heap.pop_min() == i
     assert heap.pop_max() == 99 - i
 
 assert heap.is_empty()
 ```
 
+
```

### Comparing `min_max_heap-1.0.0/setup.py` & `min_max_heap-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 
 with open("README.md", "r") as fp:
     long_desc = fp.read()
 
 setup(
     name=name,
-    version="1.0.0",
+    version="1.0.1",
     author="Yuan Yang",
     author_email="i@yangyuan.me",
     packages=[name],
     package_dir={name: "src"},
     url="https://github.com/hfi/min-max-heap",
     classifiers=classifiers,
     license="The MIT License (MIT)",
```

### Comparing `min_max_heap-1.0.0/src/min_max_heap.py` & `min_max_heap-1.0.1/src/min_max_heap.py`

 * *Files identical despite different names*

### Comparing `min_max_heap-1.0.0/src/utils.py` & `min_max_heap-1.0.1/src/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 def heaplify(heap):
     size = len(heap)
-    for i in range((size - 3)>>1, -1, -1):
+    for i in range((size - 1)>>1, -1, -1):
         siftdown(heap, i)
 
 def siftdown(heap, k):
     if (k & 1) == 0:
         siftdown_min(heap, k)
     else:
         siftdown_max(heap, k)
```

