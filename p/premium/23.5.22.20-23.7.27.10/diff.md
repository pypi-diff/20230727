# Comparing `tmp/premium-23.5.22.20.tar.gz` & `tmp/premium-23.7.27.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/premium-23.5.22.20.tar", last modified: Mon May 22 12:41:45 2023, max compression
+gzip compressed data, was "dist/premium-23.7.27.10.tar", last modified: Thu Jul 27 02:29:50 2023, max compression
```

## Comparing `premium-23.5.22.20.tar` & `premium-23.7.27.10.tar`

### file list

```diff
@@ -1,128 +1,156 @@
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.110556 premium-23.5.22.20/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      351 2023-05-22 12:41:45.110556 premium-23.5.22.20/PKG-INFO
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-08-20 00:45:22.000000 premium-23.5.22.20/README.md
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.026556 premium-23.5.22.20/data/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2022-11-05 09:52:56.000000 premium-23.5.22.20/data/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.026556 premium-23.5.22.20/data/config/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2022-11-05 09:52:37.000000 premium-23.5.22.20/data/config/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.030556 premium-23.5.22.20/premium/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       46 2023-04-12 13:39:31.000000 premium-23.5.22.20/premium/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.030556 premium-23.5.22.20/premium/algorithm/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-09-18 07:48:09.000000 premium-23.5.22.20/premium/algorithm/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.030556 premium-23.5.22.20/premium/automl/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      726 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/automl/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.030556 premium-23.5.22.20/premium/base/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-02-28 03:25:12.000000 premium-23.5.22.20/premium/base/__init__.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      988 2023-02-28 03:25:36.000000 premium-23.5.22.20/premium/base/pipeline.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.030556 premium-23.5.22.20/premium/classifiers/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-04-12 08:44:25.000000 premium-23.5.22.20/premium/classifiers/__init__.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     4771 2023-05-22 06:43:29.000000 premium-23.5.22.20/premium/classifiers/baseline.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.030556 premium-23.5.22.20/premium/classifiers/binary/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-05-08 09:46:49.000000 premium-23.5.22.20/premium/classifiers/binary/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      111 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/config.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.034556 premium-23.5.22.20/premium/corpus/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       30 2023-02-13 02:48:47.000000 premium-23.5.22.20/premium/corpus/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1074 2023-02-16 01:59:57.000000 premium-23.5.22.20/premium/corpus/stopwords.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      933 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/corpus/texts.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      447 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/corpus/utils.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.034556 premium-23.5.22.20/premium/data/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        4 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/data/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3344 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/data/_dict.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2136 2022-08-21 08:32:02.000000 premium-23.5.22.20/premium/data/augumentation.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.038556 premium-23.5.22.20/premium/data/classification/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2022-12-15 03:45:19.000000 premium-23.5.22.20/premium/data/classification/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3682 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/data/csv.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     9264 2023-05-17 00:48:53.000000 premium-23.5.22.20/premium/data/datasets.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3002 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/data/eda.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1418 2022-12-19 07:47:54.000000 premium-23.5.22.20/premium/data/loader.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     2277 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/data/postprocess.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)    12455 2023-04-28 13:08:42.000000 premium-23.5.22.20/premium/data/preprocess.py
--rwxrwxr-x   0 gaoang    (1001) gaoang    (1001)     4670 2022-12-22 11:10:43.000000 premium-23.5.22.20/premium/data/utils.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6551 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/demo.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      684 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/draw.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.038556 premium-23.5.22.20/premium/experimental/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/experimental/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     6624 2022-08-31 13:10:31.000000 premium-23.5.22.20/premium/experimental/cbow.py
--rwxr-xr-x   0 gaoang    (1001) gaoang    (1001)     2569 2022-09-06 07:29:08.000000 premium-23.5.22.20/premium/experimental/eda.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1462 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/experimental/kaggle.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     8572 2023-04-12 10:55:43.000000 premium-23.5.22.20/premium/experimental/myfasttext.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1498 2022-09-06 23:56:22.000000 premium-23.5.22.20/premium/experimental/ner.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2272 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/experimental/nn_metric.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     2914 2022-11-01 04:49:36.000000 premium-23.5.22.20/premium/experimental/segment_train.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     3315 2022-09-02 02:26:29.000000 premium-23.5.22.20/premium/experimental/textnn.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)    14328 2022-12-19 07:00:16.000000 premium-23.5.22.20/premium/experimental/torch_crf.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2385 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/frame.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     8076 2022-09-27 06:32:40.000000 premium-23.5.22.20/premium/hmm.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.038556 premium-23.5.22.20/premium/lightning/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-04-17 06:05:11.000000 premium-23.5.22.20/premium/lightning/__init__.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     2213 2023-05-04 13:34:16.000000 premium-23.5.22.20/premium/lightning/callbacks.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.082556 premium-23.5.22.20/premium/localdata/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)  1001504 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/localdata/27.mp3
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)  5340812 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/localdata/27.wav
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4695 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/localdata/cn_stopwords.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)  1134854 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/localdata/dict.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)   278548 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/localdata/emit_p.pickle
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      621 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/localdata/en_stopwords.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       61 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/localdata/oov.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)   844962 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/localdata/puredict.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)   755791 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/localdata/soledad.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      176 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/localdata/trans.pickle
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)  7310398 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/localdata/xinhua.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2803 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/measure.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.098556 premium-23.5.22.20/premium/metrics/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      660 2023-03-22 07:48:42.000000 premium-23.5.22.20/premium/metrics/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)      876 2022-10-22 08:56:25.000000 premium-23.5.22.20/premium/metrics/distance.py
--rwxr-xr-x   0 gaoang    (1001) gaoang    (1001)     2990 2023-04-12 11:56:01.000000 premium-23.5.22.20/premium/metrics/metrix.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.102556 premium-23.5.22.20/premium/models/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       42 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6835 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/base.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      200 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/bayes.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3178 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/benchmark.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)    15555 2022-09-02 07:01:51.000000 premium-23.5.22.20/premium/models/bert.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6238 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/binary_classifiers.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3939 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/clf.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)    10472 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/lgb.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2697 2022-11-03 11:20:22.000000 premium-23.5.22.20/premium/models/model_config.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6144 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/multi_classifier.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)    22231 2022-09-04 03:09:30.000000 premium-23.5.22.20/premium/models/nn.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4954 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/optuna.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     7796 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/regressor.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.106556 premium-23.5.22.20/premium/models/tensorflow/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      127 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/tensorflow/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2857 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/tensorflow/binary_classifier.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      186 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/tensorflow/info.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)    11038 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/touchstone.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1783 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/models/xgb.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.106556 premium-23.5.22.20/premium/nlp/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       66 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/nlp/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3209 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/nlp/metrics.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1212 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/nlp/net.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1086 2022-09-06 23:53:01.000000 premium-23.5.22.20/premium/nlp/nlp.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.106556 premium-23.5.22.20/premium/preprocessing/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-09-04 01:32:49.000000 premium-23.5.22.20/premium/preprocessing/__init__.py
--rwxrwxr-x   0 gaoang    (1001) gaoang    (1001)     2933 2023-05-04 12:57:40.000000 premium-23.5.22.20/premium/preprocessing/ner.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      425 2023-05-10 08:21:09.000000 premium-23.5.22.20/premium/preprocessing/text.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.106556 premium-23.5.22.20/premium/pytorch/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      849 2022-11-11 02:06:02.000000 premium-23.5.22.20/premium/pytorch/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1772 2023-02-16 13:53:00.000000 premium-23.5.22.20/premium/pytorch/data.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2471 2022-12-08 04:52:17.000000 premium-23.5.22.20/premium/pytorch/tokenizer.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2136 2022-11-11 03:50:39.000000 premium-23.5.22.20/premium/pytorch/trainer.py
--rwxr-xr-x   0 gaoang    (1001) gaoang    (1001)      275 2022-12-15 03:41:20.000000 premium-23.5.22.20/premium/pytorch/utils.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     5369 2022-09-14 00:12:27.000000 premium-23.5.22.20/premium/segment.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.110556 premium-23.5.22.20/premium/text_feature/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       36 2022-11-23 03:47:20.000000 premium-23.5.22.20/premium/text_feature/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4938 2022-11-23 03:47:52.000000 premium-23.5.22.20/premium/text_feature/bm25.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3362 2022-11-29 11:47:18.000000 premium-23.5.22.20/premium/text_feature/sif.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.110556 premium-23.5.22.20/premium/utils/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1661 2022-12-06 08:25:40.000000 premium-23.5.22.20/premium/utils/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      563 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/utils/decorators.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      988 2022-08-20 00:43:56.000000 premium-23.5.22.20/premium/zz.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-22 12:41:45.030556 premium-23.5.22.20/premium.egg-info/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      351 2023-05-22 12:41:44.000000 premium-23.5.22.20/premium.egg-info/PKG-INFO
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     2757 2023-05-22 12:41:44.000000 premium-23.5.22.20/premium.egg-info/SOURCES.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-05-22 12:41:44.000000 premium-23.5.22.20/premium.egg-info/dependency_links.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       65 2023-05-22 12:41:44.000000 premium-23.5.22.20/premium.egg-info/entry_points.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       76 2023-05-22 12:41:44.000000 premium-23.5.22.20/premium.egg-info/requires.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       13 2023-05-22 12:41:44.000000 premium-23.5.22.20/premium.egg-info/top_level.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-05-22 12:41:45.110556 premium-23.5.22.20/setup.cfg
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1133 2023-05-09 16:25:54.000000 premium-23.5.22.20/setup.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.532264 premium-23.7.27.10/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      351 2023-07-27 02:29:50.532264 premium-23.7.27.10/PKG-INFO
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-08-20 00:45:22.000000 premium-23.7.27.10/README.md
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.428263 premium-23.7.27.10/data/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2022-11-05 09:52:56.000000 premium-23.7.27.10/data/__init__.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.428263 premium-23.7.27.10/data/config/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2022-11-05 09:52:37.000000 premium-23.7.27.10/data/config/__init__.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.432263 premium-23.7.27.10/premium/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       46 2023-04-12 13:39:31.000000 premium-23.7.27.10/premium/__init__.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.432263 premium-23.7.27.10/premium/algorithm/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-09-18 07:48:09.000000 premium-23.7.27.10/premium/algorithm/__init__.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.432263 premium-23.7.27.10/premium/automl/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      726 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/automl/__init__.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.432263 premium-23.7.27.10/premium/base/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-02-28 03:25:12.000000 premium-23.7.27.10/premium/base/__init__.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      988 2023-02-28 03:25:36.000000 premium-23.7.27.10/premium/base/pipeline.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.436263 premium-23.7.27.10/premium/classifiers/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-04-12 08:44:25.000000 premium-23.7.27.10/premium/classifiers/__init__.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     4776 2023-06-02 05:51:38.000000 premium-23.7.27.10/premium/classifiers/baseline.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3923 2023-06-07 15:55:21.000000 premium-23.7.27.10/premium/classifiers/bases.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.436263 premium-23.7.27.10/premium/classifiers/binary/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-05-08 09:46:49.000000 premium-23.7.27.10/premium/classifiers/binary/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4566 2023-06-27 12:49:13.000000 premium-23.7.27.10/premium/classifiers/binary/benchmark.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     7285 2023-06-07 16:06:11.000000 premium-23.7.27.10/premium/classifiers/binary/bert.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     8609 2023-06-27 11:26:46.000000 premium-23.7.27.10/premium/classifiers/binary/lstm.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     2276 2023-05-31 10:24:47.000000 premium-23.7.27.10/premium/classifiers/binary/mlp.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1666 2023-06-27 09:54:58.000000 premium-23.7.27.10/premium/classifiers/binary/nb.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3285 2023-06-27 09:54:56.000000 premium-23.7.27.10/premium/classifiers/binary/textfast.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2590 2023-06-07 14:25:26.000000 premium-23.7.27.10/premium/classifiers/dataset.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.440263 premium-23.7.27.10/premium/classifiers/multi/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-06-27 09:02:31.000000 premium-23.7.27.10/premium/classifiers/multi/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4098 2023-07-01 10:26:31.000000 premium-23.7.27.10/premium/classifiers/multi/benchmark.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     5420 2023-07-25 04:15:37.000000 premium-23.7.27.10/premium/classifiers/multi/lstm.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6072 2023-06-30 02:48:34.000000 premium-23.7.27.10/premium/classifiers/multi/macbert.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      159 2023-06-27 09:54:48.000000 premium-23.7.27.10/premium/classifiers/multi/nb.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     2993 2023-06-27 09:54:46.000000 premium-23.7.27.10/premium/classifiers/multi/textfast.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      270 2023-06-06 12:35:41.000000 premium-23.7.27.10/premium/classifiers/tokenizers.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      987 2023-06-27 09:51:36.000000 premium-23.7.27.10/premium/classifiers/tree_models.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      789 2023-06-05 12:01:42.000000 premium-23.7.27.10/premium/classifiers/voting.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      111 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/config.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.440263 premium-23.7.27.10/premium/corpus/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       30 2023-02-13 02:48:47.000000 premium-23.7.27.10/premium/corpus/__init__.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1074 2023-02-16 01:59:57.000000 premium-23.7.27.10/premium/corpus/stopwords.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      933 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/corpus/texts.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      447 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/corpus/utils.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.448264 premium-23.7.27.10/premium/data/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)        4 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/data/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3344 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/data/_dict.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2136 2022-08-21 08:32:02.000000 premium-23.7.27.10/premium/data/augumentation.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.448264 premium-23.7.27.10/premium/data/classification/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2022-12-15 03:45:19.000000 premium-23.7.27.10/premium/data/classification/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3682 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/data/csv.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)    10017 2023-07-25 02:22:15.000000 premium-23.7.27.10/premium/data/datasets.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3002 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/data/eda.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1418 2022-12-19 07:47:54.000000 premium-23.7.27.10/premium/data/loader.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     2277 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/data/postprocess.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)    12455 2023-04-28 13:08:42.000000 premium-23.7.27.10/premium/data/preprocess.py
+-rwxrwxr-x   0 gaoang    (1001) gaoang    (1001)     4670 2022-12-22 11:10:43.000000 premium-23.7.27.10/premium/data/utils.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.452263 premium-23.7.27.10/premium/experimental/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/experimental/__init__.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     6624 2022-08-31 13:10:31.000000 premium-23.7.27.10/premium/experimental/cbow.py
+-rwxr-xr-x   0 gaoang    (1001) gaoang    (1001)     2569 2022-09-06 07:29:08.000000 premium-23.7.27.10/premium/experimental/eda.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1462 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/experimental/kaggle.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     8572 2023-04-12 10:55:43.000000 premium-23.7.27.10/premium/experimental/myfasttext.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1498 2022-09-06 23:56:22.000000 premium-23.7.27.10/premium/experimental/ner.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2272 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/experimental/nn_metric.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     2889 2023-05-26 06:17:31.000000 premium-23.7.27.10/premium/experimental/segment_train.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     3315 2022-09-02 02:26:29.000000 premium-23.7.27.10/premium/experimental/textnn.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)    14328 2022-12-19 07:00:16.000000 premium-23.7.27.10/premium/experimental/torch_crf.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.452263 premium-23.7.27.10/premium/lightning/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-04-17 06:05:11.000000 premium-23.7.27.10/premium/lightning/__init__.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      579 2023-07-25 11:54:53.000000 premium-23.7.27.10/premium/lightning/base.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2928 2023-07-26 07:08:58.000000 premium-23.7.27.10/premium/lightning/callbacks.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.496264 premium-23.7.27.10/premium/localdata/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)  1001504 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/localdata/27.mp3
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)  5340812 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/localdata/27.wav
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4695 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/localdata/cn_stopwords.txt
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)  1134854 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/localdata/dict.txt
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)   278548 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/localdata/emit_p.pickle
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      621 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/localdata/en_stopwords.txt
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       61 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/localdata/oov.txt
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)   844962 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/localdata/puredict.txt
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)   755791 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/localdata/soledad.txt
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      176 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/localdata/trans.pickle
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)  7310398 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/localdata/xinhua.txt
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2803 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/measure.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.520264 premium-23.7.27.10/premium/metrics/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      660 2023-03-22 07:48:42.000000 premium-23.7.27.10/premium/metrics/__init__.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)      876 2022-10-22 08:56:25.000000 premium-23.7.27.10/premium/metrics/distance.py
+-rwxr-xr-x   0 gaoang    (1001) gaoang    (1001)     2990 2023-04-12 11:56:01.000000 premium-23.7.27.10/premium/metrics/metrix.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.524264 premium-23.7.27.10/premium/models/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       42 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6835 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/base.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3178 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/benchmark.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)    15555 2022-09-02 07:01:51.000000 premium-23.7.27.10/premium/models/bert.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6238 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/binary_classifiers.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3939 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/clf.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)    10472 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/lgb.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2697 2022-11-03 11:20:22.000000 premium-23.7.27.10/premium/models/model_config.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6144 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/multi_classifier.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)    22231 2022-09-04 03:09:30.000000 premium-23.7.27.10/premium/models/nn.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4954 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/optuna.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     7796 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/regressor.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.524264 premium-23.7.27.10/premium/models/tensorflow/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      127 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/tensorflow/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2857 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/tensorflow/binary_classifier.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      186 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/tensorflow/info.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)    11038 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/touchstone.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1783 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/models/xgb.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.524264 premium-23.7.27.10/premium/ner/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-05-24 08:16:43.000000 premium-23.7.27.10/premium/ner/__init__.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      463 2023-05-24 08:17:08.000000 premium-23.7.27.10/premium/ner/bert.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.528264 premium-23.7.27.10/premium/nlp/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       66 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/nlp/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3209 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/nlp/metrics.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1212 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/nlp/net.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1086 2022-09-06 23:53:01.000000 premium-23.7.27.10/premium/nlp/nlp.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.528264 premium-23.7.27.10/premium/preprocessing/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-09-04 01:32:49.000000 premium-23.7.27.10/premium/preprocessing/__init__.py
+-rwxr--r--   0 gaoang    (1001) gaoang    (1001)     5677 2023-07-27 02:19:00.000000 premium-23.7.27.10/premium/preprocessing/ner.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      425 2023-05-10 08:21:09.000000 premium-23.7.27.10/premium/preprocessing/text.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-06-02 04:35:07.000000 premium-23.7.27.10/premium/preprocessing/vectorizer.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.528264 premium-23.7.27.10/premium/pytorch/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      849 2022-11-11 02:06:02.000000 premium-23.7.27.10/premium/pytorch/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2271 2023-06-05 11:33:22.000000 premium-23.7.27.10/premium/pytorch/data.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     7648 2023-06-28 16:31:31.000000 premium-23.7.27.10/premium/pytorch/tokenizer.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2136 2022-11-11 03:50:39.000000 premium-23.7.27.10/premium/pytorch/trainer.py
+-rwxr-xr-x   0 gaoang    (1001) gaoang    (1001)      275 2022-12-15 03:41:20.000000 premium-23.7.27.10/premium/pytorch/utils.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     5369 2022-09-14 00:12:27.000000 premium-23.7.27.10/premium/segment.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.528264 premium-23.7.27.10/premium/text_feature/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       36 2022-11-23 03:47:20.000000 premium-23.7.27.10/premium/text_feature/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     5642 2023-07-03 12:39:38.000000 premium-23.7.27.10/premium/text_feature/bm25.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3362 2022-11-29 11:47:18.000000 premium-23.7.27.10/premium/text_feature/sif.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.532264 premium-23.7.27.10/premium/topics/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-07-11 08:02:22.000000 premium-23.7.27.10/premium/topics/__init__.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     2407 2023-07-11 08:16:23.000000 premium-23.7.27.10/premium/topics/lsa.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.532264 premium-23.7.27.10/premium/utils/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1661 2022-12-06 08:25:40.000000 premium-23.7.27.10/premium/utils/__init__.py
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      563 2022-08-20 00:43:56.000000 premium-23.7.27.10/premium/utils/decorators.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.532264 premium-23.7.27.10/premium/wheels/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       36 2023-07-04 04:32:28.000000 premium-23.7.27.10/premium/wheels/__init__.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.532264 premium-23.7.27.10/premium/wheels/transformers/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-07-04 12:05:08.000000 premium-23.7.27.10/premium/wheels/transformers/__init__.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     3099 2023-07-19 11:17:05.000000 premium-23.7.27.10/premium/wheels/transformers/layers.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.432263 premium-23.7.27.10/premium.egg-info/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      351 2023-07-27 02:29:50.000000 premium-23.7.27.10/premium.egg-info/PKG-INFO
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     3558 2023-07-27 02:29:50.000000 premium-23.7.27.10/premium.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-07-27 02:29:50.000000 premium-23.7.27.10/premium.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       65 2023-07-27 02:29:50.000000 premium-23.7.27.10/premium.egg-info/entry_points.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      141 2023-07-27 02:29:50.000000 premium-23.7.27.10/premium.egg-info/requires.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       19 2023-07-27 02:29:50.000000 premium-23.7.27.10/premium.egg-info/top_level.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-07-27 02:29:50.532264 premium-23.7.27.10/setup.cfg
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1213 2023-06-30 08:25:02.000000 premium-23.7.27.10/setup.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-07-27 02:29:50.532264 premium-23.7.27.10/tests/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-05-29 02:33:14.000000 premium-23.7.27.10/tests/__init__.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1139 2023-05-29 02:43:39.000000 premium-23.7.27.10/tests/test_preprocessing_ner.py
```

### Comparing `premium-23.5.22.20/premium/automl/__init__.py` & `premium-23.7.27.10/premium/automl/__init__.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/base/pipeline.py` & `premium-23.7.27.10/premium/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/classifiers/baseline.py` & `premium-23.7.27.10/premium/classifiers/baseline.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 class TencentPretrainedVectorDownloader(BeeMaxin):
 
     def __init__(self, vector_name: str = 'tencent_cn_1M.txt'):
         super().__init__()
         self.vector_name = vector_name
 
-    def process(self):
+    def process(self)->str:
         return downloader.get(self.vector_name)
 
 
 class CsvLoader(BeeMaxin):
 
     def __init__(self, csv_path: str):
         super().__init__()
```

### Comparing `premium-23.5.22.20/premium/corpus/stopwords.py` & `premium-23.7.27.10/premium/corpus/stopwords.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/corpus/texts.py` & `premium-23.7.27.10/premium/corpus/texts.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/data/_dict.py` & `premium-23.7.27.10/premium/data/_dict.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/data/augumentation.py` & `premium-23.7.27.10/premium/data/augumentation.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/data/csv.py` & `premium-23.7.27.10/premium/data/csv.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/data/datasets.py` & `premium-23.7.27.10/premium/data/datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 #!/usr/bin/env python
 # Datasets manager.
 import os
 import pickle
 import re
 from dataclasses import dataclass
-from typing import Dict, List, Optional, Set, Tuple, TypeVar
+from typing import List, TypeVar
 
 import codefast as cf
 import numpy as np
+import pandas as pd
 
 from premium.utils import md5sum
 
 
 class Urls(object):
-    prefix = 'https://filedn.com/lCdtpv3siVybVynPcgXgnPm/corpus'
+    # prefix = 'https://filedn.com/lCdtpv3siVybVynPcgXgnPm/corpus'
+    prefix = 'https://file.ddot.cc/corpus'
 
 
 Path = TypeVar('Path', str, List[str])
 
 
 def fetch_from_url(remote_url: str):
     target = f'/tmp/{cf.io.basename(remote_url)}'
     cf.info(f'downloading {remote_url}')
     cf.net.download(remote_url, target)
     # unzip data if necessary
     if target.endswith(('.zip', '.gz')):
         cf.info(f'Unzip file {target}')
         cf.shell(f'7z x {target} -o/tmp -y')
+    return target
 
 
 def fetch_data(fpath: str, sub_dir: str = None) -> None:
     cf.info(f'Downloading {fpath}')
     # support downloading model from third party
     if re.search('^http', fpath):
         online_url = fpath
     else:
         online_url = os.path.join(Urls.prefix, fpath)
         if sub_dir:
             online_url = cf.urljoin(Urls.prefix, sub_dir, fpath)
-    fetch_from_url(online_url)
+    return fetch_from_url(online_url)
 
 
 @dataclass
 class DataFile(object):
     label: str
     name: str
     path: str
@@ -71,17 +74,16 @@
             DataFile('glove-twitter-200-pickle',
                      'glove.twitter.200d.pkl',
                      'pretrained/glove.twitter.200d.pkl',
                      md5sum='3cc00e6be9a9895ff3d0e4b41898d509'),
             DataFile('tencent-embedding-100-small',
                      'tencent-embedding-100-small.pkl',
                      'pretrained/tencent-embedding-100-small.pkl'),
-            DataFile('tencent-embedding-200-small',
-                     'tencent-embedding-200-small.pkl',
-                     'pretrained/tencent-embedding-200-small.pkl'),
+            DataFile('tencent-embedding-200', 'tencent-embedding-200.txt',
+                     'pretrained/tencent_cn/tencent_cn_1M.txt'),
             DataFile('glove-twitter-25', 'glove.twitter.27B.25d.txt',
                      'pretrained/glove.twitter.27B.25d.txt.gz'),
             DataFile('glove-twitter-50', 'glove.twitter.27B.50d.txt',
                      'pretrained/glove.twitter.27B.50d.txt.gz'),
             DataFile('glove-twitter-100',
                      'glove.twitter.27B.100d.txt',
                      'pretrained/glove.twitter.27B.100d.txt.gz',
@@ -109,140 +111,158 @@
     def list(self) -> list:
         return self.data_files
 
     def load_local(self, vector_file: str) -> dict:
         return dict(
             Math.get_coefs(*o.strip().split()) for o in cf.io.iter(vector_file))
 
-    def pull(self, vector_name:str)->str:
+    def pull(self, vector_name: str) -> str:
         """ Download vector file from remote url
         """
         if vector_name not in self.vectors:
             cf.warning(f'{vector_name} was not here')
             return
         df = self.vectors[vector_name]
         file_name = f'/tmp/{df.name}'
         if cf.io.exists(file_name) and md5sum(file_name) == df.md5sum:
             cf.info('{} exists and is valid, skip downloading'.format(df.name))
         else:
-            fetch_data(df.path)
+            return fetch_data(df.path)
         return file_name
 
     def load(self, vector: str = 'glove-twitter-25'):
         file_name = self.pull(vector)
         cf.info(f'loading {vector}')
         if file_name.endswith('.pkl'):
             return pickle.load(open(file_name, 'rb'))
         elif vector == 'google-news-negative-300':
             return KeyedVectors.load_word2vec_format(
                 '/tmp/GoogleNews-vectors-negative300.bin', binary=True)
         else:
             from gensim.models import KeyedVectors
             return KeyedVectors.load_word2vec_format(file_name)
-        
+
 
 word2vec = WordToVector()
 
 
 class Downloader(object):
 
     def twitter_disaster(self):
         """ Twitter real disaster or not """
         cf.info('Downloading twitter disaster data')
-        fetch_data('twitter_disaster.csv', sub_dir='classification')
+        return fetch_data('twitter_disaster.csv', sub_dir='classification')
 
     def imdb(self):
         """ Englis imdb sentiment analysis 50000
         """
         cf.info('Downloading imdg sentiment dataset')
-        fetch_data('imdb_sentiment.csv', sub_dir='classification')
+        return fetch_data('imdb_sentiment.csv', sub_dir='classification')
 
     def douban_movie_review(self):
         '''Kaggle dataset https://www.kaggle.com/liujt14/dou-ban-movie-short-comments-10377movies
         size: 686 MB
         '''
         cf.info(
             'Downloading douban movie review data: https://www.kaggle.com/liujt14/dou-ban-movie-short-comments-10377movies',
         )
-        fetch_data('douban_movie_review.zip')
+        return fetch_data('douban_movie_review.zip')
 
     def douban_movie_review_2(self):
-        fetch_data('douban_movie_review2.csv.zip')
+        return fetch_data('douban_movie_review2.csv.zip')
 
     def chinese_mnist(self):
         '''https://www.kaggle.com/fedesoriano/chinese-mnist-digit-recognizer'''
-        fetch_data('Chinese_MNIST.csv.zip')
+        return fetch_data('Chinese_MNIST.csv.zip')
 
     def toxic_comments(self):
-        fetch_data('toxic_comments.csv')
+        return fetch_data('toxic_comments.csv')
 
     def icwb(self):
         '''Data source: http://sighan.cs.uchicago.edu/bakeoff2005/
         '''
-        fetch_data('icwb2-data.zip')
+        return fetch_data('icwb2-data.zip')
 
     def news2016(self):
         ''' 中文新闻 3.6 GB 2016年语料 
         '''
-        fetch_data('news2016.zip')
+        return fetch_data('news2016.zip')
 
     def msr_training(self):
-        fetch_data('msr_training.utf8')
+        return fetch_data('msr_training.utf8')
 
     def realty_roles(self):
-        fetch_data('realty_roles.zip')
         cf.info('unzip files to /tmp/customer.txt and /tmp/salesman.txt')
+        return fetch_data('realty_roles.zip')
 
     def realty(self):
         import getpass
         cf.info("Download real estate dataset realty.csv")
         zipped_data = os.path.join(Urls.prefix, 'realty.zip')
         cf.net.download(zipped_data, '/tmp/realty.zip')
         passphrase = getpass.getpass('Type in your password: ').rstrip()
         cf.utils.shell(f'unzip -o -P {passphrase} /tmp/realty.zip -d /tmp/')
 
     def spam_en(self):
         cf.info(f'Downloading English spam ham dataset to')
-        fetch_data('spam-ham.txt')
+        return fetch_data('spam-ham.csv')
 
     def spam_cn(self, path: str = '/tmp/'):
         cf.info(f'Downloading Chinese spam ham dataset to {path}')
         zipped_data = os.path.join(Urls.prefix, 'spam_cn.zip')
         label_file = os.path.join(Urls.prefix, 'spam_cn.json')
         cf.net.download(zipped_data, '/tmp/tmp_spam.zip')
         cf.utils.shell('unzip -o /tmp/tmp_spam.zip -d /tmp/')
         cf.net.download(label_file, '/tmp/spam_cn.json')
 
     def get_waimai_10k(self):
         # 某外卖平台收集的用户评价，正向 4000 条，负向约 8000 条
-        fetch_data('waimai_10k.csv', 'classification')
+        return fetch_data('waimai_10k.csv', 'classification')
+
+    def ten_cats(self):
+        """
+        以下 10 分类的简单版本:
+        ```
+            label,text
+            0,做父母一定要有刘墉这样的心态，不断地学习，不断地进步
+            0,作者真有英国人严谨的风格，提出观点、进行论述论证
+            0,作者长篇大论借用详细报告数据处理工作和计算结果支持其新观点。
+        ```
+        """
+        pth = fetch_data('ten_cats.csv', 'classification')
+        return pth 
 
     def get_online_shopping_10_cats(self):
         """10 个类别（书籍、平板、手机、水果、洗发水、热水器、蒙牛、衣服、计算机、酒店），共 6 万多条评论数据
         正、负向评论各约 3 万条
         """
-        fetch_data('online_shopping_10_cats.csv', 'classification')
+        pth = fetch_data('online_shopping_10_cats.csv', 'classification')
+
+        df = pd.read_csv(pth)
+        df['text'] = df['review']
+        df.to_csv(pth, index=False)
+        return pth
 
     def chn_senti(self):
         """ 中文情感分析数据集. tag 用于区别 train(9000), test(2000), dev(20000)
         tag,label,text
         train,1,就是方便...
         test,1,....
         dev,1111
         """
-        fetch_data('chn_senti_corp.csv', 'classification')
+        return fetch_data('chn_senti_corp.csv', 'classification')
 
     def snli(self):
         fetch_from_url('https://host.ddot.cc/snli.zip')
 
     def mnli(self):
         """ Chinese-MNLI 自然语言推理数据集
         https://jishuin.proginn.com/p/763bfbd72666
         """
-        fetch_from_url('https://host.ddot.cc/mnli.zip')
+        return fetch_from_url('https://host.ddot.cc/mnli.zip')
 
     def get(self, filename: str) -> str:
         url_map = {
             'tencent_cn_1M.txt':
             'https://filedn.com/lCdtpv3siVybVynPcgXgnPm/corpus/pretrained/tencent_cn/tencent_cn_1M.txt',
             'glove25d.gz':
             'https://filedn.com/lCdtpv3siVybVynPcgXgnPm/corpus/pretrained/glove.twitter.27B.25d.txt.gz'
```

### Comparing `premium-23.5.22.20/premium/data/eda.py` & `premium-23.7.27.10/premium/data/eda.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/data/loader.py` & `premium-23.7.27.10/premium/data/loader.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/data/postprocess.py` & `premium-23.7.27.10/premium/data/postprocess.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/data/preprocess.py` & `premium-23.7.27.10/premium/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/data/utils.py` & `premium-23.7.27.10/premium/data/utils.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/demo.py` & `premium-23.7.27.10/premium/models/multi_classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import codefast as cf
 import tensorflow as tf
 import random
 
 
-class ClassifierDemos(object):
-    """ Some machine learning classifier demos for references.
+class MultiClassifierSet(object):
+    """ Binaray classifier demos.
     """
-
-    def tf_classifier(self,
-                      vocab_size: int = 10000,
-                      embedding_dim=64,
-                      max_length=1000):
+    def keras(self,
+              vocab_size: int = 10000,
+              embedding_dim=64,
+              max_length=1000):
         model = tf.keras.Sequential([
             tf.keras.layers.Embedding(vocab_size,
                                       embedding_dim,
                                       input_length=max_length),
             tf.keras.layers.Flatten(),
             tf.keras.layers.Dense(128, activation='relu'),
             tf.keras.layers.Dropout(0.5),
@@ -28,69 +27,68 @@
             metrics=[
                 tf.keras.metrics.CategoricalAccuracy(name='accuracy'),
                 #   tf.keras.metrics.Precision(name='precision'),
                 #   tf.keras.metrics.Recall(name='recall')
             ])
         return model
 
-    def catboost_classifier(self,
-                            loss_function: str = 'Logloss',
-                            use_gpu: bool = False) -> 'CatBoostClassifier':
+    def catboost(self,
+                 loss_function: str = 'MultiClass',
+                 use_gpu: bool = False) -> 'CatBoostClassifier':
         import catboost as cb
         return cb.CatBoostClassifier(iterations=1000,
                                      learning_rate=0.1,
                                      eval_metric='Accuracy',
                                      loss_function=loss_function,
                                      random_seed=random.randint(0, 0x3f3f3f3f),
                                      verbose=True,
                                      early_stopping_rounds=50,
                                      task_type="GPU" if use_gpu else "CPU",
                                      metric_period=50,
                                      devices='0:1')
 
-    def lightgbm_classifier(
-            self,
-            objective: str = 'binary',
-            metric: str = 'binary_logloss',
-            use_gpu: bool = False) -> 'LightGBMClassifier':
+    def lightgbm(self,
+                 objective: str = 'multiclass',
+                 metric: str = 'multi_logloss',
+                 use_gpu: bool = False) -> 'LightGBMClassifier':
         import lightgbm
         return lightgbm.LGBMClassifier(
             boosting_type='gbdt',
             learning_rate=0.1,
             n_estimators=300,
             objective=objective,  # 'binary', 'multiclass'
             metric=metric,  # 'binary_logloss', 'multi_logloss'
             random_state=42,
             verbose=1,
             n_jobs=-1,
             device='gpu' if use_gpu else 'cpu')
 
-    def xgboost_classifier(self,
-                           objective: str = 'binary:logistic',
-                           use_gpu: bool = False) -> 'XGBClassifier':
+    def xgboost(self,
+                objective: str = 'multi:softmax',
+                use_gpu: bool = False) -> 'XGBClassifier':
         import xgboost
         return xgboost.XGBClassifier(
             learning_rate=0.1,
             n_estimators=1000,
             # objective='multi:softmax', # 'binary:logistic', 'multi:softmax'
             objective=objective,
             random_state=42,
             verbose=True,
             tree_method='gpu_hist' if use_gpu else 'auto')
 
-    def extra_tree_classifier(self) -> 'ExtraTreeClassifier':
+    def extra_tree(self) -> 'ExtraTreeClassifier':
         from sklearn.ensemble import ExtraTreesClassifier
         return ExtraTreesClassifier(n_estimators=1500,
                                     max_depth=None,
                                     min_samples_split=2,
                                     n_jobs=-1,
                                     verbose=1,
                                     random_state=42)
 
-    def random_forest_classifier(self) -> 'RandomForestClassifier':
+    def random_forest(self) -> 'RandomForestClassifier':
         from sklearn.ensemble import RandomForestClassifier
         return RandomForestClassifier(n_estimators=500,
                                       max_depth=None,
                                       min_samples_split=2,
                                       random_state=42)
 
     def logistic_regression(self) -> 'LogisticRegression':
@@ -100,59 +98,48 @@
                                   solver='liblinear',
                                   multi_class='ovr')
 
     def ridge_regression(self) -> 'Ridge':
         from sklearn.linear_model import Ridge
         return Ridge(alpha=1.0, random_state=42, solver='auto')
 
-    def svm_classifier(self) -> 'SVC':
+    def svm(self) -> 'SVC':
         from sklearn.svm import SVC
         return SVC(C=1.0, kernel='rbf', random_state=42)
 
-    def decision_tree_classifier(self) -> 'DecisionTreeClassifier':
+    def decision_tree(self) -> 'DecisionTreeClassifier':
         from sklearn.tree import DecisionTreeClassifier
         return DecisionTreeClassifier(max_depth=None,
                                       min_samples_split=2,
                                       random_state=42)
 
-    def gradient_boosting_classifier(self) -> 'GradientBoostingClassifier':
+    def gradient_boosting(self) -> 'GradientBoostingClassifier':
         from sklearn.ensemble import GradientBoostingClassifier
         return GradientBoostingClassifier(n_estimators=500,
                                           learning_rate=0.1,
                                           max_depth=None,
                                           random_state=42)
 
-    def ada_boost_classifier(self) -> 'AdaBoostClassifier':
+    def ada_boost(self) -> 'AdaBoostClassifier':
         from sklearn.ensemble import AdaBoostClassifier
         return AdaBoostClassifier(n_estimators=500,
                                   learning_rate=0.1,
                                   random_state=42)
 
-    def voting_classifier(self) -> 'VotingClassifier':
+    def voting(self) -> 'VotingClassifier':
         from sklearn.ensemble import VotingClassifier
         return VotingClassifier(
             estimators=[
-                ('catboost', self.catboost_classifier()),
-                ('lightgbm', self.lightgbm_classifier()),
-                ('xgboost', self.xgboost_classifier()),
-                ('adaboost', self.ada_boost_classifier()),
+                ('catboost', self.catboost()),
+                ('lightgbm', self.lightgbm()),
+                ('xgboost', self.xgboost()),
+                ('adaboost', self.ada_boost()),
                 # ('extra_tree', self.extra_tree_classifier()),
                 # ('random_forest', self.random_forest_classifier()),
                 # ('logistic_regression', self.logistic_regression()),
                 ('ridge_regression', self.ridge_regression()),
                 # ('svm', self.svm_classifier()),
                 # ('gradient_boosting', self.gradient_boosting_classifier())
             ],
             voting='soft',
             verbose=True)
         # , weights=[1, 1, 1, 1, 1, 1, 1, 1, 1])
-
-
-classifiers = ClassifierDemos()
-
-
-class Demo(object):
-    def __init__(self) -> None:
-        self.classifiers = ClassifierDemos()
-
-
-demo_object = Demo()
```

### Comparing `premium-23.5.22.20/premium/experimental/cbow.py` & `premium-23.7.27.10/premium/experimental/cbow.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/experimental/eda.py` & `premium-23.7.27.10/premium/experimental/eda.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/experimental/kaggle.py` & `premium-23.7.27.10/premium/experimental/kaggle.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/experimental/myfasttext.py` & `premium-23.7.27.10/premium/experimental/myfasttext.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/experimental/ner.py` & `premium-23.7.27.10/premium/experimental/ner.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/experimental/nn_metric.py` & `premium-23.7.27.10/premium/experimental/nn_metric.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/experimental/segment_train.py` & `premium-23.7.27.10/premium/experimental/segment_train.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 #!/usr/bin/env python
 """ Train a Chinese sentence segment model.
 """
+from codefast.utils import timeit_decorator
 import codefast as cf
 from rich import print
 from typing import List, Union, Callable, Set, Dict, Tuple, Optional
 
-from premium.crf import CRF
+from premium.crf.crf import CRF, InputData, FeatureExtrator
 
 
 def reformat(X: List[List[str]]) -> List[List[Tuple]]:
     """ Convert a list of list of words to a list of list of (word, label) tuples.
     Args:
-        X: train corpus, a list of segmented sentences. E.g., [['我', '爱', '自由'], ['渴望', '民主']]
+        X: train corpus, a list of segmented sentences. 
+        E.g., [['我', '爱', '自由'], ['渴望', '民主']]
     Returns:
         A list of list of (word, label) tuples.
     """
     res = []
     for x in X:
         tmp = []
         for word in x:
@@ -46,52 +48,51 @@
     labels = [[p[1] for p in x] for x in X]
     # print(labels[:1])
     return X, labels
 
 
 def train(X_formatted, labels):
     # X_formatted, labels = get_data()
-    cli = CRF(X_formatted, labels)
-    cli.fit()
+    cli = CRF()
+    cli.fit(X_formatted, labels)
     cli.save_model('/tmp/lcut.model')
 
-
 def _token(text: str, tags: List[str]) -> List[str]:
     tuples, res = zip(text, tags), []
     for a, b in tuples:
         if b in ('S', 'B'):
             res.append(a)
         else:
             if not res:
                 res = ['']
             res[-1] += a
     return res
 
 
+@timeit_decorator()
 def test():
     model = CRF.load_model('/tmp/lcut.model')
     raw_texts = [
-        '可以做为通用中文语料，做预训练的语料或构建词向量，也可以用于构建知识问答。', '明天天气怎么样?',
-        '我爱自由，但是效果看起来很一般。', '全国代表大会高举邓小平理论伟大旗帜',
+        '可以做为通用中文语料，做预训练的语料或构建词向量，也可以用于构建知识问答。',
+        '明天天气怎么样?',
+        '我爱自由，但是效果看起来很一般。',
+        '全国代表大会高举邓小平理论伟大旗帜',
         '金额类实体识别使用的数据集来源于慧算账公司“询问价位”的事件结果，总计543条数据，大部分是手动标注数据，有一部分人工构造的数据。'
     ]
     cf.info('model loaded')
-    texts = [[(w, ) for w in text] for text in raw_texts]
-    feature_list = [model._sent2features(text) for text in texts]
-    tag_list = model.predict(feature_list)
-    for text, tags in zip(raw_texts, tag_list):
+    tags = model.predict(raw_texts)
+    for text, tags in zip(raw_texts, tags):
         print(_token(text, tags))
 
 
 xs = [[x for x in e.split(' ') if x]
       for e in cf.io.read('/tmp/msr_training.utf8')]
 # xs = cf.read('/tmp/corpus').top(20000).each(
 #     lambda x: [e for e in x.split(' ') if e]).filter(len).data
 xs = reformat(xs)
 print(xs[:10])
-# exit(0)
 # xs, labels = get_data()
 labels = [[_[1] for _ in x] for x in xs]
 print(xs[:10], labels[:10])
 train(xs, labels)
 
 test()
```

### Comparing `premium-23.5.22.20/premium/experimental/textnn.py` & `premium-23.7.27.10/premium/experimental/textnn.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/experimental/torch_crf.py` & `premium-23.7.27.10/premium/experimental/torch_crf.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/hmm.py` & `premium-23.7.27.10/premium/pytorch/tokenizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,188 +1,235 @@
-import math
-import pickle
-from collections import defaultdict
-from typing import List, Tuple
+#!/usr/bin/env python
+
+import os
+from abc import ABC, abstractmethod
+from typing import List, Union
 
 import codefast as cf
+import numpy as np
+import torch
 
 
-class HMM(object):
-    """ HMM Chinese word segmentation
+def seq_to_embedding(seq, to_ix):
+    '''
+    This is a good entry point for passing in different kinds of embeddings and
+    :param seq: sequence of words
+    :param to_ix: embedding lib
+    :return:
+    '''
+    idxs = [to_ix[w] for w in seq]
+    return torch.tensor(idxs, dtype=torch.long)
+
+
+def seqs_to_dictionary(training_data: list):
+    '''
+    Parameters
+    ----------
+    training_data: training data as a list of tuples.
+
+    Returns
+    -------
+    word_to_ix: a dictionary mapping words to indices
+    '''
+    # Prepare for padding; need to change count to 1 as well.
+    word_to_ix = {'<PAD>': 0}
+    count1 = 1
+
+    for sent, _ in training_data:
+        for word in sent:
+            if word not in word_to_ix:
+                word_to_ix[word] = count1
+                count1 += 1
+
+    return word_to_ix
+
+
+# Note: we are stealing this from tf.keras.preprocessing.sequence, to avoid having an additional
+# dependency for tensorflow.
+# It's perfectly fine if you want to install tf and call the function directly from there.
+
+
+def pad_sequences(sequences,
+                  maxlen=None,
+                  dtype='int32',
+                  padding='pre',
+                  truncating='pre',
+                  value=0.):
+    """Pads sequences to the same length.
+    This function transforms a list of
+    `num_samples` sequences (lists of integers)
+    into a 2D Numpy array of shape `(num_samples, num_timesteps)`.
+    `num_timesteps` is either the `maxlen` argument if provided,
+    or the length of the longest sequence otherwise.
+    Sequences that are shorter than `num_timesteps`
+    are padded with `value` at the end.
+    Sequences longer than `num_timesteps` are truncated
+    so that they fit the desired length.
+    The position where padding or truncation happens is determined by
+    the arguments `padding` and `truncating`, respectively.
+    Pre-padding is the default.
+    Arguments:
+        sequences: List of lists, where each element is a sequence.
+        maxlen: Int, maximum length of all sequences.
+        dtype: Type of the output sequences.
+        padding: String, 'pre' or 'post':
+            pad either before or after each sequence.
+        truncating: String, 'pre' or 'post':
+            remove values from sequences larger than
+            `maxlen`, either at the beginning or at the end of the sequences.
+        value: Float, padding value.
+    Returns:
+        x: Numpy array with shape `(len(sequences), maxlen)`
+    Raises:
+        ValueError: In case of invalid values for `truncating` or `padding`,
+            or in case of invalid shape for a `sequences` entry.
     """
+    if not hasattr(sequences, '__len__'):
+        raise ValueError('`sequences` must be iterable.')
+    lengths = []
+    for x in sequences:
+        if not hasattr(x, '__len__'):
+            raise ValueError('`sequences` must be a list of iterables. '
+                             'Found non-iterable: ' + str(x))
+        lengths.append(len(x))
+
+    num_samples = len(sequences)
+    if maxlen is None:
+        maxlen = np.max(lengths)
+
+    # take the sample shape from the first non empty sequence
+    # checking for consistency in the main loop below.
+    sample_shape = tuple()
+    for s in sequences:
+        if len(s) > 0:  # pylint: disable=g-explicit-length-test
+            sample_shape = np.asarray(s).shape[1:]
+            break
+
+    x = (np.ones((num_samples, maxlen) + sample_shape) * value).astype(dtype)
+    for idx, s in enumerate(sequences):
+        if not len(s):  # pylint: disable=g-explicit-length-test
+            continue  # empty list/array was found
+        if truncating == 'pre':
+            trunc = s[-maxlen:]  # pylint: disable=invalid-unary-operand-type
+        elif truncating == 'post':
+            trunc = s[:maxlen]
+        else:
+            raise ValueError('Truncating type "%s" not understood' %
+                             truncating)
+
+        # check `trunc` has expected shape
+        trunc = np.asarray(trunc, dtype=dtype)
+        if trunc.shape[1:] != sample_shape:
+            raise ValueError('Shape of sample %s of sequence at position %s '
+                             'is different from expected shape %s' %
+                             (trunc.shape[1:], idx, sample_shape))
+
+        if padding == 'post':
+            x[idx, :len(trunc)] = trunc
+        elif padding == 'pre':
+            x[idx, -len(trunc):] = trunc
+        else:
+            raise ValueError('Padding type "%s" not understood' % padding)
+    return x
+
+
+class Vectorizer(ABC):
+
+    def __init__(self, *args, **kwargs):
+        pass
+
+    @abstractmethod
+    def fit(self, texts: List[str]):
+        pass
+
+    @abstractmethod
+    def transform(self, texts: List[str]):
+        pass
+
+    @abstractmethod
+    def fit_transform(self, texts: List[str]):
+        pass
+
+    @abstractmethod
+    def inverse_transform(self, tokens: List[int]):
+        pass
+
+    @abstractmethod
+    def save(self, path: str):
+        pass
+
+    @abstractmethod
+    def load(self, path: str):
+        pass
+
+
+class VocabVectorizer(object):
+
+    def __init__(self, max_length, padding, tokenizer):
+        """
+        padding is either `pre` or `post`
+        """
+        self.vocab = {}
+        self.index2token = {}
+        self.max_length = max_length
+        self.padding = padding
+        self.tokenizer = tokenizer
+
+    def __len__(self):
+        return len(self.vocab)
+
+    def pad_sequence(self, vector: List[int]):
+        vector = vector[:self.max_length]
+        if len(vector) >= self.max_length:
+            return vector
+        if self.padding == 'pre':
+            return [0 for _ in range(self.max_length - len(vector))] + vector
+        else:
+            return vector + [0 for _ in range(self.max_length - len(vector))]
+
+    def fit(self, texts: List[List[str]]):
+        assert isinstance(self.tokenizer(texts[0]),
+                          list), 'tokenizer must return a list'
+        token_idx = 1
+        for t in texts:
+            for token in self.tokenizer(t):
+                if token not in self.vocab:
+                    self.vocab[token] = token_idx
+                    self.index2token[token_idx] = token
+                    token_idx += 1
+
+    def transform(
+        self,
+        texts: Union[str, List[str]],
+    ) -> Union[List[List[int]], np.ndarray]:
+        if isinstance(texts, str):
+            texts = [texts]
+
+        vectors = []
+        for x in texts:
+            x = x[:self.max_length]
+            vector = [self.vocab.get(token, 0) for token in self.tokenizer(x)]
+            if self.padding is not None:
+                vector = self.pad_sequence(vector)
+            vectors.append(vector)
+        return vectors
+
+    def fit_transform(self, texts: Union[str, List[str]]) -> List[List[int]]:
+        if isinstance(texts, str):
+            texts = [texts]
+        return self.fit(texts).transform(texts)
+
+    def inverse_transform(self, tokens: List[int]) -> List[str]:
+        return [self.index2token.get(idx, '') for idx in tokens]
+
+    def save(self, path: str):
+        cf.js.write(self.vocab, os.path.join(path, 'vocab.json'))
+        cf.js.write(self.index2token, os.path.join(path, 'index.json'))
+
+    def load(self, path: str):
+        vocab_path = os.path.join(path, 'vocab.json')
+        index_path = os.path.join(path, 'index.json')
+        self.vocab = cf.js(vocab_path)
+        self.index2token = cf.js(index_path)
 
-    def __init__(self):
-        cur_dir = cf.io.pwd()
-        self.TRAIN_CORPUS = f'{cur_dir}/data/msr_training.utf8'
-        self.emit_pickle = f'{cur_dir}/data/emit_p.pickle'
-        self.trans_pickle = f'{cur_dir}/data/trans.pickle'
-        self.punctuations = set('，‘’“”。！？：（）、')
-        self.MIN_FLOAT = -1e10
-        self.emission = None
-        self.transition = None
-
-    def train(self) -> Tuple[dict, list]:
-        ''' train HMM segment model from corpus '''
-        if self.emission and self.transition:     # to speedup I/O
-            return self.emission, self.transition
-
-        if cf.io.exists(self.emit_pickle) and cf.io.exists(self.trans_pickle):
-            emit_p = pickle.load(open(self.emit_pickle, 'rb'))
-            trans = pickle.load(open(self.trans_pickle, 'rb'))
-            self.emission, self.transition = emit_p, trans
-            return emit_p, trans
-
-        emit_p = defaultdict(int)
-        ci = defaultdict(int)
-        # b->0 m->1 e->2 s->3
-        trans = [[0] * 4 for _ in range(4)]
-
-        def update_trans(i, j):
-            if i < 0:
-                return j
-            trans[i][j] += 1
-            return j
-
-        with open(self.TRAIN_CORPUS, 'r') as f:
-            for ln in f.readlines():
-                pre_symbol = -1
-                _words = (e for e in ln.split(' ') if e)
-                for cur in _words:
-                    if cur in self.punctuations:
-                        pre_symbol = -1
-                    else:
-                        if len(cur) == 1:
-                            emit_p[(cur, 'S')] += 1
-                            ci['S'] += 1
-                            pre_symbol = update_trans(pre_symbol, 3)
-                        else:
-                            for i, c in enumerate(cur):
-                                if i == 0:
-                                    emit_p[(c, 'B')] += 1
-                                    ci['B'] += 1
-                                    pre_symbol = update_trans(pre_symbol, 0)
-                                elif i == len(cur) - 1:
-                                    emit_p[(c, 'E')] += 1
-                                    ci['E'] += 1
-                                    pre_symbol = update_trans(pre_symbol, 2)
-                                else:
-                                    ci['M'] += 1
-                                    emit_p[(c, 'M')] += 1
-                                    pre_symbol = update_trans(pre_symbol, 1)
-        cf.info('counting pairs completed.')
-
-        for i, t in enumerate(trans):     # normalization
-            trans[i] = [
-                math.log(e / sum(t)) if e > 0 else self.MIN_FLOAT for e in t
-            ]
-
-        for key, v in emit_p.items():
-            emit_p[key] = math.log(v / ci[key[1]])
-
-        with open(self.emit_pickle, 'wb') as f:
-            pickle.dump(emit_p, f)
-
-        with open(self.trans_pickle, 'wb') as f:
-            cf.info('tran matrix', trans)
-            pickle.dump(trans, f)
-
-        cf.info('training completed.')
-        return emit_p, trans
-
-    def calculate_trans(self, emit_p: dict, ci: dict, obs: str,
-                        state: str) -> float:
-        return (1 + emit_p.get((obs, state), 0)) / ci.get(state, 1)
-
-    def viterbi(self, text: str, emit_p: dict, trans_p: dict) -> List[str]:
-        ''' a DP method to locate the word segment scheme with maximum probability 
-        for a given Chinese sentence.
-        :param text: str, observed sequence, e.g., '人性的枷锁'
-        :param emit_p: dict, emission probability matrix, e.g., emit_p[('一', 'B')] = 0.0233
-        :param trans_p: dict, transition probability matrix, e.g., trans_p['B']['M'] = 0.123
-        :return: list[str], word segments, e.g., ['人性', '的' ,'枷锁']
-        '''
-        if not text:
-            return []
-        state_index = dict(zip('BMES', range(4)))
-        cache = {}
-
-        for i, c in enumerate(text):
-            if i == 0:
-                for s in 'BS':
-                    # this initial prob is customizable
-                    cache[s] = (-0.5, s)
-                cache['E'] = (self.MIN_FLOAT, 'E')
-                cache['M'] = (self.MIN_FLOAT, 'M')
-            else:
-                cccopy = cache.copy()
-                for s in 'BMES':
-                    max_prob, prev_seq = float('-inf'), ''
-                    for prev_state, v in cccopy.items():
-                        prev_index, cur_index = state_index[
-                            prev_state], state_index[s]
-
-                        # not '*' but '+'
-                        new_prob = v[0] + trans_p[prev_index][
-                            cur_index] + emit_p.get((c, s), self.MIN_FLOAT)
-                        if new_prob > max_prob:
-                            max_prob = new_prob
-                            prev_seq = v[1]
-                    cache[s] = (max_prob, prev_seq + '->' + s)
-
-        # assume a sentence ends with either 'E' or 'S'
-        # print(cache)
-        seq = cache['E'][1] if cache['E'][0] > cache['S'][0] else cache['S'][1]
-        return self._cut(text, seq)
-
-    def _cut(self, text: str, seq: str) -> List[str]:
-        ''' seperate a sequence by word lexeme.
-        e.g., input ('人性的枷锁', 'B->E->S->B->E'), output ['人性','的','枷锁']
-        '''
-        res = []
-        # print(seq, text)
-        # print(len(text))
-        for a, b in zip(text, seq.split('->')):
-            if (b == 'B' or b == 'S'):
-                res.append('')
-            res[-1] += a
-            # print(res)
-
-        return res
-
-    def segment(self, text: str) -> List[str]:
-        emit_p, trans = self.train()
-        res, prev_text = [], ''
-        for i, c in enumerate(text):
-            if c in self.punctuations:
-                res += self.viterbi(prev_text, emit_p, trans)
-                res.append(c)
-                prev_text = ''
-            else:
-                prev_text += c
-
-        if prev_text:
-            res += self.viterbi(prev_text, emit_p, trans)
-        return res
-
-
-if __name__ == '__main__':
-    cur_dir = cf.io.dirname()
-    cf.io.rm(f'{cur_dir}/data/emit_p.pickle')
-    texts = [
-        '看了你的信，我被你信中流露出的凄苦、迷惘以及热切求助的情绪触动了。', '这是一种基于统计的分词方案', '这位先生您手机欠费了',
-        '还有没有更快的方法', '买水果然后来世博园最后去世博会', '欢迎新老师生前来就餐', '北京大学生前来应聘', '今天天气不错哦',
-        '就问你服不服', '我们不只在和你们一家公司对接', '结婚的和尚未结婚的都沿海边去了', '这也许就是一代人的命运吧',
-        '改判被告人死刑立即执行', '检察院鲍绍坤检察长', '腾讯和阿里都在新零售大举布局', '人性的枷锁'
-    ]
-
-    texts += [
-        '好的，现在我们尝试一下带标点符号的分词效果。', '中华人民共和国不可分割，坚决捍卫我国领土。',
-        '英国白金汉宫发表声明，菲利浦亲王去世，享年九十九岁。', '扬帆远东做与中国合作的先行', '不是说伊尔新一轮裁员了。',
-        '滴滴遭调查后，投资人认为中国科技业将强化数据安全合规。', '小明硕士毕业于中国科学院计算所，后在日本京都大学深造',
-        '可以做为通用中文语料，做预训练的语料或构建词向量，也可以用于构建知识问答。', '明天天气怎么样?',
-        '我爱自由，但是效果看起来很一般。', '全国代表大会高举邓小平理论伟大旗帜',
-        '金额类实体识别使用的数据集来源于慧算账公司“询问价位”的事件结果，总计543条数据，大部分是手动标注数据，有一部分人工构造的数据。'
-
-    ]
-    for text in texts:
-        ret = ' '.join(HMM().segment(text))
-        print(ret)
+    def __call__(self, texts: Union[str, List[str]]) -> List[int]:
+        return self.transform(texts)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `premium-23.5.22.20/premium/lightning/callbacks.py` & `premium-23.7.27.10/premium/lightning/callbacks.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         self.metrics = []
 
     @abstractmethod
     def on_validation_epoch_end(self, trainer, pl_module):
         ...
 
     def on_train_end(self, trainer, pl_module):
-        print(self.metrics[-1])
+        if self.metrics:
+            print(self.metrics[-1])
 
 
 class ModelSaveCallback(pl.Callback):
     """ save best model 
     """
 
     def __init__(self, save_path: str):
@@ -54,19 +55,46 @@
         if 'val_loss' in metrics.keys():
             val_loss = metrics['val_loss'].item()
             if val_loss < self.best_loss:
                 self.best_loss = val_loss
                 trainer.save_checkpoint(self.save_path)
 
 
+class PretrainedSaveCallback(pl.Callback):
+    """ save best model 
+    """
+
+    def __init__(self, save_path: str):
+        self.save_path = save_path
+        self.best_loss = float('inf')
+
+    def on_validation_epoch_end(self, trainer, pl_module):
+        metrics = trainer.callback_metrics
+        if 'val_loss' in metrics.keys():
+            val_loss = metrics['val_loss'].item()
+            if val_loss < self.best_loss:
+                self.best_loss = val_loss
+                trainer.model.pretrained.save_pretrained(self.save_path)
+
+
+
 class AccLossCallback(ModelMetricsCallback):
 
     def on_validation_epoch_end(self, trainer, pl_module):
+        """
+        usage: 
+        def validation_step(self, batch, batch_idx):
+            ...
+            metric = {'val_loss': loss, 'val_acc': accuracy}
+            self.log_dict(metric)
+        """
         metrics = ModelMetrics(
             epoch=trainer.current_epoch,
-            train_loss=trainer.callback_metrics.get('train_loss', -1),
-            train_acc=trainer.callback_metrics.get('train_acc', -1),
-            val_loss=trainer.callback_metrics.get('val_loss', -1),
-            val_acc=trainer.callback_metrics.get('val_acc', -1),
         )
-        cf.info(metrics)
+        import torch 
+        for k, v in trainer.callback_metrics.items():
+            _v = v.cpu()
+            if isinstance(_v, torch.Tensor):
+                _v = _v.item()
+            metrics.kwargs[k] = _v
+        print(metrics)
         self.metrics.append(metrics)
```

### Comparing `premium-23.5.22.20/premium/localdata/27.mp3` & `premium-23.7.27.10/premium/localdata/27.mp3`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/localdata/27.wav` & `premium-23.7.27.10/premium/localdata/27.wav`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/localdata/cn_stopwords.txt` & `premium-23.7.27.10/premium/localdata/cn_stopwords.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/localdata/dict.txt` & `premium-23.7.27.10/premium/localdata/dict.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/localdata/emit_p.pickle` & `premium-23.7.27.10/premium/localdata/emit_p.pickle`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/localdata/en_stopwords.txt` & `premium-23.7.27.10/premium/localdata/en_stopwords.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/localdata/puredict.txt` & `premium-23.7.27.10/premium/localdata/puredict.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/localdata/soledad.txt` & `premium-23.7.27.10/premium/localdata/soledad.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/localdata/xinhua.txt` & `premium-23.7.27.10/premium/localdata/xinhua.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/measure.py` & `premium-23.7.27.10/premium/measure.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/metrics/__init__.py` & `premium-23.7.27.10/premium/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/metrics/distance.py` & `premium-23.7.27.10/premium/metrics/distance.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/metrics/metrix.py` & `premium-23.7.27.10/premium/metrics/metrix.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/base.py` & `premium-23.7.27.10/premium/models/base.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/benchmark.py` & `premium-23.7.27.10/premium/models/benchmark.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/bert.py` & `premium-23.7.27.10/premium/models/bert.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/binary_classifiers.py` & `premium-23.7.27.10/premium/models/binary_classifiers.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/clf.py` & `premium-23.7.27.10/premium/models/clf.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/lgb.py` & `premium-23.7.27.10/premium/models/lgb.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/model_config.py` & `premium-23.7.27.10/premium/models/model_config.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/nn.py` & `premium-23.7.27.10/premium/models/nn.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/optuna.py` & `premium-23.7.27.10/premium/models/optuna.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/regressor.py` & `premium-23.7.27.10/premium/models/regressor.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/tensorflow/binary_classifier.py` & `premium-23.7.27.10/premium/models/tensorflow/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/touchstone.py` & `premium-23.7.27.10/premium/models/touchstone.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/models/xgb.py` & `premium-23.7.27.10/premium/models/xgb.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/nlp/metrics.py` & `premium-23.7.27.10/premium/nlp/metrics.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/nlp/net.py` & `premium-23.7.27.10/premium/nlp/net.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/nlp/nlp.py` & `premium-23.7.27.10/premium/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/pytorch/__init__.py` & `premium-23.7.27.10/premium/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/pytorch/data.py` & `premium-23.7.27.10/premium/pytorch/data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,93 @@
 from abc import ABC, abstractmethod
 from typing import Callable
 
 import pandas as pd
 from sklearn.model_selection import train_test_split
-from torch.utils.data import Dataset
+from torch.utils.data import DataLoader, Dataset
+
 
 class BaseDataset(ABC):
+
     def __init__(self) -> None:
         super().__init__()
 
     @abstractmethod
     def __len__(self):
         pass
 
     @abstractmethod
     def __getitem__(self):
         pass
 
 
 class TextDataset(BaseDataset):
-    def __init__(self, df: pd.DataFrame, tokenizer: Callable):
+
+    def __init__(self,
+                 csv_file: str = None,
+                 df: pd.DataFrame = None,
+                 tokenizer: Callable = None):
+        """ if df is not None, csv_file is ignored 
+        otherwise, csv_file is used to load the data
+        """
         super().__init__()
-        self.df = df
+        if csv_file is not None:
+            self.df = pd.read_csv(csv_file)
+        if df is not None:
+            self.df = df
         self.tokenizer = tokenizer
 
     def __len__(self):
         return len(self.df)
 
     def __getitem__(self, idx):
         row = self.df.iloc[idx]
         text = row['text']
         label = row['label']
-        tokens = self.tokenizer(text)[0]
-        return {'text': tokens, 'label': label}
+        if self.tokenizer is None:
+            return {'text': text, 'label': label}
+        else:
+            return {'text': self.tokenizer(text)[0], 'label': label}
+
+    @property
+    def text(self):
+        return self.df['text']
+
+    @property
+    def label(self):
+        return self.df['label']
 
 
 class TrainData(Dataset):
 
     def __init__(self, X_data, y_data):
         self.X_data = X_data
         self.y_data = y_data
 
     def __getitem__(self, index):
         return self.X_data[index], self.y_data[index]
 
     def __len__(self):
         return len(self.X_data)
 
+
 def train_test_val_split(df, test_size=0.2, val_size=0.2, random_state=42):
     X, P = train_test_split(df, test_size=test_size, random_state=random_state)
     V, T = train_test_split(P, test_size=val_size, random_state=random_state)
     return X, V, T
 
 
 class AbstractLoader(ABC):
+
     def __init__(self) -> None:
         super().__init__()
 
 
-from torch.utils.data import DataLoader
-
-
 class TextLoader(AbstractLoader):
+
     def __init__(self, dataset, **kargs):
         self._DataSet = dataset
         self.kargs = kargs
 
     def __call__(self, df: pd.DataFrame, **kargs) -> DataLoader:
         self.kargs.update(kargs)
         return DataLoader(self._DataSet(df), **self.kargs)
-
-
```

### Comparing `premium-23.5.22.20/premium/pytorch/trainer.py` & `premium-23.7.27.10/premium/pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/segment.py` & `premium-23.7.27.10/premium/segment.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/text_feature/bm25.py` & `premium-23.7.27.10/premium/text_feature/bm25.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
 import math
-from typing import Any, Dict, List, Optional, Set, Tuple, Union
+from typing import List, Tuple
 
 
 class BM25(object):
     """
     Best Match 25.
 
     Parameters
@@ -36,14 +36,15 @@
 
     corpus_size_ : int
         Number of documents in the corpus.
 
     avg_doc_len_ : float
         Average number of terms for documents in the corpus.
     """
+
     def __init__(self, k1=1.5, b=0.75):
         self.b = b
         self.k1 = k1
 
     def fit(self, corpus):
         """
         Fit the various statistics that are required to calculate BM25 ranking
@@ -113,14 +114,37 @@
             denominator = freq + self.k1 * (
                 1 - self.b + self.b * doc_len / self.avg_doc_len_)
             score += (numerator / denominator)
 
         return score
 
 
+class CnBm25(BM25):
+
+    def __init__(self, k1=1.5, b=0.75, tokenizer=None):
+        super().__init__(k1, b)
+        self.tokenizer = tokenizer
+
+    def fit_sentences(self, corpus: List[List[str]]):
+        """ Given a list of sentences, fit the model.
+        """
+        self.raw_corpus = corpus
+        corpus = list(map(self.tokenizer, corpus))
+        self.fit(corpus)
+
+    def query_sentence(self,
+                       query: List[str],
+                       top_k: int = 10) -> List[Tuple[float, List[str]]]:
+        """ Given a query, return the top k sentences.
+        """
+        query = self.tokenizer(query)
+        scores = self.search(query)
+        return sorted(zip(scores, self.raw_corpus), reverse=True)[:top_k]
+
+
 if __name__ == '__main__':
     # we'll generate some fake texts to experiment with
     corpus = [
         'Human machine interface for lab abc computer applications',
         'A survey of user opinion of computer system response time',
         'The EPS user interface management system',
         'System and human system engineering testing of EPS',
```

### Comparing `premium-23.5.22.20/premium/text_feature/sif.py` & `premium-23.7.27.10/premium/text_feature/sif.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/utils/__init__.py` & `premium-23.7.27.10/premium/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/premium/utils/decorators.py` & `premium-23.7.27.10/premium/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.22.20/setup.py` & `premium-23.7.27.10/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+import codefast as cf
 import setuptools
-import codefast as cf 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="premium",
     version=cf.generate_version(),
@@ -12,23 +12,24 @@
     description="Python AI toolkits",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/",
     packages=setuptools.find_packages(),
     include_package_data=True,
     package_data={
-        # And include any *.msg files found in the "hello" package, too:
+     # And include any *.msg files found in the "hello" package, too:
         "premium": [
             'localdata/*.txt', 'localdata/*.pickle', 'localdata/*.mp3',
             'localdata/*.wav'
         ],
     },
     install_requires=[
-        'smart-open', 'optuna', 'jieba', 'matplotlib', 'scikit-learn', 
-        'codefast', 'jiwer', 'pandas', 'numpy'
+        'smart-open', 'optuna', 'jieba', 'matplotlib', 'scikit-learn',
+        'transformers', 'fasttext', 'classifiercluster', 'codefast', 'jiwer',
+        'pandas', 'numpy', 'pytorch-lightning==1.7.7'
     ],
     entry_points={
         'console_scripts': ['demo=premium.demo:entry', 'zz=premium.zz:main'],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

