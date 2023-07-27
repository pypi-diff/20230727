# Comparing `tmp/genet-0.7.2-py3-none-any.whl.zip` & `tmp/genet-0.7.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 37812 bytes, number of entries: 23
+Zip file size: 37771 bytes, number of entries: 23
 -rw-rw-rw-  2.0 fat      109 b- defN 22-Sep-02 12:38 genet/__init__.py
 -rw-rw-rw-  2.0 fat      113 b- defN 23-May-22 14:53 genet/main.py
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Dec-23 13:58 genet/analysis/__init__.py
 -rw-rw-rw-  2.0 fat    10745 b- defN 23-May-22 14:53 genet/analysis/functional.py
 -rw-rw-rw-  2.0 fat      229 b- defN 22-Nov-23 13:11 genet/database/__init__.py
 -rw-rw-rw-  2.0 fat     8457 b- defN 23-May-22 14:53 genet/database/functional.py
 -rw-rw-rw-  2.0 fat     3275 b- defN 23-May-27 06:47 genet/design/DesignUtils.py
@@ -10,16 +10,16 @@
 -rw-rw-rw-  2.0 fat    42517 b- defN 23-Jul-27 16:14 genet/design/functional.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Sep-08 11:29 genet/design/ref_transcripts.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Aug-21 12:34 genet/design/modules/__init__.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jul-27 16:14 genet/models/__init__.py
 -rw-rw-rw-  2.0 fat     5264 b- defN 23-Jul-27 16:14 genet/models/constants.py
 -rw-rw-rw-  2.0 fat     4729 b- defN 23-Jul-27 16:14 genet/models/functional.py
 -rw-rw-rw-  2.0 fat      172 b- defN 22-Nov-23 13:18 genet/predict/__init__.py
--rw-rw-rw-  2.0 fat    44460 b- defN 23-Jul-27 16:41 genet/predict/functional.py
--rw-rw-rw-  2.0 fat      180 b- defN 23-Jul-27 16:44 genet/utils/__init__.py
+-rw-rw-rw-  2.0 fat    44350 b- defN 23-Jul-27 17:50 genet/predict/functional.py
+-rw-rw-rw-  2.0 fat      180 b- defN 23-Jul-27 17:49 genet/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2150 b- defN 23-Jul-27 16:14 genet/utils/functional.py
 -rw-rw-rw-  2.0 fat       43 b- defN 22-Aug-21 11:37 tests/__init__.py
--rw-rw-rw-  2.0 fat    14237 b- defN 23-Jul-27 16:45 genet-0.7.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 16:45 genet-0.7.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-27 16:45 genet-0.7.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1830 b- defN 23-Jul-27 16:45 genet-0.7.2.dist-info/RECORD
-23 files, 138894 bytes uncompressed, 34862 bytes compressed:  74.9%
+-rw-rw-rw-  2.0 fat    14237 b- defN 23-Jul-27 17:51 genet-0.7.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 17:51 genet-0.7.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-27 17:51 genet-0.7.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1830 b- defN 23-Jul-27 17:51 genet-0.7.3.dist-info/RECORD
+23 files, 138784 bytes uncompressed, 34821 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -51,20 +51,20 @@
 
 Filename: genet/utils/functional.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
-Filename: genet-0.7.2.dist-info/METADATA
+Filename: genet-0.7.3.dist-info/METADATA
 Comment: 
 
-Filename: genet-0.7.2.dist-info/WHEEL
+Filename: genet-0.7.3.dist-info/WHEEL
 Comment: 
 
-Filename: genet-0.7.2.dist-info/top_level.txt
+Filename: genet-0.7.3.dist-info/top_level.txt
 Comment: 
 
-Filename: genet-0.7.2.dist-info/RECORD
+Filename: genet-0.7.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genet/predict/functional.py

```diff
@@ -1,21 +1,16 @@
 # from genet.utils import *
 import genet
 import genet.utils
-from genet import models
 
 import torch
 import torch.nn.functional as F
 import torch.nn as nn
 
-import inspect
-from genet.predict.models import DeepSpCas9, DeepPrime
-
-
-import os, sys, time, regex, logging
+import os, sys, regex, logging
 import numpy as np
 import pandas as pd
 
 import tensorflow.compat.v1 as tf
 
 from glob import glob
 from Bio.SeqUtils import MeltingTemp as mt
@@ -114,15 +109,14 @@
         Dict = {model.inputs: TEST_X[i * test_batch:(i + 1) * test_batch], model.is_training: False}
         TEST_Z[i * test_batch:(i + 1) * test_batch] = sess.run([model.outputs], feed_dict=Dict)[0]
 
     list_score = sum(TEST_Z.tolist(), [])
 
     return list_score
 
-
 # def end: Model_Finaltest
 
 
 
 def preprocess_seq(data, seq_length):
 
     seq_onehot = np.zeros((len(data), 1, seq_length, 4), dtype=float)
```

## genet/utils/__init__.py

```diff
@@ -1,10 +1,10 @@
 from .functional import *
 
 # for PyPI release
 # python setup.py bdist_wheel
 # twine upload dist/genet-0.5.2-py3-none-any.whl
 
-version_ = '0.7.2'
+version_ = '0.7.3'
 
 __version__ = version_
```

## Comparing `genet-0.7.2.dist-info/METADATA` & `genet-0.7.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genet
-Version: 0.7.2
+Version: 0.7.3
 Summary: GenET: Genome Editing Toolkit
 Home-page: https://github.com/Goosang-Yu/genet
 Author: Goosang Yu
 Author-email: gsyu93@gmail.com
 Project-URL: Bug Tracker, https://github.com/Goosang-Yu/genet/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
```

## Comparing `genet-0.7.2.dist-info/RECORD` & `genet-0.7.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 genet/design/functional.py,sha256=_FKn1blEyss5YJz7aX1S2PPMFnpowDF89rrynE3rP34,42517
 genet/design/ref_transcripts.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/design/modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/models/__init__.py,sha256=oqpwg8SwNvIfhVzmhiO026lqxUY01r40Dgdgtaip0so,77
 genet/models/constants.py,sha256=AuwsY2GnvcWzOGHdmigj7hATvwt5LT2A_b_OSDvsoKQ,5264
 genet/models/functional.py,sha256=mMXjcfm2Sx6VLNz_yvusAeUVeTi3rM-3Nqrxd1DncdU,4729
 genet/predict/__init__.py,sha256=ttUFncDBsvsNY_si2brLck0UUDqGX0pUN7w_CA1k-JQ,172
-genet/predict/functional.py,sha256=61uF4iQbqC5mFN4Vf4G6SYNnEd3-3DIT14TWlYSXJ3s,44460
-genet/utils/__init__.py,sha256=n9E9FAOuaUV1EgrWSx1NhFBPQayfr5HE-ISgNH4dxyE,180
+genet/predict/functional.py,sha256=aZs1Czjv3gLy53HETFwtTiFo6ldJirzgGU-GeDjLv1o,44350
+genet/utils/__init__.py,sha256=pAExFBdb9S352xpFtpnGHogupvDR1UAE6nzO96jpVs8,180
 genet/utils/functional.py,sha256=25qi_DaqhQk8E4WINfjdbachK9t5o3TMQ1RR85kfvK0,2150
 tests/__init__.py,sha256=BFhp5tyle0b2qhFpJ7tnbbjdPbPsWyi5aGVTUuNma7Y,43
-genet-0.7.2.dist-info/METADATA,sha256=EMStfjZuMyTYjwYaT2gt45tCCbdUPM3LmyRjoDOxNdc,14237
-genet-0.7.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-genet-0.7.2.dist-info/top_level.txt,sha256=r0lGZefzJjcHRFTtVrLE2EjICxN1ZkBKsFV_fgu3DuE,12
-genet-0.7.2.dist-info/RECORD,,
+genet-0.7.3.dist-info/METADATA,sha256=UXh426JSc8C90-38E4H0EPeNIZ3fwwbzD2VjyOShjWA,14237
+genet-0.7.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+genet-0.7.3.dist-info/top_level.txt,sha256=r0lGZefzJjcHRFTtVrLE2EjICxN1ZkBKsFV_fgu3DuE,12
+genet-0.7.3.dist-info/RECORD,,
```

