# Comparing `tmp/proteinflow-2.1.0.tar.gz` & `tmp/proteinflow-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-2.1.0.tar", last modified: Tue Jul 25 10:33:06 2023, max compression
+gzip compressed data, was "proteinflow-2.1.1.tar", last modified: Thu Jul 27 09:54:07 2023, max compression
```

## Comparing `proteinflow-2.1.0.tar` & `proteinflow-2.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.377544 proteinflow-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-25 10:32:48.000000 proteinflow-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-25 10:33:06.377544 proteinflow-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-07-25 10:32:48.000000 proteinflow-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.369544 proteinflow-2.1.0/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-25 10:32:48.000000 proteinflow-2.1.0/dev/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 10:32:48.000000 proteinflow-2.1.0/dev/update_init_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)    28053 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)    71926 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37617 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/data/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow/download/
--rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/download/boto.py
--rw-r--r--   0 runner    (1001) docker     (123)    36587 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/ligand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    18971 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.377544 proteinflow-2.1.0/proteinflow/split/
--rw-r--r--   0 runner    (1001) docker     (123)    50801 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/split/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-25 10:32:48.000000 proteinflow-2.1.0/proteinflow/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.373544 proteinflow-2.1.0/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-25 10:33:06.000000 proteinflow-2.1.0/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 10:33:06.000000 proteinflow-2.1.0/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:33:06.000000 proteinflow-2.1.0/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 10:33:06.000000 proteinflow-2.1.0/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-25 10:33:06.000000 proteinflow-2.1.0/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-25 10:33:06.000000 proteinflow-2.1.0/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-25 10:32:48.000000 proteinflow-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-25 10:33:06.377544 proteinflow-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:33:06.377544 proteinflow-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-25 10:32:48.000000 proteinflow-2.1.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-25 10:32:48.000000 proteinflow-2.1.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-25 10:32:48.000000 proteinflow-2.1.0/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-25 10:32:48.000000 proteinflow-2.1.0/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.244248 proteinflow-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-27 09:53:54.000000 proteinflow-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-27 09:54:07.244248 proteinflow-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-07-27 09:53:54.000000 proteinflow-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.240248 proteinflow-2.1.1/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-27 09:53:54.000000 proteinflow-2.1.1/dev/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 09:53:54.000000 proteinflow-2.1.1/dev/update_init_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.240248 proteinflow-2.1.1/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    27992 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.240248 proteinflow-2.1.1/proteinflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    71922 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37531 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/data/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.240248 proteinflow-2.1.1/proteinflow/download/
+-rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/download/boto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36587 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/ligand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.244248 proteinflow-2.1.1/proteinflow/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.244248 proteinflow-2.1.1/proteinflow/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.244248 proteinflow-2.1.1/proteinflow/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    18971 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.244248 proteinflow-2.1.1/proteinflow/split/
+-rw-r--r--   0 runner    (1001) docker     (123)    50801 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/split/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-07-27 09:53:54.000000 proteinflow-2.1.1/proteinflow/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.240248 proteinflow-2.1.1/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-27 09:54:07.000000 proteinflow-2.1.1/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 09:54:07.000000 proteinflow-2.1.1/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:54:07.000000 proteinflow-2.1.1/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 09:54:07.000000 proteinflow-2.1.1/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 09:54:07.000000 proteinflow-2.1.1/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 09:54:07.000000 proteinflow-2.1.1/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-27 09:53:54.000000 proteinflow-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-27 09:54:07.244248 proteinflow-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:54:07.244248 proteinflow-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-27 09:53:55.000000 proteinflow-2.1.1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-27 09:53:55.000000 proteinflow-2.1.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-27 09:53:55.000000 proteinflow-2.1.1/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 09:53:55.000000 proteinflow-2.1.1/tests/test_sabdab.py
```

### Comparing `proteinflow-2.1.0/LICENSE` & `proteinflow-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/PKG-INFO` & `proteinflow-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 2.1.0
+Version: 2.1.1
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 2.1.0 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 2.1.1 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-2.1.0/README.md` & `proteinflow-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/dev/bump_version.py` & `proteinflow-2.1.1/dev/bump_version.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/dev/update_init_docs.py` & `proteinflow-2.1.1/dev/update_init_docs.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/proteinflow/__init__.py` & `proteinflow-2.1.1/proteinflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,32 +166,29 @@
 """
 __pdoc__ = {
     "data.utils": False,
     "download.boto": False,
     "constants": False,
     "split": False,
     "cli": False,
-    "processing.ligand": False,
+    "ligand": False,
 }
 __docformat__ = "numpy"
 
 import os
-import pickle
 import random
 import shutil
-import socket
 import string
 import tempfile
 import warnings
 
 import boto3
 import numpy as np
 from botocore import UNSIGNED
 from botocore.config import Config
-from tqdm import tqdm
 
 from proteinflow.constants import SIDECHAIN_ORDER
 from proteinflow.data.torch import ProteinDataset, ProteinLoader
 from proteinflow.download import _download_dataset, _get_chain_pdb_ids
 from proteinflow.download.boto import _s3list
 from proteinflow.processing import run_processing
 from proteinflow.split import (
```

### Comparing `proteinflow-2.1.0/proteinflow/cli.py` & `proteinflow-2.1.1/proteinflow/cli.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/proteinflow/constants.py` & `proteinflow-2.1.1/proteinflow/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,16 +194,17 @@
 
 
 ###################################################################################
 ################################# PDB Constants ###################################
 ###################################################################################
 ALPHABET_PDB = "XACDEFGHIKLMNPQRSTVWY"
 
-ALPHABET_REVERSE = {x: i for i, x in enumerate(ALPHABET_PDB)}
-ALPHABET_REVERSE["-"] = 0
+ALPHABET_REVERSE = defaultdict(lambda: 0)
+for i, x in enumerate(ALPHABET_PDB):
+    ALPHABET_REVERSE[x] = i
 
 GLOBAL_PAD_CHAR = 0
 ONE_TO_THREE_LETTER_MAP = {
     "R": "ARG",
     "H": "HIS",
     "K": "LYS",
     "D": "ASP",
```

### Comparing `proteinflow-2.1.0/proteinflow/data/__init__.py` & `proteinflow-2.1.1/proteinflow/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
                 raise ValueError("Chain IDs must be unique")
             self.seq[chain] = entry.seq[chain]
             self.crd[chain] = entry.crd[chain]
             self.mask[chain] = entry.mask[chain]
             self.mask_original[chain] = entry.mask_original[chain]
             self.cdr[chain] = entry.cdr[chain]
             self.predict_mask[chain] = entry.predict_mask[chain]
-        if not all([x is None for x in entry.predict_mask.values()]):
+        if not all([x is None for x in self.predict_mask.values()]):
             for k, v in self.predict_mask.items():
                 if v is None:
                     self.predict_mask[k] = np.zeros(len(self.get_sequence(k)))
 
     @staticmethod
     def from_arrays(
         seqs, crds, masks, chain_id_dict, chain_id_array, predict_masks=None, cdrs=None
@@ -569,23 +569,24 @@
         """
         seqs_list = []
         crds_list = []
         masks_list = []
         chain_ids_list = []
         predict_masks_list = None if predict_masks is None else []
         cdrs_list = None if cdrs is None else []
-        if crds.shape[1] != 14:
-            crds_ = np.zeros((crds.shape[0], 14, 3))
-            crds_[:, :4, :] = ProteinEntry._to_numpy(crds)
-            crds = crds_
         for chain_id, ind in chain_id_dict.items():
             chain_ids_list.append(chain_id)
             chain_mask = chain_id_array == ind
             seqs_list.append(ProteinEntry.decode_sequence(seqs[chain_mask]))
-            crds_list.append(ProteinEntry._to_numpy(crds[chain_mask]))
+            if crds.shape[1] != 14:
+                crds_ = np.zeros((crds[chain_mask].shape[0], 14, 3))
+                crds_[:, :4, :] = ProteinEntry._to_numpy(crds[chain_mask])
+            else:
+                crds_ = ProteinEntry._to_numpy(crds[chain_mask])
+            crds_list.append(crds_)
             masks_list.append(ProteinEntry._to_numpy(masks[chain_mask]))
             if predict_masks is not None:
                 predict_masks_list.append(
                     ProteinEntry._to_numpy(predict_masks[chain_mask])
                 )
             if cdrs is not None:
                 cdrs_list.append(ProteinEntry.decode_cdr(cdrs[chain_mask]))
@@ -1252,19 +1253,17 @@
             `self.predict_mask` is not `None`, the predicted residues are highlighted
         style : str, default 'cartoon'
             The style of the visualization; one of 'cartoon', 'sphere', 'stick', 'line', 'cross'
         opacity : float or dict, default 1
             Opacity of the visualization (can be a dictionary mapping from chain IDs to opacity values)
 
         """
-        print(f"{highlight_mask=}")
         if highlight_mask is not None:
             highlight_mask_dict = self._get_highlight_mask_dict(highlight_mask)
         elif list(self.predict_mask.values())[0] is not None:
-            print("HERE")
             highlight_mask_dict = {
                 chain: self.predict_mask[chain][self.get_mask([chain]).astype(bool)]
                 for chain in self.get_chains()
             }
         else:
             highlight_mask_dict = None
         with tempfile.NamedTemporaryFile(suffix=".pdb") as tmp:
```

### Comparing `proteinflow-2.1.0/proteinflow/data/torch.py` & `proteinflow-2.1.1/proteinflow/data/torch.py`

 * *Files 0% similar despite different names*

```diff
@@ -676,17 +676,15 @@
                             if length > 0
                         ]
                     ):
                         add_name = False
                         pass_set = True
 
                 if self.entry_type == "pair":
-                    # intersect = []
                     if not data_entry.is_valid_pair(*chain_set):
-                        # if not all(intersect):
                         pass_set = True
                         add_name = False
             if pass_set:
                 continue
 
             out = {}
             out["pdb_id"] = no_extension_name.split("-")[0]
```

### Comparing `proteinflow-2.1.0/proteinflow/data/utils.py` & `proteinflow-2.1.1/proteinflow/data/utils.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/proteinflow/download/__init__.py` & `proteinflow-2.1.1/proteinflow/download/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/proteinflow/download/boto.py` & `proteinflow-2.1.1/proteinflow/download/boto.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/proteinflow/ligand.py` & `proteinflow-2.1.1/proteinflow/ligand.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/proteinflow/logging/__init__.py` & `proteinflow-2.1.1/proteinflow/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/proteinflow/metrics/__init__.py` & `proteinflow-2.1.1/proteinflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/proteinflow/processing/__init__.py` & `proteinflow-2.1.1/proteinflow/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/proteinflow/split/__init__.py` & `proteinflow-2.1.1/proteinflow/split/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/proteinflow/split/utils.py` & `proteinflow-2.1.1/proteinflow/split/utils.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/proteinflow/visualize.py` & `proteinflow-2.1.1/proteinflow/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 import numpy as np
 import py3Dmol
 
 from proteinflow.data import PDBEntry, ProteinEntry
 
 
 def show_animation_from_pdb(
-    pdb_paths, highlight_mask_dict=None, style="cartoon", opacity=1
+    pdb_paths, highlight_mask_dict=None, style="cartoon", opacity=1, direction="forward"
 ):
     """Show an animation of the given PDB files.
 
     Parameters
     ----------
     pdb_paths : list of str
         List of paths to PDB files.
     highlight_mask_dict : dict, optional
         Dictionary of masks to highlight. The keys are the names of the chains, and the values are `numpy` arrays of
         1s and 0s, where 1s indicate the atoms to highlight.
     style : str, optional
         The style of the visualization; one of 'cartoon', 'sphere', 'stick', 'line', 'cross'
     opacity : float, default 1
         The opacity of the visualization.
+    direction : {"forward", "backAndForth"}
+        The direction of the animation.
 
     """
     entries = [PDBEntry(path) for path in pdb_paths]
     models = ""
     for i, mol in enumerate(entries):
         models += "MODEL " + str(i) + "\n"
         atoms = mol._get_atom_dicts(
@@ -40,34 +42,40 @@
     view.addModelsAsFrames(models)
 
     for i, at in enumerate(atoms):
         default = {"cartoon": {"color": "black"}}
         view.setStyle({"model": -1, "serial": i + 1}, at.get("pymol", default))
 
     view.zoomTo()
-    view.animate({"loop": "forward"})
+    view.animate({"loop": direction, "step": 10})
     view.show()
 
 
 def show_animation_from_pickle(
-    pickle_paths, highlight_mask=None, style="cartoon", opacity=1
+    pickle_paths,
+    highlight_mask=None,
+    style="cartoon",
+    opacity=1,
+    direction="forward",
 ):
     """Show an animation of the given pickle files.
 
     Parameters
     ----------
     pickle_paths : list of str
         List of paths to pickle files.
     highlight_mask : numpy.ndarray, optional
         Mask to highlight. 1s indicate the atoms to highlight; assumes
         the chains to be concatenated in alphabetical order.
     style : str, optional
         The style of the visualization; one of 'cartoon', 'sphere', 'stick', 'line', 'cross'
     opacity : float, default 1
         The opacity of the visualization.
+    direction : {"forward", "backAndForth"}
+        The direction of the animation.
 
     """
     entries = [ProteinEntry.from_pickle(path) for path in pickle_paths]
     models = ""
     for i, mol in enumerate(entries):
         models += "MODEL " + str(i) + "\n"
         if highlight_mask is None:
@@ -82,15 +90,15 @@
     view.addModelsAsFrames(models)
 
     for i, at in enumerate(atoms):
         default = {"cartoon": {"color": "black"}}
         view.setStyle({"model": -1, "serial": i + 1}, at.get("pymol", default))
 
     view.zoomTo()
-    view.animate({"loop": "forward"})
+    view.animate({"loop": direction})
     view.show()
 
 
 def merge_pickle_files(paths_to_merge, save_path):
     """Merge the given pickle files into a single file.
 
     Parameters
@@ -110,15 +118,15 @@
         merged_entry.to_pdb(save_path)
     elif save_path.endswith(".pickle"):
         merged_entry.to_pickle(save_path)
     else:
         raise ValueError("save_path must end with .pdb or .pickle")
 
 
-def show_merged_pickle(file_paths, highlight_masks=None, style="cartoon", opacity=1):
+def show_merged_pickle(file_paths, highlight_masks=None, style="cartoon", opacity=1.0):
     """Show a merged visualization of the given PDB or pickle files.
 
     Parameters
     ----------
     file_paths : list of str
         List of paths to PDB or pickle files.
     highlight_masks : list of numpy.ndarray, optional
@@ -150,15 +158,17 @@
     else:
         highlight_mask = None
     merged_entry.visualize(
         style=style, highlight_mask=highlight_mask, opacity=opacity_dict
     )
 
 
-def show_merged_pdb(file_paths, highlight_mask_dicts=None, style="cartoon", opacity=1):
+def show_merged_pdb(
+    file_paths, highlight_mask_dicts=None, style="cartoon", opacity=1.0
+):
     """Show a merged visualization of the given PDB or pickle files.
 
     Parameters
     ----------
     file_paths : list of str
         List of paths to PDB or pickle files.
     highlight_mask_dicts : list of dict, optional
```

### Comparing `proteinflow-2.1.0/proteinflow.egg-info/PKG-INFO` & `proteinflow-2.1.1/proteinflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 2.1.0
+Version: 2.1.1
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 2.1.0 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 2.1.1 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-2.1.0/proteinflow.egg-info/SOURCES.txt` & `proteinflow-2.1.1/proteinflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/pyproject.toml` & `proteinflow-2.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `proteinflow-2.1.0/tests/test_download.py` & `proteinflow-2.1.1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/tests/test_entry.py` & `proteinflow-2.1.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/tests/test_generate.py` & `proteinflow-2.1.1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.1.0/tests/test_sabdab.py` & `proteinflow-2.1.1/tests/test_sabdab.py`

 * *Files identical despite different names*

