# Comparing `tmp/wpcsys-2.1.6.tar.gz` & `tmp/wpcsys-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpcsys-2.1.6.tar", last modified: Tue Jul 18 05:46:27 2023, max compression
+gzip compressed data, was "wpcsys-2.1.7.tar", last modified: Thu Jul 27 07:01:23 2023, max compression
```

## Comparing `wpcsys-2.1.6.tar` & `wpcsys-2.1.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 05:46:27.656314 wpcsys-2.1.6/
--rw-rw-rw-   0        0        0     1091 2022-10-03 09:42:47.000000 wpcsys-2.1.6/LICENSE
--rw-rw-rw-   0        0        0       64 2022-11-04 05:05:00.000000 wpcsys-2.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0    10446 2023-07-18 05:46:27.647318 wpcsys-2.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     9385 2023-07-17 09:03:28.000000 wpcsys-2.1.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-18 05:46:27.656314 wpcsys-2.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1985 2022-11-23 08:57:09.000000 wpcsys-2.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:46:27.592525 wpcsys-2.1.6/wpcsys/
--rw-rw-rw-   0        0        0        0 2022-10-06 03:03:31.000000 wpcsys-2.1.6/wpcsys/__init__.py
--rw-rw-rw-   0        0        0  1292959 2023-02-08 04:26:34.000000 wpcsys-2.1.6/wpcsys/libusb-1.0.dll
--rw-rw-rw-   0        0        0  7585280 2023-07-18 05:42:14.000000 wpcsys-2.1.6/wpcsys/pywpc.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0  8171520 2023-07-18 05:43:53.000000 wpcsys-2.1.6/wpcsys/pywpc.cp38-win_amd64.pyd
--rw-rw-rw-   0        0        0  8180224 2023-07-18 05:43:11.000000 wpcsys-2.1.6/wpcsys/pywpc.cp39-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2023-07-18 05:46:27.645338 wpcsys-2.1.6/wpcsys.egg-info/
--rw-rw-rw-   0        0        0    10446 2023-07-18 05:46:27.000000 wpcsys-2.1.6/wpcsys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-07-18 05:46:27.000000 wpcsys-2.1.6/wpcsys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 05:46:27.000000 wpcsys-2.1.6/wpcsys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2023-07-18 05:46:27.000000 wpcsys-2.1.6/wpcsys.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-18 05:46:27.000000 wpcsys-2.1.6/wpcsys.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 07:01:23.951336 wpcsys-2.1.7/
+-rw-rw-rw-   0        0        0     1091 2022-10-03 09:42:47.000000 wpcsys-2.1.7/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-11-04 05:05:00.000000 wpcsys-2.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    10345 2023-07-27 07:01:23.943330 wpcsys-2.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     9284 2023-07-27 04:47:23.000000 wpcsys-2.1.7/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-27 07:01:23.951336 wpcsys-2.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     2138 2023-07-27 04:32:46.000000 wpcsys-2.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:01:23.909185 wpcsys-2.1.7/wpcsys/
+-rw-rw-rw-   0        0        0        0 2022-10-06 03:03:31.000000 wpcsys-2.1.7/wpcsys/__init__.py
+-rw-rw-rw-   0        0        0  1292959 2023-02-08 04:26:34.000000 wpcsys-2.1.7/wpcsys/libusb-1.0.dll
+-rw-rw-rw-   0        0        0  7585280 2023-07-27 06:48:08.000000 wpcsys-2.1.7/wpcsys/pywpc.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0  8171520 2023-07-27 07:00:23.000000 wpcsys-2.1.7/wpcsys/pywpc.cp38-win_amd64.pyd
+-rw-rw-rw-   0        0        0  8180224 2023-07-27 06:59:21.000000 wpcsys-2.1.7/wpcsys/pywpc.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0       17 2023-07-27 04:53:27.000000 wpcsys-2.1.7/wpcsys/version.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:01:23.940385 wpcsys-2.1.7/wpcsys.egg-info/
+-rw-rw-rw-   0        0        0    10345 2023-07-27 07:01:23.000000 wpcsys-2.1.7/wpcsys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-07-27 07:01:23.000000 wpcsys-2.1.7/wpcsys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 07:01:23.000000 wpcsys-2.1.7/wpcsys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-07-27 07:01:23.000000 wpcsys-2.1.7/wpcsys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 07:01:23.000000 wpcsys-2.1.7/wpcsys.egg-info/top_level.txt
```

### Comparing `wpcsys-2.1.6/LICENSE` & `wpcsys-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.6/PKG-INFO` & `wpcsys-2.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpcsys
-Version: 2.1.6
+Version: 2.1.7
 Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
 Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
 Author: chunglee_people, Chieh-An Lin
 Author-email: wu@wpc.com.tw
 License: MIT
 Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,15 +34,15 @@
 
 Asynchronous mode means that processes run independently of each other and don't wait for the completion of the previous process. Instead, each process runs on its own, without blocking the execution of other processes.
 
 In general, synchronous mode is easier to understand and debug, while asynchronous mode is more scalable and allows for greater concurrency.
 
 Some API functions in the `pywpc` package may not compatible with earlier versions of WPC DAQ firmware.
 To update device firmware to the latest version, please use WPC Device Manager and `LabVIEW Run-time engine <https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view>`_.
-You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.6>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
+You can download WPC Device Manager by visiting `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
 
 +-------------------+-----------------------------------------------------------------------------------+
 |                   | Link                                                                              |
 +===================+===================================================================================+
 | WPC official site | http://www.wpc.com.tw/                                                            |
 +-------------------+-----------------------------------------------------------------------------------+
 | GitHub            | https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release                      |
```

### Comparing `wpcsys-2.1.6/README.rst` & `wpcsys-2.1.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Asynchronous mode means that processes run independently of each other and don't wait for the completion of the previous process. Instead, each process runs on its own, without blocking the execution of other processes.
 
 In general, synchronous mode is easier to understand and debug, while asynchronous mode is more scalable and allows for greater concurrency.
 
 Some API functions in the `pywpc` package may not compatible with earlier versions of WPC DAQ firmware.
 To update device firmware to the latest version, please use WPC Device Manager and `LabVIEW Run-time engine <https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view>`_.
-You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.6>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
+You can download WPC Device Manager by visiting `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
 
 +-------------------+-----------------------------------------------------------------------------------+
 |                   | Link                                                                              |
 +===================+===================================================================================+
 | WPC official site | http://www.wpc.com.tw/                                                            |
 +-------------------+-----------------------------------------------------------------------------------+
 | GitHub            | https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release                      |
```

### Comparing `wpcsys-2.1.6/setup.py` & `wpcsys-2.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 
 ## Python
 import sys
 import setuptools as sut
 
 ## WPC
 sys.path.append('wpcsys/')
-import pywpc
+
+ # --- get version ---
+version = "unknown"
+with open("wpcsys/version.py") as f:
+    line = f.read().strip()
+    version = line.replace("version = ", "").replace('"', '')
 
 class BinaryDistribution(sut.dist.Distribution):
     """Distribution which always forces a binary package with platform name"""
     def has_ext_modules(x):
         return True
 
 with open("README.rst", "r", encoding="utf-8") as fh:
@@ -22,15 +27,15 @@
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     install_requires = fh.readlines()
     install_requires = [str_.rstrip(' \n') for str_ in install_requires]
 
 sut.setup(
     name="wpcsys",
-    version=pywpc.__version__,
+    version=version,
     description='WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)',
     long_description=long_description,
     long_description_content_type='text/x-rst',
 
     author="chunglee_people, Chieh-An Lin",
     author_email="wu@wpc.com.tw",
     url="https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release",
```

### Comparing `wpcsys-2.1.6/wpcsys/libusb-1.0.dll` & `wpcsys-2.1.7/wpcsys/libusb-1.0.dll`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.6/wpcsys.egg-info/PKG-INFO` & `wpcsys-2.1.7/wpcsys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpcsys
-Version: 2.1.6
+Version: 2.1.7
 Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
 Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
 Author: chunglee_people, Chieh-An Lin
 Author-email: wu@wpc.com.tw
 License: MIT
 Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,15 +34,15 @@
 
 Asynchronous mode means that processes run independently of each other and don't wait for the completion of the previous process. Instead, each process runs on its own, without blocking the execution of other processes.
 
 In general, synchronous mode is easier to understand and debug, while asynchronous mode is more scalable and allows for greater concurrency.
 
 Some API functions in the `pywpc` package may not compatible with earlier versions of WPC DAQ firmware.
 To update device firmware to the latest version, please use WPC Device Manager and `LabVIEW Run-time engine <https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view>`_.
-You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.6>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
+You can download WPC Device Manager by visiting `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
 
 +-------------------+-----------------------------------------------------------------------------------+
 |                   | Link                                                                              |
 +===================+===================================================================================+
 | WPC official site | http://www.wpc.com.tw/                                                            |
 +-------------------+-----------------------------------------------------------------------------------+
 | GitHub            | https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release                      |
```

