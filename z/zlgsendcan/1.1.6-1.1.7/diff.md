# Comparing `tmp/zlgsendcan-1.1.6.tar.gz` & `tmp/zlgsendcan-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.1.6.tar", last modified: Wed Jul 26 12:33:41 2023, max compression
+gzip compressed data, was "zlgsendcan-1.1.7.tar", last modified: Thu Jul 27 02:43:14 2023, max compression
```

## Comparing `zlgsendcan-1.1.6.tar` & `zlgsendcan-1.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 12:33:41.374465 zlgsendcan-1.1.6/
--rw-rw-rw-   0        0        0      220 2023-07-26 12:33:41.373513 zlgsendcan-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 12:33:41.374465 zlgsendcan-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      463 2023-07-26 12:33:38.000000 zlgsendcan-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:33:41.364610 zlgsendcan-1.1.6/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.6/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.6/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.6/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5262 2023-07-26 12:12:26.000000 zlgsendcan-1.1.6/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.6/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    26010 2023-07-26 12:01:29.000000 zlgsendcan-1.1.6/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    18925 2023-07-26 12:20:21.000000 zlgsendcan-1.1.6/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:33:41.372456 zlgsendcan-1.1.6/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-26 12:33:41.000000 zlgsendcan-1.1.6/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-26 12:33:41.000000 zlgsendcan-1.1.6/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 12:33:41.000000 zlgsendcan-1.1.6/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-26 12:33:41.000000 zlgsendcan-1.1.6/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 12:33:41.000000 zlgsendcan-1.1.6/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 02:43:14.386310 zlgsendcan-1.1.7/
+-rw-rw-rw-   0        0        0      220 2023-07-27 02:43:14.386310 zlgsendcan-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-27 02:43:14.386310 zlgsendcan-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      463 2023-07-27 02:40:07.000000 zlgsendcan-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:43:14.386310 zlgsendcan-1.1.7/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.7/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.7/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.7/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5271 2023-07-27 02:13:20.000000 zlgsendcan-1.1.7/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.7/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    25691 2023-07-27 02:13:20.000000 zlgsendcan-1.1.7/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    19356 2023-07-27 01:53:33.000000 zlgsendcan-1.1.7/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:43:14.386310 zlgsendcan-1.1.7/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-07-27 02:43:14.000000 zlgsendcan-1.1.7/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-27 02:43:14.000000 zlgsendcan-1.1.7/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 02:43:14.000000 zlgsendcan-1.1.7/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-27 02:43:14.000000 zlgsendcan-1.1.7/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 02:43:14.000000 zlgsendcan-1.1.7/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.1.6/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.1.7/zlgsendcan/get_conf_info.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.6/zlgsendcan/parseDBC.py` & `zlgsendcan-1.1.7/zlgsendcan/parseDBC.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
 
 class GlobleValue:
     thread_obj = {}
     global_msg = {}
     global_msg2 = {}
     global_msg3 = {}
-    can_conf={'can_type':'can','chan':0,'zcy':None,'sjy':None}
+    can_conf = {'can_type': 'can', 'chan': 0, 'zcy': None, 'sjy': None}
     zlginit = None
     dbc_path = None
     thread_run = False
     flag_trace = False
     thread_sigchange_flag = False
     data_log = []
     sql_flag = False
```

### Comparing `zlgsendcan-1.1.6/zlgsendcan/yaml_util.py` & `zlgsendcan-1.1.7/zlgsendcan/yaml_util.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.6/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.1.7/zlgsendcan/zlgcan1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,17 @@
-# -*- coding:utf-8 -*-
-#  zlgcan.py
-#
-#  ~~~~~~~~~~~~
-#
-#  ZLGCAN API
-#
-#  ~~~~~~~~~~~~
-#
-#  ------------------------------------------------------------------
-#  Author : guochuangjian    
-#  Last change: 21.02.2019
-#
-#  Language: Python 2.7, 3.6
-#  ------------------------------------------------------------------
-#
 import os
 import re
 import sys
 from ctypes import *
 import platform
 import frozen_dir
 
 SETUP_DIR = frozen_dir.app_path() + r'\zlgcan_1.dll'
 sys.path.append(SETUP_DIR)
-
 ZCAN_DEVICE_TYPE = c_uint
-
 INVALID_DEVICE_HANDLE = 0
 INVALID_CHANNEL_HANDLE = 0
 
 '''
  Device Type
 '''
 ZCAN_PCI5121 = ZCAN_DEVICE_TYPE(1)
@@ -509,14 +491,16 @@
             raise
 
 
 ###############################################################################
 '''
 USBCANFD-MINI Demo
 '''
+
+
 def convert_speed(speed):
     # 通过正则表达式提取数字和单位
     match = re.match(r'(\d+(\.\d+)?)\s*(kbps|Mbps)', speed, re.IGNORECASE)
     if match:
         value = float(match.group(1))  # 提取数值部分
         unit = match.group(3).lower()  # 提取单位并转换为小写
 
@@ -526,14 +510,15 @@
         elif unit == 'mbps':
             value *= 1000000
 
         return str(value)  # 返回转换后的速度值
 
     return None  # 如果无法匹配，则返回None
 
+
 def canfd_start(zcanlib, device_handle, chn, data):
     # init_conf = data['can初始化配置']
     init_conf = data
     ip = zcanlib.GetIProperty(device_handle)
     # if init_conf['仲裁域'][0] == '自定义':
     #     ret = zcanlib.SetValue(ip, str(chn) + "/baud_rate_custom", init_conf['自定义波特率'])
     if init_conf['zcy'] == '自定义':
```

### Comparing `zlgsendcan-1.1.6/zlgsendcan/zlgserver.py` & `zlgsendcan-1.1.7/zlgsendcan/zlgserver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import copy
 import importlib
 import time
 from PyQt5.QtWidgets import QMessageBox
-from parseDBC import GlobleValue, DbcInit
+from zlgsendcan.parseDBC import GlobleValue, DbcInit, get_signal_data1
 from zlgsendcan.zlgcan1 import *
 import threading
-from get_conf_info import GetBaseInfo
+from zlgsendcan.get_conf_info import GetBaseInfo
 
 data_ = GetBaseInfo().get_base_config()
 condition = threading.Condition()
 
 
+# 获取dbc文件解析的db对象做成全局变量调用
+def get_dbc_db(dbc_path):
+    GlobleValue.dbc_init = get_signal_data1(dbc_path).db  # 初始化解析dbc文件
+
+
+
 class MessageDate:
-    def __init__(self,can_type,chanl,brate:dict):
+    def __init__(self, can_type, chanl, brate: dict):
         """
 
         :param can_type: 1、can 2、canfd
         :param chanl: 0,1
         :param brate: {'zcy':'500kbps 80%','sjy':'2Mbps 80%‘}注意如果自定义波特率格式如下
                         {'zcy':'自定义','sjy':‘500Kbps(85%),2.0Mbps(80%),(20,00000520,00000106)’}
         """
         GlobleValue.can_conf['chan'] = chanl
         GlobleValue.can_conf['zcy'] = brate['zcy']
         GlobleValue.can_conf['can_type'] = can_type
-        GlobleValue.can_conf['sjy']=brate['sjy']
+        GlobleValue.can_conf['sjy'] = brate['sjy']
 
         self.zcanlib = ZCAN()
         # self.testcantype = 1  # 0:CAN; 1:canfd
         self.handle = self.zcanlib.OpenDevice(ZCAN_USBCANFD_200U, 0, 0)
         if self.handle == INVALID_DEVICE_HANDLE:
             msgbox = QMessageBox(QMessageBox.Critical, '错误', "请检查周立功是否连接或重复开启！")
             msgbox.adjustSize()
@@ -36,15 +42,16 @@
             print("Open CANFD Device failed!")
             # exit(0)
         print("device handle:%d." % (self.handle))
         info = self.zcanlib.GetDeviceInf(self.handle)
         print("Device Information:\n%s" % (info))
 
         # Start CAN
-        self.chn_handle = canfd_start(self.zcanlib, self.handle, int(GlobleValue.can_conf['chan']), GlobleValue.can_conf)
+        self.chn_handle = canfd_start(self.zcanlib, self.handle, int(GlobleValue.can_conf['chan']),
+                                      GlobleValue.can_conf)
         print("channel handle:%d." % (self.chn_handle))
 
     # 检查设备是否在线
     def check_device_online(self):
         return self.zcanlib.DeviceOnLine(self.handle)
 
     def clear_buffer(self):
@@ -97,15 +104,16 @@
         # print('=============',data_len)
         canfd_msgs = (ZCANDataObj * data_len)()
         # memset(byref(canfd_msgs), 0, sizeof(canfd_msgs))
         # canfd_msgs = (ZCAN_TransmitFD_Data * 10)()
         for i in range(data_len):
             canfd_msgs[i].dataType = 1  # can/canfd frame
             canfd_msgs[i].chnl = int(GlobleValue.can_conf['chan'])  # can_channel
-            canfd_msgs[i].zcanfddata.flag.frameType = 1 if GlobleValue.can_conf['can_type'] == 'canfd' else 0  # 0-can,1-canfd
+            canfd_msgs[i].zcanfddata.flag.frameType = 1 if GlobleValue.can_conf[
+                                                               'can_type'] == 'canfd' else 0  # 0-can,1-canfd
             # canfd_msgs[i].zcanfddata.frame.eff = 0
             # canfd_msgs[i].zcanfddata.frame.rtr = 0
             # canfd_msgs[i].zcanfddata.frame.brs = 1
             # canfd_msgs[i].zcanfddata.frame.esi = 0
             # canfd_msgs[i].zcanfddata.frame.__pad = 0x20  # 队列发送，当值为0x20时，单位为ms;  当值为0x30时，单位是100us。
             # canfd_msgs[i].zcanfddata.frame.__res0 = 0x1388  # 帧间隔低位,定时100ms
             # canfd_msgs[i].zcanfddata.frame.__res1 = 0x00  # 帧间隔高位
@@ -125,30 +133,32 @@
 
 # 普通发送
 def canfd_msg_power(idx, data):
     data_ = GetBaseInfo().get_base_config()
     canfd_msgs = (ZCANDataObj * 1)()
     for i in range(1):
         canfd_msgs[i].dataType = 1  # can/canfd frame
-        canfd_msgs[i].chnl = int(GlobleValue.can_conf['chan']) # can_channel
-        canfd_msgs[i].zcanfddata.flag.frameType = 1 if GlobleValue.can_conf['can_type'] == 'canfd' else 0  # 0-can,1-canfd
+        canfd_msgs[i].chnl = int(GlobleValue.can_conf['chan'])  # can_channel
+        canfd_msgs[i].zcanfddata.flag.frameType = 1 if GlobleValue.can_conf[
+                                                           'can_type'] == 'canfd' else 0  # 0-can,1-canfd
         canfd_msgs[i].zcanfddata.flag.txDelay = 0  # 不添加延迟
         canfd_msgs[i].zcanfddata.flag.transmitType = 0  # 发送方式，0-正常发送
         canfd_msgs[i].zcanfddata.flag.txEchoRequest = 1  # 发送回显请求，0-不回显，1-回显
         canfd_msgs[i].zcanfddata.frame.can_id = int(idx, 16)
         canfd_msgs[i].zcanfddata.frame.len = 8
         canfd_msgs[i].zcanfddata.flag.txEchoed = 1  # 0发送txEchoed
         for j in range(8):
             canfd_msgs[i].zcanfddata.frame.data[j] = data[j]
     return canfd_msgs
 
 
 class ZlgSend:
 
     def __init__(self, handle, data, dbc_file, pro_name, is_key=False):
+        GlobleValue.thread_run = True
         if not is_key:
             for k, v in data.items():
                 thread_list = []
                 # for name1, msgdata in data[k].items():
                 if k not in ['cycle_time', 'send_num', 'msg_id', 'is_crc']:
                     ctime = data['cycle_time']
                     sendnum = data['send_num']
@@ -157,15 +167,15 @@
                         if isinstance(sv, dict):
                             sigchange_th = ThreadSingChange()
                             sigchange_th.flag = True
                             exit = threading.Event()
 
                             sig_th = threading.Thread(target=sigchange_th.runn,
                                                       args=(handle, k, v, ctime, sendnum, exit, is_crc, pro_name,
-                                                            dbc_file),daemon=True)
+                                                            dbc_file), daemon=True)
                             sig_th.start()
 
                             thread_list.append(sigchange_th)
                             thread_list.append(sig_th)
                             thread_list.append(exit.isSet())
                             # GlobleValue.thread_obj[k] = thread_list
                             GlobleValue.thread_obj[k] = thread_list
```

