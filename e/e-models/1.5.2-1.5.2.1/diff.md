# Comparing `tmp/e-models-1.5.2.tar.gz` & `tmp/e-models-1.5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.5.2.tar", last modified: Thu Jul 27 16:16:57 2023, max compression
+gzip compressed data, was "e-models-1.5.2.1.tar", last modified: Thu Jul 27 16:35:03 2023, max compression
```

## Comparing `e-models-1.5.2.tar` & `e-models-1.5.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.718224 e-models-1.5.2/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.5.2/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3468 2023-07-27 16:16:57.718224 e-models-1.5.2/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-07-25 17:58:30.000000 e-models-1.5.2/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.714224 e-models-1.5.2/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3468 2023-07-27 16:16:57.000000 e-models-1.5.2/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      655 2023-07-27 16:16:57.000000 e-models-1.5.2/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-07-27 16:16:57.000000 e-models-1.5.2/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       62 2023-07-27 16:16:57.000000 e-models-1.5.2/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-07-27 16:16:57.000000 e-models-1.5.2/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.714224 e-models-1.5.2/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-07-27 16:16:25.000000 e-models-1.5.2/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-07-26 22:24:33.000000 e-models-1.5.2/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.714224 e-models-1.5.2/emodels/datasets/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.5.2/emodels/datasets/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12135 2023-07-27 14:36:45.000000 e-models-1.5.2/emodels/datasets/models.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1929 2023-07-05 14:16:56.000000 e-models-1.5.2/emodels/datasets/tokenizers.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6935 2023-07-27 13:48:16.000000 e-models-1.5.2/emodels/datasets/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.714224 e-models-1.5.2/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.5.2/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.5.2/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.5.2/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.5.2/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.5.2/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.5.2/emodels/py.typed
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.714224 e-models-1.5.2/emodels/scrapyutils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.5.2/emodels/scrapyutils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2575 2023-07-26 22:24:33.000000 e-models-1.5.2/emodels/scrapyutils/loader.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6000 2023-07-21 19:40:03.000000 e-models-1.5.2/emodels/scrapyutils/response.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.5.2/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-07-27 16:16:57.718224 e-models-1.5.2/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1017 2023-07-27 16:16:20.000000 e-models-1.5.2/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.718224 e-models-1.5.2/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6346 2023-07-21 17:31:24.000000 e-models-1.5.2/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8234 2023-07-26 22:27:27.000000 e-models-1.5.2/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.443218 e-models-1.5.2.1/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.5.2.1/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3504 2023-07-27 16:35:03.443218 e-models-1.5.2.1/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-07-25 17:58:30.000000 e-models-1.5.2.1/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.439218 e-models-1.5.2.1/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3504 2023-07-27 16:35:03.000000 e-models-1.5.2.1/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      655 2023-07-27 16:35:03.000000 e-models-1.5.2.1/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-07-27 16:35:03.000000 e-models-1.5.2.1/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       83 2023-07-27 16:35:03.000000 e-models-1.5.2.1/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-07-27 16:35:03.000000 e-models-1.5.2.1/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.439218 e-models-1.5.2.1/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2023-07-27 16:34:30.000000 e-models-1.5.2.1/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-07-26 22:24:33.000000 e-models-1.5.2.1/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.443218 e-models-1.5.2.1/emodels/datasets/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.5.2.1/emodels/datasets/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12135 2023-07-27 14:36:45.000000 e-models-1.5.2.1/emodels/datasets/models.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1929 2023-07-05 14:16:56.000000 e-models-1.5.2.1/emodels/datasets/tokenizers.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6935 2023-07-27 13:48:16.000000 e-models-1.5.2.1/emodels/datasets/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.443218 e-models-1.5.2.1/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.5.2.1/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.5.2.1/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.5.2.1/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.5.2.1/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.5.2.1/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.5.2.1/emodels/py.typed
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.443218 e-models-1.5.2.1/emodels/scrapyutils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.5.2.1/emodels/scrapyutils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2575 2023-07-26 22:24:33.000000 e-models-1.5.2.1/emodels/scrapyutils/loader.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6000 2023-07-21 19:40:03.000000 e-models-1.5.2.1/emodels/scrapyutils/response.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.5.2.1/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-07-27 16:35:03.443218 e-models-1.5.2.1/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1056 2023-07-27 16:34:23.000000 e-models-1.5.2.1/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.443218 e-models-1.5.2.1/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6346 2023-07-21 17:31:24.000000 e-models-1.5.2.1/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8234 2023-07-26 22:27:27.000000 e-models-1.5.2.1/tests/test_scrapyutils.py
```

### Comparing `e-models-1.5.2/LICENSE` & `e-models-1.5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2/PKG-INFO` & `e-models-1.5.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.5.2
+Version: 1.5.2.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Provides-Extra: with-transformers
 License-File: LICENSE
 
 e-models
 ========
 
 
 Suite of tools to assist in the build of extraction models with scrapy spiders
```

### Comparing `e-models-1.5.2/README.md` & `e-models-1.5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2/e_models.egg-info/PKG-INFO` & `e-models-1.5.2.1/e_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.5.2
+Version: 1.5.2.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Provides-Extra: with-transformers
 License-File: LICENSE
 
 e-models
 ========
 
 
 Suite of tools to assist in the build of extraction models with scrapy spiders
```

### Comparing `e-models-1.5.2/e_models.egg-info/SOURCES.txt` & `e-models-1.5.2.1/e_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2/emodels/datasets/models.py` & `e-models-1.5.2.1/emodels/datasets/models.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2/emodels/datasets/tokenizers.py` & `e-models-1.5.2.1/emodels/datasets/tokenizers.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2/emodels/datasets/utils.py` & `e-models-1.5.2.1/emodels/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2/emodels/html2text/__init__.py` & `e-models-1.5.2.1/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2/emodels/html2text/config.py` & `e-models-1.5.2.1/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2/emodels/html2text/utils.py` & `e-models-1.5.2.1/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2/emodels/scrapyutils/loader.py` & `e-models-1.5.2.1/emodels/scrapyutils/loader.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2/emodels/scrapyutils/response.py` & `e-models-1.5.2.1/emodels/scrapyutils/response.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2/setup.py` & `e-models-1.5.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.5.2',
+    version      = '1.5.2.1',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
     packages     = find_packages(),
     install_requires=(
-        "datasets",
         "scikit-learn",
         "scrapy",
         "sentencepiece",
-        "torch",
-        "transformers",
     ),
+    extras_require = {
+        "with-transformers": ["datasets", "torch", "transformers"],
+    },
     scripts = [],
     classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
```

### Comparing `e-models-1.5.2/tests/test_html2text.py` & `e-models-1.5.2.1/tests/test_html2text.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2/tests/test_scrapyutils.py` & `e-models-1.5.2.1/tests/test_scrapyutils.py`

 * *Files identical despite different names*

