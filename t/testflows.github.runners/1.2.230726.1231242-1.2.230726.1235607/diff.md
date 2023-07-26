# Comparing `tmp/testflows.github.runners-1.2.230726.1231242.tar.gz` & `tmp/testflows.github.runners-1.2.230726.1235607.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230726.1231242.tar", last modified: Wed Jul 26 23:12:42 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230726.1235607.tar", last modified: Wed Jul 26 23:56:07 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230726.1231242.tar` & `testflows.github.runners-1.2.230726.1235607.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:12:42.722975 testflows.github.runners-1.2.230726.1231242/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1231242/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    33902 2023-07-26 23:12:42.722975 testflows.github.runners-1.2.230726.1231242/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    33310 2023-07-26 22:59:24.000000 testflows.github.runners-1.2.230726.1231242/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 23:12:42.722975 testflows.github.runners-1.2.230726.1231242/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 23:12:42.000000 testflows.github.runners-1.2.230726.1231242/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:12:42.718975 testflows.github.runners-1.2.230726.1231242/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:12:42.718975 testflows.github.runners-1.2.230726.1231242/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:12:42.722975 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 23:12:42.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2780 2023-07-26 21:42:21.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:12:42.722975 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    20889 2023-07-26 22:59:47.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     9007 2023-07-26 22:56:38.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    11155 2023-07-26 22:33:17.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:12:42.722975 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:12:42.722975 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      457 2023-07-26 22:51:58.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2444 2023-07-26 22:48:45.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1231242/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:12:42.722975 testflows.github.runners-1.2.230726.1231242/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33902 2023-07-26 23:12:42.000000 testflows.github.runners-1.2.230726.1231242/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 23:12:42.000000 testflows.github.runners-1.2.230726.1231242/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 23:12:42.000000 testflows.github.runners-1.2.230726.1231242/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1231242/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 23:12:42.000000 testflows.github.runners-1.2.230726.1231242/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 23:12:42.000000 testflows.github.runners-1.2.230726.1231242/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:56:07.591235 testflows.github.runners-1.2.230726.1235607/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1235607/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    33902 2023-07-26 23:56:07.591235 testflows.github.runners-1.2.230726.1235607/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    33310 2023-07-26 22:59:24.000000 testflows.github.runners-1.2.230726.1235607/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 23:56:07.591235 testflows.github.runners-1.2.230726.1235607/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 23:56:07.000000 testflows.github.runners-1.2.230726.1235607/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:56:07.587235 testflows.github.runners-1.2.230726.1235607/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:56:07.587235 testflows.github.runners-1.2.230726.1235607/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:56:07.591235 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 23:56:07.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2912 2023-07-26 23:50:21.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:56:07.591235 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    20944 2023-07-26 23:43:05.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    10794 2023-07-26 23:54:56.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11155 2023-07-26 22:33:17.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:56:07.591235 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:56:07.591235 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      517 2023-07-26 23:53:32.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2444 2023-07-26 22:48:45.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1235607/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:56:07.591235 testflows.github.runners-1.2.230726.1235607/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33902 2023-07-26 23:56:07.000000 testflows.github.runners-1.2.230726.1235607/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 23:56:07.000000 testflows.github.runners-1.2.230726.1235607/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 23:56:07.000000 testflows.github.runners-1.2.230726.1235607/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1235607/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 23:56:07.000000 testflows.github.runners-1.2.230726.1235607/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 23:56:07.000000 testflows.github.runners-1.2.230726.1235607/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230726.1231242/LICENSE` & `testflows.github.runners-1.2.230726.1235607/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/PKG-INFO` & `testflows.github.runners-1.2.230726.1235607/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1231242
+Version: 1.2.230726.1235607
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230726.1231242/README.rst` & `testflows.github.runners-1.2.230726.1235607/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/setup.py` & `testflows.github.runners-1.2.230726.1235607/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230726.1231242",
+    version="1.2.230726.1235607",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.2.230726.1231242"
+__version__ = "1.2.230726.1235607"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 from hcloud.server_types.domain import ServerType
 
 
 class ImageNotFoundError(Exception):
     pass
 
 
+def path_type(v):
+    """Path argument type."""
+    v = os.path.abspath(os.path.expanduser(v))
+    os.path.exists(v)
+    return v
+
+
 def count_type(v):
     """Count argument type."""
     v = int(v)
     assert v >= 1
     return v
```

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/bin/github-runners`

 * *Files 2% similar despite different names*

```diff
@@ -149,36 +149,36 @@
         help="number of concurrent workers, default: 10",
         default=10,
     )
 
     parser.add_argument(
         "--logger-config",
         metavar="path",
-        type=str,
+        type=args.path_type,
         help="custom logger configuration file",
     )
 
     parser.add_argument(
         "--setup-script",
         metavar="path",
-        type=str,
+        type=args.path_type,
         help="path to custom server setup script",
     )
 
     parser.add_argument(
         "--startup-x64-script",
         metavar="path",
-        type=str,
+        type=args.path_type,
         help="path to custom x64 server startup script",
     )
 
     parser.add_argument(
         "--startup-arm64-script",
         metavar="path",
-        type=str,
+        type=args.path_type,
         help="path to custom ARM64 server startup script",
     )
 
     parser.add_argument(
         "--max-powered-off-time",
         metavar="sec",
         type=args.count_type,
@@ -305,15 +305,15 @@
         default="system:ubuntu-22.04",
     )
 
     deploy_cloud_parser.add_argument(
         "--setup-script",
         metavar="path",
         dest="deploy_setup_script",
-        type=str,
+        type=args.path_type,
         help="path to custom deployment server setup script",
     )
 
     deploy_cloud_parser.set_defaults(func=cloud.deploy)
 
     logs_cloud_parser = cloud_commands.add_parser(
         "logs",
```

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/cloud.py`

 * *Files 12% similar despite different names*

```diff
@@ -95,24 +95,64 @@
         ssh(
             server,
             f"'sudo -u ubuntu pip3 install testflows.github.runners=={__version__}'",
         )
 
     with Action("Copying any custom scripts"):
         ip = ip_address(server)
-        for script in [
-            args.setup_script,
-            args.startup_x64_script,
-            args.startup_arm64_script,
-        ]:
-            if script:
-                with Action(f"Copying custom script {script}"):
-                    scp(
-                        source=script, destination=f"ubuntu@{ip}:/home/ubuntu/scripts/."
-                    )
+
+        if args.setup_script:
+            with Action(f"Copying custom setup script {args.setup_script}"):
+                scp(
+                    source=args.setup_script,
+                    destination=f"root@{ip}:/home/ubuntu/github-runners.scripts/.",
+                )
+                args.setup_script = os.path.join(
+                    "/home/ubuntu/github-runners.scripts/",
+                    os.path.basename(args.setup_script),
+                )
+
+        if args.startup_x64_script:
+            with Action(f"Copying custom setup script {args.startup_x64_script}"):
+                scp(
+                    source=args.setup_script,
+                    destination=f"root@{ip}:/home/ubuntu/github-runners.scripts/.",
+                )
+                args.startup_x64_script = os.path.join(
+                    "/home/ubuntu/github-runners.scripts/",
+                    os.path.basename(args.startup_x64_script),
+                )
+
+        if args.startup_arm64_script:
+            with Action(f"Copying custom setup script {args.startup_arm64_script}"):
+                scp(
+                    source=args.setup_script,
+                    destination=f"root@{ip}:/home/ubuntu/github-runners.scripts/.",
+                )
+                args.startup_arm64_script = os.path.join(
+                    "/home/ubuntu/github-runners.scripts/",
+                    os.path.basename(args.startup_arm64_script),
+                )
+
+    with Action("Fixing ownership of any copied scripts"):
+        ssh(server, "chown ubuntu:ubuntu /home/ubuntu/github-runners.scripts/*")
+
+    if args.logger_config:
+        with Action(f"Copying custom logger config {args.logger_config}"):
+            scp(
+                source=args.logger_config,
+                destination=f"root@{ip}:/home/ubuntu/github-runners.configs/.",
+            )
+            args.logger_config = os.path.join(
+                "/home/ubuntu/github-runners.configs/",
+                os.path.basename(args.logger_config),
+            )
+
+    with Action("Fixing ownership of any copied configs"):
+        ssh(server, "chown ubuntu:ubuntu /home/ubuntu/github-runners.configs/*")
 
     install(args, server=server)
 
 
 def install(args, server: BoundServer = None):
     """Install service on a cloud instance."""
     if server is None:
```

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230726.1235607/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230726.1235607/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1231242
+Version: 1.2.230726.1235607
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230726.1231242/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230726.1235607/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

