# Comparing `tmp/mlforce-0.1.1.tar.gz` & `tmp/mlforce-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforce-0.1.1.tar", last modified: Thu Jul 27 19:09:26 2023, max compression
+gzip compressed data, was "mlforce-0.1.2.tar", last modified: Thu Jul 27 21:53:16 2023, max compression
```

## Comparing `mlforce-0.1.1.tar` & `mlforce-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxr-xr-x   0 jiarui     (501) staff       (20)        0 2023-07-27 19:09:26.934064 mlforce-0.1.1/
--rw-r--r--   0 jiarui     (501) staff       (20)     3336 2023-07-27 19:09:26.933932 mlforce-0.1.1/PKG-INFO
--rw-r--r--   0 jiarui     (501) staff       (20)     2854 2023-07-27 19:08:18.000000 mlforce-0.1.1/README.md
-drwxr-xr-x   0 jiarui     (501) staff       (20)        0 2023-07-27 19:09:26.933778 mlforce-0.1.1/mlforce.egg-info/
--rw-r--r--   0 jiarui     (501) staff       (20)     3336 2023-07-27 19:09:26.000000 mlforce-0.1.1/mlforce.egg-info/PKG-INFO
--rw-r--r--   0 jiarui     (501) staff       (20)      172 2023-07-27 19:09:26.000000 mlforce-0.1.1/mlforce.egg-info/SOURCES.txt
--rw-r--r--   0 jiarui     (501) staff       (20)        1 2023-07-27 19:09:26.000000 mlforce-0.1.1/mlforce.egg-info/dependency_links.txt
--rw-r--r--   0 jiarui     (501) staff       (20)       98 2023-07-27 19:09:26.000000 mlforce-0.1.1/mlforce.egg-info/requires.txt
--rw-r--r--   0 jiarui     (501) staff       (20)        1 2023-07-27 19:09:26.000000 mlforce-0.1.1/mlforce.egg-info/top_level.txt
--rw-r--r--   0 jiarui     (501) staff       (20)       38 2023-07-27 19:09:26.934116 mlforce-0.1.1/setup.cfg
--rw-r--r--   0 jiarui     (501) staff       (20)     1031 2023-07-27 19:08:38.000000 mlforce-0.1.1/setup.py
+drwxr-xr-x   0 jiarui     (501) staff       (20)        0 2023-07-27 21:53:16.744063 mlforce-0.1.2/
+-rw-r--r--   0 jiarui     (501) staff       (20)     3306 2023-07-27 21:53:16.743933 mlforce-0.1.2/PKG-INFO
+-rw-r--r--   0 jiarui     (501) staff       (20)     2865 2023-07-27 21:51:06.000000 mlforce-0.1.2/README.md
+drwxr-xr-x   0 jiarui     (501) staff       (20)        0 2023-07-27 21:53:16.743191 mlforce-0.1.2/mlforce/
+-rw-r--r--   0 jiarui     (501) staff       (20)        0 2023-06-24 00:50:17.000000 mlforce-0.1.2/mlforce/__init__.py
+-rw-r--r--   0 jiarui     (501) staff       (20)    20822 2023-07-27 16:17:07.000000 mlforce-0.1.2/mlforce/datasets.py
+-rw-r--r--   0 jiarui     (501) staff       (20)    11577 2023-06-26 13:45:10.000000 mlforce-0.1.2/mlforce/digitrecognizer.py
+-rw-r--r--   0 jiarui     (501) staff       (20)    21728 2023-07-27 12:06:38.000000 mlforce-0.1.2/mlforce/mlperceptron.py
+-rw-r--r--   0 jiarui     (501) staff       (20)    60193 2023-07-27 14:51:23.000000 mlforce-0.1.2/mlforce/mlsolutions.py
+drwxr-xr-x   0 jiarui     (501) staff       (20)        0 2023-07-27 21:53:16.743780 mlforce-0.1.2/mlforce.egg-info/
+-rw-r--r--   0 jiarui     (501) staff       (20)     3306 2023-07-27 21:53:16.000000 mlforce-0.1.2/mlforce.egg-info/PKG-INFO
+-rw-r--r--   0 jiarui     (501) staff       (20)      286 2023-07-27 21:53:16.000000 mlforce-0.1.2/mlforce.egg-info/SOURCES.txt
+-rw-r--r--   0 jiarui     (501) staff       (20)        1 2023-07-27 21:53:16.000000 mlforce-0.1.2/mlforce.egg-info/dependency_links.txt
+-rw-r--r--   0 jiarui     (501) staff       (20)       25 2023-07-27 21:53:16.000000 mlforce-0.1.2/mlforce.egg-info/requires.txt
+-rw-r--r--   0 jiarui     (501) staff       (20)        8 2023-07-27 21:53:16.000000 mlforce-0.1.2/mlforce.egg-info/top_level.txt
+-rw-r--r--   0 jiarui     (501) staff       (20)       38 2023-07-27 21:53:16.744103 mlforce-0.1.2/setup.cfg
+-rw-r--r--   0 jiarui     (501) staff       (20)      799 2023-07-27 21:44:53.000000 mlforce-0.1.2/setup.py
```

### Comparing `mlforce-0.1.1/PKG-INFO` & `mlforce-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: mlforce
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy-to-use toolkit with numpy, pandas, and PyTorch for beginners
 Home-page: https://github.com/XavierSpycy/MLForce
 Author: Jiarui Xu
 Author-email: xujiarui98@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: data
 
 # Machine Learning Force -- MLForce
 
 ## Introduction
 My library, named "MLForce" which stands for Machine Learning Force, is a comprehensive Python toolkit meticulously crafted to cater to the needs of machine learning beginners. With a user-friendly design, it aims to empower aspiring data enthusiasts and learners in the fields of machine learning and data analysis. Each module in "MLForce" serves a distinct purpose, providing a seamless and efficient experience for users throughout the entire machine learning journey.
 
-By combining ease of use with powerful functionality, this library aims to nurture your understanding and practical skills in machine learning, unlocking the doors to endless possibilities in the realm of data-driven solutions. So, embrace "MaLL" and embark on a rewarding journey of mastering the art of machine learning!
+By combining ease of use with powerful functionality, this library aims to nurture your understanding and practical skills in machine learning, unlocking the doors to endless possibilities in the realm of data-driven solutions. So, embrace "MLForce" and embark on a rewarding journey of mastering the art of machine learning!
 
 ## Installation
 You can install MLForce using pip:
 ```
 pip install mlforce
 ```
 
@@ -73,13 +71,13 @@
 Contributions are welcome! If you find any issues or have suggestions for improvement, please [Open an issue](https://github.com/XavierSpycy/MLForce/issues) or submit a pull request.
 
 
 ## License
 MaLL is licensed under the MIT License.
 
 ## Version History
-- v0.1.1 (2023-07-28)
+- v0.1.0 - 0.1.2 (2023-07-28)
   * Initial release of mlforce.
 
 ## Author and contact:
 Author: Jiarui Xu      
 Email: xujiarui98@foxmail.com
```

### Comparing `mlforce-0.1.1/README.md` & `mlforce-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Machine Learning Force -- MLForce
 
 ## Introduction
 My library, named "MLForce" which stands for Machine Learning Force, is a comprehensive Python toolkit meticulously crafted to cater to the needs of machine learning beginners. With a user-friendly design, it aims to empower aspiring data enthusiasts and learners in the fields of machine learning and data analysis. Each module in "MLForce" serves a distinct purpose, providing a seamless and efficient experience for users throughout the entire machine learning journey.
 
-By combining ease of use with powerful functionality, this library aims to nurture your understanding and practical skills in machine learning, unlocking the doors to endless possibilities in the realm of data-driven solutions. So, embrace "MaLL" and embark on a rewarding journey of mastering the art of machine learning!
+By combining ease of use with powerful functionality, this library aims to nurture your understanding and practical skills in machine learning, unlocking the doors to endless possibilities in the realm of data-driven solutions. So, embrace "MLForce" and embark on a rewarding journey of mastering the art of machine learning!
 
 ## Installation
 You can install MLForce using pip:
 ```
 pip install mlforce
 ```
 
@@ -58,13 +58,13 @@
 Contributions are welcome! If you find any issues or have suggestions for improvement, please [Open an issue](https://github.com/XavierSpycy/MLForce/issues) or submit a pull request.
 
 
 ## License
 MaLL is licensed under the MIT License.
 
 ## Version History
-- v0.1.1 (2023-07-28)
+- v0.1.0 - 0.1.2 (2023-07-28)
   * Initial release of mlforce.
 
 ## Author and contact:
 Author: Jiarui Xu      
 Email: xujiarui98@foxmail.com
```

### Comparing `mlforce-0.1.1/mlforce.egg-info/PKG-INFO` & `mlforce-0.1.2/mlforce.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: mlforce
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy-to-use toolkit with numpy, pandas, and PyTorch for beginners
 Home-page: https://github.com/XavierSpycy/MLForce
 Author: Jiarui Xu
 Author-email: xujiarui98@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: data
 
 # Machine Learning Force -- MLForce
 
 ## Introduction
 My library, named "MLForce" which stands for Machine Learning Force, is a comprehensive Python toolkit meticulously crafted to cater to the needs of machine learning beginners. With a user-friendly design, it aims to empower aspiring data enthusiasts and learners in the fields of machine learning and data analysis. Each module in "MLForce" serves a distinct purpose, providing a seamless and efficient experience for users throughout the entire machine learning journey.
 
-By combining ease of use with powerful functionality, this library aims to nurture your understanding and practical skills in machine learning, unlocking the doors to endless possibilities in the realm of data-driven solutions. So, embrace "MaLL" and embark on a rewarding journey of mastering the art of machine learning!
+By combining ease of use with powerful functionality, this library aims to nurture your understanding and practical skills in machine learning, unlocking the doors to endless possibilities in the realm of data-driven solutions. So, embrace "MLForce" and embark on a rewarding journey of mastering the art of machine learning!
 
 ## Installation
 You can install MLForce using pip:
 ```
 pip install mlforce
 ```
 
@@ -73,13 +71,13 @@
 Contributions are welcome! If you find any issues or have suggestions for improvement, please [Open an issue](https://github.com/XavierSpycy/MLForce/issues) or submit a pull request.
 
 
 ## License
 MaLL is licensed under the MIT License.
 
 ## Version History
-- v0.1.1 (2023-07-28)
+- v0.1.0 - 0.1.2 (2023-07-28)
   * Initial release of mlforce.
 
 ## Author and contact:
 Author: Jiarui Xu      
 Email: xujiarui98@foxmail.com
```

### Comparing `mlforce-0.1.1/setup.py` & `mlforce-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mlforce",
-    version="0.1.1",
+    version="0.1.2",
     author="Jiarui Xu",
     author_email="xujiarui98@foxmail.com",
     description="Easy-to-use toolkit with numpy, pandas, and PyTorch for beginners",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/XavierSpycy/MLForce",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     install_requires=[
-        "numpy>=1.24.0",
-        "pandas>=1.5.3",
-        "scipy>=1.10.0",
-        "torch>=2.0.0",
+        "numpy",
+        "pandas",
+        "scipy",
+        "torch",
     ],
-    extras_require={
-        "dev": [
-            "pytest>=6.0.0",
-            "sphinx>=4.0.0",
-        ],
-        "data": [
-            #"pandas>=1.2.0",
-            #"scipy>=1.5.0",
-        ],
-    },
 )
```

