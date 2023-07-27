# Comparing `tmp/Vpro-0.295.tar.gz` & `tmp/Vpro-0.296.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Vpro-0.295.tar", last modified: Thu Jul 27 15:38:31 2023, max compression
+gzip compressed data, was "Vpro-0.296.tar", last modified: Thu Jul 27 15:41:44 2023, max compression
```

## Comparing `Vpro-0.295.tar` & `Vpro-0.296.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:38:31.375997 Vpro-0.295/
--rw-r--r--   0 Agastyaa   (502) staff       (20)      405 2023-07-27 15:38:31.375857 Vpro-0.295/PKG-INFO
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:38:31.374812 Vpro-0.295/Vpro/
--rw-r--r--   0 Agastyaa   (502) staff       (20)     8801 2023-07-27 15:38:16.000000 Vpro-0.295/Vpro/__init__.py
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:38:31.375652 Vpro-0.295/Vpro.egg-info/
--rw-r--r--   0 Agastyaa   (502) staff       (20)      405 2023-07-27 15:38:31.000000 Vpro-0.295/Vpro.egg-info/PKG-INFO
--rw-r--r--   0 Agastyaa   (502) staff       (20)      164 2023-07-27 15:38:31.000000 Vpro-0.295/Vpro.egg-info/SOURCES.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)        1 2023-07-27 15:38:31.000000 Vpro-0.295/Vpro.egg-info/dependency_links.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)       11 2023-07-27 15:38:31.000000 Vpro-0.295/Vpro.egg-info/requires.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)        5 2023-07-27 15:38:31.000000 Vpro-0.295/Vpro.egg-info/top_level.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)       38 2023-07-27 15:38:31.376034 Vpro-0.295/setup.cfg
--rw-r--r--   0 Agastyaa   (502) staff       (20)      548 2023-07-27 15:38:28.000000 Vpro-0.295/setup.py
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:41:44.192605 Vpro-0.296/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      405 2023-07-27 15:41:44.192449 Vpro-0.296/PKG-INFO
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:41:44.191071 Vpro-0.296/Vpro/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)     8805 2023-07-27 15:41:33.000000 Vpro-0.296/Vpro/__init__.py
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:41:44.192148 Vpro-0.296/Vpro.egg-info/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      405 2023-07-27 15:41:44.000000 Vpro-0.296/Vpro.egg-info/PKG-INFO
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      164 2023-07-27 15:41:44.000000 Vpro-0.296/Vpro.egg-info/SOURCES.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)        1 2023-07-27 15:41:44.000000 Vpro-0.296/Vpro.egg-info/dependency_links.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)       11 2023-07-27 15:41:44.000000 Vpro-0.296/Vpro.egg-info/requires.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)        5 2023-07-27 15:41:44.000000 Vpro-0.296/Vpro.egg-info/top_level.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)       38 2023-07-27 15:41:44.192651 Vpro-0.296/setup.cfg
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      548 2023-07-27 15:41:37.000000 Vpro-0.296/setup.py
```

### Comparing `Vpro-0.295/Vpro/__init__.py` & `Vpro-0.296/Vpro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,17 +377,17 @@
 
         for l in range(Ns):
             ACs.append(A[L[l]])
         ACs= np.array(ACs)
 
         if gclipping==0:
             X=grad(Is, w, b, ACs, activ)
-        if gclipping=='norm':
+        elif gclipping=='norm':
             X= normclip(grad(Is, w, b, ACs, activ))
-        if gclipping[0]=='range':
+        elif gclipping[0]=='range':
             X= clip(grad(Is, w, b, ACs, activ), gclipping[1], gclipping[2])
 
         for i3 in range(len(w)):
             for j in range (len(w[i3])):
                 for k in range(len(w[i3][0])):
                     w[i3][j][k]=w[i3][j][k]-h*X[0][i3][j][k]
```

### Comparing `Vpro-0.295/setup.py` & `Vpro-0.296/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 from setuptools import setup
 
 setup(name= "Vpro",
-      version= 0.295,
+      version= 0.296,
       description="This is a Machine Learning Module that grants one access to a Multilayer percepton with an adjustable number of hidden layers and neurons per each layer. It also includes functionality to train the network based on a database, and has adjustable innitialisation types, activation functions, and learning hyperparamters.", 
       author="Agastyaa Vishvanath",
       packages=["Vpro"],
       install_requires= ["numpy", "tqdm"])
```

