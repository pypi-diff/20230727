# Comparing `tmp/interactivenlp-0.1.1.tar.gz` & `tmp/interactivenlp-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactivenlp-0.1.1.tar", last modified: Wed Jun 14 20:49:06 2023, max compression
+gzip compressed data, was "interactivenlp-0.2.1.tar", last modified: Wed Jul 26 23:57:48 2023, max compression
```

## Comparing `interactivenlp-0.1.1.tar` & `interactivenlp-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 20:49:06.316816 interactivenlp-0.1.1/
--rw-rw-rw-   0        0        0     1093 2023-06-14 20:18:06.000000 interactivenlp-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      358 2023-06-14 20:49:06.308065 interactivenlp-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-05-18 19:26:55.000000 interactivenlp-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-14 20:49:06.292070 interactivenlp-0.1.1/interactivenlp/
--rw-rw-rw-   0        0        0      273 2023-06-14 20:47:39.000000 interactivenlp-0.1.1/interactivenlp/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-06-14 20:34:18.000000 interactivenlp-0.1.1/interactivenlp/server.py
--rw-rw-rw-   0        0        0     2186 2023-06-14 20:48:39.000000 interactivenlp-0.1.1/interactivenlp/types.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:49:06.307066 interactivenlp-0.1.1/interactivenlp.egg-info/
--rw-rw-rw-   0        0        0      358 2023-06-14 20:49:06.000000 interactivenlp-0.1.1/interactivenlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-14 20:49:06.000000 interactivenlp-0.1.1/interactivenlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 20:49:06.000000 interactivenlp-0.1.1/interactivenlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-14 20:49:06.000000 interactivenlp-0.1.1/interactivenlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-14 20:49:06.000000 interactivenlp-0.1.1/interactivenlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 20:49:06.317341 interactivenlp-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      616 2023-06-14 20:49:03.000000 interactivenlp-0.1.1/setup.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.920287 interactivenlp-0.2.1/
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.918061 interactivenlp-0.2.1/InteractiveNLP.egg-info/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-26 23:57:48.000000 interactivenlp-0.2.1/InteractiveNLP.egg-info/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      929 2023-07-26 23:57:48.000000 interactivenlp-0.2.1/InteractiveNLP.egg-info/SOURCES.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-26 23:57:48.000000 interactivenlp-0.2.1/InteractiveNLP.egg-info/dependency_links.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-07-26 23:57:48.000000 interactivenlp-0.2.1/InteractiveNLP.egg-info/requires.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       15 2023-07-26 23:57:48.000000 interactivenlp-0.2.1/InteractiveNLP.egg-info/top_level.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-26 23:57:48.920187 interactivenlp-0.2.1/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       62 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/README.md
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.918271 interactivenlp-0.2.1/interactivenlp/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      327 2023-07-13 19:35:24.000000 interactivenlp-0.2.1/interactivenlp/__init__.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.918815 interactivenlp-0.2.1/interactivenlp/controllers/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/interactivenlp/controllers/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     6981 2023-07-25 19:46:01.000000 interactivenlp-0.2.1/interactivenlp/controllers/reader_controller.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      831 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/interactivenlp/controllers/rss_controller.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.919515 interactivenlp-0.2.1/interactivenlp/models/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/interactivenlp/models/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      344 2023-07-13 20:16:56.000000 interactivenlp-0.2.1/interactivenlp/models/article.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2041 2023-07-24 20:16:58.000000 interactivenlp-0.2.1/interactivenlp/models/block.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 interactivenlp-0.2.1/interactivenlp/models/form.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      314 2023-07-24 19:14:33.000000 interactivenlp-0.2.1/interactivenlp/models/rss.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     5531 2023-07-25 19:46:01.000000 interactivenlp-0.2.1/interactivenlp/models/task.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1005 2023-07-24 19:17:35.000000 interactivenlp-0.2.1/interactivenlp/server.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.919812 interactivenlp-0.2.1/interactivenlp/types/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/interactivenlp/types/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2532 2023-07-25 19:46:09.000000 interactivenlp-0.2.1/interactivenlp/types/model.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-17 20:45:05.000000 interactivenlp-0.2.1/interactivenlp/types/server.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.920004 interactivenlp-0.2.1/interactivenlp/utils/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/interactivenlp/utils/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      633 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/interactivenlp/utils/extraction.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-07-26 23:57:48.920329 interactivenlp-0.2.1/setup.cfg
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1037 2023-07-26 23:57:46.000000 interactivenlp-0.2.1/setup.py
```

