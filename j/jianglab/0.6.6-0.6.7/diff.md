# Comparing `tmp/jianglab-0.6.6.tar.gz` & `tmp/jianglab-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.6.6.tar", last modified: Thu Jul 27 16:10:01 2023, max compression
+gzip compressed data, was "jianglab-0.6.7.tar", last modified: Thu Jul 27 16:13:39 2023, max compression
```

## Comparing `jianglab-0.6.6.tar` & `jianglab-0.6.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:10:01.755661 jianglab-0.6.6/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:10:01.755137 jianglab-0.6.6/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.6.6/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:10:01.750720 jianglab-0.6.6/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.6.6/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    46512 2023-07-27 16:09:35.000000 jianglab-0.6.6/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.6.6/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:10:01.754251 jianglab-0.6.6/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:10:01.000000 jianglab-0.6.6/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-27 16:10:01.000000 jianglab-0.6.6/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-27 16:10:01.000000 jianglab-0.6.6/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      147 2023-07-27 16:10:01.000000 jianglab-0.6.6/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-27 16:10:01.000000 jianglab-0.6.6/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-27 16:10:01.755827 jianglab-0.6.6/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1119 2023-07-27 16:09:53.000000 jianglab-0.6.6/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:13:39.710553 jianglab-0.6.7/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:13:39.710038 jianglab-0.6.7/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.6.7/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:13:39.705732 jianglab-0.6.7/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.6.7/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    46512 2023-07-27 16:13:26.000000 jianglab-0.6.7/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.6.7/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:13:39.709205 jianglab-0.6.7/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:13:39.000000 jianglab-0.6.7/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-27 16:13:39.000000 jianglab-0.6.7/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-27 16:13:39.000000 jianglab-0.6.7/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      147 2023-07-27 16:13:39.000000 jianglab-0.6.7/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-27 16:13:39.000000 jianglab-0.6.7/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-27 16:13:39.710809 jianglab-0.6.7/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1119 2023-07-27 16:13:33.000000 jianglab-0.6.7/setup.py
```

### Comparing `jianglab-0.6.6/PKG-INFO` & `jianglab-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.6.6
+Version: 0.6.7
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.6.6/README.md` & `jianglab-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.6.6/jianglab/common_functions.py` & `jianglab-0.6.7/jianglab/common_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -945,15 +945,15 @@
         
         score = roc_auc_score(y_val, y_pred[:, 1])
         scores.append(score)
     
     print(np.array(scores).mean())
     return scores
 
-def xgb_optuna(X, Y,params = {}, n_trials = 2, use_GPU = False, cv_splits = 10, cv_repeats = 2, cv_random_state = 42):
+def xgb_optuna(X, y,params = {}, n_trials = 2, use_GPU = False, cv_splits = 10, cv_repeats = 2, cv_random_state = 42):
     """
         params = {
                 'verbosity': 0,
 
                 'n_estimators': trial.suggest_int('n_estimators', 50, 1500),
 
                 'learning_rate': trial.suggest_float('learning_rate', 1e-7, 1e-1),
```

### Comparing `jianglab-0.6.6/jianglab.egg-info/PKG-INFO` & `jianglab-0.6.7/jianglab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.6.6
+Version: 0.6.7
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.6.6/setup.py` & `jianglab-0.6.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.6.6',
+    version='0.6.7',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

