# Comparing `tmp/watlow-0.5.3.tar.gz` & `tmp/watlow-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watlow-0.5.3.tar", last modified: Sat Jun 10 16:16:25 2023, max compression
+gzip compressed data, was "watlow-0.6.0.tar", last modified: Thu Jul 27 18:19:05 2023, max compression
```

## Comparing `watlow-0.5.3.tar` & `watlow-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-10 16:16:25.773151 watlow-0.5.3/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-06-07 16:19:52.000000 watlow-0.5.3/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-06-07 16:19:52.000000 watlow-0.5.3/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3067 2023-06-10 16:16:25.773212 watlow-0.5.3/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2031 2022-11-16 23:55:15.000000 watlow-0.5.3/README.md
--rw-r--r--   0 a.ruddick   (502) staff       (20)      159 2023-06-10 16:16:25.773419 watlow-0.5.3/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2020 2023-06-10 16:15:06.000000 watlow-0.5.3/setup.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-10 16:16:25.772333 watlow-0.5.3/watlow/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1830 2023-06-10 16:14:44.000000 watlow-0.5.3/watlow/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     9120 2023-06-10 16:14:44.000000 watlow-0.5.3/watlow/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2120 2023-06-10 16:14:44.000000 watlow-0.5.3/watlow/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5586 2023-06-10 16:14:44.000000 watlow-0.5.3/watlow/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-10 16:16:25.773053 watlow-0.5.3/watlow.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3067 2023-06-10 16:16:25.000000 watlow-0.5.3/watlow.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      295 2023-06-10 16:16:25.000000 watlow-0.5.3/watlow.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-10 16:16:25.000000 watlow-0.5.3/watlow.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       47 2023-06-10 16:16:25.000000 watlow-0.5.3/watlow.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      285 2023-06-10 16:16:25.000000 watlow-0.5.3/watlow.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        7 2023-06-10 16:16:25.000000 watlow-0.5.3/watlow.egg-info/top_level.txt
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-27 18:19:05.704739 watlow-0.6.0/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-06-07 16:19:52.000000 watlow-0.6.0/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-06-07 16:19:52.000000 watlow-0.6.0/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3017 2023-07-27 18:19:05.704805 watlow-0.6.0/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2031 2022-11-16 23:55:15.000000 watlow-0.6.0/README.md
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      159 2023-07-27 18:19:05.705029 watlow-0.6.0/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1759 2023-07-27 18:18:22.000000 watlow-0.6.0/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-27 18:19:05.703717 watlow-0.6.0/watlow/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1830 2023-06-10 16:14:44.000000 watlow-0.6.0/watlow/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     9180 2023-06-21 15:06:21.000000 watlow-0.6.0/watlow/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2120 2023-06-10 16:14:44.000000 watlow-0.6.0/watlow/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5587 2023-07-25 15:11:51.000000 watlow-0.6.0/watlow/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-27 18:19:05.704639 watlow-0.6.0/watlow.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3017 2023-07-27 18:19:05.000000 watlow-0.6.0/watlow.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      295 2023-07-27 18:19:05.000000 watlow-0.6.0/watlow.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-07-27 18:19:05.000000 watlow-0.6.0/watlow.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       47 2023-07-27 18:19:05.000000 watlow-0.6.0/watlow.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      238 2023-07-27 18:19:05.000000 watlow-0.6.0/watlow.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        7 2023-07-27 18:19:05.000000 watlow-0.6.0/watlow.egg-info/top_level.txt
```

### Comparing `watlow-0.5.3/LICENSE` & `watlow-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `watlow-0.5.3/PKG-INFO` & `watlow-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: watlow
-Version: 0.5.3
+Version: 0.6.0
 Summary: Python driver for Watlow EZ-Zone temperature controllers.
 Home-page: https://github.com/numat/watlow/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 Maintainer: Alex Ruddick
 Maintainer-email: alex@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Description-Content-Type: text/markdown
```

### Comparing `watlow-0.5.3/README.md` & `watlow-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `watlow-0.5.3/setup.py` & `watlow-0.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,51 @@
 """Install parameters for CLI and python import."""
-from sys import version_info
-
 from setuptools import setup
 
-if version_info < (3, 7):  # noqa: UP036
-    raise ImportError("This module requires Python >=3.7.  Use 0.3.1 for Python3.6")
-
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="watlow",
-    version="0.5.3",
+    version="0.6.0",
     description="Python driver for Watlow EZ-Zone temperature controllers.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/numat/watlow/",
     author="Patrick Fuller",
     author_email="pat@numat-tech.com",
     maintainer="Alex Ruddick",
     maintainer_email="alex@numat-tech.com",
     packages=["watlow"],
     install_requires=[
-        'pymodbus>=2.4.0,<3; python_version == "3.7"',
         'pymodbus>=2.4.0; python_version == "3.8"',
         'pymodbus>=2.4.0; python_version == "3.9"',
-        'pymodbus>=3.0.2,<3.4.0; python_version >= "3.10"',
+        'pymodbus>=3.0.2,<3.5.0; python_version >= "3.10"',
         "pyserial",
         "crcmod"],
     extras_require={
         'test': [
-            'mypy==1.3.0',
+            'mypy==1.4.1',
             'pytest',
             'pytest-cov',
             'pytest-asyncio',
-            'ruff==0.0.272',
+            'ruff==0.0.280',
             'types-pyserial',
         ],
     },
     entry_points={
         "console_scripts": [("watlow = watlow:command_line")]
     },
     license="GPLv2",
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Development Status :: 4 - Beta",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Human Machine Interfaces",
         "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)"
     ]
```

### Comparing `watlow-0.5.3/watlow/__init__.py` & `watlow-0.6.0/watlow/__init__.py`

 * *Files identical despite different names*

### Comparing `watlow-0.5.3/watlow/driver.py` & `watlow-0.6.0/watlow/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Drivers for Watlow EZ-Zone temperature controllers."""
 from __future__ import annotations
 
 import logging
 import re
 import struct
 from binascii import unhexlify
+from typing import ClassVar
 
 import crcmod  # type: ignore
 import serial
 from pymodbus.constants import Endian
 from pymodbus.payload import BinaryPayloadBuilder, BinaryPayloadDecoder
 
 from .util import AsyncioModbusClient
@@ -55,26 +56,26 @@
      * First checksum is a custom protocol.
      * Only known registers are 0401 for PV and 0701 for SP. Other registers
        return data, so we could hunt around for PID params if needed.
      * Instance, only 01 works. Current understanding is similar to zone.
      * Second checksum is a custom CRC-16 following Bacnet spec.
     """
 
-    commands = {
+    commands: ClassVar[dict] = {
         'actual':
             {'header': unhexlify('0510000006'),
              'body':   unhexlify('010301040101')},
         'setpoint':
             {'header': unhexlify('0510000006'),
              'body':   unhexlify('010301070101')},
         'set':
             {'header': unhexlify('051000000a'),
              'body':   unhexlify('010407010108')},
     }
-    responses = {
+    responses: ClassVar[dict] = {
         'actual': re.compile('^55ff060010000b8802030104010108'
                              '([0-9a-f]{8})([0-9a-f]{4})$'),
         'setpoint': re.compile('^55ff060010000b8802030107010108'
                                '([0-9a-f]{8})([0-9a-f]{4})$'),
         'set': re.compile('^55ff060010000a76020407010108'
                           '([0-9a-f]{8})([0-9a-f]{4})$')
     }
```

### Comparing `watlow-0.5.3/watlow/mock.py` & `watlow-0.6.0/watlow/mock.py`

 * *Files identical despite different names*

### Comparing `watlow-0.5.3/watlow/util.py` & `watlow-0.6.0/watlow/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         return registers
 
     async def read_holding_registers(self, address, count):
         """Read modbus holding registers."""
         await self._request('read_holding_registers', address, count)
 
     async def write_coil(self, address, value):
-        """Write modbus coils."""
+        """Write a modbus coil."""
         await self._request('write_coil', address, value)
 
     async def write_coils(self, address, values):
         """Write modbus coils."""
         await self._request('write_coils', address, values)
 
     async def write_register(self, address, value, skip_encode=False):
```

### Comparing `watlow-0.5.3/watlow.egg-info/PKG-INFO` & `watlow-0.6.0/watlow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: watlow
-Version: 0.5.3
+Version: 0.6.0
 Summary: Python driver for Watlow EZ-Zone temperature controllers.
 Home-page: https://github.com/numat/watlow/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 Maintainer: Alex Ruddick
 Maintainer-email: alex@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Description-Content-Type: text/markdown
```

