# Comparing `tmp/openvino_model_api-0.1.3.tar.gz` & `tmp/openvino_model_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvino_model_api-0.1.3.tar", last modified: Mon Jul 10 12:17:39 2023, max compression
+gzip compressed data, was "openvino_model_api-0.1.4.tar", last modified: Thu Jul 27 09:56:57 2023, max compression
```

## Comparing `openvino_model_api-0.1.3.tar` & `openvino_model_api-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 12:17:39.342082 openvino_model_api-0.1.3/
--rw-rw-rw-   0        0        0     7087 2023-07-10 12:17:39.342082 openvino_model_api-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-10 12:17:39.342082 openvino_model_api-0.1.3/openvino_model_api.egg-info/
--rw-rw-rw-   0        0        0     7087 2023-07-10 12:17:39.000000 openvino_model_api-0.1.3/openvino_model_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3588 2023-07-10 12:17:39.000000 openvino_model_api-0.1.3/openvino_model_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 12:17:39.000000 openvino_model_api-0.1.3/openvino_model_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2023-07-10 12:17:39.000000 openvino_model_api-0.1.3/openvino_model_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 12:17:39.000000 openvino_model_api-0.1.3/openvino_model_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 12:17:39.342082 openvino_model_api-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1681 2023-06-10 06:44:08.000000 openvino_model_api-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:56:57.203829 openvino_model_api-0.1.4/
+-rw-rw-rw-   0        0        0     7087 2023-07-27 09:56:57.202830 openvino_model_api-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 09:56:57.200829 openvino_model_api-0.1.4/openvino_model_api.egg-info/
+-rw-rw-rw-   0        0        0     7087 2023-07-27 09:56:57.000000 openvino_model_api-0.1.4/openvino_model_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3671 2023-07-27 09:56:57.000000 openvino_model_api-0.1.4/openvino_model_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 09:56:57.000000 openvino_model_api-0.1.4/openvino_model_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-07-27 09:56:57.000000 openvino_model_api-0.1.4/openvino_model_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 09:56:57.000000 openvino_model_api-0.1.4/openvino_model_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 09:56:57.204827 openvino_model_api-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1681 2023-07-11 13:11:42.000000 openvino_model_api-0.1.4/setup.py
```

### Comparing `openvino_model_api-0.1.3/PKG-INFO` & `openvino_model_api-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openvino_model_api
-Version: 0.1.3
+Version: 0.1.4
 Summary: Model API: model wrappers and pipelines for inference with OpenVINO
 Home-page: https://github.com/openvinotoolkit/model_api
 Author: Intel(R) Corporation
 License: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `openvino_model_api-0.1.3/openvino_model_api.egg-info/PKG-INFO` & `openvino_model_api-0.1.4/openvino_model_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openvino-model-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: Model API: model wrappers and pipelines for inference with OpenVINO
 Home-page: https://github.com/openvinotoolkit/model_api
 Author: Intel(R) Corporation
 License: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `openvino_model_api-0.1.3/openvino_model_api.egg-info/SOURCES.txt` & `openvino_model_api-0.1.4/openvino_model_api.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/performance_metrics.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/adapters/__init__.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/adapters/inference_adapter.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/adapters/openvino_adapter.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/adapters/ovms_adapter.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/adapters/utils.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/models/__init__.py
+C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/models/anomaly.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/models/background_matting.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/models/bert.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/models/centernet.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/models/classification.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/models/ctpn.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/models/deblurring.py
 C:/Users/vzlobin/r/model_api/model_api/python/openvino/model_api/models/detection_model.py
```

### Comparing `openvino_model_api-0.1.3/setup.py` & `openvino_model_api-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from setuptools import find_packages, setup
 
 SETUP_DIR = Path(__file__).resolve().parent
 
 setup(
     name="openvino_model_api",
-    version="0.1.3",
+    version="0.1.4",
     description="Model API: model wrappers and pipelines for inference with OpenVINO",
     author="Intel(R) Corporation",
     url="https://github.com/openvinotoolkit/model_api",
     packages=find_packages(SETUP_DIR),
     package_dir={"openvino": str(SETUP_DIR / "openvino")},
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
```

