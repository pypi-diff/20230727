# Comparing `tmp/RXN4Chemistry-1.7.0.tar.gz` & `tmp/RXN4Chemistry-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RXN4Chemistry-1.7.0.tar", last modified: Fri Feb 17 15:42:54 2023, max compression
+gzip compressed data, was "RXN4Chemistry-1.8.0.tar", last modified: Thu Jul 27 07:25:06 2023, max compression
```

## Comparing `RXN4Chemistry-1.7.0.tar` & `RXN4Chemistry-1.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:42:54.662895 RXN4Chemistry-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-17 15:42:53.000000 RXN4Chemistry-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-02-17 15:42:54.662895 RXN4Chemistry-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-02-17 15:42:53.000000 RXN4Chemistry-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:42:54.662895 RXN4Chemistry-1.7.0/RXN4Chemistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-02-17 15:42:54.000000 RXN4Chemistry-1.7.0/RXN4Chemistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-17 15:42:54.000000 RXN4Chemistry-1.7.0/RXN4Chemistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 15:42:54.000000 RXN4Chemistry-1.7.0/RXN4Chemistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-17 15:42:54.000000 RXN4Chemistry-1.7.0/RXN4Chemistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:42:54.000000 RXN4Chemistry-1.7.0/RXN4Chemistry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-17 15:42:53.000000 RXN4Chemistry-1.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:42:54.662895 RXN4Chemistry-1.7.0/rxn4chemistry/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-17 15:42:53.000000 RXN4Chemistry-1.7.0/rxn4chemistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-02-17 15:42:53.000000 RXN4Chemistry-1.7.0/rxn4chemistry/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    47048 2023-02-17 15:42:53.000000 RXN4Chemistry-1.7.0/rxn4chemistry/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-02-17 15:42:53.000000 RXN4Chemistry-1.7.0/rxn4chemistry/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-02-17 15:42:53.000000 RXN4Chemistry-1.7.0/rxn4chemistry/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-02-17 15:42:53.000000 RXN4Chemistry-1.7.0/rxn4chemistry/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-02-17 15:42:53.000000 RXN4Chemistry-1.7.0/rxn4chemistry/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 15:42:54.662895 RXN4Chemistry-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-02-17 15:42:53.000000 RXN4Chemistry-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:25:06.734037 RXN4Chemistry-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-27 07:25:02.000000 RXN4Chemistry-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-07-27 07:25:06.734037 RXN4Chemistry-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-07-27 07:25:02.000000 RXN4Chemistry-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:25:06.730038 RXN4Chemistry-1.8.0/RXN4Chemistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-07-27 07:25:06.000000 RXN4Chemistry-1.8.0/RXN4Chemistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-27 07:25:06.000000 RXN4Chemistry-1.8.0/RXN4Chemistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 07:25:06.000000 RXN4Chemistry-1.8.0/RXN4Chemistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 07:25:06.000000 RXN4Chemistry-1.8.0/RXN4Chemistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 07:25:06.000000 RXN4Chemistry-1.8.0/RXN4Chemistry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 07:25:03.000000 RXN4Chemistry-1.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:25:06.734037 RXN4Chemistry-1.8.0/rxn4chemistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-27 07:25:03.000000 RXN4Chemistry-1.8.0/rxn4chemistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-27 07:25:03.000000 RXN4Chemistry-1.8.0/rxn4chemistry/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46986 2023-07-27 07:25:03.000000 RXN4Chemistry-1.8.0/rxn4chemistry/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-27 07:25:03.000000 RXN4Chemistry-1.8.0/rxn4chemistry/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-07-27 07:25:03.000000 RXN4Chemistry-1.8.0/rxn4chemistry/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-07-27 07:25:03.000000 RXN4Chemistry-1.8.0/rxn4chemistry/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 07:25:03.000000 RXN4Chemistry-1.8.0/rxn4chemistry/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 07:25:06.734037 RXN4Chemistry-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-27 07:25:03.000000 RXN4Chemistry-1.8.0/setup.py
```

### Comparing `RXN4Chemistry-1.7.0/LICENSE` & `RXN4Chemistry-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RXN4Chemistry-1.7.0/PKG-INFO` & `RXN4Chemistry-1.8.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: RXN4Chemistry
-Version: 1.7.0
-Summary: Python wrapper for IBM RXN for Chemistry
-Home-page: https://github.com/rxn4chemistry/rxn4chemistry
-Author: RXN for Chemistry team
-Author-email: phs@zurich.ibm.com, tte@zurich.ibm.com, obc@zurich.ibm.com, ava@zurich.ibm.com, dpr@zurich.ibm.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python wrapper for the IBM RXN for Chemistry API
 
 [![Actions tests](https://github.com/rxn4chemistry/rxn4chemistry/actions/workflows/ci.yml/badge.svg)](https://github.com/rxn4chemistry/rxn4chemistry/actions)
 [![PyPI version](https://badge.fury.io/py/RXN4Chemistry.svg)](https://badge.fury.io/py/RXN4Chemistry)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/rxn4chemistry/rxn4chemistry/main)
 
@@ -73,17 +55,17 @@
 rxn4chemistry_wrapper = RXN4ChemistryWrapper(api_key=api_key)
 # NOTE: you can create a project or set an esiting one using:
 # rxn4chemistry_wrapper.set_project('PROJECT_ID')
 rxn4chemistry_wrapper.create_project('test_wrapper')
 print(rxn4chemistry_wrapper.project_id)
 ```
 
-### Reaction prediction
+### Reaction outcome prediction
 
-Running a reaction prediction is as simple as:
+Running a reaction outcome prediction is as simple as:
 
 ```python
 response = rxn4chemistry_wrapper.predict_reaction(
     'BrBr.c1ccc2cc3ccccc3cc2c1'
 )
 results = rxn4chemistry_wrapper.get_predict_reaction_results(
     response['prediction_id']
@@ -136,14 +118,44 @@
     response['prediction_id']
 )
 print(results['status'])
 # NOTE: upon 'SUCCESS' you can inspect the predicted retrosynthetic paths.
 print(results['retrosynthetic_paths'][0])
 ```
 
+
+### Prediction of reaction properties (atom-to-atom mapping, reaction yield, ...)
+
+Prediction of atom-to-atom mapping (see [paper](https://doi.org/10.1126/sciadv.abe4166)):
+```python
+response = rxn4chemistry_wrapper.predict_reaction_properties(
+    reactions=[
+        "CC(C)S.CN(C)C=O.Fc1cccnc1F.O=C([O-])[O-].[K+].[K+]>>CC(C)Sc1ncccc1F",
+        "C1COCCO1.CC(C)(C)OC(=O)CONC(=O)NCc1cccc2ccccc12.Cl>>O=C(O)CONC(=O)NCc1cccc2ccccc12",
+        "C=CCN=C=S.CNCc1ccc(C#N)cc1.NNC(=O)c1cn2c(n1)CCCC2>>C=CCN1C(C2=CN3CCCCC3=N2)=NN=C1N(C)CC1=CC=C(C#N)C=C1",
+    ],
+    ai_model="atom-mapping-2020",
+)
+for predicted_mapping_dict in response["response"]["payload"]["content"]:
+    print(predicted_mapping_dict["value"])
+```
+
+Prediction of reaction yields (see [paper](https://doi.org/10.1088/2632-2153/abc81d)):
+```python
+response = rxn4chemistry_wrapper.predict_reaction_properties(
+    reactions=[
+        "Clc1ccccn1.Cc1ccc(N)cc1.O=S(=O)(O[Pd]1c2ccccc2-c2ccccc2N~1)C(F)(F)F.COc1ccc(OC)c(P([C@]23C[C@H]4C[C@H](C[C@H](C4)C2)C3)[C@]23C[C@H]4C[C@H](C[C@H](C4)C2)C3)c1-c1c(C(C)C)cc(C(C)C)cc1C(C)C.CCN=P(N=P(N(C)C)(N(C)C)N(C)C)(N(C)C)N(C)C.Cc1cc(C)on1>>Cc1ccc(Nc2ccccn2)cc1",
+        "Brc1ccccn1.Cc1ccc(N)cc1.O=S(=O)(O[Pd]1c2ccccc2-c2ccccc2N~1)C(F)(F)F.COc1ccc(OC)c(P([C@]23C[C@H]4C[C@H](C[C@H](C4)C2)C3)[C@]23C[C@H]4C[C@H](C[C@H](C4)C2)C3)c1-c1c(C(C)C)cc(C(C)C)cc1C(C)C.CCN=P(N=P(N(C)C)(N(C)C)N(C)C)(N(C)C)N(C)C.COC(=O)c1ccno1>>Cc1ccc(Nc2ccccn2)cc1",
+    ],
+    ai_model="yield-2020-08-10",
+)
+for predicted_yield_dict in response["response"]["payload"]["content"]:
+    print(predicted_yield_dict["value"])
+```
+
 ### Create a synthesis and start it on the robot (or simulator)
 
 Create a synthesis from a retrosynthesis sequence:
 
 ```python
 # Each retrosynthetic path predicted has a unique sequence_id that can
 # be used to create a new synthesis
@@ -224,9 +236,7 @@
 ## Examples
 
 To learn more see the [examples](./examples).
 
 ## Documentation
 
 The documentation is hosted [here](https://rxn4chemistry.github.io/rxn4chemistry/) using GitHub pages.
-
-
```

### Comparing `RXN4Chemistry-1.7.0/README.md` & `RXN4Chemistry-1.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: RXN4Chemistry
+Version: 1.8.0
+Summary: Python wrapper for IBM RXN for Chemistry
+Home-page: https://github.com/rxn4chemistry/rxn4chemistry
+Author: RXN for Chemistry team
+Author-email: phs@zurich.ibm.com, tte@zurich.ibm.com, obc@zurich.ibm.com, ava@zurich.ibm.com, dpr@zurich.ibm.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Python wrapper for the IBM RXN for Chemistry API
 
 [![Actions tests](https://github.com/rxn4chemistry/rxn4chemistry/actions/workflows/ci.yml/badge.svg)](https://github.com/rxn4chemistry/rxn4chemistry/actions)
 [![PyPI version](https://badge.fury.io/py/RXN4Chemistry.svg)](https://badge.fury.io/py/RXN4Chemistry)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/rxn4chemistry/rxn4chemistry/main)
 
@@ -55,17 +73,17 @@
 rxn4chemistry_wrapper = RXN4ChemistryWrapper(api_key=api_key)
 # NOTE: you can create a project or set an esiting one using:
 # rxn4chemistry_wrapper.set_project('PROJECT_ID')
 rxn4chemistry_wrapper.create_project('test_wrapper')
 print(rxn4chemistry_wrapper.project_id)
 ```
 
-### Reaction prediction
+### Reaction outcome prediction
 
-Running a reaction prediction is as simple as:
+Running a reaction outcome prediction is as simple as:
 
 ```python
 response = rxn4chemistry_wrapper.predict_reaction(
     'BrBr.c1ccc2cc3ccccc3cc2c1'
 )
 results = rxn4chemistry_wrapper.get_predict_reaction_results(
     response['prediction_id']
@@ -118,14 +136,44 @@
     response['prediction_id']
 )
 print(results['status'])
 # NOTE: upon 'SUCCESS' you can inspect the predicted retrosynthetic paths.
 print(results['retrosynthetic_paths'][0])
 ```
 
+
+### Prediction of reaction properties (atom-to-atom mapping, reaction yield, ...)
+
+Prediction of atom-to-atom mapping (see [paper](https://doi.org/10.1126/sciadv.abe4166)):
+```python
+response = rxn4chemistry_wrapper.predict_reaction_properties(
+    reactions=[
+        "CC(C)S.CN(C)C=O.Fc1cccnc1F.O=C([O-])[O-].[K+].[K+]>>CC(C)Sc1ncccc1F",
+        "C1COCCO1.CC(C)(C)OC(=O)CONC(=O)NCc1cccc2ccccc12.Cl>>O=C(O)CONC(=O)NCc1cccc2ccccc12",
+        "C=CCN=C=S.CNCc1ccc(C#N)cc1.NNC(=O)c1cn2c(n1)CCCC2>>C=CCN1C(C2=CN3CCCCC3=N2)=NN=C1N(C)CC1=CC=C(C#N)C=C1",
+    ],
+    ai_model="atom-mapping-2020",
+)
+for predicted_mapping_dict in response["response"]["payload"]["content"]:
+    print(predicted_mapping_dict["value"])
+```
+
+Prediction of reaction yields (see [paper](https://doi.org/10.1088/2632-2153/abc81d)):
+```python
+response = rxn4chemistry_wrapper.predict_reaction_properties(
+    reactions=[
+        "Clc1ccccn1.Cc1ccc(N)cc1.O=S(=O)(O[Pd]1c2ccccc2-c2ccccc2N~1)C(F)(F)F.COc1ccc(OC)c(P([C@]23C[C@H]4C[C@H](C[C@H](C4)C2)C3)[C@]23C[C@H]4C[C@H](C[C@H](C4)C2)C3)c1-c1c(C(C)C)cc(C(C)C)cc1C(C)C.CCN=P(N=P(N(C)C)(N(C)C)N(C)C)(N(C)C)N(C)C.Cc1cc(C)on1>>Cc1ccc(Nc2ccccn2)cc1",
+        "Brc1ccccn1.Cc1ccc(N)cc1.O=S(=O)(O[Pd]1c2ccccc2-c2ccccc2N~1)C(F)(F)F.COc1ccc(OC)c(P([C@]23C[C@H]4C[C@H](C[C@H](C4)C2)C3)[C@]23C[C@H]4C[C@H](C[C@H](C4)C2)C3)c1-c1c(C(C)C)cc(C(C)C)cc1C(C)C.CCN=P(N=P(N(C)C)(N(C)C)N(C)C)(N(C)C)N(C)C.COC(=O)c1ccno1>>Cc1ccc(Nc2ccccn2)cc1",
+    ],
+    ai_model="yield-2020-08-10",
+)
+for predicted_yield_dict in response["response"]["payload"]["content"]:
+    print(predicted_yield_dict["value"])
+```
+
 ### Create a synthesis and start it on the robot (or simulator)
 
 Create a synthesis from a retrosynthesis sequence:
 
 ```python
 # Each retrosynthetic path predicted has a unique sequence_id that can
 # be used to create a new synthesis
@@ -206,7 +254,9 @@
 ## Examples
 
 To learn more see the [examples](./examples).
 
 ## Documentation
 
 The documentation is hosted [here](https://rxn4chemistry.github.io/rxn4chemistry/) using GitHub pages.
+
+
```

### Comparing `RXN4Chemistry-1.7.0/RXN4Chemistry.egg-info/PKG-INFO` & `RXN4Chemistry-1.8.0/RXN4Chemistry.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RXN4Chemistry
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python wrapper for IBM RXN for Chemistry
 Home-page: https://github.com/rxn4chemistry/rxn4chemistry
 Author: RXN for Chemistry team
 Author-email: phs@zurich.ibm.com, tte@zurich.ibm.com, obc@zurich.ibm.com, ava@zurich.ibm.com, dpr@zurich.ibm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -73,17 +73,17 @@
 rxn4chemistry_wrapper = RXN4ChemistryWrapper(api_key=api_key)
 # NOTE: you can create a project or set an esiting one using:
 # rxn4chemistry_wrapper.set_project('PROJECT_ID')
 rxn4chemistry_wrapper.create_project('test_wrapper')
 print(rxn4chemistry_wrapper.project_id)
 ```
 
-### Reaction prediction
+### Reaction outcome prediction
 
-Running a reaction prediction is as simple as:
+Running a reaction outcome prediction is as simple as:
 
 ```python
 response = rxn4chemistry_wrapper.predict_reaction(
     'BrBr.c1ccc2cc3ccccc3cc2c1'
 )
 results = rxn4chemistry_wrapper.get_predict_reaction_results(
     response['prediction_id']
@@ -136,14 +136,44 @@
     response['prediction_id']
 )
 print(results['status'])
 # NOTE: upon 'SUCCESS' you can inspect the predicted retrosynthetic paths.
 print(results['retrosynthetic_paths'][0])
 ```
 
+
+### Prediction of reaction properties (atom-to-atom mapping, reaction yield, ...)
+
+Prediction of atom-to-atom mapping (see [paper](https://doi.org/10.1126/sciadv.abe4166)):
+```python
+response = rxn4chemistry_wrapper.predict_reaction_properties(
+    reactions=[
+        "CC(C)S.CN(C)C=O.Fc1cccnc1F.O=C([O-])[O-].[K+].[K+]>>CC(C)Sc1ncccc1F",
+        "C1COCCO1.CC(C)(C)OC(=O)CONC(=O)NCc1cccc2ccccc12.Cl>>O=C(O)CONC(=O)NCc1cccc2ccccc12",
+        "C=CCN=C=S.CNCc1ccc(C#N)cc1.NNC(=O)c1cn2c(n1)CCCC2>>C=CCN1C(C2=CN3CCCCC3=N2)=NN=C1N(C)CC1=CC=C(C#N)C=C1",
+    ],
+    ai_model="atom-mapping-2020",
+)
+for predicted_mapping_dict in response["response"]["payload"]["content"]:
+    print(predicted_mapping_dict["value"])
+```
+
+Prediction of reaction yields (see [paper](https://doi.org/10.1088/2632-2153/abc81d)):
+```python
+response = rxn4chemistry_wrapper.predict_reaction_properties(
+    reactions=[
+        "Clc1ccccn1.Cc1ccc(N)cc1.O=S(=O)(O[Pd]1c2ccccc2-c2ccccc2N~1)C(F)(F)F.COc1ccc(OC)c(P([C@]23C[C@H]4C[C@H](C[C@H](C4)C2)C3)[C@]23C[C@H]4C[C@H](C[C@H](C4)C2)C3)c1-c1c(C(C)C)cc(C(C)C)cc1C(C)C.CCN=P(N=P(N(C)C)(N(C)C)N(C)C)(N(C)C)N(C)C.Cc1cc(C)on1>>Cc1ccc(Nc2ccccn2)cc1",
+        "Brc1ccccn1.Cc1ccc(N)cc1.O=S(=O)(O[Pd]1c2ccccc2-c2ccccc2N~1)C(F)(F)F.COc1ccc(OC)c(P([C@]23C[C@H]4C[C@H](C[C@H](C4)C2)C3)[C@]23C[C@H]4C[C@H](C[C@H](C4)C2)C3)c1-c1c(C(C)C)cc(C(C)C)cc1C(C)C.CCN=P(N=P(N(C)C)(N(C)C)N(C)C)(N(C)C)N(C)C.COC(=O)c1ccno1>>Cc1ccc(Nc2ccccn2)cc1",
+    ],
+    ai_model="yield-2020-08-10",
+)
+for predicted_yield_dict in response["response"]["payload"]["content"]:
+    print(predicted_yield_dict["value"])
+```
+
 ### Create a synthesis and start it on the robot (or simulator)
 
 Create a synthesis from a retrosynthesis sequence:
 
 ```python
 # Each retrosynthetic path predicted has a unique sequence_id that can
 # be used to create a new synthesis
```

### Comparing `RXN4Chemistry-1.7.0/rxn4chemistry/callbacks.py` & `RXN4Chemistry-1.8.0/rxn4chemistry/callbacks.py`

 * *Files identical despite different names*

### Comparing `RXN4Chemistry-1.7.0/rxn4chemistry/core.py` & `RXN4Chemistry-1.8.0/rxn4chemistry/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1096,48 +1096,45 @@
         """
 
         raise DeprecationWarning("Deprecated method use get_node_ids() to get the node ids and get_reaction_settings() to get the actions of a synthesis procedure!")
 
 
     @response_handling(success_status_code=200, on_success=default_on_success)
     @ibm_rxn_api_limits
-    def predict_reaction_properties_from_smiles(
+    def predict_reaction_properties(
         self,
         reactions: List[str],
-        ai_model: str = "atom-mapping-2020-08-20",
+        ai_model: str = "atom-mapping-2020",
     ) -> requests.models.Response:
         """
-        Launch prediction with given reactions SMILES.
+        Launch prediction with given reaction SMILES strings.
 
         Args:
-            ai_model (str, optional): model flavour and release. Defaults to
-                'atom-mapping-2020-08-20'.
-            reactions (List[str]): list of reaction smiles to predict reaction properties.
-
+            reactions: list of reaction smiles to predict reaction properties.
+            ai_model: model flavour and release. "atom-mapping-2020" for the default
+                atom mapping model, "yield-2020-08-10" for the default yield model.
         Returns:
-            dict: dictionary containing the
-            response.
+            dict: dictionary containing the response.
 
         Examples:
             Predict reaction properties by providing the reaction SMILES and aiModel:
 
             >>> response = rxn4chemistry_wrapper.predict_reaction_properties_from_smiles(
-                reactions=["CCCCCCO >> CCCCCCCO"],
-                ai_model="atom-mapping-2020-08-20"
-            )
+            ...     reactions=["CCCCCCO>>CCCCCCCO"],
+            ...     ai_model="atom-mapping-2020"
+            ... )
         """
-        raise NotImplementedError("This endpoint is not available for use yet.")
-        # data = {"aiModel": ai_model, "reactions": reactions, }
-        # response = requests.post(
-        #     self.routes.reaction_prediction_batch_url,
-        #     headers=self.headers,
-        #     data=json.dumps(data),
-        #     cookies={},
-        # )
-        # return response
+        data = {"aiModel": ai_model, "reactions": reactions, }
+        response = requests.post(
+            self.routes.reaction_properties_predictions_from_smiles_url,
+            headers=self.headers,
+            data=json.dumps(data),
+            cookies={},
+        )
+        return response
 
     @response_handling(success_status_code=200, on_success=default_on_success)
     @ibm_rxn_api_limits
     def current_user(self) -> requests.models.Response:
         """
         Get user info of the current user API key
```

### Comparing `RXN4Chemistry-1.7.0/rxn4chemistry/decorators.py` & `RXN4Chemistry-1.8.0/rxn4chemistry/decorators.py`

 * *Files identical despite different names*

### Comparing `RXN4Chemistry-1.7.0/rxn4chemistry/response_handler.py` & `RXN4Chemistry-1.8.0/rxn4chemistry/response_handler.py`

 * *Files identical despite different names*

### Comparing `RXN4Chemistry-1.7.0/rxn4chemistry/urls.py` & `RXN4Chemistry-1.8.0/rxn4chemistry/urls.py`

 * *Files identical despite different names*

### Comparing `RXN4Chemistry-1.7.0/rxn4chemistry/utilities.py` & `RXN4Chemistry-1.8.0/rxn4chemistry/utilities.py`

 * *Files identical despite different names*

### Comparing `RXN4Chemistry-1.7.0/setup.py` & `RXN4Chemistry-1.8.0/setup.py`

 * *Files identical despite different names*

