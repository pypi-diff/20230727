# Comparing `tmp/mlforce-0.1.0.tar.gz` & `tmp/mlforce-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlforce-0.1.0.tar", last modified: Thu Jul 27 18:46:31 2023, max compression
+gzip compressed data, was "mlforce-0.1.1.tar", last modified: Thu Jul 27 19:09:26 2023, max compression
```

## Comparing `mlforce-0.1.0.tar` & `mlforce-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jiarui     (501) staff       (20)        0 2023-07-27 18:46:31.046475 mlforce-0.1.0/
--rw-r--r--   0 jiarui     (501) staff       (20)     3342 2023-07-27 18:46:31.046336 mlforce-0.1.0/PKG-INFO
--rw-r--r--   0 jiarui     (501) staff       (20)     2858 2023-07-27 18:30:31.000000 mlforce-0.1.0/README.md
-drwxr-xr-x   0 jiarui     (501) staff       (20)        0 2023-07-27 18:46:31.046155 mlforce-0.1.0/mlforce.egg-info/
--rw-r--r--   0 jiarui     (501) staff       (20)     3342 2023-07-27 18:46:31.000000 mlforce-0.1.0/mlforce.egg-info/PKG-INFO
--rw-r--r--   0 jiarui     (501) staff       (20)      172 2023-07-27 18:46:31.000000 mlforce-0.1.0/mlforce.egg-info/SOURCES.txt
--rw-r--r--   0 jiarui     (501) staff       (20)        1 2023-07-27 18:46:31.000000 mlforce-0.1.0/mlforce.egg-info/dependency_links.txt
--rw-r--r--   0 jiarui     (501) staff       (20)       98 2023-07-27 18:46:31.000000 mlforce-0.1.0/mlforce.egg-info/requires.txt
--rw-r--r--   0 jiarui     (501) staff       (20)        1 2023-07-27 18:46:31.000000 mlforce-0.1.0/mlforce.egg-info/top_level.txt
--rw-r--r--   0 jiarui     (501) staff       (20)       38 2023-07-27 18:46:31.046522 mlforce-0.1.0/setup.cfg
--rw-r--r--   0 jiarui     (501) staff       (20)     1033 2023-07-27 18:42:35.000000 mlforce-0.1.0/setup.py
+drwxr-xr-x   0 jiarui     (501) staff       (20)        0 2023-07-27 19:09:26.934064 mlforce-0.1.1/
+-rw-r--r--   0 jiarui     (501) staff       (20)     3336 2023-07-27 19:09:26.933932 mlforce-0.1.1/PKG-INFO
+-rw-r--r--   0 jiarui     (501) staff       (20)     2854 2023-07-27 19:08:18.000000 mlforce-0.1.1/README.md
+drwxr-xr-x   0 jiarui     (501) staff       (20)        0 2023-07-27 19:09:26.933778 mlforce-0.1.1/mlforce.egg-info/
+-rw-r--r--   0 jiarui     (501) staff       (20)     3336 2023-07-27 19:09:26.000000 mlforce-0.1.1/mlforce.egg-info/PKG-INFO
+-rw-r--r--   0 jiarui     (501) staff       (20)      172 2023-07-27 19:09:26.000000 mlforce-0.1.1/mlforce.egg-info/SOURCES.txt
+-rw-r--r--   0 jiarui     (501) staff       (20)        1 2023-07-27 19:09:26.000000 mlforce-0.1.1/mlforce.egg-info/dependency_links.txt
+-rw-r--r--   0 jiarui     (501) staff       (20)       98 2023-07-27 19:09:26.000000 mlforce-0.1.1/mlforce.egg-info/requires.txt
+-rw-r--r--   0 jiarui     (501) staff       (20)        1 2023-07-27 19:09:26.000000 mlforce-0.1.1/mlforce.egg-info/top_level.txt
+-rw-r--r--   0 jiarui     (501) staff       (20)       38 2023-07-27 19:09:26.934116 mlforce-0.1.1/setup.cfg
+-rw-r--r--   0 jiarui     (501) staff       (20)     1031 2023-07-27 19:08:38.000000 mlforce-0.1.1/setup.py
```

### Comparing `mlforce-0.1.0/PKG-INFO` & `mlforce-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: mlforce
-Version: 0.1.0
+Version: 0.1.1
 Summary: Easy-to-use toolkit with numpy, pandas, and PyTorch for beginners
-Home-page: https://github.com/XavierSpycy/MLStarter
+Home-page: https://github.com/XavierSpycy/MLForce
 Author: Jiarui Xu
 Author-email: xujiarui98@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: data
 
-# Machine Learning Starter
+# Machine Learning Force -- MLForce
 
 ## Introduction
-My library, named "MLStarter" which stands for Machine Learning Starter, is a comprehensive Python toolkit meticulously crafted to cater to the needs of machine learning beginners. With a user-friendly design, it aims to empower aspiring data enthusiasts and learners in the fields of machine learning and data analysis. Each module in "MLStarter" serves a distinct purpose, providing a seamless and efficient experience for users throughout the entire machine learning journey.
+My library, named "MLForce" which stands for Machine Learning Force, is a comprehensive Python toolkit meticulously crafted to cater to the needs of machine learning beginners. With a user-friendly design, it aims to empower aspiring data enthusiasts and learners in the fields of machine learning and data analysis. Each module in "MLForce" serves a distinct purpose, providing a seamless and efficient experience for users throughout the entire machine learning journey.
 
 By combining ease of use with powerful functionality, this library aims to nurture your understanding and practical skills in machine learning, unlocking the doors to endless possibilities in the realm of data-driven solutions. So, embrace "MaLL" and embark on a rewarding journey of mastering the art of machine learning!
 
 ## Installation
-You can install MLStarter using pip:
+You can install MLForce using pip:
 ```
-pip install mlstarter
+pip install mlforce
 ```
 
 ## Quick Start
 Here's a quick example of how to use MLStarter Library:
 
 ```python
 # Import modules
-from mlstarter.datasets import StandardDataset
-from mlstarter.mlsolutions import KNearestNeighbor
+from mlforce.datasets import StandardDataset
+from mlforce.mlsolutions import KNearestNeighbor
 
 # Load the datasets
 ds = StandardDataset()
 ds.load_knn('numeric')
 X, y = ds.data, ds.target
 new_example = ds.new_example 
 
@@ -66,20 +66,20 @@
 * scipy
 * torch
 
 ## Documentation
 For more detailed usage instructions, check out the Documentation.
 
 ## Contributing
-Contributions are welcome! If you find any issues or have suggestions for improvement, please [Open an issue](https://github.com/XavierSpycy/MLStarter/issues) or submit a pull request.
+Contributions are welcome! If you find any issues or have suggestions for improvement, please [Open an issue](https://github.com/XavierSpycy/MLForce/issues) or submit a pull request.
 
 
 ## License
 MaLL is licensed under the MIT License.
 
 ## Version History
-- v0.1.0 (2023-07-28)
-  * Initial release of MaLL.
+- v0.1.1 (2023-07-28)
+  * Initial release of mlforce.
 
 ## Author and contact:
 Author: Jiarui Xu      
 Email: xujiarui98@foxmail.com
```

### Comparing `mlforce-0.1.0/README.md` & `mlforce-0.1.1/mlforce.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,42 @@
-# Machine Learning Starter
+Metadata-Version: 2.1
+Name: mlforce
+Version: 0.1.1
+Summary: Easy-to-use toolkit with numpy, pandas, and PyTorch for beginners
+Home-page: https://github.com/XavierSpycy/MLForce
+Author: Jiarui Xu
+Author-email: xujiarui98@foxmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: data
+
+# Machine Learning Force -- MLForce
 
 ## Introduction
-My library, named "MLStarter" which stands for Machine Learning Starter, is a comprehensive Python toolkit meticulously crafted to cater to the needs of machine learning beginners. With a user-friendly design, it aims to empower aspiring data enthusiasts and learners in the fields of machine learning and data analysis. Each module in "MLStarter" serves a distinct purpose, providing a seamless and efficient experience for users throughout the entire machine learning journey.
+My library, named "MLForce" which stands for Machine Learning Force, is a comprehensive Python toolkit meticulously crafted to cater to the needs of machine learning beginners. With a user-friendly design, it aims to empower aspiring data enthusiasts and learners in the fields of machine learning and data analysis. Each module in "MLForce" serves a distinct purpose, providing a seamless and efficient experience for users throughout the entire machine learning journey.
 
 By combining ease of use with powerful functionality, this library aims to nurture your understanding and practical skills in machine learning, unlocking the doors to endless possibilities in the realm of data-driven solutions. So, embrace "MaLL" and embark on a rewarding journey of mastering the art of machine learning!
 
 ## Installation
-You can install MLStarter using pip:
+You can install MLForce using pip:
 ```
-pip install mlstarter
+pip install mlforce
 ```
 
 ## Quick Start
 Here's a quick example of how to use MLStarter Library:
 
 ```python
 # Import modules
-from mlstarter.datasets import StandardDataset
-from mlstarter.mlsolutions import KNearestNeighbor
+from mlforce.datasets import StandardDataset
+from mlforce.mlsolutions import KNearestNeighbor
 
 # Load the datasets
 ds = StandardDataset()
 ds.load_knn('numeric')
 X, y = ds.data, ds.target
 new_example = ds.new_example 
 
@@ -51,20 +66,20 @@
 * scipy
 * torch
 
 ## Documentation
 For more detailed usage instructions, check out the Documentation.
 
 ## Contributing
-Contributions are welcome! If you find any issues or have suggestions for improvement, please [Open an issue](https://github.com/XavierSpycy/MLStarter/issues) or submit a pull request.
+Contributions are welcome! If you find any issues or have suggestions for improvement, please [Open an issue](https://github.com/XavierSpycy/MLForce/issues) or submit a pull request.
 
 
 ## License
 MaLL is licensed under the MIT License.
 
 ## Version History
-- v0.1.0 (2023-07-28)
-  * Initial release of MaLL.
+- v0.1.1 (2023-07-28)
+  * Initial release of mlforce.
 
 ## Author and contact:
 Author: Jiarui Xu      
 Email: xujiarui98@foxmail.com
```

### Comparing `mlforce-0.1.0/setup.py` & `mlforce-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mlforce",
-    version="0.1.0",
+    version="0.1.1",
     author="Jiarui Xu",
     author_email="xujiarui98@foxmail.com",
     description="Easy-to-use toolkit with numpy, pandas, and PyTorch for beginners",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/XavierSpycy/MLStarter",
+    url="https://github.com/XavierSpycy/MLForce",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```

