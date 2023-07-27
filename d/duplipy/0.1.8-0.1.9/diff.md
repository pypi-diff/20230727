# Comparing `tmp/duplipy-0.1.8.tar.gz` & `tmp/duplipy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duplipy-0.1.8.tar", last modified: Thu Jul 27 16:31:03 2023, max compression
+gzip compressed data, was "duplipy-0.1.9.tar", last modified: Thu Jul 27 16:54:18 2023, max compression
```

## Comparing `duplipy-0.1.8.tar` & `duplipy-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 16:31:03.918130 duplipy-0.1.8/
--rw-rw-rw-   0        0        0      955 2023-07-07 14:42:48.000000 duplipy-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1027 2023-07-27 16:31:03.914131 duplipy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4204 2023-07-27 16:04:10.000000 duplipy-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 16:31:03.857136 duplipy-0.1.8/duplipy/
--rw-rw-rw-   0        0        0      636 2023-07-27 15:31:14.000000 duplipy-0.1.8/duplipy/__init__.py
--rw-rw-rw-   0        0        0     6539 2023-07-07 08:39:46.000000 duplipy-0.1.8/duplipy/formatting.py
--rw-rw-rw-   0        0        0    10946 2023-07-27 16:28:39.000000 duplipy-0.1.8/duplipy/replication.py
--rw-rw-rw-   0        0        0     1533 2023-07-07 14:20:43.000000 duplipy-0.1.8/duplipy/similarity.py
--rw-rw-rw-   0        0        0      897 2023-07-07 14:21:51.000000 duplipy-0.1.8/duplipy/text_analysis.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:31:03.908135 duplipy-0.1.8/duplipy.egg-info/
--rw-rw-rw-   0        0        0     1027 2023-07-27 16:31:01.000000 duplipy-0.1.8/duplipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-07-27 16:31:02.000000 duplipy-0.1.8/duplipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 16:31:01.000000 duplipy-0.1.8/duplipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-27 16:31:02.000000 duplipy-0.1.8/duplipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-27 16:31:02.000000 duplipy-0.1.8/duplipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 16:31:03.921134 duplipy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1302 2023-07-27 16:27:52.000000 duplipy-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:54:18.902932 duplipy-0.1.9/
+-rw-rw-rw-   0        0        0      955 2023-07-07 14:42:48.000000 duplipy-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1027 2023-07-27 16:54:18.899935 duplipy-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4170 2023-07-27 16:33:31.000000 duplipy-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 16:54:18.871931 duplipy-0.1.9/duplipy/
+-rw-rw-rw-   0        0        0      607 2023-07-27 16:35:25.000000 duplipy-0.1.9/duplipy/__init__.py
+-rw-rw-rw-   0        0        0     6539 2023-07-07 08:39:46.000000 duplipy-0.1.9/duplipy/formatting.py
+-rw-rw-rw-   0        0        0    10946 2023-07-27 16:28:39.000000 duplipy-0.1.9/duplipy/replication.py
+-rw-rw-rw-   0        0        0     1533 2023-07-07 14:20:43.000000 duplipy-0.1.9/duplipy/similarity.py
+-rw-rw-rw-   0        0        0      897 2023-07-07 14:21:51.000000 duplipy-0.1.9/duplipy/text_analysis.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:54:18.894932 duplipy-0.1.9/duplipy.egg-info/
+-rw-rw-rw-   0        0        0     1027 2023-07-27 16:54:18.000000 duplipy-0.1.9/duplipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-27 16:54:18.000000 duplipy-0.1.9/duplipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 16:54:18.000000 duplipy-0.1.9/duplipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-27 16:54:18.000000 duplipy-0.1.9/duplipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 16:54:18.000000 duplipy-0.1.9/duplipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 16:54:18.903931 duplipy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1302 2023-07-27 16:53:55.000000 duplipy-0.1.9/setup.py
```

### Comparing `duplipy-0.1.8/LICENSE` & `duplipy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `duplipy-0.1.8/PKG-INFO` & `duplipy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplipy
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for formatting and text replication, with added support for image augmentation.
 Home-page: https://github.com/infinitode/duplipy
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplipy-0.1.8/README.md` & `duplipy-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# DupliPy 0.1.7
+# DupliPy 0.1.8
 
 An open source Python library for text formatting, augmentation, and similarity calculation tasks in NLP.
 
-## Changes to DupliPy 0.1.7
+## Changes to DupliPy
 
 DupliPy now offers support for image augmentation, with functions to rotate, resize and crop images. These are available through:
 ```python
-from duplipy.replication import flip_horizontal, flip_vertical, rotate, random_rotation, resize, crop, random_crop, perform_image_augmentation
+from duplipy.replication import flip_horizontal, flip_vertical, rotate, random_rotation, resize, crop, random_crop
 ```
 
 ## Installation
 
 You can install DupliPy using pip:
 
 ```bash
```

### Comparing `duplipy-0.1.8/duplipy/__init__.py` & `duplipy-0.1.9/duplipy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,5 +1,5 @@
-import duplipy
+import source
 from .formatting import remove_stopwords, remove_numbers, remove_whitespace, normalize_whitespace, separate_symbols, remove_special_characters, standardize_text, tokenize_text, stem_words, lemmatize_words, pos_tag
-from .replication import replace_word_with_synonym, augment_text_with_synonyms, load_text_file, augment_file_with_synonyms, insert_random_word, delete_random_word, insert_synonym, paraphrase, flip_horizontal, flip_vertical, rotate, random_rotation, resize, crop, random_crop, perform_image_augmentation
+from .replication import replace_word_with_synonym, augment_text_with_synonyms, load_text_file, augment_file_with_synonyms, insert_random_word, delete_random_word, insert_synonym, paraphrase, flip_horizontal, flip_vertical, rotate, random_rotation, resize, crop, random_crop
 from .similarity import edit_distance_score, bleu_score
 from .text_analysis import analyze_sentiment
```

### Comparing `duplipy-0.1.8/duplipy/formatting.py` & `duplipy-0.1.9/duplipy/formatting.py`

 * *Files identical despite different names*

### Comparing `duplipy-0.1.8/duplipy/replication.py` & `duplipy-0.1.9/duplipy/replication.py`

 * *Files identical despite different names*

### Comparing `duplipy-0.1.8/duplipy/similarity.py` & `duplipy-0.1.9/duplipy/similarity.py`

 * *Files identical despite different names*

### Comparing `duplipy-0.1.8/duplipy/text_analysis.py` & `duplipy-0.1.9/duplipy/text_analysis.py`

 * *Files identical despite different names*

### Comparing `duplipy-0.1.8/duplipy.egg-info/PKG-INFO` & `duplipy-0.1.9/duplipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplipy
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for formatting and text replication, with added support for image augmentation.
 Home-page: https://github.com/infinitode/duplipy
 Author: Infinitode Pty Ltd
 Author-email: infinitode.ltd@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplipy-0.1.8/setup.py` & `duplipy-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='duplipy',
-    version='0.1.8',
+    version='0.1.9',
     author='Infinitode Pty Ltd',
     author_email='infinitode.ltd@gmail.com',
     description='A package for formatting and text replication, with added support for image augmentation.',
     long_description='DupliPy is a quick and easy-to-use package that can handle text formatting and data augmentation tasks for NLP in Python, with added support for image augmentation.',
     long_description_content_type='text/markdown',
     url='https://github.com/infinitode/duplipy',
     packages=find_packages(),
```

