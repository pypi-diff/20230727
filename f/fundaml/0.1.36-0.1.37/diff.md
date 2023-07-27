# Comparing `tmp/fundaml-0.1.36.tar.gz` & `tmp/fundaml-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundaml-0.1.36.tar", max compression
+gzip compressed data, was "fundaml-0.1.37.tar", max compression
```

## Comparing `fundaml-0.1.36.tar` & `fundaml-0.1.37.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     1069 2023-07-27 00:19:23.374282 fundaml-0.1.36/LICENSE
--rw-r--r--   0        0        0     2284 2023-07-27 00:19:23.374282 fundaml-0.1.36/README.md
--rw-r--r--   0        0        0     1614 2023-07-27 00:34:08.709918 fundaml-0.1.36/pyproject.toml
--rw-r--r--   0        0        0      109 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/__init__.py
--rw-r--r--   0        0        0     1058 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/eda.py
--rw-r--r--   0        0        0     3247 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/models.py
--rw-r--r--   0        0        0     1032 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/scores.py
--rw-r--r--   0        0        0     3050 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/tokenizers.py
--rw-r--r--   0        0        0    17645 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/trainers.py
--rw-r--r--   0        0        0    24833 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/transformer_from_scratch.py
--rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 fundaml-0.1.36/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-07-27 01:30:55.592733 fundaml-0.1.37/LICENSE
+-rw-r--r--   0        0        0     2284 2023-07-27 01:30:55.592733 fundaml-0.1.37/README.md
+-rw-r--r--   0        0        0     1614 2023-07-27 01:47:01.483243 fundaml-0.1.37/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-27 01:30:55.964741 fundaml-0.1.37/src/fundaml/__init__.py
+-rw-r--r--   0        0        0     1058 2023-07-27 01:30:55.964741 fundaml-0.1.37/src/fundaml/eda.py
+-rw-r--r--   0        0        0     3247 2023-07-27 01:30:55.964741 fundaml-0.1.37/src/fundaml/models.py
+-rw-r--r--   0        0        0     1032 2023-07-27 01:30:55.964741 fundaml-0.1.37/src/fundaml/scores.py
+-rw-r--r--   0        0        0     3050 2023-07-27 01:30:55.964741 fundaml-0.1.37/src/fundaml/tokenizers.py
+-rw-r--r--   0        0        0    17645 2023-07-27 01:30:55.964741 fundaml-0.1.37/src/fundaml/trainers.py
+-rw-r--r--   0        0        0    25116 2023-07-27 01:30:55.964741 fundaml-0.1.37/src/fundaml/transformer_from_scratch.py
+-rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 fundaml-0.1.37/PKG-INFO
```

### Comparing `fundaml-0.1.36/LICENSE` & `fundaml-0.1.37/LICENSE`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.36/README.md` & `fundaml-0.1.37/README.md`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.36/pyproject.toml` & `fundaml-0.1.37/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fundaml"
-version = "0.1.36"
+version = "0.1.37"
 description = "A foundational machine learning library designed to streamline the end-to-end process of developing and deploying machine learning models. FundAML offers a broad array of tools and utilities for data preprocessing, model training, evaluation, and deployment, making it a fundamental solution for machine learning tasks."
 authors = ["Tony Zoght"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

### Comparing `fundaml-0.1.36/src/fundaml/eda.py` & `fundaml-0.1.37/src/fundaml/eda.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.36/src/fundaml/models.py` & `fundaml-0.1.37/src/fundaml/models.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.36/src/fundaml/scores.py` & `fundaml-0.1.37/src/fundaml/scores.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.36/src/fundaml/tokenizers.py` & `fundaml-0.1.37/src/fundaml/tokenizers.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.36/src/fundaml/trainers.py` & `fundaml-0.1.37/src/fundaml/trainers.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.36/src/fundaml/transformer_from_scratch.py` & `fundaml-0.1.37/src/fundaml/transformer_from_scratch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import torch
 import torch.nn as nn
-from torch.autograd import Variable
-
-import unittest
+import numpy as np
 
 def get_device():
-    # Check CUDA availability
     if torch.cuda.is_available():
         return torch.device('cuda')
     elif torch.backends.mps.is_available():
         return torch.device('mps')
     else:
         return torch.device('cpu')    
 
+def sinusoidal_positional_encoding(max_length, embed_size):
+    PE = torch.zeros(max_length, embed_size)
+    position = torch.arange(0, max_length, dtype=torch.float).unsqueeze(1)
+    div_term = torch.exp(torch.arange(0, embed_size, 2).float() * -(np.log(10000.0) / embed_size))
+    PE[:, 0::2] = torch.sin(position * div_term)
+    PE[:, 1::2] = torch.cos(position * div_term)
+    return PE
+
 class MultiHeadSelfAttentionBlock(nn.Module):
     """
     Initializes the MultiHeadSelfAttentionBlock module.
 
     Args:
         embedding_size (int): The size of the input embeddings. The value should be 
                             divisible by num_heads. This is because the embeddings 
@@ -261,15 +266,15 @@
         if device is None:
             self.device = get_device()
         else:
             self.device = device
 
         # Embeddings for the input words and positional embeddings
         self.word_embedding = nn.Embedding(src_vocab_size, embed_size)
-        self.position_embedding = nn.Embedding(max_length, embed_size)
+        self.position_embedding = sinusoidal_positional_encoding(max_length, embed_size).to(self.device)
 
         # Transformer blocks for the encoder layers
         self.layers = nn.ModuleList(
             [
                 TransformerBlock(
                     embed_size,
                     num_heads,
@@ -297,19 +302,16 @@
         """
 
         # Obtain the batch size and sequence length
         N, seq_length = x.shape
         x = x.to(self.device)
         mask = mask.to(self.device)
 
-        # Create positional indices
-        positions = torch.arange(0, seq_length).expand(N, seq_length).to(self.device)
-
         # Combine word embeddings and positional embeddings
-        embeddings = self.word_embedding(x) + self.position_embedding(positions)
+        embeddings = self.word_embedding(x) + self.position_embedding[:seq_length, :]
 
         # Apply dropout to the combined embeddings
         out = self.dropout(embeddings)
 
         # Pass the output through the layers
         for layer in self.layers:
             out = layer(out, out, out, mask)
@@ -409,15 +411,15 @@
         if device is None:
             self.device = get_device()
         else:
             self.device = device
 
         # Embeddings for the input words and positional embeddings
         self.word_embedding = nn.Embedding(trg_vocab_size, embed_size)
-        self.position_embedding = nn.Embedding(max_length, embed_size)
+        self.position_embedding = sinusoidal_positional_encoding(max_length, embed_size).to(self.device)
 
         # Decoder blocks for the decoder layers
         self.layers = nn.ModuleList(
             [
                 DecoderBlock(
                     embed_size,
                     num_heads,
@@ -455,15 +457,15 @@
         src_mask = src_mask.to(self.device)
         trg_mask = trg_mask.to(self.device)
 
         # Create positional indices
         positions = torch.arange(0, seq_length).expand(N, seq_length).to(self.device)
 
         # Combine word embeddings and positional embeddings
-        embeddings = self.word_embedding(x) + self.position_embedding(positions)
+        embeddings = self.word_embedding(x) + self.position_embedding[:seq_length, :]
 
         # Apply dropout to the combined embeddings
         x = self.dropout(embeddings)
 
         # Pass the output through the layers
         for layer in self.layers:
             x = layer(x, enc_out, enc_out, src_mask, trg_mask)
```

### Comparing `fundaml-0.1.36/PKG-INFO` & `fundaml-0.1.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundaml
-Version: 0.1.36
+Version: 0.1.37
 Summary: A foundational machine learning library designed to streamline the end-to-end process of developing and deploying machine learning models. FundAML offers a broad array of tools and utilities for data preprocessing, model training, evaluation, and deployment, making it a fundamental solution for machine learning tasks.
 License: MIT
 Author: Tony Zoght
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

