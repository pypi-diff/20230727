# Comparing `tmp/genet-0.6.0-py3-none-any.whl.zip` & `tmp/genet-0.6.1a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 38971 bytes, number of entries: 39
+Zip file size: 39170 bytes, number of entries: 39
 -rw-rw-rw-  2.0 fat      109 b- defN 22-Oct-28 02:23 genet/__init__.py
 -rw-rw-rw-  2.0 fat      113 b- defN 22-Dec-29 12:57 genet/main.py
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Dec-21 12:42 genet/analysis/__init__.py
 -rw-rw-rw-  2.0 fat    10745 b- defN 22-Dec-24 07:17 genet/analysis/functional.py
 -rw-rw-rw-  2.0 fat      229 b- defN 22-Nov-23 01:16 genet/database/__init__.py
 -rw-rw-rw-  2.0 fat     8457 b- defN 23-Feb-01 08:54 genet/database/functional.py
 -rw-rw-rw-  2.0 fat     3275 b- defN 23-May-23 03:59 genet/design/DesignUtils.py
@@ -26,16 +26,16 @@
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_DLD1_PE4max/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HCT116_PE2/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HeLa_PE2max/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_MDA_PE2/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-31 01:05 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_NIH_NRCH_PE4max/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-28 06:11 genet/predict/models/DeepPrime/DeepPrime_base/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-28 05:54 genet/predict/models/DeepSpCas9/__init__.py
--rw-rw-rw-  2.0 fat      180 b- defN 23-Jun-14 10:36 genet/utils/__init__.py
+-rw-rw-rw-  2.0 fat      181 b- defN 23-Jul-27 04:18 genet/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2150 b- defN 23-May-30 01:16 genet/utils/functional.py
 -rw-rw-rw-  2.0 fat       43 b- defN 22-Oct-28 02:23 tests/__init__.py
--rw-rw-rw-  2.0 fat    13110 b- defN 23-Jun-14 10:48 genet-0.6.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-14 10:48 genet-0.6.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      112 b- defN 23-Jun-14 10:48 genet-0.6.0.dist-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-14 10:48 genet-0.6.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     3809 b- defN 23-Jun-14 10:48 genet-0.6.0.dist-info/RECORD
-39 files, 129771 bytes uncompressed, 32565 bytes compressed:  74.9%
+-rw-rw-rw-  2.0 fat    14192 b- defN 23-Jul-27 04:33 genet-0.6.1a0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 04:33 genet-0.6.1a0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       73 b- defN 23-Jul-27 04:32 genet-0.6.1a0.dist-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-27 04:32 genet-0.6.1a0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     3818 b- defN 23-Jul-27 04:33 genet-0.6.1a0.dist-info/RECORD
+39 files, 130824 bytes uncompressed, 32744 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -96,23 +96,23 @@
 
 Filename: genet/utils/functional.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
-Filename: genet-0.6.0.dist-info/METADATA
+Filename: genet-0.6.1a0.dist-info/METADATA
 Comment: 
 
-Filename: genet-0.6.0.dist-info/WHEEL
+Filename: genet-0.6.1a0.dist-info/WHEEL
 Comment: 
 
-Filename: genet-0.6.0.dist-info/dependency_links.txt
+Filename: genet-0.6.1a0.dist-info/dependency_links.txt
 Comment: 
 
-Filename: genet-0.6.0.dist-info/top_level.txt
+Filename: genet-0.6.1a0.dist-info/top_level.txt
 Comment: 
 
-Filename: genet-0.6.0.dist-info/RECORD
+Filename: genet-0.6.1a0.dist-info/RECORD
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
 
-version_ = '0.6.0'
+version_ = '0.6.1a'
 
 __version__ = version_
```

## Comparing `genet-0.6.0.dist-info/METADATA` & `genet-0.6.1a0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 Metadata-Version: 2.1
 Name: genet
-Version: 0.6.0
+Version: 0.6.1a0
 Summary: GenET: Genome Editing Toolkit
 Home-page: https://github.com/Goosang-Yu/genet
 Author: Goosang Yu
 Author-email: gsyu93@gmail.com
 Project-URL: Bug Tracker, https://github.com/Goosang-Yu/genet/issues
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: Unix
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development
+Classifier: Typing :: Typed
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: regex
 Requires-Dist: biopython
 Requires-Dist: tensorflow (==2.8.0)
-Requires-Dist: torch (==1.11.0+cu113)
-Requires-Dist: torchvision (==0.12.0+cu113)
-Requires-Dist: torchaudio (==0.11.0)
 Requires-Dist: protobuf (==3.20.*)
 Requires-Dist: silence-tensorflow
 Requires-Dist: genet-models
 Requires-Dist: pyarrow
 Requires-Dist: fastparquet
 
 <div align="center">
@@ -45,34 +55,51 @@
 ## Welcome to GenET
 GenET (Genome Editing Toolkit) is a library of various python functions for the purpose of analyzing and evaluating data from genome editing experiments. GenET is still in its early stages of development and continue to improve and expand. Currently planned functions include guideRNA design, saturation library design, deep sequenced data analysis, and guide RNA activity prediction.
 
 ## System requirement
 GenET can be run on either Mac or Linux system. GenET is currently available on Linux or Mac based systems as one of the dependent tools, ViennaRNA package, is limited to these operating systems. Windows users must establish a docker or virtual OS environment to use this tool.
 
 ## Installation
-
+1/ Create virtual environment and install genet
 ```python
-# Create virtual env for genet.
-# python 3.8 was tested. 
+# Create virtual env for genet. (python 3.8 was tested)
 conda create -n genet python=3.8
 conda activate genet
 
 # install genet package in your env.
-pip install genet -f https://download.pytorch.org/whl/cu113/torch_stable.html git+https://github.com/Goosang-Yu/genet-models.git
+pip install genet -f git+https://github.com/Goosang-Yu/genet-models.git
+```
+
+2/ Install Pytorch (v1.11.0 was tested)
+```python
+# For OSX (MacOS)
+conda install pytorch==1.11.0 torchvision==0.12.0 torchaudio==0.11.0 -c pytorch
+
+# For Linux and Windows
+# CUDA 10.2
+conda install pytorch==1.11.0 torchvision==0.12.0 torchaudio==0.11.0 cudatoolkit=10.2 -c pytorch
 
+# CUDA 11.3
+conda install pytorch==1.11.0 torchvision==0.12.0 torchaudio==0.11.0 cudatoolkit=11.3 -c pytorch
+
+# CPU Only
+conda install pytorch==1.11.0 torchvision==0.12.0 torchaudio==0.11.0 cpuonly -c pytorch
+```
+3/ Install ViennaRNA
+```python
 # install ViennaRNA package for prediction module
 conda install viennarna
 ```
 
 ### Trouble shooting for installation
 #### 1/ GLIBCXX ImportError  
 ```
 ImportError: /lib64/libstdc++.so.6: version `GLIBCXX_3.4.20' not found (required by /home/hkim/.miniconda3/envs/genet/lib/python3.8/site-packages/RNA/_RNA.cpython-38-x86_64-linux-gnu.so)'
 ```  
-If the above error message appears in the process of loading the Vienna RNA, install  'libgcc' using mamba ([see alse](https://pypi.org/project/ViennaRNA/)).  
+If the above error message appears in the process of loading the Vienna RNA, install  higher version of 'libgcc' using mamba ([see alse](https://pypi.org/project/ViennaRNA/)).  
 ```
 conda activate genet
 conda install -c conda-forge mamba
 mamba install libgcc
 ```
 
 ## Who should use GenET?
```

## Comparing `genet-0.6.0.dist-info/RECORD` & `genet-0.6.1a0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_DLD1_PE4max/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HCT116_PE2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HeLa_PE2max/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_MDA_PE2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_NIH_NRCH_PE4max/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepSpCas9/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-genet/utils/__init__.py,sha256=IEYEUMtkO0Sx_mRLhms-m808fV_GDPlyOAG7GS8NFPE,180
+genet/utils/__init__.py,sha256=mPChwkBmd04LSFJUEeeG3ZKMClu6Djb8tAcpoafjB_Y,181
 genet/utils/functional.py,sha256=25qi_DaqhQk8E4WINfjdbachK9t5o3TMQ1RR85kfvK0,2150
 tests/__init__.py,sha256=BFhp5tyle0b2qhFpJ7tnbbjdPbPsWyi5aGVTUuNma7Y,43
-genet-0.6.0.dist-info/METADATA,sha256=lOvc0QLwlbqaGdCLE9EMFOVZEYvcr1tOFUrV1BM-6BM,13110
-genet-0.6.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-genet-0.6.0.dist-info/dependency_links.txt,sha256=S21jsUEQIXb1RnunxuUoFF2Lr-1VsDzkKFViK-_-7kQ,112
-genet-0.6.0.dist-info/top_level.txt,sha256=r0lGZefzJjcHRFTtVrLE2EjICxN1ZkBKsFV_fgu3DuE,12
-genet-0.6.0.dist-info/RECORD,,
+genet-0.6.1a0.dist-info/METADATA,sha256=0FEYQXsY2CYRZxj1czEY_BIoRL_6KgBP-A9imgVilO0,14192
+genet-0.6.1a0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+genet-0.6.1a0.dist-info/dependency_links.txt,sha256=P5B4DDpk_oHFlP5kqtdeFyTQaZZZWTCtoYf7zqzMYIA,73
+genet-0.6.1a0.dist-info/top_level.txt,sha256=r0lGZefzJjcHRFTtVrLE2EjICxN1ZkBKsFV_fgu3DuE,12
+genet-0.6.1a0.dist-info/RECORD,,
```

