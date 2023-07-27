# Comparing `tmp/zlgsendcan-1.1.7.tar.gz` & `tmp/zlgsendcan-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.1.7.tar", last modified: Thu Jul 27 02:43:14 2023, max compression
+gzip compressed data, was "zlgsendcan-1.1.8.tar", last modified: Thu Jul 27 03:06:31 2023, max compression
```

## Comparing `zlgsendcan-1.1.7.tar` & `zlgsendcan-1.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 02:43:14.386310 zlgsendcan-1.1.7/
--rw-rw-rw-   0        0        0      220 2023-07-27 02:43:14.386310 zlgsendcan-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-27 02:43:14.386310 zlgsendcan-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      463 2023-07-27 02:40:07.000000 zlgsendcan-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 02:43:14.386310 zlgsendcan-1.1.7/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.7/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.7/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.7/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5271 2023-07-27 02:13:20.000000 zlgsendcan-1.1.7/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.7/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    25691 2023-07-27 02:13:20.000000 zlgsendcan-1.1.7/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    19356 2023-07-27 01:53:33.000000 zlgsendcan-1.1.7/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-27 02:43:14.386310 zlgsendcan-1.1.7/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-27 02:43:14.000000 zlgsendcan-1.1.7/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-27 02:43:14.000000 zlgsendcan-1.1.7/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 02:43:14.000000 zlgsendcan-1.1.7/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-27 02:43:14.000000 zlgsendcan-1.1.7/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-27 02:43:14.000000 zlgsendcan-1.1.7/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 03:06:31.477833 zlgsendcan-1.1.8/
+-rw-rw-rw-   0        0        0      221 2023-07-27 03:06:31.477833 zlgsendcan-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-27 03:06:31.477833 zlgsendcan-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-07-27 03:06:04.000000 zlgsendcan-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:06:31.477833 zlgsendcan-1.1.8/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.8/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.8/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.8/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5271 2023-07-27 02:13:20.000000 zlgsendcan-1.1.8/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.8/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    25691 2023-07-27 02:13:20.000000 zlgsendcan-1.1.8/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    19137 2023-07-27 02:58:24.000000 zlgsendcan-1.1.8/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:06:31.477833 zlgsendcan-1.1.8/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-07-27 03:06:31.000000 zlgsendcan-1.1.8/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-27 03:06:31.000000 zlgsendcan-1.1.8/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 03:06:31.000000 zlgsendcan-1.1.8/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-27 03:06:31.000000 zlgsendcan-1.1.8/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 03:06:31.000000 zlgsendcan-1.1.8/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.1.7/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.1.8/zlgsendcan/get_conf_info.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.7/zlgsendcan/parseDBC.py` & `zlgsendcan-1.1.8/zlgsendcan/parseDBC.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.7/zlgsendcan/yaml_util.py` & `zlgsendcan-1.1.8/zlgsendcan/yaml_util.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.7/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.1.8/zlgsendcan/zlgcan1.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.7/zlgsendcan/zlgserver.py` & `zlgsendcan-1.1.8/zlgsendcan/zlgserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 import copy
 import importlib
 import time
 from PyQt5.QtWidgets import QMessageBox
 from zlgsendcan.parseDBC import GlobleValue, DbcInit, get_signal_data1
 from zlgsendcan.zlgcan1 import *
 import threading
-from zlgsendcan.get_conf_info import GetBaseInfo
-
-data_ = GetBaseInfo().get_base_config()
-condition = threading.Condition()
 
 
 # 获取dbc文件解析的db对象做成全局变量调用
 def get_dbc_db(dbc_path):
     GlobleValue.dbc_init = get_signal_data1(dbc_path).db  # 初始化解析dbc文件
 
 
-
 class MessageDate:
     def __init__(self, can_type, chanl, brate: dict):
         """
 
         :param can_type: 1、can 2、canfd
         :param chanl: 0,1
         :param brate: {'zcy':'500kbps 80%','sjy':'2Mbps 80%‘}注意如果自定义波特率格式如下
@@ -93,15 +88,14 @@
 
     return fun
 
 
 # dbc发送
 def canfd_msg(ob, data):
     try:
-        data_ = GetBaseInfo().get_base_config()
 
         data = [data] if type(data[0]) != list else data
         data_len = len(data)
         # print('=============',data_len)
         canfd_msgs = (ZCANDataObj * data_len)()
         # memset(byref(canfd_msgs), 0, sizeof(canfd_msgs))
         # canfd_msgs = (ZCAN_TransmitFD_Data * 10)()
@@ -129,15 +123,14 @@
         return canfd_msgs, data_len
     except Exception as e:
         print('canfd_msg组装数据错误==', e, data, ob.message_length, ob.message_frame_id)
 
 
 # 普通发送
 def canfd_msg_power(idx, data):
-    data_ = GetBaseInfo().get_base_config()
     canfd_msgs = (ZCANDataObj * 1)()
     for i in range(1):
         canfd_msgs[i].dataType = 1  # can/canfd frame
         canfd_msgs[i].chnl = int(GlobleValue.can_conf['chan'])  # can_channel
         canfd_msgs[i].zcanfddata.flag.frameType = 1 if GlobleValue.can_conf[
                                                            'can_type'] == 'canfd' else 0  # 0-can,1-canfd
         canfd_msgs[i].zcanfddata.flag.txDelay = 0  # 不添加延迟
@@ -149,15 +142,15 @@
         for j in range(8):
             canfd_msgs[i].zcanfddata.frame.data[j] = data[j]
     return canfd_msgs
 
 
 class ZlgSend:
 
-    def __init__(self, handle, data, dbc_file, pro_name, is_key=False):
+    def __init__(self, handle, data, dbc_file, pro_name=None, is_key=False):
         GlobleValue.thread_run = True
         if not is_key:
             for k, v in data.items():
                 thread_list = []
                 # for name1, msgdata in data[k].items():
                 if k not in ['cycle_time', 'send_num', 'msg_id', 'is_crc']:
                     ctime = data['cycle_time']
```

