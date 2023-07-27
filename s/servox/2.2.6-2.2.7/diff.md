# Comparing `tmp/servox-2.2.6.tar.gz` & `tmp/servox-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servox-2.2.6.tar", max compression
+gzip compressed data, was "servox-2.2.7.tar", max compression
```

## Comparing `servox-2.2.6.tar` & `servox-2.2.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    36555 2023-07-10 18:52:10.512874 servox-2.2.6/CHANGELOG.md
--rw-r--r--   0        0        0    11385 2023-07-10 18:52:10.512874 servox-2.2.6/LICENSE
--rw-r--r--   0        0        0    51279 2023-07-10 18:52:10.512874 servox-2.2.6/README.md
--rw-r--r--   0        0        0     3639 2023-07-10 18:52:10.516873 servox-2.2.6/pyproject.toml
--rw-r--r--   0        0        0     1832 2023-07-10 18:52:10.516873 servox-2.2.6/servo/__init__.py
--rw-r--r--   0        0        0    10136 2023-07-10 18:52:10.516873 servox-2.2.6/servo/api.py
--rw-r--r--   0        0        0    15480 2023-07-10 18:52:10.516873 servox-2.2.6/servo/assembly.py
--rw-r--r--   0        0        0    44344 2023-07-10 18:52:10.516873 servox-2.2.6/servo/checks.py
--rw-r--r--   0        0        0    78505 2023-07-10 18:52:10.520873 servox-2.2.6/servo/cli.py
--rw-r--r--   0        0        0    28118 2023-07-10 18:52:10.520873 servox-2.2.6/servo/configuration.py
--rw-r--r--   0        0        0    16845 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connector.py
--rw-r--r--   0        0        0      680 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/__init__.py
--rw-r--r--   0        0        0    31949 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kube_metrics.py
--rw-r--r--   0        0        0    95520 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes.py
--rw-r--r--   0        0        0      799 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/__init__.py
--rw-r--r--   0        0        0     2528 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/base.py
--rw-r--r--   0        0        0    11264 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/base_workload.py
--rw-r--r--   0        0        0     5158 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/container.py
--rw-r--r--   0        0        0    14837 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/deployment.py
--rw-r--r--   0        0        0     1195 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/namespace.py
--rw-r--r--   0        0        0    12193 2023-07-10 18:52:10.520873 servox-2.2.6/servo/connectors/kubernetes_helpers/pod.py
--rw-r--r--   0        0        0     1779 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/kubernetes_helpers/replicaset.py
--rw-r--r--   0        0        0     2722 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/kubernetes_helpers/service.py
--rw-r--r--   0        0        0     3702 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/kubernetes_helpers/statefulset.py
--rw-r--r--   0        0        0     1625 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/kubernetes_helpers/util.py
--rw-r--r--   0        0        0    47402 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/opsani_dev.py
--rw-r--r--   0        0        0    40511 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/prometheus.py
--rw-r--r--   0        0        0     1708 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/scripts.py
--rw-r--r--   0        0        0    19127 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/vegeta.py
--rw-r--r--   0        0        0      983 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/vegeta_target_schema.json
--rw-r--r--   0        0        0     2665 2023-07-10 18:52:10.524874 servox-2.2.6/servo/connectors/wait.py
--rw-r--r--   0        0        0      607 2023-07-10 18:52:10.524874 servox-2.2.6/servo/encoders.py
--rw-r--r--   0        0        0     1771 2023-07-10 18:52:10.524874 servox-2.2.6/servo/entry_points.py
--rw-r--r--   0        0        0     5459 2023-07-10 18:52:10.524874 servox-2.2.6/servo/errors.py
--rw-r--r--   0        0        0    38440 2023-07-10 18:52:10.524874 servox-2.2.6/servo/events.py
--rw-r--r--   0        0        0    10685 2023-07-10 18:52:10.524874 servox-2.2.6/servo/fast_fail.py
--rw-r--r--   0        0        0    14253 2023-07-10 18:52:10.524874 servox-2.2.6/servo/logging.py
--rw-r--r--   0        0        0    61151 2023-07-10 18:52:10.524874 servox-2.2.6/servo/pubsub.py
--rw-r--r--   0        0        0     6750 2023-07-10 18:52:10.524874 servox-2.2.6/servo/repeating.py
--rw-r--r--   0        0        0    29014 2023-07-10 18:52:10.524874 servox-2.2.6/servo/runner.py
--rw-r--r--   0        0        0    26050 2023-07-10 18:52:10.524874 servox-2.2.6/servo/servo.py
--rw-r--r--   0        0        0     7891 2023-07-10 18:52:10.524874 servox-2.2.6/servo/telemetry.py
--rw-r--r--   0        0        0      808 2023-07-10 18:52:10.524874 servox-2.2.6/servo/types/__init__.py
--rw-r--r--   0        0        0    10891 2023-07-10 18:52:10.524874 servox-2.2.6/servo/types/api.py
--rw-r--r--   0        0        0    32100 2023-07-10 18:52:10.524874 servox-2.2.6/servo/types/core.py
--rw-r--r--   0        0        0     2232 2023-07-10 18:52:10.524874 servox-2.2.6/servo/types/kubernetes.py
--rw-r--r--   0        0        0    23824 2023-07-10 18:52:10.524874 servox-2.2.6/servo/types/settings.py
--rw-r--r--   0        0        0     4575 2023-07-10 18:52:10.524874 servox-2.2.6/servo/types/slo.py
--rw-r--r--   0        0        0      777 2023-07-10 18:52:10.524874 servox-2.2.6/servo/utilities/__init__.py
--rw-r--r--   0        0        0     2854 2023-07-10 18:52:10.524874 servox-2.2.6/servo/utilities/associations.py
--rw-r--r--   0        0        0     5404 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/duration_str.py
--rw-r--r--   0        0        0     2314 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/hashing.py
--rw-r--r--   0        0        0    17660 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/inspect.py
--rw-r--r--   0        0        0     2116 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/key_paths.py
--rw-r--r--   0        0        0     2427 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/pydantic.py
--rw-r--r--   0        0        0     2529 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/strings.py
--rw-r--r--   0        0        0    15189 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/subprocess.py
--rw-r--r--   0        0        0     1016 2023-07-10 18:52:10.528874 servox-2.2.6/servo/utilities/yaml.py
--rw-r--r--   0        0        0    52862 1970-01-01 00:00:00.000000 servox-2.2.6/PKG-INFO
+-rw-r--r--   0        0        0    36945 2023-07-27 19:19:05.091898 servox-2.2.7/CHANGELOG.md
+-rw-r--r--   0        0        0    11385 2023-07-27 19:19:05.091898 servox-2.2.7/LICENSE
+-rw-r--r--   0        0        0    51279 2023-07-27 19:19:05.091898 servox-2.2.7/README.md
+-rw-r--r--   0        0        0     3639 2023-07-27 19:19:05.095898 servox-2.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1832 2023-07-27 19:19:05.095898 servox-2.2.7/servo/__init__.py
+-rw-r--r--   0        0        0    10136 2023-07-27 19:19:05.095898 servox-2.2.7/servo/api.py
+-rw-r--r--   0        0        0    15480 2023-07-27 19:19:05.095898 servox-2.2.7/servo/assembly.py
+-rw-r--r--   0        0        0    44344 2023-07-27 19:19:05.095898 servox-2.2.7/servo/checks.py
+-rw-r--r--   0        0        0    78505 2023-07-27 19:19:05.095898 servox-2.2.7/servo/cli.py
+-rw-r--r--   0        0        0    28118 2023-07-27 19:19:05.095898 servox-2.2.7/servo/configuration.py
+-rw-r--r--   0        0        0    16845 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connector.py
+-rw-r--r--   0        0        0      680 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/__init__.py
+-rw-r--r--   0        0        0    31949 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kube_metrics.py
+-rw-r--r--   0        0        0    95802 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kubernetes.py
+-rw-r--r--   0        0        0      799 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kubernetes_helpers/__init__.py
+-rw-r--r--   0        0        0     2528 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kubernetes_helpers/base.py
+-rw-r--r--   0        0        0    11264 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kubernetes_helpers/base_workload.py
+-rw-r--r--   0        0        0     5158 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kubernetes_helpers/container.py
+-rw-r--r--   0        0        0    14837 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kubernetes_helpers/deployment.py
+-rw-r--r--   0        0        0     1195 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kubernetes_helpers/namespace.py
+-rw-r--r--   0        0        0    12193 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kubernetes_helpers/pod.py
+-rw-r--r--   0        0        0     1779 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kubernetes_helpers/replicaset.py
+-rw-r--r--   0        0        0     2722 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kubernetes_helpers/service.py
+-rw-r--r--   0        0        0     3702 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kubernetes_helpers/statefulset.py
+-rw-r--r--   0        0        0     1625 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/kubernetes_helpers/util.py
+-rw-r--r--   0        0        0    47402 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/opsani_dev.py
+-rw-r--r--   0        0        0    40511 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/prometheus.py
+-rw-r--r--   0        0        0     1708 2023-07-27 19:19:05.099898 servox-2.2.7/servo/connectors/scripts.py
+-rw-r--r--   0        0        0    19127 2023-07-27 19:19:05.103898 servox-2.2.7/servo/connectors/vegeta.py
+-rw-r--r--   0        0        0      983 2023-07-27 19:19:05.103898 servox-2.2.7/servo/connectors/vegeta_target_schema.json
+-rw-r--r--   0        0        0     2665 2023-07-27 19:19:05.103898 servox-2.2.7/servo/connectors/wait.py
+-rw-r--r--   0        0        0      607 2023-07-27 19:19:05.103898 servox-2.2.7/servo/encoders.py
+-rw-r--r--   0        0        0     1771 2023-07-27 19:19:05.103898 servox-2.2.7/servo/entry_points.py
+-rw-r--r--   0        0        0     5459 2023-07-27 19:19:05.103898 servox-2.2.7/servo/errors.py
+-rw-r--r--   0        0        0    38440 2023-07-27 19:19:05.103898 servox-2.2.7/servo/events.py
+-rw-r--r--   0        0        0    10685 2023-07-27 19:19:05.103898 servox-2.2.7/servo/fast_fail.py
+-rw-r--r--   0        0        0    14410 2023-07-27 19:19:05.103898 servox-2.2.7/servo/logging.py
+-rw-r--r--   0        0        0    61151 2023-07-27 19:19:05.103898 servox-2.2.7/servo/pubsub.py
+-rw-r--r--   0        0        0     6750 2023-07-27 19:19:05.103898 servox-2.2.7/servo/repeating.py
+-rw-r--r--   0        0        0    29626 2023-07-27 19:19:05.103898 servox-2.2.7/servo/runner.py
+-rw-r--r--   0        0        0    26050 2023-07-27 19:19:05.103898 servox-2.2.7/servo/servo.py
+-rw-r--r--   0        0        0     7891 2023-07-27 19:19:05.103898 servox-2.2.7/servo/telemetry.py
+-rw-r--r--   0        0        0      808 2023-07-27 19:19:05.103898 servox-2.2.7/servo/types/__init__.py
+-rw-r--r--   0        0        0    10891 2023-07-27 19:19:05.103898 servox-2.2.7/servo/types/api.py
+-rw-r--r--   0        0        0    32100 2023-07-27 19:19:05.103898 servox-2.2.7/servo/types/core.py
+-rw-r--r--   0        0        0     2232 2023-07-27 19:19:05.103898 servox-2.2.7/servo/types/kubernetes.py
+-rw-r--r--   0        0        0    23824 2023-07-27 19:19:05.103898 servox-2.2.7/servo/types/settings.py
+-rw-r--r--   0        0        0     4575 2023-07-27 19:19:05.103898 servox-2.2.7/servo/types/slo.py
+-rw-r--r--   0        0        0      777 2023-07-27 19:19:05.103898 servox-2.2.7/servo/utilities/__init__.py
+-rw-r--r--   0        0        0     2854 2023-07-27 19:19:05.103898 servox-2.2.7/servo/utilities/associations.py
+-rw-r--r--   0        0        0     5404 2023-07-27 19:19:05.103898 servox-2.2.7/servo/utilities/duration_str.py
+-rw-r--r--   0        0        0     2314 2023-07-27 19:19:05.103898 servox-2.2.7/servo/utilities/hashing.py
+-rw-r--r--   0        0        0    17660 2023-07-27 19:19:05.103898 servox-2.2.7/servo/utilities/inspect.py
+-rw-r--r--   0        0        0     2116 2023-07-27 19:19:05.103898 servox-2.2.7/servo/utilities/key_paths.py
+-rw-r--r--   0        0        0     2427 2023-07-27 19:19:05.103898 servox-2.2.7/servo/utilities/pydantic.py
+-rw-r--r--   0        0        0     2529 2023-07-27 19:19:05.103898 servox-2.2.7/servo/utilities/strings.py
+-rw-r--r--   0        0        0    15189 2023-07-27 19:19:05.103898 servox-2.2.7/servo/utilities/subprocess.py
+-rw-r--r--   0        0        0     1016 2023-07-27 19:19:05.103898 servox-2.2.7/servo/utilities/yaml.py
+-rw-r--r--   0        0        0    52862 1970-01-01 00:00:00.000000 servox-2.2.7/PKG-INFO
```

### Comparing `servox-2.2.6/CHANGELOG.md` & `servox-2.2.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 Servo is distributed under the terms of the Apache 2.0 license.
 
 This changelog catalogs all notable changes made to the project. The format is
 based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/). Releases are
 versioned in accordance with [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.2.7] "genesis" - 2023-07-27
+
+### Changed
+
+- Progress reporting queue is cleared on command completion to prevent stale progress from being sent when pileup occurs [544](https://github.com/opsani/servox/pull/544)
+- Memory parsing logic treats unitless decimal strings as GiB (aligns with existing float parsing) per the servo protocol [546](https://github.com/opsani/servox/pull/546)
+
 ## [2.2.6] "genesis" - 2023-07-10
 
 ### Changed
 
 - A unique identifier for each servo deployment is now supported in configuration and sent with every request to the backend
 - A unique identifier for each command received from the backend is now retrieved from the response to the WHATS_NEXT request and included on all servo requests for the given command (progress and completion)
```

### Comparing `servox-2.2.6/LICENSE` & `servox-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/README.md` & `servox-2.2.7/README.md`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/pyproject.toml` & `servox-2.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servox"
-version = "2.2.6"
+version = "2.2.7"
 description = "Opsani Servo: The Next Generation"
 homepage = "https://opsani.com/"
 repository = "https://github.com/opsani/servox"
 authors = ["Blake Watters <blake@opsani.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [
```

### Comparing `servox-2.2.6/servo/__init__.py` & `servox-2.2.7/servo/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/api.py` & `servox-2.2.7/servo/api.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/assembly.py` & `servox-2.2.7/servo/assembly.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/checks.py` & `servox-2.2.7/servo/checks.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/cli.py` & `servox-2.2.7/servo/cli.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/configuration.py` & `servox-2.2.7/servo/configuration.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connector.py` & `servox-2.2.7/servo/connector.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/__init__.py` & `servox-2.2.7/servo/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/kube_metrics.py` & `servox-2.2.7/servo/connectors/kube_metrics.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/kubernetes.py` & `servox-2.2.7/servo/connectors/kubernetes.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,20 +219,25 @@
 
 class ShortByteSize(pydantic.ByteSize):
     """Kubernetes omits the 'B' suffix for some reason"""
 
     @classmethod
     def validate(cls, v: pydantic.StrIntFloat) -> "ShortByteSize":
         if isinstance(v, str):
+            # Unitless decimals are not use by k8s API but are used in servo protocol implicitly as GiB
+            if re.match(r"^\d*\.\d+$", v):
+                v = f"{v}GiB"
+
             try:
                 return super().validate(v)
             except:
                 # Append the byte suffix and retry parsing
                 return super().validate(v + "b")
         elif isinstance(v, float):
+            # Unitless decimals are not use by k8s API but are used in servo protocol implicitly as GiB
             v = v * GiB
         return super().validate(v)
 
     def human_readable(self) -> str:
         """NOTE: only represents precision up to 1 decimal place (see pydantic's human_readable)"""
         sup = super().human_readable()
         # Remove the 'B' suffix to align with Kubernetes units (`GiB` -> `Gi`)
```

### Comparing `servox-2.2.6/servo/connectors/kubernetes_helpers/__init__.py` & `servox-2.2.7/servo/connectors/kubernetes_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/kubernetes_helpers/base.py` & `servox-2.2.7/servo/connectors/kubernetes_helpers/base.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/kubernetes_helpers/base_workload.py` & `servox-2.2.7/servo/connectors/kubernetes_helpers/base_workload.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/kubernetes_helpers/container.py` & `servox-2.2.7/servo/connectors/kubernetes_helpers/container.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/kubernetes_helpers/deployment.py` & `servox-2.2.7/servo/connectors/kubernetes_helpers/deployment.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/kubernetes_helpers/namespace.py` & `servox-2.2.7/servo/connectors/kubernetes_helpers/namespace.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/kubernetes_helpers/pod.py` & `servox-2.2.7/servo/connectors/kubernetes_helpers/pod.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/kubernetes_helpers/replicaset.py` & `servox-2.2.7/servo/connectors/kubernetes_helpers/replicaset.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/kubernetes_helpers/service.py` & `servox-2.2.7/servo/connectors/kubernetes_helpers/service.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/kubernetes_helpers/statefulset.py` & `servox-2.2.7/servo/connectors/kubernetes_helpers/statefulset.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/kubernetes_helpers/util.py` & `servox-2.2.7/servo/connectors/kubernetes_helpers/util.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/opsani_dev.py` & `servox-2.2.7/servo/connectors/opsani_dev.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/prometheus.py` & `servox-2.2.7/servo/connectors/prometheus.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/scripts.py` & `servox-2.2.7/servo/connectors/scripts.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/vegeta.py` & `servox-2.2.7/servo/connectors/vegeta.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/vegeta_target_schema.json` & `servox-2.2.7/servo/connectors/vegeta_target_schema.json`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/connectors/wait.py` & `servox-2.2.7/servo/connectors/wait.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/encoders.py` & `servox-2.2.7/servo/encoders.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/entry_points.py` & `servox-2.2.7/servo/entry_points.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/errors.py` & `servox-2.2.7/servo/errors.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/events.py` & `servox-2.2.7/servo/events.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/fast_fail.py` & `servox-2.2.7/servo/fast_fail.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/logging.py` & `servox-2.2.7/servo/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,19 @@
                 event_context=event_context,
                 started_at=started_at,
                 message=message,
                 command_uid=command_uid,
             )
         )
 
+    def clear_progress_queue(self) -> None:
+        while not self._queue.empty():
+            self._queue.get_nowait()
+            self._queue.task_done()
+
     async def shutdown(self) -> None:
         """Shutdown the progress handler by emptying the queue and releasing the queue processor."""
         await self._queue.join()
 
         if self._queue_processor:
             self._queue_processor.cancel()
             await asyncio.gather(self._queue_processor, return_exceptions=True)
```

### Comparing `servox-2.2.6/servo/pubsub.py` & `servox-2.2.7/servo/pubsub.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/repeating.py` & `servox-2.2.7/servo/repeating.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/runner.py` & `servox-2.2.7/servo/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,27 +38,31 @@
 import servo.utilities.strings
 from servo.servo import _set_current_servo, set_current_command_uid
 from servo.types import Adjustment, Control, Description, Duration, Measurement
 
 
 class ServoRunner(pydantic.BaseModel, servo.logging.Mixin):
     interactive: bool = False
+    _assembly_runner: AssemblyRunner = pydantic.PrivateAttr(None)
     _servo: servo.Servo = pydantic.PrivateAttr(None)
     _connected: bool = pydantic.PrivateAttr(False)
     _running: bool = pydantic.PrivateAttr(False)
     _main_loop_task: Optional[asyncio.Task] = pydantic.PrivateAttr(None)
     _diagnostics_loop_task: Optional[asyncio.Task] = pydantic.PrivateAttr(None)
     _file_watcher_task: Optional[asyncio.Task] = pydantic.PrivateAttr(None)
 
     class Config:
         arbitrary_types_allowed = True
 
-    def __init__(self, servo_: servo, **kwargs) -> None:  # noqa: D10
+    def __init__(
+        self, servo_: servo, _assembly_runner: AssemblyRunner = None, **kwargs
+    ) -> None:  # noqa: D10
         super().__init__(**kwargs)
         self._servo = servo_
+        self._assembly_runner = _assembly_runner
 
         # initialize default servo options if not configured
         if self.config.settings is None:
             self.config.settings = servo.CommonConfiguration()
 
     @property
     def servo(self) -> servo.Servo:
@@ -151,14 +155,15 @@
             )
             self.logger.debug(devtools.pformat(description))
 
             status = servo.api.Status.ok(
                 descriptor=description.__opsani_repr__(),
                 command_uid=cmd_response.command_uid,
             )
+            self.clear_progress_queue()
             return await self.servo.post_event(servo.api.Events.describe, status.dict())
 
         elif cmd_response.command == servo.api.Commands.measure:
             try:
                 measurement = await self.measure(cmd_response.param)
                 self.logger.success(
                     f"Measured: {len(measurement.readings)} readings, {len(measurement.annotations)} annotations"
@@ -173,14 +178,15 @@
                 status = servo.api.Status.from_error(
                     error=error,
                     command_uid=cmd_response.command_uid,
                 )
                 self.logger.error(f"Responding with {status.dict()}")
                 self.logger.opt(exception=error).debug("Measure failure details")
 
+            self.clear_progress_queue()
             return await self.servo.post_event(servo.api.Events.measure, status.dict())
 
         elif cmd_response.command == servo.api.Commands.adjust:
             adjustments = servo.api.descriptor_to_adjustments(
                 cmd_response.param["state"]
             )
             control = Control(**cmd_response.param.get("control", {}))
@@ -204,14 +210,15 @@
                 status = servo.api.Status.from_error(
                     error,
                     command_uid=cmd_response.command_uid,
                 )
                 self.logger.error(f"Responding with {status.dict()}")
                 self.logger.opt(exception=error).debug("Adjust failure details")
 
+            self.clear_progress_queue()
             return await self.servo.post_event(servo.api.Events.adjust, status.dict())
 
         elif cmd_response.command == servo.api.Commands.sleep:
             # TODO: Model this
             duration = Duration(cmd_response.param.get("duration", 120))
             status = servo.utilities.key_paths.value_for_key_path(
                 cmd_response.param, "data.status", None
@@ -400,14 +407,19 @@
             if self.connected:
                 await self.servo.post_event(
                     servo.api.Events.goodbye, dict(reason=reason)
                 )
         except Exception:
             self.logger.exception(f"Exception occurred during GOODBYE request")
 
+    def clear_progress_queue(self) -> None:
+        if self._assembly_runner and self._assembly_runner.progress_handler:
+            self.logger.debug("Clearing progress handler queue")
+            self._assembly_runner.progress_handler.clear_progress_queue()
+
 
 class AssemblyRunner(pydantic.BaseModel, servo.logging.Mixin):
     assembly: servo.Assembly
     runners: list[ServoRunner] = []
     progress_handler: Optional[servo.logging.ProgressHandler] = None
     progress_handler_id: Optional[int] = None
     _running: bool = pydantic.PrivateAttr(False)
@@ -531,15 +543,17 @@
         )
         self.progress_handler_id = self.logger.add(self.progress_handler.sink)
 
         self._display_banner()
 
         try:
             for servo_ in self.assembly.servos:
-                servo_runner = ServoRunner(servo_, interactive=interactive)
+                servo_runner = ServoRunner(
+                    servo_, interactive=interactive, _assembly_runner=self
+                )
                 loop.create_task(servo_runner.run(poll=poll))
                 self.runners.append(servo_runner)
 
             loop.run_forever()
 
         finally:
             loop.close()
```

### Comparing `servox-2.2.6/servo/servo.py` & `servox-2.2.7/servo/servo.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/telemetry.py` & `servox-2.2.7/servo/telemetry.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/types/__init__.py` & `servox-2.2.7/servo/types/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/types/api.py` & `servox-2.2.7/servo/types/api.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/types/core.py` & `servox-2.2.7/servo/types/core.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/types/kubernetes.py` & `servox-2.2.7/servo/types/kubernetes.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/types/settings.py` & `servox-2.2.7/servo/types/settings.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/types/slo.py` & `servox-2.2.7/servo/types/slo.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/utilities/__init__.py` & `servox-2.2.7/servo/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/utilities/associations.py` & `servox-2.2.7/servo/utilities/associations.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/utilities/duration_str.py` & `servox-2.2.7/servo/utilities/duration_str.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/utilities/hashing.py` & `servox-2.2.7/servo/utilities/hashing.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/utilities/inspect.py` & `servox-2.2.7/servo/utilities/inspect.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/utilities/key_paths.py` & `servox-2.2.7/servo/utilities/key_paths.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/utilities/pydantic.py` & `servox-2.2.7/servo/utilities/pydantic.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/utilities/strings.py` & `servox-2.2.7/servo/utilities/strings.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/utilities/subprocess.py` & `servox-2.2.7/servo/utilities/subprocess.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/servo/utilities/yaml.py` & `servox-2.2.7/servo/utilities/yaml.py`

 * *Files identical despite different names*

### Comparing `servox-2.2.6/PKG-INFO` & `servox-2.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servox
-Version: 2.2.6
+Version: 2.2.7
 Summary: Opsani Servo: The Next Generation
 Home-page: https://opsani.com/
 License: Apache-2.0
 Author: Blake Watters
 Author-email: blake@opsani.com
 Requires-Python: >=3.8.1,<=3.9.11
 Classifier: License :: OSI Approved :: Apache Software License
```

