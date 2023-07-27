# Comparing `tmp/zlgsendcan-1.1.8.tar.gz` & `tmp/zlgsendcan-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.1.8.tar", last modified: Thu Jul 27 03:06:31 2023, max compression
+gzip compressed data, was "zlgsendcan-1.1.9.tar", last modified: Thu Jul 27 03:42:11 2023, max compression
```

## Comparing `zlgsendcan-1.1.8.tar` & `zlgsendcan-1.1.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 03:06:31.477833 zlgsendcan-1.1.8/
--rw-rw-rw-   0        0        0      221 2023-07-27 03:06:31.477833 zlgsendcan-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-27 03:06:31.477833 zlgsendcan-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-07-27 03:06:04.000000 zlgsendcan-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 03:06:31.477833 zlgsendcan-1.1.8/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.8/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.8/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.8/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5271 2023-07-27 02:13:20.000000 zlgsendcan-1.1.8/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.8/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    25691 2023-07-27 02:13:20.000000 zlgsendcan-1.1.8/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    19137 2023-07-27 02:58:24.000000 zlgsendcan-1.1.8/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-27 03:06:31.477833 zlgsendcan-1.1.8/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      221 2023-07-27 03:06:31.000000 zlgsendcan-1.1.8/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-27 03:06:31.000000 zlgsendcan-1.1.8/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 03:06:31.000000 zlgsendcan-1.1.8/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-27 03:06:31.000000 zlgsendcan-1.1.8/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-27 03:06:31.000000 zlgsendcan-1.1.8/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 03:42:11.097802 zlgsendcan-1.1.9/
+-rw-rw-rw-   0        0        0      221 2023-07-27 03:42:11.097802 zlgsendcan-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-27 03:42:11.097802 zlgsendcan-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-07-27 03:36:37.000000 zlgsendcan-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:42:11.097802 zlgsendcan-1.1.9/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.9/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0     1998 2023-07-27 03:41:41.000000 zlgsendcan-1.1.9/zlgsendcan/example_test.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.9/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.9/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5271 2023-07-27 02:13:20.000000 zlgsendcan-1.1.9/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.9/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    25691 2023-07-27 02:13:20.000000 zlgsendcan-1.1.9/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    19391 2023-07-27 03:26:06.000000 zlgsendcan-1.1.9/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:42:11.097802 zlgsendcan-1.1.9/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-07-27 03:42:10.000000 zlgsendcan-1.1.9/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-07-27 03:42:11.000000 zlgsendcan-1.1.9/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 03:42:10.000000 zlgsendcan-1.1.9/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-27 03:42:10.000000 zlgsendcan-1.1.9/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 03:42:10.000000 zlgsendcan-1.1.9/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.1.8/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.1.9/zlgsendcan/get_conf_info.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.8/zlgsendcan/parseDBC.py` & `zlgsendcan-1.1.9/zlgsendcan/parseDBC.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.8/zlgsendcan/yaml_util.py` & `zlgsendcan-1.1.9/zlgsendcan/yaml_util.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.8/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.1.9/zlgsendcan/zlgcan1.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.8/zlgsendcan/zlgserver.py` & `zlgsendcan-1.1.9/zlgsendcan/zlgserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,19 +147,18 @@
 class ZlgSend:
 
     def __init__(self, handle, data, dbc_file, pro_name=None, is_key=False):
         GlobleValue.thread_run = True
         if not is_key:
             for k, v in data.items():
                 thread_list = []
-                # for name1, msgdata in data[k].items():
                 if k not in ['cycle_time', 'send_num', 'msg_id', 'is_crc']:
-                    ctime = data['cycle_time']
+                    ctime = data.get('cycle_time')
                     sendnum = data['send_num']
-                    is_crc = data['is_crc']
+                    is_crc = '0' if data.get('is_crc') is None else data.get('is_crc')
                     for sn, sv in v.items():
                         if isinstance(sv, dict):
                             sigchange_th = ThreadSingChange()
                             sigchange_th.flag = True
                             exit = threading.Event()
 
                             sig_th = threading.Thread(target=sigchange_th.runn,
@@ -253,15 +252,18 @@
                 if isinstance(sv, dict):
                     ob = DbcInit(k, v, db_obj=GlobleValue.dbc_init)
                     # ob.crc = True if is_crc == '1' else False
                     # ob.pro_name = pro_name
                     step_value = float(sv['步长'])
                     min_value = float(sv['最小值'])
                     max_value = float(sv['最大值'])
-                    a = int(ctime) if ctime != 'null' else 0
+                    if ctime is None:
+                        a = ob.message_cycle_time
+                    else:
+                        a = int(ctime) if ctime != 'null' else 0
                     f = 0
                     c = 0
                     while GlobleValue.thread_run and self.flag:
                         v[sk] = min_value
                         if sendnnum != '-1':
                             if f <= int(sendnnum):
                                 f += 1
@@ -367,15 +369,18 @@
             while GlobleValue.thread_run and self.flag:
                 try:
                     # if self.update:
                     #     ob1.clear_buffer()
                     #     self.update = False
                     for t in range(self.data_len):
                         ret = ob1.zcanlib.TransmitData(ob1.chn_handle, self.data[t], 1)
-                        self.a = int(self.ctime) if self.ctime != 'null' else 0
+                        if self.ctime is None:
+                            self.a = ob1.message_cycle_time
+                        else:
+                            self.a = int(self.ctime) if self.ctime != 'null' else 0
                         time.sleep(self.a / 1000)
                     else:
                         if self.sendnnum != '-1':
                             for i in range(int(self.sendnnum)):
                                 ret = ob1.zcanlib.TransmitData(ob1.chn_handle, self.data[t], 1)
                                 time.sleep(self.a / 1000)
                             # print("Tranmit CANFD Num: %d." % ret)
```

