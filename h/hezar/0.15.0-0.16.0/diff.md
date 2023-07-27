# Comparing `tmp/hezar-0.15.0.tar.gz` & `tmp/hezar-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.15.0.tar", max compression
+gzip compressed data, was "hezar-0.16.0.tar", max compression
```

## Comparing `hezar-0.15.0.tar` & `hezar-0.16.0.tar`

### file list

```diff
@@ -1,87 +1,84 @@
--rw-r--r--   0        0        0     1065 2023-07-16 06:43:10.952388 hezar-0.15.0/LICENSE
--rw-r--r--   0        0        0     4427 2023-07-16 06:43:10.952388 hezar-0.15.0/README.md
--rw-r--r--   0        0        0      261 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/__init__.py
--rw-r--r--   0        0        0     5396 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/builders.py
--rw-r--r--   0        0        0    10800 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/configs.py
--rw-r--r--   0        0        0     1735 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/__init__.py
--rw-r--r--   0        0        0     6333 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/data_collators.py
--rw-r--r--   0        0        0      223 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1709 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4576 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3701 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0       26 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      282 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1136 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1208 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1172 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0     9544 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/model.py
--rw-r--r--   0        0        0       67 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     3354 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0      240 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3082 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     3217 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     3347 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_summarization/__init__.py
--rw-r--r--   0        0        0      104 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/normalizers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/normalizers/nfkc.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/normalizers/nfkd.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/normalizers/normalizer.py
--rw-r--r--   0        0        0     2218 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      231 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0    18797 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8898 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2538 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2177 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    17120 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      163 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/common_utils.py
--rw-r--r--   0        0        0     3782 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/config_utils.py
--rw-r--r--   0        0        0      482 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     2773 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/logging.py
--rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/model_utils.py
--rw-r--r--   0        0        0     1626 2023-07-16 06:43:10.956388 hezar-0.15.0/pyproject.toml
--rw-r--r--   0        0        0     6874 1970-01-01 00:00:00.000000 hezar-0.15.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-27 10:11:58.207428 hezar-0.16.0/LICENSE
+-rw-r--r--   0        0        0     4427 2023-07-27 10:11:58.207428 hezar-0.16.0/README.md
+-rw-r--r--   0        0        0      261 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/__init__.py
+-rw-r--r--   0        0        0     5383 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/builders.py
+-rw-r--r--   0        0        0    11117 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/configs.py
+-rw-r--r--   0        0        0     2068 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6333 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      223 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4502 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3627 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0       26 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      282 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1136 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1208 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1172 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0     9544 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/model.py
+-rw-r--r--   0        0        0       67 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     3354 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3082 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-07-27 10:11:58.207428 hezar-0.16.0/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     3217 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3347 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/models/text_summarization/__init__.py
+-rw-r--r--   0        0        0      118 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     3492 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/normalizer.py
+-rw-r--r--   0        0        0     2954 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      231 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0    19346 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8914 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2538 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2177 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    17120 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      161 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5614 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0     3407 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/logging.py
+-rw-r--r--   0        0        0        0 2023-07-27 10:11:58.211428 hezar-0.16.0/hezar/utils/model_utils.py
+-rw-r--r--   0        0        0     1626 2023-07-27 10:11:58.211428 hezar-0.16.0/pyproject.toml
+-rw-r--r--   0        0        0     6874 1970-01-01 00:00:00.000000 hezar-0.16.0/PKG-INFO
```

### Comparing `hezar-0.15.0/LICENSE` & `hezar-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/README.md` & `hezar-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/builders.py` & `hezar-0.16.0/hezar/builders.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .registry import (  # noqa
     datasets_registry,  # noqa
     embeddings_registry,  # noqa
     metrics_registry,  # noqa
     models_registry,  # noqa
     preprocessors_registry,  # noqa
 )
-from .utils.config_utils import snake_case
+from .utils import snake_case
 
 
 __all__ = [
     "build_model",
     "build_dataset",
     "build_preprocessor",
     "build_embedding",
```

### Comparing `hezar-0.15.0/hezar/configs.py` & `hezar-0.16.0/hezar/configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     >>> bert_config = BertLMConfig(vocab_size=50000, hidden_size=768)
     >>> bert_config.save("saved/bert")
     >>> bert_config.push_to_hub("hezarai/bert-custom")
 """
 import os
 import tempfile
 from dataclasses import asdict, dataclass, field
+from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 import torch
 from huggingface_hub import create_repo, hf_hub_download, upload_file
 from omegaconf import DictConfig, OmegaConf
 
 from .constants import DEFAULT_MODEL_CONFIG_FILE, HEZAR_CACHE_DIR, ConfigType, TaskType
@@ -148,30 +149,34 @@
             config_path = hf_hub_download(
                 hub_or_local_path,
                 filename=filename,
                 subfolder=subfolder,
                 cache_dir=HEZAR_CACHE_DIR,
                 repo_type=repo_type,
             )
-
+        # Load config file and convert to dictionary
         dict_config = OmegaConf.load(config_path)
         config = OmegaConf.to_container(dict_config)
-        config_cls = get_module_config_class(config["name"], config_type=config["config_type"])
+        config_cls = get_module_config_class(config["name"], config_type=config.get("config_type", None))
+        if config_cls is None:
+            config_cls = cls
         config = config_cls.from_dict(config, strict=False, **kwargs)
         return config
 
     @classmethod
     def from_dict(cls, dict_config: Union[Dict, DictConfig], **kwargs):
         """
         Load config from a dict-like object
         """
         # Update config parameters with kwargs
         dict_config.update(**kwargs)
+        dict_config.pop("name", None)
+        dict_config.pop("config_type", None)
 
-        config = cls(**{k: v for k, v in dict_config.items() if hasattr(cls, k) and k != "config_type"})  # noqa
+        config = cls(**{k: v for k, v in dict_config.items() if hasattr(cls, k)})  # noqa
 
         return config
 
     def save(self, save_dir: Union[str, os.PathLike], filename: str, subfolder: Optional[str] = None):
         """
         Save the *config.yaml file to a local path
 
@@ -180,14 +185,16 @@
              filename: Config file name
              subfolder: Subfolder to save the config file
         """
         subfolder = subfolder or ""
         config = self.dict()
         # exclude None items
         config = {k: v for k, v in config.items() if v is not None}
+        # convert enums to value
+        config = {k: v.value if isinstance(v, Enum) else v for k, v in config.items()}
         # make and save to directory
         os.makedirs(os.path.join(save_dir, subfolder), exist_ok=True)
         save_path = os.path.join(save_dir, subfolder, filename)
         OmegaConf.save(config, save_path)
         return save_path
 
     def push_to_hub(
@@ -225,15 +232,15 @@
             path_or_fileobj=config_path,
             path_in_repo=path_in_repo,
             repo_id=repo_id,
             repo_type=repo_type,
             commit_message=commit_message,
         )
         logger.info(
-            f"Uploaded:`{self.__class__.__name__}(name={self.name})` --> `{os.path.join(repo_id, subfolder, filename)}`"
+            f"Uploaded:`{self.__class__.__name__}(name={self.name})` --> `{os.path.join(repo_id, path_in_repo)}`"
         )
 
 
 @dataclass
 class ModelConfig(Config):
     """
     Base dataclass for all model configs
```

### Comparing `hezar-0.15.0/hezar/constants.py` & `hezar-0.16.0/hezar/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 HEZAR_CACHE_DIR = os.getenv("HEZAR_CACHE_DIR", f'{os.path.expanduser("~")}/.hezar')
 
 DEFAULT_MODEL_FILE = "model.pt"
 DEFAULT_MODEL_CONFIG_FILE = "model_config.yaml"
 DEFAULT_TRAINER_SUBFOLDER = "train"
 DEFAULT_TRAINER_CONFIG_FILE = "train_config.yaml"
 DEFAULT_PREPROCESSOR_SUBFOLDER = "preprocessor"
+DEFAULT_NORMALIZER_CONFIG_FILE = "normalizer_config.yaml"
 DEFAULT_TOKENIZER_FILE = "tokenizer.json"
 DEFAULT_TOKENIZER_CONFIG_FILE = "tokenizer_config.yaml"
 DEFAULT_DATASET_CONFIG_FILE = "dataset_config.yaml"
 DEFAULT_EMBEDDING_FILE = "embedding.bin"
 DEFAULT_EMBEDDING_CONFIG_FILE = "embedding_config.yaml"
 DEFAULT_EMBEDDING_SUBFOLDER = "embedding"
 
@@ -40,14 +41,26 @@
     MODEL = "model"
     DATASET = "dataset"
     PREPROCESSOR = "preprocessor"
     EMBEDDING = "embedding"
     TRAINER = "trainer"
     OPTIMIZER = "optimizer"
     CRITERION = "criterion"
+    LR_SCHEDULER = "lr_scheduler"
+    METRIC = "metric"
+
+
+class RegistryType(str, Enum):
+    MODEL = "model"
+    DATASET = "dataset"
+    PREPROCESSOR = "preprocessor"
+    EMBEDDING = "embedding"
+    TRAINER = "trainer"
+    OPTIMIZER = "optimizer"
+    CRITERION = "criterion"
     LR_SCHEDULER = "lr_scheduler"
     METRIC = "metric"
 
 
 class SplitType(str, Enum):
     TRAIN = "train"
     EVAL = "eval"
```

### Comparing `hezar-0.15.0/hezar/data/data_collators.py` & `hezar-0.16.0/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/data/datasets/dataset.py` & `hezar-0.16.0/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.16.0/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from typing import Dict, List, Tuple
 
 from datasets import load_dataset
 
 from ...configs import DatasetConfig
 from ...constants import TaskType
-from ...preprocessors import Sequential, Tokenizer
+from ...preprocessors import Tokenizer
 from ...registry import register_dataset
 from ...utils import get_logger
 from ..data_collators import SequenceLabelingDataCollator
 from .dataset import Dataset
 
 
 logger = get_logger(__name__)
@@ -42,15 +42,14 @@
     """
 
     def __init__(self, config: SequenceLabelingDatasetConfig, split=None, **kwargs):
         super().__init__(config, **kwargs)
         self.dataset = self._load(split)
         self._extract_labels()
         self.tokenizer = self._build_tokenizer()
-        self.normalizer = Sequential(self.config.normalizers)
         if self.tokenizer:
             self.data_collator = SequenceLabelingDataCollator(self.tokenizer)
 
     def _load(self, split):
         """
         Load the dataset
```

### Comparing `hezar-0.15.0/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.16.0/hezar/data/datasets/text_classification_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Dict, List, Tuple
 
 import torch
 from datasets import load_dataset
 
 from ...configs import DatasetConfig
 from ...constants import TaskType
-from ...preprocessors import Sequential, Tokenizer
+from ...preprocessors import Tokenizer
 from ...registry import register_dataset
 from ...utils import get_logger
 from ..data_collators import TextPaddingDataCollator
 from .dataset import Dataset
 
 
 logger = get_logger(__name__)
@@ -41,15 +41,14 @@
     """
 
     def __init__(self, config: TextClassificationDatasetConfig, split=None, **kwargs):
         super().__init__(config, **kwargs)
         self.dataset = self._load(split)
         self._extract_labels()
         self.tokenizer = self._build_tokenizer()
-        self.normalizer = Sequential(self.config.normalizers)
         self.data_collator = TextPaddingDataCollator(
             tokenizer=self.tokenizer,
             max_length=self.config.max_length,
         )
 
     def _load(self, split):
         """
```

### Comparing `hezar-0.15.0/hezar/data/utils/data_utils.py` & `hezar-0.16.0/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/embeddings/embedding.py` & `hezar-0.16.0/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/embeddings/fasttext.py` & `hezar-0.16.0/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/embeddings/word2vec.py` & `hezar-0.16.0/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/metrics/f1.py` & `hezar-0.16.0/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/metrics/metric.py` & `hezar-0.16.0/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/metrics/recall.py` & `hezar-0.16.0/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/metrics/seqeval.py` & `hezar-0.16.0/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.16.0/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.16.0/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.16.0/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.16.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.16.0/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.16.0/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/model.py` & `hezar-0.16.0/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.16.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.16.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.16.0/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.16.0/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.16.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.16.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.16.0/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.16.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/preprocessors/preprocessor.py` & `hezar-0.16.0/hezar/preprocessors/preprocessor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from typing import Dict, List, Tuple, Union
+from collections import OrderedDict
 
-from ..builders import build_preprocessor
-from ..constants import DEFAULT_PREPROCESSOR_SUBFOLDER
+from huggingface_hub import hf_hub_download
+from omegaconf import OmegaConf
+
+from ..constants import DEFAULT_PREPROCESSOR_SUBFOLDER, RegistryType, RepoType
+from ..utils import get_module_class, list_repo_files
 
 
 class Preprocessor:
     """
     Base class for all data preprocessors.
 
     Args:
@@ -13,54 +16,69 @@
     """
 
     preprocessor_subfolder = DEFAULT_PREPROCESSOR_SUBFOLDER
 
     def __init__(self, config, **kwargs):
         self.config = config.update(kwargs)
 
-    def __call__(self, inputs, *args, **kwargs):
+    def __call__(self, inputs, **kwargs):
         """
         An abstract call method for a preprocessor. All preprocessors must implement this.
 
         Args:
             inputs: Raw inputs to process. Usually a list or a dict
-            args: Extra arguments depending on the preprocessor
             **kwargs: Extra keyword arguments depending on the preprocessor
         """
         raise NotImplementedError
 
-    def save(self, path):
+    def save(self, path, **kwargs):
         raise NotImplementedError
 
     def push_to_hub(self, hub_path):
         raise NotImplementedError
 
+    @classmethod
+    def load(
+        cls,
+        hub_or_local_path,
+        subfolder=None,
+        **kwargs
+    ):
+        """
+        Load a preprocessor or a pipeline of preprocessors from a local or Hub path. This method automatically detects
+        any preprocessor in the path. If there's only one preprocessor, returns it and if there are more, returns a
+        dictionary of preprocessors.
 
-class Sequential:
-    """
-    A sequence of preprocessors
-    """
-    def __init__(self, preprocessors: Union[List[Preprocessor], List[Tuple[str, Dict]]]):
-        self._processors = self._prepare_processors(preprocessors)
+        This method must also be overriden by subclasses as it internally calls this method for every possible
+        preprocessor found in the repo.
 
-    def __str__(self):
-        return f"{self.__class__.__name__}({[p.config.name for p in self._processors] if self._processors else []})"
+        Args:
+            hub_or_local_path: Path to hub or local repo
+            subfolder: Subfolder for the preprocessor.
+            **kwargs: Extra kwargs
 
-    @staticmethod
-    def _prepare_processors(preprocessors):
-        processors = []
-        if isinstance(preprocessors, list) and len(preprocessors):
-            for p in preprocessors:
-                if isinstance(p, tuple):
-                    name, kwargs = p
-                    processors.append(build_preprocessor(name, **kwargs))
-                elif isinstance(p, Preprocessor):
-                    processors.append(p)
+        Returns:
+            A Preprocessor subclass or a dict of Preprocessor subclass instances
+        """
+        subfolder = subfolder or cls.preprocessor_subfolder
+        preprocessor_files = list_repo_files(hub_or_local_path, subfolder=subfolder)
+        preprocessors = OrderedDict()
+        for f in preprocessor_files:
+            if f.endswith(".yaml"):
+                config_file = hf_hub_download(
+                    hub_or_local_path,
+                    filename=f,
+                    subfolder=subfolder,
+                    repo_type=RepoType.MODEL
+                )
+                config = OmegaConf.load(config_file)
+                name = config.get("name", None)
+                if name:
+                    preprocessor_cls = get_module_class(name, module_type=RegistryType.PREPROCESSOR)
+                    preprocessor = preprocessor_cls.load(hub_or_local_path, subfolder=subfolder)
+                    preprocessors[name] = preprocessor
                 else:
-                    raise ValueError(f"Items in the preprocessors parameter must be either a `Preprocessor` or a tuple "
-                                     f"of `(preprocessor_name, preprocessor_kwargs)`! Got `{type(p)}`!")
-            return processors
-
-    def __call__(self, inputs, *args, **kwargs):
-        for processor in self._processors:
-            inputs = processor(inputs, **kwargs)
-        return inputs
+                    raise ValueError(f"The config file `{config_file}` does not have the property `name`!")
+        if len(preprocessors) == 1:
+            return list(preprocessors.values())[0]
+
+        return preprocessors
```

### Comparing `hezar-0.15.0/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.16.0/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.16.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.16.0/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import tempfile
 from collections import defaultdict
 from dataclasses import dataclass
-from typing import Dict, List, Mapping, Optional, Union
+from typing import Dict, List, Literal, Mapping, Optional, Union
 
 import torch
 from huggingface_hub import create_repo, upload_file
 from tokenizers import Tokenizer as HFTokenizer
 from tokenizers.decoders import Decoder
 from tokenizers.models import Model
 
@@ -70,19 +70,32 @@
         if isinstance(ids[0], list):
             return self._tokenizer.decode_batch(ids, skip_special_tokens=skip_special_tokens)
         return self._tokenizer.decode(ids, skip_special_tokens=skip_special_tokens)
 
     def pad_encoded_batch(
         self,
         inputs,
-        padding: Union[bool, str] = None,
+        padding: Literal["longest", "max_length"] = None,
         max_length: Optional[int] = None,
         return_tensors: Optional[str] = None,
         skip_keys: list = None,
     ):
+        """
+        Given a batch of encoded inputs, add padding to all of them so that the inputs are of the same length.
+
+        Args:
+            inputs: Input batch of encoded tokens
+            padding: Padding type, could be one of ["longest", "max_length"]
+            max_length: Max input length (only if padding is set to "max_length")
+            return_tensors: The type of tensors to return
+            skip_keys: A list of keys to skip padding
+
+        Returns:
+
+        """
 
         if isinstance(inputs, (list, tuple)) and isinstance(inputs[0], Mapping):
             inputs = {key: [example[key] for example in inputs] for key in inputs[0].keys()}
 
         inputs_max_length = max([len(x) for x in inputs[self.token_ids_name]])
         # resolve padding and max_length parameters
         padding = padding or self.config.padding_strategy
@@ -105,35 +118,36 @@
             if max_length is None:
                 logger.warning("Setting padding='max_length' but no max_length value is provided in the function "
                                "parameters nor the tokenizer config! Falling back to padding='longest'")
                 inputs_length = inputs_max_length
             else:
                 # TODO implement truncation if possible and remove this condition
                 if max_length <= inputs_max_length:
-                    logger.warning(f"Setting max_length to {max_length} while max input length is {inputs_max_length}!"
+                    logger.warning(f"Cannot set max_length to {max_length} "
+                                   f"while max input length is {inputs_max_length}!"
                                    f"Falling back to padding='longest' "
                                    f"since truncation is not available yet in Hezar :(")
                     inputs_length = inputs_max_length
                 else:
                     inputs_length = max_length
 
         inputs = convert_batch_dict_dtype(inputs, dtype="list", skip_keys=skip_keys)
 
         skip_keys = skip_keys or []
-        for field, batch in inputs.items():
-            if field in skip_keys:
+        for key, batch in inputs.items():
+            if key in skip_keys:
                 continue
-            padding_id = 0 if field == "attention_mask" else self.config.pad_token_id
+            padding_id = 0 if key == "attention_mask" else self.config.pad_token_id
             padded_batch = []
             for x in batch:
                 difference = inputs_length - len(x)
                 paddings = [padding_id] * difference
                 padded_x = x + paddings if self.config.padding_direction == "right" else paddings + x
                 padded_batch.append(padded_x)
-            inputs[field] = padded_batch
+            inputs[key] = padded_batch
 
         inputs = convert_batch_dict_dtype(inputs, dtype=return_tensors)
 
         return inputs
 
     def __call__(
         self,
```

### Comparing `hezar-0.15.0/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.16.0/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/registry.py` & `hezar-0.16.0/hezar/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 __all__ = [
     "register_model",
     "register_preprocessor",
     "register_dataset",
     "register_embedding",
     "register_metric",
     "register_trainer",
+    "Registry",
 ]
 
 logger = get_logger(__name__)
 
 
 @dataclass
 class Registry:
```

### Comparing `hezar-0.15.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.16.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.16.0/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/trainers/trainer.py` & `hezar-0.16.0/hezar/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/trainers/trainer_utils.py` & `hezar-0.16.0/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/utils/common_utils.py` & `hezar-0.16.0/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.15.0/hezar/utils/hub_utils.py` & `hezar-0.16.0/hezar/utils/hub_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os.path
 
 from huggingface_hub import HfApi, Repository
 
-from ..constants import HEZAR_CACHE_DIR, HEZAR_HUB_ID
+from ..constants import HEZAR_CACHE_DIR, HEZAR_HUB_ID, RepoType
 from ..utils.logging import get_logger
 
 
 __all__ = [
     "resolve_pretrained_path",
     "get_local_cache_path",
     "exists_in_cache",
     "exists_on_hub",
     "clone_repo",
+    "list_repo_files",
 ]
 
 logger = get_logger(__name__)
 
 
 def resolve_pretrained_path(hub_or_local_path):
     """
@@ -92,7 +93,29 @@
         save_path: Path to clone the repo to
 
     Returns:
         the local path to the repo
     """
     repo = Repository(local_dir=save_path, clone_from=repo_id, **kwargs)
     return repo.local_dir
+
+
+def list_repo_files(hub_or_local_path: str, subfolder: str = None):
+    """
+    List all files in a Hub or local model repo
+
+    Args:
+        hub_or_local_path: Path to hub or local repo
+        subfolder: Optional subfolder path
+
+    Returns:
+        A list of all file names
+    """
+    if os.path.isdir(hub_or_local_path):
+        files = os.listdir(hub_or_local_path)
+    else:
+        files = HfApi().list_repo_files(hub_or_local_path, repo_type=RepoType.MODEL)
+
+    if subfolder is not None:
+        files = [x.replace(f"{subfolder}/", "") for x in files if subfolder in x]
+
+    return files
```

### Comparing `hezar-0.15.0/pyproject.toml` & `hezar-0.16.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.15.0"
+version = "0.16.0"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.15.0/PKG-INFO` & `hezar-0.16.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.15.0
+Version: 0.16.0
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
```

