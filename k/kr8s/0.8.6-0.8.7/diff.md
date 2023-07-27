# Comparing `tmp/kr8s-0.8.6.tar.gz` & `tmp/kr8s-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.8.6.tar", max compression
+gzip compressed data, was "kr8s-0.8.7.tar", max compression
```

## Comparing `kr8s-0.8.6.tar` & `kr8s-0.8.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1549 2023-07-13 15:15:48.461707 kr8s-0.8.6/LICENSE
--rw-r--r--   0        0        0     2587 2023-07-13 15:15:48.461707 kr8s-0.8.6/README.md
--rw-r--r--   0        0        0     1143 2023-07-13 15:16:17.577447 kr8s-0.8.6/kr8s/__init__.py
--rw-r--r--   0        0        0    14674 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_api.py
--rw-r--r--   0        0        0     5879 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_auth.py
--rw-r--r--   0        0        0     1920 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_exceptions.py
--rw-r--r--   0        0        0     4336 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_io.py
--rw-r--r--   0        0        0    36589 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_objects.py
--rw-r--r--   0        0        0     8074 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_testutils.py
--rw-r--r--   0        0        0      248 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0     1110 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0     1681 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/asyncio/_helpers.py
--rw-r--r--   0        0        0      827 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0      168 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5503 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/conftest.py
--rw-r--r--   0        0        0     6001 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/objects.py
--rw-r--r--   0        0        0      152 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/portforward.py
--rw-r--r--   0        0        0       78 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/resources/custom/evc.yaml
--rw-r--r--   0        0        0       61 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/resources/serviceaccount.yaml
--rw-r--r--   0        0        0      369 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
--rw-r--r--   0        0        0      144 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/resources/simple/nginx_pod.yaml
--rw-r--r--   0        0        0      435 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/resources/simple/nginx_pod_service.yaml
--rwxr-xr-x   0        0        0      614 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     5909 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3394 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      824 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0     1710 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/test_io.py
--rw-r--r--   0        0        0    21028 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2676 2023-07-13 15:16:17.577447 kr8s-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 kr8s-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-07-27 15:57:43.772847 kr8s-0.8.7/LICENSE
+-rw-r--r--   0        0        0     2587 2023-07-27 15:57:43.772847 kr8s-0.8.7/README.md
+-rw-r--r--   0        0        0     1143 2023-07-27 15:58:16.827524 kr8s-0.8.7/kr8s/__init__.py
+-rw-r--r--   0        0        0    14674 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_api.py
+-rw-r--r--   0        0        0     6266 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_auth.py
+-rw-r--r--   0        0        0     1920 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_exceptions.py
+-rw-r--r--   0        0        0     4336 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_io.py
+-rw-r--r--   0        0        0    36828 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_objects.py
+-rw-r--r--   0        0        0     8074 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/_testutils.py
+-rw-r--r--   0        0        0      248 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0     1681 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/asyncio/_helpers.py
+-rw-r--r--   0        0        0      827 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0      168 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5503 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/conftest.py
+-rw-r--r--   0        0        0     6001 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/objects.py
+-rw-r--r--   0        0        0      152 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/portforward.py
+-rw-r--r--   0        0        0       78 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/tests/resources/custom/evc.yaml
+-rw-r--r--   0        0        0       61 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/tests/resources/serviceaccount.yaml
+-rw-r--r--   0        0        0      369 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
+-rw-r--r--   0        0        0      144 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/tests/resources/simple/nginx_pod.yaml
+-rw-r--r--   0        0        0      435 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/tests/resources/simple/nginx_pod_service.yaml
+-rwxr-xr-x   0        0        0      614 2023-07-27 15:57:43.792848 kr8s-0.8.7/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     5909 2023-07-27 15:57:43.796848 kr8s-0.8.7/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3394 2023-07-27 15:57:43.796848 kr8s-0.8.7/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      824 2023-07-27 15:57:43.796848 kr8s-0.8.7/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0     1710 2023-07-27 15:57:43.796848 kr8s-0.8.7/kr8s/tests/test_io.py
+-rw-r--r--   0        0        0    21028 2023-07-27 15:57:43.796848 kr8s-0.8.7/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-07-27 15:57:43.796848 kr8s-0.8.7/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2676 2023-07-27 15:58:16.827524 kr8s-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 kr8s-0.8.7/PKG-INFO
```

### Comparing `kr8s-0.8.6/LICENSE` & `kr8s-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/README.md` & `kr8s-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/__init__.py` & `kr8s-0.8.7/kr8s/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .asyncio import (
     version as _version,
 )
 from .asyncio import (
     watch as _watch,
 )
 
-__version__ = "0.8.6"
+__version__ = "0.8.7"
 
 
 @_sync
 class Api(_AsyncApi):
     __doc__ = _AsyncApi.__doc__
```

### Comparing `kr8s-0.8.6/kr8s/_api.py` & `kr8s-0.8.7/kr8s/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/_auth.py` & `kr8s-0.8.7/kr8s/_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,15 +129,22 @@
             self.token = self._user["token"]
         if "username" in self._user:
             self.username = self._user["username"]
         if "password" in self._user:
             self.password = self._user["password"]
         if self.namespace is None:
             self.namespace = self._context.get("namespace", "default")
-        # TODO: Handle auth-provider oidc auth
+        if "auth-provider" in self._user:
+            if p := self._user["auth-provider"]["name"] != "oidc":
+                raise ValueError(
+                    f"auth-provider {p} was deprecated in Kubernetes 1.21 "
+                    "and is not supported by kr8s"
+                )
+            # TODO: Handle refreshing OIDC token if missing or expired
+            self.token = self._user["auth-provider"]["config"]["id-token"]
 
     async def _load_service_account(self) -> None:
         """Load credentials from service account."""
         self._serviceaccount = os.path.expanduser(self._serviceaccount)
         if not os.path.isdir(self._serviceaccount):
             return
         host = os.environ["KUBERNETES_SERVICE_HOST"]
```

### Comparing `kr8s-0.8.6/kr8s/_data_utils.py` & `kr8s-0.8.7/kr8s/_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/_io.py` & `kr8s-0.8.7/kr8s/_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/_objects.py` & `kr8s-0.8.7/kr8s/_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,23 +267,28 @@
         await self._patch(patch, subresource=subresource)
 
     async def _patch(self, patch: Dict, *, subresource=None) -> None:
         """Patch this object in Kubernetes."""
         url = f"{self.endpoint}/{self.name}"
         if subresource:
             url = f"{url}/{subresource}"
-        async with self.api.call_api(
-            "PATCH",
-            version=self.version,
-            url=url,
-            namespace=self.namespace,
-            data=json.dumps(patch),
-            headers={"Content-Type": "application/merge-patch+json"},
-        ) as resp:
-            self.raw = resp.json()
+        try:
+            async with self.api.call_api(
+                "PATCH",
+                version=self.version,
+                url=url,
+                namespace=self.namespace,
+                data=json.dumps(patch),
+                headers={"Content-Type": "application/merge-patch+json"},
+            ) as resp:
+                self.raw = resp.json()
+        except httpx.HTTPStatusError as e:
+            if e.response.status_code == 404:
+                raise NotFoundError(f"Object {self.name} does not exist") from e
+            raise e
 
     async def scale(self, replicas: int = None) -> None:
         """Scale this object in Kubernetes."""
         if not self.scalable:
             raise NotImplementedError(f"{self.kind} is not scalable")
         await self._exists(ensure=True)
         await self._patch({"spec": dot_to_nested_dict(self.scalable_spec, replicas)})
```

### Comparing `kr8s-0.8.6/kr8s/_portforward.py` & `kr8s-0.8.7/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/_testutils.py` & `kr8s-0.8.7/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/asyncio/_api.py` & `kr8s-0.8.7/kr8s/asyncio/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/asyncio/_helpers.py` & `kr8s-0.8.7/kr8s/asyncio/_helpers.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/asyncio/objects.py` & `kr8s-0.8.7/kr8s/asyncio/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/conftest.py` & `kr8s-0.8.7/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/objects.py` & `kr8s-0.8.7/kr8s/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/tests/scripts/envexec.py` & `kr8s-0.8.7/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/tests/test_api.py` & `kr8s-0.8.7/kr8s/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/tests/test_auth.py` & `kr8s-0.8.7/kr8s/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/tests/test_data_utils.py` & `kr8s-0.8.7/kr8s/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/tests/test_io.py` & `kr8s-0.8.7/kr8s/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/tests/test_objects.py` & `kr8s-0.8.7/kr8s/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/kr8s/tests/test_testutils.py` & `kr8s-0.8.7/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.6/pyproject.toml` & `kr8s-0.8.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.8.6"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.8.7"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = true
```

### Comparing `kr8s-0.8.6/PKG-INFO` & `kr8s-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.8.6
+Version: 0.8.7
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

