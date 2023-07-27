# Comparing `tmp/jianglab-0.6.5.tar.gz` & `tmp/jianglab-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.6.5.tar", last modified: Wed Jul 26 16:20:09 2023, max compression
+gzip compressed data, was "jianglab-0.6.6.tar", last modified: Thu Jul 27 16:10:01 2023, max compression
```

## Comparing `jianglab-0.6.5.tar` & `jianglab-0.6.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 16:20:09.866637 jianglab-0.6.5/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-26 16:20:09.865988 jianglab-0.6.5/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.6.5/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 16:20:09.861953 jianglab-0.6.5/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.6.5/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    40704 2023-07-26 16:20:02.000000 jianglab-0.6.5/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.6.5/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-26 16:20:09.865126 jianglab-0.6.5/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-26 16:20:09.000000 jianglab-0.6.5/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-26 16:20:09.000000 jianglab-0.6.5/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-26 16:20:09.000000 jianglab-0.6.5/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)      147 2023-07-26 16:20:09.000000 jianglab-0.6.5/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-26 16:20:09.000000 jianglab-0.6.5/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-26 16:20:09.867041 jianglab-0.6.5/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1119 2023-07-26 16:19:25.000000 jianglab-0.6.5/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:10:01.755661 jianglab-0.6.6/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:10:01.755137 jianglab-0.6.6/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1176 2023-07-12 19:29:04.000000 jianglab-0.6.6/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:10:01.750720 jianglab-0.6.6/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.6.6/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    46512 2023-07-27 16:09:35.000000 jianglab-0.6.6/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.6.6/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-07-27 16:10:01.754251 jianglab-0.6.6/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-07-27 16:10:01.000000 jianglab-0.6.6/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-07-27 16:10:01.000000 jianglab-0.6.6/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-07-27 16:10:01.000000 jianglab-0.6.6/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      147 2023-07-27 16:10:01.000000 jianglab-0.6.6/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-07-27 16:10:01.000000 jianglab-0.6.6/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-07-27 16:10:01.755827 jianglab-0.6.6/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1119 2023-07-27 16:09:53.000000 jianglab-0.6.6/setup.py
```

### Comparing `jianglab-0.6.5/PKG-INFO` & `jianglab-0.6.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.6.5
+Version: 0.6.6
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.6.5/README.md` & `jianglab-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.6.5/jianglab/common_functions.py` & `jianglab-0.6.6/jianglab/common_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -915,15 +915,45 @@
     #plt.show()
 
 def plot_pairplot(data, hue = "target", figsize=(10,10), pallette = "viridis", size = 80):
     sns.pairplot(data=data, hue =hue, corner=True, plot_kws={'s':size, 'edgecolor':"white", 'linewidth':2.5}, palette=pallette)
     plt.figure(figsize=(10,10))
     plt.show()
 
-def xgb_optuna(X, Y,params = {}, n_trials = 2, use_GPU = False):
+def cross_validation(X, y, model_template, n_splits = 10, random_state = 42, n_repeats = 10):
+    '''
+    X: the training data # X=train_df.drop('target', axis =1) 
+                      or # X=train_df[['calc', 'gravity', 'cond']]
+    y: the target        # y=train_df['target']
+    model_template: a model template, e.g. XGBClassifier(**xgb_params)
+    n_splits: number of folds
+    random_state: random state
+    n_repeats: number of times to repeat the cross validation
+
+    ReapetedStratifiedKFold is used to keep the same distribution of target in each fold
+    '''
+
+    kf = RepeatedStratifiedKFold(n_splits = n_splits, random_state = random_state, n_repeats = n_repeats)
+    scores = []
+
+    for train_idx, val_idx in kf.split(X, y):
+        X_train, y_train = X.iloc[train_idx], y.iloc[train_idx]
+        X_val, y_val = X.iloc[val_idx], y.iloc[val_idx]
+        
+        model = model_template.fit(X_train, y_train)
+        
+        y_pred = model.predict_proba(X_val)
+        
+        score = roc_auc_score(y_val, y_pred[:, 1])
+        scores.append(score)
+    
+    print(np.array(scores).mean())
+    return scores
+
+def xgb_optuna(X, Y,params = {}, n_trials = 2, use_GPU = False, cv_splits = 10, cv_repeats = 2, cv_random_state = 42):
     """
         params = {
                 'verbosity': 0,
 
                 'n_estimators': trial.suggest_int('n_estimators', 50, 1500),
 
                 'learning_rate': trial.suggest_float('learning_rate', 1e-7, 1e-1),
@@ -966,35 +996,149 @@
                 'booster':trial.suggest_categorical("booster", ["dart", "gbtree",'gblinear']),
                 'min_child_weight': trial.suggest_int('min_child_weight', 0, 5),
             }
         if use_GPU:
             params['tree_method'] = 'gpu_hist'
         
         # n_repeats = 2 bc 10 was too long
-        kf = RepeatedStratifiedKFold(n_splits=10, n_repeats=2, random_state=42)
-        scores = []
-        for train_idx, val_idx in kf.split(X, Y):
-            X_train, X_val = X.iloc[train_idx], X.iloc[val_idx]
-            y_train, y_val = Y.iloc[train_idx], Y.iloc[val_idx]
-            
-            d_train = xgb.DMatrix(X_train, label=y_train)
-            d_val = xgb.DMatrix(X_val, label=y_val)
-            
-            evallist = [(d_val, 'eval')]
-            
-            xgb_model = xgb.train(params, d_train, num_boost_round = 100,
-                            evals = evallist, 
-                            early_stopping_rounds=20, verbose_eval=False)
-
-            y_pred = xgb_model.predict(d_val)
-            score = roc_auc_score(y_val, y_pred)
-            scores.append(score)
+        scores = cross_validation(X, y, n_splits = cv_splits, random_state = cv_random_state, n_repeats = cv_repeats)
 
         return np.mean(scores)
 
 
     study = optuna.create_study(direction='maximize')
 
     #carraying out the optimization
     study.optimize(objective, n_trials=n_trials)
     #get the best parameters
-    return study.best_params
+    return study.best_params
+
+
+def plot_feature_importance(model, X, y, n_repeats = 1, random_state = 42):
+    '''
+    model: a fitted model # model = XGBClassifier(**xgb_params)
+    X: the training data  # X=train_df.drop('target', axis =1)
+    y: the target         # y=train_df['target']
+    n_repeats: number of times to repeat the permutation importance calculation, it has to be 1
+    '''
+    def plot_fi(data,ax = None,title = None):
+        fi = pd.Series(data, index = X.columns).sort_values(ascending = True)
+        fi.plot(kind = 'barh', ax = ax)
+        
+    model.fit(X, y)
+    r = permutation_importance(model, X, y, n_repeats = n_repeats, random_state = random_state)
+
+    fig, axes = plt.subplots(2, 1, figsize=(8,12))
+    if model.__class__.__name__ == 'XGBClassifier' or model.__class__.__name__ == 'RandomForestClassifier':
+        plot_fi(model.feature_importances_, ax = axes[0])
+        plot_fi(model.feature_importances_, ax = axes[0])
+    elif model.__class__.__name__ == 'LogisticRegression':
+        plot_fi(r['importances'].reshape(X.shape[1],))
+        
+    plot_fi(r['importances'].reshape(X.shape[1],), ax = axes[1])
+
+    for i in r.importances_mean.argsort()[::-1]:
+        print(f"{X.columns[i]:<30} importance: {r.importances_mean[i]:.5f} +/- {r.importances_std[i]:.5f}")
+    return {X.columns[i]:r.importances_mean[i] for i in r.importances_mean.argsort()[::-1]}
+
+
+
+def random_forest_optuna(X, y,params = {}, n_trials = 2, use_GPU = False, cv_splits = 10, cv_repeats = 2, cv_random_state = 42):
+    """
+        params = {
+                'n_estimators': trial.suggest_int('n_estimators', 50, 1500),
+        
+                'max_depth': trial.suggest_int('max_depth', 3, 20),
+        
+                'max_features': trial.suggest_categorical('max_features', ['sqrt', 'log2', None]),
+                
+                'min_samples_split': trial.suggest_int('min_samples_split', 2, 10),
+                
+                'min_samples_leaf': trial.suggest_int('min_samples_leaf', 1, 10),
+                
+                'bootstrap': trial.suggest_categorical('bootstrap', [True, False]),
+                
+                'criterion': trial.suggest_categorical('criterion', ['gini', 'entropy']),
+                
+                'class_weight': trial.suggest_categorical('class_weight', [None, 'balanced']),
+                
+                'random_state': 42
+                
+            }
+
+        return: best parameters
+    """
+
+    #Xgb modeling and optuna selection of hyperparameters
+    optuna.logging.set_verbosity(optuna.logging.WARNING)
+
+    def objective(trial):
+        nonlocal params
+        if params == {}:
+            params = {
+                'verbosity': 0,
+                'n_estimators': trial.suggest_int('n_estimators', 50, 1500),
+                'learning_rate': trial.suggest_float('learning_rate', 1e-7, 1e-1),
+                'max_depth': trial.suggest_int('max_depth', 3, 20),
+                'colsample_bytree': trial.suggest_float('colsample_bytree', 0.1, 1.0),
+                'alpha': trial.suggest_float('alpha', 1e-5, 1e2),
+                'lambda': trial.suggest_float('lambda', 1e-5, 1e2),
+                'objective': 'binary:logistic',
+                'eval_metric': 'auc',
+                'booster':trial.suggest_categorical("booster", ["dart", "gbtree",'gblinear']),
+                'min_child_weight': trial.suggest_int('min_child_weight', 0, 5),
+            }
+        if use_GPU:
+            params['tree_method'] = 'gpu_hist'
+    
+        scores = cross_validation(X, y, n_splits = cv_splits, random_state = cv_random_state, n_repeats = cv_repeats)
+        return np.mean(scores)
+
+    study = optuna.create_study(direction='maximize')
+
+    #carraying out the optimization
+    study.optimize(objective, n_trials=n_trials)
+    #get the best parameters
+    return study.best_params
+
+def optimize_logistic_regression(X, y, n_splits = 10, n_repeats = 2, random_state = 42):
+    """
+    X: the training data # X=train_df.drop('target', axis =1)
+    y: the target        # y=train_df['target']
+    n_splits: number of folds
+    random_state: random state
+    n_repeats: number of times to repeat the cross validation
+    return: best parameters
+
+    Gridsearch was used because of the smaller hyperparameter range
+    """
+    
+    # Gridsearch was used because of the smaller hyperparameter range
+    warnings.filterwarnings("ignore")
+
+    # Define the hyperparameters grid
+    params = {
+        'penalty': ['l1', 'l2', 'elasticnet'],
+        'C': [0.001, 0.01, 0.1, 1, 10, 100],
+        'class_weight': [None, 'balanced'],
+        'solver': ['newton-cg', 'lbfgs', 'liblinear', 'sag', 'saga'],
+        'max_iter': [100, 400, 1000]
+    }
+
+    scaler = MinMaxScaler()
+    X = scaler.fit_transform(X)
+
+    # Create a logistic regression model
+    lr = LogisticRegression()
+
+    # Create a stratified k-fold cross-validator
+    skf = RepeatedStratifiedKFold(n_splits=n_splits, n_repeats=n_repeats, random_state=random_state)
+
+    # Perform grid search cross-validation
+    grid = GridSearchCV(lr, params, cv=skf, scoring='roc_auc', verbose=1, n_jobs=-1)
+    grid.fit(X, y)
+
+    # Print the best hyperparameters and the corresponding score
+    print('Best score:', grid.best_score_)
+    print('Best hyperparameters:', grid.best_params_)
+
+    return grid.best_params_
```

### Comparing `jianglab-0.6.5/jianglab.egg-info/PKG-INFO` & `jianglab-0.6.6/jianglab.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.6.5
+Version: 0.6.6
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.6.5/setup.py` & `jianglab-0.6.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.6.5',
+    version='0.6.6',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

