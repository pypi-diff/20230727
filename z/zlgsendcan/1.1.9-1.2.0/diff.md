# Comparing `tmp/zlgsendcan-1.1.9.tar.gz` & `tmp/zlgsendcan-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.1.9.tar", last modified: Thu Jul 27 03:42:11 2023, max compression
+gzip compressed data, was "zlgsendcan-1.2.0.tar", last modified: Thu Jul 27 05:06:45 2023, max compression
```

## Comparing `zlgsendcan-1.1.9.tar` & `zlgsendcan-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 03:42:11.097802 zlgsendcan-1.1.9/
--rw-rw-rw-   0        0        0      221 2023-07-27 03:42:11.097802 zlgsendcan-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-27 03:42:11.097802 zlgsendcan-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-07-27 03:36:37.000000 zlgsendcan-1.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 03:42:11.097802 zlgsendcan-1.1.9/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.9/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0     1998 2023-07-27 03:41:41.000000 zlgsendcan-1.1.9/zlgsendcan/example_test.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.9/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.9/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5271 2023-07-27 02:13:20.000000 zlgsendcan-1.1.9/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.9/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    25691 2023-07-27 02:13:20.000000 zlgsendcan-1.1.9/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    19391 2023-07-27 03:26:06.000000 zlgsendcan-1.1.9/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-27 03:42:11.097802 zlgsendcan-1.1.9/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      221 2023-07-27 03:42:10.000000 zlgsendcan-1.1.9/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-07-27 03:42:11.000000 zlgsendcan-1.1.9/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 03:42:10.000000 zlgsendcan-1.1.9/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-27 03:42:10.000000 zlgsendcan-1.1.9/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-27 03:42:10.000000 zlgsendcan-1.1.9/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 05:06:45.093339 zlgsendcan-1.2.0/
+-rw-rw-rw-   0        0        0      221 2023-07-27 05:06:45.092338 zlgsendcan-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-27 05:06:45.093339 zlgsendcan-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-07-27 05:06:39.000000 zlgsendcan-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 05:06:45.085337 zlgsendcan-1.2.0/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.2.0/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0     2076 2023-07-27 04:16:37.000000 zlgsendcan-1.2.0/zlgsendcan/example_test.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.2.0/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.2.0/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5271 2023-07-27 02:13:20.000000 zlgsendcan-1.2.0/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.2.0/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    25707 2023-07-27 05:06:39.000000 zlgsendcan-1.2.0/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    19391 2023-07-27 03:26:06.000000 zlgsendcan-1.2.0/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-27 05:06:45.091340 zlgsendcan-1.2.0/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-07-27 05:06:44.000000 zlgsendcan-1.2.0/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-07-27 05:06:45.000000 zlgsendcan-1.2.0/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 05:06:44.000000 zlgsendcan-1.2.0/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-27 05:06:44.000000 zlgsendcan-1.2.0/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 05:06:44.000000 zlgsendcan-1.2.0/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.1.9/zlgsendcan/example_test.py` & `zlgsendcan-1.2.0/zlgsendcan/example_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from zlgsendcan.zlgserver import *
-
-# 第一步初始化周立功设备,具体参数含义请进入这个类查看
+"""---------------------第一步初始化周立功设备,具体参数含义请进入这个类查看------------------"""
 zlg_init = MessageDate('can', 0, {'zcy': '500kbps 80%', 'sjy': '2Mbps 80%'})
 
+"""---------------------第二步获取dbc文件解析的db对象做成全局变量调用----------------------"""
 dbcpath = 'D:\***\***.dbc'
-# 第二步获取dbc文件解析的db对象做成全局变量调用
 get_dbc_db(dbcpath)
 
 """------------------第三步组装报文数据和发送信号------------------ 
     注意点：
         1、报文里面cycle_time如果不传，将自动获取dbc定义的周期时间，is_crc为0是不经过crc校验，1则经过，不传则默认为0，但crc涉及到机密，请结合本安装包自行在自己的工程里做crc脚本校验
         2、ZlgSend发送can信号会启动守护线程去发，主线程停止信号即停止发送
-    
 """
-
-
 # 多个报文发送组装数据格式及发送方式
 def send_many_msg():
     many_msg_data = {
         "GW_BCS_2_B": {"GW_BCS_2_B": {"BCS_VehSpdVD": 1, "BCS_VehSpd": 120}, "send_num": '-1', "cycle_time": 100,
                        'is_crc': '0'},
         "GW_BCS_2_BB": {"GW_BCS_2_BB": {"BCS_VehSpdVD": 1, "BCS_VehSpd": 120}, "send_num": '-1', "cycle_time": 100,
                         'is_crc': '0'}}
```

### Comparing `zlgsendcan-1.1.9/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.2.0/zlgsendcan/get_conf_info.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.9/zlgsendcan/parseDBC.py` & `zlgsendcan-1.2.0/zlgsendcan/parseDBC.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.9/zlgsendcan/yaml_util.py` & `zlgsendcan-1.2.0/zlgsendcan/yaml_util.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.9/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.2.0/zlgsendcan/zlgcan1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 import sys
 from ctypes import *
 import platform
-import frozen_dir
+from zlgsendcan import frozen_dir
 
 SETUP_DIR = frozen_dir.app_path() + r'\zlgcan_1.dll'
 sys.path.append(SETUP_DIR)
 ZCAN_DEVICE_TYPE = c_uint
 INVALID_DEVICE_HANDLE = 0
 INVALID_CHANNEL_HANDLE = 0
```

### Comparing `zlgsendcan-1.1.9/zlgsendcan/zlgserver.py` & `zlgsendcan-1.2.0/zlgsendcan/zlgserver.py`

 * *Files identical despite different names*

