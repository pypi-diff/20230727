# Comparing `tmp/kube_ops-1.0.2-py3-none-any.whl.zip` & `tmp/kube_ops-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18964 bytes, number of entries: 12
+Zip file size: 18992 bytes, number of entries: 12
 -rw-r--r--  2.0 unx     1310 b- defN 23-Jul-23 11:51 kube/__init__.py
 -rw-r--r--  2.0 unx    32538 b- defN 23-Jul-23 05:31 kube/api.py
 -rw-r--r--  2.0 unx     2611 b- defN 23-Jul-23 07:44 kube/common.py
--rw-r--r--  2.0 unx     5080 b- defN 23-Jul-23 11:51 kube/config.py
+-rw-r--r--  2.0 unx     5172 b- defN 23-Jul-26 11:55 kube/config.py
 -rw-r--r--  2.0 unx     1197 b- defN 23-Jul-23 06:20 kube/enums.py
 -rw-r--r--  2.0 unx    19115 b- defN 23-Jul-23 10:00 kube/manifests.py
 -rw-r--r--  2.0 unx    10932 b- defN 23-Jul-23 10:00 kube/templates.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-23 11:53 kube_ops-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3425 b- defN 23-Jul-23 11:53 kube_ops-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-23 11:53 kube_ops-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-23 11:53 kube_ops-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      894 b- defN 23-Jul-23 11:53 kube_ops-1.0.2.dist-info/RECORD
-12 files, 78268 bytes uncompressed, 17498 bytes compressed:  77.6%
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-27 01:27 kube_ops-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3425 b- defN 23-Jul-27 01:27 kube_ops-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 01:27 kube_ops-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-27 01:27 kube_ops-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      894 b- defN 23-Jul-27 01:27 kube_ops-1.0.3.dist-info/RECORD
+12 files, 78360 bytes uncompressed, 17526 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kube/manifests.py
 Comment: 
 
 Filename: kube/templates.py
 Comment: 
 
-Filename: kube_ops-1.0.2.dist-info/LICENSE
+Filename: kube_ops-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: kube_ops-1.0.2.dist-info/METADATA
+Filename: kube_ops-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: kube_ops-1.0.2.dist-info/WHEEL
+Filename: kube_ops-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: kube_ops-1.0.2.dist-info/top_level.txt
+Filename: kube_ops-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: kube_ops-1.0.2.dist-info/RECORD
+Filename: kube_ops-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kube/config.py

```diff
@@ -6,16 +6,15 @@
 import warnings
 from pathlib import Path
 from urllib.parse import urlparse
 
 import yaml
 from kubernetes import client
 from kubernetes.config.incluster_config import SERVICE_HOST_ENV_NAME, SERVICE_PORT_ENV_NAME, SERVICE_CERT_FILENAME
-from urllib3.exceptions import InsecureRequestWarning
-from urllib3.exceptions import MaxRetryError
+from urllib3.exceptions import InsecureRequestWarning, MaxRetryError
 
 from .api import KubeApi
 
 
 class Kubeconfig:
     def __init__(self):
         self.__current_context = None
@@ -63,35 +62,38 @@
         """
 
         if not server.startswith('https'):
             raise ValueError('Invalid server URL. URL must be start with https://...')
 
         parsed_url = urlparse(server)
         if not parsed_url.port:
-            server = f'{server}:443'
+            server = f'http://{parsed_url.netloc}:443'
             parsed_url = urlparse(server)
 
         namespace = kwargs.get('namespace', 'default')
 
+        ca_cert = None
         try:
-            KubeApi.from_token(server, token, namespace).configmap_get('kube-root-ca.crt')
+            cm = KubeApi.from_token(server, token, namespace).configmap_get('kube-root-ca.crt')
+            if cm:
+                ca_cert = cm.data.get('ca.crt')
         except MaxRetryError as e:
             raise ValueError(e.reason)
         except client.exceptions.ApiException as e:
             if e.status == 401:
                 raise ValueError("The token provided is invalid or expired")
 
             raise
 
         tok = base64.b64encode(hashlib.sha256(token.encode()).digest()).decode()[:12]
 
         cluster_name = kwargs.get('cluster_name', f'{parsed_url.netloc.replace(".", "-")}')
         ctx_name = kwargs.get('context_name', f'{namespace}/{cluster_name}/token-{tok}')
         user = kwargs.get('user', f'token-{tok}/{cluster_name}')
-        ca_cert = kwargs.get('ca_cert')
+        ca_cert = kwargs.get('ca_cert', ca_cert)
         insecure_skip_tls_verify = kwargs.get('skip_tls_verify', False)
 
         if not insecure_skip_tls_verify and not ca_cert:
             raise ValueError('Add CA data or set `skip_tls_verify=True`')
 
         cluster = {"server": server}
         if insecure_skip_tls_verify:
```

## Comparing `kube_ops-1.0.2.dist-info/LICENSE` & `kube_ops-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kube_ops-1.0.2.dist-info/METADATA` & `kube_ops-1.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kube-ops
-Version: 1.0.2
+Version: 1.0.3
 Summary: Kubernetes OOP
 Author-email: myback <54638513+myback@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 myback.space
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `kube_ops-1.0.2.dist-info/RECORD` & `kube_ops-1.0.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 kube/__init__.py,sha256=C7bskcMvkVYH2EoqnLUWBnv3GvTab-fEP_aFolr3uNY,1310
 kube/api.py,sha256=EBURovq7vq7BAbQBVu2Ux5GlXQc6cWqCt912Ty8Ri1g,32538
 kube/common.py,sha256=XRpVZJz700HSeErD7gFc1dWzT5GQlrhB1jEuxQ48N0Q,2611
-kube/config.py,sha256=iVa7oi0Rn3HerTlfq0OLbd_GJYhzzubkbki9AL1Q8_U,5080
+kube/config.py,sha256=EBLeUmNqxl2CKBQOLOffc_yLCeAMFpoMlCEz-Tp4ZDQ,5172
 kube/enums.py,sha256=egCkn8c3AJKzuYjKkbiX5re4J1z1rIiJc6WQcVvL9ug,1197
 kube/manifests.py,sha256=Xuftc2TeJ-F0HBSg8bQSr8RaKMntHC2Hv_rKTS6KMZI,19115
 kube/templates.py,sha256=9KcL3RUK9bexg6USf3Jp752bDND0pqzsZQSpd7A8ZtA,10932
-kube_ops-1.0.2.dist-info/LICENSE,sha256=4UMudA3MzI411FVQKHbbLdnwm2GjFrbv5LBNk5ZTT8Y,1069
-kube_ops-1.0.2.dist-info/METADATA,sha256=aTYSBVCPtEPCfjphUhYQUuL1kTg7M3rZ0gWwDWjeAMY,3425
-kube_ops-1.0.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-kube_ops-1.0.2.dist-info/top_level.txt,sha256=VviGlBjAU4SlS_NC5yQCpy0uOZb8yzwuA9KQU4Tvrgc,5
-kube_ops-1.0.2.dist-info/RECORD,,
+kube_ops-1.0.3.dist-info/LICENSE,sha256=4UMudA3MzI411FVQKHbbLdnwm2GjFrbv5LBNk5ZTT8Y,1069
+kube_ops-1.0.3.dist-info/METADATA,sha256=uNETM17433u6C40W3X-J7B7-R0kYH0uGXmHLK9oP03Y,3425
+kube_ops-1.0.3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+kube_ops-1.0.3.dist-info/top_level.txt,sha256=VviGlBjAU4SlS_NC5yQCpy0uOZb8yzwuA9KQU4Tvrgc,5
+kube_ops-1.0.3.dist-info/RECORD,,
```

