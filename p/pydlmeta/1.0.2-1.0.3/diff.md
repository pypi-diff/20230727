# Comparing `tmp/pydlmeta-1.0.2.tar.gz` & `tmp/pydlmeta-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydlmeta-1.0.2.tar", last modified: Wed Jul 26 09:58:40 2023, max compression
+gzip compressed data, was "pydlmeta-1.0.3.tar", last modified: Thu Jul 27 07:55:10 2023, max compression
```

## Comparing `pydlmeta-1.0.2.tar` & `pydlmeta-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-26 09:58:40.881665 pydlmeta-1.0.2/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1081 2023-07-26 09:58:40.877665 pydlmeta-1.0.2/PKG-INFO
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      904 2023-07-13 03:25:48.000000 pydlmeta-1.0.2/README.md
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-26 09:58:40.877665 pydlmeta-1.0.2/pydlmeta/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-11 03:40:59.000000 pydlmeta-1.0.2/pydlmeta/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      234 2023-07-12 03:15:30.000000 pydlmeta-1.0.2/pydlmeta/config.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     4619 2023-07-12 03:13:09.000000 pydlmeta-1.0.2/pydlmeta/dtype_map.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-26 09:58:40.877665 pydlmeta-1.0.2/pydlmeta/identifier/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-11 03:49:38.000000 pydlmeta-1.0.2/pydlmeta/identifier/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     7418 2023-07-12 03:13:09.000000 pydlmeta-1.0.2/pydlmeta/identifier/dataset.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)    10974 2023-07-12 03:13:09.000000 pydlmeta-1.0.2/pydlmeta/identifier/model.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2010 2023-07-26 08:02:17.000000 pydlmeta-1.0.2/pydlmeta/identifier/types.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)    16607 2023-07-26 08:00:04.000000 pydlmeta-1.0.2/pydlmeta/meta.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      567 2023-07-12 03:15:30.000000 pydlmeta-1.0.2/pydlmeta/utils.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-26 09:58:40.877665 pydlmeta-1.0.2/pydlmeta.egg-info/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1081 2023-07-26 09:58:40.000000 pydlmeta-1.0.2/pydlmeta.egg-info/PKG-INFO
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      413 2023-07-26 09:58:40.000000 pydlmeta-1.0.2/pydlmeta.egg-info/SOURCES.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       51 2023-07-26 09:58:40.000000 pydlmeta-1.0.2/pydlmeta.egg-info/dependency_links.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       80 2023-07-26 09:58:40.000000 pydlmeta-1.0.2/pydlmeta.egg-info/requires.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        9 2023-07-26 09:58:40.000000 pydlmeta-1.0.2/pydlmeta.egg-info/top_level.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       38 2023-07-26 09:58:40.881665 pydlmeta-1.0.2/setup.cfg
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1253 2023-07-26 09:58:40.000000 pydlmeta-1.0.2/setup.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-27 07:55:10.198783 pydlmeta-1.0.3/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1081 2023-07-27 07:55:10.198783 pydlmeta-1.0.3/PKG-INFO
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      904 2023-07-13 03:25:48.000000 pydlmeta-1.0.3/README.md
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-27 07:55:10.194783 pydlmeta-1.0.3/pydlmeta/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-11 03:40:59.000000 pydlmeta-1.0.3/pydlmeta/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      234 2023-07-12 03:15:30.000000 pydlmeta-1.0.3/pydlmeta/config.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4619 2023-07-12 03:13:09.000000 pydlmeta-1.0.3/pydlmeta/dtype_map.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-27 07:55:10.198783 pydlmeta-1.0.3/pydlmeta/identifier/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-11 03:49:38.000000 pydlmeta-1.0.3/pydlmeta/identifier/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     7418 2023-07-12 03:13:09.000000 pydlmeta-1.0.3/pydlmeta/identifier/dataset.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)    10974 2023-07-12 03:13:09.000000 pydlmeta-1.0.3/pydlmeta/identifier/model.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2010 2023-07-26 08:02:17.000000 pydlmeta-1.0.3/pydlmeta/identifier/types.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)    17266 2023-07-27 06:43:23.000000 pydlmeta-1.0.3/pydlmeta/meta.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      567 2023-07-12 03:15:30.000000 pydlmeta-1.0.3/pydlmeta/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-27 07:55:10.198783 pydlmeta-1.0.3/pydlmeta.egg-info/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1081 2023-07-27 07:55:10.000000 pydlmeta-1.0.3/pydlmeta.egg-info/PKG-INFO
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      413 2023-07-27 07:55:10.000000 pydlmeta-1.0.3/pydlmeta.egg-info/SOURCES.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       51 2023-07-27 07:55:10.000000 pydlmeta-1.0.3/pydlmeta.egg-info/dependency_links.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       80 2023-07-27 07:55:10.000000 pydlmeta-1.0.3/pydlmeta.egg-info/requires.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        9 2023-07-27 07:55:10.000000 pydlmeta-1.0.3/pydlmeta.egg-info/top_level.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       38 2023-07-27 07:55:10.198783 pydlmeta-1.0.3/setup.cfg
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1253 2023-07-27 07:55:09.000000 pydlmeta-1.0.3/setup.py
```

### Comparing `pydlmeta-1.0.2/PKG-INFO` & `pydlmeta-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlmeta
-Version: 1.0.2
+Version: 1.0.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # PyDLmeta
```

### Comparing `pydlmeta-1.0.2/README.md` & `pydlmeta-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.2/pydlmeta/dtype_map.py` & `pydlmeta-1.0.3/pydlmeta/dtype_map.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.2/pydlmeta/identifier/dataset.py` & `pydlmeta-1.0.3/pydlmeta/identifier/dataset.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.2/pydlmeta/identifier/model.py` & `pydlmeta-1.0.3/pydlmeta/identifier/model.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.2/pydlmeta/identifier/types.py` & `pydlmeta-1.0.3/pydlmeta/identifier/types.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.2/pydlmeta/meta.py` & `pydlmeta-1.0.3/pydlmeta/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Tuple, Dict
+from typing import List, Union, Tuple, Dict, Optional
 from abc import abstractmethod
 import zipfile
 import glob
 from dataclasses import dataclass
 
 from pydlmeta.identifier.types import ModelFormat
 from pydlmeta.identifier.model  import identify
@@ -33,21 +33,38 @@
     def __new__(cls, name, bases, attrs):
         new_cls = type.__new__(cls, name, bases, attrs)
         if name != "MetadataRetriver":
             cls.REGISTRY.append(new_cls)
         return new_cls
 
 
-class ModelMeta:
-
+class RetrievableModelMeta:
+    """
+    This class only contains information that can be retrieved automatically
+    from a model.
+    DO NOT put any supplementary information here. For example: batch_dim,
+    these type of information should be put in `CompleteModelMeta`
+    """
     def __init__(self, inputs: List[TensorMeta], outputs: List[TensorMeta],
                 format):
         self.inputs = inputs
         self.outputs = outputs
         self.format = format
+    @property
+    def input_names(self):
+        return [x.name for x in self.inputs]
+    @property
+    def input_shapes(self):
+        return [x.shape for x in self.inputs]
+    @property
+    def output_names(self):
+        return [x.shape for x in self.outputs]
+    @property
+    def output_shapes(self):
+        return [x.shape for x in self.outputs]
 
 
 class MetadataRetriver(metaclass=MetadataRetriverRegistry):
 
     FORMAT: ModelFormat = ModelFormat.NON_SPECIFIED
 
     @classmethod
@@ -58,23 +75,23 @@
     def retrieve_inputs(self, model_path) -> List[TensorMeta]:
         raise NotImplementedError("`retrieve_inputs` has to be implemented")
 
     @abstractmethod
     def retrieve_outputs(self, model_path) -> List[TensorMeta]:
         raise NotImplementedError("`retrieve_outputs` has to be implemented")
 
-    def retrieve(self, model_path) -> ModelMeta:
+    def retrieve(self, model_path) -> RetrievableModelMeta:
         inputs = self.retrieve_inputs(model_path)
         logger.debug(f"Inputs: {inputs}")
         outputs = self.retrieve_outputs(model_path)
         logger.debug(f"Outputs: {outputs}")
-        return ModelMeta(inputs=inputs, outputs=outputs, format=self.FORMAT)
+        return RetrievableModelMeta(inputs=inputs, outputs=outputs, format=self.FORMAT)
 
 
-def retrieve_model_metadata(model_path) -> ModelMeta:
+def retrieve_model_metadata(model_path) -> RetrievableModelMeta:
     for metadataretriever in MetadataRetriver.REGISTRY:
         if metadataretriever.is_me(model_path):
             return metadataretriever().retrieve(model_path)
 
     raise NotImplementedError(f"Unable to retrieve metadata of {model_path}")
```

### Comparing `pydlmeta-1.0.2/pydlmeta/utils.py` & `pydlmeta-1.0.3/pydlmeta/utils.py`

 * *Files identical despite different names*

### Comparing `pydlmeta-1.0.2/pydlmeta.egg-info/PKG-INFO` & `pydlmeta-1.0.3/pydlmeta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydlmeta
-Version: 1.0.2
+Version: 1.0.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # PyDLmeta
```

### Comparing `pydlmeta-1.0.2/setup.py` & `pydlmeta-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 # This call to setup() does all the work
 setup(
     name="pydlmeta",
-    version="1.0.2",
+    version="1.0.3",
     license="Apache License 2.0",
     long_description=README, # without this pypi upload will raise warning
     long_description_content_type="text/markdown",  # without this pypi upload will raise warning
     packages=find_packages(),
     package_data={"pydlmeta": ["*"]},
     dependency_links=[
         "https://download.pytorch.org/whl/torch_stable.html",
```

