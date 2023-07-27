# Comparing `tmp/qualitative-coding-0.2.2.tar.gz` & `tmp/qualitative-coding-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualitative-coding-0.2.2.tar", last modified: Fri Mar  3 00:49:07 2023, max compression
+gzip compressed data, was "qualitative-coding-0.2.3.tar", last modified: Thu Jul 27 13:59:57 2023, max compression
```

## Comparing `qualitative-coding-0.2.2.tar` & `qualitative-coding-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chrisp   (1690148345) AD\Domain Users (1961537676)        0 2023-03-03 00:49:07.871185 qualitative-coding-0.2.2/
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)      781 2021-07-13 19:40:03.000000 qualitative-coding-0.2.2/LICENSE
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)    12096 2023-03-03 00:49:07.870579 qualitative-coding-0.2.2/PKG-INFO
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)    11590 2023-02-23 02:45:02.000000 qualitative-coding-0.2.2/README.md
--rwxr-xr-x   0 chrisp   (1690148345) AD\Domain Users (1961537676)    10506 2023-02-23 00:35:13.000000 qualitative-coding-0.2.2/qc
-drwxr-xr-x   0 chrisp   (1690148345) AD\Domain Users (1961537676)        0 2023-03-03 00:49:07.866680 qualitative-coding-0.2.2/qualitative_coding/
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)        0 2021-07-13 19:40:03.000000 qualitative-coding-0.2.2/qualitative_coding/__init__.py
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)       96 2021-07-13 19:40:03.000000 qualitative-coding-0.2.2/qualitative_coding/codebook.py
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)    17556 2023-02-23 00:53:48.000000 qualitative-coding-0.2.2/qualitative_coding/corpus.py
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)     3242 2021-07-13 19:40:03.000000 qualitative-coding-0.2.2/qualitative_coding/helpers.py
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)      895 2021-07-13 19:40:03.000000 qualitative-coding-0.2.2/qualitative_coding/logs.py
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)     6230 2021-07-13 19:40:03.000000 qualitative-coding-0.2.2/qualitative_coding/tree_node.py
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)    12357 2023-03-03 00:47:25.000000 qualitative-coding-0.2.2/qualitative_coding/viewer.py
-drwxr-xr-x   0 chrisp   (1690148345) AD\Domain Users (1961537676)        0 2023-03-03 00:49:07.869745 qualitative-coding-0.2.2/qualitative_coding.egg-info/
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)    12096 2023-03-03 00:49:07.000000 qualitative-coding-0.2.2/qualitative_coding.egg-info/PKG-INFO
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)      447 2023-03-03 00:49:07.000000 qualitative-coding-0.2.2/qualitative_coding.egg-info/SOURCES.txt
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)        1 2023-03-03 00:49:07.000000 qualitative-coding-0.2.2/qualitative_coding.egg-info/dependency_links.txt
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)       22 2023-03-03 00:49:07.000000 qualitative-coding-0.2.2/qualitative_coding.egg-info/requires.txt
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)       19 2023-03-03 00:49:07.000000 qualitative-coding-0.2.2/qualitative_coding.egg-info/top_level.txt
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)       38 2023-03-03 00:49:07.871320 qualitative-coding-0.2.2/setup.cfg
--rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)      827 2023-03-03 00:48:57.000000 qualitative-coding-0.2.2/setup.py
+drwxr-xr-x   0 chrisp   (1690148345) AD\Domain Users (1961537676)        0 2023-07-27 13:59:57.130946 qualitative-coding-0.2.3/
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)      781 2021-07-13 19:40:03.000000 qualitative-coding-0.2.3/LICENSE
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)    12096 2023-07-27 13:59:57.130458 qualitative-coding-0.2.3/PKG-INFO
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)    11590 2023-02-23 02:45:02.000000 qualitative-coding-0.2.3/README.md
+-rwxr-xr-x   0 chrisp   (1690148345) AD\Domain Users (1961537676)    10500 2023-07-27 13:58:12.000000 qualitative-coding-0.2.3/qc
+drwxr-xr-x   0 chrisp   (1690148345) AD\Domain Users (1961537676)        0 2023-07-27 13:59:57.126228 qualitative-coding-0.2.3/qualitative_coding/
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)        0 2021-07-13 19:40:03.000000 qualitative-coding-0.2.3/qualitative_coding/__init__.py
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)       96 2021-07-13 19:40:03.000000 qualitative-coding-0.2.3/qualitative_coding/codebook.py
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)    17563 2023-07-27 13:57:25.000000 qualitative-coding-0.2.3/qualitative_coding/corpus.py
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)     3242 2021-07-13 19:40:03.000000 qualitative-coding-0.2.3/qualitative_coding/helpers.py
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)      895 2021-07-13 19:40:03.000000 qualitative-coding-0.2.3/qualitative_coding/logs.py
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)     6230 2021-07-13 19:40:03.000000 qualitative-coding-0.2.3/qualitative_coding/tree_node.py
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)    12357 2023-07-27 13:55:30.000000 qualitative-coding-0.2.3/qualitative_coding/viewer.py
+drwxr-xr-x   0 chrisp   (1690148345) AD\Domain Users (1961537676)        0 2023-07-27 13:59:57.129789 qualitative-coding-0.2.3/qualitative_coding.egg-info/
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)    12096 2023-07-27 13:59:56.000000 qualitative-coding-0.2.3/qualitative_coding.egg-info/PKG-INFO
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)      447 2023-07-27 13:59:56.000000 qualitative-coding-0.2.3/qualitative_coding.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)        1 2023-07-27 13:59:56.000000 qualitative-coding-0.2.3/qualitative_coding.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)       22 2023-07-27 13:59:56.000000 qualitative-coding-0.2.3/qualitative_coding.egg-info/requires.txt
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)       19 2023-07-27 13:59:56.000000 qualitative-coding-0.2.3/qualitative_coding.egg-info/top_level.txt
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)       38 2023-07-27 13:59:57.131056 qualitative-coding-0.2.3/setup.cfg
+-rw-r--r--   0 chrisp   (1690148345) AD\Domain Users (1961537676)      827 2023-07-27 13:56:58.000000 qualitative-coding-0.2.3/setup.py
```

### Comparing `qualitative-coding-0.2.2/LICENSE` & `qualitative-coding-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qualitative-coding-0.2.2/PKG-INFO` & `qualitative-coding-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualitative-coding
-Version: 0.2.2
+Version: 0.2.3
 Summary: Qualitative coding tools for computer scientists
 Home-page: https://github.com/cproctor/qualitative-coding
 Author: Chris Proctor
 Author-email: pypi.org@accounts.chrisproctor.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `qualitative-coding-0.2.2/README.md` & `qualitative-coding-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `qualitative-coding-0.2.2/qc` & `qualitative-coding-0.2.3/qc`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         if args.prepare_corpus:
             corpus.prepare_corpus(
                 pattern=args.pattern, 
                 file_list=file_list,
                 invert=args.invert,
                 preformatted=args.preformatted)
         if args.prepare_codes:
-            corpus.prepare_code_files(pattern=args.pattern, coder=args.coder)
+            corpus.prepare_code_files(args.coder, pattern=args.pattern)
 
     if args.command in ["codebook", "cb"]:
         corpus.update_codebook()
     if args.command in ["list", "ls"]:
         viewer.list_codes(args.expanded, depth=args.depth)
     if args.command in ["rename", "rn"]:
         corpus.rename_codes(
```

### Comparing `qualitative-coding-0.2.2/qualitative_coding/corpus.py` & `qualitative-coding-0.2.3/qualitative_coding/corpus.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         return self.codes_dir / (str(rel_path) + "." + coder + ".codes")
 
     def get_corpus_file_path(self, code_file_path):
         "Inverse of `get_code_file_path`"
         rel_path = code_file_path.relative_to(self.codes_dir)
         return self.corpus_dir / '.'.join(str(rel_path).split('.')[:-2])
 
-    def prepare_code_files(self, pattern=None, file_list=None, invert=False):
+    def prepare_code_files(self, coder, pattern=None, file_list=None, invert=False):
         "For each text in corpus, creates a blank file of equivalent length"
         for f in self.iter_corpus(pattern=pattern, file_list=file_list, invert=invert):
             with open(f) as inf:
                 file_len = len(list(inf))                
             code_path = self.get_code_file_path(f, coder)
             code_path.parent.mkdir(parents=True, exist_ok=True)
             if code_path.exists():
```

### Comparing `qualitative-coding-0.2.2/qualitative_coding/helpers.py` & `qualitative-coding-0.2.3/qualitative_coding/helpers.py`

 * *Files identical despite different names*

### Comparing `qualitative-coding-0.2.2/qualitative_coding/logs.py` & `qualitative-coding-0.2.3/qualitative_coding/logs.py`

 * *Files identical despite different names*

### Comparing `qualitative-coding-0.2.2/qualitative_coding/tree_node.py` & `qualitative-coding-0.2.3/qualitative_coding/tree_node.py`

 * *Files identical despite different names*

### Comparing `qualitative-coding-0.2.2/qualitative_coding/viewer.py` & `qualitative-coding-0.2.3/qualitative_coding/viewer.py`

 * *Files identical despite different names*

### Comparing `qualitative-coding-0.2.2/qualitative_coding.egg-info/PKG-INFO` & `qualitative-coding-0.2.3/qualitative_coding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualitative-coding
-Version: 0.2.2
+Version: 0.2.3
 Summary: Qualitative coding tools for computer scientists
 Home-page: https://github.com/cproctor/qualitative-coding
 Author: Chris Proctor
 Author-email: pypi.org@accounts.chrisproctor.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `qualitative-coding-0.2.2/setup.py` & `qualitative-coding-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qualitative-coding",
-    version="0.2.2",
+    version="0.2.3",
     author="Chris Proctor",
     author_email="pypi.org@accounts.chrisproctor.net",
     description="Qualitative coding tools for computer scientists",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cproctor/qualitative-coding",
     packages=setuptools.find_packages(),
```

