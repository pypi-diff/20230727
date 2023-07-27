# Comparing `tmp/temperature_converter_py-1.0.1.tar.gz` & `tmp/temperature_converter_py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\temperature_converter_py-1.0.1.tar", last modified: Wed Jun 17 14:27:36 2020, max compression
+gzip compressed data, was "temperature_converter_py-1.0.2.tar", last modified: Thu Jul 27 02:30:24 2023, max compression
```

## Comparing `temperature_converter_py-1.0.1.tar` & `temperature_converter_py-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2020-06-17 14:27:36.300782 temperature_converter_py-1.0.1/
--rw-rw-rw-   0        0        0     1094 2020-06-17 13:04:24.000000 temperature_converter_py-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1801 2020-06-17 14:27:36.300782 temperature_converter_py-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      740 2020-06-17 14:20:05.000000 temperature_converter_py-1.0.1/README.md
--rw-rw-rw-   0        0        0      114 2020-06-17 14:27:36.304781 temperature_converter_py-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1152 2020-06-17 14:06:02.000000 temperature_converter_py-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2020-06-17 14:27:36.240780 temperature_converter_py-1.0.1/temperature_converter_py/
--rw-rw-rw-   0        0        0       69 2020-06-16 21:13:14.000000 temperature_converter_py-1.0.1/temperature_converter_py/__init__.py
--rw-rw-rw-   0        0        0     1029 2020-06-17 13:59:08.000000 temperature_converter_py-1.0.1/temperature_converter_py/temperature_converter_py.py
-drwxrwxrwx   0        0        0        0 2020-06-17 14:27:36.297780 temperature_converter_py-1.0.1/temperature_converter_py.egg-info/
--rw-rw-rw-   0        0        0     1801 2020-06-17 14:27:35.000000 temperature_converter_py-1.0.1/temperature_converter_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2020-06-17 14:27:35.000000 temperature_converter_py-1.0.1/temperature_converter_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-06-17 14:27:35.000000 temperature_converter_py-1.0.1/temperature_converter_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2020-06-17 14:27:35.000000 temperature_converter_py-1.0.1/temperature_converter_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 02:30:24.465074 temperature_converter_py-1.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-07-27 02:19:16.000000 temperature_converter_py-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1751 2023-07-27 02:30:24.465581 temperature_converter_py-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      852 2023-07-27 02:29:28.000000 temperature_converter_py-1.0.2/README.md
+-rw-rw-rw-   0        0        0      114 2023-07-27 02:30:24.469289 temperature_converter_py-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1157 2023-07-27 02:28:52.000000 temperature_converter_py-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:30:24.446363 temperature_converter_py-1.0.2/temperature_converter_py/
+-rw-rw-rw-   0        0        0       69 2023-07-27 02:19:16.000000 temperature_converter_py-1.0.2/temperature_converter_py/__init__.py
+-rw-rw-rw-   0        0        0     2227 2023-07-27 02:21:45.000000 temperature_converter_py-1.0.2/temperature_converter_py/temperature_converter_py.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:30:24.464074 temperature_converter_py-1.0.2/temperature_converter_py.egg-info/
+-rw-rw-rw-   0        0        0     1751 2023-07-27 02:30:24.000000 temperature_converter_py-1.0.2/temperature_converter_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-07-27 02:30:24.000000 temperature_converter_py-1.0.2/temperature_converter_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 02:30:24.000000 temperature_converter_py-1.0.2/temperature_converter_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-27 02:30:24.000000 temperature_converter_py-1.0.2/temperature_converter_py.egg-info/top_level.txt
```

### Comparing `temperature_converter_py-1.0.1/LICENSE.txt` & `temperature_converter_py-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `temperature_converter_py-1.0.1/PKG-INFO` & `temperature_converter_py-1.0.2/temperature_converter_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
-Name: temperature_converter_py
-Version: 1.0.1
-Summary: UNKNOWN
+Name: temperature-converter-py
+Version: 1.0.2
 Home-page: https://github.com/BrunoASN/temperature_converter_py
 Author: Bruno Nascimento
-Author-email: bruno_freddy@hotmail.com
+Author-email: bruno-asn@hotmail.com
 License: MIT
 Project-URL: Código fonte, https://github.com/BrunoASN/temperature_converter_py
 Project-URL: Download, https://github.com/BrunoASN/temperature_converter_py/archive/master.zip
-Description: # Temperature Converter
-        
-        **temperature_converter_py** is a simple temperature converter.
-        
-        ## Functions
-        
-        - `celsius_to_fahrenheit(temp_in_celsius)`: Receives a float value in Celsius and returns in Fahrenheit.
-        
-        - `fahrenheit_to_celsius(temp_in_fahrenheit)`: Receives a float value in Fahrenheit and returns in Celsius.
-        
-        - `celsius_to_kelvin(temp_in_celsius)`: Receives a float value in Celsius and returns in Kelvin.
-        
-        - `kelvin_to_celsius(temp_in_kelvin)`: Receives a float value in Kelvin and returns in Celsius.
-        
-        - `fahrenheit_to_kelvin(temp_in_fahrenheit)`: Receives a float value in Fahrenheit and returns in Kelvin.
-        
-        - `kelvin_to_fahrenheit(temp_in_kelvin)`: Receives a float value in Kelvin and returns in Fahrenheit.
-        
 Keywords: conversor,temperatura
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Temperature Converter
+
+**temperature_converter_py** is a simple temperature converter.
+## Install
+- `pip install temperature-converter-py`
+## Import
+`import temperature_converter_py`
+
+## Functions
+
+- **celsius_to_fahrenheit(temp_in_celsius)**: Receives a float value in Celsius and returns in Fahrenheit.
+
+- **fahrenheit_to_celsius(temp_in_fahrenheit)**: Receives a float value in Fahrenheit and returns in Celsius.
+
+- **celsius_to_kelvin(temp_in_celsius)**: Receives a float value in Celsius and returns in Kelvin.
+
+- **kelvin_to_celsius(temp_in_kelvin)**: Receives a float value in Kelvin and returns in Celsius.
+
+- **fahrenheit_to_kelvin(temp_in_fahrenheit)**: Receives a float value in Fahrenheit and returns in Kelvin.
+
+- **kelvin_to_fahrenheit(temp_in_kelvin)**: Receives a float value in Kelvin and returns in Fahrenheit.
```

### Comparing `temperature_converter_py-1.0.1/README.md` & `temperature_converter_py-1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Temperature Converter
 
 **temperature_converter_py** is a simple temperature converter.
+## Install
+- `pip install temperature-converter-py`
+## Import
+`import temperature_converter_py`
 
 ## Functions
 
-- `celsius_to_fahrenheit(temp_in_celsius)`: Receives a float value in Celsius and returns in Fahrenheit.
+- **celsius_to_fahrenheit(temp_in_celsius)**: Receives a float value in Celsius and returns in Fahrenheit.
 
-- `fahrenheit_to_celsius(temp_in_fahrenheit)`: Receives a float value in Fahrenheit and returns in Celsius.
+- **fahrenheit_to_celsius(temp_in_fahrenheit)**: Receives a float value in Fahrenheit and returns in Celsius.
 
-- `celsius_to_kelvin(temp_in_celsius)`: Receives a float value in Celsius and returns in Kelvin.
+- **celsius_to_kelvin(temp_in_celsius)**: Receives a float value in Celsius and returns in Kelvin.
 
-- `kelvin_to_celsius(temp_in_kelvin)`: Receives a float value in Kelvin and returns in Celsius.
+- **kelvin_to_celsius(temp_in_kelvin)**: Receives a float value in Kelvin and returns in Celsius.
 
-- `fahrenheit_to_kelvin(temp_in_fahrenheit)`: Receives a float value in Fahrenheit and returns in Kelvin.
+- **fahrenheit_to_kelvin(temp_in_fahrenheit)**: Receives a float value in Fahrenheit and returns in Kelvin.
 
-- `kelvin_to_fahrenheit(temp_in_kelvin)`: Receives a float value in Kelvin and returns in Fahrenheit.
+- **kelvin_to_fahrenheit(temp_in_kelvin)**: Receives a float value in Kelvin and returns in Fahrenheit.
```

### Comparing `temperature_converter_py-1.0.1/setup.py` & `temperature_converter_py-1.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 with open("README.md", 'r') as fh:
-    long_description = fh.read()
+    markdown_description = fh.read()
 
 setup(
     name='temperature_converter_py',
-    version='1.0.1',
+    version='1.0.2',
     author='Bruno Nascimento',
-    author_email='bruno_freddy@hotmail.com',
-    long_description=long_description,
+    author_email='bruno-asn@hotmail.com',
+    long_description=markdown_description,
     long_description_content_type='text/markdown',
     packages=['temperature_converter_py'],
     url='https://github.com/BrunoASN/temperature_converter_py',
     project_urls={
         'Código fonte': 'https://github.com/BrunoASN/temperature_converter_py',
         'Download': 'https://github.com/BrunoASN/temperature_converter_py/archive/master.zip'
     },
```

### Comparing `temperature_converter_py-1.0.1/temperature_converter_py.egg-info/PKG-INFO` & `temperature_converter_py-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 Metadata-Version: 2.1
-Name: temperature-converter-py
-Version: 1.0.1
-Summary: UNKNOWN
+Name: temperature_converter_py
+Version: 1.0.2
 Home-page: https://github.com/BrunoASN/temperature_converter_py
 Author: Bruno Nascimento
-Author-email: bruno_freddy@hotmail.com
+Author-email: bruno-asn@hotmail.com
 License: MIT
 Project-URL: Código fonte, https://github.com/BrunoASN/temperature_converter_py
 Project-URL: Download, https://github.com/BrunoASN/temperature_converter_py/archive/master.zip
-Description: # Temperature Converter
-        
-        **temperature_converter_py** is a simple temperature converter.
-        
-        ## Functions
-        
-        - `celsius_to_fahrenheit(temp_in_celsius)`: Receives a float value in Celsius and returns in Fahrenheit.
-        
-        - `fahrenheit_to_celsius(temp_in_fahrenheit)`: Receives a float value in Fahrenheit and returns in Celsius.
-        
-        - `celsius_to_kelvin(temp_in_celsius)`: Receives a float value in Celsius and returns in Kelvin.
-        
-        - `kelvin_to_celsius(temp_in_kelvin)`: Receives a float value in Kelvin and returns in Celsius.
-        
-        - `fahrenheit_to_kelvin(temp_in_fahrenheit)`: Receives a float value in Fahrenheit and returns in Kelvin.
-        
-        - `kelvin_to_fahrenheit(temp_in_kelvin)`: Receives a float value in Kelvin and returns in Fahrenheit.
-        
 Keywords: conversor,temperatura
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Temperature Converter
+
+**temperature_converter_py** is a simple temperature converter.
+## Install
+- `pip install temperature-converter-py`
+## Import
+`import temperature_converter_py`
+
+## Functions
+
+- **celsius_to_fahrenheit(temp_in_celsius)**: Receives a float value in Celsius and returns in Fahrenheit.
+
+- **fahrenheit_to_celsius(temp_in_fahrenheit)**: Receives a float value in Fahrenheit and returns in Celsius.
+
+- **celsius_to_kelvin(temp_in_celsius)**: Receives a float value in Celsius and returns in Kelvin.
+
+- **kelvin_to_celsius(temp_in_kelvin)**: Receives a float value in Kelvin and returns in Celsius.
+
+- **fahrenheit_to_kelvin(temp_in_fahrenheit)**: Receives a float value in Fahrenheit and returns in Kelvin.
+
+- **kelvin_to_fahrenheit(temp_in_kelvin)**: Receives a float value in Kelvin and returns in Fahrenheit.
```

