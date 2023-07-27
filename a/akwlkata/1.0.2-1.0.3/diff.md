# Comparing `tmp/akwlkata-1.0.2.tar.gz` & `tmp/akwlkata-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/akwlkata-1.0.2.tar", last modified: Thu Jul 27 06:11:06 2023, max compression
+gzip compressed data, was "dist/akwlkata-1.0.3.tar", last modified: Thu Jul 27 06:14:45 2023, max compression
```

## Comparing `akwlkata-1.0.2.tar` & `akwlkata-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-27 06:11:06.000000 akwlkata-1.0.2/
--rw-r--r--   0 NikkiMac   (501) staff       (20)      303 2023-07-27 06:11:06.000000 akwlkata-1.0.2/PKG-INFO
-drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-27 06:11:06.000000 akwlkata-1.0.2/akwlkata/
--rw-r--r--   0 NikkiMac   (501) staff       (20)    11377 2023-07-27 06:07:38.000000 akwlkata-1.0.2/akwlkata/AKWlkata.py
--rw-r--r--   0 NikkiMac   (501) staff       (20)      252 2023-07-25 07:13:58.000000 akwlkata-1.0.2/akwlkata/__init__.py
-drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-27 06:11:06.000000 akwlkata-1.0.2/akwlkata.egg-info/
--rw-r--r--   0 NikkiMac   (501) staff       (20)      303 2023-07-27 06:11:05.000000 akwlkata-1.0.2/akwlkata.egg-info/PKG-INFO
--rw-r--r--   0 NikkiMac   (501) staff       (20)      209 2023-07-27 06:11:05.000000 akwlkata-1.0.2/akwlkata.egg-info/SOURCES.txt
--rw-r--r--   0 NikkiMac   (501) staff       (20)        1 2023-07-27 06:11:05.000000 akwlkata-1.0.2/akwlkata.egg-info/dependency_links.txt
--rw-r--r--   0 NikkiMac   (501) staff       (20)        9 2023-07-27 06:11:05.000000 akwlkata-1.0.2/akwlkata.egg-info/requires.txt
--rw-r--r--   0 NikkiMac   (501) staff       (20)        9 2023-07-27 06:11:05.000000 akwlkata-1.0.2/akwlkata.egg-info/top_level.txt
--rw-r--r--   0 NikkiMac   (501) staff       (20)       38 2023-07-27 06:11:06.000000 akwlkata-1.0.2/setup.cfg
--rw-r--r--   0 NikkiMac   (501) staff       (20)      798 2023-07-27 06:09:39.000000 akwlkata-1.0.2/setup.py
+drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-27 06:14:45.000000 akwlkata-1.0.3/
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      303 2023-07-27 06:14:45.000000 akwlkata-1.0.3/PKG-INFO
+drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-27 06:14:45.000000 akwlkata-1.0.3/akwlkata/
+-rw-r--r--   0 NikkiMac   (501) staff       (20)    11377 2023-07-27 06:14:21.000000 akwlkata-1.0.3/akwlkata/AKWlkata.py
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      252 2023-07-25 07:13:58.000000 akwlkata-1.0.3/akwlkata/__init__.py
+drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-27 06:14:45.000000 akwlkata-1.0.3/akwlkata.egg-info/
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      303 2023-07-27 06:14:45.000000 akwlkata-1.0.3/akwlkata.egg-info/PKG-INFO
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      209 2023-07-27 06:14:45.000000 akwlkata-1.0.3/akwlkata.egg-info/SOURCES.txt
+-rw-r--r--   0 NikkiMac   (501) staff       (20)        1 2023-07-27 06:14:45.000000 akwlkata-1.0.3/akwlkata.egg-info/dependency_links.txt
+-rw-r--r--   0 NikkiMac   (501) staff       (20)        9 2023-07-27 06:14:45.000000 akwlkata-1.0.3/akwlkata.egg-info/requires.txt
+-rw-r--r--   0 NikkiMac   (501) staff       (20)        9 2023-07-27 06:14:45.000000 akwlkata-1.0.3/akwlkata.egg-info/top_level.txt
+-rw-r--r--   0 NikkiMac   (501) staff       (20)       38 2023-07-27 06:14:45.000000 akwlkata-1.0.3/setup.cfg
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      798 2023-07-27 06:14:27.000000 akwlkata-1.0.3/setup.py
```

### Comparing `akwlkata-1.0.2/akwlkata/AKWlkata.py` & `akwlkata-1.0.3/akwlkata/AKWlkata.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,29 +10,28 @@
     
     @Copyright © 2023年 Mr.Li All rights reserved
 """
 import re
 import time
 import serial
 
-
 INITIAL_TIME = 15
 
 
 class RobotProcessor(object):
     def __init__(self, dev_n, baud_rate=115200, adr=-1):
         self.mirobot_state_all = {"state": "-1",
                                   "angle_A": -1, "angle_B": -1, "angle_C": -1, "angle_D": -1, "angle_X": -1,
                                   "angle_Y": -1,
                                   "angle_Z": -1,
                                   "coordinate_X": -1, "coordinate_Y": -1, "coordinate_Z": -1, "coordinate_RX": -1,
                                   "coordinate_RY": -1, "coordinate_RZ": -1,
                                   "pump": -1,
                                   "valve": -1,
-                                  "mooe": -1}
+                                  "mode": -1}
 
         # 串口对象+地址
         self.pSerial = serial.Serial(dev_n, baud_rate)
         self.address = adr  # -1 RS232; 1 RS485
 
         self.dev_n = dev_n
 
@@ -57,14 +56,15 @@
         elif mirobot_state in ['-1', -1]:
             print('Can Not Find Robot USB: {}'.format(self.dev_n))
             return mirobot_state
 
         # Get Current Version And State
         print('State: {} Version: {}'.format(self.getState(), self.version()))
         return mirobot_state
+
     # 穿透指令
     def sendMsg(self, string):
         if self.address != -1:
             self.string = "@" + str(self.address) + string + "\r\n"
         else:
             self.string = string + "\r\n"
         self.pSerial.write(self.string.encode("utf-8"))
@@ -235,15 +235,15 @@
             self.mirobot_state_all = {"state": " ",
                                       "angle_A": 0, "angle_B": 0, "angle_C": 0, "angle_D": 0, "angle_X": 0,
                                       "angle_Y": 0, "angle_Z": 0,
                                       "coordinate_X": 0, "coordinate_Y": 0, "coordinate_Z": 0, "coordinate_RX": 0,
                                       "coordinate_RY": 0, "coordinate_RZ": 0,
                                       "pump": 0,
                                       "valve": 0,
-                                      "mooe": 0}
+                                      "mode": 0}
 
             self.mirobot_state_all["state"] = match.group(1)
             self.mirobot_state_all["angle_A"] = match.group(2)
             self.mirobot_state_all["angle_B"] = match.group(3)
             self.mirobot_state_all["angle_C"] = match.group(4)
             self.mirobot_state_all["angle_D"] = match.group(5)
             self.mirobot_state_all["angle_X"] = match.group(6)
@@ -253,15 +253,15 @@
             self.mirobot_state_all["coordinate_Y"] = match.group(10)
             self.mirobot_state_all["coordinate_Z"] = match.group(11)
             self.mirobot_state_all["coordinate_RX"] = match.group(12)
             self.mirobot_state_all["coordinate_RY"] = match.group(13)
             self.mirobot_state_all["coordinate_RZ"] = match.group(14)
             self.mirobot_state_all["pump"] = match.group(15)
             self.mirobot_state_all["valve"] = match.group(16)
-            self.mirobot_state_all["mooe"] = match.group(17)
+            self.mirobot_state_all["mode"] = match.group(17)
             return self.mirobot_state_all
         else:
             return "parse error/解析错误"
 
     # 机械臂状态查询
     def getState(self):
         self.getStatus()
@@ -314,10 +314,10 @@
 
     # 夹爪状态查询
     def getvalve(self):
         self.getStatus()
         return self.mirobot_state_all["valve"]
 
     # 运动模式查询
-    def getmooe(self):
+    def getmode(self):
         self.getStatus()
-        return self.mirobot_state_all["mooe"]
+        return self.mirobot_state_all["mode"]
```

### Comparing `akwlkata-1.0.2/setup.py` & `akwlkata-1.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     @Copyright © 2020年 Mr.Li All rights reserved
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="akwlkata",
-    version="1.0.2",
+    version="1.0.3",
     keywords=("pip", "akwlkata", "wlkata", "wlkatarobot", "kuture", "robot"),
     description="wlkata robot driver",
     long_description="开塔机械臂驱动，兼容ubuntu与mac OS，优化控制流程",
     license="MIT Licence",
 
     url="",
     author="Kuture",
```

