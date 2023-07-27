# Comparing `tmp/bisum-0.1.tar.gz` & `tmp/bisum-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/julio/Desktop/bisum/dist/.tmp-lgxvmaqd/bisum-0.1.tar", last modified: Wed Jul 26 23:50:58 2023, max compression
+gzip compressed data, was "/home/julio/Desktop/bisum/dist/.tmp-z71p3ngb/bisum-0.1.1.tar", last modified: Thu Jul 27 00:30:05 2023, max compression
```

## Comparing `bisum-0.1.tar` & `bisum-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-07-26 23:50:58.000000 bisum-0.1/
--rw-rw-r--   0 julio     (1000) julio     (1000)     1071 2023-07-26 22:53:26.000000 bisum-0.1/LICENSE
--rw-rw-r--   0 julio     (1000) julio     (1000)       26 2023-07-26 23:40:19.000000 bisum-0.1/MANIFEST.in
--rw-rw-r--   0 julio     (1000) julio     (1000)     2029 2023-07-26 23:50:58.000000 bisum-0.1/PKG-INFO
--rw-rw-r--   0 julio     (1000) julio     (1000)     1388 2023-07-26 22:53:26.000000 bisum-0.1/README.md
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-07-26 23:50:58.000000 bisum-0.1/bisum/
--rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-07-26 22:53:26.000000 bisum-0.1/bisum/__init__.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     3339 2023-07-26 22:53:26.000000 bisum-0.1/bisum/bisum.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     2245 2023-07-26 22:53:26.000000 bisum-0.1/bisum/dense_intra.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     6508 2023-07-26 22:53:26.000000 bisum-0.1/bisum/generic_functions.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     5557 2023-07-26 22:53:26.000000 bisum-0.1/bisum/labels.py
--rw-rw-r--   0 julio     (1000) julio     (1000)    10330 2023-07-26 22:53:26.000000 bisum-0.1/bisum/sparse_intra.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     9237 2023-07-26 22:53:26.000000 bisum-0.1/bisum/tensor_to_matrix.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     9687 2023-07-26 22:53:26.000000 bisum-0.1/bisum/tensordot.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     4124 2023-07-26 22:53:26.000000 bisum-0.1/bisum/test_bisum.py
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-07-26 23:50:58.000000 bisum-0.1/bisum.egg-info/
--rw-rw-r--   0 julio     (1000) julio     (1000)     2029 2023-07-26 23:50:58.000000 bisum-0.1/bisum.egg-info/PKG-INFO
--rw-rw-r--   0 julio     (1000) julio     (1000)      376 2023-07-26 23:50:58.000000 bisum-0.1/bisum.egg-info/SOURCES.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-07-26 23:50:58.000000 bisum-0.1/bisum.egg-info/dependency_links.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        6 2023-07-26 23:50:58.000000 bisum-0.1/bisum.egg-info/requires.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        6 2023-07-26 23:50:58.000000 bisum-0.1/bisum.egg-info/top_level.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       79 2023-07-26 23:50:58.000000 bisum-0.1/setup.cfg
--rw-rw-r--   0 julio     (1000) julio     (1000)     1584 2023-07-26 23:44:51.000000 bisum-0.1/setup.py
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-07-27 00:30:05.000000 bisum-0.1.1/
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1071 2023-07-26 22:53:26.000000 bisum-0.1.1/LICENSE
+-rw-rw-r--   0 julio     (1000) julio     (1000)       26 2023-07-26 23:40:19.000000 bisum-0.1.1/MANIFEST.in
+-rw-rw-r--   0 julio     (1000) julio     (1000)     2030 2023-07-27 00:30:05.000000 bisum-0.1.1/PKG-INFO
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1387 2023-07-27 00:29:17.000000 bisum-0.1.1/README.md
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum/
+-rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-07-26 22:53:26.000000 bisum-0.1.1/bisum/__init__.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     3345 2023-07-26 23:58:42.000000 bisum-0.1.1/bisum/bisum.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     2246 2023-07-26 23:59:03.000000 bisum-0.1.1/bisum/dense_intra.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     6508 2023-07-26 22:53:26.000000 bisum-0.1.1/bisum/generic_functions.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     5560 2023-07-26 23:59:24.000000 bisum-0.1.1/bisum/labels.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)    10331 2023-07-27 00:20:46.000000 bisum-0.1.1/bisum/sparse_intra.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     9238 2023-07-26 23:59:35.000000 bisum-0.1.1/bisum/tensor_to_matrix.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     9689 2023-07-26 23:59:41.000000 bisum-0.1.1/bisum/tensordot.py
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum.egg-info/
+-rw-rw-r--   0 julio     (1000) julio     (1000)     2030 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum.egg-info/PKG-INFO
+-rw-rw-r--   0 julio     (1000) julio     (1000)      356 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum.egg-info/SOURCES.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum.egg-info/dependency_links.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)        6 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum.egg-info/requires.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)        6 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum.egg-info/top_level.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)       79 2023-07-27 00:30:05.000000 bisum-0.1.1/setup.cfg
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1586 2023-07-27 00:06:38.000000 bisum-0.1.1/setup.py
```

### Comparing `bisum-0.1/LICENSE` & `bisum-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bisum-0.1/PKG-INFO` & `bisum-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisum
-Version: 0.1
+Version: 0.1.1
 Summary: binary sparse and dense tensor partial-tracing
 Home-page: https://github.com/jcandane/bisum/
 Author: Julio Candanedo
 Author-email: juliojcandanedo@gmail.com
 License: MIT
 Keywords: pytorch,torch,tensors,Sparse Tensor,Sparse,contraction,partial-tracing,einsum,tensordot,attention
 Classifier: Development Status :: 3 - Alpha
@@ -23,21 +23,21 @@
 2. ncon (used in the tensor-network community, list of 1d int torch.tensor, labelling each tensor axis)
 3. adjacency-matrix (as in numpy.tensordot, (2,n) 2d int torch.tensor, with n being the number of indices idenified between the two tensors)
 
 ## API
 
 Let's begin by initializing the 2 tensors, we can initialize random-sparse-tensors 
 ```python
-import bisum
+from bisum.bisum import bisum
 import torch
 
 shape_A = torch.tensor([8,7,7,4,11,6])
 shape_B = torch.tensor([9,7,3,7,11,8])
-A = bisum(shape_A, density=0.05)
-B = bisum(shape_B, density=0.05)
+A = torch.rand(shape_A)
+B = torch.rand(shape_B)
 ```
 
 Suppose we would like to compute the following partial-trace/tensor-contraction $C_{njwl} = A_{iksndj} B_{wklsdi}$:
 ```python
 C_einsum = bisum("iksndj, wklsdi -> njwl", A, B)
 C_ncon   = bisum([[-1,-2,-3,4,-5,6],[1,-2,3,-3,-5,-1]], A, B)
 C_adjmat = bisum(torch.tensor([[0,1,2,4],[5,1,3,4]]), A, B)
```

### Comparing `bisum-0.1/README.md` & `bisum-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 2. ncon (used in the tensor-network community, list of 1d int torch.tensor, labelling each tensor axis)
 3. adjacency-matrix (as in numpy.tensordot, (2,n) 2d int torch.tensor, with n being the number of indices idenified between the two tensors)
 
 ## API
 
 Let's begin by initializing the 2 tensors, we can initialize random-sparse-tensors 
 ```python
-import bisum
+from bisum.bisum import bisum
 import torch
 
 shape_A = torch.tensor([8,7,7,4,11,6])
 shape_B = torch.tensor([9,7,3,7,11,8])
-A = bisum(shape_A, density=0.05)
-B = bisum(shape_B, density=0.05)
+A = torch.rand(shape_A)
+B = torch.rand(shape_B)
 ```
 
 Suppose we would like to compute the following partial-trace/tensor-contraction $C_{njwl} = A_{iksndj} B_{wklsdi}$:
 ```python
 C_einsum = bisum("iksndj, wklsdi -> njwl", A, B)
 C_ncon   = bisum([[-1,-2,-3,4,-5,6],[1,-2,3,-3,-5,-1]], A, B)
 C_adjmat = bisum(torch.tensor([[0,1,2,4],[5,1,3,4]]), A, B)
```

### Comparing `bisum-0.1/bisum/bisum.py` & `bisum-0.1.1/bisum/bisum.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 Primary Function of the bisum package, for sparse & dense tensor partial-tracing
 """
 
 import torch
 
 ###
-from labels import einsumstr_to_labels, ncon_to_labels
-from tensordot import ss_tensordot , sd_tensordot , sd_tensordot
-from tensordot import ss_tensordot_, sd_tensordot_, ds_tensordot_
-from dense_intra import den_tensor_intraTr, den_post_intraTr, den_post_trans
+from .labels import einsumstr_to_labels, ncon_to_labels
+from .tensordot import ss_tensordot , sd_tensordot , sd_tensordot
+from .tensordot import ss_tensordot_, sd_tensordot_, ds_tensordot_
+from .dense_intra import den_tensor_intraTr, den_post_intraTr, den_post_trans
 
-from sparse_intra import spa_post_trans, spa_tensor_intraTr, spa_post_intraTr 
-from sparse_intra import spa_post_trans_, spa_tensor_intraTr_, spa_post_intraTr_
+from .sparse_intra import spa_post_trans, spa_tensor_intraTr, spa_post_intraTr 
+from .sparse_intra import spa_post_trans_, spa_tensor_intraTr_, spa_post_intraTr_
 
 def bisum(Rx, a, b):
     """
 
     """
     if torch.is_tensor(Rx): # and Rx.shape[0]==2:  # is adj.matrix (no post transpose nor slice) 
         if (not a.is_sparse) and (not b.is_sparse): ## both dense
```

### Comparing `bisum-0.1/bisum/dense_intra.py` & `bisum-0.1.1/bisum/dense_intra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 dense_intra.py
 
 This contains functions for processing dense tensor intra-operations (slicing & tracing).
 """
 
 import torch
-from generic_functions import first_occurrence_mask, pytorch_delete, iargsort
+from .generic_functions import first_occurrence_mask, pytorch_delete, iargsort
 
 ### given LHS && intra-traces compute reduced/sliced sparse-tensor
 @torch.jit.script
 def den_post_trans(a, rhs, RHS):
     if torch.numel(RHS)>0:
         rhs=rhs[first_occurrence_mask(rhs)]
         j  = torch.argsort(rhs)
```

### Comparing `bisum-0.1/bisum/generic_functions.py` & `bisum-0.1.1/bisum/generic_functions.py`

 * *Files identical despite different names*

### Comparing `bisum-0.1/bisum/labels.py` & `bisum-0.1.1/bisum/labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 labels.py
 
 Einsum-string and ncon Label processing.
 """
 
-import torch
-from generic_functions import first_occurrence_mask
 from typing import List
+import torch
+
+from .generic_functions import first_occurrence_mask
+
 
 @torch.jit.script
 def einsumstr_to_labels(einsum_string : str, device : torch.device=torch.device("cpu")):
     """
     GIVEN : einsum_string (str, numpy.einsum-string)
     GET   : LHS (List[1d-int-torch.tensors] labelling each tensor in einsum_string)
             RHS (1d-int-torch.tensor labelling external indices of output tensor)
```

### Comparing `bisum-0.1/bisum/sparse_intra.py` & `bisum-0.1.1/bisum/sparse_intra.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 sparse_intra.py
 
 This contains functions for processing sparse tensor intra-operations (slicing & tracing).
 """
 
 import torch
-from generic_functions import first_occurrence_mask, lexsort, iargsort
+from .generic_functions import first_occurrence_mask, lexsort, iargsort
 
 ### given LHS && intra-traces compute reduced/sliced sparse-tensor
 
 @torch.jit.script
 def spa_post_trans(a, rhs, RHS):
     rhs=rhs[first_occurrence_mask(rhs)]
     j = torch.argsort(rhs)
```

### Comparing `bisum-0.1/bisum/tensor_to_matrix.py` & `bisum-0.1.1/bisum/tensor_to_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 tensor_to_matrix.py
 
 Fold dense and sparse tensors into matrices (dense or sparse)
 """
 
 import torch
-from generic_functions import pytorch_delete, tuples_to_ints
+from .generic_functions import pytorch_delete, tuples_to_ints
 
 
 @torch.jit.script
 def rawsp_tensor_to_matrix(index, data, shape_, adj_matrix, left : bool = True):
     """ !!!! tensor_in should instead be:    indices, data, shape (as tensors), because by DEAFULT SparseTensors change index types to int64 :(
     *** Fold a Tensor with given external xor internal indices into a external-internal matrix
     GIVEN : index (2d-int-torch.tensor)
```

### Comparing `bisum-0.1/bisum/tensordot.py` & `bisum-0.1.1/bisum/tensordot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 tensordot.py
 
 This generalizes tensordot for sparse tensors (with dense tensors).
 """
 
 import torch
-from generic_functions import ints_to_tuples, cartesian_product
-from tensor_to_matrix import sp_tensor_to_matrix, dn_tensor_to_matrix, rawsp_tensor_to_matrix
+from .generic_functions import ints_to_tuples, cartesian_product
+from .tensor_to_matrix import sp_tensor_to_matrix, dn_tensor_to_matrix, rawsp_tensor_to_matrix
 
 @torch.jit.script
 def sd_outer(a, b):
     """
     GIVEN : a (sparse)
             b (dense)
     GET   : c   (torch.tensor{dense})
```

### Comparing `bisum-0.1/bisum.egg-info/PKG-INFO` & `bisum-0.1.1/bisum.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisum
-Version: 0.1
+Version: 0.1.1
 Summary: binary sparse and dense tensor partial-tracing
 Home-page: https://github.com/jcandane/bisum/
 Author: Julio Candanedo
 Author-email: juliojcandanedo@gmail.com
 License: MIT
 Keywords: pytorch,torch,tensors,Sparse Tensor,Sparse,contraction,partial-tracing,einsum,tensordot,attention
 Classifier: Development Status :: 3 - Alpha
@@ -23,21 +23,21 @@
 2. ncon (used in the tensor-network community, list of 1d int torch.tensor, labelling each tensor axis)
 3. adjacency-matrix (as in numpy.tensordot, (2,n) 2d int torch.tensor, with n being the number of indices idenified between the two tensors)
 
 ## API
 
 Let's begin by initializing the 2 tensors, we can initialize random-sparse-tensors 
 ```python
-import bisum
+from bisum.bisum import bisum
 import torch
 
 shape_A = torch.tensor([8,7,7,4,11,6])
 shape_B = torch.tensor([9,7,3,7,11,8])
-A = bisum(shape_A, density=0.05)
-B = bisum(shape_B, density=0.05)
+A = torch.rand(shape_A)
+B = torch.rand(shape_B)
 ```
 
 Suppose we would like to compute the following partial-trace/tensor-contraction $C_{njwl} = A_{iksndj} B_{wklsdi}$:
 ```python
 C_einsum = bisum("iksndj, wklsdi -> njwl", A, B)
 C_ncon   = bisum([[-1,-2,-3,4,-5,6],[1,-2,3,-3,-5,-1]], A, B)
 C_adjmat = bisum(torch.tensor([[0,1,2,4],[5,1,3,4]]), A, B)
```

### Comparing `bisum-0.1/setup.py` & `bisum-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as readme:
     long_description = readme.read()
 
 setup(
   name = 'bisum',         # How you named your package folder (MyLib)
   packages = ['bisum'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.1.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = "binary sparse and dense tensor partial-tracing",   # Give a short description about your library
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Julio Candanedo',                   # Type in your name
   author_email = 'juliojcandanedo@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/jcandane/bisum/',   # Provide either the link to your github or to your website
```

