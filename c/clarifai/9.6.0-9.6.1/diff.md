# Comparing `tmp/clarifai-9.6.0.tar.gz` & `tmp/clarifai-9.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-9.6.0.tar", last modified: Mon Jul 17 14:39:44 2023, max compression
+gzip compressed data, was "clarifai-9.6.1.tar", last modified: Thu Jul 27 18:52:25 2023, max compression
```

## Comparing `clarifai-9.6.0.tar` & `clarifai-9.6.1.tar`

### file list

```diff
@@ -1,500 +1,248 @@
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.257110 clarifai-9.6.0/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      555 2023-06-01 21:00:24.000000 clarifai-9.6.0/LICENSE
--rw-r--r--   0 yvettezhang   (501) staff       (20)      119 2023-07-17 14:39:38.000000 clarifai-9.6.0/MANIFEST.in
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-07-17 14:39:44.256940 clarifai-9.6.0/PKG-INFO
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2347 2023-06-01 21:00:24.000000 clarifai-9.6.0/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.186212 clarifai-9.6.0/clarifai/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.187125 clarifai-9.6.0/clarifai/auth/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/auth/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    12447 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/auth/helper.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.188476 clarifai-9.6.0/clarifai/client/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/client/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/client/abc.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/client/stub.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.190028 clarifai-9.6.0/clarifai/data_upload/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3487 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/README.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     7331 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/convert_csv.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.191163 clarifai-9.6.0/clarifai/data_upload/datasets/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/datasets/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2546 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/base.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1289 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/datasets/features.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    10249 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/image.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2074 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/text.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.192201 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3961 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/README.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3684 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4894 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6291 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1605 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6451 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.192340 clarifai-9.6.0/clarifai/data_upload/examples/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      450 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.192494 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.193192 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      299 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/cifar_small_test.csv
--rw-r--r--   0 yvettezhang   (501) staff       (20)      299 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/cifar_small_train.csv
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1091 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.194934 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      963 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_700.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      921 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_701.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      907 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_702.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      828 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_703.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      922 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_704.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      877 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_705.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      859 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_706.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      937 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_707.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      875 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_708.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      826 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_709.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.195242 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1195 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.177597 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.198455 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/
--rw-r--r--   0 yvettezhang   (501) staff       (20)    59900 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/1036242.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    54450 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/1114182.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    49005 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/1420783.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    63984 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/2012944.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    62530 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/2464389.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    49264 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/3287885.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    43410 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/3617075.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    33826 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/38052.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    47755 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/39147.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    54968 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/478632.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.202048 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/
--rw-r--r--   0 yvettezhang   (501) staff       (20)    96729 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/1061270.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    55702 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/1202261.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    48391 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/1381751.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    43856 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/139558.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    47022 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/1636096.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    46176 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/2480925.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    63224 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/3289634.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    37327 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/3385808.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    32557 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/3647386.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    54823 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/862025.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.205201 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/
--rw-r--r--   0 yvettezhang   (501) staff       (20)    53968 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/102197.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    26278 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/1826869.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    45386 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/2243245.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    40566 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/259212.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    67808 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/2749372.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    47620 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/2842688.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    53419 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/2938268.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    52635 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/3035414.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    55723 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/3590861.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    56940 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/746716.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.209134 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/
--rw-r--r--   0 yvettezhang   (501) staff       (20)    44858 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/1545393.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    49950 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/2427642.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    58221 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/2955110.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    64028 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/3208966.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    62079 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/3270629.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    58751 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/3424562.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    51306 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/3520891.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    34567 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/377566.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    56869 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/503504.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    64261 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/544680.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.209348 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.209548 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.211244 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      760 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2007_000464.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)      572 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2008_000853.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1075 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2008_003182.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1319 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2008_008526.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)      570 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2009_004315.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)      570 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2009_004382.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)      568 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2011_000430.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)      874 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2011_001610.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2088 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2011_006412.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)      914 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2012_000690.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2692 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/dataset.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.214274 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99806 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2007_000464.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99739 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2008_000853.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99737 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2008_003182.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99774 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2008_008526.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99802 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2009_004315.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99794 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2009_004382.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99823 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2011_000430.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99784 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2011_001610.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99748 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2011_006412.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99747 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2012_000690.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.214776 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.214994 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.215551 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/annotations/
--rw-r--r--   0 yvettezhang   (501) staff       (20)   139780 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/annotations/instances_val2017_subset.json
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4235 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/dataset.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.219013 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101406 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000074646.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101836 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000086956.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101772 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000166563.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101669 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000176857.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101496 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000182202.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101592 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000193245.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101791 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000384850.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101556 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000409630.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101426 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000424349.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101539 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000573008.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.220587 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.221922 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1049 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)   237144 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/imdb_dataset/test.csv
--rw-r--r--   0 yvettezhang   (501) staff       (20)   270347 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/imdb_dataset/train.csv
--rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    13507 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/upload.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.222645 clarifai-9.6.0/clarifai/dataset_export/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     7475 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.223832 clarifai-9.6.0/clarifai/listing/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/concepts.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/datasets.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/inputs.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/installed_module_versions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     7764 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/lister.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/models.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/module_versions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/modules.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.224039 clarifai-9.6.0/clarifai/models/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     9555 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai/models/api.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.224652 clarifai-9.6.0/clarifai/models/model_serving/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6903 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai/models/model_serving/README.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.225139 clarifai-9.6.0/clarifai/models/model_serving/cli/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/cli/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3825 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai/models/model_serving/cli/deploy_cli.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1866 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/cli/model_zip.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1947 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/cli/repository.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      112 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/constants.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.225503 clarifai-9.6.0/clarifai/models/model_serving/docs/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1027 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/docs/dependencies.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)      943 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/docs/model_types.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1507 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/docs/output.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.225627 clarifai-9.6.0/clarifai/models/model_serving/envs/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1030 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/envs/triton_conda.yaml
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.225753 clarifai-9.6.0/clarifai/models/model_serving/examples/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      623 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.225876 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      469 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.226522 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.226909 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2251 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.227306 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      177 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/README.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)      850 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/config.json
--rw-r--r--   0 yvettezhang   (501) staff       (20)      198 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/preprocessor_config.json
--rw-r--r--   0 yvettezhang   (501) staff       (20)      344 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/config.pbtxt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       57 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/labels.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)      134 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/requirements.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       46 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/triton_conda.yaml
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.227445 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      556 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.227987 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.228328 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2173 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.228725 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      588 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/README.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)      841 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/config.json
--rw-r--r--   0 yvettezhang   (501) staff       (20)      151 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/special_tokens_map.json
--rw-r--r--   0 yvettezhang   (501) staff       (20)      326 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/config.pbtxt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       26 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/labels.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)      134 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/requirements.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       46 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/triton_conda.yaml
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.228853 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      521 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.229354 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.229603 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2906 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      520 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/config.pbtxt
--rw-r--r--   0 yvettezhang   (501) staff       (20)      621 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/labels.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)      281 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/requirements.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       46 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/triton_conda.yaml
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.230087 clarifai-9.6.0/clarifai/models/model_serving/model_config/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/model_config/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1731 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai/models/model_serving/model_config/deploy.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4231 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/model_config/serializer.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4489 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/model_config/triton_config.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.230684 clarifai-9.6.0/clarifai/models/model_serving/models/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/models/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1639 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/models/inference.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3701 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/models/model_types.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2334 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/models/output.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/models/pb_model.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3411 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/pb_model_repository.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.231247 clarifai-9.6.0/clarifai/modules/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      367 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/modules/README.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/modules/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/modules/css.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/modules/pages.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6003 2023-06-02 20:18:09.000000 clarifai-9.6.0/clarifai/modules/style.css
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.231466 clarifai-9.6.0/clarifai/urls/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4276 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/urls/helper.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.186922 clarifai-9.6.0/clarifai.egg-info/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-07-17 14:39:44.000000 clarifai-9.6.0/clarifai.egg-info/PKG-INFO
--rw-r--r--   0 yvettezhang   (501) staff       (20)    27508 2023-07-17 14:39:44.000000 clarifai-9.6.0/clarifai.egg-info/SOURCES.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)        1 2023-07-17 14:39:44.000000 clarifai-9.6.0/clarifai.egg-info/dependency_links.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)      255 2023-07-17 14:39:44.000000 clarifai-9.6.0/clarifai.egg-info/entry_points.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       52 2023-07-17 14:39:44.000000 clarifai-9.6.0/clarifai.egg-info/requires.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       24 2023-07-17 14:39:44.000000 clarifai-9.6.0/clarifai.egg-info/top_level.txt
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.231589 clarifai-9.6.0/clarifai_utils/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.231763 clarifai-9.6.0/clarifai_utils/auth/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/auth/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    12447 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/auth/helper.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.232096 clarifai-9.6.0/clarifai_utils/client/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/client/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/client/abc.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/client/stub.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.232614 clarifai-9.6.0/clarifai_utils/data_upload/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3487 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/README.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     7331 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/convert_csv.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.233134 clarifai-9.6.0/clarifai_utils/data_upload/datasets/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2546 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/base.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1289 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/features.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    10249 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/image.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2074 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/text.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.233887 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3961 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/README.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3684 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4894 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6291 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1605 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6451 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.233998 clarifai-9.6.0/clarifai_utils/data_upload/examples/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      450 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.234114 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.234526 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      299 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/cifar_small_test.csv
--rw-r--r--   0 yvettezhang   (501) staff       (20)      299 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/cifar_small_train.csv
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1091 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.235648 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      963 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_700.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      921 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_701.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      907 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_702.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      828 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_703.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      922 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_704.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      877 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_705.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      859 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_706.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      937 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_707.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      875 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_708.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)      826 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_709.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.235849 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1195 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.181226 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.237226 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/
--rw-r--r--   0 yvettezhang   (501) staff       (20)    59900 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/1036242.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    54450 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/1114182.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    49005 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/1420783.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    63984 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/2012944.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    62530 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/2464389.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    49264 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/3287885.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    43410 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/3617075.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    33826 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/38052.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    47755 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/39147.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    54968 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/478632.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.238749 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/
--rw-r--r--   0 yvettezhang   (501) staff       (20)    96729 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/1061270.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    55702 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/1202261.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    48391 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/1381751.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    43856 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/139558.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    47022 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/1636096.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    46176 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/2480925.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    63224 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/3289634.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    37327 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/3385808.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    32557 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/3647386.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    54823 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/862025.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.240185 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/
--rw-r--r--   0 yvettezhang   (501) staff       (20)    53968 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/102197.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    26278 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/1826869.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    45386 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/2243245.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    40566 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/259212.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    67808 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/2749372.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    47620 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/2842688.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    53419 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/2938268.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    52635 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/3035414.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    55723 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/3590861.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    56940 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/746716.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.241596 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/
--rw-r--r--   0 yvettezhang   (501) staff       (20)    44858 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/1545393.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    49950 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/2427642.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    58221 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/2955110.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    64028 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/3208966.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    62079 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/3270629.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    58751 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/3424562.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    51306 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/3520891.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    34567 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/377566.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    56869 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/503504.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)    64261 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/544680.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.241739 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.241943 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.243046 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      760 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2007_000464.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)      572 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2008_000853.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1075 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2008_003182.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1319 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2008_008526.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)      570 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2009_004315.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)      570 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2009_004382.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)      568 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2011_000430.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)      874 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2011_001610.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2088 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2011_006412.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)      914 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2012_000690.xml
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2692 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/dataset.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.244595 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99806 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2007_000464.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99739 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2008_000853.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99737 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2008_003182.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99774 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2008_008526.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99802 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2009_004315.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99794 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2009_004382.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99823 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2011_000430.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99784 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2011_001610.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99748 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2011_006412.jpg
--rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99747 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2012_000690.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.244770 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.244982 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.245103 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/annotations/
--rw-r--r--   0 yvettezhang   (501) staff       (20)   139780 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/annotations/instances_val2017_subset.json
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4235 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/dataset.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.246754 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101406 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000074646.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101836 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000086956.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101772 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000166563.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101669 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000176857.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101496 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000182202.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101592 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000193245.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101791 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000384850.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101556 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000409630.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101426 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000424349.jpg
--rw-r--r--   0 yvettezhang   (501) staff       (20)   101539 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000573008.jpg
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.246907 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.247411 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1049 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)   237144 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/test.csv
--rw-r--r--   0 yvettezhang   (501) staff       (20)   270347 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/train.csv
--rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)    13507 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/upload.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.247635 clarifai-9.6.0/clarifai_utils/dataset_export/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     7475 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.248561 clarifai-9.6.0/clarifai_utils/listing/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/concepts.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/datasets.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/inputs.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/installed_module_versions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     7764 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/lister.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/models.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/module_versions.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/modules.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.248768 clarifai-9.6.0/clarifai_utils/models/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     9555 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai_utils/models/api.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.249215 clarifai-9.6.0/clarifai_utils/models/model_serving/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6903 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/README.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/__init__.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.249653 clarifai-9.6.0/clarifai_utils/models/model_serving/cli/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/cli/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3825 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/cli/deploy_cli.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1866 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/cli/model_zip.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1947 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/cli/repository.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      112 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/constants.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.249991 clarifai-9.6.0/clarifai_utils/models/model_serving/docs/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1027 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/docs/dependencies.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)      943 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/docs/model_types.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1507 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/docs/output.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.250107 clarifai-9.6.0/clarifai_utils/models/model_serving/envs/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1030 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/envs/triton_conda.yaml
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.250223 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      623 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.250344 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      469 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.250806 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.251133 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2251 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.251513 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      177 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/README.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)      850 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/config.json
--rw-r--r--   0 yvettezhang   (501) staff       (20)      198 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/preprocessor_config.json
--rw-r--r--   0 yvettezhang   (501) staff       (20)      344 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/config.pbtxt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       57 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/labels.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)      134 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/requirements.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       46 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/triton_conda.yaml
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.251663 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      556 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.252473 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.252850 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2173 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.253290 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      588 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/README.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)      841 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/config.json
--rw-r--r--   0 yvettezhang   (501) staff       (20)      151 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/special_tokens_map.json
--rw-r--r--   0 yvettezhang   (501) staff       (20)      326 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/config.pbtxt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       26 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/labels.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)      134 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/requirements.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       46 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/triton_conda.yaml
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.253416 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      521 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/README.md
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.254016 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.254296 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2906 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)      520 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/config.pbtxt
--rw-r--r--   0 yvettezhang   (501) staff       (20)      621 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/labels.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)      281 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/requirements.txt
--rw-r--r--   0 yvettezhang   (501) staff       (20)       46 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/triton_conda.yaml
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.254861 clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1731 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/deploy.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4231 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/serializer.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4489 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/triton_config.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.255545 clarifai-9.6.0/clarifai_utils/models/model_serving/models/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/models/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1639 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/models/inference.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3701 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/models/model_types.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2334 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/models/output.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/models/pb_model.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3411 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/pb_model_repository.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.256116 clarifai-9.6.0/clarifai_utils/modules/
--rw-r--r--   0 yvettezhang   (501) staff       (20)      367 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/modules/README.md
--rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/modules/__init__.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/modules/css.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/modules/pages.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     6003 2023-06-02 20:18:09.000000 clarifai-9.6.0/clarifai_utils/modules/style.css
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.256232 clarifai-9.6.0/clarifai_utils/urls/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4276 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/urls/helper.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)       38 2023-07-17 14:39:44.257149 clarifai-9.6.0/setup.cfg
--rw-r--r--   0 yvettezhang   (501) staff       (20)     1297 2023-07-17 14:37:15.000000 clarifai-9.6.0/setup.py
-drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.256631 clarifai-9.6.0/tests/
--rw-r--r--   0 yvettezhang   (501) staff       (20)     2300 2023-07-13 14:56:23.000000 clarifai-9.6.0/tests/test_auth.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     4771 2023-07-13 14:56:23.000000 clarifai-9.6.0/tests/test_modules.py
--rw-r--r--   0 yvettezhang   (501) staff       (20)     3716 2023-06-01 21:00:24.000000 clarifai-9.6.0/tests/test_stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.902327 clarifai-9.6.1/
+-rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.6.1/LICENSE
+-rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.6.1/MANIFEST.in
+-rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-07-27 18:52:25.902111 clarifai-9.6.1/PKG-INFO
+-rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.6.1/README.md
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.761422 clarifai-9.6.1/clarifai/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.815892 clarifai-9.6.1/clarifai/auth/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/auth/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    13909 2023-07-27 18:51:46.000000 clarifai-9.6.1/clarifai/auth/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.818157 clarifai-9.6.1/clarifai/client/
+-rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/client/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/client/abc.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-07-06 20:11:16.000000 clarifai-9.6.1/clarifai/client/stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.820807 clarifai-9.6.1/clarifai/data_upload/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/data_upload/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7331 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/data_upload/convert_csv.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.824169 clarifai-9.6.1/clarifai/data_upload/datasets/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/datasets/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2546 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/datasets/base.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1289 2023-06-02 04:02:11.000000 clarifai-9.6.1/clarifai/data_upload/datasets/features.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    10249 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/datasets/image.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2074 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/datasets/text.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.828184 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3684 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4894 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6291 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1605 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.6.1/clarifai/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.736668 clarifai-9.6.1/clarifai/data_upload/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.829128 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.830043 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.831323 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.832132 clarifai-9.6.1/clarifai/data_upload/examples/image_detection/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_detection/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.833173 clarifai-9.6.1/clarifai/data_upload/examples/image_detection/voc/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_detection/voc/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2692 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_detection/voc/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.833925 clarifai-9.6.1/clarifai/data_upload/examples/image_segmentation/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_segmentation/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.834755 clarifai-9.6.1/clarifai/data_upload/examples/image_segmentation/coco/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_segmentation/coco/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4235 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/examples/image_segmentation/coco/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.835716 clarifai-9.6.1/clarifai/data_upload/examples/text_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.836720 clarifai-9.6.1/clarifai/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai/data_upload/examples.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    13507 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/data_upload/upload.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.837362 clarifai-9.6.1/clarifai/dataset_export/
+-rw-r--r--   0 zeiler     (503) staff       (20)     7475 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.842655 clarifai-9.6.1/clarifai/listing/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/listing/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/listing/concepts.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/listing/datasets.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/listing/inputs.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.6.1/clarifai/listing/installed_module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.6.1/clarifai/listing/lister.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/listing/models.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.6.1/clarifai/listing/module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.6.1/clarifai/listing/modules.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.843798 clarifai-9.6.1/clarifai/models/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     9555 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/models/api.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.845563 clarifai-9.6.1/clarifai/models/model_serving/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.847906 clarifai-9.6.1/clarifai/models/model_serving/cli/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/cli/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3825 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/models/model_serving/cli/deploy_cli.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1866 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/cli/model_zip.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1947 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/cli/repository.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      112 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/constants.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.740612 clarifai-9.6.1/clarifai/models/model_serving/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.738995 clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.739268 clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.849671 clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2251 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.739963 clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.740213 clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.851678 clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2173 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.740805 clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.741052 clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/yolov5x/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.852825 clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2906 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.854957 clarifai-9.6.1/clarifai/models/model_serving/model_config/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/model_config/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1731 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai/models/model_serving/model_config/deploy.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4231 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/model_config/serializer.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4489 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/model_config/triton_config.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.857492 clarifai-9.6.1/clarifai/models/model_serving/models/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/models/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1639 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/models/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3701 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/models/model_types.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2334 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai/models/model_serving/models/output.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/models/pb_model.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3411 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai/models/model_serving/pb_model_repository.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.859676 clarifai-9.6.1/clarifai/modules/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/modules/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/modules/css.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai/modules/pages.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6003 2023-07-27 16:35:07.000000 clarifai-9.6.1/clarifai/modules/style.css
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.860740 clarifai-9.6.1/clarifai/runners/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-12 02:19:11.000000 clarifai-9.6.1/clarifai/runners/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3578 2023-07-12 15:26:44.000000 clarifai-9.6.1/clarifai/runners/api.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.861798 clarifai-9.6.1/clarifai/urls/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.6.1/clarifai/urls/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4276 2023-07-07 03:41:06.000000 clarifai-9.6.1/clarifai/urls/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.813597 clarifai-9.6.1/clarifai.egg-info/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-07-27 18:52:24.000000 clarifai-9.6.1/clarifai.egg-info/PKG-INFO
+-rw-r--r--   0 zeiler     (503) staff       (20)     8294 2023-07-27 18:52:25.000000 clarifai-9.6.1/clarifai.egg-info/SOURCES.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-07-27 18:52:24.000000 clarifai-9.6.1/clarifai.egg-info/dependency_links.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)      255 2023-07-27 18:52:24.000000 clarifai-9.6.1/clarifai.egg-info/entry_points.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)       52 2023-07-27 18:52:24.000000 clarifai-9.6.1/clarifai.egg-info/requires.txt
+-rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-07-27 18:52:24.000000 clarifai-9.6.1/clarifai.egg-info/top_level.txt
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.862722 clarifai-9.6.1/clarifai_utils/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.863577 clarifai-9.6.1/clarifai_utils/auth/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/auth/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    13909 2023-07-27 18:51:46.000000 clarifai-9.6.1/clarifai_utils/auth/helper.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.864830 clarifai-9.6.1/clarifai_utils/client/
+-rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/client/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/client/abc.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-07-06 20:11:16.000000 clarifai-9.6.1/clarifai_utils/client/stub.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.866575 clarifai-9.6.1/clarifai_utils/data_upload/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/data_upload/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7331 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/data_upload/convert_csv.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.869056 clarifai-9.6.1/clarifai_utils/data_upload/datasets/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2546 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/base.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1289 2023-06-02 04:02:11.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/features.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    10249 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/image.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2074 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/text.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.871709 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3684 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4894 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6291 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1605 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.748250 clarifai-9.6.1/clarifai_utils/data_upload/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.872200 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.873056 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.874012 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.874569 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_detection/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_detection/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.875471 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_detection/voc/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_detection/voc/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2692 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_detection/voc/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.876062 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_segmentation/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_segmentation/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.877112 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_segmentation/coco/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_segmentation/coco/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4235 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/image_segmentation/coco/dataset.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.877711 clarifai-9.6.1/clarifai_utils/data_upload/examples/text_classification/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.878661 clarifai-9.6.1/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.6.1/clarifai_utils/data_upload/examples.py
+-rw-r--r--   0 zeiler     (503) staff       (20)    13507 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/data_upload/upload.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.879151 clarifai-9.6.1/clarifai_utils/dataset_export/
+-rw-r--r--   0 zeiler     (503) staff       (20)     7475 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.883813 clarifai-9.6.1/clarifai_utils/listing/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/listing/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/listing/concepts.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/listing/datasets.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/listing/inputs.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.6.1/clarifai_utils/listing/installed_module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.6.1/clarifai_utils/listing/lister.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/listing/models.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.6.1/clarifai_utils/listing/module_versions.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.6.1/clarifai_utils/listing/modules.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.884878 clarifai-9.6.1/clarifai_utils/models/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     9555 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/models/api.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.886400 clarifai-9.6.1/clarifai_utils/models/model_serving/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/__init__.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.888466 clarifai-9.6.1/clarifai_utils/models/model_serving/cli/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/cli/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3825 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/cli/deploy_cli.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1866 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/cli/model_zip.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1947 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/cli/repository.py
+-rw-r--r--   0 zeiler     (503) staff       (20)      112 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/constants.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.753763 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.751138 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.751391 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.889711 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2251 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.752157 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.752798 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.891281 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2173 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.754004 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.754449 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.892201 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/
+-rw-r--r--   0 zeiler     (503) staff       (20)     2906 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.894195 clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1731 2023-07-27 16:35:09.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/deploy.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4231 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/serializer.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4489 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/triton_config.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.896345 clarifai-9.6.1/clarifai_utils/models/model_serving/models/
+-rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/models/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1639 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/models/inference.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3701 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/models/model_types.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2334 2023-07-06 20:12:20.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/models/output.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1941 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/models/pb_model.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3411 2023-07-12 02:17:25.000000 clarifai-9.6.1/clarifai_utils/models/model_serving/pb_model_repository.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.898228 clarifai-9.6.1/clarifai_utils/modules/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/modules/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/modules/css.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.6.1/clarifai_utils/modules/pages.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     6003 2023-07-27 16:35:07.000000 clarifai-9.6.1/clarifai_utils/modules/style.css
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.899112 clarifai-9.6.1/clarifai_utils/runners/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-12 02:19:11.000000 clarifai-9.6.1/clarifai_utils/runners/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3578 2023-07-12 15:26:44.000000 clarifai-9.6.1/clarifai_utils/runners/api.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.900117 clarifai-9.6.1/clarifai_utils/urls/
+-rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.6.1/clarifai_utils/urls/__init__.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4276 2023-07-07 03:41:06.000000 clarifai-9.6.1/clarifai_utils/urls/helper.py
+-rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-07-27 18:52:25.902386 clarifai-9.6.1/setup.cfg
+-rw-r--r--   0 zeiler     (503) staff       (20)     1297 2023-07-27 18:52:03.000000 clarifai-9.6.1/setup.py
+drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-27 18:52:25.901738 clarifai-9.6.1/tests/
+-rw-r--r--   0 zeiler     (503) staff       (20)     3184 2023-07-27 18:51:46.000000 clarifai-9.6.1/tests/test_auth.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     4771 2023-07-07 03:39:45.000000 clarifai-9.6.1/tests/test_modules.py
+-rw-r--r--   0 zeiler     (503) staff       (20)     3716 2023-01-03 21:48:03.000000 clarifai-9.6.1/tests/test_stub.py
```

### Comparing `clarifai-9.6.0/LICENSE` & `clarifai-9.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/PKG-INFO` & `clarifai-9.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.6.0
+Version: 9.6.1
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.6.0/README.md` & `clarifai-9.6.1/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/auth/helper.py` & `clarifai-9.6.1/clarifai/auth/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import urllib.request
-from typing import Any
+from typing import Any, Dict
 
 from clarifai_grpc.channel.clarifai_channel import ClarifaiChannel
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2_grpc
 
 DEFAULT_BASE = "https://api.clarifai.com"
 DEFAULT_UI = "https://clarifai.com"
 
@@ -57,14 +57,15 @@
       self,
       user_id: str,
       app_id: str,
       pat: str,
       token: str = "",
       base: str = DEFAULT_BASE,
       ui: str = DEFAULT_UI,
+      validate: bool = True,
   ):
     """
         A helper to get the authorization information needed to make API calls with the grpc
         client to a specific app using a personal access token.
 
         There are classmethods to make this object easily from either query_params provided by streamlit or from env vars.
 
@@ -76,73 +77,114 @@
           app_id: an app id for the application that owns the resource you want to interact with
           pat: a personal access token.
           token: a session token (internal use only, always use a PAT).
           base: a url to the API endpoint to hit. Examples include api.clarifai.com,
         https://api.clarifai.com (default), https://host:port, http://host:port, host:port (will be treated as http, not https). It's highly recommended to include the http:// or https:// otherwise we need to check the endpoint to determine if it has SSL during this __init__
           ui: a url to the UI. Examples include clarifai.com,
         https://clarifai.com (default), https://host:port, http://host:port, host:port (will be treated as http, not https). It's highly recommended to include the http:// or https:// otherwise we need to check the endpoint to determine if it has SSL during this __init__
+          validate: whether to validate the inputs. This is useful for overriding vars then validating
         """
-    if pat != "" and token != "":
-      raise Exception(
-          "A personal access token OR a session token need to be provided, but you cannot provide both."
-      )
-    elif pat == "" and token == "":
-      raise Exception(
-          "Need 'pat' or 'token' in the query params or use one of the CLARIFAI_PAT or CLARIFAI_SESSION_TOKEN env vars"
-      )
 
     self.user_id = user_id
     self.app_id = app_id
     self._pat = pat
     self._token = token
 
-    self._base = https_cache(base_https_cache, base)
-    self._ui = https_cache(ui_https_cache, ui)
+    self.set_base(base)
+    self.set_ui(ui)
+    if validate:
+      self.validate()
+
+  def validate(self):
+    if self.user_id == "":
+      raise Exception(
+          "Need 'user_id' to not be empty in the query params or user CLARIFAI_USER_ID env var")
+    if self.app_id == "":
+      raise Exception(
+          "Need 'app_id' to not be empty in the query params or user CLARIFAI_APP_ID env var")
+    if self._pat != "" and self._token != "":
+      raise Exception(
+          "A personal access token OR a session token need to be provided, but you cannot provide both."
+      )
+    elif self._pat == "" and self._token == "":
+      raise Exception(
+          "Need 'pat' or 'token' in the query params or use one of the CLARIFAI_PAT or CLARIFAI_SESSION_TOKEN env vars"
+      )
 
   @classmethod
-  def from_streamlit(cls, st: Any, fallback_to_envvars: bool = True) -> "ClarifaiAuthHelper":
-    """This is a convenient method to check the query params from streamlit for the required
-        parameters for authentication, and then optional fallback to checking environment variables as
-        well if needed.
+  def from_streamlit(cls, st: Any) -> "ClarifaiAuthHelper":
+    """ This is a convenient method to check the environment variables first to see if there are
+    required variables for auth, then override them with any additional query parameters that may
+    have been passed in.
+
+    Note: if a .streamlit/secrets.toml is present then st.secrets will auto populate the
+    corresponding environment variables and we will pick them up from there, OVERWRITING whatever
+    matching env var that may already be present.
+
         Args:
           st: the streamlit package typically as: 'import streamlit as st'
-          fallback_to_envvars: if True then when the sufficient query params are not present it will
-        check env vars. If False then we raise the query param exception directly.
         Returns:
           auth: this class instantiated
         """
+    # start with the env vars (potentially loaded from secrets.toml)
+    # Don't validate yet as we'll layer on the query params next.
+    auth = ClarifaiAuthHelper.from_env(validate=False)
+
+    # Then add in the query params.
     try:
-      auth = cls.from_streamlit_query_params(st.experimental_get_query_params())
+      auth = auth.add_streamlit_query_params(query_params)
     except Exception as e:
-      if not fallback_to_envvars:
-        st.error(e)
-        st.stop()
-        raise e
-      else:
-        st.markdown(
-            "Could not find query params in url. For development purposes we will check for env vars next."
-        )
-        try:
-          auth = ClarifaiAuthHelper.from_env()
-        except Exception as e:
-          st.error(e)
-          st.stop()
-          raise e
+      st.error(e)
+      st.stop()
+      raise e
+
+    # Then validate.
+    try:
+      auth.validate()
+    except Exception as e:
+      st.error(e)
+      st.stop()
+      raise e
+
     return auth
 
   @classmethod
   def from_streamlit_query_params(cls, query_params: Any = "") -> "ClarifaiAuthHelper":
     """Initialize from streamlit queryparams. The following things will be looked for:
           user_id: as 'user_id' in query_params
           app_id: as 'app_id' in query_params
           one of:
             token: as 'token' in query_params
             pat: as 'pat' in query_params
           optionally:
             base: as 'base' in query_params.
+            ui: as 'ui' in query_params.
+
+    """
+
+    # Setup an empty one (not from env).
+    auth = ClarifaiAuthHelper("", "", "", "", validate=False)
+
+    # Then add in the query params.
+    auth = auth.add_streamlit_query_params(query_params)
+
+    # Then validate.
+    auth.validate()
+
+    return auth
+
+  def add_streamlit_query_params(self, query_params: Any = "") -> "ClarifaiAuthHelper":
+    """Initialize from streamlit queryparams. The following things will be looked for:
+          user_id: as 'user_id' in query_params
+          app_id: as 'app_id' in query_params
+          one of:
+            token: as 'token' in query_params
+            pat: as 'pat' in query_params
+          optionally:
+            base: as 'base' in query_params.
 
         Args:
           query_params: the streamlit.experimental_get_query_params() response or an empty dict to fall
         back to using env vars.
         """
     error_description = """
 Please check the following required query params are in the url:
@@ -153,49 +195,33 @@
 Additionally, these optional params are supported:
  - 'base': the base domain for the API such as https://api.clarifai.com
  - 'ui': the overall UI domain for redirects such as https://clarifai.com
 """
 
     if query_params == "":  # empty response from streamlit
       query_params = {}
-    if "user_id" not in query_params:
-      raise Exception("You need to set 'user_id' in the query params of the url." +
-                      error_description)
-    user_id = query_params["user_id"][0]
-    if "app_id" not in query_params:
-      raise Exception("You need to set 'app_id' in the query params of the url." +
-                      error_description)
-    app_id = query_params["app_id"][0]
-
-    token = ""
-    pat = ""
-    if "token" in query_params:
-      token = query_params["token"][0]
-    if "pat" in query_params:
-      pat = query_params["pat"][0]
     for k in ["user_id", "app_id", "token", "pat"]:
       if k in query_params and len(query_params[k]) != 1:
         err_str = "There should only be 1 query param value for key '%s'" % k
         raise Exception(err_str + error_description)
-    if token == "" and pat == "":
-      raise Exception("You must provide one of 'token' or 'pat' in the query params." +
-                      error_description)
+    if "user_id" in query_params:
+      self.user_id = query_params["user_id"][0]
+    if "app_id" in query_params:
+      self.app_id = query_params["app_id"][0]
+    if "token" in query_params:
+      self._token = query_params["token"][0]
+    if "pat" in query_params:
+      self._pat = query_params["pat"][0]
     if "base" in query_params:
-      base = query_params["base"][0]
-    else:
-      base = DEFAULT_BASE
+      self.set_base(query_params["base"][0])
     if "ui" in query_params:
-      ui = query_params["ui"][0]
-    else:
-      ui = DEFAULT_BASE
-
-    return cls(user_id, app_id, pat, token, base, ui)
+      self.set_ui(query_params["ui"][0])
 
   @classmethod
-  def from_env(cls) -> "ClarifaiAuthHelper":
+  def from_env(cls, validate: bool = True) -> "ClarifaiAuthHelper":
     """Will look for the following env vars:
         user_id: CLARIFAI_USER_ID env var.
         app_id: CLARIFAI_APP_ID env var.
         one of:
           token: CLARIFAI_SESSION_TOKEN env var.
           pat: CLARIFAI_PAT env var.
         base: CLARIFAI_API_BASE env var.
@@ -206,32 +232,21 @@
  - 'CLARIFAI_APP_ID': the app the module is being accessed from.
  - 'CLARIFAI_SESSION_TOKEN' or 'CLARIFAI_PAT': to authenticate the calling user with a session token or personal access token.
 
 Additionally, these optional params are supported:
  - 'CLARIFAI_API_BASE': the base domain for the API such as https://api.clarifai.com
  - 'CLARIFAI_UI': the overall UI domain for redirects such as https://clarifai.com
 """
-    if os.environ.get("CLARIFAI_USER_ID", "") == "":
-      raise Exception("You need to set the 'CLARIFAI_USER_ID' env var." + error_description)
-    else:
-      user_id = os.environ["CLARIFAI_USER_ID"]
+    user_id = os.environ.get("CLARIFAI_USER_ID", "")
     app_id = os.environ.get("CLARIFAI_APP_ID", "")
-    token = ""
-    pat = ""
-    if os.environ.get("CLARIFAI_SESSION_TOKEN", "") != "":
-      token = os.environ["CLARIFAI_SESSION_TOKEN"]
-    if os.environ.get("CLARIFAI_PAT", "") != "":
-      pat = os.environ["CLARIFAI_PAT"]
-    if token == "" and pat == "":
-      raise Exception(
-          "You must provide one of 'CLARIFAI_SESSION_TOKEN' or 'CLARIFAI_PAT' in your env variables."
-          + error_description)
+    token = os.environ("CLARIFAI_SESSION_TOKEN", "")
+    pat = os.environ.get("CLARIFAI_PAT", "")
     base = os.environ.get("CLARIFAI_API_BASE", DEFAULT_BASE)
     ui = os.environ.get("CLARIFAI_UI", DEFAULT_UI)
-    return cls(user_id, app_id, pat, token, base, ui)
+    return cls(user_id, app_id, pat, token, base, ui, validate)
 
   def get_user_app_id_proto(
       self,
       user_id: str = None,
       app_id: str = None,
   ) -> resources_pb2.UserAppIDSet:
     """
@@ -296,14 +311,22 @@
       if not self._ui.startswith("https://"):
         return "https://" + self._ui
       return self._ui
     if not self._ui.startswith("http://"):
       return "http://" + self._ui
     return self._ui
 
+  def set_base(self, base: str):
+    """ Set the base domain for the API. """
+    self._base = https_cache(base_https_cache, base)
+
+  def set_ui(self, ui: str):
+    """ Set the domain for the UI. """
+    self._ui = https_cache(ui_https_cache, ui)
+
   @property
   def base(self) -> str:
     """ Return the base domain for the API. """
     if self._base not in base_https_cache:
       raise Exception("Cannot determine if base %s is https" % self._base)
     https = base_https_cache[self._base]
     if https:
@@ -321,7 +344,35 @@
 
   def __str__(self):
     return "ClarifaiAuthHelper:\n- base: %s\n- user_id: %s\n- app_id: %s\n" % (
         self._base,
         self.user_id,
         self.app_id,
     )
+
+  @classmethod
+  def required_env_vars(cls):
+    """ Return the list of the required environment variables. """
+    return ["CLARIFAI_USER_ID", "CLARIFAI_APP_ID", "CLARIFAI_PAT"]
+
+  @classmethod
+  def validate_secrets_dict(cls, toml_dict: Dict[str, Any]):
+    """ Validate the secrets.toml file has been filled with non-empty values for all the auth
+    parameters that are present.
+
+    We don't load the file here so that we don't need the tomli package dependency. You can simply
+    do:
+    import tomli
+
+    d = tomli.load(open("secrets.toml"))
+    ClarifaiAuthHelper.validate_secrets_dict(d)
+
+    """
+    # We don't validate the bases because they have sensible defaults
+    auth_keys = cls.required_env_vars()
+
+    for k, v in toml_dict.items():
+      if k in auth_keys:
+        if v == "":
+          raise Exception("'%s' in secrets.toml cannot be empty" % k)
+    # for all the keys that are not present, they have a non empty value.
+    return True
```

### Comparing `clarifai-9.6.0/clarifai/client/abc.py` & `clarifai-9.6.1/clarifai/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/client/stub.py` & `clarifai-9.6.1/clarifai/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/convert_csv.py` & `clarifai-9.6.1/clarifai/data_upload/convert_csv.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/datasets/base.py` & `clarifai-9.6.1/clarifai/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/datasets/features.py` & `clarifai-9.6.1/clarifai/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/datasets/image.py` & `clarifai-9.6.1/clarifai/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/datasets/text.py` & `clarifai-9.6.1/clarifai/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.6.1/clarifai/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.6.1/clarifai/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.6.1/clarifai/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.6.1/clarifai/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.6.1/clarifai/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.6.1/clarifai/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.6.1/clarifai/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/dataset.py` & `clarifai-9.6.1/clarifai/data_upload/examples/image_detection/voc/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/dataset.py` & `clarifai-9.6.1/clarifai/data_upload/examples/image_segmentation/coco/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.6.1/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/examples.py` & `clarifai-9.6.1/clarifai/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/data_upload/upload.py` & `clarifai-9.6.1/clarifai/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/dataset_export/dataset_export_inputs.py` & `clarifai-9.6.1/clarifai/dataset_export/dataset_export_inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/listing/concepts.py` & `clarifai-9.6.1/clarifai/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/listing/datasets.py` & `clarifai-9.6.1/clarifai/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/listing/inputs.py` & `clarifai-9.6.1/clarifai/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/listing/installed_module_versions.py` & `clarifai-9.6.1/clarifai/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/listing/lister.py` & `clarifai-9.6.1/clarifai/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/listing/models.py` & `clarifai-9.6.1/clarifai/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/listing/module_versions.py` & `clarifai-9.6.1/clarifai/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/listing/modules.py` & `clarifai-9.6.1/clarifai/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/api.py` & `clarifai-9.6.1/clarifai/models/api.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/__init__.py` & `clarifai-9.6.1/clarifai/models/model_serving/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/cli/__init__.py` & `clarifai-9.6.1/clarifai/models/model_serving/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/cli/deploy_cli.py` & `clarifai-9.6.1/clarifai/models/model_serving/cli/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/cli/model_zip.py` & `clarifai-9.6.1/clarifai/models/model_serving/cli/model_zip.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/cli/repository.py` & `clarifai-9.6.1/clarifai/models/model_serving/cli/repository.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py` & `clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py` & `clarifai-9.6.1/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py` & `clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py` & `clarifai-9.6.1/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py` & `clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py` & `clarifai-9.6.1/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/model_config/__init__.py` & `clarifai-9.6.1/clarifai/models/model_serving/model_config/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/model_config/deploy.py` & `clarifai-9.6.1/clarifai/models/model_serving/model_config/deploy.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/model_config/serializer.py` & `clarifai-9.6.1/clarifai/models/model_serving/model_config/serializer.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/model_config/triton_config.py` & `clarifai-9.6.1/clarifai/models/model_serving/model_config/triton_config.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/models/__init__.py` & `clarifai-9.6.1/clarifai/models/model_serving/models/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/models/inference.py` & `clarifai-9.6.1/clarifai/models/model_serving/models/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/models/model_types.py` & `clarifai-9.6.1/clarifai/models/model_serving/models/model_types.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/models/output.py` & `clarifai-9.6.1/clarifai/models/model_serving/models/output.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/models/pb_model.py` & `clarifai-9.6.1/clarifai/models/model_serving/models/pb_model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/models/model_serving/pb_model_repository.py` & `clarifai-9.6.1/clarifai/models/model_serving/pb_model_repository.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/modules/css.py` & `clarifai-9.6.1/clarifai/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/modules/pages.py` & `clarifai-9.6.1/clarifai/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/modules/style.css` & `clarifai-9.6.1/clarifai/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai/urls/helper.py` & `clarifai-9.6.1/clarifai/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai.egg-info/PKG-INFO` & `clarifai-9.6.1/clarifai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.6.0
+Version: 9.6.1
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.6.0/clarifai_utils/auth/helper.py` & `clarifai-9.6.1/clarifai_utils/auth/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import urllib.request
-from typing import Any
+from typing import Any, Dict
 
 from clarifai_grpc.channel.clarifai_channel import ClarifaiChannel
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2_grpc
 
 DEFAULT_BASE = "https://api.clarifai.com"
 DEFAULT_UI = "https://clarifai.com"
 
@@ -57,14 +57,15 @@
       self,
       user_id: str,
       app_id: str,
       pat: str,
       token: str = "",
       base: str = DEFAULT_BASE,
       ui: str = DEFAULT_UI,
+      validate: bool = True,
   ):
     """
         A helper to get the authorization information needed to make API calls with the grpc
         client to a specific app using a personal access token.
 
         There are classmethods to make this object easily from either query_params provided by streamlit or from env vars.
 
@@ -76,73 +77,114 @@
           app_id: an app id for the application that owns the resource you want to interact with
           pat: a personal access token.
           token: a session token (internal use only, always use a PAT).
           base: a url to the API endpoint to hit. Examples include api.clarifai.com,
         https://api.clarifai.com (default), https://host:port, http://host:port, host:port (will be treated as http, not https). It's highly recommended to include the http:// or https:// otherwise we need to check the endpoint to determine if it has SSL during this __init__
           ui: a url to the UI. Examples include clarifai.com,
         https://clarifai.com (default), https://host:port, http://host:port, host:port (will be treated as http, not https). It's highly recommended to include the http:// or https:// otherwise we need to check the endpoint to determine if it has SSL during this __init__
+          validate: whether to validate the inputs. This is useful for overriding vars then validating
         """
-    if pat != "" and token != "":
-      raise Exception(
-          "A personal access token OR a session token need to be provided, but you cannot provide both."
-      )
-    elif pat == "" and token == "":
-      raise Exception(
-          "Need 'pat' or 'token' in the query params or use one of the CLARIFAI_PAT or CLARIFAI_SESSION_TOKEN env vars"
-      )
 
     self.user_id = user_id
     self.app_id = app_id
     self._pat = pat
     self._token = token
 
-    self._base = https_cache(base_https_cache, base)
-    self._ui = https_cache(ui_https_cache, ui)
+    self.set_base(base)
+    self.set_ui(ui)
+    if validate:
+      self.validate()
+
+  def validate(self):
+    if self.user_id == "":
+      raise Exception(
+          "Need 'user_id' to not be empty in the query params or user CLARIFAI_USER_ID env var")
+    if self.app_id == "":
+      raise Exception(
+          "Need 'app_id' to not be empty in the query params or user CLARIFAI_APP_ID env var")
+    if self._pat != "" and self._token != "":
+      raise Exception(
+          "A personal access token OR a session token need to be provided, but you cannot provide both."
+      )
+    elif self._pat == "" and self._token == "":
+      raise Exception(
+          "Need 'pat' or 'token' in the query params or use one of the CLARIFAI_PAT or CLARIFAI_SESSION_TOKEN env vars"
+      )
 
   @classmethod
-  def from_streamlit(cls, st: Any, fallback_to_envvars: bool = True) -> "ClarifaiAuthHelper":
-    """This is a convenient method to check the query params from streamlit for the required
-        parameters for authentication, and then optional fallback to checking environment variables as
-        well if needed.
+  def from_streamlit(cls, st: Any) -> "ClarifaiAuthHelper":
+    """ This is a convenient method to check the environment variables first to see if there are
+    required variables for auth, then override them with any additional query parameters that may
+    have been passed in.
+
+    Note: if a .streamlit/secrets.toml is present then st.secrets will auto populate the
+    corresponding environment variables and we will pick them up from there, OVERWRITING whatever
+    matching env var that may already be present.
+
         Args:
           st: the streamlit package typically as: 'import streamlit as st'
-          fallback_to_envvars: if True then when the sufficient query params are not present it will
-        check env vars. If False then we raise the query param exception directly.
         Returns:
           auth: this class instantiated
         """
+    # start with the env vars (potentially loaded from secrets.toml)
+    # Don't validate yet as we'll layer on the query params next.
+    auth = ClarifaiAuthHelper.from_env(validate=False)
+
+    # Then add in the query params.
     try:
-      auth = cls.from_streamlit_query_params(st.experimental_get_query_params())
+      auth = auth.add_streamlit_query_params(query_params)
     except Exception as e:
-      if not fallback_to_envvars:
-        st.error(e)
-        st.stop()
-        raise e
-      else:
-        st.markdown(
-            "Could not find query params in url. For development purposes we will check for env vars next."
-        )
-        try:
-          auth = ClarifaiAuthHelper.from_env()
-        except Exception as e:
-          st.error(e)
-          st.stop()
-          raise e
+      st.error(e)
+      st.stop()
+      raise e
+
+    # Then validate.
+    try:
+      auth.validate()
+    except Exception as e:
+      st.error(e)
+      st.stop()
+      raise e
+
     return auth
 
   @classmethod
   def from_streamlit_query_params(cls, query_params: Any = "") -> "ClarifaiAuthHelper":
     """Initialize from streamlit queryparams. The following things will be looked for:
           user_id: as 'user_id' in query_params
           app_id: as 'app_id' in query_params
           one of:
             token: as 'token' in query_params
             pat: as 'pat' in query_params
           optionally:
             base: as 'base' in query_params.
+            ui: as 'ui' in query_params.
+
+    """
+
+    # Setup an empty one (not from env).
+    auth = ClarifaiAuthHelper("", "", "", "", validate=False)
+
+    # Then add in the query params.
+    auth = auth.add_streamlit_query_params(query_params)
+
+    # Then validate.
+    auth.validate()
+
+    return auth
+
+  def add_streamlit_query_params(self, query_params: Any = "") -> "ClarifaiAuthHelper":
+    """Initialize from streamlit queryparams. The following things will be looked for:
+          user_id: as 'user_id' in query_params
+          app_id: as 'app_id' in query_params
+          one of:
+            token: as 'token' in query_params
+            pat: as 'pat' in query_params
+          optionally:
+            base: as 'base' in query_params.
 
         Args:
           query_params: the streamlit.experimental_get_query_params() response or an empty dict to fall
         back to using env vars.
         """
     error_description = """
 Please check the following required query params are in the url:
@@ -153,49 +195,33 @@
 Additionally, these optional params are supported:
  - 'base': the base domain for the API such as https://api.clarifai.com
  - 'ui': the overall UI domain for redirects such as https://clarifai.com
 """
 
     if query_params == "":  # empty response from streamlit
       query_params = {}
-    if "user_id" not in query_params:
-      raise Exception("You need to set 'user_id' in the query params of the url." +
-                      error_description)
-    user_id = query_params["user_id"][0]
-    if "app_id" not in query_params:
-      raise Exception("You need to set 'app_id' in the query params of the url." +
-                      error_description)
-    app_id = query_params["app_id"][0]
-
-    token = ""
-    pat = ""
-    if "token" in query_params:
-      token = query_params["token"][0]
-    if "pat" in query_params:
-      pat = query_params["pat"][0]
     for k in ["user_id", "app_id", "token", "pat"]:
       if k in query_params and len(query_params[k]) != 1:
         err_str = "There should only be 1 query param value for key '%s'" % k
         raise Exception(err_str + error_description)
-    if token == "" and pat == "":
-      raise Exception("You must provide one of 'token' or 'pat' in the query params." +
-                      error_description)
+    if "user_id" in query_params:
+      self.user_id = query_params["user_id"][0]
+    if "app_id" in query_params:
+      self.app_id = query_params["app_id"][0]
+    if "token" in query_params:
+      self._token = query_params["token"][0]
+    if "pat" in query_params:
+      self._pat = query_params["pat"][0]
     if "base" in query_params:
-      base = query_params["base"][0]
-    else:
-      base = DEFAULT_BASE
+      self.set_base(query_params["base"][0])
     if "ui" in query_params:
-      ui = query_params["ui"][0]
-    else:
-      ui = DEFAULT_BASE
-
-    return cls(user_id, app_id, pat, token, base, ui)
+      self.set_ui(query_params["ui"][0])
 
   @classmethod
-  def from_env(cls) -> "ClarifaiAuthHelper":
+  def from_env(cls, validate: bool = True) -> "ClarifaiAuthHelper":
     """Will look for the following env vars:
         user_id: CLARIFAI_USER_ID env var.
         app_id: CLARIFAI_APP_ID env var.
         one of:
           token: CLARIFAI_SESSION_TOKEN env var.
           pat: CLARIFAI_PAT env var.
         base: CLARIFAI_API_BASE env var.
@@ -206,32 +232,21 @@
  - 'CLARIFAI_APP_ID': the app the module is being accessed from.
  - 'CLARIFAI_SESSION_TOKEN' or 'CLARIFAI_PAT': to authenticate the calling user with a session token or personal access token.
 
 Additionally, these optional params are supported:
  - 'CLARIFAI_API_BASE': the base domain for the API such as https://api.clarifai.com
  - 'CLARIFAI_UI': the overall UI domain for redirects such as https://clarifai.com
 """
-    if os.environ.get("CLARIFAI_USER_ID", "") == "":
-      raise Exception("You need to set the 'CLARIFAI_USER_ID' env var." + error_description)
-    else:
-      user_id = os.environ["CLARIFAI_USER_ID"]
+    user_id = os.environ.get("CLARIFAI_USER_ID", "")
     app_id = os.environ.get("CLARIFAI_APP_ID", "")
-    token = ""
-    pat = ""
-    if os.environ.get("CLARIFAI_SESSION_TOKEN", "") != "":
-      token = os.environ["CLARIFAI_SESSION_TOKEN"]
-    if os.environ.get("CLARIFAI_PAT", "") != "":
-      pat = os.environ["CLARIFAI_PAT"]
-    if token == "" and pat == "":
-      raise Exception(
-          "You must provide one of 'CLARIFAI_SESSION_TOKEN' or 'CLARIFAI_PAT' in your env variables."
-          + error_description)
+    token = os.environ("CLARIFAI_SESSION_TOKEN", "")
+    pat = os.environ.get("CLARIFAI_PAT", "")
     base = os.environ.get("CLARIFAI_API_BASE", DEFAULT_BASE)
     ui = os.environ.get("CLARIFAI_UI", DEFAULT_UI)
-    return cls(user_id, app_id, pat, token, base, ui)
+    return cls(user_id, app_id, pat, token, base, ui, validate)
 
   def get_user_app_id_proto(
       self,
       user_id: str = None,
       app_id: str = None,
   ) -> resources_pb2.UserAppIDSet:
     """
@@ -296,14 +311,22 @@
       if not self._ui.startswith("https://"):
         return "https://" + self._ui
       return self._ui
     if not self._ui.startswith("http://"):
       return "http://" + self._ui
     return self._ui
 
+  def set_base(self, base: str):
+    """ Set the base domain for the API. """
+    self._base = https_cache(base_https_cache, base)
+
+  def set_ui(self, ui: str):
+    """ Set the domain for the UI. """
+    self._ui = https_cache(ui_https_cache, ui)
+
   @property
   def base(self) -> str:
     """ Return the base domain for the API. """
     if self._base not in base_https_cache:
       raise Exception("Cannot determine if base %s is https" % self._base)
     https = base_https_cache[self._base]
     if https:
@@ -321,7 +344,35 @@
 
   def __str__(self):
     return "ClarifaiAuthHelper:\n- base: %s\n- user_id: %s\n- app_id: %s\n" % (
         self._base,
         self.user_id,
         self.app_id,
     )
+
+  @classmethod
+  def required_env_vars(cls):
+    """ Return the list of the required environment variables. """
+    return ["CLARIFAI_USER_ID", "CLARIFAI_APP_ID", "CLARIFAI_PAT"]
+
+  @classmethod
+  def validate_secrets_dict(cls, toml_dict: Dict[str, Any]):
+    """ Validate the secrets.toml file has been filled with non-empty values for all the auth
+    parameters that are present.
+
+    We don't load the file here so that we don't need the tomli package dependency. You can simply
+    do:
+    import tomli
+
+    d = tomli.load(open("secrets.toml"))
+    ClarifaiAuthHelper.validate_secrets_dict(d)
+
+    """
+    # We don't validate the bases because they have sensible defaults
+    auth_keys = cls.required_env_vars()
+
+    for k, v in toml_dict.items():
+      if k in auth_keys:
+        if v == "":
+          raise Exception("'%s' in secrets.toml cannot be empty" % k)
+    # for all the keys that are not present, they have a non empty value.
+    return True
```

### Comparing `clarifai-9.6.0/clarifai_utils/client/abc.py` & `clarifai-9.6.1/clarifai_utils/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/client/stub.py` & `clarifai-9.6.1/clarifai_utils/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/convert_csv.py` & `clarifai-9.6.1/clarifai_utils/data_upload/convert_csv.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/datasets/base.py` & `clarifai-9.6.1/clarifai_utils/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/datasets/features.py` & `clarifai-9.6.1/clarifai_utils/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/datasets/image.py` & `clarifai-9.6.1/clarifai_utils/data_upload/datasets/image.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/datasets/text.py` & `clarifai-9.6.1/clarifai_utils/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.6.1/clarifai_utils/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.6.1/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/dataset.py` & `clarifai-9.6.1/clarifai_utils/data_upload/examples/image_detection/voc/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/dataset.py` & `clarifai-9.6.1/clarifai_utils/data_upload/examples/image_segmentation/coco/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.6.1/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/examples.py` & `clarifai-9.6.1/clarifai_utils/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/data_upload/upload.py` & `clarifai-9.6.1/clarifai_utils/data_upload/upload.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/dataset_export/dataset_export_inputs.py` & `clarifai-9.6.1/clarifai_utils/dataset_export/dataset_export_inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/listing/concepts.py` & `clarifai-9.6.1/clarifai_utils/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/listing/datasets.py` & `clarifai-9.6.1/clarifai_utils/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/listing/inputs.py` & `clarifai-9.6.1/clarifai_utils/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/listing/installed_module_versions.py` & `clarifai-9.6.1/clarifai_utils/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/listing/lister.py` & `clarifai-9.6.1/clarifai_utils/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/listing/models.py` & `clarifai-9.6.1/clarifai_utils/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/listing/module_versions.py` & `clarifai-9.6.1/clarifai_utils/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/listing/modules.py` & `clarifai-9.6.1/clarifai_utils/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/api.py` & `clarifai-9.6.1/clarifai_utils/models/api.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/__init__.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/cli/__init__.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/cli/deploy_cli.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/cli/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/cli/model_zip.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/cli/model_zip.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/cli/repository.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/cli/repository.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/__init__.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/deploy.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/deploy.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/serializer.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/serializer.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/triton_config.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/model_config/triton_config.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/models/__init__.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/models/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/models/inference.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/models/inference.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/models/model_types.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/models/model_types.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/models/output.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/models/output.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/models/pb_model.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/models/pb_model.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/models/model_serving/pb_model_repository.py` & `clarifai-9.6.1/clarifai_utils/models/model_serving/pb_model_repository.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/modules/css.py` & `clarifai-9.6.1/clarifai_utils/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/modules/pages.py` & `clarifai-9.6.1/clarifai_utils/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/modules/style.css` & `clarifai-9.6.1/clarifai_utils/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/clarifai_utils/urls/helper.py` & `clarifai-9.6.1/clarifai_utils/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/setup.py` & `clarifai-9.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 packages = setuptools.find_namespace_packages(include=["clarifai*"])
 
 setuptools.setup(
     name="clarifai",
-    version="9.6.0",
+    version="9.6.1",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai Python Utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-utils",
     packages=packages,
```

### Comparing `clarifai-9.6.0/tests/test_auth.py` & `clarifai-9.6.1/tests/test_auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -65,7 +65,33 @@
   def raise_exception():
     return Mock(side_effect=Exception("Has SSL in error"))
 
   with mock.patch('urllib.request.urlopen', new_callable=raise_exception):
     with pytest.raises(
         Exception, match="When providing an insecure url it must have both host:port format"):
       ClarifaiAuthHelper("clarifai", "main", "fake_pat", ui="localhost")
+
+
+def test_exception_empty_user():
+  ClarifaiAuthHelper("", "main", "fake_pat", validate=False)
+  with pytest.raises(
+      Exception,
+      match="Need 'user_id' to not be empty in the query params or user CLARIFAI_USER_ID env var"):
+    ClarifaiAuthHelper("", "main", "fake_pat")
+
+
+def test_exception_empty_app():
+  ClarifaiAuthHelper("clarifai", "", "fake_pat", validate=False)
+  with pytest.raises(
+      Exception,
+      match="Need 'app_id' to not be empty in the query params or user CLARIFAI_APP_ID env var"):
+    ClarifaiAuthHelper("clarifai", "", "fake_pat")
+
+
+def test_exception_empty_pat():
+  ClarifaiAuthHelper("clarifai", "main", "", validate=False)
+  with pytest.raises(
+      Exception,
+      match=
+      "Need 'pat' or 'token' in the query params or use one of the CLARIFAI_PAT or CLARIFAI_SESSION_TOKEN env vars"
+  ):
+    ClarifaiAuthHelper("clarifai", "main", "")
```

### Comparing `clarifai-9.6.0/tests/test_modules.py` & `clarifai-9.6.1/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.6.0/tests/test_stub.py` & `clarifai-9.6.1/tests/test_stub.py`

 * *Files identical despite different names*

