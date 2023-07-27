# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.28.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.28.tar", last modified: Mon Jul 24 08:53:04 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.29.tar", last modified: Thu Jul 27 04:37:01 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.28.tar` & `bytetrade-recommend-model-sdk-0.0.29.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-24 08:53:04.000000 bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-24 08:53:04.000000 bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-24 08:53:04.000000 bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      155 2023-07-24 08:53:04.000000 bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-24 08:53:04.000000 bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3875 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/bert_embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/config/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/config/content_similar_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/config/mind_base_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/eval/__init_.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/eval/eval_operation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/exp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/exp/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/experiment_enum.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.692969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14888 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/model/content_similar_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23340 2023-07-21 09:10:35.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4976 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/recommend_common_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/recommend_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5148 2023-07-21 12:55:09.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37549 2023-07-24 08:47:31.000000 bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-24 08:53:04.696969 bytetrade-recommend-model-sdk-0.0.28/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1125 2023-07-24 08:51:25.000000 bytetrade-recommend-model-sdk-0.0.28/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.558781 bytetrade-recommend-model-sdk-0.0.29/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.29/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-27 04:37:01.558781 bytetrade-recommend-model-sdk-0.0.29/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.29/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.554781 bytetrade-recommend-model-sdk-0.0.29/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-07-27 04:37:01.000000 bytetrade-recommend-model-sdk-0.0.29/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2178 2023-07-27 04:37:01.000000 bytetrade-recommend-model-sdk-0.0.29/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-27 04:37:01.000000 bytetrade-recommend-model-sdk-0.0.29/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      155 2023-07-27 04:37:01.000000 bytetrade-recommend-model-sdk-0.0.29/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-07-27 04:37:01.000000 bytetrade-recommend-model-sdk-0.0.29/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.554781 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.554781 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3875 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/embeddings/bert_embedding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.554781 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.554781 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/config/content_similar_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      396 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/config/dnn_click_predictor_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/config/mind_base_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.554781 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/dataset/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/dataset/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4244 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1769 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2719 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.554781 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/eval/__init_.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/eval/eval_operation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11667 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.554781 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/exp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/exp/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11826 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/experiment_enum.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.554781 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14888 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/model/content_similar_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2330 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.554781 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24560 2023-07-27 04:06:42.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.558781 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/recommend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/recommend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4976 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/recommend/recommend_common_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/recommend/recommend_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/recommend/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.558781 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2508 2023-07-16 23:12:22.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-27 04:37:01.558781 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5148 2023-07-21 12:55:09.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-07-03 08:24:46.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37817 2023-07-27 04:30:59.000000 bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-27 04:37:01.558781 bytetrade-recommend-model-sdk-0.0.29/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1125 2023-07-27 04:35:14.000000 bytetrade-recommend-model-sdk-0.0.29/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.28/README.md` & `bytetrade-recommend-model-sdk-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt` & `bytetrade-recommend-model-sdk-0.0.29/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/bert_embedding.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/embeddings/bert_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/embeddings/word2vec_embedding.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/embeddings/word2vec_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/config/content_similar_config.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/config/content_similar_config.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/dataset/mind_base_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_parsed_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/eval/eval_operation.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/eval/eval_operation.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/exp/mind_dnn_click_predictor_train_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/model/content_similar_model.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/model/content_similar_model.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/mind_sdk/model/dnn_click_predictor.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='embedding.proto',
   package='',
   syntax='proto3',
   serialized_options=None,
-  serialized_pb=_b('\n\x0f\x65mbedding.proto\"\xb5\x01\n\x07\x41rticle\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tfull_text\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\x12\x12\x14\n\x0cpublished_at\x18\x04 \x01(\x12\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x06 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x07 \x01(\t\x12\x0f\n\x07\x66\x65\x65\x64_id\x18\x08 \x01(\x04\x12\x0c\n\x04hash\x18\t \x01(\t\x12\x11\n\timage_url\x18\n \x01(\t\"\x83\x01\n\tEmbedding\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x12\n\nembeddings\x18\x04 \x03(\x02\x12*\n\x10subdocembeddings\x18\x05 \x03(\x0b\x32\x10.SubdocEmbedding\";\n\x0fSubdocEmbedding\x12\x14\n\x0csubdoc_index\x18\x01 \x01(\r\x12\x12\n\nembeddings\x18\x02 \x03(\x02\"K\n\rLatestPackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\x12\x1e\n\nembeddings\x18\x02 \x03(\x0b\x32\n.Embedding\",\n\x0e\x41rticlePackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\"2\n\x10\x45mbeddingPakcage\x12\x1e\n\nembeddings\x18\x01 \x03(\x0b\x32\n.Embedding\"\xc1\x01\n\x04\x46\x65\x65\x64\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08\x66\x65\x65\x64_url\x18\x02 \x01(\t\x12\x10\n\x08site_url\x18\x03 \x01(\t\x12\r\n\x05title\x18\x04 \x01(\t\x12\x13\n\x0b\x63\x61tegory_id\x18\x05 \x01(\x03\x12\x16\n\x0e\x63\x61tegory_title\x18\x06 \x01(\t\x12\x0f\n\x07icon_id\x18\x07 \x01(\x03\x12\x11\n\ticon_type\x18\x08 \x01(\t\x12\x14\n\x0cicon_content\x18\t \x01(\x0c\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\"#\n\x0b\x46\x65\x65\x64Package\x12\x14\n\x05\x66\x65\x65\x64s\x18\x01 \x03(\x0b\x32\x05.Feed\"A\n\x11KeywordSortedInfo\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\r\n\x05\x66\x65\x65\x64s\x18\x02 \x03(\x03\x12\x0f\n\x07keyword\x18\x03 \x01(\t\"M\n\x18KeywordSortedInfoPackage\x12\x31\n\x15keyword_sortinfo_list\x18\x01 \x03(\x0b\x32\x12.KeywordSortedInfob\x06proto3')
+  serialized_pb=_b('\n\x0f\x65mbedding.proto\"\xf5\x01\n\x07\x41rticle\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tfull_text\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\x12\x12\x14\n\x0cpublished_at\x18\x04 \x01(\x12\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x06 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x07 \x01(\t\x12\x0f\n\x07\x66\x65\x65\x64_id\x18\x08 \x01(\x04\x12\x0c\n\x04hash\x18\t \x01(\t\x12\x11\n\timage_url\x18\n \x01(\t\x12\x14\n\x0ckeyword_list\x18\x0b \x03(\t\x12\x10\n\x08\x63loud_id\x18\x0c \x01(\x04\x12\x16\n\x0emajor_language\x18\r \x01(\t\"\x83\x01\n\tEmbedding\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x15\n\rmodel_version\x18\x03 \x01(\t\x12\x12\n\nembeddings\x18\x04 \x03(\x02\x12*\n\x10subdocembeddings\x18\x05 \x03(\x0b\x32\x10.SubdocEmbedding\";\n\x0fSubdocEmbedding\x12\x14\n\x0csubdoc_index\x18\x01 \x01(\r\x12\x12\n\nembeddings\x18\x02 \x03(\x02\"K\n\rLatestPackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\x12\x1e\n\nembeddings\x18\x02 \x03(\x0b\x32\n.Embedding\",\n\x0e\x41rticlePackage\x12\x1a\n\x08\x61rticles\x18\x01 \x03(\x0b\x32\x08.Article\"2\n\x10\x45mbeddingPakcage\x12\x1e\n\nembeddings\x18\x01 \x03(\x0b\x32\n.Embedding\"\xc1\x01\n\x04\x46\x65\x65\x64\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08\x66\x65\x65\x64_url\x18\x02 \x01(\t\x12\x10\n\x08site_url\x18\x03 \x01(\t\x12\r\n\x05title\x18\x04 \x01(\t\x12\x13\n\x0b\x63\x61tegory_id\x18\x05 \x01(\x03\x12\x16\n\x0e\x63\x61tegory_title\x18\x06 \x01(\t\x12\x0f\n\x07icon_id\x18\x07 \x01(\x03\x12\x11\n\ticon_type\x18\x08 \x01(\t\x12\x14\n\x0cicon_content\x18\t \x01(\x0c\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\"#\n\x0b\x46\x65\x65\x64Package\x12\x14\n\x05\x66\x65\x65\x64s\x18\x01 \x03(\x0b\x32\x05.Feed\"A\n\x11KeywordSortedInfo\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\r\n\x05\x66\x65\x65\x64s\x18\x02 \x03(\x03\x12\x0f\n\x07keyword\x18\x03 \x01(\t\"M\n\x18KeywordSortedInfoPackage\x12\x31\n\x15keyword_sortinfo_list\x18\x01 \x03(\x0b\x32\x12.KeywordSortedInfob\x06proto3')
 )
 
 
 
 
 _ARTICLE = _descriptor.Descriptor(
   name='Article',
@@ -98,28 +98,49 @@
     _descriptor.FieldDescriptor(
       name='image_url', full_name='Article.image_url', index=9,
       number=10, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='keyword_list', full_name='Article.keyword_list', index=10,
+      number=11, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='cloud_id', full_name='Article.cloud_id', index=11,
+      number=12, type=4, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='major_language', full_name='Article.major_language', index=12,
+      number=13, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=20,
-  serialized_end=201,
+  serialized_end=265,
 )
 
 
 _EMBEDDING = _descriptor.Descriptor(
   name='Embedding',
   full_name='Embedding',
   filename=None,
@@ -169,16 +190,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=204,
-  serialized_end=335,
+  serialized_start=268,
+  serialized_end=399,
 )
 
 
 _SUBDOCEMBEDDING = _descriptor.Descriptor(
   name='SubdocEmbedding',
   full_name='SubdocEmbedding',
   filename=None,
@@ -207,16 +228,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=337,
-  serialized_end=396,
+  serialized_start=401,
+  serialized_end=460,
 )
 
 
 _LATESTPACKAGE = _descriptor.Descriptor(
   name='LatestPackage',
   full_name='LatestPackage',
   filename=None,
@@ -245,16 +266,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=398,
-  serialized_end=473,
+  serialized_start=462,
+  serialized_end=537,
 )
 
 
 _ARTICLEPACKAGE = _descriptor.Descriptor(
   name='ArticlePackage',
   full_name='ArticlePackage',
   filename=None,
@@ -276,16 +297,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=475,
-  serialized_end=519,
+  serialized_start=539,
+  serialized_end=583,
 )
 
 
 _EMBEDDINGPAKCAGE = _descriptor.Descriptor(
   name='EmbeddingPakcage',
   full_name='EmbeddingPakcage',
   filename=None,
@@ -307,16 +328,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=521,
-  serialized_end=571,
+  serialized_start=585,
+  serialized_end=635,
 )
 
 
 _FEED = _descriptor.Descriptor(
   name='Feed',
   full_name='Feed',
   filename=None,
@@ -401,16 +422,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=574,
-  serialized_end=767,
+  serialized_start=638,
+  serialized_end=831,
 )
 
 
 _FEEDPACKAGE = _descriptor.Descriptor(
   name='FeedPackage',
   full_name='FeedPackage',
   filename=None,
@@ -432,16 +453,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=769,
-  serialized_end=804,
+  serialized_start=833,
+  serialized_end=868,
 )
 
 
 _KEYWORDSORTEDINFO = _descriptor.Descriptor(
   name='KeywordSortedInfo',
   full_name='KeywordSortedInfo',
   filename=None,
@@ -477,16 +498,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=806,
-  serialized_end=871,
+  serialized_start=870,
+  serialized_end=935,
 )
 
 
 _KEYWORDSORTEDINFOPACKAGE = _descriptor.Descriptor(
   name='KeywordSortedInfoPackage',
   full_name='KeywordSortedInfoPackage',
   filename=None,
@@ -508,16 +529,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=873,
-  serialized_end=950,
+  serialized_start=937,
+  serialized_end=1014,
 )
 
 _EMBEDDING.fields_by_name['subdocembeddings'].message_type = _SUBDOCEMBEDDING
 _LATESTPACKAGE.fields_by_name['articles'].message_type = _ARTICLE
 _LATESTPACKAGE.fields_by_name['embeddings'].message_type = _EMBEDDING
 _ARTICLEPACKAGE.fields_by_name['articles'].message_type = _ARTICLE
 _EMBEDDINGPAKCAGE.fields_by_name['embeddings'].message_type = _EMBEDDING
```

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/recommend_common_util.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/recommend/recommend_common_util.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/recommend_tool.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/recommend/recommend_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/recommend/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/recommend/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/resources/model_management.json`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/common_tool.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/tools/common_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.28/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.0.29/recommend_model_sdk/tools/model_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,14 +545,20 @@
                     "full_text":
                     "created_at":
                     "published_at":
                     "title":
                     "author":  may not exist
                     "content":  may not exist
                     "feed_id":
+                    "hash": string
+                    "image_url": string
+                    "keyword_list": list string
+                    "cloud_id": int
+                    "major_language": string
+                    
                 }
                 "http...":{
                     
                 }
             }
             
             url_to_embedding
@@ -563,15 +569,15 @@
                     "model_version":
                     "embeddings":[] list float
                 }
             }
         """
         if isinstance(package_key,str) is False:
             raise ValueError("package_key is not str")
-        article_field_set = set(['url', 'full_text', 'created_at', 'published_at', 'title', 'author', 'content', 'feed_id', 'hash','image_url'])
+        article_field_set = set(['url', 'full_text', 'created_at', 'published_at', 'title', 'author', 'content', 'feed_id', 'hash','image_url','keyword_list','cloud_id','major_language'])
         
         self.valid_model_name_and_version(model_name,model_version)
 
         latest_package_key = package_key
         model_version_embedding_dir = os.path.join(os.path.join(os.path.join(self.__model_root_dir,model_name),model_version),'embedding')
         if os.path.exists(model_version_embedding_dir) is False or os.path.isdir(model_version_embedding_dir) is False:
             os.makedirs(model_version_embedding_dir)
```

### Comparing `bytetrade-recommend-model-sdk-0.0.28/setup.py` & `bytetrade-recommend-model-sdk-0.0.29/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.28",
+    version="0.0.29",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==3.20.1",
         "nltk==3.8.1",
         "boto3",
```

