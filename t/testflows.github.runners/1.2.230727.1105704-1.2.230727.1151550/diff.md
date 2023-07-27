# Comparing `tmp/testflows.github.runners-1.2.230727.1105704.tar.gz` & `tmp/testflows.github.runners-1.2.230727.1151550.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230727.1105704.tar", last modified: Thu Jul 27 10:57:04 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230727.1151550.tar", last modified: Thu Jul 27 15:15:50 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230727.1105704.tar` & `testflows.github.runners-1.2.230727.1151550.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 10:57:04.671359 testflows.github.runners-1.2.230727.1105704/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230727.1105704/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    33902 2023-07-27 10:57:04.671359 testflows.github.runners-1.2.230727.1105704/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    33310 2023-07-26 22:59:24.000000 testflows.github.runners-1.2.230727.1105704/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-27 10:57:04.671359 testflows.github.runners-1.2.230727.1105704/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-27 10:57:04.000000 testflows.github.runners-1.2.230727.1105704/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 10:57:04.667359 testflows.github.runners-1.2.230727.1105704/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 10:57:04.667359 testflows.github.runners-1.2.230727.1105704/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 10:57:04.671359 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-27 10:57:04.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 10:57:04.671359 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    20946 2023-07-27 01:45:28.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    10782 2023-07-27 00:08:43.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8529 2023-07-27 10:56:09.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    11155 2023-07-27 02:42:31.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 10:57:04.671359 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 10:57:04.671359 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2444 2023-07-26 22:48:45.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230727.1105704/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 10:57:04.667359 testflows.github.runners-1.2.230727.1105704/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33902 2023-07-27 10:57:04.000000 testflows.github.runners-1.2.230727.1105704/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-27 10:57:04.000000 testflows.github.runners-1.2.230727.1105704/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-27 10:57:04.000000 testflows.github.runners-1.2.230727.1105704/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230727.1105704/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-27 10:57:04.000000 testflows.github.runners-1.2.230727.1105704/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-27 10:57:04.000000 testflows.github.runners-1.2.230727.1105704/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230727.1151550/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    35591 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    34999 2023-07-27 15:15:40.000000 testflows.github.runners-1.2.230727.1151550/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.476311 testflows.github.runners-1.2.230727.1151550/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.476311 testflows.github.runners-1.2.230727.1151550/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    21712 2023-07-27 15:11:36.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    11586 2023-07-27 15:12:30.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8529 2023-07-27 10:56:09.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11155 2023-07-27 02:42:31.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    35591 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230727.1105704/LICENSE` & `testflows.github.runners-1.2.230727.1151550/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/PKG-INFO` & `testflows.github.runners-1.2.230727.1151550/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230727.1105704
+Version: 1.2.230727.1151550
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -123,14 +123,24 @@
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
+------------------------------------
+Specifying Maximum Number of Runners
+------------------------------------
+The default maximum number of runners is **10**. You can set a different value
+based on your Hetzner Cloud limits using the **-m count, --max-runners count** option. For example,
+
+.. code-block:: bash
+
+   github-runners --max-runners 40
+
 ----------------------
 Specifying Runner Type
 ----------------------
 
 x64 Runners
 ============
 
@@ -195,18 +205,66 @@
 option to force specific default server image.
 
 You can also use the **image-{type}-{name}** runner label to specify server image for a specific job. Where the **{name}** must be a valid
 Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*, and the **{type}** is either *system*, *snapshot*, *backup*, or *app*.
 
 For example,
 
-.. code-block:: yaml
+:ubuntu-20.04:
 
-   job-name:
-      runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
+
+
+:docker-ce app:
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cx11, in-ash, image-app-docker-ce]
+
+:snapshot:
+   For snapshots, specify **description** as the name. Snapshot descriptions
+   must be unique.
+
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cx11, in-ash, image-snapshot-snapshot_description]
+
+--------------------------------------------
+Specifying Custom Runner Server Setup Script
+--------------------------------------------
+
+You can specify custom runner server setup script using the **--setup-script** option.
+
+For example,
+
+:custom_setup.sh:
+   .. code-block:: bash
+   
+      #!/bin/bash
+      set -x
+      echo "Create and configure ubuntu user"
+      adduser ubuntu --disabled-password --gecos ""
+      echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
+      addgroup wheel
+      addgroup docker
+      usermod -aG wheel ubuntu
+      usermod -aG sudo ubuntu
+      usermod -aG docker ubuntu
+      # custom setup 
+      apt-get -y update
+      apt-get -y install ca-certificates curl gnupg lsb-release python3-pip git unzip
+
+:command:
+   .. code-block:: bash
+
+      github-runners --setup-script ./custom_setup.sh
 
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
@@ -850,15 +908,15 @@
 
 * **--default-image type:name_or_description**
   default runner server image type and name or description,
   where type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
-  maximum number of active runners, default: *unlimited*
+  maximum number of active runners, default: *10*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
 * **--logger-config path**
   custom logger configuration file
 
@@ -868,30 +926,30 @@
 * **--startup-x64-script path**
   path to custom server startup script
 
 * **--startup-arm64-script path**
   path to custom ARM64 server startup script
 
 * **--max-powered-off-time sec**
-  maximum time after which a powered off server is deleted, default: *20* sec
+  maximum time after which a powered off server is deleted, default: *60* sec
 
 * **--max-idle-runner-time sec**
   maximum time after which an idle runner is removed and its server deleted, default: *120* sec
 
 * **--max-runner-registration-time**
-  maximum time after which the server will be deleted if its runner is not registered with GitHub, default: *60* sec
+  maximum time after which the server will be deleted if its runner is not registered with GitHub, default: *120* sec
 
 * **--max-server-ready-time sec**
-  maximum time to wait for the server to be in the running state, default: *60* sec
+  maximum time to wait for the server to be in the running state, default: *120* sec
 
 * **--scale-up-interval sec**
-  scale up service interval, default: *10* sec
+  scale up service interval, default: *15* sec
 
 * **--scale-down-interval sec**
-  scale down service interval, default: *10* sec
+  scale down service interval, default: *15* sec
 
 * **--debug**
   enable debugging mode, default: *False*
 
 * **commands:**
 
   * *command*
@@ -948,14 +1006,20 @@
 
       * **upgrade**
         upgrade cloud service
 
         * **--version version**
           package version, default: *the latest*
 
+      * **ssh**
+        ssh to cloud service
+
+        * **command**
+          print ssh command to cloud service
+
     * **service**
       service commands
 
       * **install**
         install service
 
         * **-f, --force**
```

### Comparing `testflows.github.runners-1.2.230727.1105704/README.rst` & `testflows.github.runners-1.2.230727.1151550/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,24 @@
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
+------------------------------------
+Specifying Maximum Number of Runners
+------------------------------------
+The default maximum number of runners is **10**. You can set a different value
+based on your Hetzner Cloud limits using the **-m count, --max-runners count** option. For example,
+
+.. code-block:: bash
+
+   github-runners --max-runners 40
+
 ----------------------
 Specifying Runner Type
 ----------------------
 
 x64 Runners
 ============
 
@@ -178,18 +188,66 @@
 option to force specific default server image.
 
 You can also use the **image-{type}-{name}** runner label to specify server image for a specific job. Where the **{name}** must be a valid
 Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*, and the **{type}** is either *system*, *snapshot*, *backup*, or *app*.
 
 For example,
 
-.. code-block:: yaml
+:ubuntu-20.04:
 
-   job-name:
-      runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
+
+
+:docker-ce app:
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cx11, in-ash, image-app-docker-ce]
+
+:snapshot:
+   For snapshots, specify **description** as the name. Snapshot descriptions
+   must be unique.
+
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cx11, in-ash, image-snapshot-snapshot_description]
+
+--------------------------------------------
+Specifying Custom Runner Server Setup Script
+--------------------------------------------
+
+You can specify custom runner server setup script using the **--setup-script** option.
+
+For example,
+
+:custom_setup.sh:
+   .. code-block:: bash
+   
+      #!/bin/bash
+      set -x
+      echo "Create and configure ubuntu user"
+      adduser ubuntu --disabled-password --gecos ""
+      echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
+      addgroup wheel
+      addgroup docker
+      usermod -aG wheel ubuntu
+      usermod -aG sudo ubuntu
+      usermod -aG docker ubuntu
+      # custom setup 
+      apt-get -y update
+      apt-get -y install ca-certificates curl gnupg lsb-release python3-pip git unzip
+
+:command:
+   .. code-block:: bash
+
+      github-runners --setup-script ./custom_setup.sh
 
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
@@ -833,15 +891,15 @@
 
 * **--default-image type:name_or_description**
   default runner server image type and name or description,
   where type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
-  maximum number of active runners, default: *unlimited*
+  maximum number of active runners, default: *10*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
 * **--logger-config path**
   custom logger configuration file
 
@@ -851,30 +909,30 @@
 * **--startup-x64-script path**
   path to custom server startup script
 
 * **--startup-arm64-script path**
   path to custom ARM64 server startup script
 
 * **--max-powered-off-time sec**
-  maximum time after which a powered off server is deleted, default: *20* sec
+  maximum time after which a powered off server is deleted, default: *60* sec
 
 * **--max-idle-runner-time sec**
   maximum time after which an idle runner is removed and its server deleted, default: *120* sec
 
 * **--max-runner-registration-time**
-  maximum time after which the server will be deleted if its runner is not registered with GitHub, default: *60* sec
+  maximum time after which the server will be deleted if its runner is not registered with GitHub, default: *120* sec
 
 * **--max-server-ready-time sec**
-  maximum time to wait for the server to be in the running state, default: *60* sec
+  maximum time to wait for the server to be in the running state, default: *120* sec
 
 * **--scale-up-interval sec**
-  scale up service interval, default: *10* sec
+  scale up service interval, default: *15* sec
 
 * **--scale-down-interval sec**
-  scale down service interval, default: *10* sec
+  scale down service interval, default: *15* sec
 
 * **--debug**
   enable debugging mode, default: *False*
 
 * **commands:**
 
   * *command*
@@ -931,14 +989,20 @@
 
       * **upgrade**
         upgrade cloud service
 
         * **--version version**
           package version, default: *the latest*
 
+      * **ssh**
+        ssh to cloud service
+
+        * **command**
+          print ssh command to cloud service
+
     * **service**
       service commands
 
       * **install**
         install service
 
         * **-f, --force**
```

### Comparing `testflows.github.runners-1.2.230727.1105704/setup.py` & `testflows.github.runners-1.2.230727.1151550/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230727.1105704",
+    version="1.2.230727.1151550",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/__init__.py`

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
-__version__ = "1.2.230727.1105704"
+__version__ = "1.2.230727.1151550"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/bin/github-runners`

 * *Files 3% similar despite different names*

```diff
@@ -107,15 +107,16 @@
     )
 
     parser.add_argument(
         "-m",
         "--max-runners",
         metavar="count",
         type=args.count_type,
-        help="maximum number of active runners, default: unlimited",
+        help="maximum number of active runners, default: 10",
+        default=10,
     )
 
     parser.add_argument(
         "--default-image",
         metavar="type:name_or_description",
         type=args.image_type,
         help=(
@@ -178,56 +179,56 @@
         help="path to custom ARM64 server startup script",
     )
 
     parser.add_argument(
         "--max-powered-off-time",
         metavar="sec",
         type=args.count_type,
-        help="maximum time after which a powered off server is deleted, default: 20 sec",
-        default=20,
+        help="maximum time after which a powered off server is deleted, default: 60 sec",
+        default=60,
     )
 
     parser.add_argument(
         "--max-idle-runner-time",
         metavar="sec",
         type=args.count_type,
         help="maximum time after which an idle runner is removed and its server deleted, default: 120 sec",
         default=120,
     )
 
     parser.add_argument(
         "--max-runner-registration-time",
         metavar="sec",
         type=args.count_type,
-        help="maximum time after which the server will be deleted if it fails to register a runner, default: 60 sec",
-        default=60,
+        help="maximum time after which the server will be deleted if it fails to register a runner, default: 120 sec",
+        default=120,
     )
 
     parser.add_argument(
         "--max-server-ready-time",
         metavar="sec",
         type=args.count_type,
-        help="maximum time to wait for the server to be in the running state, default: 60 sec",
-        default=60,
+        help="maximum time to wait for the server to be in the running state, default: 120 sec",
+        default=120,
     )
 
     parser.add_argument(
         "--scale-up-interval",
         metavar="sec",
         type=args.count_type,
-        help="scale up service interval, default: 10 sec",
-        default=10,
+        help="scale up service interval, default: 15 sec",
+        default=15,
     )
 
     parser.add_argument(
         "--scale-down-interval",
         metavar="sec",
         type=args.count_type,
-        help="scale down service interval, default: 10 sec",
-        default=10,
+        help="scale down service interval, default: 15 sec",
+        default=15,
     )
 
     parser.add_argument(
         "--debug",
         action="store_true",
         help="enable debugging mode, default: False",
         default=False,
@@ -354,14 +355,36 @@
         help="stop cloud service",
         description="Stop cloud service.",
         formatter_class=RawTextHelpFormatter,
     )
 
     stop_cloud_parser.set_defaults(func=cloud.stop)
 
+    ssh_cloud_parser = cloud_commands.add_parser(
+        "ssh",
+        help="ssh to cloud service",
+        description="Open SSH client to cloud service.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    ssh_cloud_parser.set_defaults(func=cloud.ssh_client)
+
+    ssh_cloud_commands = ssh_cloud_parser.add_subparsers(
+        title="commands", metavar="command", description=None, help=None
+    )
+
+    ssh_client_command_cloud_parser = ssh_cloud_commands.add_parser(
+        "command",
+        help="print ssh command to cloud service",
+        description="Get SSH command to connect to cloud service.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    ssh_client_command_cloud_parser.set_defaults(func=cloud.ssh_client_command)
+
     install_cloud_parser = cloud_commands.add_parser(
         "install",
         help="install cloud service",
         description=(
             "Install cloud service.\n\n"
             "The `github-runners <options> service install` command will be executed on the cloud server instance.\n\n"
             "Note: Just like with the `github-runners <options> service install` command,\n"
```

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from hcloud.images.domain import Image
 from hcloud.locations.domain import Location
 
 from .actions import Action
 from .args import check, check_image
 from . import __version__
 
-from .server import wait_ready, wait_ssh, ssh, scp, ip_address
+from .server import wait_ready, wait_ssh, ssh, scp, ip_address, ssh_command
 from .service import command_options
 
 current_dir = os.path.dirname(__file__)
 deploy_scripts_folder = "/home/ubuntu/.github-runners/scripts/"
 deploy_configs_folder = "/home/ubuntu/.github-runners/configs/"
 
 
@@ -309,7 +309,34 @@
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Stopping service"):
         command = f"\"su - ubuntu -c 'github-runners service stop'\""
         ssh(server, command)
+
+
+def ssh_client(args):
+    """Open ssh client to github-runners service running
+    on Hetzner server instance.
+    """
+    server_name = args.server_name
+
+    with Action("Logging in to Hetzner Cloud"):
+        client = Client(token=args.hetzner_token)
+
+    with Action(f"Getting server {server_name}"):
+        server: BoundServer = client.servers.get_by_name(server_name)
+
+    with Action("Opening SSH client"):
+        os.system(ssh_command(server=server))
+
+
+def ssh_client_command(args):
+    """Return ssh command to connect to github-runners service running
+    on Hetzner server instance.
+    """
+    server_name = args.server_name
+
+    client = Client(token=args.hetzner_token)
+    server: BoundServer = client.servers.get_by_name(server_name)
+    print(ssh_command(server=server))
```

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,19 +42,23 @@
                 break
         if time.time() - start_time >= timeout:
             ssh(server, "hostname")
         else:
             time.sleep(5)
 
 
+def ssh_command(server: BoundServer):
+    """Return ssh command."""
+    ip = ip_address(server=server)
+    return f'ssh -q -o "StrictHostKeyChecking no" root@{ip}'
+
+
 def ssh(server: BoundServer, cmd: str, *args, **kwargs):
     """Execute command over SSH."""
-    ip = ip_address(server=server)
-    ssh_command = f'ssh -q -o "StrictHostKeyChecking no" root@{ip}'
-    return shell(f"{ssh_command} {cmd}", *args, **kwargs)
+    return shell(f"{ssh_command(server=server)} {cmd}", *args, **kwargs)
 
 
 def scp(source: str, destination: str, *args, **kwargs):
     """Execute copy over SSH."""
     scp_command = f'scp -q -o "StrictHostKeyChecking no" {source} {destination}'
     return shell(f"{scp_command}", *args, **kwargs)
```

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230727.1105704
+Version: 1.2.230727.1151550
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -123,14 +123,24 @@
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
+------------------------------------
+Specifying Maximum Number of Runners
+------------------------------------
+The default maximum number of runners is **10**. You can set a different value
+based on your Hetzner Cloud limits using the **-m count, --max-runners count** option. For example,
+
+.. code-block:: bash
+
+   github-runners --max-runners 40
+
 ----------------------
 Specifying Runner Type
 ----------------------
 
 x64 Runners
 ============
 
@@ -195,18 +205,66 @@
 option to force specific default server image.
 
 You can also use the **image-{type}-{name}** runner label to specify server image for a specific job. Where the **{name}** must be a valid
 Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*, and the **{type}** is either *system*, *snapshot*, *backup*, or *app*.
 
 For example,
 
-.. code-block:: yaml
+:ubuntu-20.04:
 
-   job-name:
-      runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
+
+
+:docker-ce app:
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cx11, in-ash, image-app-docker-ce]
+
+:snapshot:
+   For snapshots, specify **description** as the name. Snapshot descriptions
+   must be unique.
+
+   .. code-block:: yaml
+
+      job-name:
+         runs-on: [self-hosted, type-cx11, in-ash, image-snapshot-snapshot_description]
+
+--------------------------------------------
+Specifying Custom Runner Server Setup Script
+--------------------------------------------
+
+You can specify custom runner server setup script using the **--setup-script** option.
+
+For example,
+
+:custom_setup.sh:
+   .. code-block:: bash
+   
+      #!/bin/bash
+      set -x
+      echo "Create and configure ubuntu user"
+      adduser ubuntu --disabled-password --gecos ""
+      echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
+      addgroup wheel
+      addgroup docker
+      usermod -aG wheel ubuntu
+      usermod -aG sudo ubuntu
+      usermod -aG docker ubuntu
+      # custom setup 
+      apt-get -y update
+      apt-get -y install ca-certificates curl gnupg lsb-release python3-pip git unzip
+
+:command:
+   .. code-block:: bash
+
+      github-runners --setup-script ./custom_setup.sh
 
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
@@ -850,15 +908,15 @@
 
 * **--default-image type:name_or_description**
   default runner server image type and name or description,
   where type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
-  maximum number of active runners, default: *unlimited*
+  maximum number of active runners, default: *10*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
 * **--logger-config path**
   custom logger configuration file
 
@@ -868,30 +926,30 @@
 * **--startup-x64-script path**
   path to custom server startup script
 
 * **--startup-arm64-script path**
   path to custom ARM64 server startup script
 
 * **--max-powered-off-time sec**
-  maximum time after which a powered off server is deleted, default: *20* sec
+  maximum time after which a powered off server is deleted, default: *60* sec
 
 * **--max-idle-runner-time sec**
   maximum time after which an idle runner is removed and its server deleted, default: *120* sec
 
 * **--max-runner-registration-time**
-  maximum time after which the server will be deleted if its runner is not registered with GitHub, default: *60* sec
+  maximum time after which the server will be deleted if its runner is not registered with GitHub, default: *120* sec
 
 * **--max-server-ready-time sec**
-  maximum time to wait for the server to be in the running state, default: *60* sec
+  maximum time to wait for the server to be in the running state, default: *120* sec
 
 * **--scale-up-interval sec**
-  scale up service interval, default: *10* sec
+  scale up service interval, default: *15* sec
 
 * **--scale-down-interval sec**
-  scale down service interval, default: *10* sec
+  scale down service interval, default: *15* sec
 
 * **--debug**
   enable debugging mode, default: *False*
 
 * **commands:**
 
   * *command*
@@ -948,14 +1006,20 @@
 
       * **upgrade**
         upgrade cloud service
 
         * **--version version**
           package version, default: *the latest*
 
+      * **ssh**
+        ssh to cloud service
+
+        * **command**
+          print ssh command to cloud service
+
     * **service**
       service commands
 
       * **install**
         install service
 
         * **-f, --force**
```

### Comparing `testflows.github.runners-1.2.230727.1105704/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

