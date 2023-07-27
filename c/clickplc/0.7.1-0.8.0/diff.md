# Comparing `tmp/clickplc-0.7.1.tar.gz` & `tmp/clickplc-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickplc-0.7.1.tar", last modified: Mon Jun  5 21:17:35 2023, max compression
+gzip compressed data, was "clickplc-0.8.0.tar", last modified: Thu Jul 27 18:33:20 2023, max compression
```

## Comparing `clickplc-0.7.1.tar` & `clickplc-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:17:35.041057 clickplc-0.7.1/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-04-25 18:38:49.000000 clickplc-0.7.1/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-10 23:33:43.000000 clickplc-0.7.1/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)       16 2023-02-06 20:30:11.000000 clickplc-0.7.1/MANIFEST.in
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3694 2023-06-05 21:17:35.041118 clickplc-0.7.1/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2751 2023-04-11 05:40:45.000000 clickplc-0.7.1/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:17:35.039119 clickplc-0.7.1/clickplc/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1354 2022-11-17 00:56:19.000000 clickplc-0.7.1/clickplc/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)    22132 2023-04-10 23:33:43.000000 clickplc-0.7.1/clickplc/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3065 2023-06-05 21:17:10.000000 clickplc-0.7.1/clickplc/mock.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:17:35.040640 clickplc-0.7.1/clickplc/tests/
--rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:45:31.000000 clickplc-0.7.1/clickplc/tests/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)      190 2023-04-25 18:45:31.000000 clickplc-0.7.1/clickplc/tests/bad_tags.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2306 2023-04-25 18:45:31.000000 clickplc-0.7.1/clickplc/tests/plc_tags.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)    10508 2023-04-25 18:45:31.000000 clickplc-0.7.1/clickplc/tests/test_driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5541 2023-06-05 21:17:10.000000 clickplc-0.7.1/clickplc/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:17:35.039980 clickplc-0.7.1/clickplc.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3694 2023-06-05 21:17:34.000000 clickplc-0.7.1/clickplc.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      440 2023-06-05 21:17:35.000000 clickplc-0.7.1/clickplc.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-05 21:17:34.000000 clickplc-0.7.1/clickplc.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       51 2023-06-05 21:17:34.000000 clickplc-0.7.1/clickplc.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      254 2023-06-05 21:17:34.000000 clickplc-0.7.1/clickplc.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        9 2023-06-05 21:17:34.000000 clickplc-0.7.1/clickplc.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      161 2023-06-05 21:17:35.041323 clickplc-0.7.1/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1741 2023-06-05 21:17:13.000000 clickplc-0.7.1/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-27 18:33:20.619354 clickplc-0.8.0/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-04-25 18:38:49.000000 clickplc-0.8.0/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-10 23:33:43.000000 clickplc-0.8.0/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       16 2023-02-06 20:30:11.000000 clickplc-0.8.0/MANIFEST.in
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3644 2023-07-27 18:33:20.619421 clickplc-0.8.0/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2751 2023-06-28 18:39:31.000000 clickplc-0.8.0/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-27 18:33:20.616820 clickplc-0.8.0/clickplc/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1354 2022-11-17 00:56:19.000000 clickplc-0.8.0/clickplc/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    22158 2023-06-28 18:35:47.000000 clickplc-0.8.0/clickplc/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3065 2023-06-05 21:17:10.000000 clickplc-0.8.0/clickplc/mock.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-27 18:33:20.618739 clickplc-0.8.0/clickplc/tests/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:45:31.000000 clickplc-0.8.0/clickplc/tests/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      190 2023-04-25 18:45:31.000000 clickplc-0.8.0/clickplc/tests/bad_tags.csv
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2306 2023-04-25 18:45:31.000000 clickplc-0.8.0/clickplc/tests/plc_tags.csv
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    10508 2023-04-25 18:45:31.000000 clickplc-0.8.0/clickplc/tests/test_driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5480 2023-06-28 18:45:40.000000 clickplc-0.8.0/clickplc/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-27 18:33:20.617954 clickplc-0.8.0/clickplc.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3644 2023-07-27 18:33:20.000000 clickplc-0.8.0/clickplc.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      440 2023-07-27 18:33:20.000000 clickplc-0.8.0/clickplc.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-07-27 18:33:20.000000 clickplc-0.8.0/clickplc.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       51 2023-07-27 18:33:20.000000 clickplc-0.8.0/clickplc.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      207 2023-07-27 18:33:20.000000 clickplc-0.8.0/clickplc.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        9 2023-07-27 18:33:20.000000 clickplc-0.8.0/clickplc.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      161 2023-07-27 18:33:20.619635 clickplc-0.8.0/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1637 2023-07-27 18:32:53.000000 clickplc-0.8.0/setup.py
```

### Comparing `clickplc-0.7.1/LICENSE` & `clickplc-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clickplc-0.7.1/PKG-INFO` & `clickplc-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: clickplc
-Version: 0.7.1
+Version: 0.8.0
 Summary: Python driver for Koyo Ethernet ClickPLCs.
 Home-page: https://github.com/numat/clickplc/
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
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 clickplc
 ========
 
-Python ≥3.6 driver and command-line tool for [Koyo Ethernet ClickPLCs](https://www.automationdirect.com/adc/Overview/Catalog/Programmable_Controllers/CLICK_Series_PLCs_(Stackable_Micro_Brick)).
+Python ≥3.8 driver and command-line tool for [Koyo Ethernet ClickPLCs](https://www.automationdirect.com/adc/Overview/Catalog/Programmable_Controllers/CLICK_Series_PLCs_(Stackable_Micro_Brick)).
 
 <p align="center">
   <img src="https://www.automationdirect.com/microsites/clickplcs/images/expandedclick.jpg" />
 </p>
 
 Installation
 ============
```

### Comparing `clickplc-0.7.1/README.md` & `clickplc-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 clickplc
 ========
 
-Python ≥3.6 driver and command-line tool for [Koyo Ethernet ClickPLCs](https://www.automationdirect.com/adc/Overview/Catalog/Programmable_Controllers/CLICK_Series_PLCs_(Stackable_Micro_Brick)).
+Python ≥3.8 driver and command-line tool for [Koyo Ethernet ClickPLCs](https://www.automationdirect.com/adc/Overview/Catalog/Programmable_Controllers/CLICK_Series_PLCs_(Stackable_Micro_Brick)).
 
 <p align="center">
   <img src="https://www.automationdirect.com/microsites/clickplcs/images/expandedclick.jpg" />
 </p>
 
 Installation
 ============
```

### Comparing `clickplc-0.7.1/clickplc/__init__.py` & `clickplc-0.8.0/clickplc/__init__.py`

 * *Files identical despite different names*

### Comparing `clickplc-0.7.1/clickplc/driver.py` & `clickplc-0.8.0/clickplc/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 from __future__ import annotations
 
 import copy
 import csv
 import pydoc
 from collections import defaultdict
 from string import digits
-from typing import Any
+from typing import Any, ClassVar
 
 from pymodbus.constants import Endian
 from pymodbus.payload import BinaryPayloadBuilder, BinaryPayloadDecoder
 
 from clickplc.util import AsyncioModbusClient
 
 
 class ClickPLC(AsyncioModbusClient):
     """Ethernet driver for the Koyo ClickPLC.
 
     This interface handles the quirks of both Modbus TCP/IP and the ClickPLC,
     abstracting corner cases and providing a simple asynchronous interface.
     """
 
-    data_types = {
+    data_types: ClassVar[dict] = {
         'x': 'bool',     # Input point
         'y': 'bool',     # Output point
         'c': 'bool',     # (C)ontrol relay
         'df': 'float',   # (D)ata register (f)loating point
         'ds': 'int16',   # (D)ata register (s)igned int
         'sd': 'int16',   # (S)ystem (D)ata
         'ctd': 'int32',  # (C)oun(t)er Current Values, (d)ouble
```

### Comparing `clickplc-0.7.1/clickplc/mock.py` & `clickplc-0.8.0/clickplc/mock.py`

 * *Files identical despite different names*

### Comparing `clickplc-0.7.1/clickplc/tests/plc_tags.csv` & `clickplc-0.8.0/clickplc/tests/plc_tags.csv`

 * *Files identical despite different names*

### Comparing `clickplc-0.7.1/clickplc/tests/test_driver.py` & `clickplc-0.8.0/clickplc/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `clickplc-0.7.1/clickplc/util.py` & `clickplc-0.8.0/clickplc/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,39 +30,37 @@
         self._detect_pymodbus_version()
         if self.pymodbus30plus:
             self.client = AsyncModbusTcpClient(address, timeout=timeout)
         else:  # 2.x
             self.client = ReconnectingAsyncioModbusTcpClient()
         self.lock = asyncio.Lock()
         self.connectTask = asyncio.create_task(self._connect())
-        self.open = False
 
     async def __aenter__(self):
         """Asynchronously connect with the context manager."""
         return self
 
-    async def __aexit__(self, *args):
+    async def __aexit__(self, *args) -> None:
         """Provide exit to the context manager."""
         await self._close()
 
-    def _detect_pymodbus_version(self):
+    def _detect_pymodbus_version(self) -> None:
         """Detect various pymodbus versions."""
         self.pymodbus30plus = int(pymodbus.__version__[0]) == 3
         self.pymodbus32plus = self.pymodbus30plus and int(pymodbus.__version__[2]) >= 2
         self.pymodbus33plus = self.pymodbus30plus and int(pymodbus.__version__[2]) >= 3
 
-    async def _connect(self):
+    async def _connect(self) -> None:
         """Start asynchronous reconnect loop."""
         async with self.lock:
             try:
                 if self.pymodbus30plus:
                     await asyncio.wait_for(self.client.connect(), timeout=self.timeout)  # 3.x
                 else:  # 2.4.x - 2.5.x
                     await self.client.start(self.ip)  # type: ignore
-                self.open = True
             except Exception:
                 raise OSError(f"Could not connect to '{self.ip}'.")
 
     async def read_coils(self, address: int, count):
         """Read modbus output coils (0 address prefix)."""
         return await self._request('read_coils', address, count)
 
@@ -133,8 +131,7 @@
         """Close the TCP connection."""
         if self.pymodbus33plus:
             self.client.close()  # 3.3.x
         elif self.pymodbus30plus:
             await self.client.close()  # type: ignore  # 3.0.x - 3.2.x
         else:  # 2.4.x - 2.5.x
             self.client.stop()  # type: ignore
-        self.open = False
```

### Comparing `clickplc-0.7.1/clickplc.egg-info/PKG-INFO` & `clickplc-0.8.0/clickplc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: clickplc
-Version: 0.7.1
+Version: 0.8.0
 Summary: Python driver for Koyo Ethernet ClickPLCs.
 Home-page: https://github.com/numat/clickplc/
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
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 clickplc
 ========
 
-Python ≥3.6 driver and command-line tool for [Koyo Ethernet ClickPLCs](https://www.automationdirect.com/adc/Overview/Catalog/Programmable_Controllers/CLICK_Series_PLCs_(Stackable_Micro_Brick)).
+Python ≥3.8 driver and command-line tool for [Koyo Ethernet ClickPLCs](https://www.automationdirect.com/adc/Overview/Catalog/Programmable_Controllers/CLICK_Series_PLCs_(Stackable_Micro_Brick)).
 
 <p align="center">
   <img src="https://www.automationdirect.com/microsites/clickplcs/images/expandedclick.jpg" />
 </p>
 
 Installation
 ============
```

### Comparing `clickplc-0.7.1/setup.py` & `clickplc-0.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,50 +3,48 @@
 from setuptools import setup
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name='clickplc',
-    version='0.7.1',
+    version='0.8.0',
     description="Python driver for Koyo Ethernet ClickPLCs.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/numat/clickplc/',
     author='Patrick Fuller',
     author_email='pat@numat-tech.com',
     maintainer='Alex Ruddick',
     maintainer_email='alex@numat-tech.com',
     packages=['clickplc'],
     entry_points={
         'console_scripts': [('clickplc = clickplc:command_line')]
     },
     install_requires=[
-        'pymodbus>=2.4.0,<3; python_version == "3.7"',
         'pymodbus>=2.4.0; python_version == "3.8"',
         'pymodbus>=2.4.0; python_version == "3.9"',
-        'pymodbus>=3.0.2,<3.4.0; python_version >= "3.10"',
+        'pymodbus>=3.0.2,<3.5.0; python_version >= "3.10"',
     ],
     extras_require={
         'test': [
             'pytest',
             'pytest-cov',
             'pytest-asyncio',
-            'mypy==1.3.0',
-            'ruff==0.0.270',
+            'mypy==1.4.1',
+            'ruff==0.0.280',
         ],
     },
     license='GPLv2',
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Development Status :: 4 - Beta',
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Human Machine Interfaces'
     ]
 )
```

