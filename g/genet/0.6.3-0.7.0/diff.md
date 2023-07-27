# Comparing `tmp/genet-0.6.3-py3-none-any.whl.zip` & `tmp/genet-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 41651 bytes, number of entries: 41
+Zip file size: 41604 bytes, number of entries: 41
 -rw-rw-rw-  2.0 fat      109 b- defN 22-Oct-28 02:23 genet/__init__.py
 -rw-rw-rw-  2.0 fat      113 b- defN 22-Dec-29 12:57 genet/main.py
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Dec-21 12:42 genet/analysis/__init__.py
 -rw-rw-rw-  2.0 fat    10745 b- defN 22-Dec-24 07:17 genet/analysis/functional.py
 -rw-rw-rw-  2.0 fat      229 b- defN 22-Nov-23 01:16 genet/database/__init__.py
 -rw-rw-rw-  2.0 fat     8457 b- defN 23-Feb-01 08:54 genet/database/functional.py
 -rw-rw-rw-  2.0 fat     3275 b- defN 23-May-23 03:59 genet/design/DesignUtils.py
@@ -29,15 +29,15 @@
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_DLD1_PE4max/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HCT116_PE2/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HeLa_PE2max/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_MDA_PE2/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_NIH_NRCH_PE4max/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-28 06:11 genet/predict/models/DeepPrime/DeepPrime_base/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-28 05:54 genet/predict/models/DeepSpCas9/__init__.py
--rw-rw-rw-  2.0 fat      180 b- defN 23-Jul-27 14:01 genet/utils/__init__.py
+-rw-rw-rw-  2.0 fat      180 b- defN 23-Jul-27 15:16 genet/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2150 b- defN 23-Jul-27 14:00 genet/utils/functional.py
 -rw-rw-rw-  2.0 fat       43 b- defN 22-Oct-28 02:23 tests/__init__.py
--rw-rw-rw-  2.0 fat    14307 b- defN 23-Jul-27 14:10 genet-0.6.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 14:10 genet-0.6.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-27 14:10 genet-0.6.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     3955 b- defN 23-Jul-27 14:10 genet-0.6.3.dist-info/RECORD
-41 files, 141101 bytes uncompressed, 35027 bytes compressed:  75.2%
+-rw-rw-rw-  2.0 fat    14095 b- defN 23-Jul-27 15:17 genet-0.7.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 15:17 genet-0.7.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-27 15:17 genet-0.7.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     3955 b- defN 23-Jul-27 15:17 genet-0.7.0.dist-info/RECORD
+41 files, 140889 bytes uncompressed, 34980 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -105,20 +105,20 @@
 
 Filename: genet/utils/functional.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
-Filename: genet-0.6.3.dist-info/METADATA
+Filename: genet-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: genet-0.6.3.dist-info/WHEEL
+Filename: genet-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: genet-0.6.3.dist-info/top_level.txt
+Filename: genet-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: genet-0.6.3.dist-info/RECORD
+Filename: genet-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genet/utils/__init__.py

```diff
@@ -1,10 +1,10 @@
 from .functional import *
 
 # for PyPI release
 # python setup.py bdist_wheel
 # twine upload dist/genet-0.5.2-py3-none-any.whl
 
-version_ = '0.6.3'
+version_ = '0.7.0'
 
 __version__ = version_
```

## Comparing `genet-0.6.3.dist-info/METADATA` & `genet-0.7.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genet
-Version: 0.6.3
+Version: 0.7.0
 Summary: GenET: Genome Editing Toolkit
 Home-page: https://github.com/Goosang-Yu/genet
 Author: Goosang Yu
 Author-email: gsyu93@gmail.com
 Project-URL: Bug Tracker, https://github.com/Goosang-Yu/genet/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -30,63 +30,63 @@
 Requires-Dist: regex
 Requires-Dist: biopython
 Requires-Dist: tensorflow (==2.8.0)
 Requires-Dist: protobuf (==3.20.*)
 Requires-Dist: silence-tensorflow
 Requires-Dist: pyarrow
 Requires-Dist: fastparquet
+Requires-Dist: tqdm
 
 <div align="center">
   
   <img src="https://github.com/Goosang-Yu/genet/blob/main/docs/images/logo.png?raw=true" width="300"/>
 
 **Genome Editing Toolkit** </br>
 **Since 2022. 08. 19.** </br>
 
-[![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9-blue)](https://badge.fury.io/py/genet) 
+[![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://badge.fury.io/py/genet) 
 [![PyPI version](https://badge.fury.io/py/genet.svg)](https://badge.fury.io/py/genet) 
 [![Slack](https://img.shields.io/badge/slack-chat-blueviolet.svg?logo=slack)](https://genethq.slack.com/archives/C04DP727E4E)
 [![License](https://img.shields.io/pypi/l/ansicolortags.svg)](https://img.shields.io/pypi/l/ansicolortags.svg) 
 
 
 <div align="left">
 
 ## Welcome to GenET
 GenET (Genome Editing Toolkit) is a library of various python functions for the purpose of analyzing and evaluating data from genome editing experiments. GenET is still in its early stages of development and continue to improve and expand. Currently planned functions include guideRNA design, saturation library design, deep sequenced data analysis, and guide RNA activity prediction.
 
 ## System requirement
-GenET can be run on either Mac or Linux system. GenET is currently available on Linux or Mac based systems as one of the dependent tools, ViennaRNA package, is limited to these operating systems. Windows users must establish a docker or virtual OS environment to use this tool.
+GenET can be run on either Mac or Linux system. GenET is currently available on Linux or Mac based systems as one of the dependent tools, ViennaRNA package, is limited to these operating systems. Windows users must establish a WSL, docker or virtual OS environment to use this tool.
 
 ## Installation
 #### 1/ Create virtual environment and install genet
 ```python
 # Create virtual env for genet. (python 3.8 was tested)
 conda create -n genet python=3.8
 conda activate genet
 
-# install genet and models package in your env.
+# Install genet ( >= ver. 0.7.0)
 pip install genet
-pip install git+https://github.com/Goosang-Yu/genet-models.git
 ```
 
 #### 2/ Install Pytorch (v1.11.0 was tested)  
 Pytorch ver.2 is not compatible yet.
 ```python
 # For OSX (MacOS)
-pip install torch==1.11.0 torchvision==0.12.0 torchaudio==0.11.0
+pip install torch==1.11.0
 
 # For Linux and Windows
 # CUDA 11.3
-pip install torch==1.11.0+cu113 torchvision==0.12.0+cu113 torchaudio==0.11.0 --extra-index-url https://download.pytorch.org/whl/cu113
+pip install torch==1.11.0+cu113 --extra-index-url https://download.pytorch.org/whl/cu113
 
 # CUDA 10.2
-pip install torch==1.11.0+cu102 torchvision==0.12.0+cu102 torchaudio==0.11.0 --extra-index-url https://download.pytorch.org/whl/cu102
+pip install torch==1.11.0+cu102 --extra-index-url https://download.pytorch.org/whl/cu102
 
 # CPU only
-pip install torch==1.11.0+cpu torchvision==0.12.0+cpu torchaudio==0.11.0 --extra-index-url https://download.pytorch.org/whl/cpu
+pip install torch==1.11.0+cpu --extra-index-url https://download.pytorch.org/whl/cpu
 ```
 #### 3/ Install ViennaRNA
 ```python
 # install ViennaRNA package for prediction module
 conda install viennarna
 ```
```

## Comparing `genet-0.6.3.dist-info/RECORD` & `genet-0.7.0.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,14 @@
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_DLD1_PE4max/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HCT116_PE2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HeLa_PE2max/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_MDA_PE2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_NIH_NRCH_PE4max/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepSpCas9/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-genet/utils/__init__.py,sha256=Qj757DsW1BK6DVKDj_55mGMfForEQWl1lKH-Fd62BP8,180
+genet/utils/__init__.py,sha256=aOZ8NJz-3-OenCKv-wQR9Z1le6YnqKPRMC14pAqCOTs,180
 genet/utils/functional.py,sha256=25qi_DaqhQk8E4WINfjdbachK9t5o3TMQ1RR85kfvK0,2150
 tests/__init__.py,sha256=BFhp5tyle0b2qhFpJ7tnbbjdPbPsWyi5aGVTUuNma7Y,43
-genet-0.6.3.dist-info/METADATA,sha256=2-dpNSiDyvDiQxBx9mciBzjflGrjKAkQi3U0bbYH6Wo,14307
-genet-0.6.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-genet-0.6.3.dist-info/top_level.txt,sha256=r0lGZefzJjcHRFTtVrLE2EjICxN1ZkBKsFV_fgu3DuE,12
-genet-0.6.3.dist-info/RECORD,,
+genet-0.7.0.dist-info/METADATA,sha256=LNX_i_YhIxrI3b0aJirwX40VgrdwtSo5aljnGNhv32s,14095
+genet-0.7.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+genet-0.7.0.dist-info/top_level.txt,sha256=r0lGZefzJjcHRFTtVrLE2EjICxN1ZkBKsFV_fgu3DuE,12
+genet-0.7.0.dist-info/RECORD,,
```

