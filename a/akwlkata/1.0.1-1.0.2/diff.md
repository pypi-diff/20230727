# Comparing `tmp/akwlkata-1.0.1.tar.gz` & `tmp/akwlkata-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/akwlkata-1.0.1.tar", last modified: Tue Jul 25 07:58:22 2023, max compression
+gzip compressed data, was "dist/akwlkata-1.0.2.tar", last modified: Thu Jul 27 06:11:06 2023, max compression
```

## Comparing `akwlkata-1.0.1.tar` & `akwlkata-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-25 07:58:22.000000 akwlkata-1.0.1/
--rw-r--r--   0 NikkiMac   (501) staff       (20)      282 2023-07-25 07:58:22.000000 akwlkata-1.0.1/PKG-INFO
-drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata/
--rw-r--r--   0 NikkiMac   (501) staff       (20)    11100 2023-07-25 07:38:49.000000 akwlkata-1.0.1/akwlkata/AKWlkata.py
--rw-r--r--   0 NikkiMac   (501) staff       (20)      252 2023-07-25 07:13:58.000000 akwlkata-1.0.1/akwlkata/__init__.py
-drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata.egg-info/
--rw-r--r--   0 NikkiMac   (501) staff       (20)      282 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata.egg-info/PKG-INFO
--rw-r--r--   0 NikkiMac   (501) staff       (20)      209 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata.egg-info/SOURCES.txt
--rw-r--r--   0 NikkiMac   (501) staff       (20)        1 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata.egg-info/dependency_links.txt
--rw-r--r--   0 NikkiMac   (501) staff       (20)        9 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata.egg-info/requires.txt
--rw-r--r--   0 NikkiMac   (501) staff       (20)        9 2023-07-25 07:58:22.000000 akwlkata-1.0.1/akwlkata.egg-info/top_level.txt
--rw-r--r--   0 NikkiMac   (501) staff       (20)       38 2023-07-25 07:58:22.000000 akwlkata-1.0.1/setup.cfg
--rw-r--r--   0 NikkiMac   (501) staff       (20)      777 2023-07-25 07:58:21.000000 akwlkata-1.0.1/setup.py
+drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-27 06:11:06.000000 akwlkata-1.0.2/
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      303 2023-07-27 06:11:06.000000 akwlkata-1.0.2/PKG-INFO
+drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-27 06:11:06.000000 akwlkata-1.0.2/akwlkata/
+-rw-r--r--   0 NikkiMac   (501) staff       (20)    11377 2023-07-27 06:07:38.000000 akwlkata-1.0.2/akwlkata/AKWlkata.py
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      252 2023-07-25 07:13:58.000000 akwlkata-1.0.2/akwlkata/__init__.py
+drwxr-xr-x   0 NikkiMac   (501) staff       (20)        0 2023-07-27 06:11:06.000000 akwlkata-1.0.2/akwlkata.egg-info/
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      303 2023-07-27 06:11:05.000000 akwlkata-1.0.2/akwlkata.egg-info/PKG-INFO
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      209 2023-07-27 06:11:05.000000 akwlkata-1.0.2/akwlkata.egg-info/SOURCES.txt
+-rw-r--r--   0 NikkiMac   (501) staff       (20)        1 2023-07-27 06:11:05.000000 akwlkata-1.0.2/akwlkata.egg-info/dependency_links.txt
+-rw-r--r--   0 NikkiMac   (501) staff       (20)        9 2023-07-27 06:11:05.000000 akwlkata-1.0.2/akwlkata.egg-info/requires.txt
+-rw-r--r--   0 NikkiMac   (501) staff       (20)        9 2023-07-27 06:11:05.000000 akwlkata-1.0.2/akwlkata.egg-info/top_level.txt
+-rw-r--r--   0 NikkiMac   (501) staff       (20)       38 2023-07-27 06:11:06.000000 akwlkata-1.0.2/setup.cfg
+-rw-r--r--   0 NikkiMac   (501) staff       (20)      798 2023-07-27 06:09:39.000000 akwlkata-1.0.2/setup.py
```

### Comparing `akwlkata-1.0.1/akwlkata/AKWlkata.py` & `akwlkata-1.0.2/akwlkata/AKWlkata.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,34 +30,41 @@
                                   "valve": -1,
                                   "mooe": -1}
 
         # 串口对象+地址
         self.pSerial = serial.Serial(dev_n, baud_rate)
         self.address = adr  # -1 RS232; 1 RS485
 
-        # Initial Arm State
-        self.arm_init()
+        self.dev_n = dev_n
+
+        # # Initial Robot State
+        self.robot_state = self.arm_init()
 
     # 机械臂状态判断与初始化
     def arm_init(self):
 
         mirobot_state = self.getState()
+        print('Check State: {}'.format(mirobot_state))
+
         if mirobot_state in ['Alarm', 'Hold']:
             print('Controller State: {}, Initial...'.format(mirobot_state))
             if mirobot_state == 'Hold':
                 self.sendMsg('~')  # 检测到机械臂为Hold 状态时继续运行
                 self.homing()
                 time.sleep(INITIAL_TIME)
             else:
                 self.homing()
                 time.sleep(INITIAL_TIME)
+        elif mirobot_state in ['-1', -1]:
+            print('Can Not Find Robot USB: {}'.format(self.dev_n))
+            return mirobot_state
 
         # Get Current Version And State
         print('State: {} Version: {}'.format(self.getState(), self.version()))
-
+        return mirobot_state
     # 穿透指令
     def sendMsg(self, string):
         if self.address != -1:
             self.string = "@" + str(self.address) + string + "\r\n"
         else:
             self.string = string + "\r\n"
         self.pSerial.write(self.string.encode("utf-8"))
```

### Comparing `akwlkata-1.0.1/setup.py` & `akwlkata-1.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     @Copyright © 2020年 Mr.Li All rights reserved
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="akwlkata",
-    version="1.0.1",
+    version="1.0.2",
     keywords=("pip", "akwlkata", "wlkata", "wlkatarobot", "kuture", "robot"),
     description="wlkata robot driver",
-    long_description="开塔机械臂驱动，兼容ubuntu与mac OS",
+    long_description="开塔机械臂驱动，兼容ubuntu与mac OS，优化控制流程",
     license="MIT Licence",
 
     url="",
     author="Kuture",
     author_email="kuture@163.com",
 
     packages=find_packages(),
```

