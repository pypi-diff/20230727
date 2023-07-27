# Comparing `tmp/productivity-0.9.1.tar.gz` & `tmp/productivity-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "productivity-0.9.1.tar", last modified: Mon Jun  5 21:05:14 2023, max compression
+gzip compressed data, was "productivity-0.9.2.tar", last modified: Wed Jun 28 18:30:46 2023, max compression
```

## Comparing `productivity-0.9.1.tar` & `productivity-0.9.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:05:14.243499 productivity-0.9.1/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       80 2023-04-25 18:53:08.000000 productivity-0.9.1/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-18 00:56:18.000000 productivity-0.9.1/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)       16 2021-07-02 03:58:52.000000 productivity-0.9.1/MANIFEST.in
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3155 2023-06-05 21:05:14.243563 productivity-0.9.1/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2186 2023-04-11 05:00:34.000000 productivity-0.9.1/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:05:14.241815 productivity-0.9.1/productivity/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1197 2022-11-17 00:08:20.000000 productivity-0.9.1/productivity/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)    15410 2023-06-05 21:04:04.000000 productivity-0.9.1/productivity/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3368 2023-06-05 21:04:04.000000 productivity-0.9.1/productivity/mock.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:05:14.243366 productivity-0.9.1/productivity/tests/
--rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2021-07-02 03:58:52.000000 productivity-0.9.1/productivity/tests/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1246 2021-07-02 03:58:52.000000 productivity-0.9.1/productivity/tests/bad_tags.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1211 2021-09-09 18:54:10.000000 productivity-0.9.1/productivity/tests/plc_tags.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5564 2023-04-18 00:56:18.000000 productivity-0.9.1/productivity/tests/test_driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     7434 2023-06-05 21:04:04.000000 productivity-0.9.1/productivity/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-05 21:05:14.242556 productivity-0.9.1/productivity.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3155 2023-06-05 21:05:14.000000 productivity-0.9.1/productivity.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      496 2023-06-05 21:05:14.000000 productivity-0.9.1/productivity.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-05 21:05:14.000000 productivity-0.9.1/productivity.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       59 2023-06-05 21:05:14.000000 productivity-0.9.1/productivity.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      274 2023-06-05 21:05:14.000000 productivity-0.9.1/productivity.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       13 2023-06-05 21:05:14.000000 productivity-0.9.1/productivity.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      270 2023-06-05 21:05:14.243800 productivity-0.9.1/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1955 2023-06-05 21:04:21.000000 productivity-0.9.1/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-28 18:30:46.246261 productivity-0.9.2/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       96 2023-06-28 18:15:56.000000 productivity-0.9.2/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-18 00:56:18.000000 productivity-0.9.2/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       16 2021-07-02 03:58:52.000000 productivity-0.9.2/MANIFEST.in
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3105 2023-06-28 18:30:46.246334 productivity-0.9.2/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2186 2023-06-28 18:20:05.000000 productivity-0.9.2/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-28 18:30:46.244307 productivity-0.9.2/productivity/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1197 2022-11-17 00:08:20.000000 productivity-0.9.2/productivity/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    15410 2023-06-19 19:16:47.000000 productivity-0.9.2/productivity/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3420 2023-06-21 19:16:16.000000 productivity-0.9.2/productivity/mock.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-28 18:30:46.245969 productivity-0.9.2/productivity/tests/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2021-07-02 03:58:52.000000 productivity-0.9.2/productivity/tests/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1246 2021-07-02 03:58:52.000000 productivity-0.9.2/productivity/tests/bad_tags.csv
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1211 2021-09-09 18:54:10.000000 productivity-0.9.2/productivity/tests/plc_tags.csv
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5564 2023-04-18 00:56:18.000000 productivity-0.9.2/productivity/tests/test_driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     7358 2023-06-28 18:28:58.000000 productivity-0.9.2/productivity/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-28 18:30:46.245177 productivity-0.9.2/productivity.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3105 2023-06-28 18:30:46.000000 productivity-0.9.2/productivity.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      496 2023-06-28 18:30:46.000000 productivity-0.9.2/productivity.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-28 18:30:46.000000 productivity-0.9.2/productivity.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       59 2023-06-28 18:30:46.000000 productivity-0.9.2/productivity.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      227 2023-06-28 18:30:46.000000 productivity-0.9.2/productivity.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       13 2023-06-28 18:30:46.000000 productivity-0.9.2/productivity.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      270 2023-06-28 18:30:46.246573 productivity-0.9.2/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1851 2023-06-28 18:20:05.000000 productivity-0.9.2/setup.py
```

### Comparing `productivity-0.9.1/LICENSE` & `productivity-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `productivity-0.9.1/PKG-INFO` & `productivity-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: productivity
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python driver for AutomationDirect Productivity Series PLCs.
 Home-page: https://github.com/numat/productivity/
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
 
 Productivity
 ============
 
 ##### NOTE: This is in very early stages of development.
 
-Python ≥3.7 driver and command-line tool for [AutomationDirect Productivity Series PLCs](https://www.automationdirect.com/adc/overview/catalog/programmable_controllers/productivity_series_controllers).
+Python ≥3.8 driver and command-line tool for [AutomationDirect Productivity Series PLCs](https://www.automationdirect.com/adc/overview/catalog/programmable_controllers/productivity_series_controllers).
 
 <p align="center">
   <img src="https://www.automationdirect.com/images/overviews/p-series-cpus_400.jpg" />
 </p>
 
 Installation
 ============
```

### Comparing `productivity-0.9.1/README.md` & `productivity-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Productivity
 ============
 
 ##### NOTE: This is in very early stages of development.
 
-Python ≥3.7 driver and command-line tool for [AutomationDirect Productivity Series PLCs](https://www.automationdirect.com/adc/overview/catalog/programmable_controllers/productivity_series_controllers).
+Python ≥3.8 driver and command-line tool for [AutomationDirect Productivity Series PLCs](https://www.automationdirect.com/adc/overview/catalog/programmable_controllers/productivity_series_controllers).
 
 <p align="center">
   <img src="https://www.automationdirect.com/images/overviews/p-series-cpus_400.jpg" />
 </p>
 
 Installation
 ============
```

### Comparing `productivity-0.9.1/productivity/__init__.py` & `productivity-0.9.2/productivity/__init__.py`

 * *Files identical despite different names*

### Comparing `productivity-0.9.1/productivity/driver.py` & `productivity-0.9.2/productivity/driver.py`

 * *Files identical despite different names*

### Comparing `productivity-0.9.1/productivity/mock.py` & `productivity-0.9.2/productivity/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         self.tags = self._load_tags(tag_filepath)
         self.addresses = self._calculate_addresses(self.tags)
         self.map = {data['address']['start']: tag for tag, data in self.tags.items()}
         self.client = AsyncClientMock()
         self._coils = defaultdict(bool)
         self._discrete_inputs = defaultdict(bool)
         self._registers = defaultdict(bytes)
+        self._register_types = ['holding', 'input']
         self._detect_pymodbus_version()
         if self.pymodbus33plus:
             self.client.close = lambda: None
 
     async def _request(self, method, *args, **kwargs):
         if method == 'read_coils':
             address, count = args
```

### Comparing `productivity-0.9.1/productivity/tests/bad_tags.csv` & `productivity-0.9.2/productivity/tests/bad_tags.csv`

 * *Files identical despite different names*

### Comparing `productivity-0.9.1/productivity/tests/plc_tags.csv` & `productivity-0.9.2/productivity/tests/plc_tags.csv`

 * *Files identical despite different names*

### Comparing `productivity-0.9.1/productivity/tests/test_driver.py` & `productivity-0.9.2/productivity/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `productivity-0.9.1/productivity/util.py` & `productivity-0.9.2/productivity/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,51 +41,49 @@
 class AsyncioModbusClient:
     """A generic asyncio client.
 
     This expands upon the pymodbus AsyncModbusTcpClient by
     including standard timeouts, async context manager, and queued requests.
     """
 
-    _register_types = ['holding', 'input']
-
     def __init__(self, address, timeout=1):
         """Set up communication parameters."""
         self.ip = address
         self.timeout = timeout
+        self._register_types = ['holding', 'input']
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
 
     async def __aexit__(self, *args):
         """Provide exit to the context manager."""
         await self._close()
 
     def _detect_pymodbus_version(self) -> None:
+        """Detect various pymodbus versions."""
         self.pymodbus30plus = int(pymodbus.__version__[0]) == 3
         self.pymodbus32plus = self.pymodbus30plus and int(pymodbus.__version__[2]) >= 2
         self.pymodbus33plus = self.pymodbus30plus and int(pymodbus.__version__[2]) >= 3
 
     async def _connect(self):
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
 
     async def read_coils(self, address, count):
         """Read modbus output coils (0 address prefix)."""
         return await self._request('read_coils', address, count)
 
@@ -105,18 +103,17 @@
         if type not in self._register_types:
             raise ValueError(f"Register type {type} not in {self._register_types}.")
         registers = []
         while count > max_count:
             # if the last address read will be in the middle of a 32-bit tag
             # read one less address to avoid bad replies
             # https://github.com/numat/productivity/issues/38
-            last_address = self.map.get(TYPE_START[type] + address + max_count,  # type: ignore
-                                        None)
-            last_type = self.tags[last_address]['type']   # type: ignore
-            offset = -1 if (last_address and last_type in ['int32', 'float']) else 0
+            last_address = self.map.get(TYPE_START[type] + address + max_count, None)  # type: ignore
+            offset = -1 if (last_address
+                            and self.tags[last_address]['type'] in ['int32', 'float']) else 0  # type: ignore
             r = await self._request(f'read_{type}_registers', address, max_count + offset)
             address, count = address + (max_count + offset), count - (max_count + offset)
             registers += r.registers
         r = await self._request(f'read_{type}_registers', address, count)
         registers += r.registers
         return registers
 
@@ -173,8 +170,7 @@
         """Close the TCP connection."""
         if self.pymodbus33plus:
             self.client.close()  # 3.3.x
         elif self.pymodbus30plus:
             await self.client.close()  # type: ignore  # 3.0.x - 3.2.x
         else:  # 2.4.x - 2.5.x
             self.client.stop()  # type: ignore
-        self.open = False
```

### Comparing `productivity-0.9.1/productivity.egg-info/PKG-INFO` & `productivity-0.9.2/productivity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: productivity
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python driver for AutomationDirect Productivity Series PLCs.
 Home-page: https://github.com/numat/productivity/
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
 
 Productivity
 ============
 
 ##### NOTE: This is in very early stages of development.
 
-Python ≥3.7 driver and command-line tool for [AutomationDirect Productivity Series PLCs](https://www.automationdirect.com/adc/overview/catalog/programmable_controllers/productivity_series_controllers).
+Python ≥3.8 driver and command-line tool for [AutomationDirect Productivity Series PLCs](https://www.automationdirect.com/adc/overview/catalog/programmable_controllers/productivity_series_controllers).
 
 <p align="center">
   <img src="https://www.automationdirect.com/images/overviews/p-series-cpus_400.jpg" />
 </p>
 
 Installation
 ============
```

### Comparing `productivity-0.9.1/setup.py` & `productivity-0.9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,52 +7,50 @@
     raise ImportError("This module requires Python >=3.7.  Use 0.6.0 for Python3.6")
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name='productivity',
-    version='0.9.1',
+    version='0.9.2',
     description="Python driver for AutomationDirect Productivity Series PLCs.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/numat/productivity/',
     author='Patrick Fuller',
     author_email='pat@numat-tech.com',
     maintainer="Alex Ruddick",
     maintainer_email="alex@numat-tech.com",
     packages=['productivity'],
     entry_points={
         'console_scripts': [('productivity = productivity:command_line')]
     },
     install_requires=[
-        'pymodbus>=2.4.0,<3; python_version == "3.7"',
         'pymodbus>=2.4.0; python_version == "3.8"',
         'pymodbus>=2.4.0; python_version == "3.9"',
         'pymodbus>=3.0.2,<3.4.0; python_version >= "3.10"',
         'PyYAML',
     ],
     extras_require={
         'test': [
-            'mypy==1.3.0',
+            'mypy==1.4.1',
             'pytest',
             'pytest-cov',
             'pytest-asyncio',
-            'ruff==0.0.270',
+            'ruff==0.0.275',
             'types-PyYAML'
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

