# Comparing `tmp/cave_utils-1.5.2.tar.gz` & `tmp/cave_utils-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_utils-1.5.2.tar", last modified: Fri Jul 21 14:24:22 2023, max compression
+gzip compressed data, was "cave_utils-1.5.3.tar", last modified: Thu Jul 27 18:30:05 2023, max compression
```

## Comparing `cave_utils-1.5.2.tar` & `cave_utils-1.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-21 14:24:22.186586 cave_utils-1.5.2/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.2/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.2/NOTICE.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1602 2023-07-21 14:24:22.186586 cave_utils-1.5.2/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      927 2023-06-13 20:25:36.000000 cave_utils-1.5.2/README.md
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-21 14:24:22.186586 cave_utils-1.5.2/cave_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      131 2023-06-22 13:25:50.000000 cave_utils-1.5.2/cave_utils/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-06-27 13:54:10.000000 cave_utils-1.5.2/cave_utils/arguments.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1325 2023-06-16 14:30:37.000000 cave_utils-1.5.2/cave_utils/log.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-16 14:28:26.000000 cave_utils-1.5.2/cave_utils/socket.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    57226 2023-07-21 14:23:54.000000 cave_utils-1.5.2/cave_utils/validator.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-21 14:24:22.186586 cave_utils-1.5.2/cave_utils.egg-info/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1602 2023-07-21 14:24:22.000000 cave_utils-1.5.2/cave_utils.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      383 2023-07-21 14:24:22.000000 cave_utils-1.5.2/cave_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-21 14:24:22.000000 cave_utils-1.5.2/cave_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-07-21 14:24:22.000000 cave_utils-1.5.2/cave_utils.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-07-21 14:24:22.000000 cave_utils-1.5.2/cave_utils.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.2/pyproject.toml
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-21 14:24:22.190586 cave_utils-1.5.2/setup.cfg
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      993 2023-07-21 14:18:24.000000 cave_utils-1.5.2/setup.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-21 14:24:22.186586 cave_utils-1.5.2/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      305 2023-06-27 13:54:32.000000 cave_utils-1.5.2/test/test_arguments.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       39 2023-06-22 13:14:02.000000 cave_utils-1.5.2/test/test_import.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-27 18:30:05.333078 cave_utils-1.5.3/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-1.5.3/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-1.5.3/NOTICE.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1602 2023-07-27 18:30:05.333078 cave_utils-1.5.3/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      927 2023-07-27 18:29:04.000000 cave_utils-1.5.3/README.md
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-27 18:30:05.333078 cave_utils-1.5.3/cave_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      131 2023-06-22 13:25:50.000000 cave_utils-1.5.3/cave_utils/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-06-27 13:54:10.000000 cave_utils-1.5.3/cave_utils/arguments.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1325 2023-06-16 14:30:37.000000 cave_utils-1.5.3/cave_utils/log.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-16 14:28:26.000000 cave_utils-1.5.3/cave_utils/socket.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    57226 2023-07-21 14:29:30.000000 cave_utils-1.5.3/cave_utils/validator.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-27 18:30:05.333078 cave_utils-1.5.3/cave_utils.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1602 2023-07-27 18:30:05.000000 cave_utils-1.5.3/cave_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      383 2023-07-27 18:30:05.000000 cave_utils-1.5.3/cave_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-27 18:30:05.000000 cave_utils-1.5.3/cave_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       13 2023-07-27 18:30:05.000000 cave_utils-1.5.3/cave_utils.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2023-07-27 18:30:05.000000 cave_utils-1.5.3/cave_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      101 2023-06-13 14:42:48.000000 cave_utils-1.5.3/pyproject.toml
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-27 18:30:05.333078 cave_utils-1.5.3/setup.cfg
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      993 2023-07-27 18:28:53.000000 cave_utils-1.5.3/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-27 18:30:05.333078 cave_utils-1.5.3/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      305 2023-06-27 13:54:32.000000 cave_utils-1.5.3/test/test_arguments.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       39 2023-06-22 13:14:02.000000 cave_utils-1.5.3/test/test_import.py
```

### Comparing `cave_utils-1.5.2/LICENSE` & `cave_utils-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.2/NOTICE.md` & `cave_utils-1.5.3/NOTICE.md`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.2/PKG-INFO` & `cave_utils-1.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 1.5.2
+Version: 1.5.3
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.2.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.3.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.md
 
 Cave Utilities for the Cave App
 ==========
 Basic utilities for the MIT Cave App. This package is intended to be used by the Cave App and the Cave API.
 
 Setup
 ----------
 
-Make sure you have Python 3.9.x (or higher) installed on your system. You can download it [here](https://www.python.org/downloads/).
+Make sure you have Python 3.7.x (or higher) installed on your system. You can download it [here](https://www.python.org/downloads/).
 
 ### Installation
 
 ```
 pip install cave_utils
 ```
```

### Comparing `cave_utils-1.5.2/README.md` & `cave_utils-1.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Cave Utilities for the Cave App
 ==========
 Basic utilities for the MIT Cave App. This package is intended to be used by the Cave App and the Cave API.
 
 Setup
 ----------
 
-Make sure you have Python 3.9.x (or higher) installed on your system. You can download it [here](https://www.python.org/downloads/).
+Make sure you have Python 3.7.x (or higher) installed on your system. You can download it [here](https://www.python.org/downloads/).
 
 ### Installation
 
 ```
 pip install cave_utils
 ```
```

### Comparing `cave_utils-1.5.2/cave_utils/arguments.py` & `cave_utils-1.5.3/cave_utils/arguments.py`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.2/cave_utils/log.py` & `cave_utils-1.5.3/cave_utils/log.py`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.2/cave_utils/validator.py` & `cave_utils-1.5.3/cave_utils/validator.py`

 * *Files identical despite different names*

### Comparing `cave_utils-1.5.2/cave_utils.egg-info/PKG-INFO` & `cave_utils-1.5.3/cave_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: cave-utils
-Version: 1.5.2
+Version: 1.5.3
 Summary: Cave utilities for the CAVE App at the MIT
 Home-page: https://github.com/mit-cave/cave_utils
-Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.2.tar.gz
+Download-URL: https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.3.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.md
 
 Cave Utilities for the Cave App
 ==========
 Basic utilities for the MIT Cave App. This package is intended to be used by the Cave App and the Cave API.
 
 Setup
 ----------
 
-Make sure you have Python 3.9.x (or higher) installed on your system. You can download it [here](https://www.python.org/downloads/).
+Make sure you have Python 3.7.x (or higher) installed on your system. You can download it [here](https://www.python.org/downloads/).
 
 ### Installation
 
 ```
 pip install cave_utils
 ```
```

### Comparing `cave_utils-1.5.2/setup.py` & `cave_utils-1.5.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'cave_utils',
   packages=['cave_utils'],
-  version = '1.5.2',
+  version = '1.5.3',
   license='MIT',
   description = 'Cave utilities for the CAVE App at the MIT',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'connor.m.makowski@gmail.com',
   url = 'https://github.com/mit-cave/cave_utils',
-  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.2.tar.gz',
+  download_url = 'https://github.com/mit-cave/cave_utils/dist/cave_utils-1.5.3.tar.gz',
   keywords = [],
   install_requires=[
     'pamda>=2.1.2',
   ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
   ],
-  python_requires=">=3.9, <4",
+  python_requires=">=3.7, <4",
 )
```

