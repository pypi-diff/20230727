# Comparing `tmp/jianglab-0.7.0.tar.gz` & `tmp/jianglab-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.7.0.tar", last modified: Thu Jul 27 16:38:55 2023, max compression
+gzip compressed data, was "jianglab-0.7.1.tar", last modified: Thu Jul 27 16:46:57 2023, max compression
```

## Comparing `jianglab-0.7.0.tar` & `jianglab-0.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:38:55.076212 jianglab-0.7.0/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:38:55.075851 jianglab-0.7.0/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.0/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:38:55.071956 jianglab-0.7.0/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.0/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    46651 2023-07-27 16:38:36.000000 jianglab-0.7.0/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.0/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:38:55.075158 jianglab-0.7.0/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:38:54.000000 jianglab-0.7.0/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-27 16:38:54.000000 jianglab-0.7.0/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-27 16:38:54.000000 jianglab-0.7.0/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      147 2023-07-27 16:38:54.000000 jianglab-0.7.0/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-27 16:38:54.000000 jianglab-0.7.0/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-27 16:38:55.076374 jianglab-0.7.0/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1119 2023-07-27 16:38:48.000000 jianglab-0.7.0/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:46:57.013708 jianglab-0.7.1/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:46:57.013219 jianglab-0.7.1/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.7.1/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:46:57.008763 jianglab-0.7.1/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.7.1/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    46622 2023-07-27 16:46:26.000000 jianglab-0.7.1/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.7.1/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:46:57.012128 jianglab-0.7.1/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:46:56.000000 jianglab-0.7.1/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-27 16:46:56.000000 jianglab-0.7.1/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-27 16:46:56.000000 jianglab-0.7.1/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      147 2023-07-27 16:46:56.000000 jianglab-0.7.1/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-27 16:46:56.000000 jianglab-0.7.1/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-27 16:46:57.013884 jianglab-0.7.1/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1119 2023-07-27 16:46:51.000000 jianglab-0.7.1/setup.py
```

### Comparing `jianglab-0.7.0/PKG-INFO` & `jianglab-0.7.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.0
+Version: 0.7.1
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.0/README.md` & `jianglab-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.7.0/jianglab/common_functions.py` & `jianglab-0.7.1/jianglab/common_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1072,25 +1072,23 @@
     #Xgb modeling and optuna selection of hyperparameters
     optuna.logging.set_verbosity(optuna.logging.WARNING)
 
     def objective(trial):
         nonlocal params
         if params == {}:
             params = {
-                'verbosity': 0,
                 'n_estimators': trial.suggest_int('n_estimators', 50, 1500),
-                'learning_rate': trial.suggest_float('learning_rate', 1e-7, 1e-1),
                 'max_depth': trial.suggest_int('max_depth', 3, 20),
-                'colsample_bytree': trial.suggest_float('colsample_bytree', 0.1, 1.0),
-                'alpha': trial.suggest_float('alpha', 1e-5, 1e2),
-                'lambda': trial.suggest_float('lambda', 1e-5, 1e2),
-                'objective': 'binary:logistic',
-                'eval_metric': 'auc',
-                'booster':trial.suggest_categorical("booster", ["dart", "gbtree",'gblinear']),
-                'min_child_weight': trial.suggest_int('min_child_weight', 0, 5),
+                'max_features': trial.suggest_categorical('max_features', ['sqrt', 'log2', None]),
+                'min_samples_split': trial.suggest_int('min_samples_split', 2, 10),
+                'min_samples_leaf': trial.suggest_int('min_samples_leaf', 1, 10),
+                'bootstrap': trial.suggest_categorical('bootstrap', [True, False]),
+                'criterion': trial.suggest_categorical('criterion', ['gini', 'entropy']),
+                'class_weight': trial.suggest_categorical('class_weight', [None, 'balanced']),
+                'random_state': 42
             }
         if use_GPU:
             params['tree_method'] = 'gpu_hist'
 
         model_template = RandomForestClassifier(**params)
         scores = cross_validation(X, y, model_template, n_splits = cv_splits, random_state = cv_random_state, n_repeats = cv_repeats)
         return np.mean(scores)
```

### Comparing `jianglab-0.7.0/jianglab.egg-info/PKG-INFO` & `jianglab-0.7.1/jianglab.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.7.0
+Version: 0.7.1
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.7.0/setup.py` & `jianglab-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.7.0',
+    version='0.7.1',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

