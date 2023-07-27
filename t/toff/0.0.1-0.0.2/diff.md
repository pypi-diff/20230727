# Comparing `tmp/toff-0.0.1.tar.gz` & `tmp/toff-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toff-0.0.1.tar", last modified: Sun Jan  8 22:15:23 2023, max compression
+gzip compressed data, was "toff-0.0.2.tar", last modified: Mon Mar 27 20:05:41 2023, max compression
```

## Comparing `toff-0.0.1.tar` & `toff-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 22:15:23.988715 toff-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-08 22:14:59.000000 toff-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-01-08 22:15:23.988715 toff-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-01-08 22:14:59.000000 toff-0.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-01-08 22:15:23.988715 toff-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-08 22:14:59.000000 toff-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 22:15:23.988715 toff-0.0.1/toff/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-01-08 22:14:59.000000 toff-0.0.1/toff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-08 22:14:59.000000 toff-0.0.1/toff/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-01-08 22:14:59.000000 toff-0.0.1/toff/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14270 2023-01-08 22:14:59.000000 toff-0.0.1/toff/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 22:15:23.988715 toff-0.0.1/toff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-01-08 22:15:23.000000 toff-0.0.1/toff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-08 22:15:23.000000 toff-0.0.1/toff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 22:15:23.000000 toff-0.0.1/toff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-08 22:15:23.000000 toff-0.0.1/toff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-08 22:15:23.000000 toff-0.0.1/toff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-08 22:15:23.000000 toff-0.0.1/toff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:05:41.977796 toff-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-27 20:05:26.000000 toff-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-03-27 20:05:41.977796 toff-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-03-27 20:05:26.000000 toff-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-03-27 20:05:41.977796 toff-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-27 20:05:26.000000 toff-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:05:41.973796 toff-0.0.2/toff/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-27 20:05:26.000000 toff-0.0.2/toff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-27 20:05:26.000000 toff-0.0.2/toff/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-27 20:05:26.000000 toff-0.0.2/toff/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14424 2023-03-27 20:05:26.000000 toff-0.0.2/toff/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 20:05:41.977796 toff-0.0.2/toff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-03-27 20:05:41.000000 toff-0.0.2/toff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-27 20:05:41.000000 toff-0.0.2/toff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 20:05:41.000000 toff-0.0.2/toff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-27 20:05:41.000000 toff-0.0.2/toff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-27 20:05:41.000000 toff-0.0.2/toff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-27 20:05:41.000000 toff-0.0.2/toff.egg-info/top_level.txt
```

### Comparing `toff-0.0.1/LICENSE` & `toff-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toff-0.0.1/PKG-INFO` & `toff-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toff
-Version: 0.0.1
+Version: 0.0.2
 Summary: toff is a python package to get topologies from the OpenFF initiative
 Home-page: https://github.com/ale94mleon/toff
 Author: Alejandro Martínez León
 Author-email: ale94mleon@gmail.com
 License: Apache License 2.0
 Project-URL: Discussions, https://github.com/ale94mleon/toff/discussions
 Project-URL: Documentation, https://toff.readthedocs.io/en/latest/
@@ -77,14 +77,20 @@
 If you have questions on how to use **TOFF**, or if you want to give feedback or share ideas and new features, please head to the `GitHub Discussions <https://github.com/ale94mleon/TOFF/discussions>`_.
 
 Citing **TOFF**
 ------------------
 
 Please refer to the `citation page <https://TOFF.readthedocs.io/en/latest/source/citations.html>`__ on the documentation.
 
+Foundings
+---------
+
+This project received foundings from `Marie Skłodowska-Curie Actions <https://cordis.europa.eu/project/id/860592>`__. It was developed in the 
+`Computational Biophysics Group <https://biophys.uni-saarland.de/>`__ of `Saarland University <https://www.uni-saarland.de/en/home.html>`__.
+
 
 ..  |docs|  image:: https://readthedocs.org/projects/toff/badge/?version=latest
     :target: https://toff.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation
 
 ..  |binder| image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/ale94mleon/TOFF/HEAD?labpath=%2Fdocs%2Fnotebooks%2F
```

### Comparing `toff-0.0.1/README.rst` & `toff-0.0.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,20 @@
 If you have questions on how to use **TOFF**, or if you want to give feedback or share ideas and new features, please head to the `GitHub Discussions <https://github.com/ale94mleon/TOFF/discussions>`_.
 
 Citing **TOFF**
 ------------------
 
 Please refer to the `citation page <https://TOFF.readthedocs.io/en/latest/source/citations.html>`__ on the documentation.
 
+Foundings
+---------
+
+This project received foundings from `Marie Skłodowska-Curie Actions <https://cordis.europa.eu/project/id/860592>`__. It was developed in the 
+`Computational Biophysics Group <https://biophys.uni-saarland.de/>`__ of `Saarland University <https://www.uni-saarland.de/en/home.html>`__.
+
 
 ..  |docs|  image:: https://readthedocs.org/projects/toff/badge/?version=latest
     :target: https://toff.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation
 
 ..  |binder| image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/ale94mleon/TOFF/HEAD?labpath=%2Fdocs%2Fnotebooks%2F
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `toff-0.0.1/setup.cfg` & `toff-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `toff-0.0.1/toff/_version.py` & `toff-0.0.2/toff/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 # We will use semantic version (major, minor, patch)
-__main_version_tuple__ = (0, 0, 1)
+__main_version_tuple__ = (0, 0, 2)
 __pre_version_tuple__ = None # or None or an empty tuple, the first char is alpha, beta, rc, etc...
 
 if __pre_version_tuple__:
     __version_tuple__ = tuple(list(__main_version_tuple__) + list(__pre_version_tuple__))
     __version__ = '.'.join([str(i) for i in __main_version_tuple__]) + f'{__pre_version_tuple__[0][0]}' + '.'.join([str(i) for i in __pre_version_tuple__[1:]])
 else:
     __version_tuple__ = __main_version_tuple__
```

### Comparing `toff-0.0.1/toff/cli.py` & `toff-0.0.2/toff/cli.py`

 * *Files identical despite different names*

### Comparing `toff-0.0.1/toff/utils.py` & `toff-0.0.2/toff/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     ----------
     input_path_mol : str
         The path were the file molecule is. Only the foll, following extensions are valid:
 
         * ``inchi`` (only the first line of the file will be considered and should be a valid InChi string)
         * ``smi`` (only the first line of the file will be considered and should be a valid SMILES string)
         * ``mol``
+        * ``sdf`` (only the first molecule/conformer will be used)
         * ``mol2``
 
     Returns
     -------
     Chem.rdchem.Mol
         The RDKit molecule object
 
@@ -71,20 +72,22 @@
         with open(input_path_mol, 'r') as f:
             mol = Chem.MolFromInchi(f.readline())
     elif extension == 'smi':
         with open(input_path_mol, 'r') as f:
             mol = Chem.MolFromSmiles(f.readline())
     elif extension == 'mol':
         mol = Chem.MolFromMolFile(input_path_mol)
+    elif extension == 'sdf':
+        mol = Chem.SDMolSupplier(input_path_mol)[0]
     elif extension == 'mol2':
         mol = Chem.MolFromMol2File(input_path_mol)
     # elif extension == 'pdb':
     #     mol = Chem.MolFromPDBFile(input_path_mol)
     else:
-        raise NotImplementedError(f"Only: *.inchi, *.smi, *.mol, *.mol2 are valid extensions. But *.{extension} was provided")
+        raise NotImplementedError(f"Only: *.inchi, *.smi, *.mol, *.sdf *.mol2 are valid extensions. But *.{extension} was provided")
         # raise NotImplementedError(f"Only: *.inchi, *.smi, *.pdb, *.mol, *.mol2 are valid extensions. But *.{extension} was provided")
     mol = confgen(mol)
 
     if not mol:
         warnings.warn("Molecule was not converted. Check the input")
     return mol
```

### Comparing `toff-0.0.1/toff.egg-info/PKG-INFO` & `toff-0.0.2/toff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toff
-Version: 0.0.1
+Version: 0.0.2
 Summary: toff is a python package to get topologies from the OpenFF initiative
 Home-page: https://github.com/ale94mleon/toff
 Author: Alejandro Martínez León
 Author-email: ale94mleon@gmail.com
 License: Apache License 2.0
 Project-URL: Discussions, https://github.com/ale94mleon/toff/discussions
 Project-URL: Documentation, https://toff.readthedocs.io/en/latest/
@@ -77,14 +77,20 @@
 If you have questions on how to use **TOFF**, or if you want to give feedback or share ideas and new features, please head to the `GitHub Discussions <https://github.com/ale94mleon/TOFF/discussions>`_.
 
 Citing **TOFF**
 ------------------
 
 Please refer to the `citation page <https://TOFF.readthedocs.io/en/latest/source/citations.html>`__ on the documentation.
 
+Foundings
+---------
+
+This project received foundings from `Marie Skłodowska-Curie Actions <https://cordis.europa.eu/project/id/860592>`__. It was developed in the 
+`Computational Biophysics Group <https://biophys.uni-saarland.de/>`__ of `Saarland University <https://www.uni-saarland.de/en/home.html>`__.
+
 
 ..  |docs|  image:: https://readthedocs.org/projects/toff/badge/?version=latest
     :target: https://toff.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation
 
 ..  |binder| image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/ale94mleon/TOFF/HEAD?labpath=%2Fdocs%2Fnotebooks%2F
```

