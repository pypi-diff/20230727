# Comparing `tmp/genet-0.6.1-py3-none-any.whl.zip` & `tmp/genet-0.6.1a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 39135 bytes, number of entries: 39
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
--rw-rw-rw-  2.0 fat      180 b- defN 23-Jul-27 04:55 genet/utils/__init__.py
+-rw-rw-rw-  2.0 fat      181 b- defN 23-Jul-27 04:18 genet/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2150 b- defN 23-May-30 01:16 genet/utils/functional.py
 -rw-rw-rw-  2.0 fat       43 b- defN 22-Oct-28 02:23 tests/__init__.py
--rw-rw-rw-  2.0 fat    14162 b- defN 23-Jul-27 04:55 genet-0.6.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 04:55 genet-0.6.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       73 b- defN 23-Jul-27 04:55 genet-0.6.1.dist-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-27 04:55 genet-0.6.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     3808 b- defN 23-Jul-27 04:55 genet-0.6.1.dist-info/RECORD
-39 files, 130783 bytes uncompressed, 32729 bytes compressed:  75.0%
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
 
-Filename: genet-0.6.1.dist-info/METADATA
+Filename: genet-0.6.1a0.dist-info/METADATA
 Comment: 
 
-Filename: genet-0.6.1.dist-info/WHEEL
+Filename: genet-0.6.1a0.dist-info/WHEEL
 Comment: 
 
-Filename: genet-0.6.1.dist-info/dependency_links.txt
+Filename: genet-0.6.1a0.dist-info/dependency_links.txt
 Comment: 
 
-Filename: genet-0.6.1.dist-info/top_level.txt
+Filename: genet-0.6.1a0.dist-info/top_level.txt
 Comment: 
 
-Filename: genet-0.6.1.dist-info/RECORD
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
 
-version_ = '0.6.1'
+version_ = '0.6.1a'
 
 __version__ = version_
```

## Comparing `genet-0.6.1.dist-info/METADATA` & `genet-0.6.1a0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genet
-Version: 0.6.1
+Version: 0.6.1a0
 Summary: GenET: Genome Editing Toolkit
 Home-page: https://github.com/Goosang-Yu/genet
 Author: Goosang Yu
 Author-email: gsyu93@gmail.com
 Project-URL: Bug Tracker, https://github.com/Goosang-Yu/genet/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
+Classifier: Typing :: Typed
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `genet-0.6.1.dist-info/RECORD` & `genet-0.6.1a0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_DLD1_PE4max/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HCT116_PE2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_HeLa_PE2max/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_MDA_PE2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_FT/DPFT_NIH_NRCH_PE4max/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepPrime/DeepPrime_base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 genet/predict/models/DeepSpCas9/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-genet/utils/__init__.py,sha256=CYj_K--gASU99mI8VI9-SQJqRfLKpAhisllbeK8mJEw,180
+genet/utils/__init__.py,sha256=mPChwkBmd04LSFJUEeeG3ZKMClu6Djb8tAcpoafjB_Y,181
 genet/utils/functional.py,sha256=25qi_DaqhQk8E4WINfjdbachK9t5o3TMQ1RR85kfvK0,2150
 tests/__init__.py,sha256=BFhp5tyle0b2qhFpJ7tnbbjdPbPsWyi5aGVTUuNma7Y,43
-genet-0.6.1.dist-info/METADATA,sha256=pNPkNTqtq0WHGQgAbAfNvNas1__3JJVx2oRJk8L8XkY,14162
-genet-0.6.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-genet-0.6.1.dist-info/dependency_links.txt,sha256=P5B4DDpk_oHFlP5kqtdeFyTQaZZZWTCtoYf7zqzMYIA,73
-genet-0.6.1.dist-info/top_level.txt,sha256=r0lGZefzJjcHRFTtVrLE2EjICxN1ZkBKsFV_fgu3DuE,12
-genet-0.6.1.dist-info/RECORD,,
+genet-0.6.1a0.dist-info/METADATA,sha256=0FEYQXsY2CYRZxj1czEY_BIoRL_6KgBP-A9imgVilO0,14192
+genet-0.6.1a0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+genet-0.6.1a0.dist-info/dependency_links.txt,sha256=P5B4DDpk_oHFlP5kqtdeFyTQaZZZWTCtoYf7zqzMYIA,73
+genet-0.6.1a0.dist-info/top_level.txt,sha256=r0lGZefzJjcHRFTtVrLE2EjICxN1ZkBKsFV_fgu3DuE,12
+genet-0.6.1a0.dist-info/RECORD,,
```

