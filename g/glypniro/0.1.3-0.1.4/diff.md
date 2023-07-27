# Comparing `tmp/glypniro-0.1.3.tar.gz` & `tmp/glypniro-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glypniro-0.1.3.tar", max compression
+gzip compressed data, was "glypniro-0.1.4.tar", max compression
```

## Comparing `glypniro-0.1.3.tar` & `glypniro-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-07-21 19:09:43.545233 glypniro-0.1.3/glypniro/__init__.py
--rw-r--r--   0        0        0    14386 2023-07-27 01:40:55.473132 glypniro-0.1.3/glypniro/cli.py
--rw-r--r--   0        0        0    49477 2023-07-24 23:51:40.093127 glypniro-0.1.3/glypniro/common.py
--rw-r--r--   0        0        0     6572 2023-07-21 20:17:32.212490 glypniro-0.1.3/glypniro/reformat.py
--rw-r--r--   0        0        0     2599 2023-07-22 07:18:03.874051 glypniro-0.1.3/glypniro/reformat_skyline.py
--rw-r--r--   0        0        0     1087 2023-07-21 20:25:23.489670 glypniro-0.1.3/LICENSE
--rw-r--r--   0        0        0      672 2023-07-27 01:41:00.960403 glypniro-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7408 2023-07-21 20:23:34.855206 glypniro-0.1.3/README.md
--rw-r--r--   0        0        0     8073 1970-01-01 00:00:00.000000 glypniro-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 19:09:43.545233 glypniro-0.1.4/glypniro/__init__.py
+-rw-r--r--   0        0        0    14386 2023-07-27 01:40:55.473132 glypniro-0.1.4/glypniro/cli.py
+-rw-r--r--   0        0        0    49506 2023-07-27 02:22:48.052311 glypniro-0.1.4/glypniro/common.py
+-rw-r--r--   0        0        0     6572 2023-07-21 20:17:32.212490 glypniro-0.1.4/glypniro/reformat.py
+-rw-r--r--   0        0        0     2599 2023-07-22 07:18:03.874051 glypniro-0.1.4/glypniro/reformat_skyline.py
+-rw-r--r--   0        0        0     1087 2023-07-21 20:25:23.489670 glypniro-0.1.4/LICENSE
+-rw-r--r--   0        0        0      672 2023-07-27 02:22:54.750074 glypniro-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7408 2023-07-21 20:23:34.855206 glypniro-0.1.4/README.md
+-rw-r--r--   0        0        0     8073 1970-01-01 00:00:00.000000 glypniro-0.1.4/PKG-INFO
```

### Comparing `glypniro-0.1.3/glypniro/cli.py` & `glypniro-0.1.4/glypniro/cli.py`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.3/glypniro/common.py` & `glypniro-0.1.4/glypniro/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,14 +274,15 @@
         return df, samples
 
     # process the protein data
     def process(self, mode=1, tmt_info=None, tmt_minimum=2, **kwargs):
         for k in kwargs:
             if k in self.__dict__:
                 setattr(self, k, kwargs[k])
+        print(self.__dict__)
         for i, r in self.data.iterrows():
             glycan_dict = {}
             if mode == 1:
                 search = sequence_regex.search(r[self.sequence_column])
                 # get peptide sequence without flanking prefix and suffix amino acids then create a Sequence object from the string
                 seq = Sequence(search.group(0))
                 # get unformated string from the Sequence object. This unformatted string contain a "." at both end
```

### Comparing `glypniro-0.1.3/glypniro/reformat.py` & `glypniro-0.1.4/glypniro/reformat.py`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.3/glypniro/reformat_skyline.py` & `glypniro-0.1.4/glypniro/reformat_skyline.py`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.3/LICENSE` & `glypniro-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.3/pyproject.toml` & `glypniro-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glypniro"
-version = "0.1.3"
+version = "0.1.4"
 description = "A automated script for processing and combining Byonic and PD standard output."
 authors = ["Toan Phung <toan.phungkhoiquoctoan@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 scipy = "^1.11.1"
```

### Comparing `glypniro-0.1.3/README.md` & `glypniro-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `glypniro-0.1.3/PKG-INFO` & `glypniro-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glypniro
-Version: 0.1.3
+Version: 0.1.4
 Summary: A automated script for processing and combining Byonic and PD standard output.
 Author: Toan Phung
 Author-email: toan.phungkhoiquoctoan@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

