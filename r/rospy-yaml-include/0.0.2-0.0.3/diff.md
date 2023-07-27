# Comparing `tmp/rospy_yaml_include-0.0.2.tar.gz` & `tmp/rospy_yaml_include-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rospy_yaml_include-0.0.2.tar", last modified: Thu Jul 27 16:02:19 2023, max compression
+gzip compressed data, was "rospy_yaml_include-0.0.3.tar", last modified: Thu Jul 27 21:50:07 2023, max compression
```

## Comparing `rospy_yaml_include-0.0.2.tar` & `rospy_yaml_include-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-27 16:02:19.317545 rospy_yaml_include-0.0.2/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1598 2023-07-27 16:02:19.317545 rospy_yaml_include-0.0.2/PKG-INFO
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1383 2023-07-25 22:16:24.000000 rospy_yaml_include-0.0.2/README.md
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-27 16:02:19.317545 rospy_yaml_include-0.0.2/rospy_yaml_include/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)        0 2023-07-25 22:00:38.000000 rospy_yaml_include-0.0.2/rospy_yaml_include/__init__.py
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     3189 2023-07-26 22:21:08.000000 rospy_yaml_include-0.0.2/rospy_yaml_include/yaml_include.py
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-27 16:02:19.317545 rospy_yaml_include-0.0.2/rospy_yaml_include.egg-info/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1598 2023-07-27 16:02:19.000000 rospy_yaml_include-0.0.2/rospy_yaml_include.egg-info/PKG-INFO
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      338 2023-07-27 16:02:19.000000 rospy_yaml_include-0.0.2/rospy_yaml_include.egg-info/SOURCES.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)        1 2023-07-27 16:02:19.000000 rospy_yaml_include-0.0.2/rospy_yaml_include.egg-info/dependency_links.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       19 2023-07-27 16:02:19.000000 rospy_yaml_include-0.0.2/rospy_yaml_include.egg-info/top_level.txt
--rw-rw-r--   0 brennan   (1000) brennan   (1000)       38 2023-07-27 16:02:19.317545 rospy_yaml_include-0.0.2/setup.cfg
--rw-rw-r--   0 brennan   (1000) brennan   (1000)      477 2023-07-26 22:22:18.000000 rospy_yaml_include-0.0.2/setup.py
-drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-27 16:02:19.317545 rospy_yaml_include-0.0.2/tests/
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1297 2023-07-26 15:55:07.000000 rospy_yaml_include-0.0.2/tests/test_path_include.py
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1327 2023-07-26 22:21:52.000000 rospy_yaml_include-0.0.2/tests/test_relative_include.py
--rw-rw-r--   0 brennan   (1000) brennan   (1000)     1398 2023-07-25 22:00:38.000000 rospy_yaml_include-0.0.2/tests/test_rospy_include.py
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-27 21:50:07.611482 rospy_yaml_include-0.0.3/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     3112 2023-07-27 21:50:07.611482 rospy_yaml_include-0.0.3/PKG-INFO
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     2897 2023-07-27 21:48:46.000000 rospy_yaml_include-0.0.3/README.md
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-27 21:50:07.611482 rospy_yaml_include-0.0.3/rospy_yaml_include/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)        0 2023-07-25 22:00:38.000000 rospy_yaml_include-0.0.3/rospy_yaml_include/__init__.py
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     4381 2023-07-27 21:37:06.000000 rospy_yaml_include-0.0.3/rospy_yaml_include/yaml_include.py
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-27 21:50:07.611482 rospy_yaml_include-0.0.3/rospy_yaml_include.egg-info/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     3112 2023-07-27 21:50:07.000000 rospy_yaml_include-0.0.3/rospy_yaml_include.egg-info/PKG-INFO
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      368 2023-07-27 21:50:07.000000 rospy_yaml_include-0.0.3/rospy_yaml_include.egg-info/SOURCES.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)        1 2023-07-27 21:50:07.000000 rospy_yaml_include-0.0.3/rospy_yaml_include.egg-info/dependency_links.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       19 2023-07-27 21:50:07.000000 rospy_yaml_include-0.0.3/rospy_yaml_include.egg-info/top_level.txt
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)       38 2023-07-27 21:50:07.611482 rospy_yaml_include-0.0.3/setup.cfg
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)      475 2023-07-27 21:49:56.000000 rospy_yaml_include-0.0.3/setup.py
+drwxrwxr-x   0 brennan   (1000) brennan   (1000)        0 2023-07-27 21:50:07.611482 rospy_yaml_include-0.0.3/tests/
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     2403 2023-07-27 21:40:16.000000 rospy_yaml_include-0.0.3/tests/test_dynamic_include.py
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1312 2023-07-27 21:36:41.000000 rospy_yaml_include-0.0.3/tests/test_path_include.py
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1340 2023-07-27 21:39:50.000000 rospy_yaml_include-0.0.3/tests/test_relative_include.py
+-rw-rw-r--   0 brennan   (1000) brennan   (1000)     1398 2023-07-25 22:00:38.000000 rospy_yaml_include-0.0.3/tests/test_rospy_include.py
```

### Comparing `rospy_yaml_include-0.0.2/PKG-INFO` & `rospy_yaml_include-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,113 @@
 Metadata-Version: 2.1
 Name: rospy_yaml_include
-Version: 0.0.2
+Version: 0.0.3
 Summary: rospy_yaml_include
 Home-page: https://git.whoi.edu/acomms/rospy_yaml_include
 Author: WHOI Acomms Group
 Description-Content-Type: text/markdown
 
 # rospy_yaml_include
 
 ## Introduction
 
 rospy_yaml_include is a package that provides a YAML loader that can include other YAML files.
 
 It can either include a file given an absolute path, or given a ROS package name and a relative path.
 
-rospy_yaml_include has a recursive check to prevent circular imports. 
+rospy_yaml_include has a recursive check to prevent circular imports.
 
 ### Usage
 
 The following section contains code snippets showing example usage of the package.
-Additionally, the tests directory contains a few examples of how to use the package. 
+Additionally, the tests directory contains a few examples of how to use the package.
+
+Note that alternative to the below example which use inline yaml, the yaml.load command can be used within a `with open()` statement to load yaml from a file.
+
+### Including a yaml from a ROS package
 
-### Including a yaml from an absolute path
 ```python
 from rospy_yaml_include.yaml_include import RospyYamlInclude
 
 yml = """
-    value: 
+    value:
     - 10
-    fields: !path_include /path/to/file.yml
+        fields: !ros_include
+                package: rospy_yaml_include_test
+                extension: test_files/circular_import_ros.yaml
     """
 
 constructor = RospyYamlInclude()
 yaml.load(yml, Loader=constructor.add_constructor())
 ```
 
-Alternatively, the yaml.load command can be used within a `with open()` statement to load yaml from a file.
+### Dynamic loading of yaml files
+
+Using the `!include` tag, YamlInclude will attempt to infer whether a dynamic of an absolute path is provided. If the path provided has a leading / when it is treated as an absolute path, otherwise it is treated as a relative path. If the path provided is a relative path, then the base_directory parameter must be set during instantiation or else a error will be raised.
+
+#### Including a yaml from a relative path with dynamic tag
 
-### Including a yaml from a ROS package
 ```python
 from rospy_yaml_include.yaml_include import RospyYamlInclude
+import os
+
+cwd = os.getcwd()
 
 yml = """
-    value: 
+    value:
     - 10
-        fields: !ros_include 
-                package: rospy_yaml_include_test
-                extension: test_files/circular_import_ros.yaml
+    fields: !include test_files/import.yaml
+    """
+
+constructor = RospyYamlInclude(base_directory=cwd)
+yaml.load(yml, Loader=constructor.add_constructor())
+```
+
+#### Including a yaml from an absolute path with dynamic tag
+
+```python
+from rospy_yaml_include.yaml_include import RospyYamlInclude
+
+yml = """
+    value:
+    - 10
+    fields: !include /path/to/file.yml
     """
 
 constructor = RospyYamlInclude()
 yaml.load(yml, Loader=constructor.add_constructor())
 ```
 
-Alternatively, the yaml.load command can be used within a `with open()` statement to load yaml from a file.
+### Including a yaml with a relative path
+
+The YamlInclude class contains an optional parameter to set a base path. If this base path is set during instantiation, then the !relative_include flag can be used
+
+```python
+from rospy_yaml_include.yaml_include import RospyYamlInclude
+import os
+
+cwd = os.getcwd()
+
+yml = """
+    value:
+    - 10
+    fields: !relative_include test_files/import.yaml
+    """
+
+constructor = RospyYamlInclude(base_directory=cwd)
+yaml.load(yml, Loader=constructor.add_constructor())
+```
+
+### Including a yaml from an absolute path
+
+```python
+from rospy_yaml_include.yaml_include import RospyYamlInclude
+
+yml = """
+    value:
+    - 10
+    fields: !path_include /path/to/file.yml
+    """
+
+constructor = RospyYamlInclude()
+yaml.load(yml, Loader=constructor.add_constructor())
+```
```

### Comparing `rospy_yaml_include-0.0.2/rospy_yaml_include/yaml_include.py` & `rospy_yaml_include-0.0.3/rospy_yaml_include/yaml_include.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
 
 class RospyYamlInclude:
     """
     RospyYamlInclude class
     """
 
-    def __init__(self, loader: type = yaml.SafeLoader, base_directory: str = None) -> None:
+    def __init__(
+        self, loader: type = yaml.SafeLoader, base_directory: str = None
+    ) -> None:
         self.recursion_limit = 50
         self.recursion_count = 0
 
         self.loader = loader
         self.base_directory = base_directory
 
     class _RosInclude:
@@ -78,32 +80,68 @@
         """
 
         self.recursion_count += 1
         if self.recursion_count > self.recursion_limit:
             raise RecursionError(
                 "Maximum recursion limit reached, check for circular references"
             )
-        
+
         if self.base_directory is None:
-            raise ValueError("base_directory must be provided in class init to use !relative_include")
+            raise ValueError(
+                "base_directory must be provided in class init to use !relative_include"
+            )
 
         file = loader.construct_scalar(node)
 
         include_file = os.path.join(
             self.base_directory,
             file,
         )
 
         with open(include_file, encoding="utf-8") as yaml_file:
             return yaml.load(yaml_file, Loader=self.add_constructor())
 
+    def _dynamic_include_constructor(
+        self, loader: type, node: yaml.nodes.ScalarNode
+    ) -> dict:
+        """
+        _dynamic_include_constructor function handles !include tag
+
+        this constructor attempts to infer the type of include based on the file extension
+        """
+
+        self.recursion_count += 1
+        if self.recursion_count > self.recursion_limit:
+            raise RecursionError(
+                "Maximum recursion limit reached, check for circular references"
+            )
+
+        file = loader.construct_scalar(node)
+
+        if file.startswith("/"):
+            include_file = file
+        else:
+            if self.base_directory is None:
+                raise ValueError(
+                    "base_directory must be provided in class init to use relative include"
+                )
+
+            include_file = os.path.join(
+                self.base_directory,
+                file,
+            )
+
+        with open(include_file, encoding="utf-8") as yaml_file:
+            return yaml.load(yaml_file, Loader=self.add_constructor())
+
     def add_constructor(self) -> type:
         """
         add constructor to yaml
         """
 
         loader = self.loader
         loader.add_constructor("!ros_include", self._ros_include_constructor)
         loader.add_constructor("!path_include", self._path_include_constructor)
         loader.add_constructor("!relative_include", self._relative_include_constructor)
+        loader.add_constructor("!include", self._dynamic_include_constructor)
 
         return loader
```

### Comparing `rospy_yaml_include-0.0.2/tests/test_path_include.py` & `rospy_yaml_include-0.0.3/tests/test_path_include.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from rospy_yaml_include.yaml_include import RospyYamlInclude
 import yaml
 import os
 
 
 class TestPathInclude:
     """
-    Class containing unit tests for TestPathInclude
+    Class containing unit tests for absolute path include
     """
 
     def test_path_include(self):
         """
         Unit test for path_include
         """
         cwd = os.getcwd()
@@ -26,15 +26,15 @@
             constructor = RospyYamlInclude()
             yaml.load(yml, Loader=constructor.add_constructor())
         except RecursionError as error:
             pytest.fail(f"RecursionError: Maximum recursion limit reached: {error}")
 
     def test_path_circular_include(self):
         """
-        Unit test for circular includes in path_include
+        Unit test for circular includes in absolute path include
         """
         cwd = os.getcwd()
         yml = f"""
             value: 
             - 10
             fields: !path_include {cwd}/test_files/circular_import.yaml
             """
```

### Comparing `rospy_yaml_include-0.0.2/tests/test_relative_include.py` & `rospy_yaml_include-0.0.3/tests/test_relative_include.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pytest
 import sys
 from rospy_yaml_include.yaml_include import RospyYamlInclude
 import yaml
 import os
 
 
-class TestPathInclude:
+class TestRelativeInclude:
     """
-    Class containing unit tests for TestPathInclude
+    Class containing unit tests for relative_include
     """
 
-    def test_path_include(self):
+    def test_relative_include(self):
         """
         Unit test for path_include
         """
         cwd = os.getcwd()
 
         yml = """
             value: 
@@ -24,17 +24,17 @@
 
         try:
             constructor = RospyYamlInclude(base_directory=cwd)
             yaml.load(yml, Loader=constructor.add_constructor())
         except RecursionError as error:
             pytest.fail(f"RecursionError: Maximum recursion limit reached: {error}")
 
-    def test_path_circular_include(self):
+    def test_path_relative_include(self):
         """
-        Unit test for circular includes in path_include
+        Unit test for circular includes in relative_include
         """
         cwd = os.getcwd()
         yml = """
             value: 
             - 10
             fields: !relative_include test_files/circular_import.yaml
             """
```

### Comparing `rospy_yaml_include-0.0.2/tests/test_rospy_include.py` & `rospy_yaml_include-0.0.3/tests/test_rospy_include.py`

 * *Files identical despite different names*

