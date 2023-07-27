# Comparing `tmp/nemophoto-0.6.0.tar.gz` & `tmp/nemophoto-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nemophoto-0.6.0.tar", last modified: Mon Jun 12 15:59:23 2023, max compression
+gzip compressed data, was "nemophoto-0.7.0.tar", last modified: Thu Jul 27 20:12:11 2023, max compression
```

## Comparing `nemophoto-0.6.0.tar` & `nemophoto-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,21 @@
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:59:23.847919 nemophoto-0.6.0/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       51 2022-11-23 13:19:51.000000 nemophoto-0.6.0/.gitignore
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     1071 2021-10-01 13:50:37.000000 nemophoto-0.6.0/LICENSE
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       25 2021-10-30 15:21:47.000000 nemophoto-0.6.0/MANIFEST.in
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7999 2023-06-12 15:59:23.845919 nemophoto-0.6.0/PKG-INFO
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     6722 2023-05-17 06:49:22.000000 nemophoto-0.6.0/README.md
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:59:23.613918 nemophoto-0.6.0/Tutorial/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)    20260 2023-05-17 06:49:22.000000 nemophoto-0.6.0/Tutorial/Tutorial.md
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:59:23.670918 nemophoto-0.6.0/batch_examples/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      315 2021-10-06 19:56:05.000000 nemophoto-0.6.0/batch_examples/qc.sh
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      245 2021-10-06 19:56:05.000000 nemophoto-0.6.0/batch_examples/slurm.sh
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      205 2022-11-23 13:19:52.000000 nemophoto-0.6.0/batch_examples/td.in
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      118 2022-11-23 13:19:53.000000 nemophoto-0.6.0/batch_examples/ts.sh
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:59:23.825919 nemophoto-0.6.0/nemo/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)        0 2021-10-07 12:24:10.000000 nemophoto-0.6.0/nemo/__init__.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     8440 2023-05-17 06:49:22.000000 nemophoto-0.6.0/nemo/__main__.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       62 2023-06-12 15:56:49.000000 nemophoto-0.6.0/nemo/__version__.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)    41423 2023-06-12 15:51:10.000000 nemophoto-0.6.0/nemo/analysis.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     2417 2022-11-23 13:19:53.000000 nemophoto-0.6.0/nemo/batch_lx.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)    18058 2023-06-12 15:51:10.000000 nemophoto-0.6.0/nemo/tools.py
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:59:23.843919 nemophoto-0.6.0/nemophoto.egg-info/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7999 2023-06-12 15:59:22.000000 nemophoto-0.6.0/nemophoto.egg-info/PKG-INFO
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      459 2023-06-12 15:59:23.000000 nemophoto-0.6.0/nemophoto.egg-info/SOURCES.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)        1 2023-06-12 15:59:22.000000 nemophoto-0.6.0/nemophoto.egg-info/dependency_links.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       45 2023-06-12 15:59:22.000000 nemophoto-0.6.0/nemophoto.egg-info/entry_points.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       31 2023-06-12 15:59:22.000000 nemophoto-0.6.0/nemophoto.egg-info/requires.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)        5 2023-06-12 15:59:22.000000 nemophoto-0.6.0/nemophoto.egg-info/top_level.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       38 2023-06-12 15:59:23.847919 nemophoto-0.6.0/setup.cfg
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     3651 2023-06-12 15:56:49.000000 nemophoto-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:12:11.907997 nemophoto-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 20:11:57.000000 nemophoto-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 20:11:57.000000 nemophoto-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-27 20:12:11.907997 nemophoto-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-27 20:11:57.000000 nemophoto-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:12:11.907997 nemophoto-0.7.0/nemo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:11:57.000000 nemophoto-0.7.0/nemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-07-27 20:11:57.000000 nemophoto-0.7.0/nemo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 20:11:57.000000 nemophoto-0.7.0/nemo/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41742 2023-07-27 20:11:57.000000 nemophoto-0.7.0/nemo/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-27 20:11:57.000000 nemophoto-0.7.0/nemo/batch_lx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-07-27 20:11:57.000000 nemophoto-0.7.0/nemo/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:12:11.907997 nemophoto-0.7.0/nemophoto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-27 20:12:11.000000 nemophoto-0.7.0/nemophoto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-27 20:12:11.000000 nemophoto-0.7.0/nemophoto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:12:11.000000 nemophoto-0.7.0/nemophoto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-27 20:12:11.000000 nemophoto-0.7.0/nemophoto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 20:12:11.000000 nemophoto-0.7.0/nemophoto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-27 20:12:11.000000 nemophoto-0.7.0/nemophoto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:12:11.907997 nemophoto-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-27 20:11:57.000000 nemophoto-0.7.0/setup.py
```

### Comparing `nemophoto-0.6.0/LICENSE` & `nemophoto-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nemophoto-0.6.0/PKG-INFO` & `nemophoto-0.7.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,110 +1,94 @@
-Metadata-Version: 2.1
-Name: nemophoto
-Version: 0.6.0
-Summary: Absorption, fluorescence, phosphorescence spectrum simulations and ISC rate calculations.
-Home-page: https://github.com/LeonardoESousa/NEMO
-Author: Leonardo Evaristo de Sousa
-Author-email: ledso@dtu.dk
-License: MIT
-Description: 
-        # NEMO - Photophysics with the Nuclear Ensemble Method
-        
-        [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-        [![license](https://img.shields.io/github/license/LeonardoESousa/NEMO?style=plastic)]()
-        [![down](https://img.shields.io/pypi/dm/nemophoto)]()
-        [![maint](https://img.shields.io/maintenance/yes/2023)]()
-        [![commit](https://img.shields.io/github/last-commit/LeonardoESousa/NEMO?style=plastic)]()
-        
-        
-         Fluorescence, phosphorescence and intersystem crossing (ISC) rate calculations. Absorption, fluorescence and phosphorescence spectrum simulations. Förster radius and singlet exciton diffusion length estimates. Interfaces with the QChem package. 
-        
-        Table of Contents
-        =================
-        <!--ts-->
-        * [Cite as:](#cite-as)
-        * [What does this program do?](#what-does-this-program-do)
-        * [What is necessary to use it?](#what-is-necessary-to-use-it)
-        * [How to install it?](#how-to-install-it)
-        * [How to use it?](#how-to-use-it)
-           
-        <!--te-->
-        
-        ## Cite as:
-        
-        > Leonardo Evaristo de Sousa and Piotr de Silva
-        Journal of Chemical Theory and Computation 2021 17 (9), 5816-5824
-        DOI: 10.1021/acs.jctc.1c00476
-        
-        
-        ## What does this program do?
-        
-        1.  Photophysics with TD(A)-DFT:
-            - Calculates fluorescence and phosphorescence rates from an excited state.
-            - Calculates ISC rates from a given singlet state to several triplet states and vice-versa.
-            - Absorption, Fluorescence and Phosphorescence spectrum simulations.
-            - Rate calculations and spectra include vibrational contributions and state specific solvation effects.
-        2.  Exciton properties:   
-            - Calculates the Förster radius for transfers between two molecules of equal or different type.
-            - Estimates singlet exciton diffusion lengths.
-        
-            
-        ## What is necessary to use it?
-        
-         -  The program requires that the QChem quantum chemistry software be installed, since it interfaces with it.
-        
-         -  The first step for running spectrum calculations is providing either a QChem or Gaussian log file for a frequency calculation in the S0, S1 or T1 state, if the goal is computing an absorption, fluorescence or phosphorescence spectrum, respectively. All frequencies must be real.  
-        
-         -  For calculating ISC rates from the Sn state to different triplet states, a QChem/Gaussian frequency calculation at the Sn state must be provided.
-        
-         -  Similarly, for reverse ISC rates from the Tn state to different triplet states, a QChem/Gaussian frequency calculation at the Tn state must be provided.
-         
-         -  To obtain the estimates of Förster radius, fluorescence lifetimes and singlet exciton diffusion lengths, it is necessary to first perform both absorption and fluorescence spectra calculations for the molecule of interest.
-        
-        ## How to install it?
-        
-        Run:
-        
-        `pip install nemophoto`
-        
-        To get the latest commit, run:
-        
-        `pip install git+https://github.com/LeonardoESousa/NEMO`
-        
-        Alternatively, clone the repository to your computer. Inside the NEMO folder, run:
-        
-        `pip install .`
-        
-        Once installed, you should be able to run the program from any folder by just using the `nemo` command.
-        
-        ## How to use it?
-        
-        Here is a quick guide on how to use the software. For a detailed tutorial, click [here](https://github.com/LeonardoESousa/NEMO/blob/main/Tutorial/Tutorial.md).
-        
-        1. Initial steps:
-            - Create a folder for your project. Add the log file for the frequency calculation to your folder. If the frequency calculation was run with Gaussian, you must also provide a QChem input file containing some settings you wish to apply in the ensemble calculations (e.g. functional, basis set, omega value, charge and multiplicity etc). An example of such file (td.in) is provided [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples).
-            - A frequency calculation in the S0 state is suitable for computing an absorption spectrum. For fluorescence spectra and/or ISC rates calculations from Sn states to triplet states, a Sn frequency calculation is expected. Finally, for phosphorescence spectra and/or rISC rates calculations from Tn states to singlet states, a Tn frequency calculation is expected.  
-            - Run the `nemo` command. Choose option 1 and follow the instructions to select the parameters of the calculation. This includes the dielectric constant and refractive index of the medium. This information will be used to obtain state-specific solvent corrections to the TD(A)-DFT energies.  
-            - Add a bash script file to the folder. This file depends on which batch system you use. Examples of this file for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples)).
-            - Run the `nemo` command again, choose option 2 and follow the instructions. Alternatively, just run all calculations created in the Geometries folder. Once the calculations are running, you may use option 3 to check the progress or option 4 to abort.
-        
-        2. For absorption spectrum simulations:
-            - Once all calculations from step 1 are done, run the `nemo` command and choose option 5. Follow the instructions to set the parameters and the spectrum will be generated. 
-        
-        3. For photophysical rates:
-            - Once all calculations from step 1 are done, run the `nemo` command and choose option 6. Follow the instructions to set the parameters. Three files will be generated: an Ensemble file, with data from the ensemble of geometries; a differential_rate file, with the emission spectrum; a rates file, with all available rates (-> denote radiative transitions and ~> denote ISC transitions). 
-        
-        4. IMPORTANT:
-            - You may choose to calculate spectra and rates with different solvent dielectric constant and refractive index than the ones selected as input in Option 1. To do so, NEMO will resort to the extrapolation procedure described in ADD PAPER to adjust the results to the new solvent. 
-        
-        5. For exciton properties:
-            - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. Copy both spectra to a folder and inside this folder run the `nemo` command. Choose option 7. Follow the instructions to set the calculation parameters. A file will be generated with all the information. Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. These estimations follow from the procedures described in: "de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071." 
-        
-        
-        For better visualization of results, consider using  [Nemoview](https://github.com/LeonardoESousa/nemoview). 
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
+# NEMO - Photophysics with the Nuclear Ensemble Method
+
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![license](https://img.shields.io/github/license/LeonardoESousa/NEMO?style=plastic)]()
+[![down](https://img.shields.io/pypi/dm/nemophoto)]()
+[![maint](https://img.shields.io/maintenance/yes/2023)]()
+[![commit](https://img.shields.io/github/last-commit/LeonardoESousa/NEMO?style=plastic)]()
+
+
+ Fluorescence, phosphorescence and intersystem crossing (ISC) rate calculations. Absorption, fluorescence and phosphorescence spectrum simulations. Förster radius and singlet exciton diffusion length estimates. Interfaces with the QChem package. 
+
+Table of Contents
+=================
+<!--ts-->
+* [Cite as:](#cite-as)
+* [What does this program do?](#what-does-this-program-do)
+* [What is necessary to use it?](#what-is-necessary-to-use-it)
+* [How to install it?](#how-to-install-it)
+* [How to use it?](#how-to-use-it)
+   
+<!--te-->
+
+## Cite as:
+
+> Leonardo Evaristo de Sousa and Piotr de Silva
+Journal of Chemical Theory and Computation 2021 17 (9), 5816-5824
+DOI: 10.1021/acs.jctc.1c00476
+
+
+## What does this program do?
+
+1.  Photophysics with TD(A)-DFT:
+    - Calculates fluorescence and phosphorescence rates from an excited state.
+    - Calculates ISC rates from a given singlet state to several triplet states and vice-versa.
+    - Absorption, Fluorescence and Phosphorescence spectrum simulations.
+    - Rate calculations and spectra include vibrational contributions and state specific solvation effects.
+2.  Exciton properties:   
+    - Calculates the Förster radius for transfers between two molecules of equal or different type.
+    - Estimates singlet exciton diffusion lengths.
+
+    
+## What is necessary to use it?
+
+ -  The program requires that the QChem quantum chemistry software be installed, since it interfaces with it.
+
+ -  The first step for running spectrum calculations is providing either a QChem or Gaussian log file for a frequency calculation in the S0, S1 or T1 state, if the goal is computing an absorption, fluorescence or phosphorescence spectrum, respectively. All frequencies must be real.  
+
+ -  For calculating ISC rates from the Sn state to different triplet states, a QChem/Gaussian frequency calculation at the Sn state must be provided.
+
+ -  Similarly, for reverse ISC rates from the Tn state to different triplet states, a QChem/Gaussian frequency calculation at the Tn state must be provided.
+ 
+ -  To obtain the estimates of Förster radius, fluorescence lifetimes and singlet exciton diffusion lengths, it is necessary to first perform both absorption and fluorescence spectra calculations for the molecule of interest.
+
+## How to install it?
+
+Run:
+
+`pip install nemophoto`
+
+To get the latest commit, run:
+
+`pip install git+https://github.com/LeonardoESousa/NEMO`
+
+Alternatively, clone the repository to your computer. Inside the NEMO folder, run:
+
+`pip install .`
+
+Once installed, you should be able to run the program from any folder by just using the `nemo` command.
+
+## How to use it?
+
+Here is a quick guide on how to use the software. For a detailed tutorial, click [here](https://github.com/LeonardoESousa/NEMO/blob/main/Tutorial/Tutorial.md).
+
+1. Initial steps:
+    - Create a folder for your project. Add the log file for the frequency calculation to your folder. If the frequency calculation was run with Gaussian, you must also provide a QChem input file containing some settings you wish to apply in the ensemble calculations (e.g. functional, basis set, omega value, charge and multiplicity etc). An example of such file (td.in) is provided [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples).
+    - A frequency calculation in the S0 state is suitable for computing an absorption spectrum. For fluorescence spectra and/or ISC rates calculations from Sn states to triplet states, a Sn frequency calculation is expected. Finally, for phosphorescence spectra and/or rISC rates calculations from Tn states to singlet states, a Tn frequency calculation is expected.  
+    - Run the `nemo` command. Choose option 1 and follow the instructions to select the parameters of the calculation. This includes the dielectric constant and refractive index of the medium. This information will be used to obtain state-specific solvent corrections to the TD(A)-DFT energies.  
+    - Add a bash script file to the folder. This file depends on which batch system you use. Examples of this file for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples)).
+    - Run the `nemo` command again, choose option 2 and follow the instructions. Alternatively, just run all calculations created in the Geometries folder. Once the calculations are running, you may use option 3 to check the progress or option 4 to abort.
+
+2. For absorption spectrum simulations:
+    - Once all calculations from step 1 are done, run the `nemo` command and choose option 5. Follow the instructions to set the parameters and the spectrum will be generated. 
+
+3. For photophysical rates:
+    - Once all calculations from step 1 are done, run the `nemo` command and choose option 6. Follow the instructions to set the parameters. Three files will be generated: an Ensemble file, with data from the ensemble of geometries; a differential_rate file, with the emission spectrum; a rates file, with all available rates (-> denote radiative transitions and ~> denote ISC transitions). 
+
+4. IMPORTANT:
+    - You may choose to calculate spectra and rates with different solvent dielectric constant and refractive index than the ones selected as input in Option 1. To do so, NEMO will resort to the extrapolation procedure described in ADD PAPER to adjust the results to the new solvent. 
+
+5. For exciton properties:
+    - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. Copy both spectra to a folder and inside this folder run the `nemo` command. Choose option 7. Follow the instructions to set the calculation parameters. A file will be generated with all the information. Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. These estimations follow from the procedures described in: "de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071." 
+
+
+For better visualization of results, consider using  [Nemoview](https://github.com/LeonardoESousa/nemoview).
```

### Comparing `nemophoto-0.6.0/README.md` & `nemophoto-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: nemophoto
+Version: 0.7.0
+Summary: Absorption, fluorescence, phosphorescence spectrum simulations and ISC rate calculations.
+Home-page: https://github.com/LeonardoESousa/NEMO
+Author: Leonardo Evaristo de Sousa
+Author-email: ledso@dtu.dk
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # NEMO - Photophysics with the Nuclear Ensemble Method
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![license](https://img.shields.io/github/license/LeonardoESousa/NEMO?style=plastic)]()
 [![down](https://img.shields.io/pypi/dm/nemophoto)]()
 [![maint](https://img.shields.io/maintenance/yes/2023)]()
 [![commit](https://img.shields.io/github/last-commit/LeonardoESousa/NEMO?style=plastic)]()
```

### Comparing `nemophoto-0.6.0/nemo/__main__.py` & `nemophoto-0.7.0/nemo/__main__.py`

 * *Files identical despite different names*

### Comparing `nemophoto-0.6.0/nemo/analysis.py` & `nemophoto-0.7.0/nemo/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 ##GETS ENERGIES, OSCS, AND INDICES FOR Sn AND Tn STATES##################################
 def pega_energias(file):
     ss = 'Excited-state properties with   relaxed density'
     with open(file, 'r') as f:
         exc = False
         corr = False
-        correction = []
+        correction, correction2 = [], []
         for line in f:
             if 'TDDFT/TDA Excitation Energies' in line or 'TDDFT Excitation Energies' in line:
                 energies, spins, oscs, ind = [], [], [], []
                 exc = True
             elif ss in line:
                 corr = True
             elif 'Solute Internal Energy' in line:
@@ -60,29 +60,31 @@
                 spins.append(line.split()[1])
             elif 'Strength' in line and exc:
                 oscs.append(float(line.split()[2]))
             elif '---------------------------------------------------' in line and exc and len(energies) > 0:
                 exc = False
             elif 'SS-PCM correction' in line and corr:
                 correction.append(-1*float(line.split()[3]))
+            elif 'LR-PCM correction' in line and corr:
+                correction2.append(-2*float(line.split()[3]))    
             elif '------------------------ END OF SUMMARY -----------------------' in line and corr:
                 corr = False      
             elif 'Total energy in the final basis set' in line:
                 line = line.split()
                 total_nopcm =  float(line[8])    
         if len(correction) == 0: #When run on logs that do not employ pcm
             correction = np.zeros(len(energies))
             sol_int = total_nopcm
             total_free = total_nopcm
         singlets   = np.array([energies[i] for i in range(len(energies)) if spins[i] == 'Singlet'])
-        ss_s       = np.array([correction[i]   for i in range(len(correction))   if spins[i] == 'Singlet'])
+        ss_s       = np.array([correction[i]+correction2[i]   for i in range(len(correction))   if spins[i] == 'Singlet'])
         ind_s      = np.array([ind[i] for i in range(len(ind)) if spins[i] == 'Singlet'])
         oscs       = np.array([oscs[i] for i in range(len(energies)) if spins[i] == 'Singlet'])
         triplets   = np.array([energies[i] for i in range(len(energies)) if spins[i] == 'Triplet'])
-        ss_t       = np.array([correction[i]   for i in range(len(correction))   if spins[i] == 'Triplet'])
+        ss_t       = np.array([correction[i]+correction2[i]   for i in range(len(correction))   if spins[i] == 'Triplet'])
         ind_t      = np.array([ind[i] for i in range(len(ind)) if spins[i] == 'Triplet'])
         
         oscs       = np.array([x for _, x in zip(singlets, oscs)])
         ind_s      = np.array([x for _, x in zip(singlets, ind_s)])
         ind_t      = np.array([x for _, x in zip(triplets, ind_t)])
 
         order_s  = np.argsort(singlets)
@@ -712,15 +714,15 @@
         final_state   = Triplets - (alphaopt2/alphaopt1)*Ss_t
         socs_complete = data[[i for i in data.columns.values if f'soc_s' in i]].to_numpy()
         initial_state, final_state, Ss_s, Ss_t, socs_complete = reorder(initial_state, final_state, Ss_s, Ss_t, socs_complete)
         initial_state = initial_state[:,n_state]
         socs_complete = socs_complete[:,n_state,:]
         delta = final_state - np.repeat(initial_state[:,np.newaxis],final_state.shape[1],axis=1)
         lambda_b = (alphast2/alphaopt1 - alphaopt2/alphaopt1)*Ss_t
-        final    = [i.split('_')[2].upper() for i in data.columns.values if 'soc_s1' in i]
+        final    = [i.split('_')[2].upper() for i in data.columns.values if 'soc_'+initial.lower()+'_' in i]
         ##FOR WHEN IC IS AVAILABLE
         #socs_complete = np.hstack((socs_complete,0.0001*np.ones((Singlets.shape[0],Singlets.shape[1]-1))))
         #delta_ss = Singlets + np.repeat((alphast2/alphaopt1)*Ss_s[:,n_state][:,np.newaxis] - Singlets[:,n_state][:,np.newaxis],Singlets.shape[1],axis=1) - (alphaopt2/alphaopt1)*Ss_s    #Sm (final) - Sn (initial) + lambda_b
         #indices  = [i for i in range(Singlets.shape[1]) if i != n_state] #Removed Sn to Sn transfers
         #delta    = np.hstack((delta,delta_ss[:,indices]))
         #lambda_bt= (alphast2/alphaopt1 - alphaopt2/alphaopt1)*Ss_s
         #lambda_b = np.hstack((lambda_b,lambda_bt[:,indices]))
@@ -730,15 +732,15 @@
         final_state = Singlets - (alphaopt2/alphaopt1)*Ss_s
         socs_complete =  data[[i for i in data.columns.values if 'soc_t' in i and 's0' not in i and i.count('t') == 1]].to_numpy()
         initial_state, final_state, Ss_t, Ss_s, socs_complete = reorder(initial_state, final_state, Ss_t, Ss_s, socs_complete)
         initial_state = initial_state[:,n_state]
         socs_complete = socs_complete[:,n_state,:]
         delta = final_state - np.repeat(initial_state[:,np.newaxis],final_state.shape[1],axis=1)
         lambda_b = (alphast2/alphaopt1 - alphaopt2/alphaopt1)*Ss_s
-        final    = [i.split('_')[2].upper() for i in data.columns.values if 'soc_t1' in i and i.count('t') == 1]
+        final    = [i.split('_')[2].upper() for i in data.columns.values if 'soc_'+initial.lower()+'_' in i and i.count('t') == 1]
         #Tn to S0 ISC
         socs_s0 = data[[i for i in data.columns.values if f'soc_t' in i and 's0' in i]].to_numpy()
         socs_s0 = np.take_along_axis(socs_s0, argsort_emi, axis=1)
         socs_s0 = socs_s0[:,n_state]
         socs_complete = np.hstack((socs_s0[:,np.newaxis],socs_complete))
         delta = np.hstack((delta_emi[:,np.newaxis],delta))
         lambda_b = np.hstack((lambda_be[:,np.newaxis],lambda_b))
@@ -842,21 +844,22 @@
     oscs    = np.take_along_axis(oscs,argsort,axis=1)
     lambda_b= np.take_along_axis(lambda_b,argsort,axis=1)
     ds      = np.take_along_axis(ds,argsort,axis=1)	
     Ltotal = np.sqrt(2*lambda_b*kbT + kbT**2)
     left   = max(np.min(DE-2*Ltotal),0.01)
     right  = np.max(DE+2*Ltotal)    
     x      = np.linspace(left,right,int((right-left)/0.01))
-    # Add extra dimension to DE and Ltotal to match x shape
-    nstates = min(nstates,DE.shape[1])
+    if nstates == -1:
+        nstates = DE.shape[1]
+    # Add extra dimension to DE and Ltotal to match x shape    
     DE      = DE[:,:nstates,np.newaxis]
     Ltotal  = Ltotal[:,:nstates,np.newaxis]
     oscs  = oscs[:,:nstates,np.newaxis]
     lambda_b = lambda_b[:,:nstates,np.newaxis]
-    y      = constante*oscs*nemo.tools.gauss(x,(DE+lambda_b),Ltotal)
+    y      = constante*oscs*nemo.tools.gauss(x,DE,Ltotal)
     N      = oscs.shape[0]
     mean_y = np.sum(y,axis=0)/N 
     #Error estimate
     sigma    = np.sqrt(np.sum((y-mean_y)**2,axis=0)/(N*(N-1))) 
     mean_y = mean_y.T
     sigma  = sigma.T
     total = np.sum(mean_y,axis=1)
@@ -880,14 +883,15 @@
         np.savetxt(arquivo, np.hstack((x[:,np.newaxis],mean_y,sigma[:,np.newaxis])), fmt='%14.6f '+ fmt +' %14.6e', header=primeira)
         print(f'Spectrum printed in the {arquivo} file')
 
     # concatenate oscs[:,:,0] with DE[:,:,0] and ds
     colunas = [f'{initial.upper()}->{spin.upper()}{i}' for i in range(int(initial[1:])+1,int(initial[1:])+oscs.shape[1]+1)]
     colunas += [f'eng_{spin}{i}' for i in range(int(initial[1:])+1,int(initial[1:])+DE.shape[1]+1)]
     colunas += [f'chi_{spin}{i}' for i in range(int(initial[1:])+1,int(initial[1:])+ds.shape[1]+1)]
+    colunas += [f'sigma_{spin}{i}' for i in range(int(initial[1:])+1,int(initial[1:])+Ltotal.shape[1]+1)]
     # concatenate oscs[:,:,0] with DE[:,:,0] and ds
-    breakdown = pd.DataFrame(np.hstack((oscs[:,:,0],(DE+lambda_b)[:,:,0],ds/alphaopt1)),columns=colunas)
+    breakdown = pd.DataFrame(np.hstack((oscs[:,:,0],DE[:,:,0],ds/alphaopt1,Ltotal[:,:,0])),columns=colunas)
     if detailed:
         return abs_spec, breakdown
     else:
         return abs_spec          
 #########################################################################################
```

### Comparing `nemophoto-0.6.0/nemo/batch_lx.py` & `nemophoto-0.7.0/nemo/batch_lx.py`

 * *Files identical despite different names*

### Comparing `nemophoto-0.6.0/nemo/tools.py` & `nemophoto-0.7.0/nemo/tools.py`

 * *Files identical despite different names*

### Comparing `nemophoto-0.6.0/nemophoto.egg-info/PKG-INFO` & `nemophoto-0.7.0/nemophoto.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,110 @@
 Metadata-Version: 2.1
 Name: nemophoto
-Version: 0.6.0
+Version: 0.7.0
 Summary: Absorption, fluorescence, phosphorescence spectrum simulations and ISC rate calculations.
 Home-page: https://github.com/LeonardoESousa/NEMO
 Author: Leonardo Evaristo de Sousa
 Author-email: ledso@dtu.dk
 License: MIT
-Description: 
-        # NEMO - Photophysics with the Nuclear Ensemble Method
-        
-        [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-        [![license](https://img.shields.io/github/license/LeonardoESousa/NEMO?style=plastic)]()
-        [![down](https://img.shields.io/pypi/dm/nemophoto)]()
-        [![maint](https://img.shields.io/maintenance/yes/2023)]()
-        [![commit](https://img.shields.io/github/last-commit/LeonardoESousa/NEMO?style=plastic)]()
-        
-        
-         Fluorescence, phosphorescence and intersystem crossing (ISC) rate calculations. Absorption, fluorescence and phosphorescence spectrum simulations. Förster radius and singlet exciton diffusion length estimates. Interfaces with the QChem package. 
-        
-        Table of Contents
-        =================
-        <!--ts-->
-        * [Cite as:](#cite-as)
-        * [What does this program do?](#what-does-this-program-do)
-        * [What is necessary to use it?](#what-is-necessary-to-use-it)
-        * [How to install it?](#how-to-install-it)
-        * [How to use it?](#how-to-use-it)
-           
-        <!--te-->
-        
-        ## Cite as:
-        
-        > Leonardo Evaristo de Sousa and Piotr de Silva
-        Journal of Chemical Theory and Computation 2021 17 (9), 5816-5824
-        DOI: 10.1021/acs.jctc.1c00476
-        
-        
-        ## What does this program do?
-        
-        1.  Photophysics with TD(A)-DFT:
-            - Calculates fluorescence and phosphorescence rates from an excited state.
-            - Calculates ISC rates from a given singlet state to several triplet states and vice-versa.
-            - Absorption, Fluorescence and Phosphorescence spectrum simulations.
-            - Rate calculations and spectra include vibrational contributions and state specific solvation effects.
-        2.  Exciton properties:   
-            - Calculates the Förster radius for transfers between two molecules of equal or different type.
-            - Estimates singlet exciton diffusion lengths.
-        
-            
-        ## What is necessary to use it?
-        
-         -  The program requires that the QChem quantum chemistry software be installed, since it interfaces with it.
-        
-         -  The first step for running spectrum calculations is providing either a QChem or Gaussian log file for a frequency calculation in the S0, S1 or T1 state, if the goal is computing an absorption, fluorescence or phosphorescence spectrum, respectively. All frequencies must be real.  
-        
-         -  For calculating ISC rates from the Sn state to different triplet states, a QChem/Gaussian frequency calculation at the Sn state must be provided.
-        
-         -  Similarly, for reverse ISC rates from the Tn state to different triplet states, a QChem/Gaussian frequency calculation at the Tn state must be provided.
-         
-         -  To obtain the estimates of Förster radius, fluorescence lifetimes and singlet exciton diffusion lengths, it is necessary to first perform both absorption and fluorescence spectra calculations for the molecule of interest.
-        
-        ## How to install it?
-        
-        Run:
-        
-        `pip install nemophoto`
-        
-        To get the latest commit, run:
-        
-        `pip install git+https://github.com/LeonardoESousa/NEMO`
-        
-        Alternatively, clone the repository to your computer. Inside the NEMO folder, run:
-        
-        `pip install .`
-        
-        Once installed, you should be able to run the program from any folder by just using the `nemo` command.
-        
-        ## How to use it?
-        
-        Here is a quick guide on how to use the software. For a detailed tutorial, click [here](https://github.com/LeonardoESousa/NEMO/blob/main/Tutorial/Tutorial.md).
-        
-        1. Initial steps:
-            - Create a folder for your project. Add the log file for the frequency calculation to your folder. If the frequency calculation was run with Gaussian, you must also provide a QChem input file containing some settings you wish to apply in the ensemble calculations (e.g. functional, basis set, omega value, charge and multiplicity etc). An example of such file (td.in) is provided [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples).
-            - A frequency calculation in the S0 state is suitable for computing an absorption spectrum. For fluorescence spectra and/or ISC rates calculations from Sn states to triplet states, a Sn frequency calculation is expected. Finally, for phosphorescence spectra and/or rISC rates calculations from Tn states to singlet states, a Tn frequency calculation is expected.  
-            - Run the `nemo` command. Choose option 1 and follow the instructions to select the parameters of the calculation. This includes the dielectric constant and refractive index of the medium. This information will be used to obtain state-specific solvent corrections to the TD(A)-DFT energies.  
-            - Add a bash script file to the folder. This file depends on which batch system you use. Examples of this file for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples)).
-            - Run the `nemo` command again, choose option 2 and follow the instructions. Alternatively, just run all calculations created in the Geometries folder. Once the calculations are running, you may use option 3 to check the progress or option 4 to abort.
-        
-        2. For absorption spectrum simulations:
-            - Once all calculations from step 1 are done, run the `nemo` command and choose option 5. Follow the instructions to set the parameters and the spectrum will be generated. 
-        
-        3. For photophysical rates:
-            - Once all calculations from step 1 are done, run the `nemo` command and choose option 6. Follow the instructions to set the parameters. Three files will be generated: an Ensemble file, with data from the ensemble of geometries; a differential_rate file, with the emission spectrum; a rates file, with all available rates (-> denote radiative transitions and ~> denote ISC transitions). 
-        
-        4. IMPORTANT:
-            - You may choose to calculate spectra and rates with different solvent dielectric constant and refractive index than the ones selected as input in Option 1. To do so, NEMO will resort to the extrapolation procedure described in ADD PAPER to adjust the results to the new solvent. 
-        
-        5. For exciton properties:
-            - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. Copy both spectra to a folder and inside this folder run the `nemo` command. Choose option 7. Follow the instructions to set the calculation parameters. A file will be generated with all the information. Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. These estimations follow from the procedures described in: "de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071." 
-        
-        
-        For better visualization of results, consider using  [Nemoview](https://github.com/LeonardoESousa/nemoview). 
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# NEMO - Photophysics with the Nuclear Ensemble Method
+
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![license](https://img.shields.io/github/license/LeonardoESousa/NEMO?style=plastic)]()
+[![down](https://img.shields.io/pypi/dm/nemophoto)]()
+[![maint](https://img.shields.io/maintenance/yes/2023)]()
+[![commit](https://img.shields.io/github/last-commit/LeonardoESousa/NEMO?style=plastic)]()
+
+
+ Fluorescence, phosphorescence and intersystem crossing (ISC) rate calculations. Absorption, fluorescence and phosphorescence spectrum simulations. Förster radius and singlet exciton diffusion length estimates. Interfaces with the QChem package. 
+
+Table of Contents
+=================
+<!--ts-->
+* [Cite as:](#cite-as)
+* [What does this program do?](#what-does-this-program-do)
+* [What is necessary to use it?](#what-is-necessary-to-use-it)
+* [How to install it?](#how-to-install-it)
+* [How to use it?](#how-to-use-it)
+   
+<!--te-->
+
+## Cite as:
+
+> Leonardo Evaristo de Sousa and Piotr de Silva
+Journal of Chemical Theory and Computation 2021 17 (9), 5816-5824
+DOI: 10.1021/acs.jctc.1c00476
+
+
+## What does this program do?
+
+1.  Photophysics with TD(A)-DFT:
+    - Calculates fluorescence and phosphorescence rates from an excited state.
+    - Calculates ISC rates from a given singlet state to several triplet states and vice-versa.
+    - Absorption, Fluorescence and Phosphorescence spectrum simulations.
+    - Rate calculations and spectra include vibrational contributions and state specific solvation effects.
+2.  Exciton properties:   
+    - Calculates the Förster radius for transfers between two molecules of equal or different type.
+    - Estimates singlet exciton diffusion lengths.
+
+    
+## What is necessary to use it?
+
+ -  The program requires that the QChem quantum chemistry software be installed, since it interfaces with it.
+
+ -  The first step for running spectrum calculations is providing either a QChem or Gaussian log file for a frequency calculation in the S0, S1 or T1 state, if the goal is computing an absorption, fluorescence or phosphorescence spectrum, respectively. All frequencies must be real.  
+
+ -  For calculating ISC rates from the Sn state to different triplet states, a QChem/Gaussian frequency calculation at the Sn state must be provided.
+
+ -  Similarly, for reverse ISC rates from the Tn state to different triplet states, a QChem/Gaussian frequency calculation at the Tn state must be provided.
+ 
+ -  To obtain the estimates of Förster radius, fluorescence lifetimes and singlet exciton diffusion lengths, it is necessary to first perform both absorption and fluorescence spectra calculations for the molecule of interest.
+
+## How to install it?
+
+Run:
+
+`pip install nemophoto`
+
+To get the latest commit, run:
+
+`pip install git+https://github.com/LeonardoESousa/NEMO`
+
+Alternatively, clone the repository to your computer. Inside the NEMO folder, run:
+
+`pip install .`
+
+Once installed, you should be able to run the program from any folder by just using the `nemo` command.
+
+## How to use it?
+
+Here is a quick guide on how to use the software. For a detailed tutorial, click [here](https://github.com/LeonardoESousa/NEMO/blob/main/Tutorial/Tutorial.md).
+
+1. Initial steps:
+    - Create a folder for your project. Add the log file for the frequency calculation to your folder. If the frequency calculation was run with Gaussian, you must also provide a QChem input file containing some settings you wish to apply in the ensemble calculations (e.g. functional, basis set, omega value, charge and multiplicity etc). An example of such file (td.in) is provided [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples).
+    - A frequency calculation in the S0 state is suitable for computing an absorption spectrum. For fluorescence spectra and/or ISC rates calculations from Sn states to triplet states, a Sn frequency calculation is expected. Finally, for phosphorescence spectra and/or rISC rates calculations from Tn states to singlet states, a Tn frequency calculation is expected.  
+    - Run the `nemo` command. Choose option 1 and follow the instructions to select the parameters of the calculation. This includes the dielectric constant and refractive index of the medium. This information will be used to obtain state-specific solvent corrections to the TD(A)-DFT energies.  
+    - Add a bash script file to the folder. This file depends on which batch system you use. Examples of this file for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/NEMO/tree/main/batch_examples)).
+    - Run the `nemo` command again, choose option 2 and follow the instructions. Alternatively, just run all calculations created in the Geometries folder. Once the calculations are running, you may use option 3 to check the progress or option 4 to abort.
+
+2. For absorption spectrum simulations:
+    - Once all calculations from step 1 are done, run the `nemo` command and choose option 5. Follow the instructions to set the parameters and the spectrum will be generated. 
+
+3. For photophysical rates:
+    - Once all calculations from step 1 are done, run the `nemo` command and choose option 6. Follow the instructions to set the parameters. Three files will be generated: an Ensemble file, with data from the ensemble of geometries; a differential_rate file, with the emission spectrum; a rates file, with all available rates (-> denote radiative transitions and ~> denote ISC transitions). 
+
+4. IMPORTANT:
+    - You may choose to calculate spectra and rates with different solvent dielectric constant and refractive index than the ones selected as input in Option 1. To do so, NEMO will resort to the extrapolation procedure described in ADD PAPER to adjust the results to the new solvent. 
+
+5. For exciton properties:
+    - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. Copy both spectra to a folder and inside this folder run the `nemo` command. Choose option 7. Follow the instructions to set the calculation parameters. A file will be generated with all the information. Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. These estimations follow from the procedures described in: "de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071." 
+
+
+For better visualization of results, consider using  [Nemoview](https://github.com/LeonardoESousa/nemoview).
```

### Comparing `nemophoto-0.6.0/setup.py` & `nemophoto-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # Package meta-data.
 NAME = 'nemophoto'
 DESCRIPTION = 'Absorption, fluorescence, phosphorescence spectrum simulations and ISC rate calculations.'
 URL = 'https://github.com/LeonardoESousa/NEMO'
 EMAIL = 'ledso@dtu.dk'
 AUTHOR = 'Leonardo Evaristo de Sousa'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.6.0'
+VERSION = '0.7.0'
 
 # What packages are required for this module to be executed?
-REQUIRED = ['numpy', 'scipy', 'pandas', 'LeoX>=0.5.0']
+REQUIRED = ['numpy', 'scipy', 'pandas', 'LeoX>=0.6.1','wheel']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

