# Comparing `tmp/pytkUI-1.0.0.tar.gz` & `tmp/pytkUI-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytkUI-1.0.0.tar", last modified: Thu Jul 27 11:51:49 2023, max compression
+gzip compressed data, was "dist\pytkUI-1.0.1.tar", last modified: Thu Jul 27 11:48:32 2023, max compression
```

## Comparing `pytkUI-1.0.0.tar` & `pytkUI-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:51:49.328009 pytkUI-1.0.0/
--rw-rw-rw-   0        0        0     1040 2023-07-27 11:51:49.312391 pytkUI-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      811 2023-07-27 11:51:36.000000 pytkUI-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 11:51:49.281144 pytkUI-1.0.0/pytkUI/
--rw-rw-rw-   0        0        0        0 2023-06-09 06:16:51.000000 pytkUI-1.0.0/pytkUI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:51:49.296767 pytkUI-1.0.0/pytkUI/ext/
--rw-rw-rw-   0        0        0        0 2023-06-15 09:25:02.000000 pytkUI-1.0.0/pytkUI/ext/__init__.py
--rw-rw-rw-   0        0        0     4511 2023-07-27 11:48:02.000000 pytkUI-1.0.0/pytkUI/ext/ext_tabs.py
--rw-rw-rw-   0        0        0      667 2023-07-27 11:48:02.000000 pytkUI-1.0.0/pytkUI/ext/icon.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:51:49.312391 pytkUI-1.0.0/pytkUI/icons/
--rw-rw-rw-   0        0        0    49971 2023-05-31 05:59:23.000000 pytkUI-1.0.0/pytkUI/icons/bootstrap-icons.json
--rw-rw-rw-   0        0        0   164360 2023-05-31 05:59:30.000000 pytkUI-1.0.0/pytkUI/icons/bootstrap-icons.woff
-drwxrwxrwx   0        0        0        0 2023-07-27 11:51:49.312391 pytkUI-1.0.0/pytkUI/overwrite/
--rw-rw-rw-   0        0        0     2435 2023-06-14 03:32:19.000000 pytkUI-1.0.0/pytkUI/overwrite/DateEntry.py
--rw-rw-rw-   0        0        0        0 2023-06-14 14:24:28.000000 pytkUI-1.0.0/pytkUI/overwrite/__init__.py
--rw-rw-rw-   0        0        0     2215 2023-06-16 08:55:48.000000 pytkUI-1.0.0/pytkUI/utils.py
--rw-rw-rw-   0        0        0      194 2023-07-27 11:48:02.000000 pytkUI-1.0.0/pytkUI/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:51:49.281144 pytkUI-1.0.0/pytkUI.egg-info/
--rw-rw-rw-   0        0        0     1040 2023-07-27 11:51:48.000000 pytkUI-1.0.0/pytkUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-07-27 11:51:49.000000 pytkUI-1.0.0/pytkUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 11:51:48.000000 pytkUI-1.0.0/pytkUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 11:51:48.000000 pytkUI-1.0.0/pytkUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 11:51:49.328009 pytkUI-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-07-27 11:51:36.000000 pytkUI-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:48:32.216439 pytkUI-1.0.1/
+-rw-rw-rw-   0        0        0     1041 2023-07-27 11:48:32.216439 pytkUI-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      812 2023-07-27 07:50:36.000000 pytkUI-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 11:48:32.169540 pytkUI-1.0.1/pytkUI/
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:16:51.000000 pytkUI-1.0.1/pytkUI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:48:32.200806 pytkUI-1.0.1/pytkUI/ext/
+-rw-rw-rw-   0        0        0        0 2023-06-15 09:25:02.000000 pytkUI-1.0.1/pytkUI/ext/__init__.py
+-rw-rw-rw-   0        0        0     4511 2023-07-27 11:48:02.000000 pytkUI-1.0.1/pytkUI/ext/ext_tabs.py
+-rw-rw-rw-   0        0        0      667 2023-07-27 11:48:02.000000 pytkUI-1.0.1/pytkUI/ext/icon.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:48:32.200806 pytkUI-1.0.1/pytkUI/icons/
+-rw-rw-rw-   0        0        0    49971 2023-05-31 05:59:23.000000 pytkUI-1.0.1/pytkUI/icons/bootstrap-icons.json
+-rw-rw-rw-   0        0        0   164360 2023-05-31 05:59:30.000000 pytkUI-1.0.1/pytkUI/icons/bootstrap-icons.woff
+drwxrwxrwx   0        0        0        0 2023-07-27 11:48:32.216439 pytkUI-1.0.1/pytkUI/overwrite/
+-rw-rw-rw-   0        0        0     2435 2023-06-14 03:32:19.000000 pytkUI-1.0.1/pytkUI/overwrite/DateEntry.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 14:24:28.000000 pytkUI-1.0.1/pytkUI/overwrite/__init__.py
+-rw-rw-rw-   0        0        0     2215 2023-06-16 08:55:48.000000 pytkUI-1.0.1/pytkUI/utils.py
+-rw-rw-rw-   0        0        0      194 2023-07-27 11:48:02.000000 pytkUI-1.0.1/pytkUI/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:48:32.185163 pytkUI-1.0.1/pytkUI.egg-info/
+-rw-rw-rw-   0        0        0     1041 2023-07-27 11:48:31.000000 pytkUI-1.0.1/pytkUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-27 11:48:31.000000 pytkUI-1.0.1/pytkUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:48:31.000000 pytkUI-1.0.1/pytkUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 11:48:31.000000 pytkUI-1.0.1/pytkUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:48:32.216439 pytkUI-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-07-27 11:48:09.000000 pytkUI-1.0.1/setup.py
```

### Comparing `pytkUI-1.0.0/PKG-INFO` & `pytkUI-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pytkUI
-Version: 1.0.0
+Version: 1.0.1
 Summary: TkinterHelper布局助手官方拓展和工具库
 Home-page: https://www.pytk.net
 Author: iamxcd
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 TkinterHelper布局助手官方拓展和工具库
 
 ## 安装方式
 
-> pip install pytkUI
+> pip install pytknet
 
 ## 工具函数
 
 utils.py 整合了一些常用的工具函数
 
 ### 加载图片
```

### Comparing `pytkUI-1.0.0/README.md` & `pytkUI-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 TkinterHelper布局助手官方拓展和工具库
 
 ## 安装方式
 
-> pip install pytkUI
+> pip install pytknet
 
 ## 工具函数
 
 utils.py 整合了一些常用的工具函数
 
 ### 加载图片
```

### Comparing `pytkUI-1.0.0/pytkUI/ext/ext_tabs.py` & `pytkUI-1.0.1/pytkUI/ext/ext_tabs.py`

 * *Files identical despite different names*

### Comparing `pytkUI-1.0.0/pytkUI/ext/icon.py` & `pytkUI-1.0.1/pytkUI/ext/icon.py`

 * *Files identical despite different names*

### Comparing `pytkUI-1.0.0/pytkUI/icons/bootstrap-icons.json` & `pytkUI-1.0.1/pytkUI/icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `pytkUI-1.0.0/pytkUI/icons/bootstrap-icons.woff` & `pytkUI-1.0.1/pytkUI/icons/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `pytkUI-1.0.0/pytkUI/overwrite/DateEntry.py` & `pytkUI-1.0.1/pytkUI/overwrite/DateEntry.py`

 * *Files identical despite different names*

### Comparing `pytkUI-1.0.0/pytkUI/utils.py` & `pytkUI-1.0.1/pytkUI/utils.py`

 * *Files identical despite different names*

### Comparing `pytkUI-1.0.0/pytkUI.egg-info/PKG-INFO` & `pytkUI-1.0.1/pytkUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pytkUI
-Version: 1.0.0
+Version: 1.0.1
 Summary: TkinterHelper布局助手官方拓展和工具库
 Home-page: https://www.pytk.net
 Author: iamxcd
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 TkinterHelper布局助手官方拓展和工具库
 
 ## 安装方式
 
-> pip install pytkUI
+> pip install pytknet
 
 ## 工具函数
 
 utils.py 整合了一些常用的工具函数
 
 ### 加载图片
```

