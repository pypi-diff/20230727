# Comparing `tmp/TCFile-2023.4.1.tar.gz` & `tmp/tcfile-2023.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TCFile-2023.4.1.tar", last modified: Mon Apr 17 02:00:25 2023, max compression
+gzip compressed data, was "tcfile-2023.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `TCFile-2023.4.1.tar` & `tcfile-2023.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       42 2023-04-17 02:00:15.316127 TCFile-2023.4.1/.gitattributes
--rw-r--r--   0        0        0      689 2023-04-17 02:00:15.316127 TCFile-2023.4.1/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      241 2023-04-17 02:00:15.316127 TCFile-2023.4.1/.gitignore
--rw-r--r--   0        0        0     1069 2023-04-17 02:00:15.316127 TCFile-2023.4.1/LICENSE
--rw-r--r--   0        0        0      856 2023-04-17 02:00:15.316127 TCFile-2023.4.1/README.md
--rw-r--r--   0        0        0     3594 2023-04-17 02:00:15.316127 TCFile-2023.4.1/TCFile/TCFile_class.py
--rw-r--r--   0        0        0       27 2023-04-17 02:00:15.316127 TCFile-2023.4.1/TCFile/__init__.py
--rw-r--r--   0        0        0     1956 2023-04-17 02:00:15.316127 TCFile-2023.4.1/docs/structure_TCF.md
--rw-r--r--   0        0        0      807 2023-04-17 02:00:15.316127 TCFile-2023.4.1/pyproject.toml
--rw-r--r--   0        0        0       69 2023-04-17 02:00:15.316127 TCFile-2023.4.1/tests/__init__.py
--rw-r--r--   0        0        0      134 2023-04-17 02:00:15.420127 TCFile-2023.4.1/tests/sample.TCF
--rw-r--r--   0        0        0      822 2023-04-17 02:00:15.420127 TCFile-2023.4.1/tests/test_TCFile_class.py
--rw-r--r--   0        0        0     1489 1970-01-01 00:00:00.000000 TCFile-2023.4.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2023-07-27 08:25:38.070719 tcfile-2023.7/.gitattributes
+-rw-r--r--   0        0        0      689 2023-07-27 08:25:38.070719 tcfile-2023.7/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      241 2023-07-27 08:25:38.070719 tcfile-2023.7/.gitignore
+-rw-r--r--   0        0        0     1069 2023-07-27 08:25:38.070719 tcfile-2023.7/LICENSE
+-rw-r--r--   0        0        0      856 2023-07-27 08:25:38.070719 tcfile-2023.7/README.md
+-rw-r--r--   0        0        0     6750 2023-07-27 08:25:38.070719 tcfile-2023.7/TCFile/TCFile_class.py
+-rw-r--r--   0        0        0       27 2023-07-27 08:25:38.070719 tcfile-2023.7/TCFile/__init__.py
+-rw-r--r--   0        0        0     1956 2023-07-27 08:25:38.070719 tcfile-2023.7/docs/structure_TCF.md
+-rw-r--r--   0        0        0      805 2023-07-27 08:25:38.070719 tcfile-2023.7/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-27 08:25:38.070719 tcfile-2023.7/tests/__init__.py
+-rw-r--r--   0        0        0      134 2023-07-27 08:25:38.118705 tcfile-2023.7/tests/sample.TCF
+-rw-r--r--   0        0        0      824 2023-07-27 08:25:38.118705 tcfile-2023.7/tests/test_TCFile_class.py
+-rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 tcfile-2023.7/PKG-INFO
```

### Comparing `TCFile-2023.4.1/.github/workflows/deploy.yml` & `tcfile-2023.7/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `TCFile-2023.4.1/LICENSE` & `tcfile-2023.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TCFile-2023.4.1/README.md` & `tcfile-2023.7/README.md`

 * *Files identical despite different names*

### Comparing `TCFile-2023.4.1/docs/structure_TCF.md` & `tcfile-2023.7/docs/structure_TCF.md`

 * *Files identical despite different names*

### Comparing `TCFile-2023.4.1/pyproject.toml` & `tcfile-2023.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "TCFile"
-version = "2023.4.1"
+version = "2023.7"
 description = "Python package for handling TCF data. It works with Tomcube data"
 readme = "README.md"
 requires-python = ">=3.7,<4"
 license = {file = "LICENSE"}
 authors = [{name = "Dohyeon Lee", email = "dleh428@kaist.ac.kr"}]
 maintainers = [{name = "Dohyeon Lee", email = "dleh428@kaist.ac.kr"}]
```

### Comparing `TCFile-2023.4.1/tests/test_TCFile_class.py` & `tcfile-2023.7/tests/test_TCFile_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,18 @@
         except ValueError as e:
             if e.args[0] != 'The imgtype is not supported':
                 raise e
     
     def test_read(self):
         tcfile = TCFile(SAMPLE_TCF_FILE,'3D')
         data =tcfile[0]
-        assert np.array_equal(tcfile.dataShape, data.shape)
+        assert np.array_equal(tcfile.data_shape, data.shape)
     
     def test_iterative_read(self):
         tcfile = TCFile(SAMPLE_TCF_FILE,'3D')
         for data in tcfile:
-            assert np.array_equal(tcfile.dataShape, data.shape)
+            assert np.array_equal(tcfile.data_shape, data.shape)
             
     def test_attributes(self):
         tcfile = TCFile(SAMPLE_TCF_FILE,'3D')
         assert len(tcfile) == 10
         assert tcfile.dt >= 0
```

### Comparing `TCFile-2023.4.1/PKG-INFO` & `tcfile-2023.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCFile
-Version: 2023.4.1
+Version: 2023.7
 Summary: Python package for handling TCF data. It works with Tomcube data
 Author-email: Dohyeon Lee <dleh428@kaist.ac.kr>
 Maintainer-email: Dohyeon Lee <dleh428@kaist.ac.kr>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

