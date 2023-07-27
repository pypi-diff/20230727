# Comparing `tmp/unstructured-0.8.4.tar.gz` & `tmp/unstructured-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.8.4.tar", last modified: Wed Jul 26 18:24:21 2023, max compression
+gzip compressed data, was "unstructured-0.8.5.tar", last modified: Thu Jul 27 18:38:13 2023, max compression
```

## Comparing `unstructured-0.8.4.tar` & `unstructured-0.8.5.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.186249 unstructured-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-26 18:24:08.000000 unstructured-0.8.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 18:24:08.000000 unstructured-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-26 18:24:21.186249 unstructured-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-07-26 18:24:08.000000 unstructured-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.158249 unstructured-0.8.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-dropbox.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-gcs.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-onedrive.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-outlook.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 18:24:08.000000 unstructured-0.8.4/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-26 18:24:21.186249 unstructured-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-26 18:24:08.000000 unstructured-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.158249 unstructured-0.8.4/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.158249 unstructured-0.8.4/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-26 18:24:08.000000 unstructured-0.8.4/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-26 18:24:08.000000 unstructured-0.8.4/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-26 18:24:08.000000 unstructured-0.8.4/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-26 18:24:08.000000 unstructured-0.8.4/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.158249 unstructured-0.8.4/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.162248 unstructured-0.8.4/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.162248 unstructured-0.8.4/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.162248 unstructured-0.8.4/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20069 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.162248 unstructured-0.8.4/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.166248 unstructured-0.8.4/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/outlook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.166248 unstructured-0.8.4/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33906 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.166248 unstructured-0.8.4/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.178249 unstructured-0.8.4/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.182249 unstructured-0.8.4/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/org.py
--rw-r--r--   0 runner    (1001) docker     (123)    15851 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.186249 unstructured-0.8.4/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-26 18:24:08.000000 unstructured-0.8.4/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:21.162248 unstructured-0.8.4/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-26 18:24:20.000000 unstructured-0.8.4/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-26 18:24:21.000000 unstructured-0.8.4/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:24:20.000000 unstructured-0.8.4/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 18:24:20.000000 unstructured-0.8.4/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-26 18:24:20.000000 unstructured-0.8.4/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-26 18:24:20.000000 unstructured-0.8.4/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.752186 unstructured-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-27 18:38:02.000000 unstructured-0.8.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 18:38:02.000000 unstructured-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-27 18:38:13.752186 unstructured-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16273 2023-07-27 18:38:02.000000 unstructured-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.732186 unstructured-0.8.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-dropbox.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-gcs.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-onedrive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-outlook.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-27 18:38:02.000000 unstructured-0.8.5/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-27 18:38:13.752186 unstructured-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-27 18:38:02.000000 unstructured-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.732186 unstructured-0.8.5/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.732186 unstructured-0.8.5/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-27 18:38:02.000000 unstructured-0.8.5/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 18:38:02.000000 unstructured-0.8.5/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-27 18:38:02.000000 unstructured-0.8.5/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-27 18:38:02.000000 unstructured-0.8.5/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.732186 unstructured-0.8.5/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.732186 unstructured-0.8.5/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.736186 unstructured-0.8.5/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16209 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.736186 unstructured-0.8.5/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20781 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.736186 unstructured-0.8.5/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.740186 unstructured-0.8.5/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/outlook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.740186 unstructured-0.8.5/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33906 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.740186 unstructured-0.8.5/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.744186 unstructured-0.8.5/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.752186 unstructured-0.8.5/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12408 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.752186 unstructured-0.8.5/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-27 18:38:02.000000 unstructured-0.8.5/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:38:13.732186 unstructured-0.8.5/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-07-27 18:38:13.000000 unstructured-0.8.5/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-27 18:38:13.000000 unstructured-0.8.5/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:38:13.000000 unstructured-0.8.5/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 18:38:13.000000 unstructured-0.8.5/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-27 18:38:13.000000 unstructured-0.8.5/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 18:38:13.000000 unstructured-0.8.5/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.8.4/LICENSE.md` & `unstructured-0.8.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/MANIFEST.in` & `unstructured-0.8.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/PKG-INFO` & `unstructured-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.4
+Version: 0.8.5
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.4 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.5 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.8.4/README.md` & `unstructured-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/setup.py` & `unstructured-0.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.8.5/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.8.5/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/test_unstructured/test_utils.py` & `unstructured-0.8.5/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/cleaners/core.py` & `unstructured-0.8.5/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/cleaners/extract.py` & `unstructured-0.8.5/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/cleaners/translate.py` & `unstructured-0.8.5/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/documents/base.py` & `unstructured-0.8.5/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/documents/coordinates.py` & `unstructured-0.8.5/unstructured/documents/coordinates.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/documents/elements.py` & `unstructured-0.8.5/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/documents/email_elements.py` & `unstructured-0.8.5/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/documents/html.py` & `unstructured-0.8.5/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/documents/xml.py` & `unstructured-0.8.5/unstructured/documents/xml.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional, Union
 
-from lxml import etree
+from lxml import etree, html
 
 from unstructured.documents.base import Document, Page
 from unstructured.file_utils.encoding import read_txt_file
 from unstructured.logger import logger
 from unstructured.partition.text import (
     element_from_text,
     partition_text,
@@ -65,14 +65,15 @@
         # The correct output is returned once you add the initial return.
         is_html_parser = isinstance(self.parser, etree.HTMLParser)
         if content and not content.startswith("\n") and is_html_parser:
             content = "\n" + content
         if self.document_tree is None:
             try:
                 document_tree = etree.fromstring(content, self.parser)
+                print("document_tree", document_tree)
                 if document_tree is None:
                     raise ValueError("document_tree is None")
 
             # NOTE(robinson) - The following ValueError occurs with unicode strings. In that
             # case, we call back to encoding the string and passing in bytes.
             #     ValueError: Unicode strings with encoding declaration are not supported.
             #     Please use  bytes input or XML fragments without declaration.
@@ -88,14 +89,20 @@
                     for element in partition_text(text=element.text, paragraph_grouper=False):
                         text_content.append(element.text)
 
                     for text in text_content:
                         element = etree.Element("span")
                         element.text = str(element_from_text(text=text))
                         document_tree.append(element)
+            if "</a>" in content:
+                tree = html.fromstring(content)
+                links = list(tree.iterlinks())
+                print("here", links)
+                for el in document_tree:
+                    print(el)
 
             if self.stylesheet:
                 if isinstance(self.parser, etree.HTMLParser):
                     logger.warning(
                         "You are using the HTML parser with an XSLT stylesheet. "
                         "Stylesheets are more commonly parsed with the "
                         "XMLParser. If your HTML does not display properly, try "
@@ -104,14 +111,15 @@
                     )
                 xslt = etree.parse(self.stylesheet)
                 transform = etree.XSLT(xslt)
                 document_tree = transform(document_tree)
 
             self.document_tree = document_tree
 
+        print("self.document_tree", self.document_tree)
         return self.document_tree
 
     @classmethod
     def from_string(
         cls,
         text: str,
         parser: VALID_PARSERS = None,
@@ -130,8 +138,10 @@
         filename,
         parser: VALID_PARSERS = None,
         stylesheet: Optional[str] = None,
         encoding: Optional[str] = None,
         **kwargs,
     ):
         _, content = read_txt_file(filename=filename, encoding=encoding)
+        print("_____", _)
+        print("content", content)
         return cls.from_string(content, parser=parser, stylesheet=stylesheet, **kwargs)
```

### Comparing `unstructured-0.8.4/unstructured/file_utils/encoding.py` & `unstructured-0.8.5/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/file_utils/exploration.py` & `unstructured-0.8.5/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/file_utils/file_conversion.py` & `unstructured-0.8.5/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/file_utils/filetype.py` & `unstructured-0.8.5/unstructured/file_utils/filetype.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,21 +297,42 @@
             return FileType.XML
 
     elif mime_type in TXT_MIME_TYPES or mime_type.startswith("text"):
         if not encoding:
             encoding = "utf-8"
         formatted_encoding = format_encoding_str(encoding)
 
+        if extension in [
+            ".eml",
+            ".md",
+            ".rtf",
+            ".html",
+            ".rst",
+            ".org",
+            ".csv",
+            ".tsv",
+            ".json",
+        ]:
+            return EXT_TO_FILETYPE.get(extension)
+
         # NOTE(crag): for older versions of the OS libmagic package, such as is currently
         # installed on the Unstructured docker image, .json files resolve to "text/plain"
         # rather than "application/json". this corrects for that case.
-        if _is_text_file_a_json(file=file, filename=filename, encoding=formatted_encoding):
+        if _is_text_file_a_json(
+            file=file,
+            filename=filename,
+            encoding=formatted_encoding,
+        ):
             return FileType.JSON
 
-        if _is_text_file_a_csv(file=file, filename=filename, encoding=formatted_encoding):
+        if _is_text_file_a_csv(
+            file=file,
+            filename=filename,
+            encoding=formatted_encoding,
+        ):
             return FileType.CSV
 
         if file and _check_eml_from_buffer(file=file) is True:
             return FileType.EML
 
         if extension in PLAIN_TEXT_EXTENSIONS:
             return EXT_TO_FILETYPE.get(extension)
@@ -446,15 +467,19 @@
 
 def _is_text_file_a_csv(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     encoding: Optional[str] = "utf-8",
 ):
     """Detects if a file that has a text/plain MIME type is a CSV file."""
-    file_text = _read_file_start_for_type_check(file=file, filename=filename, encoding=encoding)
+    file_text = _read_file_start_for_type_check(
+        file=file,
+        filename=filename,
+        encoding=encoding,
+    )
     lines = file_text.strip().splitlines()
     if len(lines) < 2:
         return False
     lines = lines[: len(lines)] if len(lines) < 10 else lines[:10]
     header_count = _count_commas(lines[0])
     if any("," not in line for line in lines):
         return False
@@ -473,14 +498,15 @@
     return EMAIL_HEAD_RE.match(file_head) is not None
 
 
 def document_to_element_list(
     document: "DocumentLayout",
     include_page_breaks: bool = False,
     sort: bool = False,
+    last_modification_date: Optional[str] = None,
 ) -> List[Element]:
     """Converts a DocumentLayout object to a list of unstructured elements."""
     elements: List[Element] = []
     num_pages = len(document.pages)
     for i, page in enumerate(document.pages):
         page_elements: List[Element] = []
 
@@ -495,18 +521,22 @@
             else:
                 coordinate_system = None
 
             element = normalize_layout_element(layout_element, coordinate_system=coordinate_system)
 
             if isinstance(element, List):
                 for el in element:
+                    if last_modification_date:
+                        el.metadata.date = last_modification_date
                     el.metadata.page_number = i + 1
                 page_elements.extend(element)
                 continue
             else:
+                if last_modification_date:
+                    element.metadata.date = last_modification_date
                 element.metadata.text_as_html = (
                     layout_element.text_as_html if hasattr(layout_element, "text_as_html") else None
                 )
                 page_elements.append(element)
             coordinates = (
                 element.metadata.coordinates.points if element.metadata.coordinates else None
             )
@@ -528,14 +558,15 @@
                     if el.metadata.coordinates
                     else float("inf"),
                     el.id,
                 ),
             )
         if include_page_breaks and i < num_pages - 1:
             page_elements.append(PageBreak(text=""))
+        print("page_element", page_elements)
         elements.extend(page_elements)
 
     return elements
 
 
 def _get_page_image_metadata(
     page: PageLayout,
```

### Comparing `unstructured-0.8.4/unstructured/file_utils/metadata.py` & `unstructured-0.8.5/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/azure.py` & `unstructured-0.8.5/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/biomed.py` & `unstructured-0.8.5/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/confluence.py` & `unstructured-0.8.5/unstructured/ingest/connector/confluence.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/discord.py` & `unstructured-0.8.5/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/dropbox.py` & `unstructured-0.8.5/unstructured/ingest/connector/dropbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,15 @@
         if self.config.dir_path == " ":
             return Path(self.standard_config.download_dir) / re.sub(
                 "^/",
                 "",
                 self.remote_file_path,
             )
         else:
-            return Path(
-                self.standard_config.download_dir,
-            ) / self.remote_file_path.replace(
+            return Path(self.standard_config.download_dir) / self.remote_file_path.replace(
                 f"/{self.config.dir_path}/",
                 "",
             )
 
 
 @requires_dependencies(["dropboxdrivefs", "fsspec"])
 class DropboxConnector(FsspecConnector):
```

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/elasticsearch.py` & `unstructured-0.8.5/unstructured/ingest/connector/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/fsspec.py` & `unstructured-0.8.5/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/gcs.py` & `unstructured-0.8.5/unstructured/ingest/connector/gcs.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/git.py` & `unstructured-0.8.5/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/github.py` & `unstructured-0.8.5/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/gitlab.py` & `unstructured-0.8.5/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/google_drive.py` & `unstructured-0.8.5/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/local.py` & `unstructured-0.8.5/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/onedrive.py` & `unstructured-0.8.5/unstructured/ingest/connector/onedrive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/outlook.py` & `unstructured-0.8.5/unstructured/ingest/connector/outlook.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/reddit.py` & `unstructured-0.8.5/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/s3.py` & `unstructured-0.8.5/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/slack.py` & `unstructured-0.8.5/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.8.5/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.8.5/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/interfaces.py` & `unstructured-0.8.5/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/ingest/main.py` & `unstructured-0.8.5/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/nlp/english-words.txt` & `unstructured-0.8.5/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/nlp/english_words.py` & `unstructured-0.8.5/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/nlp/patterns.py` & `unstructured-0.8.5/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/nlp/tokenize.py` & `unstructured-0.8.5/unstructured/nlp/tokenize.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from functools import lru_cache
 from typing import List, Tuple
 
 if sys.version_info < (3, 8):
-    from typing_extensions import Final
+    from typing_extensions import Final  # pragma: no cover
 else:
     from typing import Final
 
 import nltk
 from nltk import pos_tag as _pos_tag
 from nltk import sent_tokenize as _sent_tokenize
 from nltk import word_tokenize as _word_tokenize
@@ -19,38 +19,33 @@
     """If the required nlt package is not present, download it."""
     try:
         nltk.find(f"{package_category}/{package_name}")
     except LookupError:
         nltk.download(package_name)
 
 
-NLTK_PACKAGES = [
-    ("tokenizers", "punkt"),
-    ("taggers", "averaged_perceptron_tagger"),
-]
-
-for package_category, package_name in NLTK_PACKAGES:
-    _download_nltk_package_if_not_present(package_name, package_category)
-
-
 @lru_cache(maxsize=CACHE_MAX_SIZE)
 def sent_tokenize(text: str) -> List[str]:
     """A wrapper around the NLTK sentence tokenizer with LRU caching enabled."""
+    _download_nltk_package_if_not_present("tokenizers", "punkt")
     return _sent_tokenize(text)
 
 
 @lru_cache(maxsize=CACHE_MAX_SIZE)
 def word_tokenize(text: str) -> List[str]:
     """A wrapper around the NLTK word tokenizer with LRU caching enabled."""
+    _download_nltk_package_if_not_present("tokenizers", "punkt")
     return _word_tokenize(text)
 
 
 @lru_cache(maxsize=CACHE_MAX_SIZE)
 def pos_tag(text: str) -> List[Tuple[str, str]]:
     """A wrapper around the NLTK POS tagger with LRU caching enabled."""
+    _download_nltk_package_if_not_present("tokenizers", "punkt")
+    _download_nltk_package_if_not_present("taggers", "averaged_perceptron_tagger")
     # NOTE(robinson) - Splitting into sentences before tokenizing. The helps with
     # situations like "ITEM 1A. PROPERTIES" where "PROPERTIES" can be mistaken
     # for a verb because it looks like it's in verb form an "ITEM 1A." looks like the subject.
     sentences = _sent_tokenize(text)
     parts_of_speech = []
     for sentence in sentences:
         tokens = _word_tokenize(sentence)
```

### Comparing `unstructured-0.8.4/unstructured/partition/__init__.py` & `unstructured-0.8.5/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/partition/api.py` & `unstructured-0.8.5/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/partition/auto.py` & `unstructured-0.8.5/unstructured/partition/auto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import io
-from typing import IO, Callable, Dict, Optional, Tuple
+from typing import IO, Callable, Dict, List, Optional, Tuple
 
 import requests
 
 from unstructured.documents.elements import DataSourceMetadata
 from unstructured.file_utils.filetype import (
     FILETYPE_TO_MIMETYPE,
     STR_TO_FILETYPE,
@@ -43,14 +43,15 @@
     file_filename: Optional[str] = None,
     url: Optional[str] = None,
     include_page_breaks: bool = False,
     strategy: str = "auto",
     encoding: Optional[str] = None,
     paragraph_grouper: Optional[Callable[[str], str]] = None,
     headers: Dict[str, str] = {},
+    skip_infer_table_types: List[str] = ["pdf", "jpg", "png"],
     ssl_verify: bool = True,
     ocr_languages: str = "eng",
     pdf_infer_table_structure: bool = False,
     xml_keep_tags: bool = False,
     data_source_metadata: Optional[DataSourceMetadata] = None,
     **kwargs,
 ):
@@ -78,14 +79,16 @@
         The strategy to use for partitioning PDF/image. Uses a layout detection model if set
         to 'hi_res', otherwise partition simply extracts the text from the document
         and processes it.
     encoding
         The encoding method used to decode the text input. If None, utf-8 will be used.
     headers
         The headers to be used in conjunction with the HTTP request if URL is set.
+    skip_infer_table_types
+        The document types that you want to skip table extraction with.
     ssl_verify
         If the URL parameter is set, determines whether or not partition uses SSL verification
         in the HTTP request.
     ocr_languages
         The languages to use for the Tesseract agent. To use a language, you'll first need
         to isntall the appropriate Tesseract language pack.
     pdf_infer_table_structure
@@ -119,14 +122,20 @@
             content_type=content_type,
             encoding=encoding,
         )
 
     if file is not None:
         file.seek(0)
 
+    infer_table_structure = decide_table_extraction(
+        filetype,
+        skip_infer_table_types,
+        pdf_infer_table_structure,
+    )
+
     if filetype == FileType.DOC:
         elements = partition_doc(filename=filename, file=file, **kwargs)
     elif filetype == FileType.DOCX:
         elements = partition_docx(filename=filename, file=file, **kwargs)
     elif filetype == FileType.ODT:
         elements = partition_odt(filename=filename, file=file, **kwargs)
     elif filetype == FileType.EML:
@@ -179,25 +188,26 @@
         )
     elif filetype == FileType.PDF:
         elements = partition_pdf(
             filename=filename,  # type: ignore
             file=file,  # type: ignore
             url=None,
             include_page_breaks=include_page_breaks,
-            infer_table_structure=pdf_infer_table_structure,
+            infer_table_structure=infer_table_structure,
             strategy=strategy,
             ocr_languages=ocr_languages,
             **kwargs,
         )
     elif (filetype == FileType.PNG) or (filetype == FileType.JPG):
         elements = partition_image(
             filename=filename,  # type: ignore
             file=file,  # type: ignore
             url=None,
             include_page_breaks=include_page_breaks,
+            infer_table_structure=infer_table_structure,
             strategy=strategy,
             ocr_languages=ocr_languages,
             **kwargs,
         )
     elif filetype == FileType.TXT:
         elements = partition_text(
             filename=filename,
@@ -270,7 +280,26 @@
     file = io.BytesIO(response.content)
 
     content_type = content_type or response.headers.get("Content-Type")
     encoding = response.headers.get("Content-Encoding", "utf-8")
 
     filetype = detect_filetype(file=file, content_type=content_type, encoding=encoding)
     return file, filetype
+
+
+def decide_table_extraction(
+    filetype: Optional[FileType],
+    skip_infer_table_types: List[str],
+    pdf_infer_table_structure: bool,
+) -> bool:
+    doc_type = filetype.name.lower() if filetype else None
+
+    if doc_type == "pdf":
+        if doc_type in skip_infer_table_types and pdf_infer_table_structure:
+            logger.warning(
+                f"Conflict between variables skip_infer_table_types: {skip_infer_table_types}"
+                f"and pdf_infer_table_structure: {pdf_infer_table_structure},"
+                "please reset skip_infer_table_types to turn on table extraction for PDFs.",
+            )
+        return not (doc_type in skip_infer_table_types) or pdf_infer_table_structure
+
+    return not (doc_type in skip_infer_table_types)
```

### Comparing `unstructured-0.8.4/unstructured/partition/common.py` & `unstructured-0.8.5/unstructured/partition/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
+import os
 import subprocess
+from datetime import datetime
 from io import BufferedReader, BytesIO, TextIOWrapper
 from tempfile import SpooledTemporaryFile
 from typing import IO, TYPE_CHECKING, Any, BinaryIO, Dict, List, Optional, Tuple, Union
 
 from docx import table as docxtable
 from tabulate import tabulate
 
@@ -25,16 +27,40 @@
 if TYPE_CHECKING:
     from unstructured_inference.inference.layoutelement import (
         LayoutElement,
         LocationlessLayoutElement,
     )
 
 
+def get_last_modified_date(filename: str) -> Union[str, None]:
+    modify_date = datetime.fromtimestamp(os.path.getmtime(filename))
+    return modify_date.strftime("%Y-%m-%dT%H:%M:%S%z")
+
+
+def get_last_modified_date_from_file(
+    file: Union[IO[bytes], SpooledTemporaryFile, BinaryIO, bytes],
+) -> Union[str, None]:
+    filename = None
+    if hasattr(file, "name"):
+        filename = file.name
+
+    if not filename:
+        return None
+
+    modify_date = get_last_modified_date(filename)
+    return modify_date
+
+
 def normalize_layout_element(
-    layout_element: Union["LayoutElement", "LocationlessLayoutElement", Element, Dict[str, Any]],
+    layout_element: Union[
+        "LayoutElement",
+        "LocationlessLayoutElement",
+        Element,
+        Dict[str, Any],
+    ],
     coordinate_system: Optional[CoordinateSystem] = None,
 ) -> Union[Element, List[Element]]:
     """Converts an unstructured_inference LayoutElement object to an unstructured Element."""
 
     if isinstance(layout_element, Element):
         return layout_element
 
@@ -48,33 +74,46 @@
         layout_dict = layout_element
 
     text = layout_dict.get("text")
     # Both `coordinates` and `coordinate_system` must be present
     # in order to add coordinates metadata to the element.
     coordinates = layout_dict.get("coordinates")
     element_type = layout_dict.get("type")
+    print("element_type", element_type)
     if element_type == "List":
         return layout_list_to_list_items(
             text,
             coordinates=coordinates,
             coordinate_system=coordinate_system,
         )
     elif element_type in TYPE_TO_TEXT_ELEMENT_MAP:
         _element_class = TYPE_TO_TEXT_ELEMENT_MAP[element_type]
         return _element_class(
             text=text,
             coordinates=coordinates,
             coordinate_system=coordinate_system,
         )
     elif element_type == "Checked":
-        return CheckBox(checked=True, coordinates=coordinates, coordinate_system=coordinate_system)
+        return CheckBox(
+            checked=True,
+            coordinates=coordinates,
+            coordinate_system=coordinate_system,
+        )
     elif element_type == "Unchecked":
-        return CheckBox(checked=False, coordinates=coordinates, coordinate_system=coordinate_system)
+        return CheckBox(
+            checked=False,
+            coordinates=coordinates,
+            coordinate_system=coordinate_system,
+        )
     else:
-        return Text(text=text, coordinates=coordinates, coordinate_system=coordinate_system)
+        return Text(
+            text=text,
+            coordinates=coordinates,
+            coordinate_system=coordinate_system,
+        )
 
 
 def layout_list_to_list_items(
     text: str,
     coordinates: Tuple[Tuple[float, float], ...],
     coordinate_system: Optional[CoordinateSystem],
 ) -> List[Element]:
@@ -275,10 +314,14 @@
             plain text string (False)
 
     Returns:
         str: An table string representation of the input table.
     """
     fmt = "html" if as_html else "plain"
     rows = list(table.rows)
-    headers = [cell.text for cell in rows[0].cells]
-    data = [[cell.text for cell in row.cells] for row in rows[1:]]
-    return tabulate(data, headers=headers, tablefmt=fmt)
+    if len(rows) > 0:
+        headers = [cell.text for cell in rows[0].cells]
+        data = [[cell.text for cell in row.cells] for row in rows[1:]]
+        table_text = tabulate(data, headers=headers, tablefmt=fmt)
+    else:
+        table_text = ""
+    return table_text
```

### Comparing `unstructured-0.8.4/unstructured/partition/csv.py` & `unstructured-0.8.5/unstructured/partition/csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,50 +7,66 @@
 from unstructured.documents.elements import (
     Element,
     ElementMetadata,
     Table,
     process_metadata,
 )
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
+from unstructured.partition.common import (
+    exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
+    spooled_to_bytes_io_if_needed,
+)
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.CSV)
 def partition_csv(
     filename: Optional[str] = None,
     file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
     include_metadata: bool = True,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft Excel Documents in .csv format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
+    metadata_filename
+        The filename to use for the metadata.
+    metadata_date
+        The last modified date for the document.
     include_metadata
         Determines whether or not metadata is included in the output.
     """
     exactly_one(filename=filename, file=file)
 
     if filename:
         table = pd.read_csv(filename)
-    else:
-        f = spooled_to_bytes_io_if_needed(cast(Union[BinaryIO, SpooledTemporaryFile], file))
+        last_modification_date = get_last_modified_date(filename)
+
+    elif file:
+        last_modification_date = get_last_modified_date_from_file(file)
+        f = spooled_to_bytes_io_if_needed(
+            cast(Union[BinaryIO, SpooledTemporaryFile], file),
+        )
         table = pd.read_csv(f)
 
     html_text = table.to_html(index=False, header=False, na_rep="")
     text = lxml.html.document_fromstring(html_text).text_content()
 
     if include_metadata:
         metadata = ElementMetadata(
             text_as_html=html_text,
             filename=metadata_filename or filename,
+            date=metadata_date or last_modification_date,
         )
     else:
         metadata = ElementMetadata()
 
     return [Table(text=text, metadata=metadata)]
```

### Comparing `unstructured-0.8.4/unstructured/partition/doc.py` & `unstructured-0.8.5/unstructured/partition/doc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 import os
 import tempfile
 from typing import IO, List, Optional
 
 from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.common import convert_office_doc, exactly_one
+from unstructured.partition.common import (
+    convert_office_doc,
+    exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
+)
 from unstructured.partition.docx import partition_docx
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.DOC)
 def partition_doc(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = True,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
     libre_office_filter: Optional[str] = "MS Word 2007 XML",
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft Word Documents in .doc format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
+    metadata_date
+        The last modified date for the document.
     libre_office_filter
         The filter to use when coverting to .doc. The default is the
         filter that is required when using LibreOffice7. Pass in None
         if you do not want to apply any filter.
     """
     # Verify that only one of the arguments was provided
     if filename is None:
@@ -38,35 +46,41 @@
     exactly_one(filename=filename, file=file)
 
     if len(filename) > 0:
         _, filename_no_path = os.path.split(os.path.abspath(filename))
         base_filename, _ = os.path.splitext(filename_no_path)
         if not os.path.exists(filename):
             raise ValueError(f"The file {filename} does not exist.")
+
+        last_modification_date = get_last_modified_date(filename)
+
     elif file is not None:
         tmp = tempfile.NamedTemporaryFile(delete=False)
         tmp.write(file.read())
         tmp.close()
         filename = tmp.name
         _, filename_no_path = os.path.split(os.path.abspath(tmp.name))
         base_filename, _ = os.path.splitext(filename_no_path)
 
+        last_modification_date = get_last_modified_date_from_file(file)
+
     with tempfile.TemporaryDirectory() as tmpdir:
         convert_office_doc(
             filename,
             tmpdir,
             target_format="docx",
             target_filter=libre_office_filter,
         )
         docx_filename = os.path.join(tmpdir, f"{base_filename}.docx")
         elements = partition_docx(
             filename=docx_filename,
             metadata_filename=metadata_filename,
             include_page_breaks=include_page_breaks,
             include_metadata=include_metadata,
+            metadata_date=metadata_date or last_modification_date,
         )
         # remove tmp.name from filename if parsing file
         if file:
             for element in elements:
                 element.metadata.filename = metadata_filename
 
     return elements
```

### Comparing `unstructured-0.8.4/unstructured/partition/docx.py` & `unstructured-0.8.5/unstructured/partition/docx.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     Title,
     process_metadata,
 )
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import (
     convert_ms_office_table_to_text,
     exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
     spooled_to_bytes_io_if_needed,
 )
 from unstructured.partition.text_type import (
     is_bulleted_text,
     is_possible_narrative_text,
     is_possible_title,
     is_us_city_state_zip,
@@ -107,36 +109,45 @@
 @add_metadata_with_filetype(FileType.DOCX)
 def partition_docx(
     filename: Optional[str] = None,
     file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
     include_page_breaks: bool = True,
     include_metadata: bool = True,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft Word Documents in .docx format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     metadata_filename
         The filename to use for the metadata. Relevant because partition_doc converts the
         document to .docx before partition. We want the original source filename in the
         metadata.
+    metadata_date
+        The last modified date for the document.
     """
 
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file)
 
+    last_modification_date = None
     if filename is not None:
+        if not filename.startswith("/tmp"):
+            last_modification_date = get_last_modified_date(filename)
+
         document = docx.Document(filename)
     elif file is not None:
+        last_modification_date = get_last_modified_date_from_file(file)
+
         document = docx.Document(
             spooled_to_bytes_io_if_needed(
                 cast(Union[BinaryIO, SpooledTemporaryFile], file),
             ),
         )
 
     elements: List[Element] = []
@@ -157,26 +168,28 @@
             text_table = convert_ms_office_table_to_text(table, as_html=False)
             element = Table(text_table)
             if element is not None:
                 element.metadata = ElementMetadata(
                     text_as_html=html_table,
                     filename=metadata_filename,
                     page_number=page_number,
+                    date=metadata_date or last_modification_date,
                 )
                 elements.append(element)
             table_index += 1
         elif element_item.tag.endswith("p"):
             if "<w:numPr>" in element_item.xml:
                 is_list = True
             paragraph = docx.text.paragraph.Paragraph(element_item, document)
             para_element: Optional[Text] = _paragraph_to_element(paragraph, is_list)
             if para_element is not None:
                 para_element.metadata = ElementMetadata(
                     filename=metadata_filename,
                     page_number=page_number,
+                    date=metadata_date or last_modification_date,
                 )
                 elements.append(para_element)
             is_list = False
         elif element_item.tag.endswith("sectPr"):
             if len(headers_and_footers) > section:
                 footers = headers_and_footers[section][1]
                 elements.extend(footers)
@@ -295,14 +308,15 @@
 
 def convert_and_partition_docx(
     source_format: str,
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
 ) -> List[Element]:
     """Converts a document to DOCX and then partitions it using partition_html. Works with
     any file format support by pandoc.
 
     Parameters
     ----------
     source_format
@@ -341,10 +355,11 @@
             format=source_format,
             outputfile=docx_filename,
         )
         elements = partition_docx(
             filename=docx_filename,
             metadata_filename=metadata_filename,
             include_metadata=include_metadata,
+            metadata_date=metadata_date,
         )
 
     return elements
```

### Comparing `unstructured-0.8.4/unstructured/partition/email.py` & `unstructured-0.8.5/unstructured/partition/email.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,19 @@
     if ip_address_names and ip_addresses:
         for name, ip in zip(ip_address_names, ip_addresses):
             elements.append(ReceivedInfo(name=name, text=ip))
     if mapi_id:
         elements.append(ReceivedInfo(name="mapi_id", text=mapi_id[0]))
     if datetimetz:
         elements.append(
-            ReceivedInfo(name="received_datetimetz", text=str(datetimetz), datestamp=datetimetz),
+            ReceivedInfo(
+                name="received_datetimetz",
+                text=str(datetimetz),
+                datestamp=datetimetz,
+            ),
         )
     return elements
 
 
 def _parse_email_address(data: str) -> Tuple[str, str]:
     email_address = extract_email_address(data)
 
@@ -100,15 +104,19 @@
             elements += _parse_received_data(item[1])
         else:
             elements.append(MetaData(name=item[0], text=item[1]))
 
     return elements
 
 
-def build_email_metadata(msg: Message, filename: Optional[str]) -> ElementMetadata:
+def build_email_metadata(
+    msg: Message,
+    filename: Optional[str],
+    metadata_date: Optional[str] = None,
+) -> ElementMetadata:
     """Creates an ElementMetadata object from the header information in the email."""
     header_dict = dict(msg.raw_items())
     email_date = header_dict.get("Date")
     if email_date is not None:
         email_date = convert_to_iso_8601(email_date)
 
     sent_from = header_dict.get("From")
@@ -119,25 +127,27 @@
     if sent_to is not None:
         sent_to = [recipient.strip() for recipient in sent_to.split(",")]
 
     return ElementMetadata(
         sent_to=sent_to,
         sent_from=sent_from,
         subject=header_dict.get("Subject"),
-        date=email_date,
+        date=metadata_date or email_date,
         filename=filename,
     )
 
 
 def convert_to_iso_8601(time: str) -> Optional[str]:
     """Converts the datetime from the email output to ISO-8601 format."""
     cleaned_time = clean_extra_whitespace(time)
     regex_match = EMAIL_DATETIMETZ_PATTERN_RE.search(cleaned_time)
     if regex_match is None:
-        logger.warning(f"{time} did not match RFC-2822 format. Unable to extract the time.")
+        logger.warning(
+            f"{time} did not match RFC-2822 format. Unable to extract the time.",
+        )
         return None
 
     start, end = regex_match.span()
     dt_string = cleaned_time[start:end]
     datetime_object = datetime.datetime.strptime(dt_string, "%a, %d %b %Y %H:%M:%S %z")
     return datetime_object.isoformat()
 
@@ -157,15 +167,17 @@
                 attachment_info = {}
 
                 if item.lower() == "attachment":
                     continue
                 key, value = item.split("=")
                 key = clean_extra_whitespace(key.replace('"', ""))
                 value = clean_extra_whitespace(value.replace('"', ""))
-                attachment_info[clean_extra_whitespace(key)] = clean_extra_whitespace(value)
+                attachment_info[clean_extra_whitespace(key)] = clean_extra_whitespace(
+                    value,
+                )
             attachment_info["payload"] = part.get_payload(decode=True)
             list_attachments.append(attachment_info)
 
             for attachment in list_attachments:
                 if output_dir:
                     filename = output_dir + "/" + attachment["filename"]
                     with open(filename, "wb") as f:
@@ -226,14 +238,15 @@
     text: Optional[str] = None,
     content_source: str = "text/html",
     encoding: Optional[str] = None,
     include_headers: bool = False,
     max_partition: Optional[int] = 1500,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
     process_attachments: bool = False,
     attachment_partitioner: Optional[Callable] = None,
     min_partition: Optional[int] = 0,
     **kwargs,
 ) -> List[Element]:
     """Partitions an .eml documents into its constituent elements.
     Parameters
@@ -250,14 +263,16 @@
     encoding
         The encoding method used to decode the text input. If None, utf-8 will be used.
     max_partition
         The maximum number of characters to include in a partition. If None is passed,
         no maximum is applied. Only applies if processing the text/plain content.
     metadata_filename
         The filename to use for the metadata.
+    metadata_date
+        The last modified date for the document.
     process_attachments
         If True, partition_email will process email attachments in addition to
         processing the content of the email itself.
     attachment_partitioner
         The partitioning function to use to process attachments.
     min_partition
         The minimum number of characters to include in a partition. Only applies if
@@ -276,15 +291,18 @@
     exactly_one(filename=filename, file=file, text=text)
     detected_encoding = "utf-8"
     if filename is not None:
         extracted_encoding, msg = parse_email(filename=filename)
         if extracted_encoding:
             detected_encoding = extracted_encoding
         else:
-            detected_encoding, file_text = read_txt_file(filename=filename, encoding=encoding)
+            detected_encoding, file_text = read_txt_file(
+                filename=filename,
+                encoding=encoding,
+            )
             msg = email.message_from_string(file_text)
     elif file is not None:
         extracted_encoding, msg = parse_email(file=file)
         if extracted_encoding:
             detected_encoding = extracted_encoding
         else:
             detected_encoding, file_text = read_txt_file(file=file, encoding=encoding)
@@ -321,28 +339,34 @@
         elements = partition_html(
             text=content,
             include_metadata=False,
             metadata_filename=metadata_filename,
         )
         for element in elements:
             if isinstance(element, Text):
-                _replace_mime_encodings = partial(replace_mime_encodings, encoding=encoding)
+                _replace_mime_encodings = partial(
+                    replace_mime_encodings,
+                    encoding=encoding,
+                )
                 try:
                     element.apply(_replace_mime_encodings)
                 except (UnicodeDecodeError, UnicodeError):
                     # If decoding fails, try decoding through common encodings
                     common_encodings = []
                     for x in COMMON_ENCODINGS:
                         _x = format_encoding_str(x)
                         if _x != encoding:
                             common_encodings.append(_x)
 
                     for enc in common_encodings:
                         try:
-                            _replace_mime_encodings = partial(replace_mime_encodings, encoding=enc)
+                            _replace_mime_encodings = partial(
+                                replace_mime_encodings,
+                                encoding=enc,
+                            )
                             element.apply(_replace_mime_encodings)
                             break
                         except (UnicodeDecodeError, UnicodeError):
                             continue
 
     elif content_source == "text/plain":
         elements = partition_text(
@@ -361,15 +385,19 @@
             elements.insert(idx + 1, image_info)
 
     header: List[Element] = []
     if include_headers:
         header = partition_email_header(msg)
     all_elements = header + elements
 
-    metadata = build_email_metadata(msg, filename=metadata_filename or filename)
+    metadata = build_email_metadata(
+        msg,
+        filename=metadata_filename or filename,
+        metadata_date=metadata_date,
+    )
     for element in all_elements:
         element.metadata = metadata
 
     if process_attachments:
         with TemporaryDirectory() as tmpdir:
             extract_attachment_info(msg, tmpdir)
             attached_files = os.listdir(tmpdir)
```

### Comparing `unstructured-0.8.4/unstructured/partition/epub.py` & `unstructured-0.8.5/unstructured/partition/org.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from typing import IO, List, Optional
 
-from unstructured.documents.elements import Element, process_metadata
+from unstructured.documents.elements import Element
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.html import convert_and_partition_html
 
 
-@process_metadata()
-@add_metadata_with_filetype(FileType.EPUB)
-def partition_epub(
+@add_metadata_with_filetype(FileType.ORG)
+def partition_org(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    **kwargs,
+    metadata_date: Optional[str] = None,
 ) -> List[Element]:
-    """Partitions an EPUB document. The document is first converted to HTML and then
-    partitoned using partiton_html.
+    """Partitions an org document. The document is first converted to HTML and then
+    partitioned using partition_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
-        If True, the output will include page breaks if the filetype supports it.
+        If True, the output will include page breaks if the filetype supports it
+    metadata_date
+        The last modified date for the document.
     """
     return convert_and_partition_html(
-        source_format="epub",
+        source_format="org",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
         metadata_filename=metadata_filename,
+        metadata_date=metadata_date,
     )
```

### Comparing `unstructured-0.8.4/unstructured/partition/html.py` & `unstructured-0.8.5/unstructured/partition/html.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from unstructured.file_utils.filetype import (
     FileType,
     add_metadata_with_filetype,
     document_to_element_list,
 )
 from unstructured.partition.common import (
     exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
 )
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.HTML)
 def partition_html(
     filename: Optional[str] = None,
@@ -28,14 +30,15 @@
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     headers: Dict[str, str] = {},
     ssl_verify: bool = True,
     parser: VALID_PARSERS = None,
     html_assemble_articles: bool = False,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an HTML document into its constituent elements.
 
     Parameters
     ----------
     filename
@@ -56,29 +59,34 @@
     headers
         The headers to be used in conjunction with the HTTP request if URL is set.
     ssl_verify
         If the URL parameter is set, determines whether or not partition uses SSL verification
         in the HTTP request.
     parser
         The parser to use for parsing the HTML document. If None, default parser will be used.
+    metadata_date
+        The last modified date for the document.
     """
     if text is not None and text.strip() == "" and not file and not filename and not url:
         return []
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file, text=text, url=url)
 
+    last_modification_date = None
     if filename is not None:
+        last_modification_date = get_last_modified_date(filename)
         document = HTMLDocument.from_file(
             filename,
             parser=parser,
             encoding=encoding,
             assemble_articles=html_assemble_articles,
         )
 
     elif file is not None:
+        last_modification_date = get_last_modified_date_from_file(file)
         _, file_text = read_txt_file(file=file, encoding=encoding)
         document = HTMLDocument.from_string(
             file_text,
             parser=parser,
             assemble_articles=html_assemble_articles,
         )
 
@@ -97,23 +105,28 @@
 
         content_type = response.headers.get("Content-Type", "")
         if not content_type.startswith("text/html"):
             raise ValueError(f"Expected content type text/html. Got {content_type}.")
 
         document = HTMLDocument.from_string(response.text, parser=parser)
 
-    return document_to_element_list(document, include_page_breaks=include_page_breaks)
+    return document_to_element_list(
+        document,
+        include_page_breaks=include_page_breaks,
+        last_modification_date=metadata_date or last_modification_date,
+    )
 
 
 def convert_and_partition_html(
     source_format: str,
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
 ) -> List[Element]:
     """Converts a document to HTML and then partitions it using partition_html. Works with
     any file format support by pandoc.
 
     Parameters
     ----------
     source_format
@@ -122,17 +135,30 @@
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, the output will include page breaks if the filetype supports it.
     metadata_filename
         The filename to use in element metadata.
+    last_modication_date
+        The last modified date for the document.
     """
-    html_text = convert_file_to_html_text(source_format=source_format, filename=filename, file=file)
+
+    last_modification_date = None
+    if filename:
+        last_modification_date = get_last_modified_date(filename)
+    elif file:
+        last_modification_date = get_last_modified_date_from_file(file)
+    html_text = convert_file_to_html_text(
+        source_format=source_format,
+        filename=filename,
+        file=file,
+    )
     # NOTE(robinson) - pypandoc returns a text string with unicode encoding
     # ref: https://github.com/JessicaTegner/pypandoc#usage
     return partition_html(
         text=html_text,
         include_page_breaks=include_page_breaks,
         encoding="unicode",
         metadata_filename=metadata_filename,
+        metadata_date=metadata_date or last_modification_date,
     )
```

### Comparing `unstructured-0.8.4/unstructured/partition/image.py` & `unstructured-0.8.5/unstructured/partition/image.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,40 +6,56 @@
 
 
 @process_metadata()
 def partition_image(
     filename: str = "",
     file: Optional[bytes] = None,
     include_page_breaks: bool = False,
+    infer_table_structure: bool = False,
     ocr_languages: str = "eng",
     strategy: str = "auto",
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Parses an image into a list of interpreted elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object as bytes --> open(filename, "rb").
+    include_page_breaks
+        If True, includes page breaks at the end of each page in the document.
+    infer_table_structure
+        Only applicable if `strategy=hi_res`.
+        If True, any Table elements that are extracted will also have a metadata field
+        named "text_as_html" where the table's text content is rendered into an html string.
+        I.e., rows and cells are preserved.
+        Whether True or False, the "text" field is always present in any Table element
+        and is the text content of the table (no structure).
     ocr_languages
         The languages to use for the Tesseract agent. To use a language, you'll first need
         to install the appropriate Tesseract language pack.
     strategy
         The strategy to use for partitioning the image. Valid strategies are "hi_res" and
         "ocr_only". When using the "hi_res" strategy, the function uses a layout detection
         model if to identify document elements. When using the "ocr_only" strategy,
         partition_image simply extracts the text from the document using OCR and processes it.
         The default strategy `auto` will determine when a image can be extracted using
         `ocr_only` mode, otherwise it will fall back to `hi_res`.
+    metadata_date
+        The last modified date for the document.
+
     """
     exactly_one(filename=filename, file=file)
 
     return partition_pdf_or_image(
         filename=filename,
         file=file,
         is_image=True,
         include_page_breaks=include_page_breaks,
+        infer_table_structure=infer_table_structure,
         ocr_languages=ocr_languages,
         strategy=strategy,
+        metadata_date=metadata_date,
     )
```

### Comparing `unstructured-0.8.4/unstructured/partition/json.py` & `unstructured-0.8.5/unstructured/partition/json.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,65 +3,80 @@
 
 from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import (
     FileType,
     add_metadata_with_filetype,
     is_json_processable,
 )
-from unstructured.partition.common import exactly_one
+from unstructured.partition.common import (
+    exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
+)
 from unstructured.staging.base import dict_to_elements
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.JSON)
 def partition_json(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     text: Optional[str] = None,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an .json document into its constituent elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object as bytes --> open(filename, "rb").
     text
         The string representation of the .json document.
+    metadata_date
+        The last modified date for the document.
     """
     if text is not None and text.strip() == "" and not file and not filename:
         return []
 
     exactly_one(filename=filename, file=file, text=text)
 
+    last_modification_date = None
     if filename is not None:
+        last_modification_date = get_last_modified_date(filename)
         with open(filename, encoding="utf8") as f:
             file_text = f.read()
+
     elif file is not None:
+        last_modification_date = get_last_modified_date_from_file(file)
+
         file_content = file.read()
         if isinstance(file_content, str):
             file_text = file_content
         else:
             file_text = file_content.decode()
         file.seek(0)
+
     elif text is not None:
         file_text = str(text)
 
     if not is_json_processable(file_text=file_text):
         raise ValueError(
             "JSON cannot be partitioned. Schema does not match the Unstructured schema.",
         )
 
     try:
         dict = json.loads(file_text)
         elements = dict_to_elements(dict)
     except json.JSONDecodeError:
         raise ValueError("Not a valid json")
 
+    for element in elements:
+        element.metadata.date = metadata_date or last_modification_date
     # NOTE(Nathan): in future PR, try extracting items that look like text
     #               if file_text is a valid json but not an unstructured json
 
     return elements
```

### Comparing `unstructured-0.8.4/unstructured/partition/md.py` & `unstructured-0.8.5/unstructured/partition/rtf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,40 @@
-from typing import IO, List, Optional, Union
-
-import markdown
-import requests
+from typing import IO, List, Optional
 
 from unstructured.documents.elements import Element, process_metadata
-from unstructured.documents.xml import VALID_PARSERS
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.common import exactly_one
-from unstructured.partition.html import partition_html
-
-
-def optional_decode(contents: Union[str, bytes]) -> str:
-    if isinstance(contents, bytes):
-        return contents.decode("utf-8")
-    return contents
+from unstructured.partition.html import convert_and_partition_html
 
 
 @process_metadata()
-@add_metadata_with_filetype(FileType.MD)
-def partition_md(
+@add_metadata_with_filetype(FileType.RTF)
+def partition_rtf(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
-    text: Optional[str] = None,
-    url: Optional[str] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
-    parser: VALID_PARSERS = None,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
-    """Partitions a markdown file into its constituent elements
+    """Partitions an RTF document. The document is first converted to HTML and then
+    partitioned using partiton_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
-    text
-        The string representation of the markdown document.
-    url
-        The URL of a webpage to parse. Only for URLs that return a markdown document.
     include_page_breaks
-        If True, the output will include page breaks if the filetype supports it.
-    include_metadata
-        Determines whether or not metadata is included in the output.
-    parser
-        The parser to use for parsing the markdown document. If None, default parser will be used.
+        If True, the output will include page breaks if the filetype supports it
+    metadata_date
+        The last modified date for the document.
     """
-    # Verify that only one of the arguments was provided
-    if text is None:
-        text = ""
-    exactly_one(filename=filename, file=file, text=text, url=url)
-
-    if filename is not None:
-        with open(filename, encoding="utf8") as f:
-            text = optional_decode(f.read())
-
-    elif file is not None:
-        text = optional_decode(file.read())
-
-    elif url is not None:
-        response = requests.get(url)
-        if not response.ok:
-            raise ValueError(f"URL return an error: {response.status_code}")
-
-        content_type = response.headers.get("Content-Type", "")
-        if not content_type.startswith("text/markdown"):
-            raise ValueError(f"Expected content type text/markdown. Got {content_type}.")
-
-        text = response.text
-
-    html = markdown.markdown(text)
-
-    return partition_html(
-        text=html,
+    return convert_and_partition_html(
+        source_format="rtf",
+        filename=filename,
+        file=file,
         include_page_breaks=include_page_breaks,
-        include_metadata=include_metadata,
-        parser=parser,
         metadata_filename=metadata_filename,
+        metadata_date=metadata_date,
     )
```

### Comparing `unstructured-0.8.4/unstructured/partition/msg.py` & `unstructured-0.8.5/unstructured/partition/msg.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 @add_metadata_with_filetype(FileType.MSG)
 def partition_msg(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     max_partition: Optional[int] = 1500,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
     process_attachments: bool = False,
     attachment_partitioner: Optional[Callable] = None,
     min_partition: Optional[int] = 0,
     **kwargs,
 ) -> List[Element]:
     """Partitions a MSFT Outlook .msg file
 
@@ -39,14 +40,16 @@
     metadata_filename
         The filename to use for the metadata.
     process_attachments
         If True, partition_email will process email attachments in addition to
         processing the content of the email itself.
     attachment_partitioner
         The partitioning function to use to process attachments.
+    metadata_date
+        The last modified date for the document.
     min_partition
         The minimum number of characters to include in a partition. Only applies if
         processing text/plain content.
     """
     exactly_one(filename=filename, file=file)
 
     if filename is not None:
@@ -63,15 +66,19 @@
     else:
         elements = partition_text(
             text=text,
             max_partition=max_partition,
             min_partition=min_partition,
         )
 
-    metadata = build_msg_metadata(msg_obj, metadata_filename or filename)
+    metadata = build_msg_metadata(
+        msg_obj,
+        metadata_filename or filename,
+        metadata_date=metadata_date,
+    )
     for element in elements:
         element.metadata = metadata
 
     if process_attachments:
         with tempfile.TemporaryDirectory() as tmpdir:
             extract_msg_attachment_info(msg_obj=msg_obj, output_dir=tmpdir)
             attached_files = os.listdir(tmpdir)
@@ -87,15 +94,19 @@
                     element.metadata.file_directory = None
                     element.metadata.attached_to_filename = metadata_filename or filename
                     elements.append(element)
 
     return elements
 
 
-def build_msg_metadata(msg_obj: msg_parser.MsOxMessage, filename: Optional[str]) -> ElementMetadata:
+def build_msg_metadata(
+    msg_obj: msg_parser.MsOxMessage,
+    filename: Optional[str],
+    metadata_date: Optional[str],
+) -> ElementMetadata:
     """Creates an ElementMetadata object from the header information in the email."""
     email_date = getattr(msg_obj, "sent_date", None)
     if email_date is not None:
         email_date = convert_to_iso_8601(email_date)
 
     sent_from = getattr(msg_obj, "sender", None)
     if sent_from is not None:
@@ -105,15 +116,15 @@
     if sent_to is not None:
         sent_to = [str(recipient) for recipient in sent_to]
 
     return ElementMetadata(
         sent_to=sent_to,
         sent_from=sent_from,
         subject=getattr(msg_obj, "subject", None),
-        date=email_date,
+        date=metadata_date or email_date,
         filename=filename,
     )
 
 
 def extract_msg_attachment_info(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
```

### Comparing `unstructured-0.8.4/unstructured/partition/odt.py` & `unstructured-0.8.5/unstructured/partition/epub.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 from typing import IO, List, Optional
 
 from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.docx import convert_and_partition_docx
+from unstructured.partition.html import convert_and_partition_html
 
 
 @process_metadata()
-@add_metadata_with_filetype(FileType.ODT)
-def partition_odt(
+@add_metadata_with_filetype(FileType.EPUB)
+def partition_epub(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
+    include_page_breaks: bool = False,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
-    """Partitions Open Office Documents in .odt format into its document elements.
+    """Partitions an EPUB document. The document is first converted to HTML and then
+    partitoned using partiton_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
+    include_page_breaks
+        If True, the output will include page breaks if the filetype supports it
+    metadata_date
+        The last modified date for the document.
+
     """
-    return convert_and_partition_docx(
-        source_format="odt",
+    return convert_and_partition_html(
+        source_format="epub",
         filename=filename,
         file=file,
+        include_page_breaks=include_page_breaks,
         metadata_filename=metadata_filename,
+        metadata_date=metadata_date,
     )
```

### Comparing `unstructured-0.8.4/unstructured/partition/org.py` & `unstructured-0.8.5/unstructured/partition/odt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 from typing import IO, List, Optional
 
-from unstructured.documents.elements import Element
+from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.html import convert_and_partition_html
+from unstructured.partition.common import (
+    get_last_modified_date,
+    get_last_modified_date_from_file,
+)
+from unstructured.partition.docx import convert_and_partition_docx
 
 
-@add_metadata_with_filetype(FileType.ORG)
-def partition_org(
+@process_metadata()
+@add_metadata_with_filetype(FileType.ODT)
+def partition_odt(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
-    include_page_breaks: bool = False,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
+    **kwargs,
 ) -> List[Element]:
-    """Partitions an org document. The document is first converted to HTML and then
-    partitioned using partition_html.
+    """Partitions Open Office Documents in .odt format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
-    include_page_breaks
-        If True, the output will include page breaks if the filetype supports it
+    metadata_date
+        The last modified date for the document.
     """
-    return convert_and_partition_html(
-        source_format="org",
+
+    last_modification_date = None
+    if filename:
+        last_modification_date = get_last_modified_date(filename)
+    elif file:
+        last_modification_date = get_last_modified_date_from_file(file)
+
+    return convert_and_partition_docx(
+        source_format="odt",
         filename=filename,
         file=file,
-        include_page_breaks=include_page_breaks,
         metadata_filename=metadata_filename,
+        metadata_date=metadata_date or last_modification_date,
     )
```

### Comparing `unstructured-0.8.4/unstructured/partition/pdf.py` & `unstructured-0.8.5/unstructured/partition/pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     add_metadata_with_filetype,
     document_to_element_list,
 )
 from unstructured.nlp.patterns import PARAGRAPH_PATTERN
 from unstructured.partition.common import (
     convert_to_bytes,
     exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
     spooled_to_bytes_io_if_needed,
 )
 from unstructured.partition.strategies import determine_pdf_or_image_strategy
 from unstructured.partition.text import element_from_text, partition_text
 from unstructured.utils import requires_dependencies
 
 RE_MULTISPACE_INCLUDING_NEWLINES = re.compile(pattern=r"\s+", flags=re.DOTALL)
@@ -45,17 +47,18 @@
     filename: str = "",
     file: Optional[Union[BinaryIO, SpooledTemporaryFile]] = None,
     include_page_breaks: bool = False,
     strategy: str = "auto",
     infer_table_structure: bool = False,
     ocr_languages: str = "eng",
     max_partition: Optional[int] = 1500,
+    min_partition: Optional[int] = 0,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
-    min_partition: Optional[int] = 0,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Parses a pdf document into a list of interpreted elements.
     Parameters
     ----------
     filename
         A string defining the target filename path.
@@ -81,64 +84,87 @@
         to isntall the appropriate Tesseract language pack.
     max_partition
         The maximum number of characters to include in a partition. If None is passed,
         no maximum is applied. Only applies to the "ocr_only" strategy.
     min_partition
         The minimum number of characters to include in a partition. Only applies if
         processing text/plain content.
+    metadata_date
+        The last modified date for the document.
     """
     exactly_one(filename=filename, file=file)
     return partition_pdf_or_image(
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
         strategy=strategy,
         infer_table_structure=infer_table_structure,
         ocr_languages=ocr_languages,
         max_partition=max_partition,
         min_partition=min_partition,
+        metadata_date=metadata_date,
         **kwargs,
     )
 
 
 def extractable_elements(
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     include_page_breaks: bool = False,
+    metadata_date: Optional[str] = None,
 ):
     return _partition_pdf_with_pdfminer(
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
+        metadata_date=metadata_date,
     )
 
 
+def get_the_last_modification_date_pdf_or_img(
+    file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
+    filename: Optional[str] = "",
+) -> Union[str, None]:
+    last_modification_date = None
+    if not file and filename:
+        last_modification_date = get_last_modified_date(filename=filename)
+    elif not filename and file:
+        last_modification_date = get_last_modified_date_from_file(file=file)
+    return last_modification_date
+
+
 def partition_pdf_or_image(
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     is_image: bool = False,
     include_page_breaks: bool = False,
     strategy: str = "auto",
     infer_table_structure: bool = False,
     ocr_languages: str = "eng",
     max_partition: Optional[int] = 1500,
     min_partition: Optional[int] = 0,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Parses a pdf or image document into a list of interpreted elements."""
     # TODO(alan): Extract information about the filetype to be processed from the template
     # route. Decoding the routing should probably be handled by a single function designed for
     # that task so as routing design changes, those changes are implemented in a single
     # function.
 
+    last_modification_date = get_the_last_modification_date_pdf_or_img(
+        file=file,
+        filename=filename,
+    )
     if not is_image:
         extracted_elements = extractable_elements(
             filename=filename,
             file=spooled_to_bytes_io_if_needed(file),
             include_page_breaks=include_page_breaks,
+            metadata_date=metadata_date or last_modification_date,
         )
         pdf_text_extractable = any(
             isinstance(el, Text) and el.text.strip() for el in extracted_elements
         )
     else:
         pdf_text_extractable = False
 
@@ -158,14 +184,15 @@
             layout_elements = _partition_pdf_or_image_local(
                 filename=filename,
                 file=spooled_to_bytes_io_if_needed(file),
                 is_image=is_image,
                 infer_table_structure=infer_table_structure,
                 include_page_breaks=include_page_breaks,
                 ocr_languages=ocr_languages,
+                metadata_date=metadata_date or last_modification_date,
                 **kwargs,
             )
 
     elif strategy == "fast":
         return extracted_elements
 
     elif strategy == "ocr_only":
@@ -175,28 +202,29 @@
                 filename=filename,
                 file=file,
                 include_page_breaks=include_page_breaks,
                 ocr_languages=ocr_languages,
                 is_image=is_image,
                 max_partition=max_partition,
                 min_partition=min_partition,
+                metadata_date=metadata_date or last_modification_date,
             )
-
     return layout_elements
 
 
 @requires_dependencies("unstructured_inference")
 def _partition_pdf_or_image_local(
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO]] = None,
     is_image: bool = False,
     infer_table_structure: bool = False,
     include_page_breaks: bool = False,
     ocr_languages: str = "eng",
     model_name: Optional[str] = None,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partition using package installed locally."""
     from unstructured_inference.inference.layout import (
         process_data_with_model,
         process_file_with_model,
     )
@@ -220,38 +248,48 @@
         layout = process_data_with_model(
             file,
             is_image=is_image,
             ocr_languages=ocr_languages,
             extract_tables=infer_table_structure,
             model_name=model_name,
         )
-    elements = document_to_element_list(layout, include_page_breaks=include_page_breaks, sort=False)
+    elements = document_to_element_list(
+        layout,
+        include_page_breaks=include_page_breaks,
+        sort=False,
+        last_modification_date=metadata_date,
+    )
     out_elements = []
 
     for el in elements:
         if (isinstance(el, PageBreak) and not include_page_breaks) or (
             # NOTE(crag): small chunks of text from Image elements tend to be garbage
             isinstance(el, Image)
             and (el.text is None or len(el.text) < 24 or el.text.find(" ") == -1)
         ):
             continue
         # NOTE(crag): this is probably always a Text object, but check for the sake of typing
         if isinstance(el, Text):
-            el.text = re.sub(RE_MULTISPACE_INCLUDING_NEWLINES, " ", el.text or "").strip()
+            el.text = re.sub(
+                RE_MULTISPACE_INCLUDING_NEWLINES,
+                " ",
+                el.text or "",
+            ).strip()
             if el.text or isinstance(el, PageBreak):
                 out_elements.append(cast(Element, el))
 
     return out_elements
 
 
 @requires_dependencies("pdfminer", "local-inference")
 def _partition_pdf_with_pdfminer(
     filename: str = "",
     file: Optional[BinaryIO] = None,
     include_page_breaks: bool = False,
+    metadata_date: Optional[str] = None,
 ) -> List[Element]:
     """Partitions a PDF using PDFMiner instead of using a layoutmodel. Used for faster
     processing or detectron2 is not available.
 
     Implementation is based on the `extract_text` implemenation in pdfminer.six, but
     modified to support tracking page numbers and working with file-like objects.
 
@@ -261,22 +299,24 @@
     if filename:
         with open_filename(filename, "rb") as fp:
             fp = cast(BinaryIO, fp)
             elements = _process_pdfminer_pages(
                 fp=fp,
                 filename=filename,
                 include_page_breaks=include_page_breaks,
+                metadata_date=metadata_date,
             )
 
     elif file:
         fp = cast(BinaryIO, file)
         elements = _process_pdfminer_pages(
             fp=fp,
             filename=filename,
             include_page_breaks=include_page_breaks,
+            metadata_date=metadata_date,
         )
 
     return elements
 
 
 def _extract_text(item: LTItem) -> str:
     """Recursively extracts text from PDFMiner objects to account
@@ -297,14 +337,15 @@
     return "\n"
 
 
 def _process_pdfminer_pages(
     fp: BinaryIO,
     filename: str = "",
     include_page_breaks: bool = False,
+    metadata_date: Optional[str] = None,
 ):
     """Uses PDF miner to split a document into pages and process them."""
     elements: List[Element] = []
 
     for i, page in enumerate(extract_pages(fp)):  # type: ignore
         width, height = page.width, page.height
 
@@ -339,14 +380,15 @@
                         points=points,
                         system=coordinate_system,
                     )
                     element.metadata = ElementMetadata(
                         filename=filename,
                         page_number=i + 1,
                         coordinates=coordinates_metadata,
+                        date=metadata_date,
                     )
                     page_elements.append(element)
 
         sorted_page_elements = sorted(
             page_elements,
             key=lambda el: (
                 el.metadata.coordinates.points[0][1] if el.metadata.coordinates else float("inf"),
@@ -401,14 +443,15 @@
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     include_page_breaks: bool = False,
     ocr_languages: str = "eng",
     is_image: bool = False,
     max_partition: Optional[int] = 1500,
     min_partition: Optional[int] = 0,
+    metadata_date: Optional[str] = None,
 ):
     """Partitions and image or PDF using Tesseract OCR. For PDFs, each page is converted
     to an image prior to processing."""
     import pytesseract
 
     if is_image:
         if file is not None:
@@ -416,21 +459,27 @@
             text = pytesseract.image_to_string(image, config=f"-l '{ocr_languages}'")
         else:
             text = pytesseract.image_to_string(filename, config=f"-l '{ocr_languages}'")
         elements = partition_text(
             text=text,
             max_partition=max_partition,
             min_partition=min_partition,
+            metadata_date=metadata_date,
         )
+
     else:
         elements = []
         page_number = 0
         for image in convert_pdf_to_images(filename, file):
             page_number += 1
-            metadata = ElementMetadata(filename=filename, page_number=page_number)
+            metadata = ElementMetadata(
+                filename=filename,
+                page_number=page_number,
+                date=metadata_date,
+            )
             text = pytesseract.image_to_string(image, config=f"-l '{ocr_languages}'")
 
             _elements = partition_text(
                 text=text,
                 max_partition=max_partition,
                 min_partition=min_partition,
             )
```

### Comparing `unstructured-0.8.4/unstructured/partition/ppt.py` & `unstructured-0.8.5/unstructured/partition/ppt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 import os
 import tempfile
 from typing import IO, List, Optional
 
 from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.common import convert_office_doc, exactly_one
+from unstructured.partition.common import (
+    convert_office_doc,
+    exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
+)
 from unstructured.partition.pptx import partition_pptx
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.PPT)
 def partition_ppt(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft PowerPoint Documents in .ppt format into their document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, includes a PageBreak element between slides
+    metadata_date
+        The last modified date for the document.
     """
     # Verify that only one of the arguments was provided
     if filename is None:
         filename = ""
     exactly_one(filename=filename, file=file)
 
+    last_modification_date = None
     if len(filename) > 0:
         _, filename_no_path = os.path.split(os.path.abspath(filename))
         base_filename, _ = os.path.splitext(filename_no_path)
         if not os.path.exists(filename):
             raise ValueError(f"The file {filename} does not exist.")
+        last_modification_date = get_last_modified_date(filename)
+
     elif file is not None:
+        last_modification_date = get_last_modified_date_from_file(file)
         tmp = tempfile.NamedTemporaryFile(delete=False)
         tmp.write(file.read())
         tmp.close()
         filename = tmp.name
         _, filename_no_path = os.path.split(os.path.abspath(tmp.name))
 
     base_filename, _ = os.path.splitext(filename_no_path)
@@ -52,15 +64,19 @@
         convert_office_doc(
             filename,
             tmpdir,
             target_format="pptx",
             target_filter="Impress MS PowerPoint 2007 XML",
         )
         pptx_filename = os.path.join(tmpdir, f"{base_filename}.pptx")
-        elements = partition_pptx(filename=pptx_filename, metadata_filename=metadata_filename)
+        elements = partition_pptx(
+            filename=pptx_filename,
+            metadata_filename=metadata_filename,
+            metadata_date=metadata_date or last_modification_date,
+        )
 
     # remove tmp.name from filename if parsing file
     if file:
         for element in elements:
             element.metadata.filename = metadata_filename
 
     return elements
```

### Comparing `unstructured-0.8.4/unstructured/partition/pptx.py` & `unstructured-0.8.5/unstructured/partition/pptx.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     Title,
     process_metadata,
 )
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.partition.common import (
     convert_ms_office_table_to_text,
     exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
     spooled_to_bytes_io_if_needed,
 )
 from unstructured.partition.text_type import (
     is_possible_narrative_text,
     is_possible_title,
 )
 
@@ -32,14 +34,15 @@
 @add_metadata_with_filetype(FileType.PPTX)
 def partition_pptx(
     filename: Optional[str] = None,
     file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     include_page_breaks: bool = True,
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
+    metadata_date: Optional[str] = None,
     include_slide_notes: bool = False,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft PowerPoint Documents in .pptx format into its document elements.
 
     Parameters
     ----------
@@ -49,33 +52,44 @@
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, includes a PageBreak element between slides
     metadata_filename
         The filename to use for the metadata. Relevant because partition_ppt converts the
         document .pptx before partition. We want the original source filename in the
         metadata.
+    metadata_date
+        The last modified date for the document.
+
+
     include_slide_notes
         If True, includes the slide notes as element
     """
 
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file)
-
+    last_modification_date = None
     if filename is not None:
+        if not filename.startswith("/tmp"):
+            last_modification_date = get_last_modified_date(filename)
+
         presentation = pptx.Presentation(filename)
     elif file is not None:
+        last_modification_date = get_last_modified_date_from_file(file)
         presentation = pptx.Presentation(
-            spooled_to_bytes_io_if_needed(cast(Union[BinaryIO, SpooledTemporaryFile], file)),
+            spooled_to_bytes_io_if_needed(
+                cast(Union[BinaryIO, SpooledTemporaryFile], file),
+            ),
         )
 
     elements: List[Element] = []
     metadata = ElementMetadata(filename=metadata_filename or filename)
     num_slides = len(presentation.slides)
     for i, slide in enumerate(presentation.slides):
         metadata = ElementMetadata.from_dict(metadata.to_dict())
+        metadata.date = metadata_date or last_modification_date
         metadata.page_number = i + 1
         if include_slide_notes and slide.has_notes_slide is True:
             notes_slide = slide.notes_slide
             if notes_slide.notes_text_frame is not None:
                 notes_text_frame = notes_slide.notes_text_frame
                 notes_text = notes_text_frame.text
                 if notes_text.strip() != "":
@@ -87,14 +101,15 @@
                 html_table = convert_ms_office_table_to_text(table, as_html=True)
                 text_table = convert_ms_office_table_to_text(table, as_html=False)
                 if (text_table := text_table.strip()) != "":
                     metadata = ElementMetadata(
                         filename=metadata_filename or filename,
                         text_as_html=html_table,
                         page_number=metadata.page_number,
+                        date=metadata_date or last_modification_date,
                     )
                     elements.append(Table(text=text_table, metadata=metadata))
                 continue
             if not shape.has_text_frame:
                 continue
             # NOTE(robinson) - avoid processing shapes that are not on the actual slide
             # NOTE - skip check if no top or left position (shape displayed top left)
```

### Comparing `unstructured-0.8.4/unstructured/partition/rst.py` & `unstructured-0.8.5/unstructured/partition/rst.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,28 +9,32 @@
 @add_metadata_with_filetype(FileType.RST)
 def partition_rst(
     filename: Optional[str] = None,
     file: Optional[IO[bytes]] = None,
     include_page_breaks: bool = False,
     include_metadata: bool = True,
     metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an RST document. The document is first converted to HTML and then
     partitioned using partition_html.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_page_breaks
         If True, the output will include page breaks if the filetype supports it.
+    metadata_date
+        The last modified date for the document.
     """
     return convert_and_partition_html(
         source_format="rst",
         filename=filename,
         file=file,
         include_page_breaks=include_page_breaks,
         metadata_filename=metadata_filename,
+        metadata_date=metadata_date,
     )
```

### Comparing `unstructured-0.8.4/unstructured/partition/strategies.py` & `unstructured-0.8.5/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/partition/text.py` & `unstructured-0.8.5/unstructured/partition/text.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,19 @@
     Title,
     process_metadata,
 )
 from unstructured.file_utils.encoding import read_txt_file
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
 from unstructured.nlp.patterns import PARAGRAPH_PATTERN
 from unstructured.nlp.tokenize import sent_tokenize
-from unstructured.partition.common import exactly_one
+from unstructured.partition.common import (
+    exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
+)
 from unstructured.partition.text_type import (
     is_bulleted_text,
     is_possible_narrative_text,
     is_possible_title,
     is_us_city_state_zip,
 )
 
@@ -154,14 +158,15 @@
     text: Optional[str] = None,
     encoding: Optional[str] = None,
     paragraph_grouper: Optional[Callable[[str], str]] = None,
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
     max_partition: Optional[int] = 1500,
     min_partition: Optional[int] = 0,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an .txt documents into its constituent paragraph elements.
     If paragraphs are below "min_partition" or above "max_partition" boundaries,
     they are combined or split.
     Parameters
     ----------
@@ -179,33 +184,38 @@
     include_metadata
         Determines whether or not metadata is included in the output.
     max_partition
         The maximum number of characters to include in a partition. If None is passed,
         no maximum is applied.
     min_partition
         The minimum number of characters to include in a partition.
+    metadata_date
+        The day of the last modification
     """
     if text is not None and text.strip() == "" and not file and not filename:
         return []
 
     if (
         min_partition is not None
         and max_partition is not None
         and (min_partition > max_partition or min_partition < 0 or max_partition < 0)
     ):
         raise ValueError("Invalid values for min_partition and/or max_partition.")
 
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file, text=text)
 
+    last_modification_date = None
     if filename is not None:
         encoding, file_text = read_txt_file(filename=filename, encoding=encoding)
+        last_modification_date = get_last_modified_date(filename)
 
     elif file is not None:
         encoding, file_text = read_txt_file(file=file, encoding=encoding)
+        last_modification_date = get_last_modified_date_from_file(file)
 
     elif text is not None:
         file_text = str(text)
 
     if paragraph_grouper is False:
         pass
     elif paragraph_grouper is not None:
@@ -232,15 +242,18 @@
                 content=paragraph,
                 max_partition=max_partition,
             ),
         )
 
     elements: List[Element] = []
     metadata = (
-        ElementMetadata(filename=metadata_filename or filename)
+        ElementMetadata(
+            filename=metadata_filename or filename,
+            date=metadata_date or last_modification_date,
+        )
         if include_metadata
         else ElementMetadata()
     )
     for ctext in file_content:
         ctext = ctext.strip()
 
         if ctext:
@@ -259,18 +272,30 @@
     if is_bulleted_text(text):
         return ListItem(
             text=clean_bullets(text),
             coordinates=coordinates,
             coordinate_system=coordinate_system,
         )
     elif is_us_city_state_zip(text):
-        return Address(text=text, coordinates=coordinates, coordinate_system=coordinate_system)
+        return Address(
+            text=text,
+            coordinates=coordinates,
+            coordinate_system=coordinate_system,
+        )
     elif is_possible_narrative_text(text):
         return NarrativeText(
             text=text,
             coordinates=coordinates,
             coordinate_system=coordinate_system,
         )
     elif is_possible_title(text):
-        return Title(text=text, coordinates=coordinates, coordinate_system=coordinate_system)
+        return Title(
+            text=text,
+            coordinates=coordinates,
+            coordinate_system=coordinate_system,
+        )
     else:
-        return Text(text=text, coordinates=coordinates, coordinate_system=coordinate_system)
+        return Text(
+            text=text,
+            coordinates=coordinates,
+            coordinate_system=coordinate_system,
+        )
```

### Comparing `unstructured-0.8.4/unstructured/partition/text_type.py` & `unstructured-0.8.5/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/partition/tsv.py` & `unstructured-0.8.5/unstructured/partition/md.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,95 @@
-from tempfile import SpooledTemporaryFile
-from typing import IO, BinaryIO, List, Optional, Union, cast
+from typing import IO, List, Optional, Union
 
-import lxml.html
-import pandas as pd
+import markdown
+import requests
 
-from unstructured.documents.elements import (
-    Element,
-    ElementMetadata,
-    Table,
-    process_metadata,
-)
+from unstructured.documents.elements import Element, process_metadata
+from unstructured.documents.xml import VALID_PARSERS
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
+from unstructured.partition.common import (
+    exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
+)
+from unstructured.partition.html import partition_html
+
+
+def optional_decode(contents: Union[str, bytes]) -> str:
+    if isinstance(contents, bytes):
+        return contents.decode("utf-8")
+    return contents
 
 
 @process_metadata()
-@add_metadata_with_filetype(FileType.TSV)
-def partition_tsv(
+@add_metadata_with_filetype(FileType.MD)
+def partition_md(
     filename: Optional[str] = None,
-    file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
-    metadata_filename: Optional[str] = None,
+    file: Optional[IO[bytes]] = None,
+    text: Optional[str] = None,
+    url: Optional[str] = None,
+    include_page_breaks: bool = False,
     include_metadata: bool = True,
+    parser: VALID_PARSERS = None,
+    metadata_filename: Optional[str] = None,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
-    """Partitions TSV files into document elements.
+    """Partitions a markdown file into its constituent elements
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
+    text
+        The string representation of the markdown document.
+    url
+        The URL of a webpage to parse. Only for URLs that return a markdown document.
+    include_page_breaks
+        If True, the output will include page breaks if the filetype supports it.
     include_metadata
         Determines whether or not metadata is included in the output.
+    parser
+        The parser to use for parsing the markdown document. If None, default parser will be used.
+    metadata_date
+        The last modified date for the document.
     """
-    exactly_one(filename=filename, file=file)
-
-    if filename:
-        table = pd.read_csv(filename, sep="\t")
-    else:
-        f = spooled_to_bytes_io_if_needed(cast(Union[BinaryIO, SpooledTemporaryFile], file))
-        table = pd.read_csv(f, sep="\t")
-
-    html_text = table.to_html(index=False, header=False, na_rep="")
-    text = lxml.html.document_fromstring(html_text).text_content()
-
-    if include_metadata:
-        metadata = ElementMetadata(
-            text_as_html=html_text,
-            filename=metadata_filename or filename,
-        )
-    else:
-        metadata = ElementMetadata()
-
-    return [Table(text=text, metadata=metadata)]
+    # Verify that only one of the arguments was provided
+    if text is None:
+        text = ""
+    exactly_one(filename=filename, file=file, text=text, url=url)
+
+    last_modification_date = None
+    if filename is not None:
+        last_modification_date = get_last_modified_date(filename)
+        with open(filename, encoding="utf8") as f:
+            text = optional_decode(f.read())
+
+    elif file is not None:
+        last_modification_date = get_last_modified_date_from_file(file)
+        text = optional_decode(file.read())
+
+    elif url is not None:
+        response = requests.get(url)
+        if not response.ok:
+            raise ValueError(f"URL return an error: {response.status_code}")
+
+        content_type = response.headers.get("Content-Type", "")
+        if not content_type.startswith("text/markdown"):
+            raise ValueError(
+                f"Expected content type text/markdown. Got {content_type}.",
+            )
+
+        text = response.text
+
+    html = markdown.markdown(text)
+
+    return partition_html(
+        text=html,
+        include_page_breaks=include_page_breaks,
+        include_metadata=include_metadata,
+        parser=parser,
+        metadata_filename=metadata_filename,
+        metadata_date=metadata_date or last_modification_date,
+    )
```

### Comparing `unstructured-0.8.4/unstructured/partition/xlsx.py` & `unstructured-0.8.5/unstructured/partition/xlsx.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,58 +7,72 @@
 from unstructured.documents.elements import (
     Element,
     ElementMetadata,
     Table,
     process_metadata,
 )
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
+from unstructured.partition.common import (
+    exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
+    spooled_to_bytes_io_if_needed,
+)
 
 
 @process_metadata()
 @add_metadata_with_filetype(FileType.XLSX)
 def partition_xlsx(
     filename: Optional[str] = None,
     file: Optional[Union[IO[bytes], SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions Microsoft Excel Documents in .xlsx format into its document elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     include_metadata
         Determines whether or not metadata is included in the output.
+    metadata_date
+        The day of the last modification
     """
     exactly_one(filename=filename, file=file)
-
+    last_modification_date = None
     if filename:
         sheets = pd.read_excel(filename, sheet_name=None)
-    else:
-        f = spooled_to_bytes_io_if_needed(cast(Union[BinaryIO, SpooledTemporaryFile], file))
+        last_modification_date = get_last_modified_date(filename)
+
+    elif file:
+        f = spooled_to_bytes_io_if_needed(
+            cast(Union[BinaryIO, SpooledTemporaryFile], file),
+        )
         sheets = pd.read_excel(f, sheet_name=None)
+        last_modification_date = get_last_modified_date_from_file(file)
 
     elements: List[Element] = []
     page_number = 0
     for sheet_name, table in sheets.items():
         page_number += 1
         html_text = table.to_html(index=False, header=False, na_rep="")
         text = lxml.html.document_fromstring(html_text).text_content()
 
         if include_metadata:
             metadata = ElementMetadata(
                 text_as_html=html_text,
                 page_name=sheet_name,
                 page_number=page_number,
                 filename=metadata_filename or filename,
+                date=metadata_date or last_modification_date,
             )
         else:
             metadata = ElementMetadata()
 
         table = Table(text=text, metadata=metadata)
         elements.append(table)
```

### Comparing `unstructured-0.8.4/unstructured/partition/xml.py` & `unstructured-0.8.5/unstructured/partition/xml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import xml.etree.ElementTree as ET
 from tempfile import SpooledTemporaryFile
 from typing import IO, BinaryIO, List, Optional, Union, cast
 
 from unstructured.documents.elements import Element, process_metadata
 from unstructured.file_utils.encoding import read_txt_file
 from unstructured.file_utils.filetype import FileType, add_metadata_with_filetype
-from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
+from unstructured.partition.common import (
+    exactly_one,
+    get_last_modified_date,
+    get_last_modified_date_from_file,
+    spooled_to_bytes_io_if_needed,
+)
 from unstructured.partition.text import partition_text
 
 
 def is_leaf(elem):
     return not bool(elem)
 
 
@@ -51,14 +56,15 @@
     xml_keep_tags: bool = False,
     xml_path: str = ".",
     metadata_filename: Optional[str] = None,
     include_metadata: bool = True,
     encoding: Optional[str] = None,
     max_partition: Optional[int] = 1500,
     min_partition: Optional[int] = 0,
+    metadata_date: Optional[str] = None,
     **kwargs,
 ) -> List[Element]:
     """Partitions an XML document into its document elements.
 
     Parameters
     ----------
     filename
@@ -76,14 +82,16 @@
         Determines whether or not metadata is included in the metadata attribute on the
         elements in the output.
     max_partition
         The maximum number of characters to include in a partition. If None is passed,
         no maximum is applied.
     min_partition
         The minimum number of characters to include in a partition.
+    metadata_date
+        The day of the last modification
     """
     exactly_one(filename=filename, file=file)
 
     if xml_keep_tags:
         if filename:
             _, raw_text = read_txt_file(filename=filename, encoding=encoding)
         elif file:
@@ -91,16 +99,24 @@
                 cast(Union[BinaryIO, SpooledTemporaryFile], file),
             )
             _, raw_text = read_txt_file(file=f, encoding=encoding)
         else:
             raise ValueError("Either 'filename' or 'file' must be provided.")
     else:
         raw_text = get_leaf_elements(filename=filename, file=file, xml_path=xml_path)
+
+    last_modification_date = None
+    if filename:
+        last_modification_date = get_last_modified_date(filename)
+    elif file:
+        last_modification_date = get_last_modified_date_from_file(file)
+
     elements = partition_text(
         text=raw_text,
         metadata_filename=metadata_filename,
         include_metadata=include_metadata,
         max_partition=max_partition,
         min_partition=min_partition,
+        metadata_date=metadata_date or last_modification_date,
     )
 
     return elements
```

### Comparing `unstructured-0.8.4/unstructured/staging/argilla.py` & `unstructured-0.8.5/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/staging/base.py` & `unstructured-0.8.5/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/staging/baseplate.py` & `unstructured-0.8.5/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/staging/datasaur.py` & `unstructured-0.8.5/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/staging/huggingface.py` & `unstructured-0.8.5/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/staging/label_box.py` & `unstructured-0.8.5/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/staging/label_studio.py` & `unstructured-0.8.5/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/staging/prodigy.py` & `unstructured-0.8.5/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/staging/weaviate.py` & `unstructured-0.8.5/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured/utils.py` & `unstructured-0.8.5/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured.egg-info/PKG-INFO` & `unstructured-0.8.5/unstructured.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.8.4
+Version: 0.8.5
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.8.4 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.8.5 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.8.4/unstructured.egg-info/SOURCES.txt` & `unstructured-0.8.5/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.8.4/unstructured.egg-info/requires.txt` & `unstructured-0.8.5/unstructured.egg-info/requires.txt`

 * *Files identical despite different names*

