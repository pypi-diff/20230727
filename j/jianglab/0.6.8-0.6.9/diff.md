# Comparing `tmp/jianglab-0.6.8.tar.gz` & `tmp/jianglab-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.6.8.tar", last modified: Thu Jul 27 16:17:18 2023, max compression
+gzip compressed data, was "jianglab-0.6.9.tar", last modified: Thu Jul 27 16:29:58 2023, max compression
```

## Comparing `jianglab-0.6.8.tar` & `jianglab-0.6.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:17:18.519672 jianglab-0.6.8/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:17:18.519214 jianglab-0.6.8/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.6.8/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:17:18.515826 jianglab-0.6.8/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.6.8/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    46581 2023-07-27 16:16:19.000000 jianglab-0.6.8/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.6.8/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:17:18.518440 jianglab-0.6.8/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:17:18.000000 jianglab-0.6.8/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-27 16:17:18.000000 jianglab-0.6.8/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-27 16:17:18.000000 jianglab-0.6.8/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      147 2023-07-27 16:17:18.000000 jianglab-0.6.8/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-27 16:17:18.000000 jianglab-0.6.8/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-27 16:17:18.519860 jianglab-0.6.8/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1119 2023-07-27 16:17:13.000000 jianglab-0.6.8/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:29:58.687528 jianglab-0.6.9/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:29:58.687207 jianglab-0.6.9/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.6.9/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:29:58.684157 jianglab-0.6.9/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.6.9/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    46647 2023-07-27 16:29:45.000000 jianglab-0.6.9/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.6.9/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:29:58.686660 jianglab-0.6.9/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:29:58.000000 jianglab-0.6.9/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-27 16:29:58.000000 jianglab-0.6.9/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-27 16:29:58.000000 jianglab-0.6.9/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      147 2023-07-27 16:29:58.000000 jianglab-0.6.9/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-27 16:29:58.000000 jianglab-0.6.9/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-27 16:29:58.687661 jianglab-0.6.9/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1119 2023-07-27 16:29:54.000000 jianglab-0.6.9/setup.py
```

### Comparing `jianglab-0.6.8/PKG-INFO` & `jianglab-0.6.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.6.8
+Version: 0.6.9
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.6.8/README.md` & `jianglab-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.6.8/jianglab/common_functions.py` & `jianglab-0.6.9/jianglab/common_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1086,16 +1086,17 @@
                 'objective': 'binary:logistic',
                 'eval_metric': 'auc',
                 'booster':trial.suggest_categorical("booster", ["dart", "gbtree",'gblinear']),
                 'min_child_weight': trial.suggest_int('min_child_weight', 0, 5),
             }
         if use_GPU:
             params['tree_method'] = 'gpu_hist'
-    
-        scores = cross_validation(X, y, n_splits = cv_splits, random_state = cv_random_state, n_repeats = cv_repeats)
+
+        model_template = LogisticRegression(**params)
+        scores = cross_validation(X, y, model_template, n_splits = cv_splits, random_state = cv_random_state, n_repeats = cv_repeats)
         return np.mean(scores)
 
     study = optuna.create_study(direction='maximize')
 
     #carraying out the optimization
     study.optimize(objective, n_trials=n_trials)
     #get the best parameters
```

### Comparing `jianglab-0.6.8/jianglab.egg-info/PKG-INFO` & `jianglab-0.6.9/jianglab.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.6.8
+Version: 0.6.9
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.6.8/setup.py` & `jianglab-0.6.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.6.8',
+    version='0.6.9',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

