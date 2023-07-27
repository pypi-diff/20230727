# Comparing `tmp/cfxplorer-0.0.dev1.tar.gz` & `tmp/CFXplorer-0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfxplorer-0.0.dev1.tar", last modified: Thu Jul 27 21:11:43 2023, max compression
+gzip compressed data, was "CFXplorer-0.0.dev4.tar", last modified: Wed Jul 26 22:58:43 2023, max compression
```

## Comparing `cfxplorer-0.0.dev1.tar` & `CFXplorer-0.0.dev4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:11:43.437259 cfxplorer-0.0.dev1/
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:11:43.432956 cfxplorer-0.0.dev1/CFXplorer.egg-info/
--rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 21:11:43.000000 cfxplorer-0.0.dev1/CFXplorer.egg-info/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)      432 2023-07-27 21:11:43.000000 cfxplorer-0.0.dev1/CFXplorer.egg-info/SOURCES.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-27 21:11:43.000000 cfxplorer-0.0.dev1/CFXplorer.egg-info/dependency_links.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)       10 2023-07-27 21:11:43.000000 cfxplorer-0.0.dev1/CFXplorer.egg-info/top_level.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)    11357 2023-02-12 17:11:08.000000 cfxplorer-0.0.dev1/LICENSE
--rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 21:11:43.437423 cfxplorer-0.0.dev1/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)     4382 2023-07-26 22:56:56.000000 cfxplorer-0.0.dev1/README.rst
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:11:43.434293 cfxplorer-0.0.dev1/cfxplorer/
--rw-r--r--   0 kyosuke    (501) staff       (20)      612 2023-07-26 21:27:24.000000 cfxplorer-0.0.dev1/cfxplorer/__init__.py
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:11:43.436583 cfxplorer-0.0.dev1/cfxplorer/tests/
--rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-26 21:27:24.000000 cfxplorer-0.0.dev1/cfxplorer/tests/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     3887 2023-07-26 21:27:24.000000 cfxplorer-0.0.dev1/cfxplorer/tests/test_focus.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4162 2023-07-26 21:27:24.000000 cfxplorer-0.0.dev1/cfxplorer/tests/test_utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)      568 2023-07-27 21:11:38.000000 cfxplorer-0.0.dev1/cfxplorer/version.py
--rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-27 21:11:43.437962 cfxplorer-0.0.dev1/setup.cfg
--rw-r--r--   0 kyosuke    (501) staff       (20)     1544 2023-07-27 21:10:00.000000 cfxplorer-0.0.dev1/setup.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-26 22:58:43.920828 CFXplorer-0.0.dev4/
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-26 22:58:43.918112 CFXplorer-0.0.dev4/CFXplorer.egg-info/
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-26 22:58:43.000000 CFXplorer-0.0.dev4/CFXplorer.egg-info/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)      300 2023-07-26 22:58:43.000000 CFXplorer-0.0.dev4/CFXplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-26 22:58:43.000000 CFXplorer-0.0.dev4/CFXplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)       10 2023-07-26 22:58:43.000000 CFXplorer-0.0.dev4/CFXplorer.egg-info/top_level.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)    11357 2023-02-12 17:11:08.000000 CFXplorer-0.0.dev4/LICENSE
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-26 22:58:43.920957 CFXplorer-0.0.dev4/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4382 2023-07-26 22:56:56.000000 CFXplorer-0.0.dev4/README.rst
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-26 22:58:43.919038 CFXplorer-0.0.dev4/cfxplorer/
+-rw-r--r--   0 kyosuke    (501) staff       (20)      612 2023-07-26 21:27:24.000000 CFXplorer-0.0.dev4/cfxplorer/__init__.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-26 22:58:43.920215 CFXplorer-0.0.dev4/cfxplorer/tests/
+-rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-26 21:27:24.000000 CFXplorer-0.0.dev4/cfxplorer/tests/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     3887 2023-07-26 21:27:24.000000 CFXplorer-0.0.dev4/cfxplorer/tests/test_focus.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4162 2023-07-26 21:27:24.000000 CFXplorer-0.0.dev4/cfxplorer/tests/test_utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)      568 2023-07-26 22:42:36.000000 CFXplorer-0.0.dev4/cfxplorer/version.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-26 22:58:43.921416 CFXplorer-0.0.dev4/setup.cfg
+-rw-r--r--   0 kyosuke    (501) staff       (20)     1544 2023-07-26 22:53:23.000000 CFXplorer-0.0.dev4/setup.py
```

### Comparing `cfxplorer-0.0.dev1/CFXplorer.egg-info/PKG-INFO` & `CFXplorer-0.0.dev4/CFXplorer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cfxplorer
-Version: 0.0.dev1
+Name: CFXplorer
+Version: 0.0.dev4
 Summary: CFXplorer is a python package for generating counterfactual explanations for given model and feature set
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cfxplorer-0.0.dev1/LICENSE` & `CFXplorer-0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev1/PKG-INFO` & `CFXplorer-0.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cfxplorer
-Version: 0.0.dev1
+Name: CFXplorer
+Version: 0.0.dev4
 Summary: CFXplorer is a python package for generating counterfactual explanations for given model and feature set
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cfxplorer-0.0.dev1/README.rst` & `CFXplorer-0.0.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev1/cfxplorer/__init__.py` & `CFXplorer-0.0.dev4/cfxplorer/__init__.py`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev1/cfxplorer/tests/test_focus.py` & `CFXplorer-0.0.dev4/cfxplorer/tests/test_focus.py`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev1/cfxplorer/tests/test_utils.py` & `CFXplorer-0.0.dev4/cfxplorer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev1/cfxplorer/version.py` & `CFXplorer-0.0.dev4/cfxplorer/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.0.dev1"  # pragma: no cover
+__version__ = "0.0.dev4"  # pragma: no cover
```

### Comparing `cfxplorer-0.0.dev1/setup.py` & `CFXplorer-0.0.dev4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # read the contents of README.rst
 def readme():
     with open(path.join(this_directory, "README.rst"), encoding="utf-8") as f:
         return f.read()
 
 
 # read the contents of requirements.txt
-with open(path.join(this_directory, 'requirements.txt'), encoding='utf-8') as f:
+with open(path.join(this_directory, "requirements.txt"), encoding="utf-8") as f:
     requirements = f.read().splitlines()
 
 setup(
-    name="cfxplorer",
+    name="CFXplorer",
     version=__version__,
     author="Kyosuke Morita",
     author_email="kq441morita@gmail.com",
     description=DESCRIPTION,
     long_description=readme(),
     packages=find_packages(),
     install_requires=[],
```

