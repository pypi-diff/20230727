# Comparing `tmp/ezsmdeploy-1.97.dev0.tar.gz` & `tmp/ezsmdeploy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezsmdeploy-1.97.dev0.tar", last modified: Tue Jul 25 19:09:48 2023, max compression
+gzip compressed data, was "ezsmdeploy-2.0.0.tar", last modified: Thu Jul 27 20:30:44 2023, max compression
```

## Comparing `ezsmdeploy-1.97.dev0.tar` & `ezsmdeploy-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-25 19:09:48.675099 ezsmdeploy-1.97.dev0/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19598 2023-07-25 19:09:48.675099 ezsmdeploy-1.97.dev0/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19108 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/README.rst
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-25 19:09:48.675099 ezsmdeploy-1.97.dev0/ezsmdeploy/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    48489 2023-07-25 19:08:36.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-25 19:09:48.675099 ezsmdeploy-1.97.dev0/ezsmdeploy/data/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2100 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/Dockerfile
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1934 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/Dockerfile_flask
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1390 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/build-docker.sh
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1603 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/conversation.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1361 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/cost.csv
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      884 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/dockerd-entrypoint.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      576 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/instancetypes.csv
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1797 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/model_handler.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      719 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/nginx.conf
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2090 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/predictor.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2429 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/serve
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1409 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/smlocust.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      432 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/train
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      202 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/data/wsgi.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      733 2023-07-18 17:32:09.000000 ezsmdeploy-1.97.dev0/ezsmdeploy/modelscript_sklearn.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-25 19:09:48.675099 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19598 2023-07-25 19:09:48.000000 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      696 2023-07-25 19:09:48.000000 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-25 19:09:48.000000 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-18 17:33:24.000000 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/not-zip-safe
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      129 2023-07-25 19:09:48.000000 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       11 2023-07-25 19:09:48.000000 ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-25 19:09:48.675099 ezsmdeploy-1.97.dev0/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1274 2023-07-25 19:09:10.000000 ezsmdeploy-1.97.dev0/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-27 20:30:44.166378 ezsmdeploy-2.0.0/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19594 2023-07-27 20:30:44.166378 ezsmdeploy-2.0.0/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19108 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/README.rst
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-27 20:30:44.162378 ezsmdeploy-2.0.0/ezsmdeploy/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    48489 2023-07-27 20:29:14.000000 ezsmdeploy-2.0.0/ezsmdeploy/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-27 20:30:44.166378 ezsmdeploy-2.0.0/ezsmdeploy/data/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2100 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/Dockerfile
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1934 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/Dockerfile_flask
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1390 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/build-docker.sh
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1603 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/conversation.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1361 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/cost.csv
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      884 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/dockerd-entrypoint.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      576 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/instancetypes.csv
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1797 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/model_handler.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      719 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/nginx.conf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2090 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/predictor.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2429 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/serve
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1409 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/smlocust.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      432 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/train
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      202 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/data/wsgi.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      733 2023-07-18 17:32:09.000000 ezsmdeploy-2.0.0/ezsmdeploy/modelscript_sklearn.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-27 20:30:44.162378 ezsmdeploy-2.0.0/ezsmdeploy.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19594 2023-07-27 20:30:44.000000 ezsmdeploy-2.0.0/ezsmdeploy.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      696 2023-07-27 20:30:44.000000 ezsmdeploy-2.0.0/ezsmdeploy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-27 20:30:44.000000 ezsmdeploy-2.0.0/ezsmdeploy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-27 20:30:44.000000 ezsmdeploy-2.0.0/ezsmdeploy.egg-info/not-zip-safe
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      129 2023-07-27 20:30:44.000000 ezsmdeploy-2.0.0/ezsmdeploy.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       11 2023-07-27 20:30:44.000000 ezsmdeploy-2.0.0/ezsmdeploy.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-27 20:30:44.166378 ezsmdeploy-2.0.0/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1272 2023-07-27 20:29:23.000000 ezsmdeploy-2.0.0/setup.py
```

### Comparing `ezsmdeploy-1.97.dev0/PKG-INFO` & `ezsmdeploy-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploy
-Version: 1.97.dev0
+Version: 2.0.0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ezsmdeploy-1.97.dev0/README.rst` & `ezsmdeploy-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/__init__.py` & `ezsmdeploy-2.0.0/ezsmdeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/data/Dockerfile` & `ezsmdeploy-2.0.0/ezsmdeploy/data/Dockerfile`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/data/Dockerfile_flask` & `ezsmdeploy-2.0.0/ezsmdeploy/data/Dockerfile_flask`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/data/build-docker.sh` & `ezsmdeploy-2.0.0/ezsmdeploy/data/build-docker.sh`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/data/conversation.py` & `ezsmdeploy-2.0.0/ezsmdeploy/data/conversation.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/data/cost.csv` & `ezsmdeploy-2.0.0/ezsmdeploy/data/cost.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/data/dockerd-entrypoint.py` & `ezsmdeploy-2.0.0/ezsmdeploy/data/dockerd-entrypoint.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/data/instancetypes.csv` & `ezsmdeploy-2.0.0/ezsmdeploy/data/instancetypes.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/data/model_handler.py` & `ezsmdeploy-2.0.0/ezsmdeploy/data/model_handler.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/data/nginx.conf` & `ezsmdeploy-2.0.0/ezsmdeploy/data/nginx.conf`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/data/predictor.py` & `ezsmdeploy-2.0.0/ezsmdeploy/data/predictor.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/data/serve` & `ezsmdeploy-2.0.0/ezsmdeploy/data/serve`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/data/smlocust.py` & `ezsmdeploy-2.0.0/ezsmdeploy/data/smlocust.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy/modelscript_sklearn.py` & `ezsmdeploy-2.0.0/ezsmdeploy/modelscript_sklearn.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/PKG-INFO` & `ezsmdeploy-2.0.0/ezsmdeploy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploy
-Version: 1.97.dev0
+Version: 2.0.0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ezsmdeploy-1.97.dev0/ezsmdeploy.egg-info/SOURCES.txt` & `ezsmdeploy-2.0.0/ezsmdeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.97.dev0/setup.py` & `ezsmdeploy-2.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 extras = {
     'locust': [
         'locustio==0.14.5'
     ]
 }
 
 setup(name='ezsmdeploy',
-      version='1.97dev',
+      version='2.0.0',
       description='SageMaker custom deployments made easy',
       url='https://pypi.python.org/pypi/ezsmdeploy',
       #scripts=['Dockerfile','dockerd-entrypoint.py','model_handler.py','build-docker.sh'],
       author='Shreyas Subramanian',
       author_email='subshrey@amazon.com',
       license='MIT',
       packages=['ezsmdeploy'],
```

