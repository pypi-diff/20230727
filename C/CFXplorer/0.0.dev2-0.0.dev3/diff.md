# Comparing `tmp/cfxplorer-0.0.dev2.tar.gz` & `tmp/CFXplorer-0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfxplorer-0.0.dev2.tar", last modified: Thu Jul 27 21:25:48 2023, max compression
+gzip compressed data, was "CFXplorer-0.0.dev3.tar", last modified: Thu Jul 27 21:48:27 2023, max compression
```

## Comparing `cfxplorer-0.0.dev2.tar` & `CFXplorer-0.0.dev3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:25:48.984387 cfxplorer-0.0.dev2/
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:25:48.981342 cfxplorer-0.0.dev2/CFXplorer.egg-info/
--rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 21:25:48.000000 cfxplorer-0.0.dev2/CFXplorer.egg-info/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)      432 2023-07-27 21:25:48.000000 cfxplorer-0.0.dev2/CFXplorer.egg-info/SOURCES.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-27 21:25:48.000000 cfxplorer-0.0.dev2/CFXplorer.egg-info/dependency_links.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)       10 2023-07-27 21:25:48.000000 cfxplorer-0.0.dev2/CFXplorer.egg-info/top_level.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)    11357 2023-02-12 17:11:08.000000 cfxplorer-0.0.dev2/LICENSE
--rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 21:25:48.984580 cfxplorer-0.0.dev2/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)     4382 2023-07-26 22:56:56.000000 cfxplorer-0.0.dev2/README.rst
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:25:48.982274 cfxplorer-0.0.dev2/cfxplorer/
--rw-r--r--   0 kyosuke    (501) staff       (20)      612 2023-07-26 21:27:24.000000 cfxplorer-0.0.dev2/cfxplorer/__init__.py
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:25:48.983720 cfxplorer-0.0.dev2/cfxplorer/tests/
--rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-26 21:27:24.000000 cfxplorer-0.0.dev2/cfxplorer/tests/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     3887 2023-07-26 21:27:24.000000 cfxplorer-0.0.dev2/cfxplorer/tests/test_focus.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4162 2023-07-26 21:27:24.000000 cfxplorer-0.0.dev2/cfxplorer/tests/test_utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)      580 2023-07-27 21:25:47.000000 cfxplorer-0.0.dev2/cfxplorer/version.py
--rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-27 21:25:48.985259 cfxplorer-0.0.dev2/setup.cfg
--rw-r--r--   0 kyosuke    (501) staff       (20)     1544 2023-07-27 21:25:23.000000 cfxplorer-0.0.dev2/setup.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:48:27.733690 CFXplorer-0.0.dev3/
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:48:27.730078 CFXplorer-0.0.dev3/CFXplorer.egg-info/
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 21:48:27.000000 CFXplorer-0.0.dev3/CFXplorer.egg-info/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)      300 2023-07-27 21:48:27.000000 CFXplorer-0.0.dev3/CFXplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-27 21:48:27.000000 CFXplorer-0.0.dev3/CFXplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)       10 2023-07-27 21:48:27.000000 CFXplorer-0.0.dev3/CFXplorer.egg-info/top_level.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)    11357 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev3/LICENSE
+-rw-r--r--   0 kyosuke    (501) staff       (20)     5155 2023-07-27 21:48:27.733966 CFXplorer-0.0.dev3/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4382 2023-07-27 21:45:55.000000 CFXplorer-0.0.dev3/README.rst
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:48:27.731246 CFXplorer-0.0.dev3/cfxplorer/
+-rw-r--r--   0 kyosuke    (501) staff       (20)      612 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev3/cfxplorer/__init__.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-27 21:48:27.732959 CFXplorer-0.0.dev3/cfxplorer/tests/
+-rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev3/cfxplorer/tests/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     3887 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev3/cfxplorer/tests/test_focus.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4162 2023-07-26 21:33:17.000000 CFXplorer-0.0.dev3/cfxplorer/tests/test_utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)      580 2023-07-27 21:48:24.000000 CFXplorer-0.0.dev3/cfxplorer/version.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-27 21:48:27.734754 CFXplorer-0.0.dev3/setup.cfg
+-rw-r--r--   0 kyosuke    (501) staff       (20)     1544 2023-07-27 21:45:55.000000 CFXplorer-0.0.dev3/setup.py
```

### Comparing `cfxplorer-0.0.dev2/CFXplorer.egg-info/PKG-INFO` & `CFXplorer-0.0.dev3/CFXplorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: cfxplorer
-Version: 0.0.dev2
-Summary: cfxplorer is a python package for generating counterfactual explanations for given model and feature set
+Name: CFXplorer
+Version: 0.0.dev3
+Summary: CFXplorer is a python package for generating counterfactual explanations for given model and feature set
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `cfxplorer-0.0.dev2/LICENSE` & `CFXplorer-0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev2/PKG-INFO` & `CFXplorer-0.0.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: cfxplorer
-Version: 0.0.dev2
-Summary: cfxplorer is a python package for generating counterfactual explanations for given model and feature set
+Name: CFXplorer
+Version: 0.0.dev3
+Summary: CFXplorer is a python package for generating counterfactual explanations for given model and feature set
 Author: Kyosuke Morita
 Author-email: kq441morita@gmail.com
 Keywords: python,counterfactual explanation,binary classification,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `cfxplorer-0.0.dev2/README.rst` & `CFXplorer-0.0.dev3/README.rst`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev2/cfxplorer/__init__.py` & `CFXplorer-0.0.dev3/cfxplorer/__init__.py`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev2/cfxplorer/tests/test_focus.py` & `CFXplorer-0.0.dev3/cfxplorer/tests/test_focus.py`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev2/cfxplorer/tests/test_utils.py` & `CFXplorer-0.0.dev3/cfxplorer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cfxplorer-0.0.dev2/cfxplorer/version.py` & `CFXplorer-0.0.dev3/cfxplorer/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-``cfxplorer`` is a python package for
+``CFXplorer`` is a python package for
 generating counterfactual explanations for a given model and feature set.
 """
 # PEP0440 compatible formatted version, see:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # Generic release markers:
 # X.Y
@@ -14,8 +14,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.0.dev2"  # pragma: no cover
+__version__ = "0.0.dev3"  # pragma: no cover
```

### Comparing `cfxplorer-0.0.dev2/setup.py` & `CFXplorer-0.0.dev3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import open
 from os import path
 
 from setuptools import find_packages, setup
 
-DESCRIPTION = "cfxplorer is a python package for generating counterfactual explanations for given model and feature set"
+DESCRIPTION = "CFXplorer is a python package for generating counterfactual explanations for given model and feature set"
 
 # get __version__ from _version.py
 ver_file = path.join("cfxplorer", "version.py")
 with open(ver_file) as f:
     exec(f.read())
 
 this_directory = path.abspath(path.dirname(__file__))
@@ -20,15 +20,15 @@
 
 
 # read the contents of requirements.txt
 with open(path.join(this_directory, "requirements.txt"), encoding="utf-8") as f:
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

