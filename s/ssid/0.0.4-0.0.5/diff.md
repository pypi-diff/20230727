# Comparing `tmp/ssid-0.0.4.tar.gz` & `tmp/ssid-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssid-0.0.4.tar", last modified: Sat Jul  8 00:36:25 2023, max compression
+gzip compressed data, was "ssid-0.0.5.tar", last modified: Thu Jul 27 17:41:25 2023, max compression
```

## Comparing `ssid-0.0.4.tar` & `ssid-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2023-07-08 00:50:27.042592 ssid-0.0.4/
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)      341 2023-07-08 00:50:27.037470 ssid-0.0.4/PKG-INFO
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)      729 2023-07-08 00:49:39.000000 ssid-0.0.4/pyproject.toml
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)       38 2023-07-08 00:50:27.042592 ssid-0.0.4/setup.cfg
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)      718 2022-08-30 21:37:12.000000 ssid-0.0.4/setup.py
-drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2023-07-08 00:50:26.221284 ssid-0.0.4/src/
-drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2023-07-08 00:50:26.699516 ssid-0.0.4/src/ssid/
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     4696 2023-03-02 04:28:15.000000 ssid-0.0.4/src/ssid/ExtractModes.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)       27 2023-05-24 23:18:45.000000 ssid-0.0.4/src/ssid/__init__.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     6086 2023-06-30 22:02:50.000000 ssid-0.0.4/src/ssid/__main__.py
-drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2023-07-08 00:50:26.949061 ssid-0.0.4/src/ssid/brace2/
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     2925 2022-08-30 21:37:12.000000 ssid-0.0.4/src/ssid/brace2/__main__.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     5997 2022-08-30 21:37:16.000000 ssid-0.0.4/src/ssid/integrate.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     2763 2023-06-26 22:44:57.000000 ssid-0.0.4/src/ssid/markov.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     2870 2023-07-07 23:42:47.000000 ssid-0.0.4/src/ssid/modal.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)    21710 2023-03-27 21:37:12.000000 ssid-0.0.4/src/ssid/okid.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)    10244 2023-07-06 17:49:47.000000 ssid-0.0.4/src/ssid/realize.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)      423 2023-07-08 00:35:36.000000 ssid-0.0.4/src/ssid/spec.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)    17469 2023-06-01 18:06:42.000000 ssid-0.0.4/src/ssid/srim.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)      711 2023-06-26 21:07:26.000000 ssid-0.0.4/src/ssid/system.py
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     3305 2023-07-06 23:04:53.000000 ssid-0.0.4/src/ssid/validation.py
-drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2023-07-08 00:50:26.903116 ssid-0.0.4/src/ssid.egg-info/
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)      341 2023-07-08 00:50:25.000000 ssid-0.0.4/src/ssid.egg-info/PKG-INFO
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)      468 2023-07-08 00:50:26.000000 ssid-0.0.4/src/ssid.egg-info/SOURCES.txt
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)        1 2023-07-08 00:50:25.000000 ssid-0.0.4/src/ssid.egg-info/dependency_links.txt
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)       44 2023-07-08 00:50:26.000000 ssid-0.0.4/src/ssid.egg-info/entry_points.txt
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)        5 2023-07-08 00:50:26.000000 ssid-0.0.4/src/ssid.egg-info/top_level.txt
-drwxrwxrwx   0 xstal     (1000) xstal     (1000)        0 2023-07-08 00:50:26.994935 ssid-0.0.4/tests/
--rwxrwxrwx   0 xstal     (1000) xstal     (1000)     3707 2022-12-20 21:47:57.000000 ssid-0.0.4/tests/test1.py
+drwxr-xr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-27 17:41:25.237501 ssid-0.0.5/
+-rw-r--r--   0 claudio   (1000) claudio   (1000)      341 2023-07-27 17:41:25.237501 ssid-0.0.5/PKG-INFO
+-rw-r--r--   0 claudio   (1000) claudio   (1000)      685 2023-07-27 17:41:17.000000 ssid-0.0.5/pyproject.toml
+-rw-r--r--   0 claudio   (1000) claudio   (1000)       38 2023-07-27 17:41:25.237501 ssid-0.0.5/setup.cfg
+-rwxr-xr-x   0 claudio   (1000) claudio   (1000)      718 2023-06-05 17:44:53.000000 ssid-0.0.5/setup.py
+drwxr-xr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-27 17:41:25.234167 ssid-0.0.5/src/
+drwxr-xr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-27 17:41:25.237501 ssid-0.0.5/src/ssid/
+-rw-r--r--   0 claudio   (1000) claudio   (1000)       27 2023-06-05 17:44:53.000000 ssid-0.0.5/src/ssid/__init__.py
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     7482 2023-07-27 17:39:53.000000 ssid-0.0.5/src/ssid/__main__.py
+drwxr-xr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-27 17:41:25.237501 ssid-0.0.5/src/ssid/archive/
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     4565 2023-07-27 17:39:53.000000 ssid-0.0.5/src/ssid/archive/ExtractModes.py
+-rw-r--r--   0 claudio   (1000) claudio   (1000)    21130 2023-07-27 17:39:53.000000 ssid-0.0.5/src/ssid/archive/okid.py
+-rw-r--r--   0 claudio   (1000) claudio   (1000)      458 2023-07-27 17:39:53.000000 ssid-0.0.5/src/ssid/archive/realization.py
+-rw-r--r--   0 claudio   (1000) claudio   (1000)    16949 2023-07-27 17:39:53.000000 ssid-0.0.5/src/ssid/archive/srim.py
+drwxr-xr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-27 17:41:25.237501 ssid-0.0.5/src/ssid/brace2/
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     2925 2023-06-05 17:44:53.000000 ssid-0.0.5/src/ssid/brace2/__main__.py
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     5997 2023-06-05 17:44:53.000000 ssid-0.0.5/src/ssid/integrate.py
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     2705 2023-06-28 00:10:49.000000 ssid-0.0.5/src/ssid/markov.py
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     3456 2023-07-27 17:39:53.000000 ssid-0.0.5/src/ssid/modal.py
+-rw-r--r--   0 claudio   (1000) claudio   (1000)      733 2023-07-27 17:39:53.000000 ssid-0.0.5/src/ssid/numerics.py
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     9823 2023-07-27 17:39:53.000000 ssid-0.0.5/src/ssid/realize.py
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     2064 2023-07-27 17:39:53.000000 ssid-0.0.5/src/ssid/spec.py
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     1020 2023-07-27 17:39:53.000000 ssid-0.0.5/src/ssid/system.py
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     3092 2023-07-12 01:47:00.000000 ssid-0.0.5/src/ssid/validation.py
+drwxr-xr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-27 17:41:25.237501 ssid-0.0.5/src/ssid.egg-info/
+-rw-r--r--   0 claudio   (1000) claudio   (1000)      341 2023-07-27 17:41:25.000000 ssid-0.0.5/src/ssid.egg-info/PKG-INFO
+-rw-r--r--   0 claudio   (1000) claudio   (1000)      545 2023-07-27 17:41:25.000000 ssid-0.0.5/src/ssid.egg-info/SOURCES.txt
+-rw-r--r--   0 claudio   (1000) claudio   (1000)        1 2023-07-27 17:41:25.000000 ssid-0.0.5/src/ssid.egg-info/dependency_links.txt
+-rw-r--r--   0 claudio   (1000) claudio   (1000)       44 2023-07-27 17:41:25.000000 ssid-0.0.5/src/ssid.egg-info/entry_points.txt
+-rw-r--r--   0 claudio   (1000) claudio   (1000)        5 2023-07-27 17:41:25.000000 ssid-0.0.5/src/ssid.egg-info/top_level.txt
+drwxr-xr-x   0 claudio   (1000) claudio   (1000)        0 2023-07-27 17:41:25.237501 ssid-0.0.5/tests/
+-rw-r--r--   0 claudio   (1000) claudio   (1000)     3468 2023-06-05 17:44:53.000000 ssid-0.0.5/tests/test1.py
```

### Comparing `ssid-0.0.4/setup.py` & `ssid-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `ssid-0.0.4/src/ssid/ExtractModes.py` & `ssid-0.0.5/src/ssid/archive/ExtractModes.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-from cmath import isclose
-from numpy import pi, log, sign
-from numpy.linalg import eig
-import numpy as np
-import scipy.linalg as sl
-
-def condeig(a): # TODO: make this match matlab source code for condeig
-    """
-    vals, vecs, conds = condeig(A) Computes condition numbers for the
-    eigenvalues of a matrix. The condition numbers are the reciprocals
-    of the cosines of the angles between the left and right eigenvectors.
-    Inspired by Arno Onken's Octave code for condeig.
-
-    https://github.com/macd/rogues/blob/master/rogues/utils/condeig.py
-    """
-    m, n = a.shape
-    # eigenvalues, left and right eigenvectors
-    lamr, vl, vr = sl.eig(a, left=True, right=True)
-    vl = vl.T.conj()
-    # Normalize vectors
-    for i in range(n):
-        vl[i, :] = vl[i, :] / np.sqrt(abs(vl[i, :] ** 2).sum())
-    # Condition numbers are reciprocal of the cosines (dot products) of the
-    # left eignevectors with the right eigenvectors.
-    c = abs(1 / np.diag(np.dot(vl, vr))) 
-    return vr, lamr, c
-
-def ComposeModes(dt, A, B, C, D, debug=False, **kwds)->dict:
-    
-    n = A.shape[0]
-    m = C.shape[0]
-
-    v, d, cnd = condeig(A)  # eigenvectors (d) & eiegenvalues (v) of the matrix A
-    # kit = np.log(d)         # logarithm of the eigenvalues
-
-    # a) Determination of modal frequencies (Eqs. 3.46 & 3.39)
-    sj1 = np.log(d)/dt            # dt is the time step
-    freq1 = (np.real(sj1*np.conj(sj1))**0.5)/(2*pi)
-
-    roots = []
-
-    # selection of proper roots
-    if np.isclose(freq1[0], freq1[1]):
-        roots.append(0)
-
-    if np.isclose(freq1[n-1], freq1[n-2]):
-        roots.append(n-1)
-
-    for i in range(2, n-2):
-        if np.isclose(freq1[i], freq1[i+1]) or np.isclose(freq1[i], freq1[i-1]):
-            roots.append(i)
- 
-
-    # b) Determination of damping ratios (Eqs. 3.46 & 3.39)
-    damp1 = -((np.real(sj1))/(2*pi*freq1))
-
-    # Represent the identified frequency & damping information
-    # of the proper roots in a matrix
-
-    # NOTE: These values are stored in one array like this for legacy reasons,
-    # but this should be cleaned and a proper data structure should be used!
-    freqdmp = np.array([
-               [freq1[i],   # first column: identified frequency
-                damp1[i],   # second column: identified damping ratio
-                cnd[i]]     # condition number of the eigenvalue
-            for i in roots
-    ])
-
-    # c) Determination of mode shapes
-    modes_raw = C@v   # mode shapes (Eq. 3.40)
-
-    modeshape = np.zeros((m,len(roots)), dtype=complex)
-
-    # extract mode shapes from mod corresponding to a frequency
-    for q,root in enumerate(roots):
-        modeshape[:m,q] = modes_raw[:m, root]
-
-    for q,root in enumerate(roots):
-        om  = np.argmax(abs(np.real(modeshape[:,q])))
-        mx  = abs(np.real(modeshape[om,q]))
-        modeshape[:,q] = np.real(modeshape[:,q])/mx*sign(np.real(modeshape[om,q]))
-
-    if debug:
-        return locals()
-    return freqdmp, modeshape, None, v, d
-
-def modes(dt, A, C):
-
-    # eigendecomp A
-    Psi,Gam,cnd = condeig(A)  # eigenvectors (Psi) & eigenvalues (Gam) of the matrix A
-
-    # get damping and frequencies from eigendecomp of A
-    Lam = (np.log(Gam))/dt
-    Omega = np.real((Lam*np.conj(Lam))**0.5)  # radians per second. taking the real part because np keeps a +0j.
-    freq = Omega/(2*pi) # cycles per second (Hz)
-    damp = -np.real(Lam)/Omega
-
-    # get modeshapes from C and eigendecomp of A
-    modeshape = C @ Psi
-
-    # nroots = int(len(freq)/2)
-    # # print(f"{freq=}")
-    # for i in range(nroots):
-    #     assert np.isclose(freq[2*i],freq[2*i+1])  # make sure we have pairs of roots
-
-    # modes = {str(i):
-    #             {'cnd': cnd[2*i],   # condition number of the eigenvalue
-    #             'freq': freq[2*i],  # identified frequency
-    #             'damp': damp[2*i],  # identified damping ratio
-    #             'modeshape': modeshape[:,2*i]
-    #             }
-    #         for i in range(nroots)
-    #         }
-
-    # return modes
-
-    # weed out unique roots: get indices of roots that only show up once, and
-    # the index of the first of each pair.
-    _, notroots = np.unique(freq.round(decimals=5), return_index=True)
-    
-    # print(notroots)
-    modes = {str(i):
-                {'cnd': cnd[i],   # condition number of the eigenvalue
-                'freq': freq[i],  # identified frequency
-                'damp': damp[i],  # identified damping ratio
-                'modeshape': modeshape[:,i]
-                }
-            for i in range(len(freq)) if i not in notroots
-            }
-
-    return modes
+from cmath import isclose
+from numpy import pi, log, sign
+from numpy.linalg import eig
+import numpy as np
+import scipy.linalg as sl
+
+def condeig(a): # TODO: make this match matlab source code for condeig
+    """
+    vals, vecs, conds = condeig(A) Computes condition numbers for the
+    eigenvalues of a matrix. The condition numbers are the reciprocals
+    of the cosines of the angles between the left and right eigenvectors.
+    Inspired by Arno Onken's Octave code for condeig.
+
+    https://github.com/macd/rogues/blob/master/rogues/utils/condeig.py
+    """
+    m, n = a.shape
+    # eigenvalues, left and right eigenvectors
+    lamr, vl, vr = sl.eig(a, left=True, right=True)
+    vl = vl.T.conj()
+    # Normalize vectors
+    for i in range(n):
+        vl[i, :] = vl[i, :] / np.sqrt(abs(vl[i, :] ** 2).sum())
+    # Condition numbers are reciprocal of the cosines (dot products) of the
+    # left eignevectors with the right eigenvectors.
+    c = abs(1 / np.diag(np.dot(vl, vr))) 
+    return vr, lamr, c
+
+def ComposeModes(dt, A, B, C, D, debug=False, **kwds)->dict:
+    
+    n = A.shape[0]
+    m = C.shape[0]
+
+    v, d, cnd = condeig(A)  # eigenvectors (d) & eiegenvalues (v) of the matrix A
+    # kit = np.log(d)         # logarithm of the eigenvalues
+
+    # a) Determination of modal frequencies (Eqs. 3.46 & 3.39)
+    sj1 = np.log(d)/dt            # dt is the time step
+    freq1 = (np.real(sj1*np.conj(sj1))**0.5)/(2*pi)
+
+    roots = []
+
+    # selection of proper roots
+    if np.isclose(freq1[0], freq1[1]):
+        roots.append(0)
+
+    if np.isclose(freq1[n-1], freq1[n-2]):
+        roots.append(n-1)
+
+    for i in range(2, n-2):
+        if np.isclose(freq1[i], freq1[i+1]) or np.isclose(freq1[i], freq1[i-1]):
+            roots.append(i)
+ 
+
+    # b) Determination of damping ratios (Eqs. 3.46 & 3.39)
+    damp1 = -((np.real(sj1))/(2*pi*freq1))
+
+    # Represent the identified frequency & damping information
+    # of the proper roots in a matrix
+
+    # NOTE: These values are stored in one array like this for legacy reasons,
+    # but this should be cleaned and a proper data structure should be used!
+    freqdmp = np.array([
+               [freq1[i],   # first column: identified frequency
+                damp1[i],   # second column: identified damping ratio
+                cnd[i]]     # condition number of the eigenvalue
+            for i in roots
+    ])
+
+    # c) Determination of mode shapes
+    modes_raw = C@v   # mode shapes (Eq. 3.40)
+
+    modeshape = np.zeros((m,len(roots)), dtype=complex)
+
+    # extract mode shapes from mod corresponding to a frequency
+    for q,root in enumerate(roots):
+        modeshape[:m,q] = modes_raw[:m, root]
+
+    for q,root in enumerate(roots):
+        om  = np.argmax(abs(np.real(modeshape[:,q])))
+        mx  = abs(np.real(modeshape[om,q]))
+        modeshape[:,q] = np.real(modeshape[:,q])/mx*sign(np.real(modeshape[om,q]))
+
+    if debug:
+        return locals()
+    return freqdmp, modeshape, None, v, d
+
+def modes(dt, A, C):
+
+    # eigendecomp A
+    Psi,Gam,cnd = condeig(A)  # eigenvectors (Psi) & eigenvalues (Gam) of the matrix A
+
+    # get damping and frequencies from eigendecomp of A
+    Lam = (np.log(Gam))/dt
+    Omega = np.real((Lam*np.conj(Lam))**0.5)  # radians per second. taking the real part because np keeps a +0j.
+    freq = Omega/(2*pi) # cycles per second (Hz)
+    damp = -np.real(Lam)/Omega
+
+    # get modeshapes from C and eigendecomp of A
+    modeshape = C @ Psi
+
+    # nroots = int(len(freq)/2)
+    # # print(f"{freq=}")
+    # for i in range(nroots):
+    #     assert np.isclose(freq[2*i],freq[2*i+1])  # make sure we have pairs of roots
+
+    # modes = {str(i):
+    #             {'cnd': cnd[2*i],   # condition number of the eigenvalue
+    #             'freq': freq[2*i],  # identified frequency
+    #             'damp': damp[2*i],  # identified damping ratio
+    #             'modeshape': modeshape[:,2*i]
+    #             }
+    #         for i in range(nroots)
+    #         }
+
+    # return modes
+
+    # weed out unique roots: get indices of roots that only show up once, and
+    # the index of the first of each pair.
+    _, notroots = np.unique(freq.round(decimals=5), return_index=True)
+    
+    # print(notroots)
+    modes = {str(i):
+                {'cnd': cnd[i],   # condition number of the eigenvalue
+                'freq': freq[i],  # identified frequency
+                'damp': damp[i],  # identified damping ratio
+                'modeshape': modeshape[:,i]
+                }
+            for i in range(len(freq)) if i not in notroots
+            }
+
+    return modes
```

### Comparing `ssid-0.0.4/src/ssid/brace2/__main__.py` & `ssid-0.0.5/src/ssid/brace2/__main__.py`

 * *Files identical despite different names*

### Comparing `ssid-0.0.4/src/ssid/integrate.py` & `ssid-0.0.5/src/ssid/integrate.py`

 * *Files identical despite different names*

### Comparing `ssid-0.0.4/src/ssid/markov.py` & `ssid-0.0.5/src/ssid/markov.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import numpy as np
-import warnings
-
-# inputs = input data. dimensions of inputs: q x nt, where nt = number of timesteps.
-# outputs = response data due to input data. dimensions of outputs: p x nt.
-# m = number of Markov parameters (impulse response timesteps), not including timestep zero, to solve for.
-def okid(inputs,outputs,m=None,**options):
-    if len(inputs.shape) == 1:
-        inputs = inputs[None,:]
-    if len(outputs.shape) == 1:
-        outputs = outputs[None,:]
-    
-    if inputs.shape[0] > inputs.shape[1]:
-        warnings.warn("input data has more channels (dim 1) than timesteps (dim 2)")
-    if outputs.shape[0] > outputs.shape[1]:
-        warnings.warn("output data has more channels (dim 1) than timesteps (dim 2)")
-
-    q,nt = inputs.shape
-    p = outputs.shape[0]
-    assert nt == outputs.shape[1]
-    
-    if m is None:
-        m = min(300,nt)
-
-    # Form data matrix V
-    V = np.zeros((m+1,nt,q+p))                  # m+1 block rows, each with nt columns and q+p rows each.  DIM: (m+1)x(nt)x(q+p)
-    for i in range(m+1):                        # From block row 0 to block row m
-        V[i,-(nt-i):,:q] = inputs[:,:nt-i].T     # Populate the first q rows of the ith block row, last nt-i columns, with the first nt-i inputs.  DIM: (nt-i)x(q)
-        V[i,-(nt-i):,-p:] = outputs[:,:nt-i].T   # Populate the last p rows of the ith block row, last nt-i columns, with the first nt-i outputs.  DIM: (nt-i)x(p)
-    V = V.transpose((1,0,2)).reshape((nt,(m+1)*(p+q))).T    # Transpose and reshape data matrix to stack the block rows in.  DIM: ((m+1)(q+p))x(nt)
-    # V = np.concatenate((V[:q,:],V[q+p:,:]))     # Remove rows q+1 to q+p (TODO: see if it's necessary to remove rows, or if solving for Ybar can include these)
-    V = np.delete(V, slice(q,q+p), axis=0)      # Remove rows q+1 to q+p (TODO: see if it's necessary to remove rows, or if solving for Ybar can include these)
-
-    # Solve for observer Markov parameters Ybar
-    Ybar = outputs @ np.linalg.pinv(V,rcond=10**(-3))  # DIM: (p)x(q+m(q+p))
-    assert Ybar.shape == (p,q+m*(q+p))
-    
-    # Isolate system Markov parameters
-    H = np.zeros((p,q,m+1))
-    D = Ybar[:,:q] # feed-through term (or D matrix) is the first block column
-    H[:,:,0] = D
-
-    Y = np.zeros((p,q,m))
-    Ybar1 = np.zeros((p,q,m))
-    Ybar2 = np.zeros((p,q,m))
-    
-    for i in range(m):
-        Ybar1[:,:,i] = Ybar[:,q+(q+p)*i : q+(q+p)*i+q]
-        Ybar2[:,:,i] = Ybar[:,q+(q+p)*i+q : q+(q+p)*(i+1)]
-    
-    Y[:,:,0] = Ybar1[:,:,0] + Ybar2[:,:,0] @ D
-    for k in range(1,m):
-        Y[:,:,k] = Ybar1[:,:,k] + Ybar2[:,:,k] @ D
-        for i in range(k-1):
-            Y[:,:,k] += Ybar2[:,:,i] @ Y[:,:,k-i-1]
-
-    H[:,:,1:] = Y
-
+import numpy as np
+import warnings
+
+# inputs = input data. dimensions of inputs: q x nt, where nt = number of timesteps.
+# outputs = response data due to input data. dimensions of outputs: p x nt.
+# m = number of Markov parameters (impulse response timesteps), not including timestep zero, to solve for.
+def okid(inputs,outputs,m=None,**options):
+    if len(inputs.shape) == 1:
+        inputs = inputs[None,:]
+    if len(outputs.shape) == 1:
+        outputs = outputs[None,:]
+    
+    if inputs.shape[0] > inputs.shape[1]:
+        warnings.warn("input data has more channels (dim 1) than timesteps (dim 2)")
+    if outputs.shape[0] > outputs.shape[1]:
+        warnings.warn("output data has more channels (dim 1) than timesteps (dim 2)")
+
+    q,nt = inputs.shape
+    p = outputs.shape[0]
+    assert nt == outputs.shape[1]
+    
+    if m is None:
+        m = min(300,nt)
+
+    # Form data matrix V
+    V = np.zeros((m+1,nt,q+p))                  # m+1 block rows, each with nt columns and q+p rows each.  DIM: (m+1)x(nt)x(q+p)
+    for i in range(m+1):                        # From block row 0 to block row m
+        V[i,-(nt-i):,:q] = inputs[:,:nt-i].T     # Populate the first q rows of the ith block row, last nt-i columns, with the first nt-i inputs.  DIM: (nt-i)x(q)
+        V[i,-(nt-i):,-p:] = outputs[:,:nt-i].T   # Populate the last p rows of the ith block row, last nt-i columns, with the first nt-i outputs.  DIM: (nt-i)x(p)
+    V = V.transpose((1,0,2)).reshape((nt,(m+1)*(p+q))).T    # Transpose and reshape data matrix to stack the block rows in.  DIM: ((m+1)(q+p))x(nt)
+    # V = np.concatenate((V[:q,:],V[q+p:,:]))     # Remove rows q+1 to q+p (TODO: see if it's necessary to remove rows, or if solving for Ybar can include these)
+    V = np.delete(V, slice(q,q+p), axis=0)      # Remove rows q+1 to q+p (TODO: see if it's necessary to remove rows, or if solving for Ybar can include these)
+
+    # Solve for observer Markov parameters Ybar
+    Ybar = outputs @ np.linalg.pinv(V,rcond=10**(-3))  # DIM: (p)x(q+m(q+p))
+    assert Ybar.shape == (p,q+m*(q+p))
+    
+    # Isolate system Markov parameters
+    H = np.zeros((p,q,m+1))
+    D = Ybar[:,:q] # feed-through term (or D matrix) is the first block column
+    H[:,:,0] = D
+
+    Y = np.zeros((p,q,m))
+    Ybar1 = np.zeros((p,q,m))
+    Ybar2 = np.zeros((p,q,m))
+    
+    for i in range(m):
+        Ybar1[:,:,i] = Ybar[:,q+(q+p)*i : q+(q+p)*i+q]
+        Ybar2[:,:,i] = Ybar[:,q+(q+p)*i+q : q+(q+p)*(i+1)]
+    
+    Y[:,:,0] = Ybar1[:,:,0] + Ybar2[:,:,0] @ D
+    for k in range(1,m):
+        Y[:,:,k] = Ybar1[:,:,k] + Ybar2[:,:,k] @ D
+        for i in range(k-1):
+            Y[:,:,k] += Ybar2[:,:,i] @ Y[:,:,k-i-1]
+
+    H[:,:,1:] = Y
+
     return H
```

### Comparing `ssid-0.0.4/src/ssid/modal.py` & `ssid-0.0.5/src/ssid/modal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,91 @@
-import numpy as np
-import scipy.linalg as sl
-from numpy import pi
-from ssid.validation import OutputEMAC, MPC
-
-def condeig(a): # TODO: make this match matlab source code for condeig
-    """
-    vals, vecs, conds = condeig(A) Computes condition numbers for the
-    eigenvalues of a matrix. The condition numbers are the reciprocals
-    of the cosines of the angles between the left and right eigenvectors.
-    Inspired by Arno Onken's Octave code for condeig.
-
-    https://github.com/macd/rogues/blob/master/rogues/utils/condeig.py
-    """
-    m, n = a.shape
-    # eigenvalues, left and right eigenvectors
-    lamr, vl, vr = sl.eig(a, left=True, right=True)
-    vl = vl.T.conj()
-    # Normalize vectors
-    for i in range(n):
-        vl[i, :] = vl[i, :] / np.sqrt(abs(vl[i, :] ** 2).sum())
-    # Condition numbers are reciprocal of the cosines (dot products) of the
-    # left eignevectors with the right eigenvectors.
-    c = abs(1 / np.diag(np.dot(vl, vr))) 
-    return vr, lamr, c
-
-def system_modes(realization, dt, Observability=None, nt=None):
-
-    if nt is None:
-        nt = 100
-
-    A,_,C,_ = realization
-    # eigendecomp A
-    Psi,Gam,cnd = condeig(A)  # eigenvectors (Psi) & eigenvalues (Gam) of the matrix A
-
-    # get damping and frequencies from eigendecomp of A
-    Lam = (np.log(Gam))/dt
-    # TODO: maybe clean
-    Omega = np.real((Lam*np.conj(Lam))**0.5)  # radians per second. taking the real part because numpy keeps a +0j.
-    # Omega = np.real_if_close((Lam*np.conj(Lam))**0.5) # use real_if_close
-    freq = Omega/(2*pi) # cycles per second (Hz)
-    Omega.__str__() # helps to avoid "divide by zero" numpy warning message
-    # print(Omega)
-    damp = -np.real(Lam)/Omega
-
-    # get modeshapes from C and eigendecomp of A
-    modeshape = C@Psi
-
-    # energy condensed output EMAC (extended modal amplitude coherence)
-    energy_condensed_emaco = OutputEMAC(A,C,nt,Observability=Observability,Psi=Psi,Gam=Gam)
-
-    # MPC (modal phase collinearity)
-    mpc = MPC(A,C,Psi=Psi)
-
-    # weed out unique roots: get indices of (1) roots that only show up once, and
-    # (2) the first of each pair.
-    _, notroots = np.unique(freq.round(decimals=5), return_index=True)
-    
-    # print(notroots)
-    modes = {str(i):
-                {'freq': freq[i],  # identified frequency
-                'damp': damp[i],   # identified damping ratio
-                'modeshape': modeshape[:,i],  # identified modeshape
-                'cnd': cnd[i],     # condition number of the eigenvalue
-                'energy_condensed_emaco': energy_condensed_emaco[i],  # energy condensed output emac
-                'mpc': mpc[i],     # MPC
-                }
-            for i in range(len(freq)) if i not in notroots # and energy_condensed_emaco[i] > 0.5 and mpc[i] > 0.5
-            }
-
-    return modes
+import numpy as np
+import scipy.linalg as sl
+from numpy import pi
+from ssid.validation import OutputEMAC, MPC
+
+def condeig(a): # TODO: make this match matlab source code for condeig
+    """
+    vals, vecs, conds = condeig(A) Computes condition numbers for the
+    eigenvalues of a matrix. The condition numbers are the reciprocals
+    of the cosines of the angles between the left and right eigenvectors.
+    Inspired by Arno Onken's Octave code for condeig.
+
+    https://github.com/macd/rogues/blob/master/rogues/utils/condeig.py
+    """
+    m, n = a.shape
+    # eigenvalues, left and right eigenvectors
+    lamr, vl, vr = sl.eig(a, left=True, right=True)
+    vl = vl.T.conj()
+    # Normalize vectors
+    for i in range(n):
+        vl[i, :] = vl[i, :] / np.sqrt(abs(vl[i, :] ** 2).sum())
+    # Condition numbers are reciprocal of the cosines (dot products) of the
+    # left eignevectors with the right eigenvectors.
+    c = abs(1 / np.diag(np.dot(vl, vr))) 
+    return vr, lamr, c
+
+def system_modes(realization, dt, decimation=1, Observability=None, nt=None):
+
+    dt = dt*decimation
+
+    if nt is None:
+        nt = 100
+
+    A,_,C,_ = realization
+    # eigendecomp A
+    Psi,Gam,cnd = condeig(A)  # eigenvectors (Psi) & eigenvalues (Gam) of the matrix A
+
+    # get damping and frequencies from eigendecomp of A
+    Lam = (np.log(Gam))/dt
+    # TODO: maybe clean
+    Omega = np.real((Lam*np.conj(Lam))**0.5)  # radians per second. taking the real part because numpy keeps a +0j.
+    # Omega = np.real_if_close((Lam*np.conj(Lam))**0.5) # use real_if_close
+    freq = Omega/(2*pi) # cycles per second (Hz)
+    Omega.__str__() # helps to avoid "divide by zero" numpy warning message
+    # Lam_real = np.real(Lam)
+    # Lam_real+=1
+    # Lam_real-=1
+    # Omega_real = np.real(Omega)
+    # Omega_real+=1
+    # Omega_real-=1
+    # del Omega
+    # del Lam
+    # import gc
+    # gc.collect()
+    # print(Omega_real)
+    # print(Lam_real)
+    # damp = -Lam_real/Omega_real
+    damp = -np.real(Lam)/Omega
+
+    # get modeshapes from C and eigendecomp of A
+    modeshape = C@Psi
+
+    # energy condensed output EMAC (extended modal amplitude coherence)
+    energy_condensed_emaco = OutputEMAC(A,C,nt,Observability=Observability,Psi=Psi,Gam=Gam)
+
+    # MPC (modal phase collinearity)
+    mpc = MPC(A,C,Psi=Psi)
+
+    # weed out unique roots: get indices of (1) roots that only show up once, and
+    # (2) the first of each pair.
+    _, notroots = np.unique(freq.round(decimals=5), return_index=True)
+    
+    # print(notroots)
+    modes = {str(i):
+                {'freq': freq[i],  # identified frequency
+                'damp': damp[i],   # identified damping ratio
+                'modeshape': modeshape[:,i],  # identified modeshape
+                'cnd': cnd[i],     # condition number of the eigenvalue
+                'energy_condensed_emaco': energy_condensed_emaco[i],  # energy condensed output emac
+                'mpc': mpc[i],     # MPC
+                }
+            for i in range(len(freq)) if i not in notroots # and energy_condensed_emaco[i] > 0.5 and mpc[i] > 0.5
+            }
+
+    return modes
+
+def spectrum_modes(periods, amplitudes, nmodes=1):
+    highest_amplitude_indices = np.argpartition(-amplitudes, range(nmodes))[:nmodes]  # TODO: peak picking algorithm
+    fundamental_periods = periods[highest_amplitude_indices]
+    fundamental_amplitudes = amplitudes[highest_amplitude_indices]
+    return (fundamental_periods, fundamental_amplitudes)
```

### Comparing `ssid-0.0.4/src/ssid/okid.py` & `ssid-0.0.5/src/ssid/archive/okid.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,580 +1,580 @@
-import numpy as np
-from numpy import zeros, pi, size
-import scipy.linalg
-from scipy.linalg import fractional_matrix_power as matpow
-
-linsolve = scipy.linalg.solve
-
-lsqminnorm = lambda *args: np.linalg.lstsq(*args, rcond=None)[0]
-
-def parse_okid(args, config):
-    """
-    p determines order of the observer Kalman ARX filter used in OKID-ERA-DC.
-    n determines size of the state-space model used for representing the system.
-    """
-    return config
-
-# y = output data: forced response. dimensions of y: p x nt, where nt = number of timesteps
-# u = input data: input. dimensions of u: q x nt.
-# m = number of Markov parameters (impulse response timesteps) to solve for
-def get_impulse(y, u):
-    p = y.shape[0]
-    q = u.shape[0]
-    nt = y.shape[1]
-    assert y.shape[1] == u.shape[1]
-    # form a blockwise upper triangular matrix of inputs
-    U = np.zeros((q*nt, nt))
-    for i in range(nt):
-        for j in range(nt-i):
-            U[q*j:q*(j+1),i] = u[:,i]
-    Y_impulse = y @ np.linalg.pinv(U)
-    assert Y_impulse.shape == (p, q*nt)
-    return Y_impulse
-
-def okid2(y, u, m):
-    p = y.shape[0]
-    q = u.shape[0]
-    nt = y.shape[1]
-    assert y.shape[1] == u.shape[1]
-    # form a blockwise upper triangular matrix of inputs
-    U = np.zeros((q*nt, nt))
-    for i in range(nt):
-        for j in range(nt-i):
-            U[q*j:q*(j+1),i] = u[:,i]
-    Y_impulse = y @ np.linalg.pinv(U)
-    assert Y_impulse.shape == (p, q*nt)
-    return Y_impulse
-
-def OKID_brunton(y,u,m):
-    
-    p = y.shape[0]
-    q = u.shape[0]
-    nt = y.shape[1]
-    assert y.shape[1] == u.shape[1]
-    
-    # Form data matrices y and V
-    V = np.zeros((q+(q+p)*m,nt))
-    for i in range(nt):
-        V[:q,i] = u[:q,i]
-        
-    for i in range(1,m+1):
-        for j in range(nt-i):
-            vtemp = np.concatenate((u[:,j],y[:,j]))
-            V[q+(i-1)*(q+p):q+i*(q+p),i+j] = vtemp
-    
-    # Solve for observer Markov parameters Ybar
-    Ybar = y @ np.linalg.pinv(V,rcond=10**(-3))
-    
-    # Isolate system Markov parameters H, and observer gain M
-    D = Ybar[:,:q] # feed-through term (or D matrix) is the first term
-    
-    Y = np.zeros((p,q,m))
-    Ybar1 = np.zeros((p,q,m))
-    Ybar2 = np.zeros((p,q,m))
-    
-    for i in range(m):
-        Ybar1[:,:,i] = Ybar[:,q+(q+p)*i : q+(q+p)*i+q]
-        Ybar2[:,:,i] = Ybar[:,q+(q+p)*i+q : q+(q+p)*(i+1)]
-    
-    Y[:,:,0] = Ybar1[:,:,0] + Ybar2[:,:,0] @ D
-    for k in range(1,m):
-        Y[:,:,k] = Ybar1[:,:,k] + Ybar2[:,:,k] @ D
-        for i in range(k-1):
-            Y[:,:,k] += Ybar2[:,:,i] @ Y[:,:,k-i-1]
-            
-    H = np.zeros((D.shape[0],D.shape[1],m+1))
-    H[:,:,0] = D
-    
-    for k in range(1,m+1):
-        H[:,:,k] = Y[:,:,k-1]
-        
-    return H
-
-# Y = output data: response to unit impulse, or "impulse response," or "Markov parameters".
-# dimensions of Y: p x q x nt, where nt = number of timesteps = number of Markov parameters = number of blocks
-# mc = number of block rows in Hankel matrix = order of controllability matrix
-# mo = number of block columns in Hankel matrix = order of observability matrix
-# p = number of outputs
-# q = number of inputs
-# r = reduced model order = dimension of reduced A = newly assumed dimension of state variable
-def era(Y,mo,mc,p,q,r):
-    # get D from first p x q block of impulse response
-    Dr = Y[:,:,0]  # first block of output data
-    
-    assert Y.shape[:2] == (p,q)  # sanity check that we're passing in the right output data
-    assert Y.shape[2] >= mo+mc   # make sure there are enough timesteps to assemble this size of Hankel matrix
-    
-    # make impulse response into Hankel matrix and shifted Hankel matrix
-    H = np.zeros((p*(mo), q*(mc+1)))
-    for i in range(mo):
-        for j in range(mc+1):
-            H[p*i:p*(i+1), q*j:q*(j+1)] = Y[:,:,i+j+1]
-    H0 = H[:,:-q]
-    H1 = H[:,q:]
-    assert H0.shape == H1.shape == (p*(mo), q*(mc))
-
-    # reduced SVD of Hankel matrix
-    def _svd(*args):
-        U,S,V = scipy.linalg.svd(*args, lapack_driver="gesvd")
-        return U,S,V.T.conj()
-    U,S,V = _svd(H0)
-    SigmaInvSqrt = np.diag(S[:r]**-0.5)
-    SigmaSqrt = np.diag(S[:r]**0.5)
-    Ur = U[:,:r]
-    Vr = V[:,:r]
-
-    # get A from SVD and shifted Hankel matrix
-    Ar = SigmaInvSqrt @ Ur.T.conj() @ H1 @ Vr @ SigmaInvSqrt
-
-    # get B and C
-    Br = (SigmaSqrt @ Vr.T.conj())[:,:q]
-    Cr = (Ur @ SigmaSqrt)[:p,:]
-
-    return (Ar,Br,Cr,Dr,S)
-
-# l = initial lag for data correlations
-# g = lags between correlation matrices
-# a = number of block rows in Hankel of correlation matrix
-# b = number of block columns in Hankel of correlation matrix
-def era_dc(Y,mo,mc,p,q,r,l,g,a,b):
-    # get D from first p x q block of impulse response
-    Dr = Y[:,:,0]  # first block of output data
-    
-    assert Y.shape[:2] == (p,q)  # sanity check that we're passing in the right output data
-    assert Y.shape[2] >= l+(a+1+b+1)*g+mo+mc   # make sure there are enough timesteps to assemble the Hankel matrices
-    
-    # make impulse response into Hankel matrix
-    H = np.zeros((p*(mo), q*(mc+l+(a+1+b+1)*g))) # Hankel of Markov parameters
-    for i in range(mo):
-        for j in range(mc+l+(a+1+b+1)*g):
-            H[p*i:p*(i+1), q*j:q*(j+1)] = Y[:,:,i+j+1]
-    H0 = H[:,:q*mc]
-    assert H0.shape == (p*(mo), q*(mc))
-
-    dimR = p*mo # Dimension of square correlation matrices
-    dimHRl = (dimR*(a+1), dimR*(b+1)) # Dimension of Hankels of correlation matrices
-    HRl = np.zeros(dimHRl) # Hankel of correlation matrices
-    HRl1 = np.zeros(dimHRl) # Shifted Hankel of correlation matrices
-    for i in range(a+1):
-        for j in range(b+1):
-            Hl = H[:, q*(l+1+(i+j)*g):q*(l+1+(i+j)*g+mc)]
-            Hl1 = H[:, q*(l+1+(i+j)*g+1):q*(l+1+(i+j)*g+mc+1)]
-            assert Hl.shape == Hl1.shape == (p*(mo), q*(mc))
-            R = Hl@H0
-            R1 = Hl1@H0
-            assert R.shape == R1.shape == (dimR,dimR)
-            HRl[dimR*i:dimR*(i+1), dimR*j:dimR*(j+1)] = R
-            HRl1[dimR*i:dimR*(i+1), dimR*j:dimR*(j+1)] = R1
-
-    # reduced SVD of Hankel matrix
-    def _svd(*args):
-        U,S,V = scipy.linalg.svd(*args, lapack_driver="gesvd")
-        return U,S,V.T.conj()
-    U,S,V = _svd(HRl)
-    SigmaInvSqrt = np.diag(S[:r]**-0.5)
-    SigmaSqrt = np.diag(S[:r]**0.5)
-    Ur = U[:,:r]
-    Vr = V[:,:r]
-
-    # get A from SVD and shifted Hankel matrix
-    Ar = SigmaInvSqrt @ Ur.T.conj() @ HRl1 @ Vr @ SigmaInvSqrt
-
-    # get B and C
-    Br = ((SigmaInvSqrt @ Ur.T.conj())[:,:dimR] @ H0)[:,:q]
-    Cr = (Ur @ SigmaSqrt)[:p,:]
-
-    return (Ar,Br,Cr,Dr,S)
-
-
-def _era_ya(kmax, m, l, r, Y, n, svd="gesvd"):
-    # ERA/DC
-    #
-    # Form Hankel matrix (H) from the Markov parameters (Y) (Eq. 3.80)
-
-    # Obtain Hankel Matrix of Zeroth Order & First Order
-    H0,H1 = np.zeros((2, kmax*m, l*r))
-    #H0 = hankel(Y,0)
-    for hj in range(kmax):
-        for jh in range(l):
-            H0[hj*m:hj*m+m, jh*r:jh*r+r] = Y[jh+hj+1]
-            H1[hj*m:hj*m+m, jh*r:jh*r+r] = Y[jh+hj+2]
-    
-    if svd in ["gesvd", "gesdd"]:
-        import scipy.linalg
-        def _svd(*args):
-            U,S,V = scipy.linalg.svd(*args, lapack_driver=svd)
-            return U,S,V.T.conj()
-
-    ## 2c. Use H matrix to compute system matrices A, B & C
-    R1,sis,S1 = _svd(H0) # singular value decomposition
-    Sis = np.diag(sis[:n])
-
-    Siv = np.diag(1/np.sqrt(sis[:n]))
-    # A: state transition matrix (Eqs. 3.32 & 3.82)
-    A  = Siv@R1[:,:n].T@H1@S1[:,:n]@Siv
-    # B: input influence matrix (Eqs. 3.32 & 3.83)
-    B = (np.sqrt(Sis)@S1[:,:n].T)[:,:r]
-    Observability = R1[:,:n]@np.sqrt(Sis)
-    # C: output influence matrix (Eqs. 3.34 & 3.84)
-    C  = Observability[:m,:]
-
-    return A,B,C
-
-
-def okid(dati, dato, svd="gesvd", debug=False, **config):
-    """
-    PART 2: OKID-ERA-DC (Observer Kalman filter Identification -
-            Eigen Realization with Direct Correlations)
-    -----------------------------------------------------------------
-
-    # Inputs
-    Modelparameters
-        div = 1;     # A parameter used for decimating data. 1 uses entire data without downsampling.
-        mro = 10;    # Model reduction order
-        orm = 4;     # Order of the model. # of computed and plotted modes dep on orm.
-                     # For orm = 2, one mode is found, for orm = 4, two modes are found.
-    svd:
-        GESDD: a two-stage algorithm. It first reduces the input matrix to bidiagonal form via 
-        Householder reflection, then divides the bidiagonal matrix into smaller matrices to calculate 
-        singular values and the unitary matrices U and V. Finally, the singular values of the entire 
-        input matrix is simply the those of the smaller sub-matrices.
-        
-        GESVD: also a two-stage algorithm where the first step is identical to GESDD. The second step 
-        can be done using iterative QR decomposition to derive singular values. More mathematical details are available here.
-
-    Sometimes higher orm still gives fewer modes, e.g. orm = 8 for case 1 gives
-    three modes, but one of them is invalid according to the EMAC & MPC criteria.
-    kmax = 100;  #Number of computed Markov parameters, indicated as 1000 on page 43 of
-    (Arici & Mosalam, 2006). However, it was input as 100 in the code.
-    kmax = 100 runs much faster & both kmax = 100 & 1000 give the same results.
-
-    # Outputs
-    1. freqdamp variable is a matrix that includes the information of identified
-       frequencies, damping ratios & validation of the modes with MPC & EMAC criteria
-       Each row of freqdamp corresponds to a mode. Columns are as follows:
-       1) frequency, 2) damping ratio, 3) order index, 4) condition number, 5) input EMAC,
-       6) output EMAC, 7) MPC. If values in columns 5-7 are > 0.5, identified mode is valid.
-    2. modeshape stores the mode shape information for identified modes.
-    3. RMSEpred: root mean square error of the predicted output from
-       identified parameters with respect to the actual output.
-    4. Markovparamerror: root mean square error used to validate accurate
-       computation of Markov parameters
-
-    # Description of the Methodology
-    More information on OKID-ERA-DC method can be found in
-    Section 3.4.6 of (Arici & Mosalam, 2006). Equations below refer to this report.
-    OKID-ERA-DC is a Multiple Input - Multiple Output (MIMO) System Identification (SI) method
-    that consists of the following steps:
-    1. Data pre-processing (baseline correction, filtering & decimation)
-    2. Identify observer Kalman filters using Observer Kalman filter Identification (OKID)
-       methodology. This step basically consists of developing a simple observer model of
-       a system from a MIMO ARX structure, Eq. (3.76), which is broken into these 6 steps:
-   
-    3a. Determine Markov parameters (M) in a least squares sense, Eq. (3.76).
-
-    3b. Establish the Hankel matrix (H) from the Markov parameters, (Eq. 3.80).
-    3c. Use H to compute system matrices A, B & C, in which modal information is embedded.
-    // 3d. Obtain the modal information from matrices A, B & C.
-    3e. Spatial & temporal validation of the identified modes.
-    3f. Back calculate (estimate) the output accelerations with the state-space system &
-        check against the actual output accelerations.
-    """ 
-    dt = to = config.get("dt", None) or dati["time_step"]
-    p = config.get("p", config.get("mro")) # # steps used for the identification (ie, prediction horizon)
-    n = n1 = config.get("n", config.get("orm", 4))  # Order of the model.
-    
-    if svd in ["gesvd", "gesdd"]:
-        import scipy.linalg
-        def _svd(*args):
-            U,S,V = scipy.linalg.svd(*args, lapack_driver=svd)
-            return U,S,V.T.conj()
-
-    elif svd in ["xla", "jax"]:
-        from jax.scipy.linalg import svd as _svd
-
-    if isinstance(dati, list):
-        dati = np.array([i.data for i in dati]).T
-    elif issubclass(dati.__class__, dict):
-        dati = dati.data
-
-    if isinstance(dato, list):
-        dato = np.array([i.data for i in dato]).T
-    elif issubclass(dato.__class__, dict):
-        dato = dato.data
-
-    if len(dati.shape) < 2:
-        dati = np.atleast_2d(dati).T
-    if len(dato.shape) < 2:
-        dato = np.atleast_2d(dato).T
-        
-    dati = dati[:-1,:]
-    dato = dato[:-1,:]
-
-    #verbose = True
-    #dn = config.get("dn", None) or dati.shape[0]
-    kmax    = config["kmax"]
-    n = config["orm"]   # assign order of model input to variable n, consistent with Eqs. 3.81-3.84
-    p = config["mro"]   # assign input model reduction order to variable p, consistent with Eq. 3.76
-
-
-    l,m = dato.shape # m is the number of output channels
-    _,r = dati.shape # r is the number of input channels
-
-    # ASSERT SIZE(DATO,1) == SIZE(DATI,1)
-
-    ## 2a. Obtain Observer Markov Parameters
-    # The Markov parameters are computed in two steps:
-    # i)  The Observer Markov matrices are computed from Eq. 3.76 using a linear regression approach
-    # ii) Compute the system Markov parameters from the Markov matrices using recursive relations
-
-    # Compute matrix U that represents ARX equation of current output on p time steps of past output
-    # & input values (Eq. 3.76)
-    U = np.zeros(((m+r)*p+r, l))
-    U[:r,:] = dati.T
-    for b in range(1,p+1):
-        U[(b-1)*(r+m)+r:(b-1)*(r+m)+r+r+m, b:] = [*dati[:-b,:r].T, *dato[:-b, :m].T]
-
-
-    # i) Compute the matrix of Observer Markov Parameter Matrix (M)
-    #    in Eq 3.76 using Linear Regression
-    uu,wr,V = _svd(U,0)
-    pg = (r+m)*p+r
-    for i in range((r+m)*p+r):
-        if wr[i] <= 0.001:
-            pg = i
-            break
-
-    s = np.diag(wr)
-
-    pss = V[:,:pg]@linsolve(s[:pg,:pg], uu[:,:pg].T)
-    M = dato.T@pss           # M: Observer Markov Parameter Matrix
-
-    # Fit for multiple regression
-    # RMSE between actual output & y on left hand side in Eq. 3.76. It should be 
-    # quite small (e.g., 10^-3) for accurately computed Markow parameters.
-    # ypreo = M@U
-    # markovParamError = 1/m*sum((
-    #     sum((dato[:,i] - ypreo[i,:].T)**2)/sum(dato[:,i]**2)
-    #     for i in range(m)
-    # ))  
-
-
-    ## ii) Compute Markov parameters (Y) using recursive relations in Eqs. 3.78 & 3.79
-    #      (Equation 6.21 in Juang 1994)
-
-    # Matrix D is directly equal to the Observer Markov parameter matrix (Eq. 3.77)
-    D = M[:, :r]  # D: Direct Transmission term
-
-    Y = [D]
-    # First p steps (Eq. 3.78)
-    for i in range(p):
-        Y.append(
-            M[:, r+i*(r+m):r+i*(r+m)+r] + sum(
-                M[:, r+j*(r+m)+r:r+j*(r+m)+r+m]@Y[i-j]
-                for j in range(i+1)
-            )
-        )
-    # Remainder (Eq. 3.79)
-    for i in range(p, l+kmax):
-        sumt = zeros((m,r))
-        for j in range(p):
-            sumt += M[:,r+j*(r+m)+r:r+j*(r+m)+r+m]@Y[i-j]
-
-        Y.append(sumt)
-
-    # The Markow parameters Y have been computed.
-
-    A,B,C = _era_ya(kmax, m, l, r, Y, _svd, n)
-
-    if debug:
-        return locals()
-
-    return A,B,C,D
-
-
-def validate(freqdmp, v, system, **config):
-    """2e. Validation Analysis
-
-    Two criteria are used for selection of identified genuine modes
-    (in the sense of spatial & temporal consistency).
-
-    a) Modal Phase Collinearity (MPC) testing spatial consistency of identification results.
-       Modes having MPC value above 0.5 (mpc parameter below) are considered as genuine modal quantities.
-
-    b) Exted Modal Amplitude Coherence (EMAC), evaluates temporal consistency of the identification results.
-       Both output EMAC & input EMAC can be computed. Input EMAC requires the controllability matrix.
-       Because the controllability matrix is not estimated by all considered SI methods,
-       this criterion is computed, but not used.
-       Modes with output EMAC values < 0.5 are considered spurious & therefore not reported.
-
-    """
-    mpc = MPC(n, v, system)
-
-    # Add the input EMAC, output EMAC, and MPC to the matrix freqdamp
-    for lih in range(size(freqdmp)[0]):
-        freqdmp[lih,4] = emacif(freqdmp[lih,2])
-        freqdmp[lih,5] = emacof(freqdmp[lih,2])
-        freqdmp[lih,6] = mpc[freqdmp(lih,3)]
-        if freqdmp[lih,5]>0.5 and freqdmp[lih,7]>0.5:
-            # valid
-            return True
-        else:
-            # not valid
-            return False
-
-def MPC(n, v, system):
-    """a) Modal Phase Collinearity (MPC) [Eqs. 3.85-3.87]"""
-    _,__,C,___ = system
-    modes_raw = C@v
-    _, n = modes_raw.shape
-    sxx, syy, sxy = np.zeros((3, *modes_raw.shape))
-    nu, mpc = np.zeros((2, n))
-    lam = np.zeros((2, n))
-    for i in range(n):
-        sxx[:,i] = np.real(modes_raw[:,i]).T@np.real(modes_raw[:,i])
-        syy[:,i] = np.imag(modes_raw[:,i]).T@np.imag(modes_raw[:,i])
-        sxy[:,i] = np.real(modes_raw[:,i]).T@np.imag(modes_raw[:,i])
-        nu[i]    = (syy[:,i]-sxx[:,i])/(2*sxy[:,i])
-        lam[1,i] = (sxx[:,i]+syy[:,i])/2 + sxy[:,i]*np.sqrt(nu[i]**2+1);
-        lam[2,i] = (sxx[:,i]+syy[:,i])/2 - sxy[:,i]*np.sqrt(nu[i]**2+1);
-        mpc[i]   = ((lam[0,i]-lam[1,i])/(lam[0,i]+lam[1,i]))**2;
-    return mpc
-
-def EMAC_Matrix(n, m, pto, ptop, debug=False):
-    emac = np.zeros((n, m))
-    for i in range(n):
-        for j in range(m):
-            Rij = min(
-                (abs(pto[j,i])/abs(ptop[j,i])),
-                (abs(ptop[j,i])/abs(pto[j,i]))
-            )
-            Pij = np.angle(pto[j,i]/ptop[j,i])
-            Wij = max(
-                1 - abs(Pij)/(pi/4),
-                0
-            )
-            emac[i,j] = Rij*Wij
-    return emac
-
-def EMAC_Variation(n,m,pto,ptop):
-    pass
-
-
-def EnergyCondensedEMAC(n,m,emac,phi,debug=False):
-    "Equation 3.93"
-    return np.array([
-        sum(emac[i,j]*abs(phi[i,j])**2 
-            for j in range(m)
-        )/np.real(phi[i,:].conjugate().transpose()@phi[i,:])
-        for i in range(n) 
-    ])
-
-def MAC(shape,v, v_inv, A, B):
-    n,m,r,l = shape
-    lamb = v_inv@A@v
-    bkh = v_inv@B
-    for i in range(n):
-        for j in range(l):
-            qhat[i,j*r+1:j*r+r] = bkh[i,:]*(lamb[i,i])**j
-
-    selsiz = min(size(qlin),size(qhat))
-
-    for hnd in range(n):
-        ql = qlin[hnd,:selsiz(2)]
-        qh = qhat[hnd,:selsiz(2)]
-        mac[hnd] = abs(ql*qh.T)/(abs(ql*ql.T)*abs(qh*qh.T))**0.5
-
-
-def EMAC_Validate(shape, kmax, v, d, dt, system):
-    "b) Exted Modal Amplitude Coherence (EMAC)"
-    A,B,C,D = system
-    n,m,r,l = shape
-
-def OutputEMAC(n,m,kmax,A,C,Observability, debug=False,d=None,v=None, **_):
-    """Output EMAC (Eqs. 3.88-3.89)"""
-    if d is None:
-        assert v is None
-        from .ExtractModes import condeig 
-        v, d, _ = condeig(A)
-    pto = Observability[-m:,:]@v # the identified value at T0 ( last block row)
-    ptop = C@v@np.diag(d**(kmax-1))
-    emaco  = EMAC_Matrix(n,m,pto,ptop)
-    if debug:
-        return locals()
-    return EnergyCondensedEMAC(n, m, emaco, (C@v).T)
-
-
-def InputEMAC(Ctrl,A,B):
-    #
-    # Input EMAC
-    #
-    # # EMAC Input Variation
-    # for i in range(l):
-    #     qtovar = qlin[:,i*r:(i+1)*r]
-    #     qtopvar = (np.diag(d)**i)*inm
-    #     emaci = EMAC_Matrix(n,m,qtovar,qtopvar)
-    #     emacivar[:,i] = EnergyCondensedEMAC(n,m,emaci,inm);
-
-    # Pick the last block column
-    v, d  = A.eigen()
-    v_inv = np.linalg.inv(v)
-    inm   = linsolve(v,B)   # Initial mode contribution
-    qlin  = v_inv@Ctrl;     # Modal controllability Matrix (F' in Pappa 1993)
-    qto   = qlin[:, (l-1)*r+1:l*r]
-    qtop  = d**(l-1)@inm
-    emaci = EMAC_Matrix(n, m, qto, qtop)
-    return EnergyCondensedEMAC(n, m, emaci, inm)
-    
-
-
-if __name__ == "__main__":
-    from pathlib import Path
-    import quakeio
-    # import ssid as si
-    import okid
-    import numpy as np
-    channels = dict( # PAINTER RIO DELL
-        inputs  = [17, 3, 20],
-        outputs = [ 9, 7 , 4]
-    )
-    channels = dict( # HAYWARD
-        inputs  = [17, 18, 24, 25],
-        outputs = [19, 20 , 22, 23]
-    )
-    for file in Path("hwd_recs").glob("RioDell_P*.zip"):
-        event = quakeio.read(file)
-        try:
-            inputs = [
-                event.match("r", file_name=f".*{chan}.*").accel
-                for chan in channels["inputs"]
-            ]
-            outpts = [
-                event.match("r", file_name=f".*{chan}.*").accel
-                for chan in channels["outputs"]
-            ]
-        except:
-            print(f"failed {file.name}")    
-    for file in Path("painter").glob("RioDell_P*.zip"):
-        event = quakeio.read(file)
-        try:
-            inputs = [
-                event.match("r", file_name=f".*{chan}.*").accel
-                for chan in channels["inputs"]
-            ]
-            outpts = [
-                event.match("r", file_name=f".*{chan}.*").accel
-                for chan in channels["outputs"]
-            ]
-        except:
-            print(f"failed {file.name}")
-
-        else:
-            dt = inputs[0]["time_step"]
-            V = OKID.okid(inputs, outpts, dt=dt, kmax=500, mro=10, orm=4, verbose=True)
-            break
-
-            A,B,C,D = OKID.okid(inputs, outpts, dt=dt, kmax=500, mro=10, orm=4, verbose=True)
-            freqdmpSRIM, modeshapeSRIM, *_ = si.ComposeModes(dt, A, B, C, D)
-            # Add validation
-            print(si.IdentifiedSystem(dt, A, B, C, D))
-            # print(file, np.real(1/freqdmpSRIM[:,0]))
+import numpy as np
+from numpy import zeros, pi, size
+import scipy.linalg
+from scipy.linalg import fractional_matrix_power as matpow
+
+linsolve = scipy.linalg.solve
+
+lsqminnorm = lambda *args: np.linalg.lstsq(*args, rcond=None)[0]
+
+def parse_okid(args, config):
+    """
+    p determines order of the observer Kalman ARX filter used in OKID-ERA-DC.
+    n determines size of the state-space model used for representing the system.
+    """
+    return config
+
+# y = output data: forced response. dimensions of y: p x nt, where nt = number of timesteps
+# u = input data: input. dimensions of u: q x nt.
+# m = number of Markov parameters (impulse response timesteps) to solve for
+def get_impulse(y, u):
+    p = y.shape[0]
+    q = u.shape[0]
+    nt = y.shape[1]
+    assert y.shape[1] == u.shape[1]
+    # form a blockwise upper triangular matrix of inputs
+    U = np.zeros((q*nt, nt))
+    for i in range(nt):
+        for j in range(nt-i):
+            U[q*j:q*(j+1),i] = u[:,i]
+    Y_impulse = y @ np.linalg.pinv(U)
+    assert Y_impulse.shape == (p, q*nt)
+    return Y_impulse
+
+def okid2(y, u, m):
+    p = y.shape[0]
+    q = u.shape[0]
+    nt = y.shape[1]
+    assert y.shape[1] == u.shape[1]
+    # form a blockwise upper triangular matrix of inputs
+    U = np.zeros((q*nt, nt))
+    for i in range(nt):
+        for j in range(nt-i):
+            U[q*j:q*(j+1),i] = u[:,i]
+    Y_impulse = y @ np.linalg.pinv(U)
+    assert Y_impulse.shape == (p, q*nt)
+    return Y_impulse
+
+def OKID_brunton(y,u,m):
+    
+    p = y.shape[0]
+    q = u.shape[0]
+    nt = y.shape[1]
+    assert y.shape[1] == u.shape[1]
+    
+    # Form data matrices y and V
+    V = np.zeros((q+(q+p)*m,nt))
+    for i in range(nt):
+        V[:q,i] = u[:q,i]
+        
+    for i in range(1,m+1):
+        for j in range(nt-i):
+            vtemp = np.concatenate((u[:,j],y[:,j]))
+            V[q+(i-1)*(q+p):q+i*(q+p),i+j] = vtemp
+    
+    # Solve for observer Markov parameters Ybar
+    Ybar = y @ np.linalg.pinv(V,rcond=10**(-3))
+    
+    # Isolate system Markov parameters H, and observer gain M
+    D = Ybar[:,:q] # feed-through term (or D matrix) is the first term
+    
+    Y = np.zeros((p,q,m))
+    Ybar1 = np.zeros((p,q,m))
+    Ybar2 = np.zeros((p,q,m))
+    
+    for i in range(m):
+        Ybar1[:,:,i] = Ybar[:,q+(q+p)*i : q+(q+p)*i+q]
+        Ybar2[:,:,i] = Ybar[:,q+(q+p)*i+q : q+(q+p)*(i+1)]
+    
+    Y[:,:,0] = Ybar1[:,:,0] + Ybar2[:,:,0] @ D
+    for k in range(1,m):
+        Y[:,:,k] = Ybar1[:,:,k] + Ybar2[:,:,k] @ D
+        for i in range(k-1):
+            Y[:,:,k] += Ybar2[:,:,i] @ Y[:,:,k-i-1]
+            
+    H = np.zeros((D.shape[0],D.shape[1],m+1))
+    H[:,:,0] = D
+    
+    for k in range(1,m+1):
+        H[:,:,k] = Y[:,:,k-1]
+        
+    return H
+
+# Y = output data: response to unit impulse, or "impulse response," or "Markov parameters".
+# dimensions of Y: p x q x nt, where nt = number of timesteps = number of Markov parameters = number of blocks
+# mc = number of block rows in Hankel matrix = order of controllability matrix
+# mo = number of block columns in Hankel matrix = order of observability matrix
+# p = number of outputs
+# q = number of inputs
+# r = reduced model order = dimension of reduced A = newly assumed dimension of state variable
+def era(Y,mo,mc,p,q,r):
+    # get D from first p x q block of impulse response
+    Dr = Y[:,:,0]  # first block of output data
+    
+    assert Y.shape[:2] == (p,q)  # sanity check that we're passing in the right output data
+    assert Y.shape[2] >= mo+mc   # make sure there are enough timesteps to assemble this size of Hankel matrix
+    
+    # make impulse response into Hankel matrix and shifted Hankel matrix
+    H = np.zeros((p*(mo), q*(mc+1)))
+    for i in range(mo):
+        for j in range(mc+1):
+            H[p*i:p*(i+1), q*j:q*(j+1)] = Y[:,:,i+j+1]
+    H0 = H[:,:-q]
+    H1 = H[:,q:]
+    assert H0.shape == H1.shape == (p*(mo), q*(mc))
+
+    # reduced SVD of Hankel matrix
+    def _svd(*args):
+        U,S,V = scipy.linalg.svd(*args, lapack_driver="gesvd")
+        return U,S,V.T.conj()
+    U,S,V = _svd(H0)
+    SigmaInvSqrt = np.diag(S[:r]**-0.5)
+    SigmaSqrt = np.diag(S[:r]**0.5)
+    Ur = U[:,:r]
+    Vr = V[:,:r]
+
+    # get A from SVD and shifted Hankel matrix
+    Ar = SigmaInvSqrt @ Ur.T.conj() @ H1 @ Vr @ SigmaInvSqrt
+
+    # get B and C
+    Br = (SigmaSqrt @ Vr.T.conj())[:,:q]
+    Cr = (Ur @ SigmaSqrt)[:p,:]
+
+    return (Ar,Br,Cr,Dr,S)
+
+# l = initial lag for data correlations
+# g = lags between correlation matrices
+# a = number of block rows in Hankel of correlation matrix
+# b = number of block columns in Hankel of correlation matrix
+def era_dc(Y,mo,mc,p,q,r,l,g,a,b):
+    # get D from first p x q block of impulse response
+    Dr = Y[:,:,0]  # first block of output data
+    
+    assert Y.shape[:2] == (p,q)  # sanity check that we're passing in the right output data
+    assert Y.shape[2] >= l+(a+1+b+1)*g+mo+mc   # make sure there are enough timesteps to assemble the Hankel matrices
+    
+    # make impulse response into Hankel matrix
+    H = np.zeros((p*(mo), q*(mc+l+(a+1+b+1)*g))) # Hankel of Markov parameters
+    for i in range(mo):
+        for j in range(mc+l+(a+1+b+1)*g):
+            H[p*i:p*(i+1), q*j:q*(j+1)] = Y[:,:,i+j+1]
+    H0 = H[:,:q*mc]
+    assert H0.shape == (p*(mo), q*(mc))
+
+    dimR = p*mo # Dimension of square correlation matrices
+    dimHRl = (dimR*(a+1), dimR*(b+1)) # Dimension of Hankels of correlation matrices
+    HRl = np.zeros(dimHRl) # Hankel of correlation matrices
+    HRl1 = np.zeros(dimHRl) # Shifted Hankel of correlation matrices
+    for i in range(a+1):
+        for j in range(b+1):
+            Hl = H[:, q*(l+1+(i+j)*g):q*(l+1+(i+j)*g+mc)]
+            Hl1 = H[:, q*(l+1+(i+j)*g+1):q*(l+1+(i+j)*g+mc+1)]
+            assert Hl.shape == Hl1.shape == (p*(mo), q*(mc))
+            R = Hl@H0
+            R1 = Hl1@H0
+            assert R.shape == R1.shape == (dimR,dimR)
+            HRl[dimR*i:dimR*(i+1), dimR*j:dimR*(j+1)] = R
+            HRl1[dimR*i:dimR*(i+1), dimR*j:dimR*(j+1)] = R1
+
+    # reduced SVD of Hankel matrix
+    def _svd(*args):
+        U,S,V = scipy.linalg.svd(*args, lapack_driver="gesvd")
+        return U,S,V.T.conj()
+    U,S,V = _svd(HRl)
+    SigmaInvSqrt = np.diag(S[:r]**-0.5)
+    SigmaSqrt = np.diag(S[:r]**0.5)
+    Ur = U[:,:r]
+    Vr = V[:,:r]
+
+    # get A from SVD and shifted Hankel matrix
+    Ar = SigmaInvSqrt @ Ur.T.conj() @ HRl1 @ Vr @ SigmaInvSqrt
+
+    # get B and C
+    Br = ((SigmaInvSqrt @ Ur.T.conj())[:,:dimR] @ H0)[:,:q]
+    Cr = (Ur @ SigmaSqrt)[:p,:]
+
+    return (Ar,Br,Cr,Dr,S)
+
+
+def _era_ya(kmax, m, l, r, Y, n, svd="gesvd"):
+    # ERA/DC
+    #
+    # Form Hankel matrix (H) from the Markov parameters (Y) (Eq. 3.80)
+
+    # Obtain Hankel Matrix of Zeroth Order & First Order
+    H0,H1 = np.zeros((2, kmax*m, l*r))
+    #H0 = hankel(Y,0)
+    for hj in range(kmax):
+        for jh in range(l):
+            H0[hj*m:hj*m+m, jh*r:jh*r+r] = Y[jh+hj+1]
+            H1[hj*m:hj*m+m, jh*r:jh*r+r] = Y[jh+hj+2]
+    
+    if svd in ["gesvd", "gesdd"]:
+        import scipy.linalg
+        def _svd(*args):
+            U,S,V = scipy.linalg.svd(*args, lapack_driver=svd)
+            return U,S,V.T.conj()
+
+    ## 2c. Use H matrix to compute system matrices A, B & C
+    R1,sis,S1 = _svd(H0) # singular value decomposition
+    Sis = np.diag(sis[:n])
+
+    Siv = np.diag(1/np.sqrt(sis[:n]))
+    # A: state transition matrix (Eqs. 3.32 & 3.82)
+    A  = Siv@R1[:,:n].T@H1@S1[:,:n]@Siv
+    # B: input influence matrix (Eqs. 3.32 & 3.83)
+    B = (np.sqrt(Sis)@S1[:,:n].T)[:,:r]
+    Observability = R1[:,:n]@np.sqrt(Sis)
+    # C: output influence matrix (Eqs. 3.34 & 3.84)
+    C  = Observability[:m,:]
+
+    return A,B,C
+
+
+def okid(dati, dato, svd="gesvd", debug=False, **config):
+    """
+    PART 2: OKID-ERA-DC (Observer Kalman filter Identification -
+            Eigen Realization with Direct Correlations)
+    -----------------------------------------------------------------
+
+    # Inputs
+    Modelparameters
+        div = 1;     # A parameter used for decimating data. 1 uses entire data without downsampling.
+        mro = 10;    # Model reduction order
+        orm = 4;     # Order of the model. # of computed and plotted modes dep on orm.
+                     # For orm = 2, one mode is found, for orm = 4, two modes are found.
+    svd:
+        GESDD: a two-stage algorithm. It first reduces the input matrix to bidiagonal form via 
+        Householder reflection, then divides the bidiagonal matrix into smaller matrices to calculate 
+        singular values and the unitary matrices U and V. Finally, the singular values of the entire 
+        input matrix is simply the those of the smaller sub-matrices.
+        
+        GESVD: also a two-stage algorithm where the first step is identical to GESDD. The second step 
+        can be done using iterative QR decomposition to derive singular values. More mathematical details are available here.
+
+    Sometimes higher orm still gives fewer modes, e.g. orm = 8 for case 1 gives
+    three modes, but one of them is invalid according to the EMAC & MPC criteria.
+    kmax = 100;  #Number of computed Markov parameters, indicated as 1000 on page 43 of
+    (Arici & Mosalam, 2006). However, it was input as 100 in the code.
+    kmax = 100 runs much faster & both kmax = 100 & 1000 give the same results.
+
+    # Outputs
+    1. freqdamp variable is a matrix that includes the information of identified
+       frequencies, damping ratios & validation of the modes with MPC & EMAC criteria
+       Each row of freqdamp corresponds to a mode. Columns are as follows:
+       1) frequency, 2) damping ratio, 3) order index, 4) condition number, 5) input EMAC,
+       6) output EMAC, 7) MPC. If values in columns 5-7 are > 0.5, identified mode is valid.
+    2. modeshape stores the mode shape information for identified modes.
+    3. RMSEpred: root mean square error of the predicted output from
+       identified parameters with respect to the actual output.
+    4. Markovparamerror: root mean square error used to validate accurate
+       computation of Markov parameters
+
+    # Description of the Methodology
+    More information on OKID-ERA-DC method can be found in
+    Section 3.4.6 of (Arici & Mosalam, 2006). Equations below refer to this report.
+    OKID-ERA-DC is a Multiple Input - Multiple Output (MIMO) System Identification (SI) method
+    that consists of the following steps:
+    1. Data pre-processing (baseline correction, filtering & decimation)
+    2. Identify observer Kalman filters using Observer Kalman filter Identification (OKID)
+       methodology. This step basically consists of developing a simple observer model of
+       a system from a MIMO ARX structure, Eq. (3.76), which is broken into these 6 steps:
+   
+    3a. Determine Markov parameters (M) in a least squares sense, Eq. (3.76).
+
+    3b. Establish the Hankel matrix (H) from the Markov parameters, (Eq. 3.80).
+    3c. Use H to compute system matrices A, B & C, in which modal information is embedded.
+    // 3d. Obtain the modal information from matrices A, B & C.
+    3e. Spatial & temporal validation of the identified modes.
+    3f. Back calculate (estimate) the output accelerations with the state-space system &
+        check against the actual output accelerations.
+    """ 
+    dt = to = config.get("dt", None) or dati["time_step"]
+    p = config.get("p", config.get("mro")) # # steps used for the identification (ie, prediction horizon)
+    n = n1 = config.get("n", config.get("orm", 4))  # Order of the model.
+    
+    if svd in ["gesvd", "gesdd"]:
+        import scipy.linalg
+        def _svd(*args):
+            U,S,V = scipy.linalg.svd(*args, lapack_driver=svd)
+            return U,S,V.T.conj()
+
+    elif svd in ["xla", "jax"]:
+        from jax.scipy.linalg import svd as _svd
+
+    if isinstance(dati, list):
+        dati = np.array([i.data for i in dati]).T
+    elif issubclass(dati.__class__, dict):
+        dati = dati.data
+
+    if isinstance(dato, list):
+        dato = np.array([i.data for i in dato]).T
+    elif issubclass(dato.__class__, dict):
+        dato = dato.data
+
+    if len(dati.shape) < 2:
+        dati = np.atleast_2d(dati).T
+    if len(dato.shape) < 2:
+        dato = np.atleast_2d(dato).T
+        
+    dati = dati[:-1,:]
+    dato = dato[:-1,:]
+
+    #verbose = True
+    #dn = config.get("dn", None) or dati.shape[0]
+    kmax    = config["kmax"]
+    n = config["orm"]   # assign order of model input to variable n, consistent with Eqs. 3.81-3.84
+    p = config["mro"]   # assign input model reduction order to variable p, consistent with Eq. 3.76
+
+
+    l,m = dato.shape # m is the number of output channels
+    _,r = dati.shape # r is the number of input channels
+
+    # ASSERT SIZE(DATO,1) == SIZE(DATI,1)
+
+    ## 2a. Obtain Observer Markov Parameters
+    # The Markov parameters are computed in two steps:
+    # i)  The Observer Markov matrices are computed from Eq. 3.76 using a linear regression approach
+    # ii) Compute the system Markov parameters from the Markov matrices using recursive relations
+
+    # Compute matrix U that represents ARX equation of current output on p time steps of past output
+    # & input values (Eq. 3.76)
+    U = np.zeros(((m+r)*p+r, l))
+    U[:r,:] = dati.T
+    for b in range(1,p+1):
+        U[(b-1)*(r+m)+r:(b-1)*(r+m)+r+r+m, b:] = [*dati[:-b,:r].T, *dato[:-b, :m].T]
+
+
+    # i) Compute the matrix of Observer Markov Parameter Matrix (M)
+    #    in Eq 3.76 using Linear Regression
+    uu,wr,V = _svd(U,0)
+    pg = (r+m)*p+r
+    for i in range((r+m)*p+r):
+        if wr[i] <= 0.001:
+            pg = i
+            break
+
+    s = np.diag(wr)
+
+    pss = V[:,:pg]@linsolve(s[:pg,:pg], uu[:,:pg].T)
+    M = dato.T@pss           # M: Observer Markov Parameter Matrix
+
+    # Fit for multiple regression
+    # RMSE between actual output & y on left hand side in Eq. 3.76. It should be 
+    # quite small (e.g., 10^-3) for accurately computed Markow parameters.
+    # ypreo = M@U
+    # markovParamError = 1/m*sum((
+    #     sum((dato[:,i] - ypreo[i,:].T)**2)/sum(dato[:,i]**2)
+    #     for i in range(m)
+    # ))  
+
+
+    ## ii) Compute Markov parameters (Y) using recursive relations in Eqs. 3.78 & 3.79
+    #      (Equation 6.21 in Juang 1994)
+
+    # Matrix D is directly equal to the Observer Markov parameter matrix (Eq. 3.77)
+    D = M[:, :r]  # D: Direct Transmission term
+
+    Y = [D]
+    # First p steps (Eq. 3.78)
+    for i in range(p):
+        Y.append(
+            M[:, r+i*(r+m):r+i*(r+m)+r] + sum(
+                M[:, r+j*(r+m)+r:r+j*(r+m)+r+m]@Y[i-j]
+                for j in range(i+1)
+            )
+        )
+    # Remainder (Eq. 3.79)
+    for i in range(p, l+kmax):
+        sumt = zeros((m,r))
+        for j in range(p):
+            sumt += M[:,r+j*(r+m)+r:r+j*(r+m)+r+m]@Y[i-j]
+
+        Y.append(sumt)
+
+    # The Markow parameters Y have been computed.
+
+    A,B,C = _era_ya(kmax, m, l, r, Y, _svd, n)
+
+    if debug:
+        return locals()
+
+    return A,B,C,D
+
+
+def validate(freqdmp, v, system, **config):
+    """2e. Validation Analysis
+
+    Two criteria are used for selection of identified genuine modes
+    (in the sense of spatial & temporal consistency).
+
+    a) Modal Phase Collinearity (MPC) testing spatial consistency of identification results.
+       Modes having MPC value above 0.5 (mpc parameter below) are considered as genuine modal quantities.
+
+    b) Exted Modal Amplitude Coherence (EMAC), evaluates temporal consistency of the identification results.
+       Both output EMAC & input EMAC can be computed. Input EMAC requires the controllability matrix.
+       Because the controllability matrix is not estimated by all considered SI methods,
+       this criterion is computed, but not used.
+       Modes with output EMAC values < 0.5 are considered spurious & therefore not reported.
+
+    """
+    mpc = MPC(n, v, system)
+
+    # Add the input EMAC, output EMAC, and MPC to the matrix freqdamp
+    for lih in range(size(freqdmp)[0]):
+        freqdmp[lih,4] = emacif(freqdmp[lih,2])
+        freqdmp[lih,5] = emacof(freqdmp[lih,2])
+        freqdmp[lih,6] = mpc[freqdmp(lih,3)]
+        if freqdmp[lih,5]>0.5 and freqdmp[lih,7]>0.5:
+            # valid
+            return True
+        else:
+            # not valid
+            return False
+
+def MPC(n, v, system):
+    """a) Modal Phase Collinearity (MPC) [Eqs. 3.85-3.87]"""
+    _,__,C,___ = system
+    modes_raw = C@v
+    _, n = modes_raw.shape
+    sxx, syy, sxy = np.zeros((3, *modes_raw.shape))
+    nu, mpc = np.zeros((2, n))
+    lam = np.zeros((2, n))
+    for i in range(n):
+        sxx[:,i] = np.real(modes_raw[:,i]).T@np.real(modes_raw[:,i])
+        syy[:,i] = np.imag(modes_raw[:,i]).T@np.imag(modes_raw[:,i])
+        sxy[:,i] = np.real(modes_raw[:,i]).T@np.imag(modes_raw[:,i])
+        nu[i]    = (syy[:,i]-sxx[:,i])/(2*sxy[:,i])
+        lam[1,i] = (sxx[:,i]+syy[:,i])/2 + sxy[:,i]*np.sqrt(nu[i]**2+1);
+        lam[2,i] = (sxx[:,i]+syy[:,i])/2 - sxy[:,i]*np.sqrt(nu[i]**2+1);
+        mpc[i]   = ((lam[0,i]-lam[1,i])/(lam[0,i]+lam[1,i]))**2;
+    return mpc
+
+def EMAC_Matrix(n, m, pto, ptop, debug=False):
+    emac = np.zeros((n, m))
+    for i in range(n):
+        for j in range(m):
+            Rij = min(
+                (abs(pto[j,i])/abs(ptop[j,i])),
+                (abs(ptop[j,i])/abs(pto[j,i]))
+            )
+            Pij = np.angle(pto[j,i]/ptop[j,i])
+            Wij = max(
+                1 - abs(Pij)/(pi/4),
+                0
+            )
+            emac[i,j] = Rij*Wij
+    return emac
+
+def EMAC_Variation(n,m,pto,ptop):
+    pass
+
+
+def EnergyCondensedEMAC(n,m,emac,phi,debug=False):
+    "Equation 3.93"
+    return np.array([
+        sum(emac[i,j]*abs(phi[i,j])**2 
+            for j in range(m)
+        )/np.real(phi[i,:].conjugate().transpose()@phi[i,:])
+        for i in range(n) 
+    ])
+
+def MAC(shape,v, v_inv, A, B):
+    n,m,r,l = shape
+    lamb = v_inv@A@v
+    bkh = v_inv@B
+    for i in range(n):
+        for j in range(l):
+            qhat[i,j*r+1:j*r+r] = bkh[i,:]*(lamb[i,i])**j
+
+    selsiz = min(size(qlin),size(qhat))
+
+    for hnd in range(n):
+        ql = qlin[hnd,:selsiz(2)]
+        qh = qhat[hnd,:selsiz(2)]
+        mac[hnd] = abs(ql*qh.T)/(abs(ql*ql.T)*abs(qh*qh.T))**0.5
+
+
+def EMAC_Validate(shape, kmax, v, d, dt, system):
+    "b) Exted Modal Amplitude Coherence (EMAC)"
+    A,B,C,D = system
+    n,m,r,l = shape
+
+def OutputEMAC(n,m,kmax,A,C,Observability, debug=False,d=None,v=None, **_):
+    """Output EMAC (Eqs. 3.88-3.89)"""
+    if d is None:
+        assert v is None
+        from .ExtractModes import condeig 
+        v, d, _ = condeig(A)
+    pto = Observability[-m:,:]@v # the identified value at T0 ( last block row)
+    ptop = C@v@np.diag(d**(kmax-1))
+    emaco  = EMAC_Matrix(n,m,pto,ptop)
+    if debug:
+        return locals()
+    return EnergyCondensedEMAC(n, m, emaco, (C@v).T)
+
+
+def InputEMAC(Ctrl,A,B):
+    #
+    # Input EMAC
+    #
+    # # EMAC Input Variation
+    # for i in range(l):
+    #     qtovar = qlin[:,i*r:(i+1)*r]
+    #     qtopvar = (np.diag(d)**i)*inm
+    #     emaci = EMAC_Matrix(n,m,qtovar,qtopvar)
+    #     emacivar[:,i] = EnergyCondensedEMAC(n,m,emaci,inm);
+
+    # Pick the last block column
+    v, d  = A.eigen()
+    v_inv = np.linalg.inv(v)
+    inm   = linsolve(v,B)   # Initial mode contribution
+    qlin  = v_inv@Ctrl;     # Modal controllability Matrix (F' in Pappa 1993)
+    qto   = qlin[:, (l-1)*r+1:l*r]
+    qtop  = d**(l-1)@inm
+    emaci = EMAC_Matrix(n, m, qto, qtop)
+    return EnergyCondensedEMAC(n, m, emaci, inm)
+    
+
+
+if __name__ == "__main__":
+    from pathlib import Path
+    import quakeio
+    # import ssid as si
+    import okid
+    import numpy as np
+    channels = dict( # PAINTER RIO DELL
+        inputs  = [17, 3, 20],
+        outputs = [ 9, 7 , 4]
+    )
+    channels = dict( # HAYWARD
+        inputs  = [17, 18, 24, 25],
+        outputs = [19, 20 , 22, 23]
+    )
+    for file in Path("hwd_recs").glob("RioDell_P*.zip"):
+        event = quakeio.read(file)
+        try:
+            inputs = [
+                event.match("r", file_name=f".*{chan}.*").accel
+                for chan in channels["inputs"]
+            ]
+            outpts = [
+                event.match("r", file_name=f".*{chan}.*").accel
+                for chan in channels["outputs"]
+            ]
+        except:
+            print(f"failed {file.name}")    
+    for file in Path("painter").glob("RioDell_P*.zip"):
+        event = quakeio.read(file)
+        try:
+            inputs = [
+                event.match("r", file_name=f".*{chan}.*").accel
+                for chan in channels["inputs"]
+            ]
+            outpts = [
+                event.match("r", file_name=f".*{chan}.*").accel
+                for chan in channels["outputs"]
+            ]
+        except:
+            print(f"failed {file.name}")
+
+        else:
+            dt = inputs[0]["time_step"]
+            V = OKID.okid(inputs, outpts, dt=dt, kmax=500, mro=10, orm=4, verbose=True)
+            break
+
+            A,B,C,D = OKID.okid(inputs, outpts, dt=dt, kmax=500, mro=10, orm=4, verbose=True)
+            freqdmpSRIM, modeshapeSRIM, *_ = si.ComposeModes(dt, A, B, C, D)
+            # Add validation
+            print(si.IdentifiedSystem(dt, A, B, C, D))
+            # print(file, np.real(1/freqdmpSRIM[:,0]))
```

### Comparing `ssid-0.0.4/src/ssid/realize.py` & `ssid-0.0.5/src/ssid/realize.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,303 +1,304 @@
-import numpy as np
-import scipy
-linsolve = np.linalg.solve
-lsqminnorm = lambda *args: np.linalg.lstsq(*args, rcond=None)[0]
-import multiprocessing
-from functools import partial
-import warnings
-try:
-    from tqdm import tqdm as progress_bar
-
-except:
-    def progress_bar(arg, **kwds): return arg 
-
-## ERA ##
-# Y = output data: response to unit impulse, or "impulse response," or "Markov parameters".
-# dimensions of Y: p x q x nt, where nt = number of timesteps = number of Markov parameters = number of blocks
-# no = number of block rows in Hankel matrix = order of observability matrix
-# nc = number of block columns in Hankel matrix = order of controllability matrix
-# r = reduced model order = dimension of reduced A = newly assumed dimension of state variable
-def era(Y,no=None,nc=None,r=None,**options):
-    p,q,nt = Y.shape # p = number of outputs, q = number of inputs, nt = number of timesteps
-    if r is None:
-        r = min(20, int(nt/2))
-    
-    # get D from first p x q block of impulse response
-    Dr = Y[:,:,0]  # first block of output data
-    
-    # size of Hankel matrix
-    if no is None:
-        if nc is None:
-            no = nc = min(300, int((nt-1)/2))
-        else:
-            no = min(300, int(nt-1-nc))
-    elif nc is None:
-        nc = min(300, int(nt-1-no))
-    else:
-        # make sure there are enough timesteps to assemble this size of Hankel matrix
-        assert nt >= no+nc
-    
-    # make impulse response into Hankel matrix and shifted Hankel matrix
-    H = np.zeros((p*(no), q*(nc+1)))
-    for i in range(no):
-        for j in range(nc+1):
-            H[p*i:p*(i+1), q*j:q*(j+1)] = Y[:,:,i+j+1]
-    H0 = H[:,:-q]
-    H1 = H[:,q:]
-    assert H0.shape == H1.shape == (p*(no), q*(nc))
-
-    # reduced SVD of Hankel matrix
-    def _svd(*args):
-        U,S,V = scipy.linalg.svd(*args, lapack_driver="gesvd")
-        return U,S,V.T.conj()
-    U,S,V = _svd(H0)
-    SigmaInvSqrt = np.diag(S[:r]**-0.5)
-    SigmaSqrt = np.diag(S[:r]**0.5)
-    Ur = U[:,:r]
-    Vr = V[:,:r]
-
-    # get A from SVD and shifted Hankel matrix
-    Ar = SigmaInvSqrt @ Ur.T.conj() @ H1 @ Vr @ SigmaInvSqrt
-
-    # get B and C
-    Br = (SigmaSqrt @ Vr.T.conj())[:,:q]
-    Cr = (Ur @ SigmaSqrt)[:p,:]
-
-    return (Ar,Br,Cr,Dr)
-
-## ERA-DC ##
-# a = (alpha) number of block rows in Hankel of correlation matrix
-# b = (beta) number of block columns in Hankel of correlation matrix
-# l = initial lag for data correlations
-# g = lags (gap) between correlation matrices
-def era_dc(Y,no=None,nc=None,a=0,b=0,l=0,g=1,r=None,**options):
-    p,q,nt = Y.shape # p = number of outputs, q = number of inputs, nt = number of timesteps
-    if r is None:
-        r = int(nt/2)
-
-    # get D from first p x q block of impulse response
-    Dr = Y[:,:,0]  # first block of output data
-
-    # size of Hankel matrix
-    if no is None:
-        if nc is None:
-            no = nc = min(300, int(nt/2-1))
-        else:
-            no = min(300, int(nt/2-1))
-    elif nc is None:
-        nc = min(300, int(nt-no-2))
-    # make sure there are enough timesteps to assemble the Hankel matrices
-    assert nt >= l+(a+1+b+1)*g+no+nc
-
-    # Hankel matrix of impulse response (Markov parameters)
-    H = np.zeros((p*(no), q*(nc+l+(a+1+b+1)*g)))
-    for i in range(no):
-        for j in range(nc+l+(a+1+b+1)*g):
-            H[p*i:p*(i+1), q*j:q*(j+1)] = Y[:,:,i+j+1]
-    H0 = H[:,:q*nc]
-    assert H0.shape == (p*(no), q*(nc))
-
-    dimR = p*no # Dimension of square correlation matrices
-    dimHRl = (dimR*(a+1), dimR*(b+1)) # Dimension of Hankel matrix of correlation matrices
-    HRl = np.zeros(dimHRl) # Hankel matrix of correlation matrices
-    HRl1 = np.zeros(dimHRl) # Shifted Hankel matrix of correlation matrices
-    for i in range(a+1):
-        for j in range(b+1):
-            Hl = H[:, q*(l+1+(i+j)*g):q*(l+1+(i+j)*g+nc)]
-            Hl1 = H[:, q*(l+1+(i+j)*g+1):q*(l+1+(i+j)*g+nc+1)]
-            assert Hl.shape == Hl1.shape == (p*(no), q*(nc))
-            R = Hl@H0       # correlation matrix
-            R1 = Hl1@H0     # shifted correlation matrix
-            assert R.shape == R1.shape == (dimR,dimR)
-            HRl[dimR*i:dimR*(i+1), dimR*j:dimR*(j+1)] = R
-            HRl1[dimR*i:dimR*(i+1), dimR*j:dimR*(j+1)] = R1
-
-    # reduced SVD of Hankel matrix of correlation matrices
-    def _svd(*args):
-        U,S,V = scipy.linalg.svd(*args, lapack_driver="gesvd")
-        return U,S,V.T.conj()
-    U,S,V = _svd(HRl)
-    SigmaInvSqrt = np.diag(S[:r]**-0.5)
-    SigmaSqrt = np.diag(S[:r]**0.5)
-    Ur = U[:,:r]
-    Vr = V[:,:r]
-
-    # get A from SVD and shifted Hankel matrix of correlation matrices
-    Ar = SigmaInvSqrt @ Ur.T.conj() @ HRl1 @ Vr @ SigmaInvSqrt
-
-    # get B and C
-    Br = ((SigmaInvSqrt @ Ur.T.conj())[:,:dimR] @ H0)[:,:q]
-    Cr = (Ur @ SigmaSqrt)[:p,:]
-
-    return (Ar,Br,Cr,Dr)
-
-
-def _blk_3(i, CA, U):
-    return i, np.einsum('kil,klj->ij', CA[:i,:,:], U[-i:,:,:])
-
-
-## SRIM ##
-# inputs = input data. dimensions of inputs: q x nt, where nt = number of timesteps.
-# outputs = response data due to input data. dimensions of outputs: p x nt.
-# no = number of steps used for identification (prediction horizon),
-    # and the order of the observability matrix.
-    # analagous to order (number of autoregressors) of the observer Kalman
-    # ARX filter used in OKID-ERA-DC.
-# r = size of the state-space model used for representing the system.
-# Juang 1997, "System Realization Using Information Matrix," Journal of Guidance, Control, and Dynamics
-def srim(inputs,outputs,no=None,r=None,full=True,pool_size=6,**options):
-    if len(inputs.shape) == 1:
-        inputs = inputs[None,:]
-    if len(outputs.shape) == 1:
-        outputs = outputs[None,:]
-
-    if inputs.shape[0] > inputs.shape[1]:
-        warnings.warn("input data has more channels (dim 1) than timesteps (dim 2)")
-    if outputs.shape[0] > outputs.shape[1]:
-        warnings.warn("output data has more channels (dim 1) than timesteps (dim 2)")
-
-    q,nt = inputs.shape
-    p = outputs.shape[0]
-    assert nt == outputs.shape[1]
-
-    if no is None:
-        no = min(300, nt)
-
-    if r is None:
-        r = min(10, int(no/2))
-
-    # maximum possible number of columns in the Y and U data matrices
-    ns = nt-1-no+2
-
-    assert no >= r/p + 1    # make sure prediction horizon is large enough that
-                            # observability matrix is full rank (Juang Eq. 8)
-
-    Yno = np.zeros((p*no,ns))
-    Uno = np.zeros((q*no,ns))
-
-    # progress_bar = lambda arg, **kwds: (i for i in arg)
-
-    # Construct Y (output) & U (input) data matrices (Eqs. 3.58 & 3.60 Arici 2006)
-    for i in range(no):
-        Yno[i*p:(i+1)*p,:] = outputs[:,i:ns+i]
-        Uno[i*q:(i+1)*q,:] = inputs[:,i:ns+i]
-
-
-    # 2b. Compute the correlation terms and the coefficient matrix 
-    #     (Eqs. 3.68 & 3.69).
-
-    # Compute the correlation terms (Eq. 3.68)
-    Ryy = Yno@Yno.T/ns
-    Ruu = Uno@Uno.T/ns
-    Ruy = Uno@Yno.T/ns
-
-    assert Ryy.shape[0] == Ryy.shape[1] == no*p
-    assert Ruy.shape[0] == no*q
-    assert Ruy.shape[1] == no*p
-
-    # Compute the correlation matrix (Eq. 3.69)
-    Rhh = Ryy - Ruy.T@linsolve(Ruu,Ruy)
-
-    # 2c. Obtain observability matrix using full or partial decomposition 
-    #     (Eqs. 3.72 & 3.74).
-    if full:
-        # Full Decomposition Method
-        un,*_ = np.linalg.svd(Rhh,0)           # Eq. 3.74
-        Observability = un[:,:r]               # Eq. 3.72
-        A = lsqminnorm(Observability[:(no-1)*p,:], Observability[p:no*p,:])
-        C = Observability[:p,:]
-    else:
-        # Partial Decomposition Method
-        un,*_ = np.linalg.svd(Rhh[:,:(no-1)*p+1],0)
-        Observability = un[:,:r]
-        A = lsqminnorm(Observability[:(no-1)*p,:], Observability[p:no*p,:])
-        C = un[:p,:]
-
-    # Computation of system matrices B & D
-    # Output Error Minimization
-
-    # Setting up the Phi matrix
-    Phi  = np.zeros((p*ns, r+p*q+r*q))
-    CA_powers = np.zeros((ns, p, A.shape[1]))
-    CA_powers[0, :, :] = C
-    A_p = A
-    for pwr in range(1,ns):
-        CA_powers[pwr,:,:] =  C@A_p
-        A_p = A@A_p
-
-    # First block column of Phi
-    for df in range(ns):
-        Phi[df*p:(df+1)*p,:r] = CA_powers[df,:,:]
-
-    # Second block column of Phi
-    Ipp = np.eye(p)
-    for i in range(ns):
-        Phi[i*p:(i+1)*p, r:r+p*q] = np.kron(inputs[:,i],Ipp)
-
-    # Third block column of Phi
-    In1n1 = np.eye(r)
-    cc = r + p*q + 1
-    dd = r + p*q + r*q
-
-    krn = np.array([np.kron(inputs[:,i],In1n1) for i in range(ns)])
-
-    # Execute a loop in parallel that looks something like:
-    #    for i in  range(1,ns):
-    #        Phi[] = _blk_3(i, CA_Powers, np.flip(...))
-
-    with multiprocessing.Pool(pool_size) as pool:
-        for i,res in progress_bar(
-                pool.imap_unordered(
-                    partial(_blk_3, CA=CA_powers,U=np.flip(krn,0)),
-                    range(1,ns),
-                    200
-                ),
-                total = ns
-            ):
-            Phi[i*p:(i+1)*p,cc-1:dd] = res
-
-    y = outputs[:,:ns].flatten()
-
-    teta = lsqminnorm(Phi,y)
-
-    x0 = teta[:r]
-    dcol = teta[r:r+p*q]
-    bcol = teta[r+p*q:r+p*q+r*q]
-
-    D = np.zeros((p,q))
-    B = np.zeros((r,q))
-    for wq in range(q):
-        D[:,wq] = dcol[wq*p:(wq+1)*p]
-
-    for ww in range(q):
-        B[:,ww] = bcol[ww*r:(ww+1)*r]
-
-    assert A.shape[0] == A.shape[1] == r
-
-    return A,B,C,D
-
-def subspace(outputs,no=None,r=None,cov_driven=True,**options):
-    outputs = np.atleast_2d(outputs)
-    p,nt = outputs.shape
-    assert nt > p
-
-    if no == None:
-        no = min(300, int(nt/2))
-    if r == None:
-        r = min(10,no-1)
-    
-    if cov_driven:
-        Toep = np.zeros((p*no,p*no))
-        for i in range(2*no-1):
-            covs = np.zeros((p,p,no-1))
-            for k in range(no-1):
-                covs[:,:,k] = outputs[:,k+i]@outputs[k]
-            Ri = np.sum(covs,axis=3)/no
-            for j in range(i):
-                for l in range(j):
-                    Toep[j,-l-1] = Ri
-
-    else:
-        pass
-
-    return
+
+import numpy as np
+lin_solve = np.linalg.solve
+import multiprocessing
+from functools import partial
+import warnings
+try:
+    from tqdm import tqdm as progress_bar
+
+except:
+    def progress_bar(arg, **kwds): return arg
+
+from . import numerics
+
+## ERA ##
+# Y = output data: response to unit impulse, or "impulse response," or "Markov parameters".
+# dimensions of Y: p x q x nt, where nt = number of timesteps = number of Markov parameters = number of blocks
+# no = number of block rows in Hankel matrix = order of observability matrix
+# nc = number of block columns in Hankel matrix = order of controllability matrix
+# r = reduced model order = dimension of reduced A = newly assumed dimension of state variable
+def era(Y,no=None,nc=None,r=None,**options):
+    p,q,nt = Y.shape # p = number of outputs, q = number of inputs, nt = number of timesteps
+    if r is None:
+        r = min(20, int(nt/2))
+
+    # get D from first p x q block of impulse response
+    Dr = Y[:,:,0]  # first block of output data
+
+    # size of Hankel matrix
+    if no is None:
+        if nc is None:
+            no = nc = min(300, int((nt-1)/2))
+        else:
+            no = min(300, int(nt-1-nc))
+    elif nc is None:
+        nc = min(300, int(nt-1-no))
+    else:
+        # make sure there are enough timesteps to assemble this size of Hankel matrix
+        assert nt >= no+nc
+
+    # make impulse response into Hankel matrix and shifted Hankel matrix
+    H = np.zeros((p*(no), q*(nc+1)))
+    for i in range(no):
+        for j in range(nc+1):
+            H[p*i:p*(i+1), q*j:q*(j+1)] = Y[:,:,i+j+1]
+    H0 = H[:,:-q]
+    H1 = H[:,q:]
+    assert H0.shape == H1.shape == (p*(no), q*(nc))
+
+    # reduced SVD of Hankel matrix
+    _svd = numerics.svd_routine(**options.get("svd", {}))
+
+    U,S,V = _svd(H0)
+    SigmaInvSqrt = np.diag(S[:r]**-0.5)
+    SigmaSqrt = np.diag(S[:r]**0.5)
+    Ur = U[:,:r]
+    Vr = V[:,:r]
+
+    # get A from SVD and shifted Hankel matrix
+    Ar = SigmaInvSqrt @ Ur.T.conj() @ H1 @ Vr @ SigmaInvSqrt
+
+    # get B and C
+    Br = (SigmaSqrt @ Vr.T.conj())[:,:q]
+    Cr = (Ur @ SigmaSqrt)[:p,:]
+
+    return (Ar,Br,Cr,Dr)
+
+## ERA-DC ##
+# a = (alpha) number of block rows in Hankel of correlation matrix
+# b = (beta) number of block columns in Hankel of correlation matrix
+# l = initial lag for data correlations
+# g = lags (gap) between correlation matrices
+def era_dc(Y,no=None,nc=None,a=0,b=0,l=0,g=1,r=None,**options):
+    p,q,nt = Y.shape # p = number of outputs, q = number of inputs, nt = number of timesteps
+    if r is None:
+        r = int(nt/2)
+
+    # get D from first p x q block of impulse response
+    Dr = Y[:,:,0]  # first block of output data
+
+    # size of Hankel matrix
+    if no is None:
+        if nc is None:
+            no = nc = min(300, int(nt/2-1))
+        else:
+            no = min(300, int(nt/2-1))
+    elif nc is None:
+        nc = min(300, int(nt-no-2))
+    # make sure there are enough timesteps to assemble the Hankel matrices
+    assert nt >= l+(a+1+b+1)*g+no+nc
+
+    # Hankel matrix of impulse response (Markov parameters)
+    H = np.zeros((p*(no), q*(nc+l+(a+1+b+1)*g)))
+    for i in range(no):
+        for j in range(nc+l+(a+1+b+1)*g):
+            H[p*i:p*(i+1), q*j:q*(j+1)] = Y[:,:,i+j+1]
+    H0 = H[:,:q*nc]
+    assert H0.shape == (p*(no), q*(nc))
+
+    dimR = p*no # Dimension of square correlation matrices
+    dimHRl = (dimR*(a+1), dimR*(b+1)) # Dimension of Hankel matrix of correlation matrices
+    HRl = np.zeros(dimHRl) # Hankel matrix of correlation matrices
+    HRl1 = np.zeros(dimHRl) # Shifted Hankel matrix of correlation matrices
+    for i in range(a+1):
+        for j in range(b+1):
+            Hl = H[:, q*(l+1+(i+j)*g):q*(l+1+(i+j)*g+nc)]
+            Hl1 = H[:, q*(l+1+(i+j)*g+1):q*(l+1+(i+j)*g+nc+1)]
+            assert Hl.shape == Hl1.shape == (p*(no), q*(nc))
+            R = Hl@H0       # correlation matrix
+            R1 = Hl1@H0     # shifted correlation matrix
+            assert R.shape == R1.shape == (dimR,dimR)
+            HRl[dimR*i:dimR*(i+1), dimR*j:dimR*(j+1)] = R
+            HRl1[dimR*i:dimR*(i+1), dimR*j:dimR*(j+1)] = R1
+
+    # reduced SVD of Hankel matrix of correlation matrices
+    _svd = numerics.svd_routine(**options.get("svd", {}))
+
+    U,S,V = _svd(HRl)
+    SigmaInvSqrt = np.diag(S[:r]**-0.5)
+    SigmaSqrt = np.diag(S[:r]**0.5)
+    Ur = U[:,:r]
+    Vr = V[:,:r]
+
+    # get A from SVD and shifted Hankel matrix of correlation matrices
+    Ar = SigmaInvSqrt @ Ur.T.conj() @ HRl1 @ Vr @ SigmaInvSqrt
+
+    # get B and C
+    Br = ((SigmaInvSqrt @ Ur.T.conj())[:,:dimR] @ H0)[:,:q]
+    Cr = (Ur @ SigmaSqrt)[:p,:]
+
+    return (Ar,Br,Cr,Dr)
+
+
+def _blk_3(i, CA, U):
+    return i, np.einsum('kil,klj->ij', CA[:i,:,:], U[-i:,:,:])
+
+
+## SRIM ##
+# inputs = input data. dimensions of inputs: q x nt, where nt = number of timesteps.
+# outputs = response data due to input data. dimensions of outputs: p x nt.
+# no = number of steps used for identification (prediction horizon),
+    # and the order of the observability matrix.
+    # analagous to order (number of autoregressors) of the observer Kalman
+    # ARX filter used in OKID-ERA-DC.
+# r = size of the state-space model used for representing the system.
+# Juang 1997, "System Realization Using Information Matrix," Journal of Guidance, Control, and Dynamics
+def srim(inputs,outputs,no=None,r=None,full=True,pool_size=6,**options):
+    lsq_solve = numerics.lsq_solver(options.get("lsq", {}))
+
+    if len(inputs.shape) == 1:
+        inputs = inputs[None,:]
+    if len(outputs.shape) == 1:
+        outputs = outputs[None,:]
+
+    if inputs.shape[0] > inputs.shape[1]:
+        warnings.warn("input data has more channels (dim 1) than timesteps (dim 2)")
+    if outputs.shape[0] > outputs.shape[1]:
+        warnings.warn("output data has more channels (dim 1) than timesteps (dim 2)")
+
+    q,nt = inputs.shape
+    p = outputs.shape[0]
+    assert nt == outputs.shape[1]
+
+    if no is None:
+        no = min(300, nt)
+
+    if r is None:
+        r = min(10, int(no/2))
+
+    # maximum possible number of columns in the Y and U data matrices
+    ns = nt-1-no+2
+
+    assert no >= r/p + 1    # make sure prediction horizon is large enough that
+                            # observability matrix is full rank (Juang Eq. 8)
+
+    Yno = np.zeros((p*no,ns))
+    Uno = np.zeros((q*no,ns))
+
+    # progress_bar = lambda arg, **kwds: (i for i in arg)
+
+    # Construct Y (output) & U (input) data matrices (Eqs. 3.58 & 3.60 Arici 2006)
+    for i in range(no):
+        Yno[i*p:(i+1)*p,:] = outputs[:,i:ns+i]
+        Uno[i*q:(i+1)*q,:] = inputs[:,i:ns+i]
+
+
+    # 2b. Compute the correlation terms and the coefficient matrix 
+    #     (Eqs. 3.68 & 3.69).
+
+    # Compute the correlation terms (Eq. 3.68)
+    Ryy = Yno@Yno.T/ns
+    Ruu = Uno@Uno.T/ns
+    Ruy = Uno@Yno.T/ns
+
+    assert Ryy.shape[0] == Ryy.shape[1] == no*p
+    assert Ruy.shape[0] == no*q
+    assert Ruy.shape[1] == no*p
+
+    # Compute the correlation matrix (Eq. 3.69)
+    Rhh = Ryy - Ruy.T@lin_solve(Ruu,Ruy)
+
+    # 2c. Obtain observability matrix using full or partial decomposition 
+    #     (Eqs. 3.72 & 3.74).
+    if full:
+        # Full Decomposition Method
+        un,*_ = np.linalg.svd(Rhh,0)           # Eq. 3.74
+        Observability = un[:,:r]               # Eq. 3.72
+        A = lsq_solve(Observability[:(no-1)*p,:], Observability[p:no*p,:])
+        C = Observability[:p,:]
+    else:
+        # Partial Decomposition Method
+        un,*_ = np.linalg.svd(Rhh[:,:(no-1)*p+1],0)
+        Observability = un[:,:r]
+        A = lsq_solve(Observability[:(no-1)*p,:], Observability[p:no*p,:])
+        C = un[:p,:]
+
+    # Computation of system matrices B & D
+    # Output Error Minimization
+
+    # Setting up the Phi matrix
+    Phi  = np.zeros((p*ns, r+p*q+r*q))
+    CA_powers = np.zeros((ns, p, A.shape[1]))
+    CA_powers[0, :, :] = C
+    A_p = A
+    for pwr in range(1,ns):
+        CA_powers[pwr,:,:] =  C@A_p
+        A_p = A@A_p
+
+    # First block column of Phi
+    for df in range(ns):
+        Phi[df*p:(df+1)*p,:r] = CA_powers[df,:,:]
+
+    # Second block column of Phi
+    Ipp = np.eye(p)
+    for i in range(ns):
+        Phi[i*p:(i+1)*p, r:r+p*q] = np.kron(inputs[:,i],Ipp)
+
+    # Third block column of Phi
+    In1n1 = np.eye(r)
+    cc = r + p*q + 1
+    dd = r + p*q + r*q
+
+    krn = np.array([np.kron(inputs[:,i],In1n1) for i in range(ns)])
+
+    # Execute a loop in parallel that looks something like:
+    #    for i in  range(1,ns):
+    #        Phi[] = _blk_3(i, CA_Powers, np.flip(...))
+
+    with multiprocessing.Pool(pool_size) as pool:
+        for i,res in progress_bar(
+                pool.imap_unordered(
+                    partial(_blk_3, CA=CA_powers,U=np.flip(krn,0)),
+                    range(1,ns),
+                    200
+                ),
+                total = ns
+            ):
+            Phi[i*p:(i+1)*p,cc-1:dd] = res
+
+    y = outputs[:,:ns].flatten()
+
+    teta = lsq_solve(Phi,y)
+
+    x0 = teta[:r]
+    dcol = teta[r:r+p*q]
+    bcol = teta[r+p*q:r+p*q+r*q]
+
+    D = np.zeros((p,q))
+    B = np.zeros((r,q))
+    for wq in range(q):
+        D[:,wq] = dcol[wq*p:(wq+1)*p]
+
+    for ww in range(q):
+        B[:,ww] = bcol[ww*r:(ww+1)*r]
+
+    assert A.shape[0] == A.shape[1] == r
+
+    return A,B,C,D
+
+def subspace(outputs,no=None,r=None,cov_driven=True,**options):
+    outputs = np.atleast_2d(outputs)
+    p,nt = outputs.shape
+    assert nt > p
+
+    if no == None:
+        no = min(300, int(nt/2))
+    if r == None:
+        r = min(10,no-1)
+
+    if cov_driven:
+        Toep = np.zeros((p*no,p*no))
+        for i in range(2*no-1):
+            covs = np.zeros((p,p,no-1))
+            for k in range(no-1):
+                covs[:,:,k] = outputs[:,k+i]@outputs[k]
+            Ri = np.sum(covs,axis=3)/no
+            for j in range(i):
+                for l in range(j):
+                    Toep[j,-l-1] = Ri
+
+    else:
+        pass
+
+    return
```

### Comparing `ssid-0.0.4/src/ssid/srim.py` & `ssid-0.0.5/src/ssid/archive/srim.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,520 +1,520 @@
-__doc__="""
-# ssid : Structural System Identification
-"""
-# Standard library
-import sys
-import json
-import multiprocessing
-from functools import partial
-# Dependencies
-try:
-    from tqdm import tqdm
-except:
-    tqdm = lambda x,*args,**kwds: x
-
-import quakeio
-import numpy as np
-# from numpy import pi, log, sign
-from numpy.linalg import eig
-# import scipy.linalg as sl
-from ssid import ExtractModes
-
-linsolve = np.linalg.solve
-lsqminnorm = lambda *args: np.linalg.lstsq(*args, rcond=None)[0]
-
-class JSON_Encoder(json.JSONEncoder):
-    def default(self, obj):
-        if isinstance(obj, np.ndarray):
-            return obj.tolist()
-        elif isinstance(obj, np.integer):
-            return int(obj)
-        elif isinstance(obj, np.floating):
-            return float(obj)
-        return json.JSONEncoder.default(self, obj)
-
-REQUIREMENTS = """
-numpy
-scipy
-tqdm
-quakeio
-"""
-
-"""
-ssid srim <event.zip> <options>
-
-Options
--p
--m
-"""
-
-class IdentifiedSystem:
-    def __init__(self, time_step, A, B, C, D, **kwds):
-        self.system = A, B, C, D
-        self.freqdmp, modeshapeSRIM, *_ = ExtractModes.ComposeModes(time_step, A, B, C, D)
-
-    def __repr__(self):
-        import textwrap
-        try:
-            nln = "\n                "
-            return textwrap.dedent(f"""
-            Spectral quantities:
-                   T      \N{Mathematical Italic Small F}       \N{Greek Small Letter Zeta}
-                {nln.join(f"{1/i: <6.4}  {i: <6.4}  {j: <6.4}" for i,j in np.real(self.freqdmp[:,:2]))}
-            """)
-        except Exception as e:
-            return f"Error extracting modes: {e}; got '{self.freqdmp = }'"
-
-def parse_args(args):
-    outputs = []
-    parsers = {
-        "srim": parse_srim,
-        "test": parse_srim,
-        "okid": parse_okid
-    }
-    config = {}
-    argi = iter(args[1:])
-    for arg in argi:
-        if arg == "-p":
-            outputs.append(next(arg))
-        if arg == "--setup":
-            install_me()
-            sys.exit()
-        elif arg in ["--help", "-h"]:
-            print(HELP)
-            sys.exit()
-        else:
-            config["method"] = arg
-            return parsers[arg](argi, config), outputs
-
-#
-# SRIM
-#
-def _blk_3(i, CA, U):
-    return i, np.einsum('kil,klj->ij', CA[:i,:,:], U[-i:,:,:])
-
-
-def parse_srim(argi, config):
-    help="""
-    SRIM -- System Identification with Information Matrix
-
-    Parameters
-    p           order of the observer Kalman ARX filter.
-    n           size of the state-space model used for 
-                representing the system.
-    """
-    config.update({"p"  :  5, "orm":  4})
-    #argi = iter(args)
-    channels = [[17, 3, 20], [9, 7, 4]]
-    for arg in argi:
-        if arg == "-p":
-            config["p"] = int(next(argi))
-        elif arg == "--dt":
-            config["dt"] = float(next(argi))
-        elif arg == "-n":
-            config["orm"] = int(next(argi))
-        elif arg in ["--help", "-h"]:
-            print(help)
-            sys.exit()
-        elif arg == "--inputs":
-            inputs = next(argi)[1:-1].split(",")
-            if isinstance(inputs, str):
-                channels[0] = [int(inputs)]
-            else:
-                channels[0] = list(map(int, inputs))
-        elif arg == "--outputs":
-            outputs = next(argi)[1:-1].split(",")
-            if isinstance(outputs, str):
-                channels[1] = [int(outputs)]
-            else:
-                channels[1] = list(map(int, outputs))
-        elif arg == "--":
-            continue
-
-        else:
-            config["event_file"] = arg
-
-
-    event = quakeio.read(config["event_file"])
-    inputs = np.array([
-        event.match("l", station_channel=f"{i}").accel.data for i in channels[0]
-    ]).T
-    outputs = np.array([
-        event.match("l", station_channel=f"{i}").accel.data for i in channels[1]
-        #event.at(file_name=f"CHAN{i:03d}.V2").accel.data for i in channels[1]
-    ]).T
-    npoints = len(inputs[:,0])
-    dt = event.at(station_channel=f"{channels[0][0]}").accel["time_step"]
-    config["dt"] = dt
-
-    A,B,C,D = srim(inputs, outputs, **config)
-    freqdmpSRIM, modeshapeSRIM, *_ = ComposeModes(dt, A, B, C, D)
-    output = [
-            {"frequency": np.real(x[0]), "damping": np.real(x[1])} 
-            for x in freqdmpSRIM if all(x > 0.0)
-    ]
-    import json
-    print(json.dumps(output, cls=JSON_Encoder, indent=4))
-    return config
-
-def srim(
-    dati,
-    dato,
-    debug = False,
-    full     : bool = True,
-    verbose  : bool = False,
-    pool_size: int  = 6,
-    **config
-):
-    """
-    mro $(p)$ determines order of the observer Kalman ARX filter used in OKID-ERA-DC.
-    orm $(n)$ determines size of the state-space model used for representing the system.
-
-    Returns
-    =======
-     freqdampSRIM:
-        variable is a matrix that includes the information of identified
-        frequencies, damping ratios & validation of the modes with MPC & EMAC criteria.
-        Each row of freqdamp corresponds to a mode. Columns are as follows:
-        1) frequency, 2) damping ratio, 3) order index, 4) condition number, 5) MPC.
-        If values in columns 5 is > 0.5, identified mode is valid.
-     modeshapeSRIM:
-         stores the mode shape information for identified modes.
-     RMSEpredSRIM:
-         root mean square error of the predicted output from
-         identified parameters with respect to the actual output
-
-    ## SRIM Methodology
-
-    More information on SRIM algorithm can be found in Sections 3.4.4 & 3.4.5 of
-    (Arici & Mosalam, 2006). Equations below refer to this report. SRIM is a MIMO
-    SI method that is based on state space identification using least squares and
-    consists of the following steps:
-
-
-    2a. Determine output (y) & input (u) vectors [Eqs. 3.58 & 3.60].
-    2b. Compute the correlation terms & the coefficient matrix (Eqs. 3.68 & 3.69).
-    2c. Obtain observability matrix using full or partial decomposition (Eqs. 3.72 & 3.74).
-    2d. Use the observability matrix to compute system matrices A, B & C, in which modal 
-        information is embedded.
-    2e. Obtain the modal information from matrices A, B & C.
-    2f. Spatial & temporal validation of the identified modes.
-    2g. Back calculate (estimate) the output accelerations with the state-space system &
-        check against the actual output accelerations.
-
-    For orm = 2, one mode is found, for orm = 4, two modes are found.
-    For case 1, one mode is transverse & the other is torsion.
-    For all other cases, the second mode is a higher mode.
-    Sometimes higher orm still gives fewer modes, e.g. orm = 8 for case 1 gives
-    three modes, but one of them is invalid according to the EMAC & MPC criteria.
-    same orm in OKID-ERA-DC is used. It can be changed if needed.
-
-    """
-    #
-    # Convenience argument handling
-    #
-    dt = to = config.get("dt", None) or dati["time_step"]
-    p = config.get("p", config.get("mro"))         # # steps used for the identification (ie, prediction horizon)
-    n = n1 = config.get("n", config.get("orm", 4))  # Order of the model.
-
-    if isinstance(dati, list):
-        dati = np.array([i.data for i in dati]).T
-    elif issubclass(dati.__class__, dict):
-        dati = dati.data
-
-    if isinstance(dato, list):
-        dato = np.array([i.data for i in dato]).T
-    elif issubclass(dato.__class__, dict):
-        dato = dato.data
-
-    if len(dati.shape) < 2:
-        dati = np.atleast_2d(dati).T
-    if len(dato.shape) < 2:
-        dato = np.atleast_2d(dato).T
-
-    if verbose:
-        progress_bar = tqdm
-    else:
-        progress_bar = lambda arg, **kwds: (i for i in arg)
-
-    dn = config.get("dn", None) or dati.shape[0]
-
-    # 2a. Compute y (output) and u (input) vectors (Eqs. 3.58 & 3.60)
-
-    # Note that main Step 2 develops Eq. 3.57.
-    # Therefore, it is not part of the code.
-    # Accordingly, the code continues with Step 2a to compute the output & input vectors.
-
-    # Calculate the usable size of the data matrix
-    # dn = size(dat,1)/div;       # total # time steps after decimating
-    nsizS = dn-1-p+2
-
-    l,m = dato.shape # m is the number of output channels
-    _,r = dati.shape # r is the number of input channels
-
-
-    assert p >= n/m + 1
-
-    ypS = np.zeros((m*p,nsizS))
-    upS = np.zeros((r*p,nsizS))
-
-    # Compute Y (output) & U (input) vectors (Eqs. 3.58 & 3.60 Arici 2006)
-    for b in range(p):
-        ypS[b*m:(b+1)*m,:nsizS+1] = dato[b:nsizS+b, :].T
-        upS[b*r:(b+1)*r,:nsizS+1] = dati[b:nsizS+b, :].T
-
-
-    # 2b. Compute the correlation terms and the coefficient matrix 
-    #     (Eqs. 3.68 & 3.69).
-
-    # Compute the correlation terms (Eq. 3.68)
-    Ryy = ypS@ypS.T/nsizS
-    Ruu = upS@upS.T/nsizS
-    Ruy = upS@ypS.T/nsizS
-
-    assert Ryy.shape[0] == Ryy.shape[1] == p*m
-    assert Ruy.shape[0] == p*r
-    assert Ruy.shape[1] == p*m
-
-    # Compute the correlation matrix (Eq. 3.69)
-    Rhh = Ryy - Ruy.T@linsolve(Ruu,Ruy)
-
-    # 2c. Obtain observability matrix using full or partial decomposition 
-    #     (Eqs. 3.72 & 3.74).
-    if full:
-        # Full Decomposition Method
-        un,*_ = np.linalg.svd(Rhh,0)           # Eq. 3.74
-        Observability = un[:,:n]                          # Eq. 3.72
-        A = lsqminnorm(Observability[:(p-1)*m,:], Observability[m:p*m,:])
-        C = Observability[:m,:]
-    else:
-        # Partial Decomposition Method
-        un,*_ = np.linalg.svd(Rhh[:,:(p-1)*m+1],0)
-        Observability = un[:,:n]
-        A = lsqminnorm(Observability[:(p-1)*m,:], Observability[m:p*m,:])
-        C = un[:m,:]
-
-    # Computation of system matrices B & D
-    # Output Error Minimization
-
-    # Setting up the Phi matrix
-    Phi  = np.zeros((m*nsizS, n+m*r+n*r))
-    CA_powers = np.zeros((nsizS, m, A.shape[1]))
-    CA_powers[0, :, :] = C
-    A_p = A
-    for pwr in range(1,nsizS):
-        CA_powers[pwr,:,:] =  C@A_p
-        A_p = A@A_p
-
-    # First block column of Phi
-    for df in range(nsizS):
-        Phi[df*m:(df+1)*m,:n] = CA_powers[df,:,:]
-
-    # Second block column of Phi
-    Imm = np.eye(m)
-    for i in range(nsizS):
-        Phi[i*m:(i+1)*m, n:n+m*r] = np.kron(dati[i,:],Imm)
-
-    # Third block column of Phi
-    In1n1 = np.eye(n)
-    cc = n + m*r + 1
-    dd = n + m*r + n*r
-
-    krn = np.array([np.kron(dati[i,:],In1n1) for i in range(nsizS)])
-
-    with multiprocessing.Pool(pool_size) as pool:
-        for i,res in progress_bar(
-                pool.imap_unordered(
-                    partial(_blk_3,CA=CA_powers,U=np.flip(krn,0)),
-                    range(1,nsizS),
-                    200
-                ),
-                total = nsizS
-            ):
-            Phi[i*m:(i+1)*m,cc-1:dd] = res
-
-    y = dato[:nsizS,:].flatten()
-
-    teta = lsqminnorm(Phi,y)
-
-    x0 = teta[:n1]
-    dcol = teta[n1:n1+m*r]
-    bcol = teta[n1+m*r:n1+m*r+n1*r]
-
-    D = np.zeros((m,r))
-    B = np.zeros((n,r))
-    for wq in range(r):
-        D[:,wq] = dcol[wq*m:(wq+1)*m]
-
-    for ww in range(r):
-        B[:,ww] = bcol[ww*n:(ww+1)*n]
-
-    assert A.shape[0] == A.shape[1] == n
-    if debug:
-        return locals()
-    return A,B,C,D
-
-#PY
-# #% 2e. Obtain the modal information from the system matrices A & C
-# # This includes determination of: a) modal frequencies, b) damping ratios & c) mode shapes
-# # c) Determination of mode shapes
-#     mod = C1@vS                 # mode shapes (Eq. 3.40), v is the eigenvectors of matrix A
-# 
-
-#% 2f. Validation Analysis
-
-# Two criteria are used for selection of identified genuine modes, in terms of spatial & temporal consistency.
-# a) Modal Phase Collinearity (MPC) testing spatial consistency of identification results.
-#    Modes having MPC value above 0.5 (mpc parameter below) are considered as genuine modal quantities.
-# b) Extended Modal Amplitude Coherence (EMAC), evaluates temporal consistency of the identification results.
-#    Both output EMAC & input EMAC can be computed. Input EMAC requires the controllability matrix.
-#    Because the controllability matrix is not estimated by all considered SI methods,
-#    this criterion is computed, but not used.
-#    Modes with output EMAC values < 0.5 are considered spurious & therefore not reported.
-
-# a) Modal Phase Collinearity (MPC) [Eqs. 3.85-3.87]
-#Py
-##    for q in range(n):
-##        a = real(mod[:,q])
-##        b = imag(mod[:,q])
-##        sxx[:,q] = a.T*a
-##        syy[:,q] = b.T*b
-##        sxy[:,q] = a.T*b
-##        nu[q] = (syy[:,q]-sxx[:,q])/(2*sxy[:,q])
-##        lam[1,q] = (sxx[:,q]+syy[:,q])/2+sxy[:,q]*(nu(q)**2+1)**0.5
-##        lam[2,q] = (sxx[:,q]+syy[:,q])/2-sxy[:,q]*(nu(q)**2+1)**0.5
-##        mpc[q] = ((lam[0,q]-lam[1,q])/(lam[0,q]+lam[1,q]))**2
-
-
-# b) Extended Modal Amplitude Coherence (EMAC)
-
-# Only EMAC Output is computed as there is no Controllability Matrix
-
-# Note that the computations are commented out as the matrix B is needed
-
-#%KKKKK
-##PY
-##    plin = Op1@vS                # Observability Matrix used for the output-EMAC
-##    lamb = linsolve(vS,A1)*vS
-##    bkh = linsolve(vS,B)
-### Pick the last block row
-##    pto = plin((p-1)*m+1:m*p,:)  # the identified value at T0
-##    for ds in range(n):
-##        ptop[:,ds] = mod[:,ds]*exp(sj1S(ds)*to*(p-1))
-##
-### Computation of rij
-##    for qa in range(n):
-##        for qz in range(m):
-##            Rij(qa,qz) = min((abs(pto(qz,qa))/abs(ptop(qz,qa))),(abs(ptop(qz,qa))/abs(pto(qz,qa))))
-##            Pij = angle(pto(qz,qa)/ptop(qz,qa))
-##            Pijn(qa,qz) = Pij
-##            if abs(Pij) <= pi/4:
-##                Wij[qa,qz] = 1-abs(Pij)/(pi/4)
-##            else:
-##                Wij[qa,qz] = 0
-##
-##            emaco[qa,qz] = Rij[qa,qz]*Wij[qa,qz]
-##
-##
-### Computation of final emac
-##    for xc in range(n):
-##        # Weight for emaco
-##        sumo = 0.0
-##        for la in range(m):
-##            sumo = emaco(xc,la)*abs(mod(la,xc))**2+sumo
-##        emacof[xc] = sumo/((mod[:,xc].T*mod[:,xc]))
-##        emac[xc] = emaco[xc]
-#%KKKKK
-
-# Add the MPC to the matrix freqdampSRIM
-#    for lih = 1:size(freqdmpSRIM,1)
-#        freqdmpSRIM[lih,5] = emacof(freqdmpSRIM(lih,3))
-#        freqdmpSRIM[lih,6] = mpc(freqdmpSRIM(lih,3))
-#        if freqdmpSRIM[lih,5]>0.5 and freqdmpSRIM[lih,6]>0.5:
-#            validationm = ' valid'
-#        else:
-#            validationm = ' not valid'
-#
-#        scroutput = strcat('Mode',num2str(lih), ...
-#            ': Output EMAC =  ',num2str(freqdmpSRIM(lih,5)),...
-#            ', MPC =  ',num2str(freqdmpSRIM(lih,6)),...
-#            ' -->',' SRIM Identified Mode ',...
-#            num2str(lih), ' is',validationm)
-#        sprintf(scroutput)
-
-
-#% 2g. Back calculate (estimate) output accelerations with state-space system &
-#%     check against actual output accelerations
-
-# Note that the computations are commented out as the matrix B is needed
-
-# Prediction using state space model
-#%KKKKK
-##PY
-##    ms1 = modstruc(A1,B,C1,D,zeros(n,m),x0)
-##    th1 = ms2th(ms1,'d')
-##    e,r = resid([dato dati],th1)
-##    simy = idsim([dati],th1);                # simy represents the estimated accelerations
-##
-##    for i in range(m):
-##        temsum = sum((dato[:,i]-simy[:,i]).**2)
-##        Jm[i] = temsum/(sum(dato[:,i].**2));     # Root mean square error of estimated accelerations
-##
-##    RMSEpredSRIM = sum(Jm)/m
-###%KKKKK
-##    return freqdmpSRIM,modeshapeSRIM,RMSEpredSRIM
-
-
-if __name__ == "__main__":
-    import sys
-    import quakeio
-    from pathlib import Path
-    method = None
-
-    config, out_ops = parse_args(sys.argv)
-
-    if config["method"] == "test":
-        data_dir = Path("RioDell_Petrolia_Processed_Data")
-
-        first_input = quakeio.read(data_dir/f"CHAN{channels[0][0]:03d}.V2")
-        npoints = len(first_input.accel.data)
-        inputs, outputs = np.zeros((2,npoints,len(channels[0])))
-
-        # Inputs
-        inputs[:,0] = first_input.accel.data
-        for i,inp in enumerate(channels[0][1:]):
-            inputs[:,i+1] = quakeio.read(data_dir/f"CHAN{inp:03d}.V2").accel.data
-
-        # Outputs
-        for i,inp in enumerate(channels[1]):
-            outputs[:,i] = quakeio.read(data_dir/f"CHAN{inp:03d}.V2").accel.data
-
-        dt = first_input.accel["time_step"]
-        config["dt"] = dt
-
-    elif "event_file" in config:
-        event = quakeio.read(config["event_file"])
-        inputs = np.array([
-            event.match("l", station_channel=f"{i}").accel.data for i in channels[0]
-        ]).T
-        outputs = np.array([
-            event.match("l", station_channel=f"{i}").accel.data for i in channels[1]
-        ]).T
-        npoints = len(inputs[:,0])
-        dt = event.match("l", station_channel=f"{channels[0][0]}").accel["time_step"]
-        config["dt"] = dt
-
-    # print(config)
-    # sys.exit()
-
-    A,B,C,D = srim(inputs, outputs, **config)
-
-    freqdmpSRIM, modeshapeSRIM, *_ = ExtractModes.ComposeModes(dt, A, B, C, D)
-
-    if not out_ops:
-        print(f"period: {np.real(1/freqdmpSRIM[:,0])}")
-    elif "freq" in out_ops:
-        print(f"frequency: {freqdmpSRIM[:,0]}")
-    elif "cycl" in out_ops:
-        print(f"cyclic_frequency: {2*np.pi*freqdmpSRIM[:,0]}")
-
-
+__doc__="""
+# ssid : Structural System Identification
+"""
+# Standard library
+import sys
+import json
+import multiprocessing
+from functools import partial
+# Dependencies
+try:
+    from tqdm import tqdm
+except:
+    tqdm = lambda x,*args,**kwds: x
+
+import quakeio
+import numpy as np
+# from numpy import pi, log, sign
+from numpy.linalg import eig
+# import scipy.linalg as sl
+from ssid import ExtractModes
+
+linsolve = np.linalg.solve
+lsqminnorm = lambda *args: np.linalg.lstsq(*args, rcond=None)[0]
+
+class JSON_Encoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, np.ndarray):
+            return obj.tolist()
+        elif isinstance(obj, np.integer):
+            return int(obj)
+        elif isinstance(obj, np.floating):
+            return float(obj)
+        return json.JSONEncoder.default(self, obj)
+
+REQUIREMENTS = """
+numpy
+scipy
+tqdm
+quakeio
+"""
+
+"""
+ssid srim <event.zip> <options>
+
+Options
+-p
+-m
+"""
+
+class IdentifiedSystem:
+    def __init__(self, time_step, A, B, C, D, **kwds):
+        self.system = A, B, C, D
+        self.freqdmp, modeshapeSRIM, *_ = ExtractModes.ComposeModes(time_step, A, B, C, D)
+
+    def __repr__(self):
+        import textwrap
+        try:
+            nln = "\n                "
+            return textwrap.dedent(f"""
+            Spectral quantities:
+                   T      \N{Mathematical Italic Small F}       \N{Greek Small Letter Zeta}
+                {nln.join(f"{1/i: <6.4}  {i: <6.4}  {j: <6.4}" for i,j in np.real(self.freqdmp[:,:2]))}
+            """)
+        except Exception as e:
+            return f"Error extracting modes: {e}; got '{self.freqdmp = }'"
+
+def parse_args(args):
+    outputs = []
+    parsers = {
+        "srim": parse_srim,
+        "test": parse_srim,
+        "okid": parse_okid
+    }
+    config = {}
+    argi = iter(args[1:])
+    for arg in argi:
+        if arg == "-p":
+            outputs.append(next(arg))
+        if arg == "--setup":
+            install_me()
+            sys.exit()
+        elif arg in ["--help", "-h"]:
+            print(HELP)
+            sys.exit()
+        else:
+            config["method"] = arg
+            return parsers[arg](argi, config), outputs
+
+#
+# SRIM
+#
+def _blk_3(i, CA, U):
+    return i, np.einsum('kil,klj->ij', CA[:i,:,:], U[-i:,:,:])
+
+
+def parse_srim(argi, config):
+    help="""
+    SRIM -- System Identification with Information Matrix
+
+    Parameters
+    p           order of the observer Kalman ARX filter.
+    n           size of the state-space model used for 
+                representing the system.
+    """
+    config.update({"p"  :  5, "orm":  4})
+    #argi = iter(args)
+    channels = [[17, 3, 20], [9, 7, 4]]
+    for arg in argi:
+        if arg == "-p":
+            config["p"] = int(next(argi))
+        elif arg == "--dt":
+            config["dt"] = float(next(argi))
+        elif arg == "-n":
+            config["orm"] = int(next(argi))
+        elif arg in ["--help", "-h"]:
+            print(help)
+            sys.exit()
+        elif arg == "--inputs":
+            inputs = next(argi)[1:-1].split(",")
+            if isinstance(inputs, str):
+                channels[0] = [int(inputs)]
+            else:
+                channels[0] = list(map(int, inputs))
+        elif arg == "--outputs":
+            outputs = next(argi)[1:-1].split(",")
+            if isinstance(outputs, str):
+                channels[1] = [int(outputs)]
+            else:
+                channels[1] = list(map(int, outputs))
+        elif arg == "--":
+            continue
+
+        else:
+            config["event_file"] = arg
+
+
+    event = quakeio.read(config["event_file"])
+    inputs = np.array([
+        event.match("l", station_channel=f"{i}").accel.data for i in channels[0]
+    ]).T
+    outputs = np.array([
+        event.match("l", station_channel=f"{i}").accel.data for i in channels[1]
+        #event.at(file_name=f"CHAN{i:03d}.V2").accel.data for i in channels[1]
+    ]).T
+    npoints = len(inputs[:,0])
+    dt = event.at(station_channel=f"{channels[0][0]}").accel["time_step"]
+    config["dt"] = dt
+
+    A,B,C,D = srim(inputs, outputs, **config)
+    freqdmpSRIM, modeshapeSRIM, *_ = ComposeModes(dt, A, B, C, D)
+    output = [
+            {"frequency": np.real(x[0]), "damping": np.real(x[1])} 
+            for x in freqdmpSRIM if all(x > 0.0)
+    ]
+    import json
+    print(json.dumps(output, cls=JSON_Encoder, indent=4))
+    return config
+
+def srim(
+    dati,
+    dato,
+    debug = False,
+    full     : bool = True,
+    verbose  : bool = False,
+    pool_size: int  = 6,
+    **config
+):
+    """
+    mro $(p)$ determines order of the observer Kalman ARX filter used in OKID-ERA-DC.
+    orm $(n)$ determines size of the state-space model used for representing the system.
+
+    Returns
+    =======
+     freqdampSRIM:
+        variable is a matrix that includes the information of identified
+        frequencies, damping ratios & validation of the modes with MPC & EMAC criteria.
+        Each row of freqdamp corresponds to a mode. Columns are as follows:
+        1) frequency, 2) damping ratio, 3) order index, 4) condition number, 5) MPC.
+        If values in columns 5 is > 0.5, identified mode is valid.
+     modeshapeSRIM:
+         stores the mode shape information for identified modes.
+     RMSEpredSRIM:
+         root mean square error of the predicted output from
+         identified parameters with respect to the actual output
+
+    ## SRIM Methodology
+
+    More information on SRIM algorithm can be found in Sections 3.4.4 & 3.4.5 of
+    (Arici & Mosalam, 2006). Equations below refer to this report. SRIM is a MIMO
+    SI method that is based on state space identification using least squares and
+    consists of the following steps:
+
+
+    2a. Determine output (y) & input (u) vectors [Eqs. 3.58 & 3.60].
+    2b. Compute the correlation terms & the coefficient matrix (Eqs. 3.68 & 3.69).
+    2c. Obtain observability matrix using full or partial decomposition (Eqs. 3.72 & 3.74).
+    2d. Use the observability matrix to compute system matrices A, B & C, in which modal 
+        information is embedded.
+    2e. Obtain the modal information from matrices A, B & C.
+    2f. Spatial & temporal validation of the identified modes.
+    2g. Back calculate (estimate) the output accelerations with the state-space system &
+        check against the actual output accelerations.
+
+    For orm = 2, one mode is found, for orm = 4, two modes are found.
+    For case 1, one mode is transverse & the other is torsion.
+    For all other cases, the second mode is a higher mode.
+    Sometimes higher orm still gives fewer modes, e.g. orm = 8 for case 1 gives
+    three modes, but one of them is invalid according to the EMAC & MPC criteria.
+    same orm in OKID-ERA-DC is used. It can be changed if needed.
+
+    """
+    #
+    # Convenience argument handling
+    #
+    dt = to = config.get("dt", None) or dati["time_step"]
+    p = config.get("p", config.get("mro"))         # # steps used for the identification (ie, prediction horizon)
+    n = n1 = config.get("n", config.get("orm", 4))  # Order of the model.
+
+    if isinstance(dati, list):
+        dati = np.array([i.data for i in dati]).T
+    elif issubclass(dati.__class__, dict):
+        dati = dati.data
+
+    if isinstance(dato, list):
+        dato = np.array([i.data for i in dato]).T
+    elif issubclass(dato.__class__, dict):
+        dato = dato.data
+
+    if len(dati.shape) < 2:
+        dati = np.atleast_2d(dati).T
+    if len(dato.shape) < 2:
+        dato = np.atleast_2d(dato).T
+
+    if verbose:
+        progress_bar = tqdm
+    else:
+        progress_bar = lambda arg, **kwds: (i for i in arg)
+
+    dn = config.get("dn", None) or dati.shape[0]
+
+    # 2a. Compute y (output) and u (input) vectors (Eqs. 3.58 & 3.60)
+
+    # Note that main Step 2 develops Eq. 3.57.
+    # Therefore, it is not part of the code.
+    # Accordingly, the code continues with Step 2a to compute the output & input vectors.
+
+    # Calculate the usable size of the data matrix
+    # dn = size(dat,1)/div;       # total # time steps after decimating
+    nsizS = dn-1-p+2
+
+    l,m = dato.shape # m is the number of output channels
+    _,r = dati.shape # r is the number of input channels
+
+
+    assert p >= n/m + 1
+
+    ypS = np.zeros((m*p,nsizS))
+    upS = np.zeros((r*p,nsizS))
+
+    # Compute Y (output) & U (input) vectors (Eqs. 3.58 & 3.60 Arici 2006)
+    for b in range(p):
+        ypS[b*m:(b+1)*m,:nsizS+1] = dato[b:nsizS+b, :].T
+        upS[b*r:(b+1)*r,:nsizS+1] = dati[b:nsizS+b, :].T
+
+
+    # 2b. Compute the correlation terms and the coefficient matrix 
+    #     (Eqs. 3.68 & 3.69).
+
+    # Compute the correlation terms (Eq. 3.68)
+    Ryy = ypS@ypS.T/nsizS
+    Ruu = upS@upS.T/nsizS
+    Ruy = upS@ypS.T/nsizS
+
+    assert Ryy.shape[0] == Ryy.shape[1] == p*m
+    assert Ruy.shape[0] == p*r
+    assert Ruy.shape[1] == p*m
+
+    # Compute the correlation matrix (Eq. 3.69)
+    Rhh = Ryy - Ruy.T@linsolve(Ruu,Ruy)
+
+    # 2c. Obtain observability matrix using full or partial decomposition 
+    #     (Eqs. 3.72 & 3.74).
+    if full:
+        # Full Decomposition Method
+        un,*_ = np.linalg.svd(Rhh,0)           # Eq. 3.74
+        Observability = un[:,:n]                          # Eq. 3.72
+        A = lsqminnorm(Observability[:(p-1)*m,:], Observability[m:p*m,:])
+        C = Observability[:m,:]
+    else:
+        # Partial Decomposition Method
+        un,*_ = np.linalg.svd(Rhh[:,:(p-1)*m+1],0)
+        Observability = un[:,:n]
+        A = lsqminnorm(Observability[:(p-1)*m,:], Observability[m:p*m,:])
+        C = un[:m,:]
+
+    # Computation of system matrices B & D
+    # Output Error Minimization
+
+    # Setting up the Phi matrix
+    Phi  = np.zeros((m*nsizS, n+m*r+n*r))
+    CA_powers = np.zeros((nsizS, m, A.shape[1]))
+    CA_powers[0, :, :] = C
+    A_p = A
+    for pwr in range(1,nsizS):
+        CA_powers[pwr,:,:] =  C@A_p
+        A_p = A@A_p
+
+    # First block column of Phi
+    for df in range(nsizS):
+        Phi[df*m:(df+1)*m,:n] = CA_powers[df,:,:]
+
+    # Second block column of Phi
+    Imm = np.eye(m)
+    for i in range(nsizS):
+        Phi[i*m:(i+1)*m, n:n+m*r] = np.kron(dati[i,:],Imm)
+
+    # Third block column of Phi
+    In1n1 = np.eye(n)
+    cc = n + m*r + 1
+    dd = n + m*r + n*r
+
+    krn = np.array([np.kron(dati[i,:],In1n1) for i in range(nsizS)])
+
+    with multiprocessing.Pool(pool_size) as pool:
+        for i,res in progress_bar(
+                pool.imap_unordered(
+                    partial(_blk_3,CA=CA_powers,U=np.flip(krn,0)),
+                    range(1,nsizS),
+                    200
+                ),
+                total = nsizS
+            ):
+            Phi[i*m:(i+1)*m,cc-1:dd] = res
+
+    y = dato[:nsizS,:].flatten()
+
+    teta = lsqminnorm(Phi,y)
+
+    x0 = teta[:n1]
+    dcol = teta[n1:n1+m*r]
+    bcol = teta[n1+m*r:n1+m*r+n1*r]
+
+    D = np.zeros((m,r))
+    B = np.zeros((n,r))
+    for wq in range(r):
+        D[:,wq] = dcol[wq*m:(wq+1)*m]
+
+    for ww in range(r):
+        B[:,ww] = bcol[ww*n:(ww+1)*n]
+
+    assert A.shape[0] == A.shape[1] == n
+    if debug:
+        return locals()
+    return A,B,C,D
+
+#PY
+# #% 2e. Obtain the modal information from the system matrices A & C
+# # This includes determination of: a) modal frequencies, b) damping ratios & c) mode shapes
+# # c) Determination of mode shapes
+#     mod = C1@vS                 # mode shapes (Eq. 3.40), v is the eigenvectors of matrix A
+# 
+
+#% 2f. Validation Analysis
+
+# Two criteria are used for selection of identified genuine modes, in terms of spatial & temporal consistency.
+# a) Modal Phase Collinearity (MPC) testing spatial consistency of identification results.
+#    Modes having MPC value above 0.5 (mpc parameter below) are considered as genuine modal quantities.
+# b) Extended Modal Amplitude Coherence (EMAC), evaluates temporal consistency of the identification results.
+#    Both output EMAC & input EMAC can be computed. Input EMAC requires the controllability matrix.
+#    Because the controllability matrix is not estimated by all considered SI methods,
+#    this criterion is computed, but not used.
+#    Modes with output EMAC values < 0.5 are considered spurious & therefore not reported.
+
+# a) Modal Phase Collinearity (MPC) [Eqs. 3.85-3.87]
+#Py
+##    for q in range(n):
+##        a = real(mod[:,q])
+##        b = imag(mod[:,q])
+##        sxx[:,q] = a.T*a
+##        syy[:,q] = b.T*b
+##        sxy[:,q] = a.T*b
+##        nu[q] = (syy[:,q]-sxx[:,q])/(2*sxy[:,q])
+##        lam[1,q] = (sxx[:,q]+syy[:,q])/2+sxy[:,q]*(nu(q)**2+1)**0.5
+##        lam[2,q] = (sxx[:,q]+syy[:,q])/2-sxy[:,q]*(nu(q)**2+1)**0.5
+##        mpc[q] = ((lam[0,q]-lam[1,q])/(lam[0,q]+lam[1,q]))**2
+
+
+# b) Extended Modal Amplitude Coherence (EMAC)
+
+# Only EMAC Output is computed as there is no Controllability Matrix
+
+# Note that the computations are commented out as the matrix B is needed
+
+#%KKKKK
+##PY
+##    plin = Op1@vS                # Observability Matrix used for the output-EMAC
+##    lamb = linsolve(vS,A1)*vS
+##    bkh = linsolve(vS,B)
+### Pick the last block row
+##    pto = plin((p-1)*m+1:m*p,:)  # the identified value at T0
+##    for ds in range(n):
+##        ptop[:,ds] = mod[:,ds]*exp(sj1S(ds)*to*(p-1))
+##
+### Computation of rij
+##    for qa in range(n):
+##        for qz in range(m):
+##            Rij(qa,qz) = min((abs(pto(qz,qa))/abs(ptop(qz,qa))),(abs(ptop(qz,qa))/abs(pto(qz,qa))))
+##            Pij = angle(pto(qz,qa)/ptop(qz,qa))
+##            Pijn(qa,qz) = Pij
+##            if abs(Pij) <= pi/4:
+##                Wij[qa,qz] = 1-abs(Pij)/(pi/4)
+##            else:
+##                Wij[qa,qz] = 0
+##
+##            emaco[qa,qz] = Rij[qa,qz]*Wij[qa,qz]
+##
+##
+### Computation of final emac
+##    for xc in range(n):
+##        # Weight for emaco
+##        sumo = 0.0
+##        for la in range(m):
+##            sumo = emaco(xc,la)*abs(mod(la,xc))**2+sumo
+##        emacof[xc] = sumo/((mod[:,xc].T*mod[:,xc]))
+##        emac[xc] = emaco[xc]
+#%KKKKK
+
+# Add the MPC to the matrix freqdampSRIM
+#    for lih = 1:size(freqdmpSRIM,1)
+#        freqdmpSRIM[lih,5] = emacof(freqdmpSRIM(lih,3))
+#        freqdmpSRIM[lih,6] = mpc(freqdmpSRIM(lih,3))
+#        if freqdmpSRIM[lih,5]>0.5 and freqdmpSRIM[lih,6]>0.5:
+#            validationm = ' valid'
+#        else:
+#            validationm = ' not valid'
+#
+#        scroutput = strcat('Mode',num2str(lih), ...
+#            ': Output EMAC =  ',num2str(freqdmpSRIM(lih,5)),...
+#            ', MPC =  ',num2str(freqdmpSRIM(lih,6)),...
+#            ' -->',' SRIM Identified Mode ',...
+#            num2str(lih), ' is',validationm)
+#        sprintf(scroutput)
+
+
+#% 2g. Back calculate (estimate) output accelerations with state-space system &
+#%     check against actual output accelerations
+
+# Note that the computations are commented out as the matrix B is needed
+
+# Prediction using state space model
+#%KKKKK
+##PY
+##    ms1 = modstruc(A1,B,C1,D,zeros(n,m),x0)
+##    th1 = ms2th(ms1,'d')
+##    e,r = resid([dato dati],th1)
+##    simy = idsim([dati],th1);                # simy represents the estimated accelerations
+##
+##    for i in range(m):
+##        temsum = sum((dato[:,i]-simy[:,i]).**2)
+##        Jm[i] = temsum/(sum(dato[:,i].**2));     # Root mean square error of estimated accelerations
+##
+##    RMSEpredSRIM = sum(Jm)/m
+###%KKKKK
+##    return freqdmpSRIM,modeshapeSRIM,RMSEpredSRIM
+
+
+if __name__ == "__main__":
+    import sys
+    import quakeio
+    from pathlib import Path
+    method = None
+
+    config, out_ops = parse_args(sys.argv)
+
+    if config["method"] == "test":
+        data_dir = Path("RioDell_Petrolia_Processed_Data")
+
+        first_input = quakeio.read(data_dir/f"CHAN{channels[0][0]:03d}.V2")
+        npoints = len(first_input.accel.data)
+        inputs, outputs = np.zeros((2,npoints,len(channels[0])))
+
+        # Inputs
+        inputs[:,0] = first_input.accel.data
+        for i,inp in enumerate(channels[0][1:]):
+            inputs[:,i+1] = quakeio.read(data_dir/f"CHAN{inp:03d}.V2").accel.data
+
+        # Outputs
+        for i,inp in enumerate(channels[1]):
+            outputs[:,i] = quakeio.read(data_dir/f"CHAN{inp:03d}.V2").accel.data
+
+        dt = first_input.accel["time_step"]
+        config["dt"] = dt
+
+    elif "event_file" in config:
+        event = quakeio.read(config["event_file"])
+        inputs = np.array([
+            event.match("l", station_channel=f"{i}").accel.data for i in channels[0]
+        ]).T
+        outputs = np.array([
+            event.match("l", station_channel=f"{i}").accel.data for i in channels[1]
+        ]).T
+        npoints = len(inputs[:,0])
+        dt = event.match("l", station_channel=f"{channels[0][0]}").accel["time_step"]
+        config["dt"] = dt
+
+    # print(config)
+    # sys.exit()
+
+    A,B,C,D = srim(inputs, outputs, **config)
+
+    freqdmpSRIM, modeshapeSRIM, *_ = ExtractModes.ComposeModes(dt, A, B, C, D)
+
+    if not out_ops:
+        print(f"period: {np.real(1/freqdmpSRIM[:,0])}")
+    elif "freq" in out_ops:
+        print(f"frequency: {freqdmpSRIM[:,0]}")
+    elif "cycl" in out_ops:
+        print(f"cyclic_frequency: {2*np.pi*freqdmpSRIM[:,0]}")
+
+
```

### Comparing `ssid-0.0.4/src/ssid/validation.py` & `ssid-0.0.5/src/ssid/validation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,80 @@
-import numpy as np
-from numpy import pi
-
-def EnergyCondensedEMAC(emac,phi):
-    n,p = emac.shape
-    assert emac.shape == phi.shape
-    "Equation 3.93"
-    return np.array([
-        sum(emac[i,j]*abs(phi[i,j])**2 
-            for j in range(p)
-        )/np.real(phi[i,:].conjugate().transpose()@phi[i,:])
-        for i in range(n) 
-    ])
-
-def EMAC_Matrix(Phi_final, Phi_final_hat):
-    p,n = Phi_final.shape
-    emac = np.zeros((n,p))
-    for i in range(n):
-        for j in range(p):
-            Rij = min(
-                (abs(Phi_final[j,i])/abs(Phi_final_hat[j,i])),
-                (abs(Phi_final_hat[j,i])/abs(Phi_final[j,i]))
-            )
-            Pij = np.angle(Phi_final[j,i]/Phi_final_hat[j,i])
-            Wij = max(
-                1 - abs(Pij)/(pi/4),
-                0
-            )
-            emac[i,j] = Rij*Wij
-    return emac
-
-# nt = number of timesteps (for OKID-ERA-DC and OKID-ERA, number of Markov parameters)
-# Psi = eigenvectors of A, as columns of a matrix. can be reused from modal.system_modes().
-# Gam = eigenvalues of A, as items of a vector. can be reused from modal.system_modes().
-# Observability matrix can be reused from realize.srim().
-# p = number of outputs
-# n = model order (number of system variables)
-def OutputEMAC(A,C,nt,Observability=None,Psi=None,Gam=None):
-    p,n = C.shape
-    assert A.shape == (n,n)
-    """Output EMAC (Eqs. 3.88-3.89)"""
-    if Gam is None:
-        assert Psi is None
-        from ssid.modal import condeig 
-        Psi,Gam,_ = condeig(A)
-    if Observability is None:
-        Observability = np.empty((nt,p,n))
-        Observability[0,:,:] = C
-        A_pwr = A
-        for pwr in range(1,nt):
-            Observability[pwr,:,:] =  C@A_pwr
-            A_pwr = A@A_pwr
-        Observability = Observability.reshape((nt*p,n))
-    Phi_final = Observability[-p:,:]@Psi                    # identified modal observability at the last timestep (last block row)
-    Phi_final = Observability[-p:,:]@Psi                    # identified modal observability at the last timestep (last block row)
-    Phi_final_hat = C@Psi@np.diag(Gam**(nt-1))              # expected modal observability at the last timestep
-    assert Phi_final.shape == Phi_final_hat.shape == (p,n)
-    emaco  = EMAC_Matrix(Phi_final,Phi_final_hat)
-    return EnergyCondensedEMAC(emaco,(C@Psi).T)             # DIM: nxp, nxp
-
-def MPC(A,C,Psi=None):
-    """a) Modal Phase Collinearity (MPC) [Eqs. 3.85-3.87]"""
-    if Psi is None:
-        from ssid.modal import condeig 
-        Psi,_,_ = condeig(A)
-    _,n = C.shape
-    assert Psi.shape == (n,n)
-    modes_raw = C@Psi
-    s11, s22, s12 = np.zeros((3,n))
-    nu, mpc = np.zeros((2, n))
-    lam = np.zeros((2, n))
-    for i in range(n):
-        mode_i = modes_raw[:,i]
-        s11[i] = np.real(mode_i).conjugate().transpose()@np.real(mode_i)
-        s22[i] = np.imag(mode_i).conjugate().transpose()@np.imag(mode_i)
-        s12[i] = np.real(mode_i).conjugate().transpose()@np.imag(mode_i)
-        nu[i]    = (s22[i]-s11[i])/(2*s12[i])
-        lam[0,i] = (s11[i]+s22[i])/2 + s12[i]*np.sqrt(nu[i]**2+1)
-        lam[1,i] = (s11[i]+s22[i])/2 - s12[i]*np.sqrt(nu[i]**2+1)
-        mpc[i]   = ((lam[0,i]-lam[1,i])/(lam[0,i]+lam[1,i]))**2
+import numpy as np
+from numpy import pi
+
+def EnergyCondensedEMAC(emac,phi):
+    n,p = emac.shape
+    assert emac.shape == phi.shape
+    "Equation 3.93"
+    return np.array([
+        sum(emac[i,j]*abs(phi[i,j])**2 
+            for j in range(p)
+        )/np.real(phi[i,:].conjugate().transpose()@phi[i,:])
+        for i in range(n) 
+    ])
+
+def EMAC_Matrix(Phi_final, Phi_final_hat):
+    p,n = Phi_final.shape
+    emac = np.zeros((n,p))
+    for i in range(n):
+        for j in range(p):
+            Rij = min(
+                (abs(Phi_final[j,i])/abs(Phi_final_hat[j,i])),
+                (abs(Phi_final_hat[j,i])/abs(Phi_final[j,i]))
+            )
+            Pij = np.angle(Phi_final[j,i]/Phi_final_hat[j,i])
+            Wij = max(
+                1 - abs(Pij)/(pi/4),
+                0
+            )
+            emac[i,j] = Rij*Wij
+    return emac
+
+# nt = number of timesteps (for OKID-ERA-DC and OKID-ERA, number of Markov parameters)
+# Psi = eigenvectors of A, as columns of a matrix. can be reused from modal.system_modes().
+# Gam = eigenvalues of A, as items of a vector. can be reused from modal.system_modes().
+# Observability matrix can be reused from realize.srim().
+# p = number of outputs
+# n = model order (number of system variables)
+def OutputEMAC(A,C,nt,Observability=None,Psi=None,Gam=None):
+    p,n = C.shape
+    assert A.shape == (n,n)
+    """Output EMAC (Eqs. 3.88-3.89)"""
+    if Gam is None:
+        assert Psi is None
+        from ssid.modal import condeig 
+        Psi,Gam,_ = condeig(A)
+    if Observability is None:
+        Observability = np.empty((nt,p,n))
+        Observability[0,:,:] = C
+        A_pwr = A
+        for pwr in range(1,nt):
+            Observability[pwr,:,:] =  C@A_pwr
+            A_pwr = A@A_pwr
+        Observability = Observability.reshape((nt*p,n))
+    Phi_final = Observability[-p:,:]@Psi                    # identified modal observability at the last timestep (last block row)
+    Phi_final_hat = C@Psi@np.diag(Gam**(nt-1))              # expected modal observability at the last timestep
+    assert Phi_final.shape == Phi_final_hat.shape == (p,n)
+    emaco  = EMAC_Matrix(Phi_final,Phi_final_hat)
+    return EnergyCondensedEMAC(emaco,(C@Psi).T)             # DIM: nxp, nxp
+
+def MPC(A,C,Psi=None):
+    """a) Modal Phase Collinearity (MPC) [Eqs. 3.85-3.87]"""
+    if Psi is None:
+        from ssid.modal import condeig 
+        Psi,_,_ = condeig(A)
+    _,n = C.shape
+    assert Psi.shape == (n,n)
+    modes_raw = C@Psi
+    s11, s22, s12 = np.zeros((3,n))
+    nu, mpc = np.zeros((2,n))
+    lam = np.zeros((2,n))
+    for i in range(n):
+        mode_i = modes_raw[:,i]
+        s11[i] = np.real(mode_i).conjugate().transpose()@np.real(mode_i)
+        s22[i] = np.imag(mode_i).conjugate().transpose()@np.imag(mode_i)
+        s12[i] = np.real(mode_i).conjugate().transpose()@np.imag(mode_i)
+        nu[i]    = (s22[i]-s11[i])/(2*s12[i])
+        lam[0,i] = (s11[i]+s22[i])/2 + s12[i]*np.sqrt(nu[i]**2+1)
+        lam[1,i] = (s11[i]+s22[i])/2 - s12[i]*np.sqrt(nu[i]**2+1)
+        mpc[i]   = ((lam[0,i]-lam[1,i])/(lam[0,i]+lam[1,i]))**2
     return mpc
```

### Comparing `ssid-0.0.4/tests/test1.py` & `ssid-0.0.5/tests/test1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# use the environment intel or py39
-
 import quakeio
 import ssid
 import sys
 from pathlib import Path
 import numpy as np
 from ssid import okid, srim, ExtractModes
 
@@ -80,29 +78,21 @@
 #     }
 # }
 
 
 # config = hwd_configs[1]["config"]
 
 
-# config = dict(
-#     # Transverse
-#     bridge  = "painter",
-#     # inputs  = [3],
-#     # outputs = [7]    
-#     inputs  = [17, 3, 20],
-#     outputs = [ 9, 7 , 4]
-# )
-
-
 config = dict(
-    # Transverse hayward
-    bridge = "hayward",
-    inputs = [2,7,25,18],
-    outputs = [13,15,23,20]
+    # Transverse
+    bridge  = "painter",
+    # inputs  = [3],
+    # outputs = [7]    
+    inputs  = [17, 3, 20],
+    outputs = [ 9, 7 , 4]
 )
 
 
 mro = 10
 # mro = 20
 # mro = 100
 orm = 4
@@ -127,19 +117,18 @@
         outpts = [
             event.match("l", station_channel=str(chan)).accel
             for chan in config["outputs"]
         ]
         dt = inputs[0]["time_step"]
         # A,B,C,D = ssid.srim(inputs, outpts, dt=dt, mro=100,orm=10,verbose=True)
         if True:
-            local_vars = ssid.okid.okid(inputs, outpts, dt=dt, mro=mro,orm=orm,kmax=kmax, verbose=True, debug=True)
-            # local_vars = ssid.srim(inputs, outpts, dt=dt, mro=mro,orm=orm, verbose=True, debug=True)
+            # local_vars = ssid.okid.okid(inputs, outpts, dt=dt, mro=mro,orm=orm,kmax=kmax, verbose=True, debug=True)
+            local_vars = ssid.srim(inputs, outpts, dt=dt, mro=mro,orm=orm, verbose=True, debug=True)
             local_vars["debug"] = False
-            emacof = ssid.validation.OutputEMAC(**local_vars)
-            # emacof = ssid.validation.OutputEMAC(kmax=mro,**local_vars)
+            emacof = ssid.validation.OutputEMAC(kmax=mro,**local_vars)
             break
         A,B,C,D = ssid.okid.okid(inputs, outpts, dt=dt, mro=mro,orm=orm,kmax=kmax, verbose=True)
 
     except:
         raise 
         print(f"failed {file.name}")
```

