# Comparing `tmp/tomodachi_testcontainers-0.2.0.tar.gz` & `tmp/tomodachi_testcontainers-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomodachi_testcontainers-0.2.0.tar", max compression
+gzip compressed data, was "tomodachi_testcontainers-0.2.1.tar", max compression
```

## Comparing `tomodachi_testcontainers-0.2.0.tar` & `tomodachi_testcontainers-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.2.0/LICENSE
--rw-r--r--   0        0        0    26475 2023-07-27 14:17:21.581583 tomodachi_testcontainers-0.2.0/README.md
--rw-r--r--   0        0        0     3649 2023-07-27 14:17:30.478183 tomodachi_testcontainers-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/clients/__init__.py
--rw-r--r--   0        0        0     2300 2023-07-23 10:30:40.087069 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/clients/snssqs_client.py
--rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/__init__.py
--rw-r--r--   0        0        0     2185 2023-07-27 14:17:21.582366 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/common.py
--rw-r--r--   0        0        0     1818 2023-07-27 14:17:21.582876 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/localstack.py
--rw-r--r--   0        0        0     2085 2023-07-27 14:17:21.583252 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/moto.py
--rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/sftp.py
--rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/tomodachi.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/py.typed
--rw-r--r--   0        0        0     1346 2023-07-23 10:30:40.088641 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/__init__.py
--rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/assertions.py
--rw-r--r--   0        0        0     2290 2023-07-27 13:30:06.032389 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
--rw-r--r--   0        0        0     2109 2023-07-27 13:30:09.023818 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/moto_fixtures.py
--rw-r--r--   0        0        0     1594 2023-07-27 13:30:16.939169 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
--rw-r--r--   0        0        0      605 2023-07-23 10:30:40.089418 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
--rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/utils.py
--rw-r--r--   0        0        0    27664 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.2.1/LICENSE
+-rw-r--r--   0        0        0    26475 2023-07-27 14:17:21.581583 tomodachi_testcontainers-0.2.1/README.md
+-rw-r--r--   0        0        0     3649 2023-07-27 15:28:09.358579 tomodachi_testcontainers-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/clients/__init__.py
+-rw-r--r--   0        0        0     2300 2023-07-23 10:30:40.087069 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/clients/snssqs_client.py
+-rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/__init__.py
+-rw-r--r--   0        0        0     2918 2023-07-27 15:28:03.606413 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/common.py
+-rw-r--r--   0        0        0     1818 2023-07-27 14:17:21.582876 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/localstack.py
+-rw-r--r--   0        0        0     2085 2023-07-27 14:17:21.583252 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/moto.py
+-rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/sftp.py
+-rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/tomodachi.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/py.typed
+-rw-r--r--   0        0        0     1346 2023-07-23 10:30:40.088641 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/__init__.py
+-rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/assertions.py
+-rw-r--r--   0        0        0     2290 2023-07-27 13:30:06.032389 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
+-rw-r--r--   0        0        0     2109 2023-07-27 13:30:09.023818 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/moto_fixtures.py
+-rw-r--r--   0        0        0     1594 2023-07-27 13:30:16.939169 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
+-rw-r--r--   0        0        0      605 2023-07-23 10:30:40.089418 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
+-rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/utils.py
+-rw-r--r--   0        0        0    27664 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.2.1/PKG-INFO
```

### Comparing `tomodachi_testcontainers-0.2.0/LICENSE` & `tomodachi_testcontainers-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/README.md` & `tomodachi_testcontainers-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/pyproject.toml` & `tomodachi_testcontainers-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomodachi-testcontainers"
-version = "0.2.0"
+version = "0.2.1"
 description = "Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing."
 authors = ["Filips Nastins <nastinsfilips@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/filipsnastins/tomodachi-testcontainers"
 repository = "https://github.com/filipsnastins/tomodachi-testcontainers"
```

### Comparing `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/clients/snssqs_client.py` & `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/clients/snssqs_client.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/__init__.py` & `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/common.py` & `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,42 @@
 import pathlib
 from typing import Any, Dict, Iterator, Optional, Tuple, cast
 
 import testcontainers.core.container
 from docker.errors import ImageNotFound
 from docker.models.images import Image as DockerImage
 from testcontainers.core.docker_client import DockerClient
+from testcontainers.core.utils import inside_container
 
 
 class DockerContainer(testcontainers.core.container.DockerContainer):
     def __init__(self, *args: Any, network: Optional[str] = None, **kwargs: Any) -> None:
         self.network = network or os.getenv("TESTCONTAINER_DOCKER_NETWORK", "bridge")
         super().__init__(*args, **kwargs, network=self.network)
 
+    def get_container_host_ip(self) -> str:
+        host = self.get_docker_client().host()
+        if not host:
+            return "localhost"
+
+        if inside_container() and not os.getenv("DOCKER_HOST"):
+            gateway_ip = self.get_container_gateway_ip()
+            if gateway_ip == host:
+                return self.get_container_internal_ip()
+            return gateway_ip
+        return host
+
     def get_container_internal_ip(self) -> str:
         container = self.get_docker_client().get_container(self.get_wrapped_container().id)
         return container["NetworkSettings"]["Networks"][self.network]["IPAddress"]
 
+    def get_container_gateway_ip(self) -> str:
+        container = self.get_docker_client().get_container(self.get_wrapped_container().id)
+        return container["NetworkSettings"]["Networks"][self.network]["Gateway"]
+
 
 class EphemeralDockerImage:
     def __init__(self, dockerfile: pathlib.Path, docker_client_kw: Optional[Dict] = None) -> None:
         self.client = DockerClient(**(docker_client_kw or {}))
         self.image = self.build_image(dockerfile)
 
     def __enter__(self) -> DockerImage:
@@ -54,8 +71,8 @@
 def get_docker_image(image_id: str, docker_client_kw: Optional[Dict] = None) -> Optional[DockerImage]:
     client = DockerClient(**(docker_client_kw or {}))
     if not image_id:
         return None
     try:
         return cast(DockerImage, client.client.images.get(image_id))
     except ImageNotFound:
-        return None
+        return cast(DockerImage, client.client.images.pull(image_id))
```

### Comparing `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/localstack.py` & `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/localstack.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/moto.py` & `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/moto.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/sftp.py` & `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/sftp.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/tomodachi.py` & `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/containers/tomodachi.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/__init__.py` & `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/localstack_fixtures.py` & `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/localstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/moto_fixtures.py` & `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/moto_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/sftp_fixtures.py` & `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/sftp_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py` & `tomodachi_testcontainers-0.2.1/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.2.0/PKG-INFO` & `tomodachi_testcontainers-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomodachi-testcontainers
-Version: 0.2.0
+Version: 0.2.1
 Summary: Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing.
 Home-page: https://github.com/filipsnastins/tomodachi-testcontainers
 License: MIT
 Author: Filips Nastins
 Author-email: nastinsfilips@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

