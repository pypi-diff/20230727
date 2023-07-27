# Comparing `tmp/lmfitxps-1.2.0.tar.gz` & `tmp/lmfitxps-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/julian/Desktop/lmfit-additional-models/dist/.tmp-x9u_r598/lmfitxps-1.2.0.tar", last modified: Wed Jul 26 15:01:05 2023, max compression
+gzip compressed data, was "/home/julian/Desktop/lmfit-additional-models/dist/.tmp-bwaaq7ei/lmfitxps-1.3.0.tar", last modified: Thu Jul 27 16:08:33 2023, max compression
```

## Comparing `lmfitxps-1.2.0.tar` & `lmfitxps-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-07-26 15:01:05.364823 lmfitxps-1.2.0/
--rw-rw-r--   0 julian    (1000) julian    (1000)     3057 2023-07-25 12:03:21.000000 lmfitxps-1.2.0/LICENSE
--rw-rw-r--   0 julian    (1000) julian    (1000)     5379 2023-07-26 15:01:05.364823 lmfitxps-1.2.0/PKG-INFO
--rw-rw-r--   0 julian    (1000) julian    (1000)     1412 2023-07-25 12:04:12.000000 lmfitxps-1.2.0/README.md
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-07-26 15:01:05.360823 lmfitxps-1.2.0/lmfitxps/
--rw-rw-r--   0 julian    (1000) julian    (1000)        0 2023-07-25 12:03:21.000000 lmfitxps-1.2.0/lmfitxps/__init__.py
--rw-rw-r--   0 julian    (1000) julian    (1000)    12073 2023-07-26 14:59:53.000000 lmfitxps-1.2.0/lmfitxps/backgrounds.py
--rw-rw-r--   0 julian    (1000) julian    (1000)     7048 2023-07-26 14:59:53.000000 lmfitxps-1.2.0/lmfitxps/lineshapes.py
--rw-rw-r--   0 julian    (1000) julian    (1000)    12986 2023-07-26 14:59:53.000000 lmfitxps-1.2.0/lmfitxps/models.py
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-07-26 15:01:05.360823 lmfitxps-1.2.0/lmfitxps.egg-info/
--rw-rw-r--   0 julian    (1000) julian    (1000)     5379 2023-07-26 15:01:05.000000 lmfitxps-1.2.0/lmfitxps.egg-info/PKG-INFO
--rw-rw-r--   0 julian    (1000) julian    (1000)      273 2023-07-26 15:01:05.000000 lmfitxps-1.2.0/lmfitxps.egg-info/SOURCES.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)        1 2023-07-26 15:01:05.000000 lmfitxps-1.2.0/lmfitxps.egg-info/dependency_links.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)        9 2023-07-26 15:01:05.000000 lmfitxps-1.2.0/lmfitxps.egg-info/top_level.txt
--rw-rw-r--   0 julian    (1000) julian    (1000)      552 2023-07-26 14:59:53.000000 lmfitxps-1.2.0/pyproject.toml
--rw-rw-r--   0 julian    (1000) julian    (1000)       38 2023-07-26 15:01:05.364823 lmfitxps-1.2.0/setup.cfg
-drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-07-26 15:01:05.364823 lmfitxps-1.2.0/tests/
--rw-rw-r--   0 julian    (1000) julian    (1000)      209 2023-07-26 13:48:02.000000 lmfitxps-1.2.0/tests/test_backgrounds.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-07-27 16:08:33.651634 lmfitxps-1.3.0/
+-rw-rw-r--   0 julian    (1000) julian    (1000)     3057 2023-07-25 12:03:21.000000 lmfitxps-1.3.0/LICENSE
+-rw-rw-r--   0 julian    (1000) julian    (1000)     5379 2023-07-27 16:08:33.647634 lmfitxps-1.3.0/PKG-INFO
+-rw-rw-r--   0 julian    (1000) julian    (1000)     1412 2023-07-25 12:04:12.000000 lmfitxps-1.3.0/README.md
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-07-27 16:08:33.647634 lmfitxps-1.3.0/lmfitxps/
+-rw-rw-r--   0 julian    (1000) julian    (1000)        0 2023-07-25 12:03:21.000000 lmfitxps-1.3.0/lmfitxps/__init__.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)    11543 2023-07-27 16:07:41.000000 lmfitxps-1.3.0/lmfitxps/backgrounds.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)     7048 2023-07-27 16:07:41.000000 lmfitxps-1.3.0/lmfitxps/lineshapes.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)    13001 2023-07-27 16:07:41.000000 lmfitxps-1.3.0/lmfitxps/models.py
+-rw-rw-r--   0 julian    (1000) julian    (1000)       21 2023-07-27 08:49:02.000000 lmfitxps-1.3.0/lmfitxps/test.py
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-07-27 16:08:33.647634 lmfitxps-1.3.0/lmfitxps.egg-info/
+-rw-rw-r--   0 julian    (1000) julian    (1000)     5379 2023-07-27 16:08:33.000000 lmfitxps-1.3.0/lmfitxps.egg-info/PKG-INFO
+-rw-rw-r--   0 julian    (1000) julian    (1000)      290 2023-07-27 16:08:33.000000 lmfitxps-1.3.0/lmfitxps.egg-info/SOURCES.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)        1 2023-07-27 16:08:33.000000 lmfitxps-1.3.0/lmfitxps.egg-info/dependency_links.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)        9 2023-07-27 16:08:33.000000 lmfitxps-1.3.0/lmfitxps.egg-info/top_level.txt
+-rw-rw-r--   0 julian    (1000) julian    (1000)      552 2023-07-27 16:07:41.000000 lmfitxps-1.3.0/pyproject.toml
+-rw-rw-r--   0 julian    (1000) julian    (1000)       38 2023-07-27 16:08:33.651634 lmfitxps-1.3.0/setup.cfg
+drwxrwxr-x   0 julian    (1000) julian    (1000)        0 2023-07-27 16:08:33.647634 lmfitxps-1.3.0/tests/
+-rw-rw-r--   0 julian    (1000) julian    (1000)     3482 2023-07-27 16:06:16.000000 lmfitxps-1.3.0/tests/test_backgrounds.py
```

### Comparing `lmfitxps-1.2.0/LICENSE` & `lmfitxps-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmfitxps-1.2.0/PKG-INFO` & `lmfitxps-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmfitxps
-Version: 1.2.0
+Version: 1.3.0
 Summary: This package contains additional models for the lmfit package for fitting XPS spectra.
 Author-email: Julian Hochhaus <julian.hochhaus@tu-dortmund.de>
 License: MIT License
         
         Copyright (c) 2023 Julian-Hochhaus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lmfitxps-1.2.0/README.md` & `lmfitxps-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lmfitxps-1.2.0/lmfitxps/backgrounds.py` & `lmfitxps-1.3.0/lmfitxps/backgrounds.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 __author__ = "Julian Andreas Hochhaus"
 __copyright__ = "Copyright 2023"
 __credits__ = ["Julian Andreas Hochhaus"]
 __license__ = "MIT"
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 __maintainer__ = "Julian Andreas Hochhaus"
 __email__ = "julian.hochhaus@tu-dortmund.de"
 
 def tougaard_closure():
     bgrnd = [[], [], []]  # This will act as the closure to store the precalculated data
-    def tougaard(x, y, B, C, C_d, D, extend=30, only_vary_B=True):
+    def tougaard(x, y, B, C, C_d, D, extend=30):
         """
                 Calculates the Tougaard background of an X-ray photoelectron spectroscopy (XPS) spectrum.
 
                 The following implementation is based on the four-parameter loss function (4-PIESCS)
                 as suggested by [R.Hesse](
                 https://doi.org/10.1002/sia.3746). In contrast to R.Hesse, the Tougaard background is not leveled with the data
                 using a constant, but the background on the high-energy side is extended. This approach was found to lead to
@@ -57,15 +57,15 @@
                     The Tougaard background of the XPS spectrum.
 
                 See Also ------- The following implementation is based on the four-parameter loss function as suggested by
                 R.Hesse [https://doi.org/10.1002/sia.3746].
                 """
         nonlocal bgrnd
 
-        if np.array_equal(bgrnd[0], y) and only_vary_B and bgrnd[2][0] == extend:
+        if np.array_equal(bgrnd[0], y) and bgrnd[2][0] == extend:
             # Check if loss function was already calculated
             return [B * elem for elem in bgrnd[1]]
         else:
             bgrnd[0] = y
             bgrnd[2] = [extend]
             bg = []
             delta_x = abs((x[-1] - x[0]) / len(x))
@@ -78,15 +78,14 @@
                 for j in range(len(padded_y[k:])):
                     padded_x_kj = padded_x[k + j]
                     bg_temp += (padded_x_kj - x_k) / ((C + C_d * (padded_x_kj - x_k) ** 2) ** 2
                                                       + D * (padded_x_kj - x_k) ** 2) * padded_y[k + j] * delta_x
                 bg.append(bg_temp)
             bgrnd[1] = bg
             return np.asarray([B * elem for elem in bgrnd[1]])
-
     return tougaard
 
 # Create the tougaard function with the closure
 tougaard = tougaard_closure()
 
 def shirley(y, k, const):
     """
@@ -160,91 +159,72 @@
         y (array-like): The y-values of the data.
         tol (float, optional): Tolerance for convergence. Defaults to 1e-5.
         maxit (int, optional): Maximum number of iterations. Defaults to 10.
 
     Returns:
         array: The Shirley background calculated from the input data.
     """
-    # Make sure we've been passed arrays and not lists.
-    x = np.array(x)
-    y = np.array(y)
 
+    n = len(y)
     # Sanity check: Do we actually have data to process here?
-    if not (np.any(x) and np.any(y)):
+    # print(any(x), any(y), (any(x) and any(y)))
+    if not (any(x) and any(y)):
         print("One of the arrays x or y is empty. Returning zero background.")
-        return np.asarray(x * 0)
+        return x * 0
 
     # Next ensure the energy values are *decreasing* in the array,
     # if not, reverse them.
     if x[0] < x[-1]:
         is_reversed = True
         x = x[::-1]
         y = y[::-1]
     else:
         is_reversed = False
 
-    # Locate the biggest peak.
-    maxidx = np.abs(y - y.max()).argmin()
-
-    # It's possible that maxidx will be 0 or -1. If that is the case,
-    # we can't use this algorithm, we return a zero background.
-    if maxidx == 0 or maxidx >= len(y) - 1:
-        print("Boundaries too high for algorithm: returning a zero background.")
-        return np.asarray(x * 0)
-
-    # Locate the minima either side of maxidx.
-    lmidx = np.abs(y[0:maxidx] - y[0:maxidx].min()).argmin()
-    rmidx = np.abs(y[maxidx:] - y[maxidx:].min()).argmin() + maxidx
-
-    xl = x[lmidx]
-    yl = y[lmidx]
-    xr = x[rmidx]
-    yr = y[rmidx]
-
-    # Max integration index
-    imax = rmidx - 1
+    yl = y[0]
+    yr = y[-1]
 
     # Initial value of the background shape B. The total background S = yr + B,
     # and B is equal to (yl - yr) below lmidx and initially zero above.
     B = y * 0
-    B[:lmidx] = yl - yr
+
     Bnew = B.copy()
 
     it = 0
     while it < maxit:
         # Calculate new k = (yl - yr) / (int_(xl)^(xr) J(x') - yr - B(x') dx')
         ksum = 0.0
-        for i in range(lmidx, imax):
+        for i in range(n - 1):
             ksum += (x[i] - x[i + 1]) * 0.5 * (y[i] + y[i + 1] - 2 * yr - B[i] - B[i + 1])
         k = (yl - yr) / ksum
-
         # Calculate new B
-        for i in range(lmidx, rmidx):
+        for i in range(n):
             ysum = 0.0
-            for j in range(i, imax):
+            for j in range(i, n - 1):
                 ysum += (x[j] - x[j + 1]) * 0.5 * (y[j] + y[j + 1] - 2 * yr - B[j] - B[j + 1])
             Bnew[i] = k * ysum
-
         # If Bnew is close to B, exit.
+        # if norm(Bnew - B) < tol:
         B = Bnew - B
+        # print(it, (B**2).sum(), tol**2)
         if (B ** 2).sum() < tol ** 2:
             B = Bnew.copy()
             break
         else:
             B = Bnew.copy()
         it += 1
 
     if it >= maxit:
         print("Max iterations exceeded before convergence.")
-
     if is_reversed:
-        return np.asarray((yr + B)[::-1])
+        # print("Shirley BG: tol (ini = ", tol, ") , iteration (max = ", maxit, "): ", it)
+        return (yr + B)[::-1]
     else:
-        return np.asarray(yr + B)
-
+        # print("Shirley BG: tol (ini = ", tol, ") , iteration (max = ", maxit, "): ", it)
+        return yr + B
 
 
 def tougaard_calculate(x, y, tb=2866, tc=1643, tcd=1, td=1, maxit=100):
     """
     Calculate the Tougaard background for a given set of x and y data. Inspired from https://warwick.ac.uk/fac/sci/physics/research/condensedmatt/surface/people/james_mudd/igor/
 
     Args:
```

### Comparing `lmfitxps-1.2.0/lmfitxps/lineshapes.py` & `lmfitxps-1.3.0/lmfitxps/lineshapes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from lmfit.lineshapes import doniach, gaussian, thermal_distribution
 from scipy.signal import convolve as sc_convolve
 __author__ = "Julian Andreas Hochhaus"
 __copyright__ = "Copyright 2023"
 __credits__ = ["Julian Andreas Hochhaus"]
 __license__ = "MIT"
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 __maintainer__ = "Julian Andreas Hochhaus"
 __email__ = "julian.hochhaus@tu-dortmund.de"
 
 def dublett(x, amplitude, sigma, gamma, gaussian_sigma, center, soc, height_ratio, fct_coster_kronig):
     """
     Calculates the convolution of a Doniach-Sunjic Dublett with a Gaussian. Thereby, the Gaussian acts as the
     convolution kernel.
```

### Comparing `lmfitxps-1.2.0/lmfitxps/models.py` & `lmfitxps-1.3.0/lmfitxps/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import numpy as np
 from lmfit.lineshapes import doniach, gaussian, thermal_distribution
-from lineshapes import singlett, dublett, fermi_edge, convolve, fft_convolve
-from backgrounds import tougaard, slope, shirley
+from .lineshapes import singlett, dublett, fermi_edge, convolve, fft_convolve
+from .backgrounds import tougaard, slope, shirley
 from lmfit import Model
+import lmfit
 from lmfit.models import guess_from_peak
 from scipy.signal import convolve as sc_convolve
 
 __author__ = "Julian Andreas Hochhaus"
 __copyright__ = "Copyright 2023"
 __credits__ = ["Julian Andreas Hochhaus"]
 __license__ = "MIT"
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 __maintainer__ = "Julian Andreas Hochhaus"
 __email__ = "julian.hochhaus@tu-dortmund.de"
 
 
 class ConvGaussianDoniachSinglett(lmfit.model.Model):
     __doc__ = "Model of a Doniach dublett profile convoluted with a gaussian. " \
               "See also lmfit->lineshape.gaussian and lmfit->lineshape.doniach." + lmfit.models.COMMON_INIT_DOC
```

### Comparing `lmfitxps-1.2.0/lmfitxps.egg-info/PKG-INFO` & `lmfitxps-1.3.0/lmfitxps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmfitxps
-Version: 1.2.0
+Version: 1.3.0
 Summary: This package contains additional models for the lmfit package for fitting XPS spectra.
 Author-email: Julian Hochhaus <julian.hochhaus@tu-dortmund.de>
 License: MIT License
         
         Copyright (c) 2023 Julian-Hochhaus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

