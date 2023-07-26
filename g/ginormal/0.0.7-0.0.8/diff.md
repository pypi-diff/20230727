# Comparing `tmp/ginormal-0.0.7.tar.gz` & `tmp/ginormal-0.0.8.tar.gz`

## Comparing `ginormal-0.0.7.tar` & `ginormal-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 ginormal-0.0.7/src/ginormal/__init__.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 ginormal-0.0.7/src/ginormal/example.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 ginormal-0.0.7/src/ginormal/main.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 ginormal-0.0.7/src/intermediate/_F0g.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 ginormal-0.0.7/src/intermediate/__init__.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 ginormal-0.0.7/src/intermediate/_dg1.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ginormal-0.0.7/src/intermediate/_msh.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ginormal-0.0.7/src/intermediate/_pbd.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 ginormal-0.0.7/src/intermediate/_rtg1.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ginormal-0.0.7/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ginormal-0.0.7/LICENSE.md
--rw-r--r--   0        0        0     8518 2020-02-02 00:00:00.000000 ginormal-0.0.7/README.md
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 ginormal-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     9377 2020-02-02 00:00:00.000000 ginormal-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 ginormal-0.0.8/src/ginormal/__init__.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 ginormal-0.0.8/src/ginormal/dgin.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 ginormal-0.0.8/src/ginormal/dtgin.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 ginormal-0.0.8/src/ginormal/example.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 ginormal-0.0.8/src/ginormal/rgin.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 ginormal-0.0.8/src/ginormal/rtgin.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 ginormal-0.0.8/src/ginormal/utils/F0gin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ginormal-0.0.8/src/ginormal/utils/__init__.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 ginormal-0.0.8/src/ginormal/utils/dgin1.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ginormal-0.0.8/src/ginormal/utils/mshift.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ginormal-0.0.8/src/ginormal/utils/pbdam.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 ginormal-0.0.8/src/ginormal/utils/rtgin1.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ginormal-0.0.8/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ginormal-0.0.8/LICENSE.md
+-rw-r--r--   0        0        0     8518 2020-02-02 00:00:00.000000 ginormal-0.0.8/README.md
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 ginormal-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     9377 2020-02-02 00:00:00.000000 ginormal-0.0.8/PKG-INFO
```

### Comparing `ginormal-0.0.7/src/ginormal/example.py` & `ginormal-0.0.8/src/ginormal/example.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.7/src/intermediate/_dg1.py` & `ginormal-0.0.8/src/ginormal/utils/dgin1.py`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.7/src/intermediate/_rtg1.py` & `ginormal-0.0.8/src/ginormal/utils/rtgin1.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 import numpy as np
 from scipy import special, stats
 from cardano_method import CubicEquation
 import warnings
 
-from intermediate import _msh as msh
-from intermediate import _dg1 as dg_1
-from intermediate import _pbd as pbd
+from ginormal.utils.mshift import mshift
+from ginormal.utils.dgin1 import dgin1
+from ginormal.utils.pbdam import pbdam
 
 def rtgin1(a, m, sign, algo='hormann', verbose=False):
     # If sign = True, draw from the positive region Z > 0
     # If sign = False, draw from the negative region Z < 0
     if algo == 'hormann':
         algo_1 = True
     elif algo == 'leydold':
         algo_1 = False
     else:
         raise ValueError("algo_method must be either 'hormann' or 'leydold'")
     
     # Compute necessary values for ratio-of-uniforms method
-    if (sign):
-        mode = (-m + np.sqrt(m ** 2 + 4 * a)) / (2 * a)
-        mult = -1
-    else:
-        mode = (-m - np.sqrt(m ** 2 + 4 * a)) / (2 * a)
-        mult = 1
+    mult = 1 - 2*sign
+    mode = (-m - mult*np.sqrt(m ** 2 + 4 * a)) / (2 * a)
     
-
     # Draw from minimal bounding rectangle and accept draw
-    vmax = msh.mshift(mode, mode, a, m, False)
+    vmax = mshift(mode, mode, a, m, False)
     if algo_1:
         # Hörmann and Leydold (2014) using Cardano method
         roots = np.real(CubicEquation([2 - a, -m + a * mode, 1 + m * mode, -mode]).answers)
         roots = roots[-mult * roots > 0]
-        uvals = np.sort([msh.mshift(roots[j], mode, a, m) for j in range(2)])
+        uvals = np.sort([mshift(roots[j], mode, a, m) for j in range(2)])
     else:
         # Leydold (2001) using the proportionality constant
-        lcons = -0.25 * m ** 2 + special.loggamma(a - 1) + np.log(pbd.pbdam(a, mult * m))
+        lcons = -0.25 * m ** 2 + special.loggamma(a - 1) + np.log(pbdam(a, mult * m))
         vp = np.exp(lcons) / vmax
         uvals = np.array([-vp, vp])
 
     # Acceptance-Rejection algorithm (ratio-of-uniforms)
     test = False
     counter = 0
     max_iter = 100
     while (not test):
         u = stats.uniform.rvs(uvals[0], uvals[1] - uvals[0], size=1)[0]
         v = stats.uniform.rvs(0, vmax, size=1)[0]
         x = (u / v) + mode
-        test = (2 * np.log(v) <= dg_1.dgin1(x, a, m, True, True)) & (-mult * x > 0)
+        test = (2 * np.log(v) <= dgin1(x, a, m, True, True)) & (-mult * x > 0)
         counter += 1
         if counter > max_iter:
             x = mode
             warnings.warn("No candidate draw found for these parameter values. Giving up an returning the mode of the distribution")
             break
     if verbose:
         return {'value': x, 'ARiters': counter}
```

### Comparing `ginormal-0.0.7/README.md` & `ginormal-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ginormal-0.0.7/pyproject.toml` & `ginormal-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 # Package metadata
 [project]
 name = "ginormal"
-version = "0.0.7"
+version = "0.0.8"
 requires-python = ">=3.8"
 description = "Generalized Inverse Normal distribution density and generation"
 readme = "README.md"
 authors = [
   { name = "Santiago Montoya-Blandón", email = "Santiago.Montoya-Blandon@glasgow.ac.uk" },
   { name = "Cheng Ding", email = "cheng.ding.emory@gmail.com"},
   { name = "Juan Estrada", email = "jjestra@emory.edu"},
```

### Comparing `ginormal-0.0.7/PKG-INFO` & `ginormal-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ginormal
-Version: 0.0.7
+Version: 0.0.8
 Summary: Generalized Inverse Normal distribution density and generation
 Project-URL: Homepage, https://github.com/smonto2/GIN
 Project-URL: Bug tracking, https://github.com/smonto2/GIN/issues
 Author-email: Santiago Montoya-Blandón <Santiago.Montoya-Blandon@glasgow.ac.uk>, Cheng Ding <cheng.ding.emory@gmail.com>, Juan Estrada <jjestra@emory.edu>, Zhilang Xia <zhilang.xia@glasgow.ac.uk>
 Maintainer-email: Santiago Montoya-Blandón <Santiago.Montoya-Blandon@glasgow.ac.uk>
 License-File: LICENSE.md
 Keywords: distribution,generalized inverse normal,random variable generation,statistics
```

