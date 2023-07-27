# Comparing `tmp/midas-0.6.3.tar.gz` & `tmp/midas-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-0.6.3.tar", last modified: Tue Jun 13 17:55:24 2023, max compression
+gzip compressed data, was "midas-0.6.4.tar", last modified: Thu Jul 27 18:43:08 2023, max compression
```

## Comparing `midas-0.6.3.tar` & `midas-0.6.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-13 17:55:24.282996 midas-0.6.3/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-04-25 18:49:18.000000 midas-0.6.3/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-10 19:06:41.000000 midas-0.6.3/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3269 2023-06-13 17:55:24.283079 midas-0.6.3/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2376 2023-03-10 04:22:14.000000 midas-0.6.3/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-13 17:55:24.281435 midas-0.6.3/midas/
--rw-r--r--   0 a.ruddick   (502) staff       (20)      993 2023-06-02 19:43:38.000000 midas-0.6.3/midas/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5904 2023-05-01 20:34:55.000000 midas-0.6.3/midas/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     4028 2021-06-30 14:46:51.000000 midas-0.6.3/midas/faults.csv
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1889 2023-06-05 20:43:02.000000 midas-0.6.3/midas/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:34:55.000000 midas-0.6.3/midas/py.typed
--rw-r--r--   0 a.ruddick   (502) staff       (20)     6030 2023-06-13 17:47:50.000000 midas-0.6.3/midas/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-06-13 17:55:24.282826 midas-0.6.3/midas.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3269 2023-06-13 17:55:24.000000 midas-0.6.3/midas.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      317 2023-06-13 17:55:24.000000 midas-0.6.3/midas.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-06-13 17:55:24.000000 midas-0.6.3/midas.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       45 2023-06-13 17:55:24.000000 midas-0.6.3/midas.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      207 2023-06-13 17:55:24.000000 midas-0.6.3/midas.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        6 2023-06-13 17:55:24.000000 midas-0.6.3/midas.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      252 2023-06-13 17:55:24.283429 midas-0.6.3/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1825 2023-06-13 17:54:47.000000 midas-0.6.3/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-27 18:43:08.577567 midas-0.6.4/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       69 2023-04-25 18:49:18.000000 midas-0.6.4/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18026 2023-04-10 19:06:41.000000 midas-0.6.4/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3269 2023-07-27 18:43:08.577660 midas-0.6.4/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2376 2023-03-10 04:22:14.000000 midas-0.6.4/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-27 18:43:08.576300 midas-0.6.4/midas/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      993 2023-06-02 19:43:38.000000 midas-0.6.4/midas/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5904 2023-06-13 20:35:10.000000 midas-0.6.4/midas/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     4028 2021-06-30 14:46:51.000000 midas-0.6.4/midas/faults.csv
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1889 2023-06-05 20:43:02.000000 midas-0.6.4/midas/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-05-01 20:34:55.000000 midas-0.6.4/midas/py.typed
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     6066 2023-06-13 18:28:18.000000 midas-0.6.4/midas/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-07-27 18:43:08.577330 midas-0.6.4/midas.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3269 2023-07-27 18:43:08.000000 midas-0.6.4/midas.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      317 2023-07-27 18:43:08.000000 midas-0.6.4/midas.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-07-27 18:43:08.000000 midas-0.6.4/midas.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       45 2023-07-27 18:43:08.000000 midas-0.6.4/midas.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      207 2023-07-27 18:43:08.000000 midas-0.6.4/midas.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        6 2023-07-27 18:43:08.000000 midas-0.6.4/midas.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      252 2023-07-27 18:43:08.577923 midas-0.6.4/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1825 2023-07-27 18:42:24.000000 midas-0.6.4/setup.py
```

### Comparing `midas-0.6.3/LICENSE` & `midas-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-0.6.3/PKG-INFO` & `midas-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python driver for Honeywell Midas gas detectors.
 Home-page: https://github.com/numat/midas/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 Maintainer: Alex Ruddick
 Maintainer-email: alex@numat-tech.com
 License: GPLv2
```

### Comparing `midas-0.6.3/README.md` & `midas-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `midas-0.6.3/midas/__init__.py` & `midas-0.6.4/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `midas-0.6.3/midas/driver.py` & `midas-0.6.4/midas/driver.py`

 * *Files identical despite different names*

### Comparing `midas-0.6.3/midas/faults.csv` & `midas-0.6.4/midas/faults.csv`

 * *Files identical despite different names*

### Comparing `midas-0.6.3/midas/mock.py` & `midas-0.6.4/midas/mock.py`

 * *Files identical despite different names*

### Comparing `midas-0.6.3/midas/util.py` & `midas-0.6.4/midas/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,16 @@
         async with self.lock:
             try:
                 if self.pymodbus32plus:
                     future = getattr(self.client, method)
                 else:
                     future = getattr(self.client.protocol, method)  # type: ignore
                 return await future(*args, **kwargs)
-            except (asyncio.TimeoutError, pymodbus.exceptions.ConnectionException) as e:
+            except (asyncio.TimeoutError, pymodbus.exceptions.ConnectionException,
+                    AttributeError) as e:
                 raise TimeoutError("Not connected to Midas.") from e
 
     async def _close(self) -> None:
         """Close the TCP connection."""
         if self.pymodbus33plus:
             self.client.close()  # 3.3.x
         elif self.pymodbus30plus:
```

### Comparing `midas-0.6.3/midas.egg-info/PKG-INFO` & `midas-0.6.4/midas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python driver for Honeywell Midas gas detectors.
 Home-page: https://github.com/numat/midas/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 Maintainer: Alex Ruddick
 Maintainer-email: alex@numat-tech.com
 License: GPLv2
```

### Comparing `midas-0.6.3/setup.py` & `midas-0.6.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,37 +7,37 @@
     raise ImportError("This module requires Python >=3.8.  Use 0.5.1 for Python3.7")
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="midas",
-    version="0.6.3",
+    version="0.6.4",
     description="Python driver for Honeywell Midas gas detectors.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/numat/midas/",
     author="Patrick Fuller",
     author_email="pat@numat-tech.com",
     maintainer="Alex Ruddick",
     maintainer_email="alex@numat-tech.com",
     packages=['midas'],
     package_data={'midas': ['faults.csv', 'py.typed']},
     install_requires=[
         'pymodbus>=2.4.0; python_version == "3.8"',
         'pymodbus>=2.4.0; python_version == "3.9"',
-        'pymodbus>=3.0.2,<3.4.0; python_version >= "3.10"',
+        'pymodbus>=3.0.2,<3.5.0; python_version >= "3.10"',
     ],
     extras_require={
         'test': [
             'mypy>=1.1.1',
             'pytest',
             'pytest-cov',
             'pytest-asyncio',
-            'ruff==0.0.272',
+            'ruff==0.0.280',
         ],
     },
     entry_points={
         'console_scripts': [('midas = midas:command_line')]
     },
     license='GPLv2',
     classifiers=[
```

