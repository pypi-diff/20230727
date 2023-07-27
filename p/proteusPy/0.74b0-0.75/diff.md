# Comparing `tmp/proteusPy-0.74b0.tar.gz` & `tmp/proteusPy-0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteusPy-0.74b0.tar", last modified: Wed Jul 12 22:56:22 2023, max compression
+gzip compressed data, was "proteusPy-0.75.tar", last modified: Thu Jul 27 18:06:24 2023, max compression
```

## Comparing `proteusPy-0.74b0.tar` & `proteusPy-0.75.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-12 22:56:22.034607 proteusPy-0.74b0/
--rw-r--r--   0 egs        (505) staff       (20)       65 2023-07-09 01:16:52.000000 proteusPy-0.74b0/MANIFEST.in
--rw-r--r--   0 egs        (505) staff       (20)     5281 2023-07-12 22:56:22.034685 proteusPy-0.74b0/PKG-INFO
--rw-r--r--   0 egs        (505) staff       (20)     4141 2023-07-05 01:07:02.000000 proteusPy-0.74b0/README.md
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-12 22:56:22.030958 proteusPy-0.74b0/proteusPy/
--rw-r--r--   0 egs        (505) staff       (20)    93591 2023-03-16 23:40:51.000000 proteusPy-0.74b0/proteusPy/Disulfide.py
--rw-r--r--   0 egs        (505) staff       (20)    20687 2023-03-20 23:29:05.000000 proteusPy-0.74b0/proteusPy/DisulfideClass_Constructor.py
--rw-r--r--   0 egs        (505) staff       (20)    17282 2023-03-23 00:51:13.000000 proteusPy-0.74b0/proteusPy/DisulfideClasses.py
--rw-r--r--   0 egs        (505) staff       (20)     1027 2023-07-11 00:53:43.000000 proteusPy-0.74b0/proteusPy/DisulfideExceptions.py
--rw-r--r--   0 egs        (505) staff       (20)    38292 2023-06-16 22:53:38.000000 proteusPy-0.74b0/proteusPy/DisulfideList.py
--rw-r--r--   0 egs        (505) staff       (20)    23705 2023-07-06 15:13:40.000000 proteusPy-0.74b0/proteusPy/DisulfideLoader.py
--rw-r--r--   0 egs        (505) staff       (20)      830 2023-07-03 22:51:19.000000 proteusPy-0.74b0/proteusPy/ProteusGlobals.py
--rw-r--r--   0 egs        (505) staff       (20)      395 2022-12-04 05:59:19.000000 proteusPy-0.74b0/proteusPy/ProteusPyWarning.py
--rw-r--r--   0 egs        (505) staff       (20)     4934 2023-02-21 01:14:53.000000 proteusPy-0.74b0/proteusPy/Residue.py
--rw-r--r--   0 egs        (505) staff       (20)     1642 2023-07-12 22:55:58.000000 proteusPy-0.74b0/proteusPy/__init__.py
--rw-r--r--   0 egs        (505) staff       (20)    13442 2023-03-09 14:54:17.000000 proteusPy-0.74b0/proteusPy/angle_annotation.py
--rw-r--r--   0 egs        (505) staff       (20)     1297 2023-02-10 03:20:34.000000 proteusPy-0.74b0/proteusPy/atoms.py
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-12 22:56:22.034251 proteusPy-0.74b0/proteusPy/data/
--rw-r--r--   0 egs        (505) staff       (20)     2687 2023-07-04 13:46:04.000000 proteusPy-0.74b0/proteusPy/data/__init__.py
--rw-r--r--   0 egs        (505) staff       (20)     8670 2022-12-12 14:44:16.000000 proteusPy-0.74b0/proteusPy/data/ss_completed.txt
--rw-r--r--   0 egs        (505) staff       (20)   191074 2022-11-27 00:05:31.000000 proteusPy-0.74b0/proteusPy/data/ss_ids.txt
--rw-r--r--   0 egs        (505) staff       (20)      800 2023-02-05 06:37:57.000000 proteusPy-0.74b0/proteusPy/data/ss_query.json
--rw-r--r--   0 egs        (505) staff       (20)    21224 2023-02-21 01:10:52.000000 proteusPy-0.74b0/proteusPy/turtle3D.py
--rw-r--r--   0 egs        (505) staff       (20)    12468 2023-07-11 00:53:43.000000 proteusPy-0.74b0/proteusPy/utility.py
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-12 22:56:22.032138 proteusPy-0.74b0/proteusPy.egg-info/
--rw-r--r--   0 egs        (505) staff       (20)     5281 2023-07-12 22:56:21.000000 proteusPy-0.74b0/proteusPy.egg-info/PKG-INFO
--rw-r--r--   0 egs        (505) staff       (20)      776 2023-07-12 22:56:21.000000 proteusPy-0.74b0/proteusPy.egg-info/SOURCES.txt
--rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-12 22:56:21.000000 proteusPy-0.74b0/proteusPy.egg-info/dependency_links.txt
--rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-02 20:10:40.000000 proteusPy-0.74b0/proteusPy.egg-info/not-zip-safe
--rw-r--r--   0 egs        (505) staff       (20)       47 2023-07-12 22:56:21.000000 proteusPy-0.74b0/proteusPy.egg-info/requires.txt
--rw-r--r--   0 egs        (505) staff       (20)       10 2023-07-12 22:56:21.000000 proteusPy-0.74b0/proteusPy.egg-info/top_level.txt
--rw-r--r--   0 egs        (505) staff       (20)      107 2023-07-12 22:56:22.034908 proteusPy-0.74b0/setup.cfg
--rw-r--r--   0 egs        (505) staff       (20)     3693 2023-07-12 22:55:43.000000 proteusPy-0.74b0/setup.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-27 18:06:24.369599 proteusPy-0.75/
+-rw-r--r--   0 egs        (505) staff       (20)       65 2023-07-09 01:16:52.000000 proteusPy-0.75/MANIFEST.in
+-rw-r--r--   0 egs        (505) staff       (20)     5087 2023-07-27 18:06:24.369661 proteusPy-0.75/PKG-INFO
+-rw-r--r--   0 egs        (505) staff       (20)     4000 2023-07-26 00:26:52.000000 proteusPy-0.75/README.md
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-27 18:06:24.366454 proteusPy-0.75/proteusPy/
+-rw-r--r--   0 egs        (505) staff       (20)    93581 2023-07-16 03:29:22.000000 proteusPy-0.75/proteusPy/Disulfide.py
+-rw-r--r--   0 egs        (505) staff       (20)    20687 2023-03-20 23:29:05.000000 proteusPy-0.75/proteusPy/DisulfideClass_Constructor.py
+-rw-r--r--   0 egs        (505) staff       (20)    17282 2023-03-23 00:51:13.000000 proteusPy-0.75/proteusPy/DisulfideClasses.py
+-rw-r--r--   0 egs        (505) staff       (20)     1027 2023-07-11 00:53:43.000000 proteusPy-0.75/proteusPy/DisulfideExceptions.py
+-rw-r--r--   0 egs        (505) staff       (20)    38194 2023-07-13 01:45:02.000000 proteusPy-0.75/proteusPy/DisulfideList.py
+-rw-r--r--   0 egs        (505) staff       (20)    23705 2023-07-06 15:13:40.000000 proteusPy-0.75/proteusPy/DisulfideLoader.py
+-rw-r--r--   0 egs        (505) staff       (20)      830 2023-07-03 22:51:19.000000 proteusPy-0.75/proteusPy/ProteusGlobals.py
+-rw-r--r--   0 egs        (505) staff       (20)      395 2022-12-04 05:59:19.000000 proteusPy-0.75/proteusPy/ProteusPyWarning.py
+-rw-r--r--   0 egs        (505) staff       (20)     4934 2023-02-21 01:14:53.000000 proteusPy-0.75/proteusPy/Residue.py
+-rw-r--r--   0 egs        (505) staff       (20)     1641 2023-07-13 01:45:45.000000 proteusPy-0.75/proteusPy/__init__.py
+-rw-r--r--   0 egs        (505) staff       (20)    13442 2023-03-09 14:54:17.000000 proteusPy-0.75/proteusPy/angle_annotation.py
+-rw-r--r--   0 egs        (505) staff       (20)     1297 2023-02-10 03:20:34.000000 proteusPy-0.75/proteusPy/atoms.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-27 18:06:24.369269 proteusPy-0.75/proteusPy/data/
+-rw-r--r--   0 egs        (505) staff       (20)     2687 2023-07-04 13:46:04.000000 proteusPy-0.75/proteusPy/data/__init__.py
+-rw-r--r--   0 egs        (505) staff       (20)     8670 2022-12-12 14:44:16.000000 proteusPy-0.75/proteusPy/data/ss_completed.txt
+-rw-r--r--   0 egs        (505) staff       (20)   191074 2022-11-27 00:05:31.000000 proteusPy-0.75/proteusPy/data/ss_ids.txt
+-rw-r--r--   0 egs        (505) staff       (20)      800 2023-02-05 06:37:57.000000 proteusPy-0.75/proteusPy/data/ss_query.json
+-rw-r--r--   0 egs        (505) staff       (20)    21225 2023-07-15 22:25:26.000000 proteusPy-0.75/proteusPy/turtle3D.py
+-rw-r--r--   0 egs        (505) staff       (20)    12468 2023-07-11 00:53:43.000000 proteusPy-0.75/proteusPy/utility.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-27 18:06:24.367402 proteusPy-0.75/proteusPy.egg-info/
+-rw-r--r--   0 egs        (505) staff       (20)     5087 2023-07-27 18:06:24.000000 proteusPy-0.75/proteusPy.egg-info/PKG-INFO
+-rw-r--r--   0 egs        (505) staff       (20)      744 2023-07-27 18:06:24.000000 proteusPy-0.75/proteusPy.egg-info/SOURCES.txt
+-rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-27 18:06:24.000000 proteusPy-0.75/proteusPy.egg-info/dependency_links.txt
+-rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-02 20:10:40.000000 proteusPy-0.75/proteusPy.egg-info/not-zip-safe
+-rw-r--r--   0 egs        (505) staff       (20)       10 2023-07-27 18:06:24.000000 proteusPy-0.75/proteusPy.egg-info/top_level.txt
+-rw-r--r--   0 egs        (505) staff       (20)      107 2023-07-27 18:06:24.370121 proteusPy-0.75/setup.cfg
+-rw-r--r--   0 egs        (505) staff       (20)     3522 2023-07-13 00:54:34.000000 proteusPy-0.75/setup.py
```

### Comparing `proteusPy-0.74b0/PKG-INFO` & `proteusPy-0.75/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,60 +1,54 @@
 Metadata-Version: 2.1
 Name: proteusPy
-Version: 0.74b0
+Version: 0.75
 Summary: proteusPy - Protein Structure Analysis and Modeling Tools
 Home-page: https://github.com/suchanek/proteusPy/
 Author: Eric G. Suchanek, PhD
 Author-email: suchanek@mac.com
 License: MIT
 Project-URL: Documentation, https://suchanek.github.io/proteusPy/
 Project-URL: Source, https://github.com/suchanek/proteusPy/
 Project-URL: Tracker, https://github.com/suchanek/proteusPy/issues
 Keywords: proteus suchanek disulfide
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 *proteusPy* is a Python package specializing in the modeling and analysis of proteins of known structure with an emphasis on Disulfide Bonds. This package reprises my molecular modeling program [Proteus](https://doi.org/10.1021/bi00368a023), and relies on the [Turtle3D](https://suchanek.github.io/proteusPy/proteusPy/turtle3D.html) class. The turtle implements the functions ``Move``, ``Roll``, ``Yaw``, ``Pitch`` and ``Turn`` for movement in a three-dimensional space. The [Disulfide](https://suchanek.github.io/proteusPy/proteusPy/Disulfide.html) class implements methods to analyze the protein structure stabilizing element known as a *Disulfide Bond*. This class and its underlying methods are being used to perform a structural analysis of over 35,800 disulfide-bond containing proteins in the RCSB protein data bank.
 
-### Virtual Environment Installation/Creation
-
+# Virtual Environment Creation
 1. *Install Anaconda (<http://anaconda.org>)*
 2. *Build the environment.* 
-   At this point it's probably best to clone the repo via github since it contains all
-   of the notebooks test programs and raw Disulfide databases. The source code distribution can be used from pyPi as a normal
-   package, within your own environment.
-   - Using pyPi:
-     - python3 -m pip install proteusPy
+   It's simplest to clone the repo via github since it contains all of the notebooks, test programs and raw Disulfide databases. The source code distribution can be also be used from pyPi as a normal package, within your own environment.
    - From the gitHub repository:
      - Install git-lfs
        - https://help.github.com/en/github/managing-large-files/installing-git-large-file-storage
        - From a shell prompt: 
          ```
           $ git-lfs track "*.csv" "*.pkl" "*.mp4"
-          $ git clone https://github.com/suchanek/proteusPy/proteusPy.git
+          $ git clone https://github.com/suchanek/proteusPy
           $ cd proteusPy
           $ conda env create --name proteusPy --file=proteusPy.yml
           $ conda activate proteusPy
           $ pip install .
           $ jupyter nbextension enable --py --sys-prefix widgetsnbextension
 
-         ```
-3. *Profit!* OK, just kidding. I hope you enjoy using proteusPy and would love to hear any success/insights gleaned from it. The Disulfide database is unique as far as I know, and is ripe for mining. 
+  ```
+I hope you enjoy using proteusPy and would love to hear any success/insights gleaned from it. The Disulfide database is unique as far as I know, and is ripe for mining. 
 
 ### General Usage
 Once the package is installed one can use the existing notebooks for analysis of the RCSB Disulfide database. The ``notebooks`` directory contains all of my Jupyter notebooks and is a good place to start. The ``DisulfideAnalysis.ipynb`` notebook contains the first analysis paper. The ``programs`` subdirectory contains the primary programs for downloading the RCSB disulfide-containing structure files, (``DisulfideDownloader.py``), extracting the disulfides and creating the database loaders (``DisulfideExtractor.py``) and cluster analysis, (``DisulfideClass_Analysis.py``).
 
 The first time one loads the database via ``Load_PDB_SS()`` the system will attempt to download the full and subset database from my Google Drive. If this fails the system will attempt to rebuild the database from the repo's ``data`` subdirectory (not the package's). If you've downloaded from github this will work correctly. If you've installed from pyPi via ``pip`` it will fail.
 
 ### The Future
```

### Comparing `proteusPy-0.74b0/README.md` & `proteusPy-0.75/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 *proteusPy* is a Python package specializing in the modeling and analysis of proteins of known structure with an emphasis on Disulfide Bonds. This package reprises my molecular modeling program [Proteus](https://doi.org/10.1021/bi00368a023), and relies on the [Turtle3D](https://suchanek.github.io/proteusPy/proteusPy/turtle3D.html) class. The turtle implements the functions ``Move``, ``Roll``, ``Yaw``, ``Pitch`` and ``Turn`` for movement in a three-dimensional space. The [Disulfide](https://suchanek.github.io/proteusPy/proteusPy/Disulfide.html) class implements methods to analyze the protein structure stabilizing element known as a *Disulfide Bond*. This class and its underlying methods are being used to perform a structural analysis of over 35,800 disulfide-bond containing proteins in the RCSB protein data bank.
 
-### Virtual Environment Installation/Creation
-
+# Virtual Environment Creation
 1. *Install Anaconda (<http://anaconda.org>)*
 2. *Build the environment.* 
-   At this point it's probably best to clone the repo via github since it contains all
-   of the notebooks test programs and raw Disulfide databases. The source code distribution can be used from pyPi as a normal
-   package, within your own environment.
-   - Using pyPi:
-     - python3 -m pip install proteusPy
+   It's simplest to clone the repo via github since it contains all of the notebooks, test programs and raw Disulfide databases. The source code distribution can be also be used from pyPi as a normal package, within your own environment.
    - From the gitHub repository:
      - Install git-lfs
        - https://help.github.com/en/github/managing-large-files/installing-git-large-file-storage
        - From a shell prompt: 
          ```
           $ git-lfs track "*.csv" "*.pkl" "*.mp4"
-          $ git clone https://github.com/suchanek/proteusPy/proteusPy.git
+          $ git clone https://github.com/suchanek/proteusPy
           $ cd proteusPy
           $ conda env create --name proteusPy --file=proteusPy.yml
           $ conda activate proteusPy
           $ pip install .
           $ jupyter nbextension enable --py --sys-prefix widgetsnbextension
 
-         ```
-3. *Profit!* OK, just kidding. I hope you enjoy using proteusPy and would love to hear any success/insights gleaned from it. The Disulfide database is unique as far as I know, and is ripe for mining. 
+  ```
+I hope you enjoy using proteusPy and would love to hear any success/insights gleaned from it. The Disulfide database is unique as far as I know, and is ripe for mining. 
 
 ### General Usage
 Once the package is installed one can use the existing notebooks for analysis of the RCSB Disulfide database. The ``notebooks`` directory contains all of my Jupyter notebooks and is a good place to start. The ``DisulfideAnalysis.ipynb`` notebook contains the first analysis paper. The ``programs`` subdirectory contains the primary programs for downloading the RCSB disulfide-containing structure files, (``DisulfideDownloader.py``), extracting the disulfides and creating the database loaders (``DisulfideExtractor.py``) and cluster analysis, (``DisulfideClass_Analysis.py``).
 
 The first time one loads the database via ``Load_PDB_SS()`` the system will attempt to download the full and subset database from my Google Drive. If this fails the system will attempt to rebuild the database from the repo's ``data`` subdirectory (not the package's). If you've downloaded from github this will work correctly. If you've installed from pyPi via ``pip`` it will fail.
 
 ### The Future
```

### Comparing `proteusPy-0.74b0/proteusPy/Disulfide.py` & `proteusPy-0.75/proteusPy/Disulfide.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,42 +58,41 @@
            'psi_dist', 'torsion_length', 'rho']
 
 class Disulfide:
     """
     This class provides a Python object and methods representing a physical disulfide bond 
     either extracted from the RCSB protein databank or built using the 
     [proteusPy.Turtle3D](turtle3D.html) class. The disulfide bond is an important
-    intermolecular stabilizing structural element and is characterized by:
+    intramolecular stabilizing structural element and is characterized by:
 
     * Atomic coordinates for the atoms N, Cα, Cβ, C', Sγ for both residues. 
     These are stored as both raw atomic coordinates as read from the RCSB file 
     and internal local coordinates.
     * The dihedral angles Χ1 - Χ5 for the disulfide bond
     * A name, by default {pdb_id}{prox_resnumb}{prox_chain}_{distal_resnum}{distal_chain} 
     * Proximal residue number
     * Distal residue number
     * Approximate bond torsional energy (kcal/mol):
     
     $$ 
     E_{kcal/mol} \\approx 2.0 * cos(3.0 * \\chi_{1}) + cos(3.0 * \\chi_{5}) + cos(3.0 * \\chi_{2}) + 
     $$
-
     $$
-    cos(3.0 * \\chi_{4}) + 3.5 * cos(2.0 * \\chi_{3}) + 0.6 * cos(3.0 * \\chi_{3}) + 10.1 
+    cos(3.0 * \chi_{4}) + 3.5 * cos(2.0 * \chi_{3}) + 0.6 * cos(3.0 * \chi_{3}) + 10.1 
     $$
     
     The equation embodies the typical 3-fold rotation barriers associated with single bonds,
     (Χ1, Χ5, Χ2, Χ4) and a high 2-fold barrier for Χ3, resulting from the partial double bond
     character of the S-S bond. This property leads to two major disulfide families, characterized
     by the sign of Χ3. *Left-handed* disulfides have Χ3 < 0° and *right-handed* disulfides have
     Χ3 > 0°. Within this breakdown there are numerous subfamilies, broadly known as the *hook*,
     *spiral* and *staple*. These are under characgterization.
 
     * Euclidean length of the dihedral angles (degrees) defined as:
-    $$\\sqrt(\\chi_{1}^{2} + \\chi_{2}^{2} + \\chi_{3}^{2} + \\chi_{4}^{2} + \\chi_{5}^{2})$$
+    $$\sqrt(\chi_{1}^{2} + \chi_{2}^{2} + \chi_{3}^{2} + \chi_{4}^{2} + \chi_{5}^{2})$$
     * Cα - Cα distance (Å)
     * Cβ - Cβ distance (Å)
     * The previous C' and next N for both the proximal and distal residues. These are needed
     to calculate the backbone dihedral angles Φ and Ψ.
     * Backbone dihedral angles Φ and Ψ, when possible. Not all structures are complete and
     in those cases the atoms needed may be undefined. In this case the Φ and Ψ angles are set
     to -180°.
```

### Comparing `proteusPy-0.74b0/proteusPy/DisulfideClass_Constructor.py` & `proteusPy-0.75/proteusPy/DisulfideClass_Constructor.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy/DisulfideClasses.py` & `proteusPy-0.75/proteusPy/DisulfideClasses.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy/DisulfideExceptions.py` & `proteusPy-0.75/proteusPy/DisulfideExceptions.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy/DisulfideList.py` & `proteusPy-0.75/proteusPy/DisulfideList.py`

 * *Files 1% similar despite different names*

```diff
@@ -901,23 +901,20 @@
 
         modelss.build_model(chi1, chi2, chi3, chi4, chi5)
         res = DisulfideList([], 'neighbors')
         res = modelss.Torsion_neighbors(sslist, cutoff)
 
         return res
         
-    def nearest_neighbors(self, ss, cutoff: float):
+    def nearest_neighbors_ss(self, ss, cutoff: float):
         '''
         Given an input Disulfide and overall torsional cutoff, return 
         the list of Disulfides within the cutoff 
 
-        :param chi1: Chi1 (degrees)
-        :param chi2: Chi2 (degrees)
-        :param chi3: Chi3 (degrees)
-        :param chi4: Chi4 (degrees)
+        :param ss: Disulfide to compare to
         :param chi5: Chi5 (degrees)
         :param cutoff: Distance cutoff, degrees
         :return: DisulfideList of neighbors
         '''
 
         chi1 = ss.chi1
         chi2 = ss.chi2
```

### Comparing `proteusPy-0.74b0/proteusPy/DisulfideLoader.py` & `proteusPy-0.75/proteusPy/DisulfideLoader.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy/ProteusGlobals.py` & `proteusPy-0.75/proteusPy/ProteusGlobals.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy/Residue.py` & `proteusPy-0.75/proteusPy/Residue.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy/__init__.py` & `proteusPy-0.75/proteusPy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2023 Eric G. Suchanek, PhD., all rights reserved
 # Subject to the MIT public license.
 
 """
 .. include:: ../README.md
 """
 
-__version__ = "0.74b"
+__version__ = "0.75"
 
 import sys
 import os
 import glob
 import warnings
 import copy
```

### Comparing `proteusPy-0.74b0/proteusPy/angle_annotation.py` & `proteusPy-0.75/proteusPy/angle_annotation.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy/atoms.py` & `proteusPy-0.75/proteusPy/atoms.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy/data/__init__.py` & `proteusPy-0.75/proteusPy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy/data/ss_completed.txt` & `proteusPy-0.75/proteusPy/data/ss_completed.txt`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy/data/ss_ids.txt` & `proteusPy-0.75/proteusPy/data/ss_ids.txt`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy/data/ss_query.json` & `proteusPy-0.75/proteusPy/data/ss_query.json`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy/turtle3D.py` & `proteusPy-0.75/proteusPy/turtle3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '''
-Implementation of a 3D Turtle in Python.
+Implementation of a 3D 'Turtle' in Python.
 
-A part of the program proteusPy, https://github.com/suchanek/proteusPy, 
+Part of the program proteusPy, https://github.com/suchanek/proteusPy, 
 a Python packages for the manipulation and analysis of macromolecules. 
 Based on the C implementation originally authored by Eric G. Suchanek PhD, 1990.
 
 '''
 
-# Last modification 2/2/23 -egs-
+# Last modification 7/15/23 -egs-
 
 __pdoc__ = {'__all__': True}
 
 import numpy
 import math
 
 numpy.set_printoptions(suppress=True)
```

### Comparing `proteusPy-0.74b0/proteusPy/utility.py` & `proteusPy-0.75/proteusPy/utility.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.74b0/proteusPy.egg-info/PKG-INFO` & `proteusPy-0.75/proteusPy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,60 +1,54 @@
 Metadata-Version: 2.1
 Name: proteusPy
-Version: 0.74b0
+Version: 0.75
 Summary: proteusPy - Protein Structure Analysis and Modeling Tools
 Home-page: https://github.com/suchanek/proteusPy/
 Author: Eric G. Suchanek, PhD
 Author-email: suchanek@mac.com
 License: MIT
 Project-URL: Documentation, https://suchanek.github.io/proteusPy/
 Project-URL: Source, https://github.com/suchanek/proteusPy/
 Project-URL: Tracker, https://github.com/suchanek/proteusPy/issues
 Keywords: proteus suchanek disulfide
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 *proteusPy* is a Python package specializing in the modeling and analysis of proteins of known structure with an emphasis on Disulfide Bonds. This package reprises my molecular modeling program [Proteus](https://doi.org/10.1021/bi00368a023), and relies on the [Turtle3D](https://suchanek.github.io/proteusPy/proteusPy/turtle3D.html) class. The turtle implements the functions ``Move``, ``Roll``, ``Yaw``, ``Pitch`` and ``Turn`` for movement in a three-dimensional space. The [Disulfide](https://suchanek.github.io/proteusPy/proteusPy/Disulfide.html) class implements methods to analyze the protein structure stabilizing element known as a *Disulfide Bond*. This class and its underlying methods are being used to perform a structural analysis of over 35,800 disulfide-bond containing proteins in the RCSB protein data bank.
 
-### Virtual Environment Installation/Creation
-
+# Virtual Environment Creation
 1. *Install Anaconda (<http://anaconda.org>)*
 2. *Build the environment.* 
-   At this point it's probably best to clone the repo via github since it contains all
-   of the notebooks test programs and raw Disulfide databases. The source code distribution can be used from pyPi as a normal
-   package, within your own environment.
-   - Using pyPi:
-     - python3 -m pip install proteusPy
+   It's simplest to clone the repo via github since it contains all of the notebooks, test programs and raw Disulfide databases. The source code distribution can be also be used from pyPi as a normal package, within your own environment.
    - From the gitHub repository:
      - Install git-lfs
        - https://help.github.com/en/github/managing-large-files/installing-git-large-file-storage
        - From a shell prompt: 
          ```
           $ git-lfs track "*.csv" "*.pkl" "*.mp4"
-          $ git clone https://github.com/suchanek/proteusPy/proteusPy.git
+          $ git clone https://github.com/suchanek/proteusPy
           $ cd proteusPy
           $ conda env create --name proteusPy --file=proteusPy.yml
           $ conda activate proteusPy
           $ pip install .
           $ jupyter nbextension enable --py --sys-prefix widgetsnbextension
 
-         ```
-3. *Profit!* OK, just kidding. I hope you enjoy using proteusPy and would love to hear any success/insights gleaned from it. The Disulfide database is unique as far as I know, and is ripe for mining. 
+  ```
+I hope you enjoy using proteusPy and would love to hear any success/insights gleaned from it. The Disulfide database is unique as far as I know, and is ripe for mining. 
 
 ### General Usage
 Once the package is installed one can use the existing notebooks for analysis of the RCSB Disulfide database. The ``notebooks`` directory contains all of my Jupyter notebooks and is a good place to start. The ``DisulfideAnalysis.ipynb`` notebook contains the first analysis paper. The ``programs`` subdirectory contains the primary programs for downloading the RCSB disulfide-containing structure files, (``DisulfideDownloader.py``), extracting the disulfides and creating the database loaders (``DisulfideExtractor.py``) and cluster analysis, (``DisulfideClass_Analysis.py``).
 
 The first time one loads the database via ``Load_PDB_SS()`` the system will attempt to download the full and subset database from my Google Drive. If this fails the system will attempt to rebuild the database from the repo's ``data`` subdirectory (not the package's). If you've downloaded from github this will work correctly. If you've installed from pyPi via ``pip`` it will fail.
 
 ### The Future
```

### Comparing `proteusPy-0.74b0/proteusPy.egg-info/SOURCES.txt` & `proteusPy-0.75/proteusPy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,13 +18,12 @@
 proteusPy/residue.py
 proteusPy/turtle3D.py
 proteusPy/utility.py
 proteusPy.egg-info/PKG-INFO
 proteusPy.egg-info/SOURCES.txt
 proteusPy.egg-info/dependency_links.txt
 proteusPy.egg-info/not-zip-safe
-proteusPy.egg-info/requires.txt
 proteusPy.egg-info/top_level.txt
 proteusPy/data/__init__.py
 proteusPy/data/ss_completed.txt
 proteusPy/data/ss_ids.txt
 proteusPy/data/ss_query.json
```

### Comparing `proteusPy-0.74b0/setup.py` & `proteusPy-0.75/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 installation just type the command::
 
     python setup.py install
 
 However, you would normally install the latest proteusPy release from
 the PyPI archive with::
 
-    python -m pip install --index-url https://test.pypi.org/simple/ proteusPy
+    python -m pip install proteusPy
 
 For more in-depth instructions, see the installation section of the
 proteusPy documentation, linked to from:
 
 http://suchanek.github.io/proteusPy/
 
-This code is in alpha pre-release.
+This code is in beta.
 """
 import sys
 import os
 
 try:
     from setuptools import setup
     from setuptools import Command
@@ -38,15 +38,15 @@
     except ImportError:
         sys.exit(
             "We need both setuptools AND wheel packages installed "
             "for bdist_wheel to work. Try running: pip install wheel"
         )
 
 # Make sure we have the right Python version.
-MIN_PY_VER = (3, 8)
+MIN_PY_VER = (3, 9)
 if sys.version_info[:2] < MIN_PY_VER:
     sys.stderr.write(
         ("ERROR: proteusPy requires Python %i.%i or later. " % MIN_PY_VER)
         + ("Python %d.%d detected.\n" % sys.version_info[:2])
     )
     sys.exit(1)
 
@@ -73,28 +73,27 @@
       long_description_content_type='text/markdown',
       url='https://github.com/suchanek/proteusPy/',
       author='Eric G. Suchanek, PhD',
       author_email='suchanek@mac.com',
       license='MIT',
       packages=['proteusPy'],
       keywords='proteus suchanek disulfide',
-      install_requires=['pandas', 'numpy', 'matplotlib', 'pyvista', 'pip', 'tqdm', 'gdown'],
+      install_requires=[],
       source='https://github.com/suchanek/proteusPy/',
       project_urls={
         "Documentation": "https://suchanek.github.io/proteusPy/",
         "Source": "https://github.com/suchanek/proteusPy/",
         "Tracker": "https://github.com/suchanek/proteusPy/issues",
       },
       classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Topic :: Scientific/Engineering :: Chemistry',
         'Programming Language :: Python :: 3.9'],
       include_package_data=True,
```

