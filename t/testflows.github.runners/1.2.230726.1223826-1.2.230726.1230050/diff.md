# Comparing `tmp/testflows.github.runners-1.2.230726.1223826.tar.gz` & `tmp/testflows.github.runners-1.2.230726.1230050.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230726.1223826.tar", last modified: Wed Jul 26 22:38:26 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230726.1230050.tar", last modified: Wed Jul 26 23:00:51 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230726.1223826.tar` & `testflows.github.runners-1.2.230726.1230050.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1223826/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    33811 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    33219 2023-07-26 22:37:54.000000 testflows.github.runners-1.2.230726.1223826/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.945905 testflows.github.runners-1.2.230726.1223826/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.945905 testflows.github.runners-1.2.230726.1223826/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2780 2023-07-26 21:42:21.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    20678 2023-07-26 22:30:15.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     8457 2023-07-26 22:33:31.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    11155 2023-07-26 22:33:17.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-26 20:21:59.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2219 2023-07-26 22:34:32.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1223826/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 22:38:26.949905 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33811 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 22:38:26.000000 testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:00:51.111023 testflows.github.runners-1.2.230726.1230050/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1230050/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    33902 2023-07-26 23:00:51.111023 testflows.github.runners-1.2.230726.1230050/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    33310 2023-07-26 22:59:24.000000 testflows.github.runners-1.2.230726.1230050/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 23:00:51.111023 testflows.github.runners-1.2.230726.1230050/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 23:00:50.000000 testflows.github.runners-1.2.230726.1230050/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:00:51.107023 testflows.github.runners-1.2.230726.1230050/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:00:51.107023 testflows.github.runners-1.2.230726.1230050/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:00:51.107023 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 23:00:50.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2780 2023-07-26 21:42:21.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:00:51.107023 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    20889 2023-07-26 22:59:47.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     9007 2023-07-26 22:56:38.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11155 2023-07-26 22:33:17.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:00:51.111023 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:00:51.111023 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      457 2023-07-26 22:51:58.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2444 2023-07-26 22:48:45.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1230050/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 23:00:51.107023 testflows.github.runners-1.2.230726.1230050/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33902 2023-07-26 23:00:51.000000 testflows.github.runners-1.2.230726.1230050/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 23:00:51.000000 testflows.github.runners-1.2.230726.1230050/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 23:00:51.000000 testflows.github.runners-1.2.230726.1230050/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1230050/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 23:00:51.000000 testflows.github.runners-1.2.230726.1230050/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 23:00:51.000000 testflows.github.runners-1.2.230726.1230050/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230726.1223826/LICENSE` & `testflows.github.runners-1.2.230726.1230050/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1223826/PKG-INFO` & `testflows.github.runners-1.2.230726.1230050/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1223826
+Version: 1.2.230726.1230050
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -915,14 +915,17 @@
           deployment server type, default: *cpx11*
 
         * **-i type:name_or_description, --image type:name_or_description**
           deployment server image type and name or description,
           where the type is either: 'system','snapshot','backup','app',
           default: *system:ubuntu-22.04*
 
+        * **--setup-script path**
+          path to custom deployment server setup script
+
       * **logs**
         get cloud service logs
 
         * **-f, --follow**
           follow logs journal, default: *False*
 
       * **status**
```

### Comparing `testflows.github.runners-1.2.230726.1223826/README.rst` & `testflows.github.runners-1.2.230726.1230050/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -898,14 +898,17 @@
           deployment server type, default: *cpx11*
 
         * **-i type:name_or_description, --image type:name_or_description**
           deployment server image type and name or description,
           where the type is either: 'system','snapshot','backup','app',
           default: *system:ubuntu-22.04*
 
+        * **--setup-script path**
+          path to custom deployment server setup script
+
       * **logs**
         get cloud service logs
 
         * **-f, --follow**
           follow logs journal, default: *False*
 
       * **status**
```

### Comparing `testflows.github.runners-1.2.230726.1223826/setup.py` & `testflows.github.runners-1.2.230726.1230050/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230726.1223826",
+    version="1.2.230726.1230050",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.2.230726.1223826"
+__version__ = "1.2.230726.1230050"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/bin/github-runners`

 * *Files 2% similar despite different names*

```diff
@@ -301,14 +301,22 @@
             "deployment server image type and name or description,\n"
             "where the type is either: 'system','snapshot','backup','app',\n"
             "default: system:ubuntu-22.04"
         ),
         default="system:ubuntu-22.04",
     )
 
+    deploy_cloud_parser.add_argument(
+        "--setup-script",
+        metavar="path",
+        dest="deploy_setup_script",
+        type=str,
+        help="path to custom deployment server setup script",
+    )
+
     deploy_cloud_parser.set_defaults(func=cloud.deploy)
 
     logs_cloud_parser = cloud_commands.add_parser(
         "logs",
         help="get cloud service logs",
         description="Get cloud service logs.",
         formatter_class=RawTextHelpFormatter,
```

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,26 +22,29 @@
 from hcloud.images.domain import Image
 from hcloud.locations.domain import Location
 
 from .actions import Action
 from .args import check, check_image
 from . import __version__
 
-from .server import wait_ready, wait_ssh, ssh
+from .server import wait_ready, wait_ssh, ssh, scp, ip_address
 from .service import command_options
 
 current_dir = os.path.dirname(__file__)
 
 
 def deploy(args):
     """Deploy github-runners as a service to a
     new Hetzner server instance."""
     check(args)
 
     server_name = args.server_name
+    deploy_setup_script = args.deploy_setup_script or os.path.join(
+        current_dir, "scripts", "deploy", "setup.sh"
+    )
 
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=args.hetzner_token)
 
     if args.force:
         with Action(
             f"Checking if server {server_name} already exists", ignore_fail=True
@@ -81,23 +84,36 @@
 
     with Action("Wait for SSH connection to be ready"):
         wait_ssh(server=server, timeout=args.max_server_ready_time)
 
     with Action("Executing setup.sh script"):
         ssh(
             server,
-            f"bash -s  < {os.path.join(current_dir, 'scripts', 'deploy', 'setup.sh')}",
+            f"bash -s  < {deploy_setup_script}",
         )
 
     with Action("Installing github-runners"):
         ssh(
             server,
             f"'sudo -u ubuntu pip3 install testflows.github.runners=={__version__}'",
         )
 
+    with Action("Copying any custom scripts"):
+        ip = ip_address(server)
+        for script in [
+            args.setup_script,
+            args.startup_x64_script,
+            args.startup_arm64_script,
+        ]:
+            if script:
+                with Action(f"Copying custom script {script}"):
+                    scp(
+                        source=script, destination=f"ubuntu@{ip}:/home/ubuntu/scripts/."
+                    )
+
     install(args, server=server)
 
 
 def install(args, server: BoundServer = None):
     """Install service on a cloud instance."""
     if server is None:
         check(args)
```

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,14 +49,20 @@
 def ssh(server: BoundServer, cmd: str, *args, **kwargs):
     """Execute command over SSH."""
     ip = ip_address(server=server)
     ssh_command = f'ssh -q -o "StrictHostKeyChecking no" root@{ip}'
     return shell(f"{ssh_command} {cmd}", *args, **kwargs)
 
 
+def scp(source: str, destination: str, *args, **kwargs):
+    """Execute copy over SSH."""
+    scp_command = f'scp -q -o "StrictHostKeyChecking no" {source} {destination}'
+    return shell(f"{scp_command}", *args, **kwargs)
+
+
 def wait_ready(server: BoundServer, timeout: float, action: Action = None):
     """Wait for server to be ready."""
     start_time = time.time()
 
     while True:
         status = server.status
         if action:
```

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230726.1230050/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230726.1230050/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1223826
+Version: 1.2.230726.1230050
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -915,14 +915,17 @@
           deployment server type, default: *cpx11*
 
         * **-i type:name_or_description, --image type:name_or_description**
           deployment server image type and name or description,
           where the type is either: 'system','snapshot','backup','app',
           default: *system:ubuntu-22.04*
 
+        * **--setup-script path**
+          path to custom deployment server setup script
+
       * **logs**
         get cloud service logs
 
         * **-f, --follow**
           follow logs journal, default: *False*
 
       * **status**
```

### Comparing `testflows.github.runners-1.2.230726.1223826/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230726.1230050/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

