# Comparing `tmp/gps_sentences-0.1.0.tar.gz` & `tmp/gps_sentences-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gps_sentences-0.1.0.tar", last modified: Fri Jul 14 21:13:21 2023, max compression
+gzip compressed data, was "gps_sentences-0.1.2.tar", last modified: Thu Jul 27 18:40:59 2023, max compression
```

## Comparing `gps_sentences-0.1.0.tar` & `gps_sentences-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-14 21:13:21.080586 gps_sentences-0.1.0/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      123 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/.gitignore
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      939 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/CHANGELOG.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-07-13 21:25:53.000000 gps_sentences-0.1.0/LICENSE.rst
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4283 2023-07-14 21:13:21.080586 gps_sentences-0.1.0/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3739 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/README.md
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-14 21:13:21.077253 gps_sentences-0.1.0/gps_sentences.egg-info/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4283 2023-07-14 21:13:21.000000 gps_sentences-0.1.0/gps_sentences.egg-info/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      655 2023-07-14 21:13:21.000000 gps_sentences-0.1.0/gps_sentences.egg-info/SOURCES.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-07-14 21:13:21.000000 gps_sentences-0.1.0/gps_sentences.egg-info/dependency_links.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       34 2023-07-14 21:13:21.000000 gps_sentences-0.1.0/gps_sentences.egg-info/entry_points.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      483 2023-07-14 21:13:21.000000 gps_sentences-0.1.0/gps_sentences.egg-info/requires.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       14 2023-07-14 21:13:21.000000 gps_sentences-0.1.0/gps_sentences.egg-info/top_level.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1150 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/pyproject.toml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      420 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/requirements.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-07-14 21:13:21.080586 gps_sentences-0.1.0/setup.cfg
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-14 21:13:21.077253 gps_sentences-0.1.0/src/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 21:25:53.000000 gps_sentences-0.1.0/src/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-14 21:13:21.077253 gps_sentences-0.1.0/src/helpers/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 21:25:53.000000 gps_sentences-0.1.0/src/helpers/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9865 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/src/helpers/helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-14 21:13:21.077253 gps_sentences-0.1.0/src/helpers/json_dumps/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/src/helpers/json_dumps/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      438 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/src/helpers/json_dumps/json_dump_alt.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      510 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/src/helpers/json_dumps/json_dump_date.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      660 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/src/helpers/json_dumps/json_dump_lat_long.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      445 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/src/helpers/json_dumps/json_dump_utctime.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1457 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/src/helpers/serial_run.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1766 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/src/main.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-14 21:13:21.080586 gps_sentences-0.1.0/src/tests/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-13 21:25:53.000000 gps_sentences-0.1.0/src/tests/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3520 2023-07-14 21:12:14.000000 gps_sentences-0.1.0/src/tests/test_helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-27 18:40:59.563907 gps_sentences-0.1.2/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      123 2023-07-26 13:49:52.000000 gps_sentences-0.1.2/.gitignore
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1399 2023-07-27 18:26:15.000000 gps_sentences-0.1.2/CHANGELOG.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-07-26 13:49:52.000000 gps_sentences-0.1.2/LICENSE.rst
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4283 2023-07-27 18:40:59.563907 gps_sentences-0.1.2/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3739 2023-07-26 13:49:52.000000 gps_sentences-0.1.2/README.md
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-27 18:40:59.563907 gps_sentences-0.1.2/gps_sentences.egg-info/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4283 2023-07-27 18:40:59.000000 gps_sentences-0.1.2/gps_sentences.egg-info/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      668 2023-07-27 18:40:59.000000 gps_sentences-0.1.2/gps_sentences.egg-info/SOURCES.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-07-27 18:40:59.000000 gps_sentences-0.1.2/gps_sentences.egg-info/dependency_links.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       34 2023-07-27 18:40:59.000000 gps_sentences-0.1.2/gps_sentences.egg-info/entry_points.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      570 2023-07-27 18:40:59.000000 gps_sentences-0.1.2/gps_sentences.egg-info/requires.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       14 2023-07-27 18:40:59.000000 gps_sentences-0.1.2/gps_sentences.egg-info/top_level.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      367 2023-07-27 17:27:36.000000 gps_sentences-0.1.2/logging.conf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1150 2023-07-26 13:49:52.000000 gps_sentences-0.1.2/pyproject.toml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      507 2023-07-27 18:39:45.000000 gps_sentences-0.1.2/requirements.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-07-27 18:40:59.563907 gps_sentences-0.1.2/setup.cfg
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-27 18:40:59.563907 gps_sentences-0.1.2/src/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-26 13:49:52.000000 gps_sentences-0.1.2/src/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-27 18:40:59.563907 gps_sentences-0.1.2/src/helpers/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-26 13:49:52.000000 gps_sentences-0.1.2/src/helpers/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    11014 2023-07-27 18:17:11.000000 gps_sentences-0.1.2/src/helpers/helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-27 18:40:59.563907 gps_sentences-0.1.2/src/helpers/json_dumps/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-26 13:49:52.000000 gps_sentences-0.1.2/src/helpers/json_dumps/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      556 2023-07-27 18:16:48.000000 gps_sentences-0.1.2/src/helpers/json_dumps/json_dump_alt.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      477 2023-07-27 18:18:29.000000 gps_sentences-0.1.2/src/helpers/json_dumps/json_dump_date.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      812 2023-07-27 18:16:48.000000 gps_sentences-0.1.2/src/helpers/json_dumps/json_dump_lat_long.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      574 2023-07-27 18:16:48.000000 gps_sentences-0.1.2/src/helpers/json_dumps/json_dump_utctime.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1601 2023-07-27 18:16:48.000000 gps_sentences-0.1.2/src/helpers/serial_run.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2881 2023-07-27 18:17:02.000000 gps_sentences-0.1.2/src/main.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-27 18:40:59.563907 gps_sentences-0.1.2/src/tests/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-26 13:49:52.000000 gps_sentences-0.1.2/src/tests/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     5043 2023-07-27 18:16:48.000000 gps_sentences-0.1.2/src/tests/test_helpers.py
```

### Comparing `gps_sentences-0.1.0/CHANGELOG.md` & `gps_sentences-0.1.2/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -17,12 +17,24 @@
 ⭐ MAJOR version when you make incompatible API changes,
 
 ✴️ MINOR version when you add functionality in a backwards compatible manner
 
 ✳️ PATCH version when you make backwards compatible bug fixes.
 
 -------------------------------------------------------------------------------
+✴️ [0.1.2] -2023 JUL 27
+- Reformatted the code to be more readable.
+- Added more log statements to the code, to provide more information to the user.
+- Updated the requirements.txt, as well as the README.md.
+- Updated the changelog.
 
-⭐ [0.1.0] - 2023 JUL 23
+✳️ [0.1.1] -2023 JUL 18
+- Can now catch the error that is encounted when no GPS device is plugged in to the terminal.
+- Updated the requirements.txt to reflect new colored print statements.
+- Updated the changelog.
+
+⭐ [0.1.0] - 2023 JUL 13
 - MVP (Minimum Viable Product) has been created.
 - This current version of the product can obtain the altitude, latitude and longitude, utc time, and date and time in your time zone, from information found from the serial connection with the GPS reciever.
-- Changelog created.
+- Changelog created.
+
+
```

### Comparing `gps_sentences-0.1.0/LICENSE.rst` & `gps_sentences-0.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gps_sentences-0.1.0/PKG-INFO` & `gps_sentences-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gps_sentences
-Version: 0.1.0
+Version: 0.1.2
 Summary: Package for reading GPS sentences from a serial port, and decoding them into a usable format.
 Author-email: "Battieste, Nahjay" <nahjaybattieste@gmail.com>
 Project-URL: Source, https://github.com/cellantenna/gps_sentences
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

### Comparing `gps_sentences-0.1.0/README.md` & `gps_sentences-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gps_sentences-0.1.0/gps_sentences.egg-info/PKG-INFO` & `gps_sentences-0.1.2/gps_sentences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gps-sentences
-Version: 0.1.0
+Version: 0.1.2
 Summary: Package for reading GPS sentences from a serial port, and decoding them into a usable format.
 Author-email: "Battieste, Nahjay" <nahjaybattieste@gmail.com>
 Project-URL: Source, https://github.com/cellantenna/gps_sentences
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

### Comparing `gps_sentences-0.1.0/gps_sentences.egg-info/SOURCES.txt` & `gps_sentences-0.1.2/gps_sentences.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 CHANGELOG.md
 LICENSE.rst
 README.md
+logging.conf
 pyproject.toml
 requirements.txt
 gps_sentences.egg-info/PKG-INFO
 gps_sentences.egg-info/SOURCES.txt
 gps_sentences.egg-info/dependency_links.txt
 gps_sentences.egg-info/entry_points.txt
 gps_sentences.egg-info/requires.txt
```

### Comparing `gps_sentences-0.1.0/pyproject.toml` & `gps_sentences-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gps_sentences-0.1.0/src/helpers/helpers.py` & `gps_sentences-0.1.2/src/helpers/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """ a helpers file to provide functions to the main program """
 
 import serial
-import sys
-import glob
 import logging
 import pathlib
 import time
 import datetime
 import platform
 import subprocess
 
@@ -30,15 +28,16 @@
 def device_names() -> list[str]:
     """Use a bash script to list connected microarchitectures."""
     if platform.system().lower != "windows":
         # Avoid crashing program if there are no devices detected
         try:
             listing_script = [
                 # f'#!/bin/bash\n'
-                f'for sysdevpath in $(find /sys/bus/usb/devices/usb*/ -name dev | grep "ACM"); do\n'
+                f"for sysdevpath in $(find /sys/bus/usb/devices/usb*/ "
+                f'-name dev | grep "ACM"); do\n'
                 f'(syspath={"${sysdevpath%/dev}"}\n'
                 f'devname={"$(udevadm info -q name -p $syspath)"}\n'
                 f'[[ {"$devname"} == "bus/"* ]] && exit\n'
                 f'eval "$(udevadm info -q property --export -p $syspath)"\n'
                 f'[[ -z "$ID_SERIAL" ]] && exit\n'
                 f'echo "/dev/$devname - $ID_SERIAL"\n'
                 f") done"
@@ -49,114 +48,144 @@
                 stdout=subprocess.PIPE,
                 text=True,
                 encoding="utf-8",
                 capture_output=False,
                 check=True,
             )
         except TypeError:
-            logger.warning(
-                msg=f"No devices detected | {device_names.__name__}")
+            logger.warning(msg=f"No devices detected | {device_names.__name__}")
             devices = subprocess.CompletedProcess(
                 args="",
                 returncode=1,
                 stdout="",
                 stderr="",
             )
 
     _devices: list = list(
-        devices.stdout.strip().split(sep="\n")) # type: ignore  
+        devices.stdout.strip().split(sep="\n"))  # type: ignore
 
     logger.info(msg=f"Devices found: {_devices} | {device_names.__name__}")
 
     # If there is only one device skip the hooplah
     if len(_devices) == 1:
         return _devices
     return sorted(_devices)
 
 
 DEVICE: list[str] = device_names()
 
 
-def return_device_info(device_list: list[str] = DEVICE, device_to_find: str = "GPS", path_to_find: str = "dev") -> dict[str, str] | str:
+def return_device_info(
+    device_list: list[str] = DEVICE,
+    device_to_find: str = "GPS",
+    path_to_find: str = "dev",
+) -> dict[str, str] | str:
     """Return the device path and serial of the name Teensy."""
     teensy_info: dict[str, str] = {}
 
     # Initial process the device names
     devices = [device.split(sep="_") for device in device_list]
 
     # filter and return only specified devices
+
     desired_device = [i for i in devices if device_to_find in i]
-    intended_device_path = desired_device[0]
-    path = intended_device_path[0]
-    path_try = path.split(sep="-")[0]
-    path_corrected = path_try[:-1]
-    path_type_corrected = str(path_corrected)
+    if not len(desired_device):
+        logger.error(
+            """Device not found. Ensure your GPS 
+            device is plugged into the serial port."""
+        )
+        logger.error(
+            """Index Error has been triggered. No GPS device is plugged in 
+            or the device is not being detected from the serial port."""
+        )
+        exit()
+    else:
+        intended_device_path = desired_device[0]
+        path = intended_device_path[0]
+        path_try = path.split(sep="-")[0]
+        path_corrected = path_try[:-1]
+        path_type_corrected = str(path_corrected)
+        logger.info(path_type_corrected)
+        logger.debug("GPS device information has been found.")
 
     # Create the dictionary of the Teensy path and serial number
     for _i, val in enumerate(desired_device):
         teensy_info[val[-1]] = val[0].split(sep="-")[0]
 
     # if teensy_info == {}:
     #     loggey.error(msg="No Teensy device found")
     #     return {"0": "0"}
 
     return teensy_info if device_to_find != "GPS" else path_type_corrected
 
 
-""" Creation of the variable that is used to store the path to the GPS device. """
+"""Creation of the variable that is used to store the path to the GPS device"""
 corret_path = return_device_info()
 
 
 def time_zone() -> str:
-    """ Creation of the method that is used to display the time zone. """
-    logger.info("Displaying time zone function is in use")
+    """Creation of the method that is used to display the time zone."""
+    logger.debug("Displaying time zone function is in use")
     y = time.tzname
+    logger.info(y[0])
     return y[0]
 
 
 def local_time() -> str:
-    """ Creation of the method that is used to display the local time. """
+    """Creation of the method that is used to display the local time."""
 
-    logger.info("Displaying local time function is in use")
+    logger.debug("Displaying local time function is in use")
     t = time.localtime()
     current_time = time.strftime("%H:%M:%S", t)
+    logger.info(current_time)
     return current_time
 
 
 def date() -> str:
-    """ Creation of the method that is used to display the date. """
-    logger.info("Displaying date function is in use")
+    """Creation of the method that is used to display the date."""
+    logger.debug("Displaying date function is in use")
     today = datetime.date.today()
+    logger.info(today)
     return today.strftime("%d-%b-%y")
 
 
 class NMEASerialReader:
-    """ Creation of the class and class variable that is used to read the serial data from the serial port. """
+    """Creation of the class and class variable that is
+    used to read the serial data from the serial port."""
 
     _port_info_corrected = corret_path
     logger.info(_port_info_corrected)
+    logger.debug("Serial reader class has been called")
 
     def __init__(self) -> None:
-        """ Creation of the constructor that is used to initialize the serial port. """
+        """Creation of the constructor that
+        is used to initialize the serial port."""
         self.ser = serial.Serial(
-            str(NMEASerialReader._port_info_corrected), baudrate=9600, timeout=5)
+            str(NMEASerialReader._port_info_corrected), baudrate=9600, timeout=5
+        )
 
     @classmethod
     def change_to_list(cls, string: str) -> list:
-        """ Creation of the classmethod that is used to later convert a string to a list for later implementation with spaces being the delimitter. """
+        """Creation of the classmethod that is used to later convert a
+        string to a list for later implementation with
+        spaces being the delimitter."""
 
-        logger.info("Conversion to string function is in use")
+        logger.debug("Conversion to string function is in use")
         li = list(string.split(","))
+        logger.info(li)
         return li
 
     @classmethod
     def read_all(cls) -> list:
-        """ Creation of the classmethod that is used to read all the data from the serial port. """
+        """Creation of the classmethod that is used
+        to read all the data from the serial port."""
+        logger.debug("Read all function is in use")
         ser = serial.Serial(
-            f"{NMEASerialReader._port_info_corrected}", baudrate=9600, timeout=5)
+            f"{NMEASerialReader._port_info_corrected}", baudrate=9600, timeout=5
+        )
         # read all the data from the serial port and store it in a list of strings
         data = ser.readline()
         store = []
         while True:
             data_type_corrected = str(data)
             data_corrected = data_type_corrected[2:-5]
             data = ser.readline()
@@ -167,99 +196,113 @@
                 store_list = NMEASerialReader.change_to_list(store_corrected)
                 logger.info(store_corrected)
                 break
         return store_list
 
 
 class NMEASerialDecode(NMEASerialReader):
-
     def __init__(self) -> None:
-        """ Creation of the constructor that is used to initialize the decoding of the serial port. """
+        """Creation of the constructor that is
+        used to initialize the decoding of the serial port."""
         self.ser = serial.Serial(
-            str(NMEASerialReader._port_info_corrected), baudrate=9600, timeout=5)
+            str(NMEASerialReader._port_info_corrected), baudrate=9600, timeout=5
+        )
+        logger.debug("Serial decode class has been called")
 
     @classmethod
     def slice_time(cls, utc_time: str) -> str:
-        """ Creation of the classmethod that is used to properly format the UTC time from the serial port. """
+        """Creation of the classmethod that is used
+        to properly format the UTC time from the serial port."""
+        logger.debug("Slicing time function is in use")
         string = str(utc_time)
         time1 = string[0:2]
         time2 = string[2:4]
         time3 = string[4:6]
         joined_time = f"{time1}:{time2}:{time3}"
+        logger.info(joined_time)
         return joined_time
 
     @classmethod
     def lat_conversion(cls, lat_value: str) -> float:
-        """ Creation of the classmethod that is used to properly convert the latitude from the serial port. """
-        logger.info(
-            "Conversion to lat decimal degrees float function is in use")
+        """Creation of the classmethod that is used
+        to properly convert the latitude from the serial port."""
+        logger.debug("Conversion to lat dec degrees float function is in use")
         try:
             lat_value = str(lat_value)
             first_two_digits = lat_value[0:2]
             remainder = lat_value[2:]
             deg = float(first_two_digits)
             min = float(remainder)
-            decDegrees = float(deg) + float(min/60)
+            decDegrees = float(deg) + float(min / 60)
             decDegrees_rounded = round(decDegrees, 6)
+            logger.info(decDegrees_rounded)
             return decDegrees_rounded
         except ValueError:
             logger.error("Latitude value is not found")
             return 0
 
     @classmethod
     def long_conversion(cls, long_value: str) -> float:
-        """ Creation of the classmethod that is used to properly convert the longitude from the serial port. """
-        logger.info(
-            "Conversion to long decimal degrees float function is in use")
+        """Creation of the classmethod that is used to
+        properly convert the longitude from the serial port."""
+        logger.debug("Conversion to long dec degrees float function is in use")
         try:
             long_value = str(long_value)
             first_three_digits = long_value[0:3]
             remainder = long_value[3:]
             deg = float(first_three_digits)
             min = float(remainder)
-            decDegrees = float(deg) + float(min/60)
+            decDegrees = float(deg) + float(min / 60)
             decDegrees_rounded = round(decDegrees, 6)
+            logger.info(decDegrees_rounded)
             return decDegrees_rounded
         except ValueError:
             logger.error("Longitude value is not found")
             return 0
 
     @classmethod
     def decode_time(cls, nmea_list_sentence: list) -> str:
-        """ Creation of the classmethod that is used to decode the time from the NMEA sentences from the serial port. """
+        """Creation of the classmethod that is used to
+        decode the time from the NMEA sentences from the serial port."""
 
-        logger.info("Decoding time function is in use")
+        logger.debug("Decoding time function is in use")
         time = nmea_list_sentence[1]
         time_type_corrected = str(time)
         time_formatted = time_type_corrected[:-3]
         time_formatted = NMEASerialDecode.slice_time(time_formatted)
+        logger.info(time_formatted)
         return time_formatted
 
     @classmethod
     def decode_alt(cls, nmea_list_sentence: list) -> str:
-        """ Creation of the classmethod that is used to decode the altitude from the NMEA sentences from the serial port. """
+        """Creation of the classmethod that is used to decode
+        the altitude from the NMEA sentences from the serial port."""
 
-        logger.info("Decoding alt function is in use")
+        logger.debug("Decoding alt function is in use")
         alt = nmea_list_sentence[9]
         alt_type_corrected = str(alt)
+        logger.info(alt_type_corrected)
         return alt_type_corrected
 
     @classmethod
     def decode_lat(cls, nmea_list_sentence: list) -> float:
-        """ Creation of the classmethod that is used to decode the latitude from the NMEA sentences from the serial port. """
+        """Creation of the classmethod that is used
+        to decode the latitude from the NMEA sentences from the serial port."""
 
-        logger.info("Decoding lat function is in use")
+        logger.debug("Decoding lat function is in use")
         lat = nmea_list_sentence[2]
         lat_type_corrected = str(lat)
         final_lat_value = NMEASerialDecode.lat_conversion(lat_type_corrected)
+        logger.info(final_lat_value)
         return final_lat_value
 
     @classmethod
     def decode_long(cls, nmea_list_sentence: list) -> float:
-        """ Creation of the classmethod that is used to decode the longitude from the NMEA sentences from the serial port. """
+        """Creation of the classmethod that is used to decode
+        the longitude from the NMEA sentences from the serial port."""
 
-        logger.info("Decoding long function is in use")
+        logger.debug("Decoding long function is in use")
         long = nmea_list_sentence[4]
         long_type_corrected = str(long)
-        final_long_value = NMEASerialDecode.long_conversion(
-            long_type_corrected)
+        final_long_value = NMEASerialDecode.long_conversion(long_type_corrected)
+        logger.info(final_long_value)
         return final_long_value
```

### Comparing `gps_sentences-0.1.0/src/helpers/json_dumps/json_dump_lat_long.py` & `gps_sentences-0.1.2/src/helpers/json_dumps/json_dump_lat_long.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from src.helpers.helpers import NMEASerialReader, NMEASerialDecode
 import json
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 def json_lat_long():
-    """ Returns the latitude and longitude of the current location in JSON format """
+    """Returns the latitude and longitude of
+    the current location in JSON format"""
+    logger.debug("json_lat_long function has been called")
     read = NMEASerialReader()
     decode = NMEASerialDecode()
     gpgga_nmea = read.read_all()
     direction_lat = gpgga_nmea[3]
     direction_long = gpgga_nmea[5]
     lat = decode.decode_lat(gpgga_nmea)
     long = decode.decode_long(gpgga_nmea)
-    lat_value_pair = (f"{lat} {direction_lat}")
-    long_value_pair = (f"{long} {direction_long}")
-    values = {
-        "latitude": lat_value_pair,
-        "longitude": long_value_pair
-    }
+    lat_value_pair = f"{lat} {direction_lat}"
+    long_value_pair = f"{long} {direction_long}"
+    logging.info(lat_value_pair)
+    logging.info(long_value_pair)
+    values = {"latitude": lat_value_pair, "longitude": long_value_pair}
     return json.dumps(values)
-
-
-
```

### Comparing `gps_sentences-0.1.0/src/helpers/serial_run.py` & `gps_sentences-0.1.2/src/helpers/serial_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,28 @@
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
 def time_information():
-    """ Function that provides the time and date information """
+    """Function that provides the time and date information"""
     tz = time_zone()
     lt = local_time()
     day = date()
-    date_value_pair = (f"{day} {lt} {tz}")
+    date_value_pair = f"{day} {lt} {tz}"
+
+    logger.debug("Time and date information has been aquired.")
+
     return date_value_pair
 
 
 def serial_reader(date_time: str) -> str:
-    """ This function reads the data from the NMEA serial port and logs it to the log file. """
+    """This function reads the data from the NMEA
+    serial port and logs it to the log file."""
 
     read = NMEASerialReader()
     decode = NMEASerialDecode()
 
     gpgga_nmea = read.read_all()
     logger.info(gpgga_nmea)
 
@@ -29,25 +33,28 @@
     direction_long = gpgga_nmea[5]
 
     utc_time = decode.decode_time(gpgga_nmea)
     alt = decode.decode_alt(gpgga_nmea) + "M"
     lat = decode.decode_lat(gpgga_nmea)
     long = decode.decode_long(gpgga_nmea)
 
-    time_value_pair = (f"{utc_time} UTC")
-    alt_value_pair = (f"{alt}")
-    lat_value_pair = (f"{lat} degrees {direction_lat}")
-    long_value_pair = (f"{long} degrees {direction_long}")
+    time_value_pair = f"{utc_time} UTC"
+    alt_value_pair = f"{alt}"
+    lat_value_pair = f"{lat} degrees {direction_lat}"
+    long_value_pair = f"{long} degrees {direction_long}"
 
     values = {
         "date_and_time": date_time,
         "utc_time": time_value_pair,
         "altitude": alt_value_pair,
         "latitude": lat_value_pair,
-        "longitude": long_value_pair
+        "longitude": long_value_pair,
     }
 
+    logger.info(date_time)
     logger.info(time_value_pair)
     logger.info(alt_value_pair)
     logger.info(lat_value_pair)
     logger.info(long_value_pair)
+
+    logger.debug("Serial reader function has been called")
     return json.dumps(values)
```

### Comparing `gps_sentences-0.1.0/src/main.py` & `gps_sentences-0.1.2/src/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,89 @@
-""" Create a package that will read and decode GPS sentences from the serial terminal. """
+""" Create a package that will read and decode GPS sentences."""
 from .helpers.serial_run import serial_reader
 from .helpers.serial_run import time_information
 from .helpers.json_dumps.json_dump_lat_long import json_lat_long
 from .helpers.json_dumps.json_dump_alt import json_alt
 from .helpers.json_dumps.json_dump_utctime import json_utc_time
 from .helpers.json_dumps.json_dump_date import json_date_time
 from fastapi import FastAPI
 import uvicorn
+import logging
+import pathlib
+import logging.config
+
+
+# Initialize the logger
+logger = logging.getLogger(name=__name__)
+
+# Log file path
+ROOT = pathlib.Path(__file__).parent.parent.absolute()
+log_config = ROOT / "logging.conf"
+log_file_path = ROOT / "gps_sentences.log"
+
+# Configure the logger
+logging.config.fileConfig(
+    "logging.conf",
+    disable_existing_loggers=False,
+    defaults={"gps_sentences.log": f"{log_file_path}"},
+)
 
 
 def main():
-    """ Main function """
+    """Main function"""
     serial_reader(time_information())
+    logger.debug("Main serial reader function has been called.")
     app = FastAPI()
+    logger.debug("FastAPI app has been initialized.")
 
     @app.get("/")
     async def index():
-        """ Root endpoint """
+        """Root endpoint"""
+        logger.debug("Root endpoint has been called.")
         return {"message": "This is the root endpoint."}
 
     @app.get("/all_serial_data")
     async def all_serial_data():
-        """ Returns all serial data """
+        """Returns all serial data"""
+        logger.debug("All serial data endpoint has been called.")
         return {serial_reader(time_information())}
 
     @app.get("/all_serial_data/lat_long")
     async def all_serial_data_lat_long():
-        """ Returns the latitude and longitude of the current location in JSON format"""
+        """Returns the latitude and longitude of the
+        current location in JSON format"""
+        logger.debug("Latitude and longitude endpoint has been called.")
         return {json_lat_long()}
 
     @app.get("/all_serial_data/altitude")
     async def all_serial_data_altitude():
-        """ Returns the altitude of the current location in JSON format"""
+        """Returns the altitude of the current location in JSON format"""
+        logger.debug("Altitude endpoint has been called.")
         return {json_alt()}
 
     @app.get("/all_serial_data/utc_time")
     async def all_serial_data_utc_time():
-        """ Returns the UTC time of the current location in JSON format"""
+        """Returns the UTC time of the current location in JSON format"""
+        logger.debug("UTC time endpoint has been called.")
         return {json_utc_time()}
 
     @app.get("/all_serial_data/date_time")
     async def all_serial_data_date_time():
-        """ Returns the date and time of the current location in JSON format"""
+        """Returns the date and time of the current location in JSON format"""
+        logger.debug("Date and time endpoint has been called.")
         return {json_date_time()}
 
-    uvicorn.run(app, host="127.0.0.1", port=8084)
+    uvicorn.run(
+        app,
+        host="127.0.0.1",
+        port=8084,
+        log_level="debug",
+        log_config=str(log_config),
+        use_colors=True,
+    )
+    logger.debug("Uvicorn has been called.")
 
 
-if __name__ == '__main__':
-    """ Main function """
+if __name__ == "__main__":
+    """Main function"""
     main()
+    logger.debug("Main function has been called.")
```

