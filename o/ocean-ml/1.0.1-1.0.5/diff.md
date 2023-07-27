# Comparing `tmp/ocean-ml-1.0.1.tar.gz` & `tmp/ocean-ml-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocean-ml-1.0.1.tar", last modified: Sat Jul 22 16:09:01 2023, max compression
+gzip compressed data, was "ocean-ml-1.0.5.tar", last modified: Thu Jul 27 07:58:39 2023, max compression
```

## Comparing `ocean-ml-1.0.1.tar` & `ocean-ml-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 16:09:01.136904 ocean-ml-1.0.1/
--rw-rw-rw-   0        0        0     1088 2023-07-22 11:34:30.000000 ocean-ml-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1366 2023-07-22 16:09:01.135906 ocean-ml-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      891 2023-07-22 15:47:55.000000 ocean-ml-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 16:09:01.118262 ocean-ml-1.0.1/ocean/
--rw-rw-rw-   0        0        0      284 2023-07-12 08:52:40.000000 ocean-ml-1.0.1/ocean/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 16:09:01.121689 ocean-ml-1.0.1/ocean/automl/
--rw-rw-rw-   0        0        0      289 2023-07-12 08:52:17.000000 ocean-ml-1.0.1/ocean/automl/__init__.py
--rw-rw-rw-   0        0        0    20495 2023-07-21 02:51:03.000000 ocean-ml-1.0.1/ocean/automl/_auto.py
--rw-rw-rw-   0        0        0     3088 2023-07-21 02:51:54.000000 ocean-ml-1.0.1/ocean/automl/_params.py
--rw-rw-rw-   0        0        0     1107 2023-07-21 02:52:28.000000 ocean-ml-1.0.1/ocean/automl/_prep.py
--rw-rw-rw-   0        0        0    16620 2023-07-21 02:54:02.000000 ocean-ml-1.0.1/ocean/automl/_result.py
-drwxrwxrwx   0        0        0        0 2023-07-22 16:09:01.135906 ocean-ml-1.0.1/ocean_ml.egg-info/
--rw-rw-rw-   0        0        0     1366 2023-07-22 16:09:01.000000 ocean-ml-1.0.1/ocean_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-07-22 16:09:01.000000 ocean-ml-1.0.1/ocean_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 16:09:01.000000 ocean-ml-1.0.1/ocean_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-07-22 16:09:01.000000 ocean-ml-1.0.1/ocean_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-22 16:09:01.000000 ocean-ml-1.0.1/ocean_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 16:09:01.136904 ocean-ml-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1407 2023-07-22 16:08:06.000000 ocean-ml-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:58:39.601096 ocean-ml-1.0.5/
+-rw-rw-rw-   0        0        0     1088 2023-07-22 11:34:30.000000 ocean-ml-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1307 2023-07-27 07:58:39.599728 ocean-ml-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      834 2023-07-27 07:29:23.000000 ocean-ml-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 07:58:39.538932 ocean-ml-1.0.5/ocean/
+-rw-rw-rw-   0        0        0      357 2023-07-27 07:19:56.000000 ocean-ml-1.0.5/ocean/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:58:39.539960 ocean-ml-1.0.5/ocean/automl/
+-rw-rw-rw-   0        0        0      120 2023-07-27 07:17:18.000000 ocean-ml-1.0.5/ocean/automl/__init__.py
+-rw-rw-rw-   0        0        0    20495 2023-07-25 03:36:43.000000 ocean-ml-1.0.5/ocean/automl/_auto.py
+-rw-rw-rw-   0        0        0     3088 2023-07-21 02:51:54.000000 ocean-ml-1.0.5/ocean/automl/_params.py
+-rw-rw-rw-   0        0        0     1107 2023-07-21 02:52:28.000000 ocean-ml-1.0.5/ocean/automl/_prep.py
+-rw-rw-rw-   0        0        0    16620 2023-07-25 03:37:12.000000 ocean-ml-1.0.5/ocean/automl/_result.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:58:39.552395 ocean-ml-1.0.5/ocean/preprocessing/
+-rw-rw-rw-   0        0        0       82 2023-07-27 07:20:48.000000 ocean-ml-1.0.5/ocean/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     4540 2023-07-27 07:20:46.000000 ocean-ml-1.0.5/ocean/preprocessing/_flow.py
+-rw-rw-rw-   0        0        0     2674 2023-07-27 07:20:42.000000 ocean-ml-1.0.5/ocean/preprocessing/_preprocessing.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:58:39.555190 ocean-ml-1.0.5/ocean/save_load_model/
+-rw-rw-rw-   0        0        0      115 2023-07-27 07:16:44.000000 ocean-ml-1.0.5/ocean/save_load_model/__init__.py
+-rw-rw-rw-   0        0        0      637 2023-07-27 07:16:44.000000 ocean-ml-1.0.5/ocean/save_load_model/_load.py
+-rw-rw-rw-   0        0        0      716 2023-07-27 07:16:44.000000 ocean-ml-1.0.5/ocean/save_load_model/_save.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:58:39.595688 ocean-ml-1.0.5/ocean_ml.egg-info/
+-rw-rw-rw-   0        0        0     1307 2023-07-27 07:58:39.000000 ocean-ml-1.0.5/ocean_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2023-07-27 07:58:39.000000 ocean-ml-1.0.5/ocean_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 07:58:39.000000 ocean-ml-1.0.5/ocean_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-07-27 07:58:39.000000 ocean-ml-1.0.5/ocean_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-27 07:58:39.000000 ocean-ml-1.0.5/ocean_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 07:58:39.601096 ocean-ml-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1427 2023-07-27 07:55:43.000000 ocean-ml-1.0.5/setup.py
```

### Comparing `ocean-ml-1.0.1/LICENSE.txt` & `ocean-ml-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ocean-ml-1.0.1/PKG-INFO` & `ocean-ml-1.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocean-ml
-Version: 1.0.1
+Version: 1.0.5
 Home-page: https://github.com/AgufSamudra/ocean
 Author: Gufranaka Samudra
 Author-email: gufranakasamudra348@gmail.com
 License: MIT
 Keywords: python,ocean,machine,learning,machinelearning,automl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,42 +16,39 @@
 
 ## Easy ML workflows built on scikit-learn
 
 Ocean is a package for machine learning workflows that makes it easier to create models. It is made using several tools from scikit-learn, to speed up the machine learning process.
 
 ## Feature
 
-This package will continue to be developed to add more features, but for now there is only one feature, namely automl.
+This package will continue to be developed to add more features, here are some features
+which is in package ocean
 
 - automl
+- preprocessing
+- save and load model
 
 ## Dependency
 
 ```console
 numpy==1.25.1
 scikit-learn==1.3.0
 scipy==1.11.1
 tabulate==0.9.0
 xgboost==1.7.6
+pandas==2.0.3
 ```
 
 ## How to Install
 
 You can install ocean with pip using this command:
 ```console
 pip install ocean-ml
 ```
 
-## Example
+## Pypi Link
 
-#### AutoML
-
-```python
-from ocean.automl import AutoMLRegressor
-
-model = AutoMLRegressor(X, y, categoric, tune_params=True)
-model.fit()
-```
+https://pypi.org/project/ocean-ml/
 
 ## Github Link
 https://github.com/AgufSamudra/ocean <br>
 [Ocean](https://github.com/AgufSamudra/ocean)
```

### Comparing `ocean-ml-1.0.1/ocean/automl/_auto.py` & `ocean-ml-1.0.5/ocean/automl/_auto.py`

 * *Files identical despite different names*

### Comparing `ocean-ml-1.0.1/ocean/automl/_params.py` & `ocean-ml-1.0.5/ocean/automl/_params.py`

 * *Files identical despite different names*

### Comparing `ocean-ml-1.0.1/ocean/automl/_prep.py` & `ocean-ml-1.0.5/ocean/automl/_prep.py`

 * *Files identical despite different names*

### Comparing `ocean-ml-1.0.1/ocean/automl/_result.py` & `ocean-ml-1.0.5/ocean/automl/_result.py`

 * *Files identical despite different names*

### Comparing `ocean-ml-1.0.1/ocean_ml.egg-info/PKG-INFO` & `ocean-ml-1.0.5/ocean_ml.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocean-ml
-Version: 1.0.1
+Version: 1.0.5
 Home-page: https://github.com/AgufSamudra/ocean
 Author: Gufranaka Samudra
 Author-email: gufranakasamudra348@gmail.com
 License: MIT
 Keywords: python,ocean,machine,learning,machinelearning,automl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,42 +16,39 @@
 
 ## Easy ML workflows built on scikit-learn
 
 Ocean is a package for machine learning workflows that makes it easier to create models. It is made using several tools from scikit-learn, to speed up the machine learning process.
 
 ## Feature
 
-This package will continue to be developed to add more features, but for now there is only one feature, namely automl.
+This package will continue to be developed to add more features, here are some features
+which is in package ocean
 
 - automl
+- preprocessing
+- save and load model
 
 ## Dependency
 
 ```console
 numpy==1.25.1
 scikit-learn==1.3.0
 scipy==1.11.1
 tabulate==0.9.0
 xgboost==1.7.6
+pandas==2.0.3
 ```
 
 ## How to Install
 
 You can install ocean with pip using this command:
 ```console
 pip install ocean-ml
 ```
 
-## Example
+## Pypi Link
 
-#### AutoML
-
-```python
-from ocean.automl import AutoMLRegressor
-
-model = AutoMLRegressor(X, y, categoric, tune_params=True)
-model.fit()
-```
+https://pypi.org/project/ocean-ml/
 
 ## Github Link
 https://github.com/AgufSamudra/ocean <br>
 [Ocean](https://github.com/AgufSamudra/ocean)
```

### Comparing `ocean-ml-1.0.1/setup.py` & `ocean-ml-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 	long_description = fh.read()
 
 setuptools.setup(
 	# Here is the module name.
 	name="ocean-ml",
 
 	# version of the module
-	version="1.0.1",
+	version="1.0.5",
 
 	# Name of Author
 	author="Gufranaka Samudra",
 
 	# your Email address
 	author_email="gufranakasamudra348@gmail.com",
 
@@ -34,15 +34,16 @@
 	# then you must add there, in order to download every requirement of package
 
 	install_requires=[
 		"numpy==1.25.1",
 		"scikit-learn==1.3.0",
 		"scipy==1.11.1",
 		"tabulate==0.9.0",
-		"xgboost==1.7.6"
+		"xgboost==1.7.6",
+		"pandas==2.0.3"
      ],
  
 	keywords=['python', 'ocean', 'machine', 'learning', 'machinelearning', 'automl'],
 
 
 	license="MIT",
```

