# Comparing `tmp/il-datasets-0.1.1.tar.gz` & `tmp/il-datasets-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "il-datasets-0.1.1.tar", last modified: Thu Jun 15 13:12:32 2023, max compression
+gzip compressed data, was "il-datasets-0.2.0.tar", last modified: Thu Jul 27 15:20:28 2023, max compression
```

## Comparing `il-datasets-0.1.1.tar` & `il-datasets-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-06-15 13:12:32.675661 il-datasets-0.1.1/
--rw-rw-r--   0 nathan    (1001) nathan    (1001)     1081 2023-01-09 12:54:57.000000 il-datasets-0.1.1/LICENSE
--rw-rw-r--   0 nathan    (1001) nathan    (1001)     3987 2023-06-15 13:12:32.675661 il-datasets-0.1.1/PKG-INFO
--rw-rw-r--   0 nathan    (1001) nathan    (1001)     3534 2023-01-09 12:54:57.000000 il-datasets-0.1.1/README.md
--rw-rw-r--   0 nathan    (1001) nathan    (1001)      444 2023-06-15 13:11:16.000000 il-datasets-0.1.1/pyproject.toml
--rw-rw-r--   0 nathan    (1001) nathan    (1001)      746 2023-06-15 13:12:32.675661 il-datasets-0.1.1/setup.cfg
--rw-rw-r--   0 nathan    (1001) nathan    (1001)       68 2023-06-15 12:30:41.000000 il-datasets-0.1.1/setup.py
-drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-06-15 13:12:32.671661 il-datasets-0.1.1/src/
-drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-06-15 13:12:32.675661 il-datasets-0.1.1/src/il_datasets.egg-info/
--rw-rw-r--   0 nathan    (1001) nathan    (1001)     3987 2023-06-15 13:12:32.000000 il-datasets-0.1.1/src/il_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 nathan    (1001) nathan    (1001)      584 2023-06-15 13:12:32.000000 il-datasets-0.1.1/src/il_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 nathan    (1001) nathan    (1001)        1 2023-06-15 13:12:32.000000 il-datasets-0.1.1/src/il_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 nathan    (1001) nathan    (1001)       64 2023-06-15 13:12:32.000000 il-datasets-0.1.1/src/il_datasets.egg-info/requires.txt
--rw-rw-r--   0 nathan    (1001) nathan    (1001)       19 2023-06-15 13:12:32.000000 il-datasets-0.1.1/src/il_datasets.egg-info/top_level.txt
-drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-06-15 13:12:32.675661 il-datasets-0.1.1/src/imitation_datasets/
--rw-rw-r--   0 nathan    (1001) nathan    (1001)      187 2023-01-09 12:54:57.000000 il-datasets-0.1.1/src/imitation_datasets/__init__.py
--rw-rw-r--   0 nathan    (1001) nathan    (1001)      758 2023-06-15 12:22:01.000000 il-datasets-0.1.1/src/imitation_datasets/args.py
--rw-rw-r--   0 nathan    (1001) nathan    (1001)     3461 2023-04-12 10:04:01.000000 il-datasets-0.1.1/src/imitation_datasets/controller.py
--rw-rw-r--   0 nathan    (1001) nathan    (1001)     1894 2023-01-09 12:54:57.000000 il-datasets-0.1.1/src/imitation_datasets/experts.py
-drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-06-15 13:12:32.675661 il-datasets-0.1.1/src/imitation_datasets/register/
--rw-rw-r--   0 nathan    (1001) nathan    (1001)       80 2023-01-09 12:54:57.000000 il-datasets-0.1.1/src/imitation_datasets/register/__init__.py
--rw-rw-r--   0 nathan    (1001) nathan    (1001)     2112 2023-01-09 12:54:57.000000 il-datasets-0.1.1/src/imitation_datasets/register/atari.py
--rw-rw-r--   0 nathan    (1001) nathan    (1001)      436 2023-04-12 09:47:37.000000 il-datasets-0.1.1/src/imitation_datasets/register/classic.py
--rw-rw-r--   0 nathan    (1001) nathan    (1001)     1357 2023-01-12 10:29:09.000000 il-datasets-0.1.1/src/imitation_datasets/register/mujoco.py
--rw-rw-r--   0 nathan    (1001) nathan    (1001)     2938 2023-04-12 09:57:05.000000 il-datasets-0.1.1/src/imitation_datasets/utils.py
+drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-07-27 15:20:28.505546 il-datasets-0.2.0/
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     1081 2023-01-09 12:54:57.000000 il-datasets-0.2.0/LICENSE
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     3987 2023-07-27 15:20:28.505546 il-datasets-0.2.0/PKG-INFO
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     3534 2023-01-09 12:54:57.000000 il-datasets-0.2.0/README.md
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)      444 2023-07-27 15:18:45.000000 il-datasets-0.2.0/pyproject.toml
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)      746 2023-07-27 15:20:28.505546 il-datasets-0.2.0/setup.cfg
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)       68 2023-06-15 12:30:41.000000 il-datasets-0.2.0/setup.py
+drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-07-27 15:20:28.501546 il-datasets-0.2.0/src/
+drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-07-27 15:20:28.501546 il-datasets-0.2.0/src/il_datasets.egg-info/
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     3987 2023-07-27 15:20:28.000000 il-datasets-0.2.0/src/il_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)      620 2023-07-27 15:20:28.000000 il-datasets-0.2.0/src/il_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)        1 2023-07-27 15:20:28.000000 il-datasets-0.2.0/src/il_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)       64 2023-07-27 15:20:28.000000 il-datasets-0.2.0/src/il_datasets.egg-info/requires.txt
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)       19 2023-07-27 15:20:28.000000 il-datasets-0.2.0/src/il_datasets.egg-info/top_level.txt
+drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-07-27 15:20:28.501546 il-datasets-0.2.0/src/imitation_datasets/
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)      264 2023-07-27 15:18:45.000000 il-datasets-0.2.0/src/imitation_datasets/__init__.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)      758 2023-06-15 12:22:01.000000 il-datasets-0.2.0/src/imitation_datasets/args.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     3485 2023-07-27 14:04:42.000000 il-datasets-0.2.0/src/imitation_datasets/controller.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     1894 2023-01-09 12:54:57.000000 il-datasets-0.2.0/src/imitation_datasets/experts.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     4143 2023-07-27 14:57:20.000000 il-datasets-0.2.0/src/imitation_datasets/functions.py
+drwxrwxr-x   0 nathan    (1001) nathan    (1001)        0 2023-07-27 15:20:28.505546 il-datasets-0.2.0/src/imitation_datasets/register/
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)       80 2023-01-09 12:54:57.000000 il-datasets-0.2.0/src/imitation_datasets/register/__init__.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     2112 2023-01-09 12:54:57.000000 il-datasets-0.2.0/src/imitation_datasets/register/atari.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)      436 2023-04-12 09:47:37.000000 il-datasets-0.2.0/src/imitation_datasets/register/classic.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     1357 2023-01-12 10:29:09.000000 il-datasets-0.2.0/src/imitation_datasets/register/mujoco.py
+-rw-rw-r--   0 nathan    (1001) nathan    (1001)     5212 2023-07-27 14:58:48.000000 il-datasets-0.2.0/src/imitation_datasets/utils.py
```

### Comparing `il-datasets-0.1.1/LICENSE` & `il-datasets-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `il-datasets-0.1.1/PKG-INFO` & `il-datasets-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: il-datasets
-Version: 0.1.1
+Version: 0.2.0
 Summary: A package for creating IL datasets
 Home-page: https://github.com/NathanGavenski/IL-Datasets
 Author: Nathan Gavenski
 Author-email: nathangavenski@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `il-datasets-0.1.1/README.md` & `il-datasets-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `il-datasets-0.1.1/setup.cfg` & `il-datasets-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = il-datasets
-version = 0.1.1
+version = 0.2.0
 author = Nathan Gavenski
 author_email = nathangavenski@gmail.com
 description = A package for creating IL datasets
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/NathanGavenski/IL-Datasets
 project_urls =
```

### Comparing `il-datasets-0.1.1/src/il_datasets.egg-info/PKG-INFO` & `il-datasets-0.2.0/src/il_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: il-datasets
-Version: 0.1.1
+Version: 0.2.0
 Summary: A package for creating IL datasets
 Home-page: https://github.com/NathanGavenski/IL-Datasets
 Author: Nathan Gavenski
 Author-email: nathangavenski@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `il-datasets-0.1.1/src/il_datasets.egg-info/SOURCES.txt` & `il-datasets-0.2.0/src/il_datasets.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 src/il_datasets.egg-info/dependency_links.txt
 src/il_datasets.egg-info/requires.txt
 src/il_datasets.egg-info/top_level.txt
 src/imitation_datasets/__init__.py
 src/imitation_datasets/args.py
 src/imitation_datasets/controller.py
 src/imitation_datasets/experts.py
+src/imitation_datasets/functions.py
 src/imitation_datasets/utils.py
 src/imitation_datasets/register/__init__.py
 src/imitation_datasets/register/atari.py
 src/imitation_datasets/register/classic.py
 src/imitation_datasets/register/mujoco.py
```

### Comparing `il-datasets-0.1.1/src/imitation_datasets/args.py` & `il-datasets-0.2.0/src/imitation_datasets/args.py`

 * *Files identical despite different names*

### Comparing `il-datasets-0.1.1/src/imitation_datasets/controller.py` & `il-datasets-0.2.0/src/imitation_datasets/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,12 +90,12 @@
                 loop.close()
 
             if opt.mode in ['all', 'collate']:
                 self.pbar = tqdm(range(self.experiments.amount), desc='Running collate')
                 collate = self.collate_closure(opt)
                 collate()
 
-        except Exception as e:
-            self.experiments.add_log(-99, e)
-            raise e
+        except Exception as exception:
+            self.experiments.add_log(-99, exception)
+            raise exception
         finally:
             self.experiments.write_log()
```

### Comparing `il-datasets-0.1.1/src/imitation_datasets/experts.py` & `il-datasets-0.2.0/src/imitation_datasets/experts.py`

 * *Files identical despite different names*

### Comparing `il-datasets-0.1.1/src/imitation_datasets/register/atari.py` & `il-datasets-0.2.0/src/imitation_datasets/register/atari.py`

 * *Files identical despite different names*

### Comparing `il-datasets-0.1.1/src/imitation_datasets/register/mujoco.py` & `il-datasets-0.2.0/src/imitation_datasets/register/mujoco.py`

 * *Files identical despite different names*

