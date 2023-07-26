# Comparing `tmp/testflows.github.runners-1.2.230726.1222247.tar.gz` & `tmp/testflows.github.runners-1.2.230726.1223826.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230726.1222247.tar", last modified: Wed Jul 26 22:22:47 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230726.1223826.tar", last modified: Wed Jul 26 22:38:26 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230726.1222247.tar` & `testflows.github.runners-1.2.230726.1223826.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:22:47.750168 testflows.github.runners-1.2.230726.1222247/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1222247/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    33692 2023-07-26 22:22:47.750168 testflows.github.runners-1.2.230726.1222247/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    33100 2023-07-26 21:20:58.000000 testflows.github.runners-1.2.230726.1222247/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 22:22:47.750168 testflows.github.runners-1.2.230726.1222247/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 22:22:47.000000 testflows.github.runners-1.2.230726.1222247/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:22:47.750168 testflows.github.runners-1.2.230726.1222247/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:22:47.750168 testflows.github.runners-1.2.230726.1222247/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:22:47.750168 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 22:22:47.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2780 2023-07-26 21:42:21.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:22:47.750168 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    20372 2023-07-26 21:40:30.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     8431 2023-07-26 21:41:13.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    11027 2023-07-26 22:21:21.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:22:47.750168 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:22:47.750168 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-26 20:21:59.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4856 2023-07-26 21:48:39.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1222247/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:22:47.750168 testflows.github.runners-1.2.230726.1222247/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33692 2023-07-26 22:22:47.000000 testflows.github.runners-1.2.230726.1222247/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 22:22:47.000000 testflows.github.runners-1.2.230726.1222247/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 22:22:47.000000 testflows.github.runners-1.2.230726.1222247/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1222247/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 22:22:47.000000 testflows.github.runners-1.2.230726.1222247/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 22:22:47.000000 testflows.github.runners-1.2.230726.1222247/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1223826/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    33811 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    33219 2023-07-26 22:37:54.000000 testflows.github.runners-1.2.230726.1223826/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.945905 testflows.github.runners-1.2.230726.1223826/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.945905 testflows.github.runners-1.2.230726.1223826/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2780 2023-07-26 21:42:21.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    20678 2023-07-26 22:30:15.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     8457 2023-07-26 22:33:31.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11155 2023-07-26 22:33:17.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-26 20:21:59.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2219 2023-07-26 22:34:32.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33811 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230726.1222247/LICENSE` & `testflows.github.runners-1.2.230726.1223826/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1222247/PKG-INFO` & `testflows.github.runners-1.2.230726.1223826/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1222247
+Version: 1.2.230726.1223826
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -876,14 +876,17 @@
 
 * **--max-idle-runner-time sec**
   maximum time after which an idle runner is removed and its server deleted, default: *120* sec
 
 * **--max-runner-registration-time**
   maximum time after which the server will be deleted if its runner is not registered with GitHub, default: *60* sec
 
+* **--max-server-ready-time sec**
+  maximum time to wait for the server to be in the running state, default: *60* sec
+
 * **--scale-up-interval sec**
   scale up service interval, default: *10* sec
 
 * **--scale-down-interval sec**
   scale down service interval, default: *10* sec
 
 * **--debug**
```

### Comparing `testflows.github.runners-1.2.230726.1222247/README.rst` & `testflows.github.runners-1.2.230726.1223826/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -859,14 +859,17 @@
 
 * **--max-idle-runner-time sec**
   maximum time after which an idle runner is removed and its server deleted, default: *120* sec
 
 * **--max-runner-registration-time**
   maximum time after which the server will be deleted if its runner is not registered with GitHub, default: *60* sec
 
+* **--max-server-ready-time sec**
+  maximum time to wait for the server to be in the running state, default: *60* sec
+
 * **--scale-up-interval sec**
   scale up service interval, default: *10* sec
 
 * **--scale-down-interval sec**
   scale down service interval, default: *10* sec
 
 * **--debug**
```

### Comparing `testflows.github.runners-1.2.230726.1222247/setup.py` & `testflows.github.runners-1.2.230726.1223826/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230726.1222247",
+    version="1.2.230726.1223826",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.2.230726.1222247"
+__version__ = "1.2.230726.1223826"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/bin/github-runners`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,22 @@
         metavar="sec",
         type=args.count_type,
         help="maximum time after which the server will be deleted if it fails to register a runner, default: 60 sec",
         default=60,
     )
 
     parser.add_argument(
+        "--max-server-ready-time",
+        metavar="sec",
+        type=args.count_type,
+        help="maximum time to wait for the server to be in the running state, default: 60 sec",
+        default=60,
+    )
+
+    parser.add_argument(
         "--scale-up-interval",
         metavar="sec",
         type=args.count_type,
         help="scale up service interval, default: 10 sec",
         default=10,
     )
 
@@ -544,14 +552,15 @@
                     default_image=args.default_image,
                     default_location=args.default_location,
                     worker_pool=worker_pool,
                     github_token=args.github_token,
                     github_repository=args.github_repository,
                     interval=args.scale_up_interval,
                     max_servers=args.max_runners,
+                    max_server_ready_time=args.max_server_ready_time,
                 )
 
             with Action("Creating scale down service"):
                 scale_down_service: Future = worker_pool.submit(
                     scale_down,
                     terminate=terminate,
                     repo=repo,
```

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from .server import wait_ready, wait_ssh, ssh
 from .service import command_options
 
 current_dir = os.path.dirname(__file__)
 
 
-def deploy(args, timeout=60):
+def deploy(args):
     """Deploy github-runners as a service to a
     new Hetzner server instance."""
     check(args)
 
     server_name = args.server_name
 
     with Action("Logging in to Hetzner Cloud"):
@@ -73,18 +73,18 @@
             image=args.image,
             location=args.location,
             ssh_keys=[ssh_key],
         )
         server: BoundServer = response.server
 
     with Action(f"Waiting for server to be ready") as action:
-        wait_ready(server=server, timeout=timeout, action=action)
+        wait_ready(server=server, timeout=args.max_server_ready_time, action=action)
 
     with Action("Wait for SSH connection to be ready"):
-        wait_ssh(server=server, timeout=timeout)
+        wait_ssh(server=server, timeout=args.max_server_ready_time)
 
     with Action("Executing setup.sh script"):
         ssh(
             server,
             f"bash -s  < {os.path.join(current_dir, 'scripts', 'deploy', 'setup.sh')}",
         )
```

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scale_up.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
         server_setup,
         server=response.server,
         setup_script=setup_script,
         startup_script=startup_script,
         github_token=github_token,
         github_repository=github_repository,
         runner_labels=",".join(job.raw_data["labels"]),
+        timeout=timeout,
     )
 
 
 def get_server_type(job: WorkflowJob, default: ServerType, label_prefix="type-"):
     """Get server type for the specified job."""
     server_type = None
 
@@ -202,14 +203,15 @@
     github_repository: str,
     ssh_key: SSHKey,
     default_type: ServerType,
     default_location: Location,
     default_image: Image,
     interval: int,
     max_servers: int,
+    max_server_ready_time: int,
 ):
     """Scale up service."""
 
     with ThreadPoolExecutor(
         max_workers=worker_pool._max_workers, thread_name_prefix=f"setup-worker"
     ) as setup_worker_pool:
 
@@ -284,14 +286,15 @@
                                         server_location=server_location,
                                         server_image=server_image,
                                         setup_script=scripts.setup,
                                         startup_script=startup_script,
                                         github_token=github_token,
                                         github_repository=github_repository,
                                         ssh_key=ssh_key,
+                                        timeout=max_server_ready_time,
                                     )
                                 )
 
             for future in futures:
                 with Action("Waiting to finish creating server", ignore_fail=True):
                     future.result()
```

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     start_time = time.time()
 
     while True:
         attempt += 1
         with Action(
             f"Trying to connect to {server.name}@{ip}...{attempt}", ignore_fail=True
         ):
-            returncode = ssh(server, "hostname")
+            returncode = ssh(server, "hostname", check=False)
             if returncode == 0:
                 break
         if time.time() - start_time >= timeout:
             ssh(server, "hostname")
         else:
             time.sleep(5)
```

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         if args.startup_arm64_script
         else ""
     )
     command += (
         f" --max-powered-off-time {args.max_powered_off_time}"
         f" --max-idle-runner-time {args.max_idle_runner_time}"
         f" --max-runner-registration-time {args.max_runner_registration_time}"
+        f" --max-server-ready-time {args.max_server_ready_time}"
         f" --scale-up-interval {args.scale_up_interval}"
         f" --scale-down-interval {args.scale_down_interval}"
     )
     command += f" --debug" if args.debug else ""
 
     return command
```

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1222247
+Version: 1.2.230726.1223826
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -876,14 +876,17 @@
 
 * **--max-idle-runner-time sec**
   maximum time after which an idle runner is removed and its server deleted, default: *120* sec
 
 * **--max-runner-registration-time**
   maximum time after which the server will be deleted if its runner is not registered with GitHub, default: *60* sec
 
+* **--max-server-ready-time sec**
+  maximum time to wait for the server to be in the running state, default: *60* sec
+
 * **--scale-up-interval sec**
   scale up service interval, default: *10* sec
 
 * **--scale-down-interval sec**
   scale down service interval, default: *10* sec
 
 * **--debug**
```

### Comparing `testflows.github.runners-1.2.230726.1222247/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

