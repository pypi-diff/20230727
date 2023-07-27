# Comparing `tmp/Vpro-0.28.tar.gz` & `tmp/Vpro-0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Vpro-0.28.tar", last modified: Sun Jul 23 15:48:16 2023, max compression
+gzip compressed data, was "Vpro-0.29.tar", last modified: Thu Jul 27 15:31:01 2023, max compression
```

## Comparing `Vpro-0.28.tar` & `Vpro-0.29.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-23 15:48:16.836190 Vpro-0.28/
--rw-r--r--   0 Agastyaa   (502) staff       (20)      404 2023-07-23 15:48:16.836050 Vpro-0.28/PKG-INFO
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-23 15:48:16.833396 Vpro-0.28/Vpro/
--rw-r--r--   0 Agastyaa   (502) staff       (20)     7757 2023-07-23 15:47:51.000000 Vpro-0.28/Vpro/__init__.py
-drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-23 15:48:16.835815 Vpro-0.28/Vpro.egg-info/
--rw-r--r--   0 Agastyaa   (502) staff       (20)      404 2023-07-23 15:48:16.000000 Vpro-0.28/Vpro.egg-info/PKG-INFO
--rw-r--r--   0 Agastyaa   (502) staff       (20)      164 2023-07-23 15:48:16.000000 Vpro-0.28/Vpro.egg-info/SOURCES.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)        1 2023-07-23 15:48:16.000000 Vpro-0.28/Vpro.egg-info/dependency_links.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)       11 2023-07-23 15:48:16.000000 Vpro-0.28/Vpro.egg-info/requires.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)        5 2023-07-23 15:48:16.000000 Vpro-0.28/Vpro.egg-info/top_level.txt
--rw-r--r--   0 Agastyaa   (502) staff       (20)       38 2023-07-23 15:48:16.836260 Vpro-0.28/setup.cfg
--rw-r--r--   0 Agastyaa   (502) staff       (20)      547 2023-07-23 15:48:10.000000 Vpro-0.28/setup.py
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:31:01.199586 Vpro-0.29/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      404 2023-07-27 15:31:01.199429 Vpro-0.29/PKG-INFO
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:31:01.197506 Vpro-0.29/Vpro/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)     9009 2023-07-27 15:27:41.000000 Vpro-0.29/Vpro/__init__.py
+drwxr-xr-x   0 Agastyaa   (502) staff       (20)        0 2023-07-27 15:31:01.199081 Vpro-0.29/Vpro.egg-info/
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      404 2023-07-27 15:31:01.000000 Vpro-0.29/Vpro.egg-info/PKG-INFO
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      164 2023-07-27 15:31:01.000000 Vpro-0.29/Vpro.egg-info/SOURCES.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)        1 2023-07-27 15:31:01.000000 Vpro-0.29/Vpro.egg-info/dependency_links.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)       11 2023-07-27 15:31:01.000000 Vpro-0.29/Vpro.egg-info/requires.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)        5 2023-07-27 15:31:01.000000 Vpro-0.29/Vpro.egg-info/top_level.txt
+-rw-r--r--   0 Agastyaa   (502) staff       (20)       38 2023-07-27 15:31:01.199694 Vpro-0.29/setup.cfg
+-rw-r--r--   0 Agastyaa   (502) staff       (20)      547 2023-07-27 15:27:45.000000 Vpro-0.29/setup.py
```

### Comparing `Vpro-0.28/Vpro/__init__.py` & `Vpro-0.29/Vpro/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,14 +180,63 @@
     L=[]
     for i in range(len(I)):
         X= neural_network(I[i], w, b, activ)[2*U+1]-A[i]
         for j in range(len(A[0])):
             L.append((X[j])**2)
     return (sum(L)/len(I))   
 
+def normclip(grad):
+    G= []
+    for i in grad[0]:
+        for j in i:
+            for k in j:
+                for l in k:
+                    G.append(np.abs(l))
+    for i in grad[1]:
+        for j in i:
+            for k in j:
+                G.append(np.abs(k))
+    
+    X=G[0]
+    i=1
+    while i<len(G):
+        if G[i]>G[i-1]:
+            X=G[i]
+    
+    for i in grad[0]:
+        for j in i:
+            for k in j:
+                for l in k:
+                    l = l/X
+    for i in grad[1]:
+        for j in i:
+            for k in j:
+                k = k/X
+    
+    return grad
+
+def clip(grad, a1, a2):
+    for i in grad[0]:
+        for j in i:
+            for k in j:
+                for l in k:
+                    if l<a1:
+                        l=a1
+                    elif l>a2:
+                        l=a2
+    
+    for i in grad[1]:
+        for j in i:
+            for k in j:
+                if k<a1:
+                    k=a1
+                if k>a2:
+                    k=a2
+    
+    return grad
 
 def grad(I, w, b, A, activ):
 
     U=len(w)-1
 
     O=len(A[0])
 
@@ -312,18 +361,15 @@
     GW.insert(0, GW1)
     GB.insert(0, GB1)
     
     GRAD= [GW, GB]
     return GRAD
 
 
-
-
-
-def train(I, w, b, A, Ns, h, T, activ):
+def train(I, w, b, A, Ns, h, T, activ, gclipping=0):
 
     for i in tqdm(range(T)):
         
         
 
         L=[]
         for i1 in range(Ns):
@@ -335,20 +381,26 @@
 
         ACs=[]
 
         for l in range(Ns):
             ACs.append(A[L[l]])
         ACs= np.array(ACs)
 
-        X=grad(Is, w, b, ACs, activ)
+        if gclipping==0:
+            X=grad(Is, w, b, ACs, activ)
+        if gclipping=='norm':
+            X= normclip(grad(Is, w, b, ACs, activ))
+        if gclipping[0]=='range':
+            X= clip(grad(Is, w, b, ACs, activ), gclipping[1], gclipping[2])
 
         for i3 in range(len(w)):
             for j in range (len(w[i3])):
                 for k in range(len(w[i3][0])):
                     w[i3][j][k]=w[i3][j][k]-h*X[0][i3][j][k]
         
 
         for i4 in range(len(b)):
             for j in range(len(b[i4])):
                 b[i4][j]=b[i4][j]-h*X[1][i4][j]
 
     return [w, b]
+
```

### Comparing `Vpro-0.28/setup.py` & `Vpro-0.29/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 from setuptools import setup
 
 setup(name= "Vpro",
-      version= 0.28,
+      version= 0.29,
       description="This is a Machine Learning Module that grants one access to a Multilayer percepton with an adjustable number of hidden layers and neurons per each layer. It also includes functionality to train the network based on a database, and has adjustable innitialisation types, activation functions, and learning hyperparamters.", 
       author="Agastyaa Vishvanath",
       packages=["Vpro"],
       install_requires= ["numpy", "tqdm"])
```

