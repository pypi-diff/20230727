# Comparing `tmp/cfxplorer-0.0.dev1.tar.gz` & `tmp/cfxplorer-0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfxplorer-0.0.dev1.tar", last modified: Thu Jul 27 21:11:43 2023, max compression
+gzip compressed data, was "cfxplorer-0.0.dev2.tar", last modified: Thu Jul 27 21:25:48 2023, max compression
```

## Comparing `cfxplorer-0.0.dev1.tar` & `cfxplorer-0.0.dev2.tar`

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
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:25:48.984387 cfxplorer-0.0.dev2/
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:25:48.981342 cfxplorer-0.0.dev2/CFXplorer.egg-info/
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 21:25:48.000000 cfxplorer-0.0.dev2/CFXplorer.egg-info/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)      432 2023-07-27 21:25:48.000000 cfxplorer-0.0.dev2/CFXplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-27 21:25:48.000000 cfxplorer-0.0.dev2/CFXplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)       10 2023-07-27 21:25:48.000000 cfxplorer-0.0.dev2/CFXplorer.egg-info/top_level.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)    11357 2023-02-12 17:11:08.000000 cfxplorer-0.0.dev2/LICENSE
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 21:25:48.984580 cfxplorer-0.0.dev2/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4382 2023-07-26 22:56:56.000000 cfxplorer-0.0.dev2/README.rst
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:25:48.982274 cfxplorer-0.0.dev2/cfxplorer/
+-rw-r--r--   0 kyosuke    (501) staff       (20)      612 2023-07-26 21:27:24.000000 cfxplorer-0.0.dev2/cfxplorer/__init__.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:25:48.983720 cfxplorer-0.0.dev2/cfxplorer/tests/
+-rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-26 21:27:24.000000 cfxplorer-0.0.dev2/cfxplorer/tests/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     3887 2023-07-26 21:27:24.000000 cfxplorer-0.0.dev2/cfxplorer/tests/test_focus.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4162 2023-07-26 21:27:24.000000 cfxplorer-0.0.dev2/cfxplorer/tests/test_utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)      580 2023-07-27 21:25:47.000000 cfxplorer-0.0.dev2/cfxplorer/version.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-27 21:25:48.985259 cfxplorer-0.0.dev2/setup.cfg
+-rw-r--r--   0 kyosuke    (501) staff       (20)     1544 2023-07-27 21:25:23.000000 cfxplorer-0.0.dev2/setup.py
```

### Comparing `cfxplorer-0.0.dev1/CFXplorer.egg-info/PKG-INFO` & `cfxplorer-0.0.dev2/CFXplorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cfxplorer
-Version: 0.0.dev1
-Summary: CFXplorer is a python package for generating counterfactual explanations for given model and feature set
+Version: 0.0.dev2
+Summary: cfxplorer is a python package for generating counterfactual explanations for given model and feature set
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `cfxplorer-0.0.dev1/LICENSE` & `cfxplorer-0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev1/PKG-INFO` & `cfxplorer-0.0.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cfxplorer
-Version: 0.0.dev1
-Summary: CFXplorer is a python package for generating counterfactual explanations for given model and feature set
+Version: 0.0.dev2
+Summary: cfxplorer is a python package for generating counterfactual explanations for given model and feature set
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `cfxplorer-0.0.dev1/README.rst` & `cfxplorer-0.0.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev1/cfxplorer/__init__.py` & `cfxplorer-0.0.dev2/cfxplorer/__init__.py`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev1/cfxplorer/tests/test_focus.py` & `cfxplorer-0.0.dev2/cfxplorer/tests/test_focus.py`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev1/cfxplorer/tests/test_utils.py` & `cfxplorer-0.0.dev2/cfxplorer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev1/cfxplorer/version.py` & `cfxplorer-0.0.dev2/cfxplorer/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ``cfxplorer`` is a python package for
-generating counterfactual explanations for a tree-based model
+generating counterfactual explanations for a given model and feature set.
 """
 # PEP0440 compatible formatted version, see:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # Generic release markers:
 # X.Y
 # X.Y.Z # For bug fix releases
@@ -14,8 +14,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.0.dev1"  # pragma: no cover
+__version__ = "0.0.dev2"  # pragma: no cover
```

### Comparing `cfxplorer-0.0.dev1/setup.py` & `cfxplorer-0.0.dev2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import open
 from os import path
 
 from setuptools import find_packages, setup
 
-DESCRIPTION = "CFXplorer is a python package for generating counterfactual explanations for given model and feature set"
+DESCRIPTION = "cfxplorer is a python package for generating counterfactual explanations for given model and feature set"
 
 # get __version__ from _version.py
 ver_file = path.join("cfxplorer", "version.py")
 with open(ver_file) as f:
     exec(f.read())
 
 this_directory = path.abspath(path.dirname(__file__))
@@ -16,15 +16,15 @@
 # read the contents of README.rst
 def readme():
     with open(path.join(this_directory, "README.rst"), encoding="utf-8") as f:
         return f.read()
 
 
 # read the contents of requirements.txt
-with open(path.join(this_directory, 'requirements.txt'), encoding='utf-8') as f:
+with open(path.join(this_directory, "requirements.txt"), encoding="utf-8") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="cfxplorer",
     version=__version__,
     author="Kyosuke Morita",
     author_email="kq441morita@gmail.com",
```

