# Comparing `tmp/constellation-1.0.0.tar.gz` & `tmp/constellation-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constellation-1.0.0.tar", last modified: Wed May 24 13:51:30 2023, max compression
+gzip compressed data, was "constellation-1.1.0.tar", last modified: Thu Jul 27 10:30:54 2023, max compression
```

## Comparing `constellation-1.0.0.tar` & `constellation-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-05-24 13:51:30.848389 constellation-1.0.0/
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     1096 2023-05-23 18:31:17.000000 constellation-1.0.0/LICENSE
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      960 2023-05-24 13:51:30.848389 constellation-1.0.0/PKG-INFO
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      481 2023-05-23 18:31:17.000000 constellation-1.0.0/README.md
-drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-05-24 13:51:30.848389 constellation-1.0.0/constellation/
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      337 2023-05-23 18:31:17.000000 constellation-1.0.0/constellation/__init__.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     4750 2023-05-23 18:31:17.000000 constellation-1.0.0/constellation/config.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)    10451 2023-05-24 11:08:31.000000 constellation-1.0.0/constellation/constellation.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     6866 2023-05-23 18:31:17.000000 constellation-1.0.0/constellation/docker_util.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     1460 2023-05-23 18:31:17.000000 constellation-1.0.0/constellation/notifier.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      536 2023-05-23 18:31:17.000000 constellation-1.0.0/constellation/util.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     2737 2023-05-23 18:31:17.000000 constellation-1.0.0/constellation/vault.py
-drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-05-24 13:51:30.848389 constellation-1.0.0/constellation.egg-info/
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      960 2023-05-24 13:51:30.000000 constellation-1.0.0/constellation.egg-info/PKG-INFO
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      566 2023-05-24 13:51:30.000000 constellation-1.0.0/constellation.egg-info/SOURCES.txt
--rw-rw-r--   0 aehill    (1000) aehill    (1000)        1 2023-05-24 13:51:30.000000 constellation-1.0.0/constellation.egg-info/dependency_links.txt
--rw-rw-r--   0 aehill    (1000) aehill    (1000)        1 2023-05-24 12:13:36.000000 constellation-1.0.0/constellation.egg-info/not-zip-safe
--rw-rw-r--   0 aehill    (1000) aehill    (1000)       36 2023-05-24 13:51:30.000000 constellation-1.0.0/constellation.egg-info/requires.txt
--rw-rw-r--   0 aehill    (1000) aehill    (1000)       14 2023-05-24 13:51:30.000000 constellation-1.0.0/constellation.egg-info/top_level.txt
--rw-rw-r--   0 aehill    (1000) aehill    (1000)       63 2023-05-24 13:51:30.852388 constellation-1.0.0/setup.cfg
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     1007 2023-05-23 18:36:40.000000 constellation-1.0.0/setup.py
-drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-05-24 13:51:30.848389 constellation-1.0.0/test/
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     7411 2023-05-23 18:31:17.000000 constellation-1.0.0/test/test_config.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)    14233 2023-05-24 11:11:50.000000 constellation-1.0.0/test/test_constellation.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     7595 2023-05-23 18:31:17.000000 constellation-1.0.0/test/test_docker_util.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     1805 2023-05-23 18:31:17.000000 constellation-1.0.0/test/test_notify.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)      398 2023-05-23 18:31:17.000000 constellation-1.0.0/test/test_util.py
--rw-rw-r--   0 aehill    (1000) aehill    (1000)     4892 2023-05-23 18:31:17.000000 constellation-1.0.0/test/test_vault.py
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-27 10:30:54.495949 constellation-1.1.0/
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1096 2023-05-23 18:31:17.000000 constellation-1.1.0/LICENSE
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      960 2023-07-27 10:30:54.495949 constellation-1.1.0/PKG-INFO
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      481 2023-05-23 18:31:17.000000 constellation-1.1.0/README.md
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-27 10:30:54.495949 constellation-1.1.0/constellation/
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      337 2023-05-23 18:31:17.000000 constellation-1.1.0/constellation/__init__.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     4910 2023-07-27 08:12:12.000000 constellation-1.1.0/constellation/config.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)    10451 2023-07-27 08:09:53.000000 constellation-1.1.0/constellation/constellation.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     6866 2023-05-23 18:31:17.000000 constellation-1.1.0/constellation/docker_util.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1460 2023-05-23 18:31:17.000000 constellation-1.1.0/constellation/notifier.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      536 2023-05-23 18:31:17.000000 constellation-1.1.0/constellation/util.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     2737 2023-05-23 18:31:17.000000 constellation-1.1.0/constellation/vault.py
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-27 10:30:54.495949 constellation-1.1.0/constellation.egg-info/
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      960 2023-07-27 10:30:54.000000 constellation-1.1.0/constellation.egg-info/PKG-INFO
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      566 2023-07-27 10:30:54.000000 constellation-1.1.0/constellation.egg-info/SOURCES.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)        1 2023-07-27 10:30:54.000000 constellation-1.1.0/constellation.egg-info/dependency_links.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)        1 2023-07-27 10:30:54.000000 constellation-1.1.0/constellation.egg-info/not-zip-safe
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)       36 2023-07-27 10:30:54.000000 constellation-1.1.0/constellation.egg-info/requires.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)       14 2023-07-27 10:30:54.000000 constellation-1.1.0/constellation.egg-info/top_level.txt
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)       63 2023-07-27 10:30:54.495949 constellation-1.1.0/setup.cfg
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1007 2023-07-27 10:25:34.000000 constellation-1.1.0/setup.py
+drwxrwxr-x   0 aehill    (1000) aehill    (1000)        0 2023-07-27 10:30:54.495949 constellation-1.1.0/test/
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     7550 2023-07-27 08:12:46.000000 constellation-1.1.0/test/test_config.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)    14233 2023-07-27 08:09:53.000000 constellation-1.1.0/test/test_constellation.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     7595 2023-05-23 18:31:17.000000 constellation-1.1.0/test/test_docker_util.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     1805 2023-05-23 18:31:17.000000 constellation-1.1.0/test/test_notify.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)      398 2023-05-23 18:31:17.000000 constellation-1.1.0/test/test_util.py
+-rw-rw-r--   0 aehill    (1000) aehill    (1000)     4892 2023-05-23 18:31:17.000000 constellation-1.1.0/test/test_vault.py
```

### Comparing `constellation-1.0.0/LICENSE` & `constellation-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `constellation-1.0.0/PKG-INFO` & `constellation-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constellation
-Version: 1.0.0
+Version: 1.1.0
 Summary: Deploy scripts for constellations of docker containers
 Home-page: https://github.com/reside-ic/constellation
 Author: Rich FitzJohn
 Author-email: r.fitzjohn@imperial.ac.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `constellation-1.0.0/constellation/config.py` & `constellation-1.1.0/constellation/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
                 return default
             e.args = (":".join(path[:(i + 1)]),)
             raise e
 
     expected = {"string": str,
                 "integer": int,
                 "boolean": bool,
-                "dict": dict}
+                "dict": dict,
+                "list": list}
     if type(data) is not expected[data_type]:
         raise ValueError("Expected {} for {}".format(
             data_type, ":".join(path)))
     return data
 
 
 # TODO: This can be made better with respect to optional values (e.g.,
@@ -90,14 +91,18 @@
     for k, v in d.items():
         if type(v) is not str:
             raise ValueError("Expected a string for {}".format(
                 ":".join(path + [k])))
     return d
 
 
+def config_list(data, path, is_optional=False, default=None):
+    return config_value(data, path, "list", is_optional, default)
+
+
 def config_enum(data, path, values, is_optional=False, default=None):
     value = config_string(data, path, is_optional, default)
     if value not in values:
         raise ValueError("Expected one of [{}] for {}".format(
             ", ".join(values), ":".join(path)))
     return value
```

### Comparing `constellation-1.0.0/constellation/constellation.py` & `constellation-1.1.0/constellation/constellation.py`

 * *Files identical despite different names*

### Comparing `constellation-1.0.0/constellation/docker_util.py` & `constellation-1.1.0/constellation/docker_util.py`

 * *Files identical despite different names*

### Comparing `constellation-1.0.0/constellation/notifier.py` & `constellation-1.1.0/constellation/notifier.py`

 * *Files identical despite different names*

### Comparing `constellation-1.0.0/constellation/util.py` & `constellation-1.1.0/constellation/util.py`

 * *Files identical despite different names*

### Comparing `constellation-1.0.0/constellation/vault.py` & `constellation-1.1.0/constellation/vault.py`

 * *Files identical despite different names*

### Comparing `constellation-1.0.0/constellation.egg-info/PKG-INFO` & `constellation-1.1.0/constellation.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constellation
-Version: 1.0.0
+Version: 1.1.0
 Summary: Deploy scripts for constellations of docker containers
 Home-page: https://github.com/reside-ic/constellation
 Author: Rich FitzJohn
 Author-email: r.fitzjohn@imperial.ac.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `constellation-1.0.0/constellation.egg-info/SOURCES.txt` & `constellation-1.1.0/constellation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `constellation-1.0.0/setup.py` & `constellation-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "docker",
     "hvac",
     "pytest",
     "pyyaml",
     "vault_dev"]
 
 setup(name="constellation",
-      version="1.0.0",
+      version="1.1.0",
       description="Deploy scripts for constellations of docker containers",
       long_description=long_description,
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
       ],
```

### Comparing `constellation-1.0.0/test/test_config.py` & `constellation-1.1.0/test/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pytest
 
 from unittest import mock
 
 from constellation.config import *
 
 sample_data = {"a": "value1", "b": {"x": "value2"}, "c": 1, "d": True,
-               "e": None, "f": "$EXAMPLE_ENV_VAR"}
+               "e": None, "f": "$EXAMPLE_ENV_VAR", "g": [1, 2, 3]}
 
 
 def test_config_string_reads_simple_values():
     assert config_string(sample_data, "a") == "value1"
     assert config_string(sample_data, ["a"]) == "value1"
 
 
@@ -68,17 +68,21 @@
 
 
 def test_config_dict_strict_returns_null_if_optional():
     dat = {"a": {"b": {"c": 1}}}
     assert config_dict_strict(dat, ["x"], "c", True) is None
 
 
+def test_config_list_returns_list():
+    assert config_list(sample_data, ["g"]) == sample_data["g"]
+
+
 def test_config_enum_returns_string():
     assert config_enum(sample_data, ["b", "x"], ["value1", "value2"]) == \
-        "value2"
+           "value2"
 
 
 def test_config_enum_raises_if_invalid():
     with pytest.raises(ValueError,
                        match=r"Expected one of \[enum1, enum2\] for b:x"):
         config_enum(sample_data, ["b", "x"], ["enum1", "enum2"])
 
@@ -168,21 +172,21 @@
 def test_combine():
     def do_combine(a, b):
         """lets us use combine with unnamed data"""
         combine(a, b)
         return a
 
     assert do_combine({"a": 1}, {"b": 2}) == \
-        {"a": 1, "b": 2}
+           {"a": 1, "b": 2}
     assert do_combine({"a": {"x": 1}, "b": 2}, {"a": {"x": 3}}) == \
-        {"a": {"x": 3}, "b": 2}
+           {"a": {"x": 3}, "b": 2}
     assert do_combine({"a": {"x": 1, "y": 4}, "b": 2}, {"a": {"x": 3}}) == \
-        {"a": {"x": 3, "y": 4}, "b": 2}
+           {"a": {"x": 3, "y": 4}, "b": 2}
     assert do_combine({"a": None, "b": 2}, {"a": {"x": 3}}) == \
-        {"a": {"x": 3}, "b": 2}
+           {"a": {"x": 3}, "b": 2}
 
 
 def test_combine_can_replace_dict():
     base = {"a": {"c": {"d": "x"}}, "b": "y"}
     options = {"a": {"c": None}}
     combine(base, options)
     assert base["a"]["c"] is None
@@ -207,17 +211,17 @@
         path_extra = path + "/options.yml"
         write_file(base, path_base)
         write_file(extra, path_extra)
         data = read_yaml(path_base)
         assert config_build(path, data) == data
         assert config_build(path, data, "options") == {"a": 2, "b": 4, "c": 3}
         assert config_build(path, data, None, options) == \
-            {"a": 3, "b": 2, "c": 9, "x": "y"}
+               {"a": 3, "b": 2, "c": 9, "x": "y"}
         assert config_build(path, data, None, options2) == \
-            {"a": 3, "b": 2, "c": 9, "x": "z"}
+               {"a": 3, "b": 2, "c": 9, "x": "z"}
 
 
 def test_config_build_prevents_changing_container_prefix():
     base = "container_prefix: a\nb: 2\nc: 3\n"
     extra = "container_prefix: b\na: 2"
     options = {"container_prefix": "c", "a": 3}
     with tempfile.TemporaryDirectory() as path:
```

### Comparing `constellation-1.0.0/test/test_constellation.py` & `constellation-1.1.0/test/test_constellation.py`

 * *Files identical despite different names*

### Comparing `constellation-1.0.0/test/test_docker_util.py` & `constellation-1.1.0/test/test_docker_util.py`

 * *Files identical despite different names*

### Comparing `constellation-1.0.0/test/test_notify.py` & `constellation-1.1.0/test/test_notify.py`

 * *Files identical despite different names*

### Comparing `constellation-1.0.0/test/test_vault.py` & `constellation-1.1.0/test/test_vault.py`

 * *Files identical despite different names*

