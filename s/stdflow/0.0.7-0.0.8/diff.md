# Comparing `tmp/stdflow-0.0.7.tar.gz` & `tmp/stdflow-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdflow-0.0.7.tar", last modified: Thu Jul 27 03:54:28 2023, max compression
+gzip compressed data, was "/Users/cyprien/Documents/artefact/stdflow/dist/.tmp-jzu1q9wv/stdflow-0.0.8.tar", last modified: Thu Jul 27 08:59:45 2023, max compression
```

## Comparing `stdflow-0.0.7.tar` & `stdflow-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:28.677455 stdflow-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 03:54:15.000000 stdflow-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-27 03:54:28.677455 stdflow-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-27 03:54:15.000000 stdflow-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-27 03:54:15.000000 stdflow-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 03:54:28.677455 stdflow-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:28.677455 stdflow-0.0.7/stdflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-27 03:54:28.000000 stdflow-0.0.7/stdflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-27 03:54:28.000000 stdflow-0.0.7/stdflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:54:28.000000 stdflow-0.0.7/stdflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-27 03:54:28.000000 stdflow-0.0.7/stdflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 03:54:28.000000 stdflow-0.0.7/stdflow.egg-info/top_level.txt
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-27 08:59:45.000000 stdflow-0.0.8/
+-rw-r--r--   0 cyprien    (501) staff       (20)     1071 2023-07-24 15:57:38.000000 stdflow-0.0.8/LICENSE
+-rw-r--r--   0 cyprien    (501) staff       (20)     4257 2023-07-27 08:59:45.000000 stdflow-0.0.8/PKG-INFO
+-rw-r--r--   0 cyprien    (501) staff       (20)     3598 2023-07-27 06:00:59.000000 stdflow-0.0.8/README.md
+-rw-r--r--   0 cyprien    (501) staff       (20)     1140 2023-07-27 08:59:37.000000 stdflow-0.0.8/pyproject.toml
+-rw-r--r--   0 cyprien    (501) staff       (20)       38 2023-07-27 08:59:45.000000 stdflow-0.0.8/setup.cfg
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-27 08:59:45.000000 stdflow-0.0.8/stdflow/
+-rw-r--r--   0 cyprien    (501) staff       (20)     8615 2023-07-27 08:59:37.000000 stdflow-0.0.8/stdflow/__init__.py
+-rw-r--r--   0 cyprien    (501) staff       (20)      135 2023-07-25 05:16:26.000000 stdflow-0.0.8/stdflow/config.py
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-27 08:59:45.000000 stdflow-0.0.8/stdflow/loaders/
+-rw-r--r--   0 cyprien    (501) staff       (20)      339 2023-07-24 02:46:01.000000 stdflow-0.0.8/stdflow/loaders/__init__.py
+-rw-r--r--   0 cyprien    (501) staff       (20)     1134 2023-07-25 03:46:32.000000 stdflow-0.0.8/stdflow/loaders/csv.py
+-rw-r--r--   0 cyprien    (501) staff       (20)     3524 2023-07-27 08:58:17.000000 stdflow-0.0.8/stdflow/metadata.py
+-rw-r--r--   0 cyprien    (501) staff       (20)    16590 2023-07-27 08:58:17.000000 stdflow-0.0.8/stdflow/step.py
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-27 08:59:45.000000 stdflow-0.0.8/stdflow/utils/
+-rw-r--r--   0 cyprien    (501) staff       (20)     8173 2023-07-26 09:06:50.000000 stdflow-0.0.8/stdflow/utils/__init__.py
+drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-27 08:59:45.000000 stdflow-0.0.8/stdflow.egg-info/
+-rw-r--r--   0 cyprien    (501) staff       (20)     4257 2023-07-27 08:59:45.000000 stdflow-0.0.8/stdflow.egg-info/PKG-INFO
+-rw-r--r--   0 cyprien    (501) staff       (20)      337 2023-07-27 08:59:45.000000 stdflow-0.0.8/stdflow.egg-info/SOURCES.txt
+-rw-r--r--   0 cyprien    (501) staff       (20)        1 2023-07-27 08:59:45.000000 stdflow-0.0.8/stdflow.egg-info/dependency_links.txt
+-rw-r--r--   0 cyprien    (501) staff       (20)      145 2023-07-27 08:59:45.000000 stdflow-0.0.8/stdflow.egg-info/requires.txt
+-rw-r--r--   0 cyprien    (501) staff       (20)        8 2023-07-27 08:59:45.000000 stdflow-0.0.8/stdflow.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `stdflow-0.0.7/LICENSE` & `stdflow-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.7/PKG-INFO` & `stdflow-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdflow
-Version: 0.0.7
+Version: 0.0.8
 Summary: [alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output.
 Author-email: Cyprien Ricque <ricque.cyprien@gmail.com>
 Keywords: data science,data,flow,data flow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -114,9 +114,9 @@
 - .gitignore
 TODO: setup pipelines_root, models_root, tests_root, notebooks_root, src_root, config_root, logs_root, reports_root
 TODO: setup the situation in which you chain small function in a directory and it deletes the previous file 
   before creating a new one with another name. in the chain it will appear with different names showing the process
 TODO: a processing step can delete the loaded files.
 TODO: common steps of moving a file / deleting a file
 TODO: setting export=False ? delete_after_n_usage=4 ? 
-
+TODO: version :last should use the metadata (datetime in file and of the file to know which one is the last)
```

### Comparing `stdflow-0.0.7/README.md` & `stdflow-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -98,9 +98,9 @@
 - .gitignore
 TODO: setup pipelines_root, models_root, tests_root, notebooks_root, src_root, config_root, logs_root, reports_root
 TODO: setup the situation in which you chain small function in a directory and it deletes the previous file 
   before creating a new one with another name. in the chain it will appear with different names showing the process
 TODO: a processing step can delete the loaded files.
 TODO: common steps of moving a file / deleting a file
 TODO: setting export=False ? delete_after_n_usage=4 ? 
-
+TODO: version :last should use the metadata (datetime in file and of the file to know which one is the last)
```

### Comparing `stdflow-0.0.7/pyproject.toml` & `stdflow-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ["stdflow"]
 
 [project]
 name = "stdflow"
-version = "0.0.7"
+version = "0.0.8"
 description = "[alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output."
 readme = "README.md"
 authors = [
     { name = "Cyprien Ricque", email = "ricque.cyprien@gmail.com" },
 ]
 keywords = ["data science", "data", "flow", "data flow"]
 requires-python = ">=3.7"
```

### Comparing `stdflow-0.0.7/stdflow.egg-info/PKG-INFO` & `stdflow-0.0.8/stdflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdflow
-Version: 0.0.7
+Version: 0.0.8
 Summary: [alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output.
 Author-email: Cyprien Ricque <ricque.cyprien@gmail.com>
 Keywords: data science,data,flow,data flow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -114,9 +114,9 @@
 - .gitignore
 TODO: setup pipelines_root, models_root, tests_root, notebooks_root, src_root, config_root, logs_root, reports_root
 TODO: setup the situation in which you chain small function in a directory and it deletes the previous file 
   before creating a new one with another name. in the chain it will appear with different names showing the process
 TODO: a processing step can delete the loaded files.
 TODO: common steps of moving a file / deleting a file
 TODO: setting export=False ? delete_after_n_usage=4 ? 
-
+TODO: version :last should use the metadata (datetime in file and of the file to know which one is the last)
```

