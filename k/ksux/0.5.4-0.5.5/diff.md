# Comparing `tmp/ksux-0.5.4.tar.gz` & `tmp/ksux-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksux-0.5.4.tar", last modified: Tue Apr 11 07:23:59 2023, max compression
+gzip compressed data, was "ksux-0.5.5.tar", last modified: Thu Jul 27 12:45:58 2023, max compression
```

## Comparing `ksux-0.5.4.tar` & `ksux-0.5.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:23:59.338125 ksux-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-11 07:23:39.000000 ksux-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 07:23:39.000000 ksux-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-04-11 07:23:59.338125 ksux-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-11 07:23:39.000000 ksux-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-11 07:23:50.000000 ksux-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 07:23:59.338125 ksux-0.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:23:59.334125 ksux-0.5.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:23:39.000000 ksux-0.5.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:23:59.338125 ksux-0.5.4/src/ksux/
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-11 07:23:50.000000 ksux-0.5.4/src/ksux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 07:23:39.000000 ksux-0.5.4/src/ksux/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:23:59.338125 ksux-0.5.4/src/ksux/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-11 07:23:39.000000 ksux-0.5.4/src/ksux/src/create_manifests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-11 07:23:39.000000 ksux-0.5.4/src/ksux/src/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-11 07:23:39.000000 ksux-0.5.4/src/ksux/src/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-11 07:23:39.000000 ksux-0.5.4/src/ksux/src/save_manifests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-11 07:23:39.000000 ksux-0.5.4/src/ksux/src/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:23:59.338125 ksux-0.5.4/src/ksux/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:23:39.000000 ksux-0.5.4/src/ksux/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 07:23:39.000000 ksux-0.5.4/src/ksux/tests/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-11 07:23:39.000000 ksux-0.5.4/src/ksux/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-11 07:23:39.000000 ksux-0.5.4/src/ksux/tests/test_read_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:23:59.338125 ksux-0.5.4/src/ksux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-04-11 07:23:59.000000 ksux-0.5.4/src/ksux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-11 07:23:59.000000 ksux-0.5.4/src/ksux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:23:59.000000 ksux-0.5.4/src/ksux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 07:23:59.000000 ksux-0.5.4/src/ksux.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 07:23:59.000000 ksux-0.5.4/src/ksux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 07:23:59.000000 ksux-0.5.4/src/ksux.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:58.040868 ksux-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 12:45:46.000000 ksux-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 12:45:46.000000 ksux-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-27 12:45:58.040868 ksux-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-27 12:45:46.000000 ksux-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-27 12:45:51.000000 ksux-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:45:58.040868 ksux-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:58.036868 ksux-0.5.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:46.000000 ksux-0.5.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:58.036868 ksux-0.5.5/src/ksux/
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-27 12:45:51.000000 ksux-0.5.5/src/ksux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:58.036868 ksux-0.5.5/src/ksux/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/src/create_manifests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/src/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/src/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/src/save_manifests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/src/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:58.036868 ksux-0.5.5/src/ksux/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/tests/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 12:45:46.000000 ksux-0.5.5/src/ksux/tests/test_read_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:45:58.036868 ksux-0.5.5/src/ksux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-27 12:45:58.000000 ksux-0.5.5/src/ksux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-27 12:45:58.000000 ksux-0.5.5/src/ksux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:45:58.000000 ksux-0.5.5/src/ksux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 12:45:58.000000 ksux-0.5.5/src/ksux.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 12:45:58.000000 ksux-0.5.5/src/ksux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 12:45:58.000000 ksux-0.5.5/src/ksux.egg-info/top_level.txt
```

### Comparing `ksux-0.5.4/LICENSE` & `ksux-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ksux-0.5.4/PKG-INFO` & `ksux-0.5.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,7 @@
-Metadata-Version: 2.1
-Name: ksux
-Version: 0.5.4
-Summary: Easy customization of kubernetes manifests
-Author: Tomas Sladecek
-License: MIT License
-        
-        Copyright (c) 2022 Tomáš Sládeček
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/tsladecek/ksux
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <img src="misc/logo.svg" width="75%">
 </p>
 
 <p align=center>
    <em>A simple way for templating kubernetes manifests.</em>
 </p>
@@ -43,14 +9,15 @@
 <p align=center>
    <img src='https://img.shields.io/github/actions/workflow/status/tsladecek/ksux/test.yml?branch=main&label=tests&logo=GitHub' alt=''/>
    <img src='https://img.shields.io/github/repo-size/tsladecek/ksux' alt=''/>
    <img src='https://img.shields.io/github/license/tsladecek/ksux' alt='License: MIT'/>
    <img src='https://img.shields.io/github/v/tag/tsladecek/ksux?color=yellow&label=version&logo=GitHub'/>
    <a href='https://pypi.org/project/ksux/'><img src='https://img.shields.io/pypi/v/ksux?logo=Pypi'/></a>
    <a href='https://hub.docker.com/r/tsladecek/ksux'><img src='https://img.shields.io/docker/image-size/tsladecek/ksux?logo=Docker&sort=date' /></a>
+   <a href='https://tsladecek.github.io/ksux/'><img src='https://img.shields.io/badge/Documentation-link-green' /></a>
 </p>
 
 ---
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
    1. [Local](#local)
@@ -139,14 +106,15 @@
   kind: <Deployment type of targeted resource>
   name: <name of targeted resource>
 ops:
   - name: <operation description>
     path: <path to the part of the manifest to be patched>
     value: <value which should be replaced or added>
     action: <add|replace|remove>
+    list_key: <Optional - key by which an element in list should be targeted. Defaults to "name">
 ```
 
 each patch file can be a list of patches. You can use the classic yaml format, e.g.:
 
 ```yaml
 - name: deployment_patches
   target:
@@ -218,14 +186,17 @@
 ```shell
 ksux -b <path_to_base_dir> -p <path_to_patches_dir> -o <output_dir>
 ```
 
 This will save all patched manifests to the output dir. You can use the `--dry-run` flag to print the patched
 manifests to stdout:
 
+**note**: By default, ksux will output patched manifests in `json` format. If you wish to output them in `yaml`, provide
+the `-e yaml` flag to the command below
+
 ```shell
 ksux -b <path_to_base_dir> -p <path_to_patches_dir> --dry-run
 ```
 
 For list of all options see:
 
 ```shell
@@ -256,15 +227,76 @@
       targetPort: 443
   selector:
     app: web
   type: ClusterIP
 ```
 
 To target the `https` service and change its name, you can specify the path: `/spec/ports/https/name` and then
-set the value to the new name 💪.
+set the value to the new name:
+
+```yaml
+name: service_patches
+target:
+  apiVersion: v1
+  kind: Service
+  name: nginx-service
+ops:
+- name: rename_https_port
+  path: /spec/ports/https/name
+  action: replace
+  value: new_name
+```
+
+---
+
+You can extend this even further. If you provide the `list_key` prop to a patch, you can target any list item with any
+key you wish to use. For example, lets say you have an ingress:
+
+```yaml
+apiVersion: networking.k8s.io/v1
+kind: Ingress
+metadata:
+  name: ingress
+  namespace: default
+  annotations:
+    nginx.ingress.kubernetes.io/rewrite-target: /
+spec:
+  ingressClassName: nginx
+  rules:
+    - host: "domain.com"
+      http:
+        paths:
+        - path: /api
+          pathType: Prefix
+          backend:
+            service:
+              name: backend
+              port:
+                number: 80
+```
+
+and you wish to use a different host in each of your environments. E.g. in `dev` environment, you would like the host to be `dev.domain.com`, in `staging` environment `staging.domain.com`, etc.
+
+You can easily write a patch for each such environment:
+
+```yaml
+name: ingress dev patches
+target:
+  apiVersion: networking.k8s.io/v1
+  kind: Ingress
+  name: ingress
+ops:
+  - name: replace host
+    path: /spec/rules/domain.com/host
+    action: replace
+    value: "dev.domain.com"
+    list_key: "host"
+```
+
+Ez 🙃
 
 ## Example
 
 In the `./examples` folder there are 3 sub-folders:
     - `/examples/base` with deployment, service and a configmap manifests. These are the base manifests which we wish
     to patch
     - `/examples/patches` contain the patches (notice that both base kubernetes manifests and patches can be either in
```

#### html2text {}

```diff
@@ -1,32 +1,14 @@
-Metadata-Version: 2.1 Name: ksux Version: 0.5.4 Summary: Easy customization of
-kubernetes manifests Author: Tomas Sladecek License: MIT License Copyright (c)
-2022 TomÃ¡Å¡ SlÃ¡deÄek Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated documentation files
-(the "Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish, distribute,
-sublicense, and/or sell copies of the Software, and to permit persons to whom
-the Software is furnished to do so, subject to the following conditions: The
-above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
-IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
-LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
-AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
-SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage,
-https://github.com/tsladecek/ksux Classifier: Programming Language :: Python ::
-3 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE
                                 [misc/logo.svg]
                A simple way for templating kubernetes manifests.
          [License: MIT] [https://img.shields.io/github/v/tag/tsladecek/
  ksux?color=yellow&label=version&logo=GitHub] [https://img.shields.io/pypi/v/
      ksux?logo=Pypi] [https://img.shields.io/docker/image-size/tsladecek/
-                          ksux?logo=Docker&sort=date]
+ ksux?logo=Docker&sort=date] [https://img.shields.io/badge/Documentation-link-
+                                    green]
 --- 1. [Requirements](#requirements) 2. [Installation](#installation) 1.
 [Local](#local) 2. [Docker](#docker) 3. [How does it work?](#how-does-it-work)
 1. [The `op.path`](#the-oppath) 4. [Example](#example) **tldr.** ```shell ksux
 -b  -p  -o  ``` or using docker: ```shell docker run --rm -v /path/to/your/
 configs:/configs tsladecek/ksux ksux -b /configs/base -p /configs/patches -o /
 configs/out ``` --- ## Requirements This is a python package. So the only
 requirements are `python3` and `pip` ## Installation ### Local - Optional:
@@ -43,47 +25,66 @@
 configs/out ``` the important part is the `-v` flag, which will mount your
 local folder as volume to the container. ## How does it work? Let's say that
 you have many manifests in some directory (`base` directory) that you wish to
 patch with patches (in the `patches`) directory. Patches could be in `yaml` or
 `json` format (as well as your manifests). However, they must adhere to
 following schema: ```yaml name:  target: apiVersion:  kind:  name:  ops: -
 name:  path:  value:  action:
-replace|remove> ``` each patch file can be a list of patches. You can use the
-classic yaml format, e.g.: ```yaml - name: deployment_patches target:
-apiVersion: apps/v1 kind: Deployment name: web ops: - name: replace_image path:
-/spec/template/spec/containers/nginx/image value: nginx:1.23 action: replace -
-name: service_patches target: apiVersion: v1 kind: Service name: nginx-service
-ops: - name: add_https_port path: /spec/ports value: name: https port: 443
-protocol: TCP targetPort: 443 action: add - name: rename_http_port path: /spec/
-ports/http/name action: replace value: new_name ``` or use the `---` separator:
+replace|remove> list_key:
+ key by which an element in list should be targeted. Defaults to "name"> ```
+each patch file can be a list of patches. You can use the classic yaml format,
+e.g.: ```yaml - name: deployment_patches target: apiVersion: apps/v1 kind:
+Deployment name: web ops: - name: replace_image path: /spec/template/spec/
+containers/nginx/image value: nginx:1.23 action: replace - name:
+service_patches target: apiVersion: v1 kind: Service name: nginx-service ops: -
+name: add_https_port path: /spec/ports value: name: https port: 443 protocol:
+TCP targetPort: 443 action: add - name: rename_http_port path: /spec/ports/
+http/name action: replace value: new_name ``` or use the `---` separator:
 ```yaml --- name: deployment_patches target: apiVersion: apps/v1 kind:
 Deployment name: web ops: - name: replace_image path: /spec/template/spec/
 containers/nginx/image value: nginx:1.23 action: replace --- name:
 service_patches target: apiVersion: v1 kind: Service name: nginx-service ops: -
 name: add_https_port path: /spec/ports value: name: https port: 443 protocol:
 TCP targetPort: 443 action: add - name: rename_http_port path: /spec/ports/
 http/name action: replace value: new_name ``` Then all you need to do, is run:
 ```shell ksux -b  -p  -o  ``` This will save all patched manifests to the
 output dir. You can use the `--dry-run` flag to print the patched manifests to
-stdout: ```shell ksux -b  -p  --dry-run ``` For list of all options see:
+stdout: **note**: By default, ksux will output patched manifests in `json`
+format. If you wish to output them in `yaml`, provide the `-e yaml` flag to the
+command below ```shell ksux -b  -p  --dry-run ``` For list of all options see:
 ```shell ksux --help ``` ### the `op.path` This is a pretty cool thing. Similar
 to kustomize path, however you can target list item by names of child objects.
 E.g. say you have a list of ports in a service: ```yaml apiVersion: v1 kind:
 Service metadata: labels: app: nginx-service name: nginx-service spec: ports: -
 name: new_name port: 80 protocol: TCP targetPort: 80 - name: https port: 443
 protocol: TCP targetPort: 443 selector: app: web type: ClusterIP ``` To target
 the `https` service and change its name, you can specify the path: `/spec/
-ports/https/name` and then set the value to the new name ðª. ## Example In
-the `./examples` folder there are 3 sub-folders: - `/examples/base` with
-deployment, service and a configmap manifests. These are the base manifests
-which we wish to patch - `/examples/patches` contain the patches (notice that
-both base kubernetes manifests and patches can be either in `json` or `yml`/
-`yaml` format) - `/examples/out` is the output directory where the patched
-resources will be output First, we will `dry-run` the patching: ```shell ksux -
-b examples/base -p examples/patches --dry-run ``` You should see the patched
-manifests printed out to the console. Now we can run it and save the patched
-manifests to the `output` folder: ```shell ksux -b examples/base -p examples/
-patches -o examples/out ``` By default, the manifests will be saved in `yaml`
-format with `.yaml` extension. If you wish to use the `.yml` extension or save
-the manifests in `json` format, simply provide the `-e` flag with corresponding
-extension. E.g.: ```shell ksux -b examples/base -p examples/patches -
-o examples/out -e json ```
+ports/https/name` and then set the value to the new name: ```yaml name:
+service_patches target: apiVersion: v1 kind: Service name: nginx-service ops: -
+name: rename_https_port path: /spec/ports/https/name action: replace value:
+new_name ``` --- You can extend this even further. If you provide the
+`list_key` prop to a patch, you can target any list item with any key you wish
+to use. For example, lets say you have an ingress: ```yaml apiVersion:
+networking.k8s.io/v1 kind: Ingress metadata: name: ingress namespace: default
+annotations: nginx.ingress.kubernetes.io/rewrite-target: / spec:
+ingressClassName: nginx rules: - host: "domain.com" http: paths: - path: /api
+pathType: Prefix backend: service: name: backend port: number: 80 ``` and you
+wish to use a different host in each of your environments. E.g. in `dev`
+environment, you would like the host to be `dev.domain.com`, in `staging`
+environment `staging.domain.com`, etc. You can easily write a patch for each
+such environment: ```yaml name: ingress dev patches target: apiVersion:
+networking.k8s.io/v1 kind: Ingress name: ingress ops: - name: replace host
+path: /spec/rules/domain.com/host action: replace value: "dev.domain.com"
+list_key: "host" ``` Ez ð ## Example In the `./examples` folder there are 3
+sub-folders: - `/examples/base` with deployment, service and a configmap
+manifests. These are the base manifests which we wish to patch - `/examples/
+patches` contain the patches (notice that both base kubernetes manifests and
+patches can be either in `json` or `yml`/`yaml` format) - `/examples/out` is
+the output directory where the patched resources will be output First, we will
+`dry-run` the patching: ```shell ksux -b examples/base -p examples/patches --
+dry-run ``` You should see the patched manifests printed out to the console.
+Now we can run it and save the patched manifests to the `output` folder:
+```shell ksux -b examples/base -p examples/patches -o examples/out ``` By
+default, the manifests will be saved in `yaml` format with `.yaml` extension.
+If you wish to use the `.yml` extension or save the manifests in `json` format,
+simply provide the `-e` flag with corresponding extension. E.g.: ```shell ksux
+-b examples/base -p examples/patches -o examples/out -e json ```
```

### Comparing `ksux-0.5.4/README.md` & `ksux-0.5.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1
+Name: ksux
+Version: 0.5.5
+Summary: Easy customization of kubernetes manifests
+Author: Tomas Sladecek
+License: MIT License
+        
+        Copyright (c) 2022 Tomáš Sládeček
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/tsladecek/ksux
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <img src="misc/logo.svg" width="75%">
 </p>
 
 <p align=center>
    <em>A simple way for templating kubernetes manifests.</em>
 </p>
@@ -9,14 +43,15 @@
 <p align=center>
    <img src='https://img.shields.io/github/actions/workflow/status/tsladecek/ksux/test.yml?branch=main&label=tests&logo=GitHub' alt=''/>
    <img src='https://img.shields.io/github/repo-size/tsladecek/ksux' alt=''/>
    <img src='https://img.shields.io/github/license/tsladecek/ksux' alt='License: MIT'/>
    <img src='https://img.shields.io/github/v/tag/tsladecek/ksux?color=yellow&label=version&logo=GitHub'/>
    <a href='https://pypi.org/project/ksux/'><img src='https://img.shields.io/pypi/v/ksux?logo=Pypi'/></a>
    <a href='https://hub.docker.com/r/tsladecek/ksux'><img src='https://img.shields.io/docker/image-size/tsladecek/ksux?logo=Docker&sort=date' /></a>
+   <a href='https://tsladecek.github.io/ksux/'><img src='https://img.shields.io/badge/Documentation-link-green' /></a>
 </p>
 
 ---
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
    1. [Local](#local)
@@ -105,14 +140,15 @@
   kind: <Deployment type of targeted resource>
   name: <name of targeted resource>
 ops:
   - name: <operation description>
     path: <path to the part of the manifest to be patched>
     value: <value which should be replaced or added>
     action: <add|replace|remove>
+    list_key: <Optional - key by which an element in list should be targeted. Defaults to "name">
 ```
 
 each patch file can be a list of patches. You can use the classic yaml format, e.g.:
 
 ```yaml
 - name: deployment_patches
   target:
@@ -184,14 +220,17 @@
 ```shell
 ksux -b <path_to_base_dir> -p <path_to_patches_dir> -o <output_dir>
 ```
 
 This will save all patched manifests to the output dir. You can use the `--dry-run` flag to print the patched
 manifests to stdout:
 
+**note**: By default, ksux will output patched manifests in `json` format. If you wish to output them in `yaml`, provide
+the `-e yaml` flag to the command below
+
 ```shell
 ksux -b <path_to_base_dir> -p <path_to_patches_dir> --dry-run
 ```
 
 For list of all options see:
 
 ```shell
@@ -222,15 +261,76 @@
       targetPort: 443
   selector:
     app: web
   type: ClusterIP
 ```
 
 To target the `https` service and change its name, you can specify the path: `/spec/ports/https/name` and then
-set the value to the new name 💪.
+set the value to the new name:
+
+```yaml
+name: service_patches
+target:
+  apiVersion: v1
+  kind: Service
+  name: nginx-service
+ops:
+- name: rename_https_port
+  path: /spec/ports/https/name
+  action: replace
+  value: new_name
+```
+
+---
+
+You can extend this even further. If you provide the `list_key` prop to a patch, you can target any list item with any
+key you wish to use. For example, lets say you have an ingress:
+
+```yaml
+apiVersion: networking.k8s.io/v1
+kind: Ingress
+metadata:
+  name: ingress
+  namespace: default
+  annotations:
+    nginx.ingress.kubernetes.io/rewrite-target: /
+spec:
+  ingressClassName: nginx
+  rules:
+    - host: "domain.com"
+      http:
+        paths:
+        - path: /api
+          pathType: Prefix
+          backend:
+            service:
+              name: backend
+              port:
+                number: 80
+```
+
+and you wish to use a different host in each of your environments. E.g. in `dev` environment, you would like the host to be `dev.domain.com`, in `staging` environment `staging.domain.com`, etc.
+
+You can easily write a patch for each such environment:
+
+```yaml
+name: ingress dev patches
+target:
+  apiVersion: networking.k8s.io/v1
+  kind: Ingress
+  name: ingress
+ops:
+  - name: replace host
+    path: /spec/rules/domain.com/host
+    action: replace
+    value: "dev.domain.com"
+    list_key: "host"
+```
+
+Ez 🙃
 
 ## Example
 
 In the `./examples` folder there are 3 sub-folders:
     - `/examples/base` with deployment, service and a configmap manifests. These are the base manifests which we wish
     to patch
     - `/examples/patches` contain the patches (notice that both base kubernetes manifests and patches can be either in
```

#### html2text {}

```diff
@@ -1,13 +1,33 @@
+Metadata-Version: 2.1 Name: ksux Version: 0.5.5 Summary: Easy customization of
+kubernetes manifests Author: Tomas Sladecek License: MIT License Copyright (c)
+2022 TomÃ¡Å¡ SlÃ¡deÄek Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated documentation files
+(the "Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish, distribute,
+sublicense, and/or sell copies of the Software, and to permit persons to whom
+the Software is furnished to do so, subject to the following conditions: The
+above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
+IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
+LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
+AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: Homepage,
+https://github.com/tsladecek/ksux Classifier: Programming Language :: Python ::
+3 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE
                                 [misc/logo.svg]
                A simple way for templating kubernetes manifests.
          [License: MIT] [https://img.shields.io/github/v/tag/tsladecek/
  ksux?color=yellow&label=version&logo=GitHub] [https://img.shields.io/pypi/v/
      ksux?logo=Pypi] [https://img.shields.io/docker/image-size/tsladecek/
-                          ksux?logo=Docker&sort=date]
+ ksux?logo=Docker&sort=date] [https://img.shields.io/badge/Documentation-link-
+                                    green]
 --- 1. [Requirements](#requirements) 2. [Installation](#installation) 1.
 [Local](#local) 2. [Docker](#docker) 3. [How does it work?](#how-does-it-work)
 1. [The `op.path`](#the-oppath) 4. [Example](#example) **tldr.** ```shell ksux
 -b  -p  -o  ``` or using docker: ```shell docker run --rm -v /path/to/your/
 configs:/configs tsladecek/ksux ksux -b /configs/base -p /configs/patches -o /
 configs/out ``` --- ## Requirements This is a python package. So the only
 requirements are `python3` and `pip` ## Installation ### Local - Optional:
@@ -24,47 +44,66 @@
 configs/out ``` the important part is the `-v` flag, which will mount your
 local folder as volume to the container. ## How does it work? Let's say that
 you have many manifests in some directory (`base` directory) that you wish to
 patch with patches (in the `patches`) directory. Patches could be in `yaml` or
 `json` format (as well as your manifests). However, they must adhere to
 following schema: ```yaml name:  target: apiVersion:  kind:  name:  ops: -
 name:  path:  value:  action:
-replace|remove> ``` each patch file can be a list of patches. You can use the
-classic yaml format, e.g.: ```yaml - name: deployment_patches target:
-apiVersion: apps/v1 kind: Deployment name: web ops: - name: replace_image path:
-/spec/template/spec/containers/nginx/image value: nginx:1.23 action: replace -
-name: service_patches target: apiVersion: v1 kind: Service name: nginx-service
-ops: - name: add_https_port path: /spec/ports value: name: https port: 443
-protocol: TCP targetPort: 443 action: add - name: rename_http_port path: /spec/
-ports/http/name action: replace value: new_name ``` or use the `---` separator:
+replace|remove> list_key:
+ key by which an element in list should be targeted. Defaults to "name"> ```
+each patch file can be a list of patches. You can use the classic yaml format,
+e.g.: ```yaml - name: deployment_patches target: apiVersion: apps/v1 kind:
+Deployment name: web ops: - name: replace_image path: /spec/template/spec/
+containers/nginx/image value: nginx:1.23 action: replace - name:
+service_patches target: apiVersion: v1 kind: Service name: nginx-service ops: -
+name: add_https_port path: /spec/ports value: name: https port: 443 protocol:
+TCP targetPort: 443 action: add - name: rename_http_port path: /spec/ports/
+http/name action: replace value: new_name ``` or use the `---` separator:
 ```yaml --- name: deployment_patches target: apiVersion: apps/v1 kind:
 Deployment name: web ops: - name: replace_image path: /spec/template/spec/
 containers/nginx/image value: nginx:1.23 action: replace --- name:
 service_patches target: apiVersion: v1 kind: Service name: nginx-service ops: -
 name: add_https_port path: /spec/ports value: name: https port: 443 protocol:
 TCP targetPort: 443 action: add - name: rename_http_port path: /spec/ports/
 http/name action: replace value: new_name ``` Then all you need to do, is run:
 ```shell ksux -b  -p  -o  ``` This will save all patched manifests to the
 output dir. You can use the `--dry-run` flag to print the patched manifests to
-stdout: ```shell ksux -b  -p  --dry-run ``` For list of all options see:
+stdout: **note**: By default, ksux will output patched manifests in `json`
+format. If you wish to output them in `yaml`, provide the `-e yaml` flag to the
+command below ```shell ksux -b  -p  --dry-run ``` For list of all options see:
 ```shell ksux --help ``` ### the `op.path` This is a pretty cool thing. Similar
 to kustomize path, however you can target list item by names of child objects.
 E.g. say you have a list of ports in a service: ```yaml apiVersion: v1 kind:
 Service metadata: labels: app: nginx-service name: nginx-service spec: ports: -
 name: new_name port: 80 protocol: TCP targetPort: 80 - name: https port: 443
 protocol: TCP targetPort: 443 selector: app: web type: ClusterIP ``` To target
 the `https` service and change its name, you can specify the path: `/spec/
-ports/https/name` and then set the value to the new name ðª. ## Example In
-the `./examples` folder there are 3 sub-folders: - `/examples/base` with
-deployment, service and a configmap manifests. These are the base manifests
-which we wish to patch - `/examples/patches` contain the patches (notice that
-both base kubernetes manifests and patches can be either in `json` or `yml`/
-`yaml` format) - `/examples/out` is the output directory where the patched
-resources will be output First, we will `dry-run` the patching: ```shell ksux -
-b examples/base -p examples/patches --dry-run ``` You should see the patched
-manifests printed out to the console. Now we can run it and save the patched
-manifests to the `output` folder: ```shell ksux -b examples/base -p examples/
-patches -o examples/out ``` By default, the manifests will be saved in `yaml`
-format with `.yaml` extension. If you wish to use the `.yml` extension or save
-the manifests in `json` format, simply provide the `-e` flag with corresponding
-extension. E.g.: ```shell ksux -b examples/base -p examples/patches -
-o examples/out -e json ```
+ports/https/name` and then set the value to the new name: ```yaml name:
+service_patches target: apiVersion: v1 kind: Service name: nginx-service ops: -
+name: rename_https_port path: /spec/ports/https/name action: replace value:
+new_name ``` --- You can extend this even further. If you provide the
+`list_key` prop to a patch, you can target any list item with any key you wish
+to use. For example, lets say you have an ingress: ```yaml apiVersion:
+networking.k8s.io/v1 kind: Ingress metadata: name: ingress namespace: default
+annotations: nginx.ingress.kubernetes.io/rewrite-target: / spec:
+ingressClassName: nginx rules: - host: "domain.com" http: paths: - path: /api
+pathType: Prefix backend: service: name: backend port: number: 80 ``` and you
+wish to use a different host in each of your environments. E.g. in `dev`
+environment, you would like the host to be `dev.domain.com`, in `staging`
+environment `staging.domain.com`, etc. You can easily write a patch for each
+such environment: ```yaml name: ingress dev patches target: apiVersion:
+networking.k8s.io/v1 kind: Ingress name: ingress ops: - name: replace host
+path: /spec/rules/domain.com/host action: replace value: "dev.domain.com"
+list_key: "host" ``` Ez ð ## Example In the `./examples` folder there are 3
+sub-folders: - `/examples/base` with deployment, service and a configmap
+manifests. These are the base manifests which we wish to patch - `/examples/
+patches` contain the patches (notice that both base kubernetes manifests and
+patches can be either in `json` or `yml`/`yaml` format) - `/examples/out` is
+the output directory where the patched resources will be output First, we will
+`dry-run` the patching: ```shell ksux -b examples/base -p examples/patches --
+dry-run ``` You should see the patched manifests printed out to the console.
+Now we can run it and save the patched manifests to the `output` folder:
+```shell ksux -b examples/base -p examples/patches -o examples/out ``` By
+default, the manifests will be saved in `yaml` format with `.yaml` extension.
+If you wish to use the `.yml` extension or save the manifests in `json` format,
+simply provide the `-e` flag with corresponding extension. E.g.: ```shell ksux
+-b examples/base -p examples/patches -o examples/out -e json ```
```

### Comparing `ksux-0.5.4/pyproject.toml` & `ksux-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ksux"
-version = "0.5.4"
+version = "0.5.5"
 authors = [
     { name = "Tomas Sladecek" }
 ]
 description = "Easy customization of kubernetes manifests"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `ksux-0.5.4/src/ksux/__init__.py` & `ksux-0.5.5/src/ksux/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,30 +21,45 @@
     parser.add_argument('--patched_only', help='If all manifests should be saved, even those which were not patched',
                         action='store_true')
     parser.add_argument('-x', '--exclude', help='Exclude one or more manifests. To target the manifest, argument '
                                                 'expects format: {apiVersion}_{kind}_{name}. E.g. if you wished to '
                                                 'exclude deployment with name "backend", the option would look like: '
                                                 'ksux -b ... -p ... -o ... -x apps/v1_Deployment_backend',
                         action='append')
+    parser.add_argument('-xf', '--exclude-file', help='File with a list of resources to be excluded. Resources'
+                                                      'must follow the format: {apiVersion}_{kind}_{name}')
     parser.add_argument('--dry-run', help='Print manifests to stdout', action="store_true")
     parser.add_argument('-q', '--quiet', help='Do not print debug, info and warning messages', action='store_true')
     parser.add_argument('--version', help='Package version', action="store_true")
 
     args = parser.parse_args()
 
     if args.version:
-        print('0.5.4')
+        print('0.5.5')
         exit(0)
 
     if args.quiet:
         logging.root.setLevel(logging.ERROR)
     else:
         logging.root.setLevel(logging.INFO)
 
     exclude = [] if not args.exclude else args.exclude
+
+    if args.exclude_file:
+        try:
+            with open(args.exclude_file) as f:
+                for line in f.readlines():
+                    res = line.strip()
+
+                    # ignore comments (lines starting with "#") and empty lines
+                    if res and not res.startswith('#'):
+                        exclude.append(res)
+        except FileNotFoundError:
+            logging.error(f'File {args.exclude_file} not found')
+
     # validate exclude
     for e in exclude:
         try:
             apiVersion, kind, name = e.split('_')
         except ValueError:
             logging.error('Exclude items have to be in format: {apiVersion}_{kind}_{name}')
             exit(1)
```

### Comparing `ksux-0.5.4/src/ksux/src/create_manifests.py` & `ksux-0.5.5/src/ksux/src/create_manifests.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.4/src/ksux/src/patch.py` & `ksux-0.5.5/src/ksux/src/patch.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.4/src/ksux/src/read_file.py` & `ksux-0.5.5/src/ksux/src/read_file.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.4/src/ksux/src/save_manifests.py` & `ksux-0.5.5/src/ksux/src/save_manifests.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.4/src/ksux/src/schemas.py` & `ksux-0.5.5/src/ksux/src/schemas.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.4/src/ksux/tests/test_patch.py` & `ksux-0.5.5/src/ksux/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.4/src/ksux/tests/test_read_file.py` & `ksux-0.5.5/src/ksux/tests/test_read_file.py`

 * *Files identical despite different names*

### Comparing `ksux-0.5.4/src/ksux.egg-info/PKG-INFO` & `ksux-0.5.5/src/ksux.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ksux
-Version: 0.5.4
+Version: 0.5.5
 Summary: Easy customization of kubernetes manifests
 Author: Tomas Sladecek
 License: MIT License
         
         Copyright (c) 2022 Tomáš Sládeček
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,15 @@
 <p align=center>
    <img src='https://img.shields.io/github/actions/workflow/status/tsladecek/ksux/test.yml?branch=main&label=tests&logo=GitHub' alt=''/>
    <img src='https://img.shields.io/github/repo-size/tsladecek/ksux' alt=''/>
    <img src='https://img.shields.io/github/license/tsladecek/ksux' alt='License: MIT'/>
    <img src='https://img.shields.io/github/v/tag/tsladecek/ksux?color=yellow&label=version&logo=GitHub'/>
    <a href='https://pypi.org/project/ksux/'><img src='https://img.shields.io/pypi/v/ksux?logo=Pypi'/></a>
    <a href='https://hub.docker.com/r/tsladecek/ksux'><img src='https://img.shields.io/docker/image-size/tsladecek/ksux?logo=Docker&sort=date' /></a>
+   <a href='https://tsladecek.github.io/ksux/'><img src='https://img.shields.io/badge/Documentation-link-green' /></a>
 </p>
 
 ---
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
    1. [Local](#local)
@@ -139,14 +140,15 @@
   kind: <Deployment type of targeted resource>
   name: <name of targeted resource>
 ops:
   - name: <operation description>
     path: <path to the part of the manifest to be patched>
     value: <value which should be replaced or added>
     action: <add|replace|remove>
+    list_key: <Optional - key by which an element in list should be targeted. Defaults to "name">
 ```
 
 each patch file can be a list of patches. You can use the classic yaml format, e.g.:
 
 ```yaml
 - name: deployment_patches
   target:
@@ -218,14 +220,17 @@
 ```shell
 ksux -b <path_to_base_dir> -p <path_to_patches_dir> -o <output_dir>
 ```
 
 This will save all patched manifests to the output dir. You can use the `--dry-run` flag to print the patched
 manifests to stdout:
 
+**note**: By default, ksux will output patched manifests in `json` format. If you wish to output them in `yaml`, provide
+the `-e yaml` flag to the command below
+
 ```shell
 ksux -b <path_to_base_dir> -p <path_to_patches_dir> --dry-run
 ```
 
 For list of all options see:
 
 ```shell
@@ -256,15 +261,76 @@
       targetPort: 443
   selector:
     app: web
   type: ClusterIP
 ```
 
 To target the `https` service and change its name, you can specify the path: `/spec/ports/https/name` and then
-set the value to the new name 💪.
+set the value to the new name:
+
+```yaml
+name: service_patches
+target:
+  apiVersion: v1
+  kind: Service
+  name: nginx-service
+ops:
+- name: rename_https_port
+  path: /spec/ports/https/name
+  action: replace
+  value: new_name
+```
+
+---
+
+You can extend this even further. If you provide the `list_key` prop to a patch, you can target any list item with any
+key you wish to use. For example, lets say you have an ingress:
+
+```yaml
+apiVersion: networking.k8s.io/v1
+kind: Ingress
+metadata:
+  name: ingress
+  namespace: default
+  annotations:
+    nginx.ingress.kubernetes.io/rewrite-target: /
+spec:
+  ingressClassName: nginx
+  rules:
+    - host: "domain.com"
+      http:
+        paths:
+        - path: /api
+          pathType: Prefix
+          backend:
+            service:
+              name: backend
+              port:
+                number: 80
+```
+
+and you wish to use a different host in each of your environments. E.g. in `dev` environment, you would like the host to be `dev.domain.com`, in `staging` environment `staging.domain.com`, etc.
+
+You can easily write a patch for each such environment:
+
+```yaml
+name: ingress dev patches
+target:
+  apiVersion: networking.k8s.io/v1
+  kind: Ingress
+  name: ingress
+ops:
+  - name: replace host
+    path: /spec/rules/domain.com/host
+    action: replace
+    value: "dev.domain.com"
+    list_key: "host"
+```
+
+Ez 🙃
 
 ## Example
 
 In the `./examples` folder there are 3 sub-folders:
     - `/examples/base` with deployment, service and a configmap manifests. These are the base manifests which we wish
     to patch
     - `/examples/patches` contain the patches (notice that both base kubernetes manifests and patches can be either in
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ksux Version: 0.5.4 Summary: Easy customization of
+Metadata-Version: 2.1 Name: ksux Version: 0.5.5 Summary: Easy customization of
 kubernetes manifests Author: Tomas Sladecek License: MIT License Copyright (c)
 2022 TomÃ¡Å¡ SlÃ¡deÄek Permission is hereby granted, free of charge, to any
 person obtaining a copy of this software and associated documentation files
 (the "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
@@ -18,15 +18,16 @@
 3 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE
                                 [misc/logo.svg]
                A simple way for templating kubernetes manifests.
          [License: MIT] [https://img.shields.io/github/v/tag/tsladecek/
  ksux?color=yellow&label=version&logo=GitHub] [https://img.shields.io/pypi/v/
      ksux?logo=Pypi] [https://img.shields.io/docker/image-size/tsladecek/
-                          ksux?logo=Docker&sort=date]
+ ksux?logo=Docker&sort=date] [https://img.shields.io/badge/Documentation-link-
+                                    green]
 --- 1. [Requirements](#requirements) 2. [Installation](#installation) 1.
 [Local](#local) 2. [Docker](#docker) 3. [How does it work?](#how-does-it-work)
 1. [The `op.path`](#the-oppath) 4. [Example](#example) **tldr.** ```shell ksux
 -b  -p  -o  ``` or using docker: ```shell docker run --rm -v /path/to/your/
 configs:/configs tsladecek/ksux ksux -b /configs/base -p /configs/patches -o /
 configs/out ``` --- ## Requirements This is a python package. So the only
 requirements are `python3` and `pip` ## Installation ### Local - Optional:
@@ -43,47 +44,66 @@
 configs/out ``` the important part is the `-v` flag, which will mount your
 local folder as volume to the container. ## How does it work? Let's say that
 you have many manifests in some directory (`base` directory) that you wish to
 patch with patches (in the `patches`) directory. Patches could be in `yaml` or
 `json` format (as well as your manifests). However, they must adhere to
 following schema: ```yaml name:  target: apiVersion:  kind:  name:  ops: -
 name:  path:  value:  action:
-replace|remove> ``` each patch file can be a list of patches. You can use the
-classic yaml format, e.g.: ```yaml - name: deployment_patches target:
-apiVersion: apps/v1 kind: Deployment name: web ops: - name: replace_image path:
-/spec/template/spec/containers/nginx/image value: nginx:1.23 action: replace -
-name: service_patches target: apiVersion: v1 kind: Service name: nginx-service
-ops: - name: add_https_port path: /spec/ports value: name: https port: 443
-protocol: TCP targetPort: 443 action: add - name: rename_http_port path: /spec/
-ports/http/name action: replace value: new_name ``` or use the `---` separator:
+replace|remove> list_key:
+ key by which an element in list should be targeted. Defaults to "name"> ```
+each patch file can be a list of patches. You can use the classic yaml format,
+e.g.: ```yaml - name: deployment_patches target: apiVersion: apps/v1 kind:
+Deployment name: web ops: - name: replace_image path: /spec/template/spec/
+containers/nginx/image value: nginx:1.23 action: replace - name:
+service_patches target: apiVersion: v1 kind: Service name: nginx-service ops: -
+name: add_https_port path: /spec/ports value: name: https port: 443 protocol:
+TCP targetPort: 443 action: add - name: rename_http_port path: /spec/ports/
+http/name action: replace value: new_name ``` or use the `---` separator:
 ```yaml --- name: deployment_patches target: apiVersion: apps/v1 kind:
 Deployment name: web ops: - name: replace_image path: /spec/template/spec/
 containers/nginx/image value: nginx:1.23 action: replace --- name:
 service_patches target: apiVersion: v1 kind: Service name: nginx-service ops: -
 name: add_https_port path: /spec/ports value: name: https port: 443 protocol:
 TCP targetPort: 443 action: add - name: rename_http_port path: /spec/ports/
 http/name action: replace value: new_name ``` Then all you need to do, is run:
 ```shell ksux -b  -p  -o  ``` This will save all patched manifests to the
 output dir. You can use the `--dry-run` flag to print the patched manifests to
-stdout: ```shell ksux -b  -p  --dry-run ``` For list of all options see:
+stdout: **note**: By default, ksux will output patched manifests in `json`
+format. If you wish to output them in `yaml`, provide the `-e yaml` flag to the
+command below ```shell ksux -b  -p  --dry-run ``` For list of all options see:
 ```shell ksux --help ``` ### the `op.path` This is a pretty cool thing. Similar
 to kustomize path, however you can target list item by names of child objects.
 E.g. say you have a list of ports in a service: ```yaml apiVersion: v1 kind:
 Service metadata: labels: app: nginx-service name: nginx-service spec: ports: -
 name: new_name port: 80 protocol: TCP targetPort: 80 - name: https port: 443
 protocol: TCP targetPort: 443 selector: app: web type: ClusterIP ``` To target
 the `https` service and change its name, you can specify the path: `/spec/
-ports/https/name` and then set the value to the new name ðª. ## Example In
-the `./examples` folder there are 3 sub-folders: - `/examples/base` with
-deployment, service and a configmap manifests. These are the base manifests
-which we wish to patch - `/examples/patches` contain the patches (notice that
-both base kubernetes manifests and patches can be either in `json` or `yml`/
-`yaml` format) - `/examples/out` is the output directory where the patched
-resources will be output First, we will `dry-run` the patching: ```shell ksux -
-b examples/base -p examples/patches --dry-run ``` You should see the patched
-manifests printed out to the console. Now we can run it and save the patched
-manifests to the `output` folder: ```shell ksux -b examples/base -p examples/
-patches -o examples/out ``` By default, the manifests will be saved in `yaml`
-format with `.yaml` extension. If you wish to use the `.yml` extension or save
-the manifests in `json` format, simply provide the `-e` flag with corresponding
-extension. E.g.: ```shell ksux -b examples/base -p examples/patches -
-o examples/out -e json ```
+ports/https/name` and then set the value to the new name: ```yaml name:
+service_patches target: apiVersion: v1 kind: Service name: nginx-service ops: -
+name: rename_https_port path: /spec/ports/https/name action: replace value:
+new_name ``` --- You can extend this even further. If you provide the
+`list_key` prop to a patch, you can target any list item with any key you wish
+to use. For example, lets say you have an ingress: ```yaml apiVersion:
+networking.k8s.io/v1 kind: Ingress metadata: name: ingress namespace: default
+annotations: nginx.ingress.kubernetes.io/rewrite-target: / spec:
+ingressClassName: nginx rules: - host: "domain.com" http: paths: - path: /api
+pathType: Prefix backend: service: name: backend port: number: 80 ``` and you
+wish to use a different host in each of your environments. E.g. in `dev`
+environment, you would like the host to be `dev.domain.com`, in `staging`
+environment `staging.domain.com`, etc. You can easily write a patch for each
+such environment: ```yaml name: ingress dev patches target: apiVersion:
+networking.k8s.io/v1 kind: Ingress name: ingress ops: - name: replace host
+path: /spec/rules/domain.com/host action: replace value: "dev.domain.com"
+list_key: "host" ``` Ez ð ## Example In the `./examples` folder there are 3
+sub-folders: - `/examples/base` with deployment, service and a configmap
+manifests. These are the base manifests which we wish to patch - `/examples/
+patches` contain the patches (notice that both base kubernetes manifests and
+patches can be either in `json` or `yml`/`yaml` format) - `/examples/out` is
+the output directory where the patched resources will be output First, we will
+`dry-run` the patching: ```shell ksux -b examples/base -p examples/patches --
+dry-run ``` You should see the patched manifests printed out to the console.
+Now we can run it and save the patched manifests to the `output` folder:
+```shell ksux -b examples/base -p examples/patches -o examples/out ``` By
+default, the manifests will be saved in `yaml` format with `.yaml` extension.
+If you wish to use the `.yml` extension or save the manifests in `json` format,
+simply provide the `-e` flag with corresponding extension. E.g.: ```shell ksux
+-b examples/base -p examples/patches -o examples/out -e json ```
```

### Comparing `ksux-0.5.4/src/ksux.egg-info/SOURCES.txt` & `ksux-0.5.5/src/ksux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

