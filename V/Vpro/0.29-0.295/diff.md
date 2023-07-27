# Comparing `tmp/Vpro-0.29.tar.gz` & `tmp/Vpro-0.295.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Vpro-0.29.tar", last modified: Thu Jul 27 15:31:01 2023, max compression
+gzip compressed data, was "Vpro-0.295.tar", last modified: Thu Jul 27 15:38:31 2023, max compression
```

## Comparing `Vpro-0.29.tar` & `Vpro-0.295.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:31:01.199586 Vpro-0.29/
--rw-r--r--   0 Agastyaa   (502) staff       (20)      404 2023-07-27 15:31:01.199429 Vpro-0.29/PKG-INFO
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:31:01.197506 Vpro-0.29/Vpro/
--rw-r--r--   0 Agastyaa   (502) staff       (20)     9009 2023-07-27 15:27:41.000000 Vpro-0.29/Vpro/__init__.py
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:31:01.199081 Vpro-0.29/Vpro.egg-info/
--rw-r--r--   0 Agastyaa   (502) staff       (20)      404 2023-07-27 15:31:01.000000 Vpro-0.29/Vpro.egg-info/PKG-INFO
--rw-r--r--   0 Agastyaa   (502) staff       (20)      164 2023-07-27 15:31:01.000000 Vpro-0.29/Vpro.egg-info/SOURCES.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)        1 2023-07-27 15:31:01.000000 Vpro-0.29/Vpro.egg-info/dependency_links.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)       11 2023-07-27 15:31:01.000000 Vpro-0.29/Vpro.egg-info/requires.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)        5 2023-07-27 15:31:01.000000 Vpro-0.29/Vpro.egg-info/top_level.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)       38 2023-07-27 15:31:01.199694 Vpro-0.29/setup.cfg
--rw-r--r--   0 Agastyaa   (502) staff       (20)      547 2023-07-27 15:27:45.000000 Vpro-0.29/setup.py
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:38:31.375997 Vpro-0.295/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      405 2023-07-27 15:38:31.375857 Vpro-0.295/PKG-INFO
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:38:31.374812 Vpro-0.295/Vpro/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)     8801 2023-07-27 15:38:16.000000 Vpro-0.295/Vpro/__init__.py
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:38:31.375652 Vpro-0.295/Vpro.egg-info/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      405 2023-07-27 15:38:31.000000 Vpro-0.295/Vpro.egg-info/PKG-INFO
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      164 2023-07-27 15:38:31.000000 Vpro-0.295/Vpro.egg-info/SOURCES.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)        1 2023-07-27 15:38:31.000000 Vpro-0.295/Vpro.egg-info/dependency_links.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)       11 2023-07-27 15:38:31.000000 Vpro-0.295/Vpro.egg-info/requires.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)        5 2023-07-27 15:38:31.000000 Vpro-0.295/Vpro.egg-info/top_level.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)       38 2023-07-27 15:38:31.376034 Vpro-0.295/setup.cfg
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      548 2023-07-27 15:38:28.000000 Vpro-0.295/setup.py
```

### Comparing `Vpro-0.29/Vpro/__init__.py` & `Vpro-0.295/Vpro/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,57 +185,51 @@
     return (sum(L)/len(I))   
 
 def normclip(grad):
     G= []
     for i in grad[0]:
         for j in i:
             for k in j:
-                for l in k:
-                    G.append(np.abs(l))
+                G.append(np.abs(k))
     for i in grad[1]:
         for j in i:
-            for k in j:
-                G.append(np.abs(k))
+            G.append(np.abs(j))
     
     X=G[0]
     i=1
     while i<len(G):
         if G[i]>G[i-1]:
             X=G[i]
     
     for i in grad[0]:
         for j in i:
             for k in j:
-                for l in k:
-                    l = l/X
+                k= k/X
     for i in grad[1]:
         for j in i:
-            for k in j:
-                k = k/X
+            j= j/X
     
     return grad
 
 def clip(grad, a1, a2):
     for i in grad[0]:
         for j in i:
             for k in j:
-                for l in k:
-                    if l<a1:
-                        l=a1
-                    elif l>a2:
-                        l=a2
-    
-    for i in grad[1]:
-        for j in i:
-            for k in j:
                 if k<a1:
                     k=a1
                 if k>a2:
                     k=a2
     
+    for i in grad[1]:
+        for j in i:
+            if j<a1:
+                k=a1
+            if j>a2:
+                k=a2
+    
     return grad
 
 def grad(I, w, b, A, activ):
 
     U=len(w)-1
 
     O=len(A[0])
```

### Comparing `Vpro-0.29/setup.py` & `Vpro-0.295/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 from setuptools import setup
 
 setup(name= "Vpro",
-      version= 0.29,
+      version= 0.295,
       description="This is a Machine Learning Module that grants one access to a Multilayer percepton with an adjustable number of hidden layers and neurons per each layer. It also includes functionality to train the network based on a database, and has adjustable innitialisation types, activation functions, and learning hyperparamters.", 
       author="Agastyaa Vishvanath",
       packages=["Vpro"],
       install_requires= ["numpy", "tqdm"])
```

