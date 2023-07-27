# Comparing `tmp/pydantic_numpy-3.1.1.tar.gz` & `tmp/pydantic_numpy-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_numpy-3.1.1.tar", max compression
+gzip compressed data, was "pydantic_numpy-3.1.2.tar", max compression
```

## Comparing `pydantic_numpy-3.1.1.tar` & `pydantic_numpy-3.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-03-01 05:05:36.172059 pydantic_numpy-3.1.1/LICENSE
--rw-r--r--   0        0        0     2703 2023-07-25 16:46:39.932073 pydantic_numpy-3.1.1/README.md
--rw-r--r--   0        0        0      138 2023-07-25 16:46:39.932073 pydantic_numpy-3.1.1/pydantic_numpy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 16:46:39.932073 pydantic_numpy-3.1.1/pydantic_numpy/helper/__init__.py
--rw-r--r--   0        0        0     5502 2023-07-25 16:46:48.615024 pydantic_numpy-3.1.1/pydantic_numpy/helper/annotation.py
--rw-r--r--   0        0        0     3891 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/helper/validation.py
--rw-r--r--   0        0        0      118 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/model/__init__.py
--rw-r--r--   0        0        0     1116 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/model/multi_array.py
--rw-r--r--   0        0        0     8605 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/model/np_model.py
--rw-r--r--   0        0        0      474 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/__init__.py
--rw-r--r--   0        0        0     2285 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/i_dimensional.py
--rw-r--r--   0        0        0     2285 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/ii_dimensional.py
--rw-r--r--   0        0        0     2284 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/iii_dimensional.py
--rw-r--r--   0        0        0     2036 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/n_dimensional.py
--rw-r--r--   0        0        0        0 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/__init__.py
--rw-r--r--   0        0        0     2860 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/i_dimensional.py
--rw-r--r--   0        0        0     2860 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
--rw-r--r--   0        0        0     2859 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
--rw-r--r--   0        0        0     2578 2023-07-25 16:46:39.934073 pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/n_dimensional.py
--rw-r--r--   0        0        0     1621 2023-07-26 10:42:16.751707 pydantic_numpy-3.1.1/pydantic_numpy/util.py
--rw-r--r--   0        0        0     1206 2023-07-26 10:44:36.410938 pydantic_numpy-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 pydantic_numpy-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-01 05:05:36.172059 pydantic_numpy-3.1.2/LICENSE
+-rw-r--r--   0        0        0     2703 2023-07-25 16:46:39.932073 pydantic_numpy-3.1.2/README.md
+-rw-r--r--   0        0        0      130 2023-07-27 08:24:24.004488 pydantic_numpy-3.1.2/pydantic_numpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 16:46:39.932073 pydantic_numpy-3.1.2/pydantic_numpy/helper/__init__.py
+-rw-r--r--   0        0        0     5502 2023-07-26 16:19:01.494117 pydantic_numpy-3.1.2/pydantic_numpy/helper/annotation.py
+-rw-r--r--   0        0        0     3891 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/helper/validation.py
+-rw-r--r--   0        0        0      118 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/model/__init__.py
+-rw-r--r--   0        0        0     1116 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/model/multi_array.py
+-rw-r--r--   0        0        0     8605 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/model/np_model.py
+-rw-r--r--   0        0        0      474 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/__init__.py
+-rw-r--r--   0        0        0     2285 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/i_dimensional.py
+-rw-r--r--   0        0        0     2285 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/ii_dimensional.py
+-rw-r--r--   0        0        0     2284 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/iii_dimensional.py
+-rw-r--r--   0        0        0     2036 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/n_dimensional.py
+-rw-r--r--   0        0        0        0 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/__init__.py
+-rw-r--r--   0        0        0     2860 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/i_dimensional.py
+-rw-r--r--   0        0        0     2860 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
+-rw-r--r--   0        0        0     2859 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
+-rw-r--r--   0        0        0     2578 2023-07-25 16:46:39.934073 pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/n_dimensional.py
+-rw-r--r--   0        0        0     1621 2023-07-26 16:19:01.494117 pydantic_numpy-3.1.2/pydantic_numpy/util.py
+-rw-r--r--   0        0        0     1206 2023-07-27 08:24:29.314455 pydantic_numpy-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 pydantic_numpy-3.1.2/PKG-INFO
```

### Comparing `pydantic_numpy-3.1.1/LICENSE` & `pydantic_numpy-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/README.md` & `pydantic_numpy-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/helper/annotation.py` & `pydantic_numpy-3.1.2/pydantic_numpy/helper/annotation.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/helper/validation.py` & `pydantic_numpy-3.1.2/pydantic_numpy/helper/validation.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/model/multi_array.py` & `pydantic_numpy-3.1.2/pydantic_numpy/model/multi_array.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/model/np_model.py` & `pydantic_numpy-3.1.2/pydantic_numpy/model/np_model.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/typing/i_dimensional.py` & `pydantic_numpy-3.1.2/pydantic_numpy/typing/i_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/typing/ii_dimensional.py` & `pydantic_numpy-3.1.2/pydantic_numpy/typing/ii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/typing/iii_dimensional.py` & `pydantic_numpy-3.1.2/pydantic_numpy/typing/iii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/typing/n_dimensional.py` & `pydantic_numpy-3.1.2/pydantic_numpy/typing/n_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/i_dimensional.py` & `pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/i_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/ii_dimensional.py` & `pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/ii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/iii_dimensional.py` & `pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/iii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/n_dimensional.py` & `pydantic_numpy-3.1.2/pydantic_numpy/typing/strict_data_type/n_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pydantic_numpy/util.py` & `pydantic_numpy-3.1.2/pydantic_numpy/util.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.1/pyproject.toml` & `pydantic_numpy-3.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic_numpy"
-version = "3.1.1"
+version = "3.1.2"
 description = "Pydantic Model integration of the NumPy array"
 authors = ["Can H. Tartanoglu", "Christoph Heindl"]
 maintainers = ["Can H. Tartanoglu <python@rotas.mozmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/caniko/pydantic-numpy"
 license = "BSD-4"
```

### Comparing `pydantic_numpy-3.1.1/PKG-INFO` & `pydantic_numpy-3.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-numpy
-Version: 3.1.1
+Version: 3.1.2
 Summary: Pydantic Model integration of the NumPy array
 Home-page: https://github.com/caniko/pydantic-numpy
 License: BSD-4
 Keywords: pydantic,numpy,typing
 Author: Can H. Tartanoglu
 Maintainer: Can H. Tartanoglu
 Maintainer-email: python@rotas.mozmail.com
```

