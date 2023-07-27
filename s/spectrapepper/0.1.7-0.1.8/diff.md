# Comparing `tmp/spectrapepper-0.1.7.tar.gz` & `tmp/spectrapepper-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrapepper-0.1.7.tar", last modified: Mon Nov 21 14:38:36 2022, max compression
+gzip compressed data, was "spectrapepper-0.1.8.tar", last modified: Thu Jul 27 10:30:04 2023, max compression
```

## Comparing `spectrapepper-0.1.7.tar` & `spectrapepper-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-11-21 14:38:36.802890 spectrapepper-0.1.7/
--rw-rw-rw-   0        0        0     1124 2021-09-16 07:59:43.000000 spectrapepper-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      158 2021-06-21 08:07:31.000000 spectrapepper-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     5240 2022-11-21 14:38:36.802890 spectrapepper-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4288 2022-06-07 13:22:05.000000 spectrapepper-0.1.7/README.md
--rw-rw-rw-   0        0        0     4328 2022-06-07 13:24:07.000000 spectrapepper-0.1.7/README.rst
--rw-rw-rw-   0        0        0       50 2022-11-21 14:00:09.000000 spectrapepper-0.1.7/requirements.txt
--rw-rw-rw-   0        0        0      458 2022-11-21 14:38:36.807890 spectrapepper-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     2173 2022-11-21 12:44:17.000000 spectrapepper-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-21 14:38:36.765392 spectrapepper-0.1.7/spectrapepper/
--rw-rw-rw-   0        0        0      314 2022-11-21 11:54:22.000000 spectrapepper-0.1.7/spectrapepper/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-21 14:38:36.801389 spectrapepper-0.1.7/spectrapepper/datasets/
--rw-rw-rw-   0        0        0    65800 2021-01-25 13:28:57.000000 spectrapepper-0.1.7/spectrapepper/datasets/params.txt
--rw-rw-rw-   0        0        0  1683763 2020-11-11 10:28:55.000000 spectrapepper-0.1.7/spectrapepper/datasets/spectras.txt
--rw-rw-rw-   0        0        0     1506 2020-09-15 12:23:07.000000 spectrapepper-0.1.7/spectrapepper/datasets/targets.txt
--rw-rw-rw-   0        0        0   119551 2022-11-21 10:53:23.000000 spectrapepper-0.1.7/spectrapepper/functions.py
-drwxrwxrwx   0        0        0        0 2022-11-21 14:38:36.789390 spectrapepper-0.1.7/spectrapepper.egg-info/
--rw-rw-rw-   0        0        0     5240 2022-11-21 14:38:36.000000 spectrapepper-0.1.7/spectrapepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2022-11-21 14:38:36.000000 spectrapepper-0.1.7/spectrapepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       46 2022-11-21 14:38:36.000000 spectrapepper-0.1.7/spectrapepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-04-26 13:02:10.000000 spectrapepper-0.1.7/spectrapepper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2022-11-21 14:38:36.000000 spectrapepper-0.1.7/spectrapepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-11-21 14:38:36.000000 spectrapepper-0.1.7/spectrapepper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 10:30:04.533081 spectrapepper-0.1.8/
+-rw-rw-rw-   0        0        0     1124 2021-09-16 07:59:43.000000 spectrapepper-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      158 2021-06-21 08:07:31.000000 spectrapepper-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5213 2023-07-27 10:30:04.533081 spectrapepper-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4283 2022-11-22 09:25:50.000000 spectrapepper-0.1.8/README.md
+-rw-rw-rw-   0        0        0     4321 2022-11-22 09:08:46.000000 spectrapepper-0.1.8/README.rst
+-rw-rw-rw-   0        0        0      164 2022-02-13 18:34:42.000000 spectrapepper-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       50 2022-11-21 14:00:09.000000 spectrapepper-0.1.8/requirements.txt
+-rw-rw-rw-   0        0        0      458 2023-07-27 10:30:04.533081 spectrapepper-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2173 2023-07-27 09:56:43.000000 spectrapepper-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:30:04.417185 spectrapepper-0.1.8/spectrapepper/
+-rw-rw-rw-   0        0        0      314 2023-07-27 09:57:14.000000 spectrapepper-0.1.8/spectrapepper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:30:04.533081 spectrapepper-0.1.8/spectrapepper/datasets/
+-rw-rw-rw-   0        0        0    65800 2021-01-25 13:28:57.000000 spectrapepper-0.1.8/spectrapepper/datasets/params.txt
+-rw-rw-rw-   0        0        0  1683763 2020-11-11 10:28:55.000000 spectrapepper-0.1.8/spectrapepper/datasets/spectras.txt
+-rw-rw-rw-   0        0        0     1506 2020-09-15 12:23:07.000000 spectrapepper-0.1.8/spectrapepper/datasets/targets.txt
+-rw-rw-rw-   0        0        0   114245 2023-07-27 10:04:51.000000 spectrapepper-0.1.8/spectrapepper/functions.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:30:04.479671 spectrapepper-0.1.8/spectrapepper.egg-info/
+-rw-rw-rw-   0        0        0     5213 2023-07-27 10:30:04.000000 spectrapepper-0.1.8/spectrapepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-07-27 10:30:04.000000 spectrapepper-0.1.8/spectrapepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       46 2023-07-27 10:30:04.000000 spectrapepper-0.1.8/spectrapepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-04-26 13:02:10.000000 spectrapepper-0.1.8/spectrapepper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       43 2023-07-27 10:30:04.000000 spectrapepper-0.1.8/spectrapepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-27 10:30:04.000000 spectrapepper-0.1.8/spectrapepper.egg-info/top_level.txt
```

### Comparing `spectrapepper-0.1.7/LICENSE` & `spectrapepper-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrapepper-0.1.7/PKG-INFO` & `spectrapepper-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: spectrapepper
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package to simplify and accelerate analysis of spectroscopy data
 Home-page: https://github.com/spectrapepper/spectrapepper
 Author: spectrapepper
 Author-email: spectrapepper@gmail.com
 License: MIT license
 Keywords: spectrapepper
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -24,22 +23,23 @@
 <center>
     <img src="https://raw.githubusercontent.com/spectrapepper/spectrapepper/main/docs/_static/spectrapepperlogo-alt.png" width="50%">
 </center>
 
 [![image](https://img.shields.io/pypi/v/spectrapepper.svg)](https://pypi.python.org/pypi/spectrapepper)
 [![image](https://img.shields.io/conda/vn/conda-forge/spectrapepper.svg)](https://anaconda.org/conda-forge/spectrapepper)
 [![image](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![image](https://img.shields.io/lgtm/grade/python/g/spectrapepper/spectrapepper.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/spectrapepper/spectrapepper/context:python)
+[![CodeQL](https://github.com/spectrapepper/spectrapepper/actions/workflows/codeql.yml/badge.svg)](https://github.com/spectrapepper/spectrapepper/actions/workflows/codeql.yml)
 [![image](https://github.com/spectrapepper/spectrapepper/workflows/docs/badge.svg)](https://spectrapepper.github.io/spectrapepper)
 [![codecov](https://codecov.io/gh/spectrapepper/spectrapepper/branch/main/graph/badge.svg?token=DC0QIwuYel)](https://codecov.io/gh/spectrapepper/spectrapepper)
 [![Downloads](https://static.pepy.tech/personalized-badge/spectrapepper?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=pypi%20downloads)](https://pepy.tech/project/spectrapepper)
 [![image](https://img.shields.io/conda/dn/conda-forge/spectrapepper?color=blue&label=conda%20downloads)](https://anaconda.org/conda-forge/spectrapepper)
 [![image](https://img.shields.io/badge/stackoverflow-Ask%20a%20question-brown?logo=stackoverflow&logoWidth=18&logoColor=white)](https://stackoverflow.com/questions/tagged/spectrapepper)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03781/status.svg)](https://doi.org/10.21105/joss.03781)
 
+
 **A Python package to simplify and accelerate analysis of spectroscopy data.**
 
 * GitHub repo: https://github.com/spectrapepper/spectrapepper
 * Documentation: https://spectrapepper.github.io/spectrapepper
 * PyPI: https://pypi.python.org/pypi/spectrapepper
 * Conda-forge: https://anaconda.org/conda-forge/spectrapepper
 * Free software: MIT license
@@ -103,9 +103,7 @@
         conda remove spectrapepper
 
 
 # Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the
 [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
-
-
```

### Comparing `spectrapepper-0.1.7/README.md` & `spectrapepper-0.1.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 <center>
     <img src="https://raw.githubusercontent.com/spectrapepper/spectrapepper/main/docs/_static/spectrapepperlogo-alt.png" width="50%">
 </center>
 
 [![image](https://img.shields.io/pypi/v/spectrapepper.svg)](https://pypi.python.org/pypi/spectrapepper)
 [![image](https://img.shields.io/conda/vn/conda-forge/spectrapepper.svg)](https://anaconda.org/conda-forge/spectrapepper)
 [![image](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![image](https://img.shields.io/lgtm/grade/python/g/spectrapepper/spectrapepper.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/spectrapepper/spectrapepper/context:python)
+[![CodeQL](https://github.com/spectrapepper/spectrapepper/actions/workflows/codeql.yml/badge.svg)](https://github.com/spectrapepper/spectrapepper/actions/workflows/codeql.yml)
 [![image](https://github.com/spectrapepper/spectrapepper/workflows/docs/badge.svg)](https://spectrapepper.github.io/spectrapepper)
 [![codecov](https://codecov.io/gh/spectrapepper/spectrapepper/branch/main/graph/badge.svg?token=DC0QIwuYel)](https://codecov.io/gh/spectrapepper/spectrapepper)
 [![Downloads](https://static.pepy.tech/personalized-badge/spectrapepper?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=pypi%20downloads)](https://pepy.tech/project/spectrapepper)
 [![image](https://img.shields.io/conda/dn/conda-forge/spectrapepper?color=blue&label=conda%20downloads)](https://anaconda.org/conda-forge/spectrapepper)
 [![image](https://img.shields.io/badge/stackoverflow-Ask%20a%20question-brown?logo=stackoverflow&logoWidth=18&logoColor=white)](https://stackoverflow.com/questions/tagged/spectrapepper)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03781/status.svg)](https://doi.org/10.21105/joss.03781)
 
+
 **A Python package to simplify and accelerate analysis of spectroscopy data.**
 
 * GitHub repo: https://github.com/spectrapepper/spectrapepper
 * Documentation: https://spectrapepper.github.io/spectrapepper
 * PyPI: https://pypi.python.org/pypi/spectrapepper
 * Conda-forge: https://anaconda.org/conda-forge/spectrapepper
 * Free software: MIT license
```

### Comparing `spectrapepper-0.1.7/README.rst` & `spectrapepper-0.1.8/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 .. image:: https://img.shields.io/pypi/v/spectrapepper.svg
         :target: https://pypi.python.org/pypi/spectrapepper
 .. image:: https://img.shields.io/conda/vn/conda-forge/spectrapepper.svg
         :target: https://anaconda.org/conda-forge/spectrapepper
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
         :target: https://opensource.org/licenses/MIT
-.. image:: https://img.shields.io/lgtm/grade/python/g/spectrapepper/spectrapepper.svg?logo=lgtm&logoWidth=18
-        :target: https://lgtm.com/projects/g/spectrapepper/spectrapepper/context:python
+.. image:: https://github.com/spectrapepper/spectrapepper/actions/workflows/codeql.yml/badge.svg
+        :target: https://github.com/spectrapepper/spectrapepper/actions/workflows/codeql.yml
 .. image:: https://github.com/spectrapepper/spectrapepper/workflows/docs/badge.svg
         :target: https://spectrapepper.github.io/spectrapepper
 .. image:: https://codecov.io/gh/spectrapepper/spectrapepper/branch/main/graph/badge.svg?token=DC0QIwuYel
         :target: https://codecov.io/gh/spectrapepper/spectrapepper
 .. image:: https://img.shields.io/conda/dn/conda-forge/spectrapepper.svg?color=blue&label=conda%20downloads
         :target: https://pepy.tech/project/spectrapepper
 .. image:: https://static.pepy.tech/personalized-badge/spectrapepper?period=total&units=international_system&left_color=grey&left_text=pypi%20downloads&right_color=blue
```

### Comparing `spectrapepper-0.1.7/setup.py` & `spectrapepper-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     keywords='spectrapepper',
     name='spectrapepper',
     packages=find_packages(include=['spectrapepper', 'spectrapepper.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/spectrapepper/spectrapepper',
-    version='0.1.7',
+    version='0.1.8',
     zip_safe=False,
     package_data={'spectrapepper': ['datasets/headers.txt',
                                     'datasets/mapping1.txt',
                                     'datasets/mapping2.txt',
                                     'datasets/params.txt',
                                     'datasets/spectras.txt',
                                     'datasets/targets.txt']}
```

### Comparing `spectrapepper-0.1.7/spectrapepper/datasets/params.txt` & `spectrapepper-0.1.8/spectrapepper/datasets/params.txt`

 * *Files identical despite different names*

### Comparing `spectrapepper-0.1.7/spectrapepper/datasets/spectras.txt` & `spectrapepper-0.1.8/spectrapepper/datasets/spectras.txt`

 * *Files identical despite different names*

### Comparing `spectrapepper-0.1.7/spectrapepper/datasets/targets.txt` & `spectrapepper-0.1.8/spectrapepper/datasets/targets.txt`

 * *Files identical despite different names*

### Comparing `spectrapepper-0.1.7/spectrapepper/functions.py` & `spectrapepper-0.1.8/spectrapepper/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 """
 This main module contains all the functions available in spectrapepper. Please
 use the search function to look up specific functionalities and keywords.
 """
 
-import math
-import copy
-import random
-import numpy as np
-import pandas as pd
-from scipy import sparse
-from scipy import interpolate
-from scipy.special import gamma
-from scipy.stats import stats
-from scipy.signal import butter, filtfilt
-from scipy.optimize import minimize
+from matplotlib.colors import LinearSegmentedColormap
 from scipy.interpolate import splev, splrep
+from scipy.signal import butter, filtfilt
 from scipy.sparse.linalg import spsolve
-import itertools
+import matplotlib.gridspec as gridspec
+from matplotlib.lines import Line2D
+from scipy.optimize import minimize
 from itertools import combinations
+import matplotlib.pyplot as plt
+from scipy.special import gamma
+from scipy import interpolate
+from scipy.stats import stats
 import statistics as sta
 import matplotlib as mpl
-import matplotlib.pyplot as plt
-import matplotlib.gridspec as gridspec
-from matplotlib.colors import LinearSegmentedColormap
-from matplotlib.lines import Line2D
+import statistics as sta
+from scipy import sparse
+import pandas as pd
+import numpy as np
 import linecache
+import itertools
 import os.path
+import random
+import math
+import copy
 import os
 
 
 def load_spectras(sample=None):
     """
     Load sample specrtal data, axis included in the first line.
-    
+
     :type sample: int, tuple
     :param sample: Index of the sample spectra wanted or a tuple with the range
         of the indeces of a groups of spectras.
-    
+
     :returns: X axis and the sample spectral data selected.
     :rtype: list[float], list[float]
     """ 
     location = os.path.dirname(os.path.realpath(__file__))
     my_file = os.path.join(location, 'datasets', 'spectras.txt')
     data = load(my_file)
     x = data[0]
-    y = [list(i) for i in data[1:]]
+    y = data[1:]
     
-    dims = len(np.array(sample).shape)
-    
-    if dims == 1:
+    if isinstance(sample, tuple):
         y = y[sample[0]: sample[1]]
-    if dims == 0 and sample is not None:
+    elif isinstance(sample, int):
         y = y[sample]
     
     return x, y
 
 
 def load_targets(flatten=True):
     """
@@ -88,84 +87,74 @@
     
     if transpose:
         data = np.transpose(data)
     
     return data
 
 
-def load(file, fromline=0, line=None, transpose=False, dtype=float, split=False):
+def load(file, fromline=0, toline=None, line=None, transpose=False, dtype=float, 
+          separators=[";"], blanks=["NaN", "nan", "--"], replacewith="0"):
     """
-    Load data from a standard text file obtained from LabSpec and other
-    spectroscopy instruments. Normally, when single measurement these come in 
+    Load data from a text file obtained from LabSpec and other
+    spectroscopy software. Normally, single measurements come in 
     columns with the first one being the x-axis. When it is a mapping, the
     first row is the x-axis and the following are the measurements. It can also
-    perofrm random access toa particular ´line´.
+    peroform random access to a particular ´line´ and also it is possibel to define
+    specific range to load with 'fromline' and 'toline'.
     
     :type file: str
     :param file: Url of data file. Must not have headers and separated by 
         'spaces' (LabSpec).
     
     :type fromline: int
     :param fromline: Line of file from which to start loading data. The default
         is 0.
+
+    :type toline: int
+    :param fromline: Line of file to which to end loading data. The default
+        is 'None' which idicates the full range of data.
     
     :type line: int
     :param line: Random access to file. Loads a specific line in a file. Default
         is ´None´.
     
     :type transpose: boolean
     :param transpose: If True transposes the data. Default is False.
     
     :type dtype: str
     :param dtype: Type of data. If its numeric then 'float', if text then 'string'.
         Default is 'float'.
-    
-    :type split: boolean
-    :param split: True to make a list of strings when 'dtype' is 'string', 
-        separated by space. The default is False.
-    
+        
     :returns: List of the data.
     :rtype: list[float]
     """
+    
     new_data = []
+    def process_row(row, dtype):
+        for i in separators:
+            row = row.replace(i, " ")
+        for i in blanks:
+            row = row.replace(i, replacewith)
+
+        row = str.split(row)
+        return np.array(row, dtype=dtype)
+    
     with open(file, 'r') as raw_data:
-        # raw_data = open(file, "r")
-        i = 0
-        
         if line is not None:
-            line = int(line) + 1
-            file = str(file)
-            info = linecache.getline(file, line)
-            
-            if dtype == 'float':
-                info = info.replace("NaN", "-1")
-                info = info.replace("nan", "-1")
-                info = info.replace("--", "-1")
-                info = str.split(info)
-                info = np.array(info, dtype=float)
-    
-            if dtype == 'string':
-                if split:
-                        info = str.split(info)
-                info = np.array(info, dtype=str)
-                
-        elif line is None:
-            for row in raw_data:
+            new_data = linecache.getline(file, line+1)
+            new_data = process_row(new_data, dtype)
+        else:
+            new_data = []
+            for i, row in enumerate(raw_data):
                 if i >= fromline:
-                    # row = row.replace(",", ".")
-                    row = row.replace(";", " ")
-                    row = row.replace("NaN", "-1")
-                    row = row.replace("nan", "-1")
-                    row = row.replace("--", "-1")
-                    s_row = str.split(row)
-                    s_row = np.array(s_row, dtype=dtype)
+                    if toline is not None and i > toline:
+                        break
+                    s_row = process_row(row, dtype)
                     new_data.append(s_row)
-                i += 1
-            # raw_data.close()
-        
+
         if transpose:
             new_data = np.transpose(new_data)
 
     return new_data
 
 
 def lowpass(y, cutoff=0.25, fs=30, order=2, nyq=0.75):
@@ -206,47 +195,44 @@
         y = y[0]
     
     return y
 
 
 def normtomax(y, to=1, zeromin=False):
     """
-    Normalizes spectras to the maximum value of each, in other words, the
-    maximum value of each spectras is set to 1.
+    Normalizes spectra to the maximum value of each, in other words, the
+    maximum value of each spectra is set to the specified value.
 
-    :type y: list[float]
+    :type y: list[float], numpy.ndarray
     :param y: Single or multiple vectors to normalize.
-    
+
     :type to: float
     :param to: value to which normalize to. Default is 1.
-    
+
     :type zeromin: boolean
-    :param zeromin: If `True`, the minimum value is traslated to 0. Default
-        values is `False`
-    
+    :param zeromin: If `True`, the minimum value is translated to 0. Default
+        value is `False`
+
     :returns: Normalized data.
-    :rtype: list[float]
+    :rtype: list[float], numpy.ndarray
     """
-    y = copy.deepcopy(y)  # so it does not chamge the input list
-    dims = len(np.array(y).shape)  # detect dimensions
-    
+    y = copy.deepcopy(y)
+
+    dims = len(np.array(y).shape)
     if dims == 1:
         y = [y]
-    
-    for i in range(len(y)):           
-        if zeromin:
-            min_data = min(y[i])
-            y[i] = y[i] - min_data
-        max_data = max(y[i])
 
-        y[i] = to*np.array(y[i])/max_data
+    for i in range(len(y)):
+        if zeromin:
+            y[i] = y[i] - np.min(y[i])
+        y[i] = y[i] / np.max(y[i]) * to
 
     if dims == 1:
         y = y[0]
-    
+
     return y
 
 
 def normtovalue(y, val):
     """
     Normalizes the spectras to a set value, in other words, the defined value
     will be reescaled to 1 in all the spectras.
@@ -348,29 +334,27 @@
     :returns: The baseline.
     :rtype: list[float]
     """
     data = copy.deepcopy(y)
     x = list(x)
     points = list(points)
     pos = valtoind(points, x)
-    avg = int(avg)
     dims = len(np.array(data).shape)
 
     if len(np.array(points).shape) == 2:
         avg = 0
     else:
         pos = [[i, i] for i in pos]
         points = [[i, i] for i in points]
 
     if dims == 1:
         data = [data]
     
     baseline = []
     result = []
-    
     for j in range(len(data)):
         y_p = []
         for i in range(len(pos)):
             temp = np.mean(data[j][pos[i][0] - avg: pos[i][1] + avg + 1])
             y_p.append(temp)
         
         points = [np.mean(i) for i in points]
@@ -475,50 +459,27 @@
     :type x: list[float]
     :param x: Axis.
 
     :returns: Index, or position, in the axis of the values in vals
     :rtype: list[int], int
     """
     vals = copy.deepcopy(vals)
-    shape = len(np.array(vals).shape)
-    
-    if shape > 1:
-        pos = [[0 for _ in range(len(vals[0]))] for _ in range(len(vals))]  # i position of area limits
-        for i in range(len(vals)):  # this loop takes the approx. x and takes its position
-            for j in range(len(vals[0])):
-                dif_temp = 999  # safe initial difference
-                temp_pos = 0  # temporal best position
-                for k in range(len(x)):  # search in axis
-                    if abs(vals[i][j] - x[k]) < dif_temp:  # compare if better
-                        temp_pos = k  # save best value
-                        dif_temp = abs(vals[i][j] - x[k])  # calculate new diff
-                vals[i][j] = x[temp_pos]  # save real value in axis
-                pos[i][j] = temp_pos  # save the position
-                
-    if shape == 1:
-        pos = [0 for _ in range(len(vals))]  # i position of area limits
-        for i in range(len(vals)):  # this loop takes the approx. x and takes its position
-            dif_temp = 999  # safe initial difference
-            temp_pos = 0  # temporal best position
-            for k in range(len(x)):  # search in axis
-                if abs(vals[i] - x[k]) < dif_temp:  # compare if better
-                    temp_pos = k  # save best value
-                    dif_temp = abs(vals[i] - x[k])  # calculate new diff
-            vals[i] = x[temp_pos]  # save real value in axis
-            pos[i] = temp_pos  # save the position           
-                
-    if shape == 0:
-        dif_temp = 9999999  # safe initial difference
-        temp_pos = 0  # temporal best position
-        for k in range(len(x)):
-            if abs(vals - x[k]) < dif_temp:
-                temp_pos = k
-                dif_temp = abs(vals - x[k])
-        vals = x[temp_pos]  # save real value in axis
-        pos = temp_pos
+    x_np = np.array(x)
+    vals_np = np.array(vals)
+    shape_dim = vals_np.ndim
+    
+    if shape_dim > 1:
+        pos = [[np.argmin(np.abs(x_np - val)) for val in val_row] for val_row in vals_np]
+    elif shape_dim == 1:
+        pos = [np.argmin(np.abs(x_np - val)) for val in vals_np]
+        vals[:] = [x_np[p] for p in pos]
+    elif shape_dim == 0:
+        pos = np.argmin(np.abs(x_np - vals_np))
+        vals = x_np[pos]
+        
     return pos
 
 
 def areacalculator(y, x, limits, norm=False):
     """
     Area calculator using the data (x_data) and the limits in position, not
     values.
@@ -543,26 +504,27 @@
 
     if len(np.array(limits).shape) == 1:
         limits = [limits]
 
     if dims == 1:
         y = [y]
 
-    areas = [[0 for _ in range(len(limits))] for _ in range(len(y))]  # final values of areas
-    
-    for i in range(len(y)):  # calculate the areas for all the points
-        for j in range(len(limits)):  # for all the areas
-            areas[i][j] = np.sum(y[i][limits[j][0]:limits[j][1]])  # calculate the sum
-            if norm:
-                areas[i][j] = areas[i][j] / np.sum(y[i])
+    areas = np.zeros((len(y), len(limits)))
+    y = np.array(y)
+    for j, (start, end) in enumerate(limits):
+        areas[:, j] = y[:, start:end].sum(axis=1)
+
+    # Normalize if necessary
+    if norm:
+        areas /= y.sum(axis=1)[:, np.newaxis]
 
     if dims == 1:
         areas = areas[0]
     
-    return areas
+    return areas.tolist()
 
 
 def bincombs(n, s_min=1, s_max=0):
     """
     Returns all possible unique combinations.
 
     :type n: int
@@ -620,33 +582,33 @@
     :param lims: Limits of the vector to normalize the sum. Default is `None`.
         For example, if ´lims = [N, M]´, the the sum under the curve betwween
         N and M is normalized to 1.
 
     :returns: Normalized data
     :rtype: list[float]
     """
-    y = copy.deepcopy(y)
-    dims = len(np.array(y).shape)
-    if x is not None:
-        pos = valtoind(lims, x)
-    
+    y = np.array(y, copy=True)
+    dims = y.ndim
+
     if dims == 1:
-        y = [y]
-    
-    for i in range(len(y)):
-        if lims is None:
-            s = sum(y[i])
-        else:
-            s = sum(y[i][pos[0]:pos[1]])
-        
-        for j in range(len(y[i])):
-            y[i][j] = y[i][j] / s
+        y = y.reshape(1, -1)
+
+    if x is None:
+        x = np.arange(y.shape[1])
+
+    if lims is None:
+        pos = [0, y.shape[1]]
+    else:
+        pos = valtoind(lims, x)
+
+    s = y[:, pos[0]:pos[1]].sum(axis=1)
+    y = y / s[:, np.newaxis]
     
     if dims == 1:
-        y = y[0]
+        y = y.ravel()
     
     return y
 
 
 def normtoratio(y, r1, r2, x=None):
     """
     Normalizes a peak to the ratio value respect to another. That is, the peak
@@ -664,79 +626,64 @@
     :type x: list[float]
     :param x: Axis of the data. If `None` then it goes from 0 to N, where
         N is the length of the spectras.
 
     :returns: Normalized data
     :rtype: list[float]
     """
-    y = copy.deepcopy(y)
-    dims = len(np.array(y).shape)
-    
+    y = np.array(y, copy=True)
+    dims = y.ndim
+
     if dims == 1:
-        y = [y]
-    
+        y = y.reshape(1, -1)
+
     if x is None:
         r1, r2 = r1, r2
     else:
         r1 = valtoind(r1, x)
         r2 = valtoind(r2, x)
-    
-    for i in range(len(y)):
-        a1 = sum(y[i][r1[0]:r1[1]])
-        a2 = sum(y[i][r2[0]:r2[1]])
-        ratio = a1/(a1+a2)
-        m = ratio/max(y[i])
-        y[i] = np.array(y[i])*m
+
+    a1 = y[:, r1[0]:r1[1]].sum(axis=1)
+    a2 = y[:, r2[0]:r2[1]].sum(axis=1)
+    ratio = a1/(a1+a2)
+    m = ratio[:, np.newaxis]/y.max(axis=1)[:, np.newaxis]
+    y = y * m
     
     if dims == 1:
-        y = y[0]
+        y = y.ravel()
     
-    return list(y)
+    return y.tolist()
 
 
 def normtoglobalmax(y, globalmin=False):
     """
     Normalizes a list of spectras to the global max.
 
     :type y: list[float]
     :param y: List of spectras.
 
     :type globalmin: Bool
     :param globalmin: If `True`, the global minimum is reescaled to 0. Default
         is `False`.
 
-
     :returns: Normalized data
     :rtype: list[float]
     """
-    y = copy.deepcopy(y)
-    dims = len(np.array(y).shape)
+    y = np.array(y, copy=True)
+    dims = y.ndim
     if dims > 1:
-        maximum = -999999999  # safe start
-        
-        if globalmin==True:
-            minimum = 999999999
-        else:
-            minimum = 0
-            
-        for i in range(len(y)):
-            for j in range(len(y[0])):
-                if y[i][j] > maximum:
-                    maximum = y[i][j]
-                if y[i][j] < minimum and globalmin==True:
-                    minimum = y[i][j]
-        
-        if globalmin==True:
-            for i in range(len(y)):
-                for j in range(len(y[0])):
-                    y[i][j] -= minimum
-        
-        y = normtovalue(y, (maximum-minimum))
-    else:  # if s single vector, then is the same as nortomax (local)
-        y = normtomax(y, zeromin=globalmin)
+        y_min, y_max = y.min(), y.max()
+        if globalmin:
+            y = y - y_min
+        y = y / (y_max - y_min)
+    else:
+        y_min, y_max = y.min(), y.max()
+        if globalmin:
+            y = y - y_min
+        y = y / y_max
     return y
 
 
 def normtoglobalsum(y):
     """
     Normalizes a list of spectras to the global max sum under the curve. In 
         other words, looks to the largest sum under the curve and sets it to 1,
@@ -744,27 +691,22 @@
 
     :type y: list[float]
     :param y: List of spectras.
 
     :returns: Normalized data
     :rtype: list[float]
     """
-    y = copy.deepcopy(y)
-    dims = len(np.array(y).shape)
+    y = np.array(y, copy=True)
+    dims = y.ndim
     if dims > 1:
-        sums = []
-        for i in y:
-            sums.append(sum(i))
-        maxsum = max(sums)
-        
-        for i in range(len(y)):
-            y[i] = y[i] / maxsum
-        
-    else:  # if s single vector, then is the same as normtomax (local)
-        y = normsum(y)
+        sums = y.sum(axis=1)
+        maxsum = sums.max()
+        y = y / maxsum
+    else:
+        y = y / y.sum()
     return y
 
 
 def interpolation(y, x, step=1, start=0, finish=0):
     """
     Interpolates data to a new axis.
 
@@ -779,18 +721,17 @@
 
     :returns: Interpolated data and the new axis
     :rtype: list[float], list[float]
     """
     temp_y = copy.deepcopy(y)
     dims = len(np.array(y).shape)
 
-    # NEW AXIS
     if start == 0 and start == finish:
-        new_start = -9999999
-        new_end = 99999999
+        new_start = math.ceil(min(x))
+        new_end = math.floor(max(x))
     else:
         new_start = start
         new_end = finish
         
     if min(x) > new_start:
         new_start = math.ceil(min(x))
     if max(x) < new_end:
@@ -1026,15 +967,15 @@
 
     :type y: list[float]
     :param y: Data to be normalized.
 
     :type x: list[float]
     :param x: x axis of the data
 
-    :type peak: int
+    :type peak: float
     :param peak: Peak position in x-axis values.
 
     :type shift: int
     :param shift: Range to look for the real peak. The default is 10.
 
     :returns: Normalized data.
     :rtype: list[float]
@@ -1105,16 +1046,17 @@
 
     if len(peaks) == 1:
         peaks = int(peaks[0])
     
     return peaks
 
 
-def confusionmatrix(tt, tp, gn=None, plot=False, title='', ndw=True, cmm='Blues',
-                    fontsize=20, figsize=(12, 15), ylabel='True', xlabel='Prediction'):
+def confusionmatrix(tt, tp, gn=None, plot=False, save=False, title='', ndw=True, cmm='Blues',
+                    fontsize=20, figsize=(12, 15), ylabel='True', xlabel='Prediction', 
+                    filename='cm.png', rotation=(45, 0)):
     """
     Calculates and/or plots the confusion matrix for machine learning algorithm
     results.
 
     :type tt: list[float]
     :param tt: Real targets.
 
@@ -1149,69 +1091,63 @@
     
     :type xlabel: str
     :param xlabel: Label for x axis. Default is `Prediction`.
     
     :returns: The confusion matrix
     :rtype: list[float]
     """
-    tt = list(tt)
-    tp = list(tp)
+    tt = np.array([int(i) for i in tt])
+    tp = np.array([int(i) for i in tp])
     plot = bool(plot)
-    
+
     if gn is None:
-        t = int(max(max(tt), max(tp)))
-        gn = [i for i in range(t+1)]
+        gn = np.arange(int(np.max([tt, tp])) + 1)
     
     group_names = list(gn)
     gn = len(group_names)
     title = str(title)
     cmm = str(cmm)
     fontsize = int(fontsize)
 
-    m = [[0 for _ in range(gn)] for _ in range(gn)]
-    p = [0 for _ in range(gn)] # number in each class
+    m = np.zeros((gn, gn))
+    p = np.bincount(tt, minlength=gn)
 
-    for i in range(len(p)): # count them
-        for j in tt:
-            if i == j:
-                p[i] += 1
-
-    for i in range(len(tt)):
-        for row in range(len(p)):
-            for col in range(len(p)):
-                if tp[i] == col and tt[i] == row:
-                    m[row][col] += 1
-
-    for i in range(len(m)):
+    for i in range(gn):
         if p[i] == 0:
-            # if ndw == True:
             if ndw is True:
-                print('No data with label (class) ' + str(i) + ' where found when making the confusion matrix. Check if the count is out of bounds or none samples of the class where included in the sample.\n')
+                print(f'No data with label (class) {i} was found when making the confusion matrix. '
+                      'Check if the count is out of bounds or none samples of the class were included in the sample.\n')
         else:
-            m[i] = np.array(m[i]) / p[i]
 
-    if plot:
+            m[i] = np.bincount(tp[tt == i], minlength=gn) / p[i]
+
+    if plot or save:
         fig = plt.figure(tight_layout=True, figsize=figsize)
         plt.rc('font', size=fontsize)
         ax = fig.add_subplot()
         ax.imshow(m, cmap=cmm)
         ax.set_title(title)
         ax.set_xticks(np.arange(len(group_names)))
         ax.set_yticks(np.arange(len(group_names)))
         ax.set_xticklabels(group_names)
         ax.set_yticklabels(group_names)
         plt.ylabel(ylabel)
         plt.xlabel(xlabel)
-        plt.setp(ax.get_xticklabels(), rotation=45, ha="right", rotation_mode="anchor")
+        plt.setp(ax.get_xticklabels(), rotation=rotation[0], ha="right", rotation_mode="anchor")
+        plt.setp(ax.get_yticklabels(), rotation=rotation[1], ha="right", rotation_mode="anchor")
 
         for i in range(gn):
             for j in range(gn):
-                ax.text(j, i, round(m[i][j], 2), ha='center', va='center', color='black')
+                ax.text(j, i, "{:.2f}".format(round(m[i][j], 2)), ha='center', va='center', color='black')
         
-        plt.show()
+        if plot:
+            plt.show()
+
+        if save:
+            plt.savefig(filename)
         
     return m
 
 
 def avg(y):
     """
     Calculates the average vector from a list of vectors.
@@ -1221,18 +1157,15 @@
 
     :returns: The average of the vectors in the list.
     :rtype: list[float]
     """
     dims = len(np.array(y).shape)  # detect dimensions 
     
     if dims > 1:
-        avg_data = np.array([0 for _ in range(len(y[0]))])
-        for i in y:
-            avg_data = avg_data + i
-        avg_data = avg_data / len(y)
+        avg_data = np.mean(y, axis=0)
     else:
         avg_data = sum(y)/len(y)
     
     return avg_data
 
 
 def sdev(y):
@@ -1241,24 +1174,17 @@
 
     :type y: list[float]
     :param y: List of vectors.
 
     :returns: Standard deviation curve
     :rtype: list[float]
     """
-    dims = len(np.array(y).shape)  # detect dimensions    
-    curve_std = []  # stdev for each step
-
-    if dims > 1:
-        for i in range(len(y[0])):
-            temp = []
-            for j in range(len(y)):
-                temp.append(y[j][i])
-            curve_std.append(sta.stdev(temp))  # stdev for each step
-        curve_std = np.array(curve_std)
+    y = np.array(y)
+    if y.ndim > 1:
+        curve_std = np.std(y, axis=0)
     else:
         curve_std = sta.stdev(y)
     return curve_std
 
 
 def median(y):
     """
@@ -1266,23 +1192,20 @@
     
     :type y: list[float]
     :param y: List of vectors.
 
     :returns: median curve
     :rtype: list[float]    
     """
+    dims = len(np.array(y).shape)  
     median = []
-    length = len(y[0])
-    meas = len(y)
-    
-    for j in range(length):
-        temp = []
-        for i in range(meas):
-            temp.append(y[i][j])
-        median.append(np.median(temp))    
+    if dims > 1:
+        median = np.median(y, axis=0) 
+    else:
+        median = np.median(y)
     return median
 
 
 def lorentzfit(y=[0], x=[0], pos=0, look=5, shift=2, gamma=5, alpha=1, manual=False):
     """
     Fits peak as an optimization problem or manual fit for Lorentz distirbution,
     also known as Cauchy. A curve `y` is only mandatory if the optimixzation is
@@ -1320,37 +1243,35 @@
     :rtype: list[float]
     """
     ax = list(x)
     y = list(y)      
     
     if manual:
         if ax == [0]: # if no axis is passed
-            ax = [i for i in range(-100, 100)]
+            ax = range(-100, 100)
         
-        fit = []
-        for i in ax:
-            fit.append(alpha/(np.pi*gamma*(1+((i-pos)/gamma)**2)))
+        fit = [alpha/(np.pi*gamma*(1+((i-pos)/gamma)**2)) for i in ax]
 
     else:            
         if ax == [0]: # if no axis is passed
-            ax = [i for i in range(len(y))]
+            # ax = [i for i in range(len(y))]
+            ax = range(len(y))
         
         s = int(shift/abs(ax[1]-ax[0]))
         look = int(look/abs(ax[1]-ax[0]))
         
         pos = int(valtoind(pos, ax))
         
         for k in range(pos-s, pos+s):
                 if y[k] > y[pos]:
                     pos = k
         p = ax[pos]
     
         def objective(x):
-            fit = 0
-            error = 0
+            fit, error = 0, 0
             ppos = valtoind(x[2], ax)
                 
             for i in range(ppos-look, ppos+look+1):  # for all the points            
                 fit = x[0]*(1/(np.pi*x[1]*(1+((ax[i]-x[2])/x[1])**2)))
                 error += (fit-y[i])**2
             
             return error**0.5
@@ -1361,23 +1282,20 @@
         x0 = np.array([alpha, gamma, p])  # master vector to optimize, initial values
         bnds = [[0.00000001, max(y)*9999999], [0.1, 9999], [p-s, p+s]]
         con1 = {'type': 'ineq', 'fun': constraint1}
         cons = ([con1])
         solution = minimize(objective, x0, method='SLSQP', bounds=bnds, constraints=cons)
         x = solution.x
         
-        fit = []
-    
-        for l in range(len(ax)):  # for all the points
-            fit.append(x[0]*(1/(np.pi*x[1]*(1+((ax[l]-x[2])/x[1])**2))))
+        fit = [x[0]*(1/(np.pi*x[1]*(1+((ax[l]-x[2])/x[1])**2))) for l in range(len(ax))]
         
     return fit
 
 
-def gaussfit(y=[0], x=None, pos=0, look=5, shift=2, sigma=4.4, alpha=1, manual=False, params=False):
+def gaussfit(y=[0], x=[0], pos=0, look=5, shift=2, sigma=4.4, alpha=1, manual=False, params=False):
     """
     Fits peak as an optimization problem or manual fit. A curve `y` is only 
     mandatory if the optimixzation is needed (manual=False, default). If no
     axis 'ax' is defined, then a default axis is generated for both options. 
 
     :type y: list[float]
     :param y: Data to fit. Single vector.
@@ -1409,27 +1327,26 @@
     :type params: boolean
     :param params: If `True`, it returns the parameters of the fit in the
         order of `alpha`, `sigma` and `peak position`. Default is `False`.
 
     :returns: Fitted curve.
     :rtype: list[float]
     """
-
     ax = list(x) # from now foreward, x is the variable for the optimization.
-    
+
     if manual:
-        if ax is None: # if no axis is passed
+        if ax == [0]: # if no axis is passed
             ax = [i for i in range(-100, 100)]
 
         fit = []
         for i in ax:
             fit.append((alpha/(sigma*(np.sqrt(2*np.pi))))*(np.exp(-0.5*(((i-pos)/sigma)**2))))    
         
     else:
-        if ax is None: # if no axis is passed
+        if ax == [0]: # if no axis is passed
             ax = [i for i in range(len(y))]
             
         y = list(y)
         
         pos = int(valtoind(pos, ax))
         
         for i in range(len(y)):
@@ -1746,15 +1663,14 @@
                 count = 0
                 for k in range(len(x_p)):
                     if (x_cords[i] < x_p[k] <= x_cords[i+1] and
                             y_cords[j] < y_p[k] <= y_cords[j+1] and
                             groups[k] == l):
                         count += 1
                         
-              
                 if count > th:
                     pmap[j][i] = count
                 else:
                     pmap[j][i] = 0
         
         maximum = max(np.array(pmap).flatten())
         
@@ -1764,52 +1680,30 @@
         else:
             pmap = np.array(pmap) / maximum
         
         master.append(pmap)
     return master
 
 
-def colormap(colors, name='my_name', n=100):
-    """
-    Simplify the creation of colormaps.
-
-    :type colors: list
-    :param colors: List of colors thaat you ant on the colormap
-
-    :type name: string, optional
-    :param name: Name of the colormap. The default is 'my_name'.
-
-    :type n: int, optional
-    :param n: Divisions. The default is 100.
-
-    :returns: Colormap in Matplotlib format.
-    :rtype: cmap
-    """    
-    return LinearSegmentedColormap.from_list(name, colors, N=n)
-
-
-def isaxis(data):
+def isaxis(y):
     """
     Detects if there is an axis in the data.
 
     :type data: list[float]
     :param data: Data containing spectras an possible axis.
 
     :returns: True if there is axis.
     :rtype: bool
     """
-    features = list(data)
+    features = list(y)
+    axis = features[0]
+    if len(np.array(y).shape) == 1:
+        axis = features
+    return all(axis[i] <= axis[i + 1] for i in range(len(axis) - 1))
 
-    is_axis = True  # there is axis by default
-    axis = features[0]  # axis should be the first
-    for i in range(len(axis) - 1):  # check all the vector
-        if axis[i] > axis[i + 1]:
-            is_axis = False
-            break
-    return is_axis
 
 
 def trim(y, start=0, finish=0):
     """
     Deletes columns in a list from start to finish.
 
     :type y: list
@@ -1830,17 +1724,18 @@
     if dims == 1:
         y = [y]
     
     final = []
     if finish == 0 or finish > len(y[0]):
         finish = len(y[0])
     t = finish - start    
+
     for j in y:
         temp = j
-        for i in range(t):
+        for _ in range(t):
             temp = np.delete(temp, start, 0)   
         final.append(list(temp))
     y = final
     
     if dims == 1:
         y = y[0]
         
@@ -1866,16 +1761,14 @@
     features = all_list[0]
     for i in range(1, len(all_list)):
         features = np.c_[features, all_list[i]]
 
     np.random.shuffle(features)  # shuffle data before training the ML
 
     if delratio > 0:  # to random delete an amount of data
-        if delratio >= 1:
-            delratio = 0.99
 
         delnum = int(math.floor(delratio * len(features)))  # amount to delete
 
         for i in range(delnum):
             row = random.randrange(0, len(features))  # row to delete
             features = np.delete(features, row, 0)
 
@@ -2120,48 +2013,44 @@
 
     :type plot: bool
     :param plot: To plot or not a visual aid. The default is True.
 
     :returns: Data with the subtracted reference.
     :rtype: list[float]
     """
-    data = copy.deepcopy(data)
-    ref = list(ref)
-    sample = int(sample)  # spectrum chosen to work with. 0 is the first
-    alpha = float(alpha)  # multiplication factor to delete the ref spectrum on the sample
-    
-    dims = len(np.array(data).shape)
-    
-    if dims > 1:
-        for i in range(len(data)):
-            data[i] = np.array(data[i]) - np.array(ref) * alpha  
-        toplot = data[sample]
-        final =  np.array(toplot) -  np.array(ref) * alpha
-    else:
-        toplot = copy.deepcopy(data)
-        final = np.array(data) - np.array(ref) * alpha    
-        data = final
+    data = copy.deepcopy(data)   
+    dims = len(np.shape(data))
+    data_sub = []
+
+    if dims == 1:
+        data = [data]
+
+    for i in data:
+        data_sub.append(np.array(i) - np.array(ref) * alpha)
         
     if plot:
         if axis == 0:
                 axis = [i for i in range(len(ref))]
         else:
             axis = list(axis)
         
-        plt.plot(axis, toplot, linewidth=1, label='Original', linestyle='--')
+        plt.plot(axis, data_sub[sample], linewidth=1, label='Original', linestyle='--')
         plt.plot(axis, np.array(ref)*alpha, linewidth=1, label='Air*Alpha', linestyle='--')
-        plt.plot(axis, final, linewidth=1, label='Final')
+        plt.plot(axis, data[sample], linewidth=1, label='Final')
         if lims[0] < lims[1]:
             plt.gca().set_xlim(lims[0], lims[1])
         plt.legend(loc=0)
         plt.ylabel('a.u.')
         plt.xlabel('Shift (cm-1)')
         plt.show()
 
-    return list(data)
+    if dims == 1:
+        data_sub = data_sub[0]
+
+    return data_sub
 
 
 def pearson(data, labels=[], cm="seismic", fons=20, figs=(20, 17), tfs=25, 
             ti="Pearson", plot=True):
     """
     Calculates Pearson matrix and plots it.
 
@@ -2237,15 +2126,15 @@
         pcm = ax.pcolormesh(pears, cmap=cm, vmin=-1, vmax=1)
         fig.colorbar(pcm, ax=ax)
         ax.set_title(title, fontsize=titlefs)
         ax.xaxis.set_major_locator(ticks)
         ax.yaxis.set_major_locator(ticks)
         ax.xaxis.set_major_formatter(formatt)
         ax.yaxis.set_major_formatter(formatt)
-        plt.xticks(rotation='90')
+        plt.xticks(rotation='vertical')
         plt.show()
 
     return pears
 
 def spearman(data, labels=[], cm="seismic", fons=20, figs=(20, 17), 
              tfs=25, ti="Spearman", plot=True):
     """
@@ -2323,15 +2212,15 @@
         pcm = ax.pcolormesh(spear, cmap=cm, vmin=-1, vmax=1)
         fig.colorbar(pcm, ax=ax)
         ax.set_title(title, fontsize=titlefs)
         ax.xaxis.set_major_locator(ticks)
         ax.yaxis.set_major_locator(ticks)
         ax.xaxis.set_major_formatter(formatt)
         ax.yaxis.set_major_formatter(formatt)
-        plt.xticks(rotation='90')
+        plt.xticks(rotation='vertical')
         plt.show()
     
     return spear
 
 
 def grau(data, labels=[], cm="seismic", fons=20, figs=(25, 15),
          tfs=25, ti="Grau (Beta)", marker="s", marks=100, plot=True):
@@ -2438,15 +2327,15 @@
         sc = ax.scatter(g2_shift, g3, alpha=1, edgecolors='none',
                         c=mse, cmap=cm, s=marks, marker=marker)
         plt.colorbar(sc)
         ax.set_xticks(x_ticks)
         ax.set_xticklabels(xtick_labels, fontsize=9)
         ax.set_xlim(0, max(x_ticks))
         ax.get_xticklabels()[0].set_fontweight('bold')
-        plt.xticks(rotation='90')
+        plt.xticks(rotation=90)
         ax.set_yticks(y_ticks)
         ax.set_ylim(min(y_ticks) - 0.5, max(y_ticks) + 0.5)
         ax.set_yticklabels(ytick_labels, fontsize=20)
         ax.grid(linestyle='--')
     
         temp = 0
         for i in range(len(t_c)):
@@ -2886,26 +2775,16 @@
     
     :type y: list 
     :param y: List of vectors to calculate the minimum and maximum vectors.
                 
     :returns: minimum and maximum vectors.
     :rtype: list[float]
     """
-    minimum = []
-    maximum = []
-    for i in range(len(y[0])):
-        temp_min = 99999999999999999999
-        temp_max = -9999999999999999999
-        for j in range(len(y)):
-            if y[j][i] < temp_min:
-                temp_min = y[j][i]
-            if y[j][i] > temp_max:
-                temp_max = y[j][i] 
-        minimum.append(temp_min)
-        maximum.append(temp_max)
+    minimum = [min(col) for col in zip(*y)]
+    maximum = [max(col) for col in zip(*y)]
     return minimum, maximum
 
 
 def fwhm(y, x, peaks, alpha=0.5, s=10):
     """
     Calculates the Full Width Half Maximum of specific peak or list of
     peaks for a single or multiple spectras.
@@ -2954,23 +2833,24 @@
         fwhm = []
         for j in range(len(ind)):
             for i in range(ind[j] - s, ind[j] + s):
                 if h[i] > h[ind[j]]:
                     ind[j] = i
                        
             h_m = h[ind[j]]*alpha # half maximum 
-            temp = 999999999
+
+            temp = float('inf')
             left = 0
             for i in range(ind[j]):
                 delta = abs(h[ind[j]-i] - h_m)
                 if temp > delta:
                     temp = delta
                     left = ind[j]-i
             
-            temp = 999999999
+            temp = float('inf')
             right = 0
             for i in range(len(x)-ind[j]):
                 delta = abs(h[ind[j]+i] - h_m)
                 if temp > delta:
                     temp = delta
                     right = ind[j]+i
             
@@ -3126,30 +3006,22 @@
     :param y: Vector, or list of vectors, that needs to be checked.
     
     :returns: True if contains the same value. False if there are different. If
         `y` is a list of vectors then it returns a list of booleans with the 
         respective answer.
     :rtype: bool
     """
-    dims = len(np.array(y).shape)
-    if dims == 1:
-        y = [y]
-    isequal = [True for _ in range(len(y))]
-    
-    for i in range(len(y)):
-        sample = y[i][0] # take the first to check
-        for j in y[i]:
-            if j != sample:
-                isequal[i] = False
-            if j == sample and isequal[i] != False:
-                isequal[i] = True
-    
-    if dims == 1:
-        isequal = isequal[0]
-    
+    dims = len(np.shape(y))
+    print(dims)
+    if 1 < dims: # checks if y is a list of lists
+        print('dsa')
+        isequal = [len(set(i))==1 for i in y] # applies the check to each list in y
+    elif dims == 1:
+        print('what')
+        isequal = len(set(y))==1 # checks if all elements in the list are equal
     return isequal
 
 
 def mahalanobis(v):
     """
     Calculates the Mahalanobis distance for a groups of vectors to the center 
     of mass, or average coordinates.
@@ -3200,20 +3072,21 @@
         if temp < std:
             std = temp
             reptve = i
     
     return reptve
 
 
-def voigtfit(y=None, x=None, pos=0, look=5, shift=2, gamma=5, sigma=4, alpha=1, amp=None, manual=False):
+def voigtfit(y=None, x=None, pos=0, look=5, shift=2, gamma=5, sigma=4, alpha=1, manual=False):
     """
     Fits peak as an optimization problem or manual fit for Voigt distirbution,
     also known as a convoluted Gaussian-Lorentz curve. A curve `y` is only
     needed for the optimization (manual=False, default). If no axis `x` is 
-    defined, then a default axis is generated for both options.
+    defined, then a default axis is generated for both options. It is reccomended to
+    Normalize the data before fitting.
 
     :type y: list[float]
     :param y: Data to fit. Single vector.
 
     :type x: list[float]
     :param x: x axis.
 
@@ -3240,16 +3113,15 @@
     :type manual: boolean
     :param manual: If `True`, 1 curve will be generated using the declared 
         parameter `gamma` and perform a manual fit. Default is `False`.
 
     :returns: Fitted curve.
     :rtype: list[float]
     """
-    ax = x
-    # y = list(y)      
+    ax = x  
         
     if manual:
         if ax is None: # if no axis is passed
             ax = [i for i in range(-100, 100)]
         
         s = int(shift/abs(ax[1]-ax[0]))
         
@@ -3271,15 +3143,14 @@
         for k in range(pos-s, pos+s):
                 if y[k] > y[pos]:
                     pos = k
         p = ax[pos]
     
         def objective(x):
             ppos = valtoind(x[3], ax)
-            fit = 0
             error = 0
             
             for i in range(ppos-look, ppos+look):  # for all the points            
                 gau = (1/(x[2]*(np.sqrt(2*np.pi))))*(np.exp(-0.5*(((ax[i]-x[3])/x[2])**2)))    
                 lor = (1/(np.pi*x[1]*(1+((ax[i]-x[3])/x[1])**2))) 
                 fit = gau*lor*x[0]
                 
@@ -3429,50 +3300,44 @@
     :param deg: degree of the derivative. That is, number of timess the vector
         will be derivated. In other words, if `deg=2`, will calculate the 
         second derivative. Default is `1`.
         
     :returns: derivative values, either in a list or single value.
     :rtype: float, list[float]
     """
+
     y = copy.deepcopy(y)
-    
-    if x is None:
-        x = [i for i in range(len(y))]
-    
+
+
     dims = len(np.array(y).shape)
     if dims == 1:
         y = [y]
-    
+
     tl = len(y[0])
-    
-    for k in range(deg):
+
+    if x is None:
+        x = list(range(tl))
+
+    for _ in range(deg):
         fd = []
         for j in y:
-            temp = []
-            for i in range(tl):
-                if i <= s:
-                    dx = x[i+s]-x[i]
-                    dy = j[i+s]-j[i]
-                elif i >= tl-s:
-                    dx = x[i]-x[i-s]
-                    dy = j[i]-j[i-s]
-                else:
-                    dx = x[i+s]-x[i-s]
-                    dy = j[i+s]-j[i-s]
-                temp.append(dy/dx)
+            temp = [((j[i + s] - j[i]) / (x[i + s] - x[i])) if i <= s else
+                    ((j[i] - j[i - s]) / (x[i] - x[i - s])) if i >= tl - s else
+                    ((j[i + s] - j[i - s]) / (x[i + s] - x[i - s])) for i in range(tl)]
             fd.append(temp)
         y = fd
-    
+
     if dims == 1:
         fd = fd[0]
-    
+
     return fd
 
 
-def peaksimilarity(y1, y2, p1, p2, n=5, x=None, plot=False, cmm='inferno', fontsize=10, title='Peak similarity'):    
+def peaksimilarity(y1, y2, p1, p2, n=5, x=None, plot=False, cmm='inferno', 
+                   fontsize=10, title='Peak similarity'):    
     """
     Calculates the similarity matrix as described in ´doi:10.1142/S021972001350011X´.
     It quantifyes the difference of the derivative function of the peaks and 
     puts them into a matrix. This can be used for peak alignment.
    
     :type y1: list[float]
     :param y1: First vector to compare.
@@ -3512,18 +3377,19 @@
     :rtype: list[float]
     """
     if x is None:
         x = [i for i in range(len(y1))]
     
     if len(p1) < len(p2):
         p1.append(0)
-    if len(p1) > len(p2):
+    elif len(p1) > len(p2):
         p2.append(0)        
     
     peaks = [p1, p2]
+
     peaks = valtoind(peaks, x)
     
     sm = []
     names = []
     for i in peaks[0]:
         temp = []
         names.append(i)
@@ -3538,93 +3404,84 @@
         fig = plt.figure(tight_layout=True, figsize=(6, 7.5))
         plt.rc('font', size=fontsize)
         ax = fig.add_subplot()
         ax.imshow(sm, cmap=cmm)
         ax.set_title(title)
         ax.set_xticks(np.arange(len(names)))
         ax.set_yticks(np.arange(len(names)))
-        ax.set_xticklabels(peaks[0])
-        ax.set_yticklabels(peaks[1])
+        p0 = [x[int(i)] for i in peaks[0]]
+        p1 = [x[int(i)] for i in peaks[1]]
+        ax.set_xticklabels(p0)
+        ax.set_yticklabels(p1)
         plt.ylabel('y2')
         plt.xlabel('y1')
         plt.setp(ax.get_xticklabels(), rotation=45, ha="right", rotation_mode="anchor")
         plt.show()
         
     return sm
-
+       
 
 def reverse(y):
     """
     Reverses a vector or a list of vectors.
     
     :type y: list[float]
     :param y: list of vectors to reverse. Single or multiple.
 
     :rtype: list[float]
     :returns: Reversed data.
     """
     dims = len(np.array(y).shape)
-    rev = []
+    
     if dims == 1:
         y = [y]
     
-    for i in y:
-        temp = []
-        for j in reversed(i):
-            temp.append(j)
-        rev.append(temp)
+    rev = [list(reversed(row)) for row in y]
     
     if dims == 1:
         rev = rev[0]
     
     return rev
-        
+
 
 def count(y, value=0):
     """
     Counts the number of values that coincide with `value`.
     
     :type y: list[float]
     :param y: vector or list of vectors to search for values.
     
     :type value: float
     :param value: Value or list of values to search in `y`. If many values are
-        passed, then it rteturns a list with the counted equalities. Default is 0.
+        passed, then it returns a list with the counted equalities. Default is 0.
 
     :rtype: list[float]
     :returns: Reversed data.
     """
     y = copy.deepcopy(y)
     dims_val = len(np.array(value).shape)
     dims_y = len(np.array(y).shape)
     
-    print(dims_y, dims_val)
-    
     if dims_val < 1:
         value = [value]
         
     if dims_y == 1:
         y = [y]
     
-    count = [[0 for _ in range(len(value))] for _ in range(len(y))]
-    
-    for k in range(len(y)):
-        for j in range(len(value)):
-            for i in y[k]:
-                if i == value[j]:
-                    count[k][j] += 1
+    count = [[list(row).count(val) for val in value] for row in y]
     
     if dims_val < 1:
         count = [i[0] for i in count]
     
     if dims_y == 1:
         count = count[0]
     
     return count
 
+
 def vectortoimg(y, negatives='remove', inverted=False):
     """
     Transforms 1-D vecctors into an image. Useful for more insightful results
         when performing deep learning.
 
     :type y: list[float]
     :param y: vector or list of vectors.
@@ -3777,8 +3634,9 @@
             temp = lorentzfit(x=ax, pos=x[i], gamma=x[i+n], alpha=x[i+2*n], manual=True)
         if method == 'voigt':
             temp = voigtfit(x=ax, pos=x[i], gamma=x[i+n], sigma=x[i+2*n], alpha=x[i+3*n], manual=True)
         f.append(temp)
         for j in range(len(ax)):
             y0[j] += temp[j]
     
-    return f[0]
+    return f[0]
+
```

### Comparing `spectrapepper-0.1.7/spectrapepper.egg-info/PKG-INFO` & `spectrapepper-0.1.8/spectrapepper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: spectrapepper
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package to simplify and accelerate analysis of spectroscopy data
 Home-page: https://github.com/spectrapepper/spectrapepper
 Author: spectrapepper
 Author-email: spectrapepper@gmail.com
 License: MIT license
 Keywords: spectrapepper
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -24,22 +23,23 @@
 <center>
     <img src="https://raw.githubusercontent.com/spectrapepper/spectrapepper/main/docs/_static/spectrapepperlogo-alt.png" width="50%">
 </center>
 
 [![image](https://img.shields.io/pypi/v/spectrapepper.svg)](https://pypi.python.org/pypi/spectrapepper)
 [![image](https://img.shields.io/conda/vn/conda-forge/spectrapepper.svg)](https://anaconda.org/conda-forge/spectrapepper)
 [![image](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![image](https://img.shields.io/lgtm/grade/python/g/spectrapepper/spectrapepper.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/spectrapepper/spectrapepper/context:python)
+[![CodeQL](https://github.com/spectrapepper/spectrapepper/actions/workflows/codeql.yml/badge.svg)](https://github.com/spectrapepper/spectrapepper/actions/workflows/codeql.yml)
 [![image](https://github.com/spectrapepper/spectrapepper/workflows/docs/badge.svg)](https://spectrapepper.github.io/spectrapepper)
 [![codecov](https://codecov.io/gh/spectrapepper/spectrapepper/branch/main/graph/badge.svg?token=DC0QIwuYel)](https://codecov.io/gh/spectrapepper/spectrapepper)
 [![Downloads](https://static.pepy.tech/personalized-badge/spectrapepper?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=pypi%20downloads)](https://pepy.tech/project/spectrapepper)
 [![image](https://img.shields.io/conda/dn/conda-forge/spectrapepper?color=blue&label=conda%20downloads)](https://anaconda.org/conda-forge/spectrapepper)
 [![image](https://img.shields.io/badge/stackoverflow-Ask%20a%20question-brown?logo=stackoverflow&logoWidth=18&logoColor=white)](https://stackoverflow.com/questions/tagged/spectrapepper)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03781/status.svg)](https://doi.org/10.21105/joss.03781)
 
+
 **A Python package to simplify and accelerate analysis of spectroscopy data.**
 
 * GitHub repo: https://github.com/spectrapepper/spectrapepper
 * Documentation: https://spectrapepper.github.io/spectrapepper
 * PyPI: https://pypi.python.org/pypi/spectrapepper
 * Conda-forge: https://anaconda.org/conda-forge/spectrapepper
 * Free software: MIT license
@@ -103,9 +103,7 @@
         conda remove spectrapepper
 
 
 # Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the
 [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
-
-
```

