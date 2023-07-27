# Comparing `tmp/pyrandonaut-0.1.6.tar.gz` & `tmp/pyrandonaut-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrandonaut-0.1.6.tar", last modified: Wed Aug  3 22:30:35 2022, max compression
+gzip compressed data, was "pyrandonaut-0.1.7.tar", last modified: Thu Jul 27 04:53:04 2023, max compression
```

## Comparing `pyrandonaut-0.1.6.tar` & `pyrandonaut-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aesthese   (501) staff       (20)        0 2022-08-03 22:30:35.612985 pyrandonaut-0.1.6/
--rw-r--r--   0 aesthese   (501) staff       (20)    35149 2022-08-01 11:28:15.000000 pyrandonaut-0.1.6/LICENSE
--rw-r--r--   0 aesthese   (501) staff       (20)     7143 2022-08-03 22:30:35.612683 pyrandonaut-0.1.6/PKG-INFO
--rw-r--r--   0 aesthese   (501) staff       (20)     6366 2022-08-03 15:40:47.000000 pyrandonaut-0.1.6/README.md
-drwxr-xr-x   0 aesthese   (501) staff       (20)        0 2022-08-03 22:30:35.610500 pyrandonaut-0.1.6/pyrandonaut/
--rw-r--r--   0 aesthese   (501) staff       (20)     7160 2022-08-03 22:28:32.000000 pyrandonaut-0.1.6/pyrandonaut/__init__.py
-drwxr-xr-x   0 aesthese   (501) staff       (20)        0 2022-08-03 22:30:35.612151 pyrandonaut-0.1.6/pyrandonaut.egg-info/
--rw-r--r--   0 aesthese   (501) staff       (20)     7143 2022-08-03 22:30:35.000000 pyrandonaut-0.1.6/pyrandonaut.egg-info/PKG-INFO
--rw-r--r--   0 aesthese   (501) staff       (20)      224 2022-08-03 22:30:35.000000 pyrandonaut-0.1.6/pyrandonaut.egg-info/SOURCES.txt
--rw-r--r--   0 aesthese   (501) staff       (20)        1 2022-08-03 22:30:35.000000 pyrandonaut-0.1.6/pyrandonaut.egg-info/dependency_links.txt
--rw-r--r--   0 aesthese   (501) staff       (20)       81 2022-08-03 22:30:35.000000 pyrandonaut-0.1.6/pyrandonaut.egg-info/requires.txt
--rw-r--r--   0 aesthese   (501) staff       (20)       12 2022-08-03 22:30:35.000000 pyrandonaut-0.1.6/pyrandonaut.egg-info/top_level.txt
--rw-r--r--   0 aesthese   (501) staff       (20)       38 2022-08-03 22:30:35.613092 pyrandonaut-0.1.6/setup.cfg
--rw-r--r--   0 aesthese   (501) staff       (20)     1588 2022-08-03 22:29:27.000000 pyrandonaut-0.1.6/setup.py
+drwx------   0 aesthese   (501) staff       (20)        0 2023-07-27 04:53:04.552708 pyrandonaut-0.1.7/
+-rw-------   0 aesthese   (501) staff       (20)    35149 2023-07-27 03:48:57.000000 pyrandonaut-0.1.7/LICENSE
+-rw-------   0 aesthese   (501) staff       (20)     7070 2023-07-27 04:53:04.552386 pyrandonaut-0.1.7/PKG-INFO
+-rw-------   0 aesthese   (501) staff       (20)     6313 2023-07-27 03:49:58.000000 pyrandonaut-0.1.7/README.md
+drwx------   0 aesthese   (501) staff       (20)        0 2023-07-27 04:53:04.549298 pyrandonaut-0.1.7/pyrandonaut/
+-rw-------   0 aesthese   (501) staff       (20)     7378 2023-07-27 04:48:00.000000 pyrandonaut-0.1.7/pyrandonaut/__init__.py
+drwx------   0 aesthese   (501) staff       (20)        0 2023-07-27 04:53:04.551955 pyrandonaut-0.1.7/pyrandonaut.egg-info/
+-rw-------   0 aesthese   (501) staff       (20)     7070 2023-07-27 04:53:04.000000 pyrandonaut-0.1.7/pyrandonaut.egg-info/PKG-INFO
+-rw-------   0 aesthese   (501) staff       (20)      224 2023-07-27 04:53:04.000000 pyrandonaut-0.1.7/pyrandonaut.egg-info/SOURCES.txt
+-rw-------   0 aesthese   (501) staff       (20)        1 2023-07-27 04:53:04.000000 pyrandonaut-0.1.7/pyrandonaut.egg-info/dependency_links.txt
+-rw-------   0 aesthese   (501) staff       (20)       84 2023-07-27 04:53:04.000000 pyrandonaut-0.1.7/pyrandonaut.egg-info/requires.txt
+-rw-------   0 aesthese   (501) staff       (20)       12 2023-07-27 04:53:04.000000 pyrandonaut-0.1.7/pyrandonaut.egg-info/top_level.txt
+-rw-------   0 aesthese   (501) staff       (20)       38 2023-07-27 04:53:04.552809 pyrandonaut-0.1.7/setup.cfg
+-rw-------   0 aesthese   (501) staff       (20)     1579 2023-07-27 04:53:02.000000 pyrandonaut-0.1.7/setup.py
```

### Comparing `pyrandonaut-0.1.6/LICENSE` & `pyrandonaut-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrandonaut-0.1.6/PKG-INFO` & `pyrandonaut-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyrandonaut
-Version: 0.1.6
+Version: 0.1.7
 Summary: Open-source quantum random coordinate generation for randonauts.
 Home-page: https://github.com/openrandonaut/pyrandonaut
 Author: narkopolo
 Author-email: openrandonaut@riseup.net
 License: GPL-3.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
@@ -22,15 +21,15 @@
 ## PyRandonaut
 ![Python](https://img.shields.io/badge/built%20with-Python3-red.svg)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
 
 ### Open-source quantum random coordinate generation for randonauts ❤️
 <img align="left" src="https://i.imgur.com/RJxATsu.png" width="170">
 
-This is a Python3 module for generating quantum random coordinates. It interfaces with the [QRNG](https://qrng.anu.edu.au/), at The Australian National University where it gets a list of [quantum random](https://en.wikipedia.org/wiki/Hardware_random_number_generator#Quantum_random_properties) numbers, converts them to coordinates and then computes the [gaussian kernel density estimate](https://en.wikipedia.org/wiki/Kernel_density_estimation) of those coordinates to find a point with a statistically anomalous density, similar to how an Attractor point is generated by [Randonautica](https://www.randonautica.com/).
+This is a Python3 module for generating quantum random coordinates. It interfaces with the QRNG at Randonautica where it gets a list of [quantum random](https://en.wikipedia.org/wiki/Hardware_random_number_generator#Quantum_random_properties) numbers, converts them to coordinates and then computes the [gaussian kernel density estimate](https://en.wikipedia.org/wiki/Kernel_density_estimation) of those coordinates to find a point with a statistically anomalous density, similar to how an Attractor point is generated by [Randonautica](https://www.randonautica.com/).
 	<br><br>
 	This gives you the ability to implement quantum random coordinates in your own applications. Just `import pyrandonaut` and off you go!
 	<br><br>
 	If you're unfamiliar with Randonautica, the concepts of Probability Blind-Spots and Quantum Randomness, I recommend reading [fatum_theory.txt](https://github.com/anonyhoney/fatum-en/blob/master/docs/fatum_theory.txt) which shipped with the original Fatum Project bot that inspired Randonautica. [This video](https://www.youtube.com/watch?v=6C6aXta3m1M) gives a lot of great background info too. If you have no idea what any of this is about and is completely new to this, watch [this video](https://www.youtube.com/watch?v=nDX81AUm8yE) and/or read [this article](https://medium.com/swlh/randonauts-how-a-random-number-generator-can-set-you-free-dfc2a2413e15).
 
 Contributions greatly appreciated!
 
@@ -59,15 +58,15 @@
 	
 	```python
 	# Define a starting point
 	my_latitude = 51.178840902136464
 	my_longitude = -1.8261452442305293
 	
 	# Call get_coordinate() with starting point values and store the result
-	result = openrandonaut.get_coordinate(my_latitude, my_longitude)	
+	result = pyrandonaut.get_coordinate(my_latitude, my_longitude)	
 	# Print result to screen
 	print(f"Go here to escape the stasis field: {result}")
 	``` 
 	`get_coordinate()` will return a tuple with the calculated coordinate. By default it uses a radius of 5000 meters and a value of 1024 random points to base the calculation on. These values can be specified in the arguments.
 	
 	* **Functions and arguments:**
 		* **`get_coordinate()`** is the main functionality of the library, generating a coordinate equivalent to an Attractor point in Randonautica. It takes the following arguments:
@@ -127,9 +126,7 @@
 
 ## To-do
 - [ ] Get people excited about the project!
 - [ ] Add more QRNG sources (If you can help supply hardware modules for testing, please get in touch!)
 - [ ] Make requests to ANU QRNG API asynchronous
 - [ ] Implement heatmap generation from [openrandonaut-bot](https://github.com/openrandonaut/openrandonaut-bot)
 - [ ] Add ability to calculate Void and Power points as well
-
-
```

### Comparing `pyrandonaut-0.1.6/README.md` & `pyrandonaut-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ## PyRandonaut
 ![Python](https://img.shields.io/badge/built%20with-Python3-red.svg)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
 
 ### Open-source quantum random coordinate generation for randonauts ❤️
 <img align="left" src="https://i.imgur.com/RJxATsu.png" width="170">
 
-This is a Python3 module for generating quantum random coordinates. It interfaces with the [QRNG](https://qrng.anu.edu.au/), at The Australian National University where it gets a list of [quantum random](https://en.wikipedia.org/wiki/Hardware_random_number_generator#Quantum_random_properties) numbers, converts them to coordinates and then computes the [gaussian kernel density estimate](https://en.wikipedia.org/wiki/Kernel_density_estimation) of those coordinates to find a point with a statistically anomalous density, similar to how an Attractor point is generated by [Randonautica](https://www.randonautica.com/).
+This is a Python3 module for generating quantum random coordinates. It interfaces with the QRNG at Randonautica where it gets a list of [quantum random](https://en.wikipedia.org/wiki/Hardware_random_number_generator#Quantum_random_properties) numbers, converts them to coordinates and then computes the [gaussian kernel density estimate](https://en.wikipedia.org/wiki/Kernel_density_estimation) of those coordinates to find a point with a statistically anomalous density, similar to how an Attractor point is generated by [Randonautica](https://www.randonautica.com/).
 	<br><br>
 	This gives you the ability to implement quantum random coordinates in your own applications. Just `import pyrandonaut` and off you go!
 	<br><br>
 	If you're unfamiliar with Randonautica, the concepts of Probability Blind-Spots and Quantum Randomness, I recommend reading [fatum_theory.txt](https://github.com/anonyhoney/fatum-en/blob/master/docs/fatum_theory.txt) which shipped with the original Fatum Project bot that inspired Randonautica. [This video](https://www.youtube.com/watch?v=6C6aXta3m1M) gives a lot of great background info too. If you have no idea what any of this is about and is completely new to this, watch [this video](https://www.youtube.com/watch?v=nDX81AUm8yE) and/or read [this article](https://medium.com/swlh/randonauts-how-a-random-number-generator-can-set-you-free-dfc2a2413e15).
 
 Contributions greatly appreciated!
 
@@ -38,15 +38,15 @@
 	
 	```python
 	# Define a starting point
 	my_latitude = 51.178840902136464
 	my_longitude = -1.8261452442305293
 	
 	# Call get_coordinate() with starting point values and store the result
-	result = openrandonaut.get_coordinate(my_latitude, my_longitude)	
+	result = pyrandonaut.get_coordinate(my_latitude, my_longitude)	
 	# Print result to screen
 	print(f"Go here to escape the stasis field: {result}")
 	``` 
 	`get_coordinate()` will return a tuple with the calculated coordinate. By default it uses a radius of 5000 meters and a value of 1024 random points to base the calculation on. These values can be specified in the arguments.
 	
 	* **Functions and arguments:**
 		* **`get_coordinate()`** is the main functionality of the library, generating a coordinate equivalent to an Attractor point in Randonautica. It takes the following arguments:
```

### Comparing `pyrandonaut-0.1.6/pyrandonaut/__init__.py` & `pyrandonaut-0.1.7/pyrandonaut/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,57 +8,66 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """This module interfaces with the Quantum Random Number Generator
-at the The Australian National University, where it gets a listof
-n truly random numbers, converts them to coordinates and computes the
-gaussian kernel density estimate of those coordinates, returning the
-point within the defined radius, where the density of random coordinates
+at Randonautica , where it gets a listof n truly random numbers, converts them 
+to coordinates and computes the gaussian kernel density estimate of those coordinates, 
+returning the point within the defined radius, where the density of random coordinates
 is highest, similar to how an Attractor point is calculated by Randonautica."""
 
 import argparse
 import logging
 import math
+import sys
+import binascii
+import ctypes
 
 import numpy as np
 import pandas as pd
-import quantumrandom
+import randonautentropy
 from scipy import stats
 
 __author__ = 'openrandonaut'
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 
 class Error(Exception):
     """Base class for other exceptions"""
 
 
 class DivisionError(Error):
     """Raised when number of requested point isn't divisible by 1024"""
 
 
 EARTH_RADIUS = 6371  # km
 ONE_DEGREE = EARTH_RADIUS * 2 * math.pi / 360 * 1000  # 1° latitude in meters
 
+def get_data(amount: int):
+    """Gets a string of 4096 bytes from Randonautica's QRNG
+       and turns it into a list of uint16 values"""
+    
+    hex_string = randonautentropy.rndo.get(4 * amount)
+    chunks = [hex_string[i:i+4] for i in range(0, len(hex_string), 4)]
+    return [ctypes.c_uint16(int(chunk, 16)).value for chunk in chunks]
 
 def int_to_float(input_integer: int) -> float:
     """Converts an integer to a floating point value"""
 
     source_bits = int(math.ceil(math.log(1 + 1, 2)))
-    source_size = int(math.ceil(source_bits / float(quantumrandom.INT_BITS)))
-    source_max = 2 ** (source_size * quantumrandom.INT_BITS) - 1
+    source_size = int(math.ceil(source_bits / 16.0))
+    source_max = 2 ** (source_size * 16) - 1
 
     modulos = source_max / 1
 
     while True:
         num = 0
         for _ in range(source_size):
-            num <<= quantumrandom.INT_BITS
+            num <<= 16
             num += input_integer
 
         if num >= modulos:
             return None
         return num / modulos
 
 
@@ -130,15 +139,15 @@
         value += 1
         logging.info(
             "Getting %d out of %d random unsigned 16-bit integers from QRNG...",
             1024 * value,
             num_points,
         )
         numbers.extend(
-            quantumrandom.get_data(data_type="uint16", array_length=1024, block_size=1)
+            get_data(1024)
         )
 
     logging.info("Converting integers to coordinates... ")
     coord_list = []
     # Iterate over numbers from QRNG in pairs and convert them to coordinates
     for value_1, value_2 in pairwise(numbers):
         value_1 = int_to_float(value_1)
@@ -157,19 +166,19 @@
 
 
 def main():
     """If run as a script, take arguments using argparse and print result to stdout"""
 
     parser = argparse.ArgumentParser(
         description="This script interfaces with the Quantum Random Number Generator\
-                     at the The Australian National University, where it gets a list of\
+                     at Randonautica, where it gets a list of\
                      quantum random numbers, converts them to coordinates and computes the\
                      gaussian kernel density estimate of those coordinates, returning the\
                      point within the defined radius, where the density of random coordinates\
-                     is highest, similar to how an Attractor point is calculated by Randonautica."
+                     is highest, similar to how an Attractor point is calculated by the Randonautica app."
     )
 
     parser.add_argument(
         "latitude", metavar="LATITUDE", type=float, help="starting position latitude"
     )
 
     parser.add_argument(
@@ -187,15 +196,15 @@
 
     parser.add_argument(
         "-p",
         metavar="POINTS",
         type=int,
         dest="points",
         default=4096,
-        help="number of points to base KDE on (must be divisible by 2014)",
+        help="number of points to base KDE on (must be divisible by 1024)",
     )
 
     parser.add_argument(
         "-v", action="store_true", dest="verbose", help="verbose logging"
     )
 
     args = parser.parse_args()
```

### Comparing `pyrandonaut-0.1.6/pyrandonaut.egg-info/PKG-INFO` & `pyrandonaut-0.1.7/pyrandonaut.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pyrandonaut
-Version: 0.1.6
+Version: 0.1.7
 Summary: Open-source quantum random coordinate generation for randonauts.
 Home-page: https://github.com/openrandonaut/pyrandonaut
 Author: narkopolo
 Author-email: openrandonaut@riseup.net
 License: GPL-3.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
@@ -22,15 +21,15 @@
 ## PyRandonaut
 ![Python](https://img.shields.io/badge/built%20with-Python3-red.svg)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
 
 ### Open-source quantum random coordinate generation for randonauts ❤️
 <img align="left" src="https://i.imgur.com/RJxATsu.png" width="170">
 
-This is a Python3 module for generating quantum random coordinates. It interfaces with the [QRNG](https://qrng.anu.edu.au/), at The Australian National University where it gets a list of [quantum random](https://en.wikipedia.org/wiki/Hardware_random_number_generator#Quantum_random_properties) numbers, converts them to coordinates and then computes the [gaussian kernel density estimate](https://en.wikipedia.org/wiki/Kernel_density_estimation) of those coordinates to find a point with a statistically anomalous density, similar to how an Attractor point is generated by [Randonautica](https://www.randonautica.com/).
+This is a Python3 module for generating quantum random coordinates. It interfaces with the QRNG at Randonautica where it gets a list of [quantum random](https://en.wikipedia.org/wiki/Hardware_random_number_generator#Quantum_random_properties) numbers, converts them to coordinates and then computes the [gaussian kernel density estimate](https://en.wikipedia.org/wiki/Kernel_density_estimation) of those coordinates to find a point with a statistically anomalous density, similar to how an Attractor point is generated by [Randonautica](https://www.randonautica.com/).
 	<br><br>
 	This gives you the ability to implement quantum random coordinates in your own applications. Just `import pyrandonaut` and off you go!
 	<br><br>
 	If you're unfamiliar with Randonautica, the concepts of Probability Blind-Spots and Quantum Randomness, I recommend reading [fatum_theory.txt](https://github.com/anonyhoney/fatum-en/blob/master/docs/fatum_theory.txt) which shipped with the original Fatum Project bot that inspired Randonautica. [This video](https://www.youtube.com/watch?v=6C6aXta3m1M) gives a lot of great background info too. If you have no idea what any of this is about and is completely new to this, watch [this video](https://www.youtube.com/watch?v=nDX81AUm8yE) and/or read [this article](https://medium.com/swlh/randonauts-how-a-random-number-generator-can-set-you-free-dfc2a2413e15).
 
 Contributions greatly appreciated!
 
@@ -59,15 +58,15 @@
 	
 	```python
 	# Define a starting point
 	my_latitude = 51.178840902136464
 	my_longitude = -1.8261452442305293
 	
 	# Call get_coordinate() with starting point values and store the result
-	result = openrandonaut.get_coordinate(my_latitude, my_longitude)	
+	result = pyrandonaut.get_coordinate(my_latitude, my_longitude)	
 	# Print result to screen
 	print(f"Go here to escape the stasis field: {result}")
 	``` 
 	`get_coordinate()` will return a tuple with the calculated coordinate. By default it uses a radius of 5000 meters and a value of 1024 random points to base the calculation on. These values can be specified in the arguments.
 	
 	* **Functions and arguments:**
 		* **`get_coordinate()`** is the main functionality of the library, generating a coordinate equivalent to an Attractor point in Randonautica. It takes the following arguments:
@@ -127,9 +126,7 @@
 
 ## To-do
 - [ ] Get people excited about the project!
 - [ ] Add more QRNG sources (If you can help supply hardware modules for testing, please get in touch!)
 - [ ] Make requests to ANU QRNG API asynchronous
 - [ ] Implement heatmap generation from [openrandonaut-bot](https://github.com/openrandonaut/openrandonaut-bot)
 - [ ] Add ability to calculate Void and Power points as well
-
-
```

### Comparing `pyrandonaut-0.1.6/setup.py` & `pyrandonaut-0.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,43 +6,43 @@
 
 with open('README.md') as readme_file:
     long_description = readme_file.read()
 
 
 # 'setup.py publish' shortcut.
 if argv[-1] == 'publish':
-    os.system('python setup.py sdist bdist_wheel')
+    os.system('python setup.py sdist')
     os.system('twine upload dist/*')
     exit()
 elif argv[-1] == 'clean':
     import shutil
     if os.path.isdir('build'):
         shutil.rmtree('build')
     if os.path.isdir('dist'):
         shutil.rmtree('dist')
     if os.path.isdir('pyrandonaut.egg-info'):
         shutil.rmtree('pyrandonaut.egg-info')
 
 
 setup(
     name="pyrandonaut",
-    version="0.1.6",
+    version="0.1.7",
     description="Open-source quantum random coordinate generation for randonauts.",
     long_description_content_type='text/markdown',
     long_description=long_description,
     url="https://github.com/openrandonaut/pyrandonaut",
     author="narkopolo",
     author_email="openrandonaut@riseup.net",
     license="GPL-3.0",
     packages=["pyrandonaut"],
     python_requires=">=3.9",
     install_requires=[
     "numpy==1.23.1",
     "pandas==1.4.3",
-    "quantumrandom==1.9.0",
+    "randonautentropy==1.0.2",
     "scipy==1.9.0",
     "setuptools==58.1.0"
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         'Topic :: System :: Installation/Setup',
         "Intended Audience :: Developers",
```

