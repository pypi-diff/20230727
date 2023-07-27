# Comparing `tmp/testflows.github.runners-1.2.230727.1151550.tar.gz` & `tmp/testflows.github.runners-1.2.230727.1162300.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230727.1151550.tar", last modified: Thu Jul 27 15:15:50 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230727.1162300.tar", last modified: Thu Jul 27 16:23:00 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230727.1151550.tar` & `testflows.github.runners-1.2.230727.1162300.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230727.1151550/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    35591 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    34999 2023-07-27 15:15:40.000000 testflows.github.runners-1.2.230727.1151550/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.476311 testflows.github.runners-1.2.230727.1151550/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.476311 testflows.github.runners-1.2.230727.1151550/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    21712 2023-07-27 15:11:36.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    11586 2023-07-27 15:12:30.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8529 2023-07-27 10:56:09.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    11155 2023-07-27 02:42:31.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230727.1151550/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 15:15:50.480311 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    35591 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-27 15:15:50.000000 testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 16:23:00.652616 testflows.github.runners-1.2.230727.1162300/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230727.1162300/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    38494 2023-07-27 16:23:00.652616 testflows.github.runners-1.2.230727.1162300/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    37902 2023-07-27 16:22:53.000000 testflows.github.runners-1.2.230727.1162300/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-27 16:23:00.652616 testflows.github.runners-1.2.230727.1162300/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-27 16:23:00.000000 testflows.github.runners-1.2.230727.1162300/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 16:23:00.652616 testflows.github.runners-1.2.230727.1162300/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 16:23:00.652616 testflows.github.runners-1.2.230727.1162300/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 16:23:00.652616 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-27 16:23:00.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3011 2023-07-27 02:43:16.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 16:23:00.652616 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    22613 2023-07-27 16:08:42.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    12777 2023-07-27 16:04:17.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8529 2023-07-27 10:56:09.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11155 2023-07-27 02:42:31.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 16:23:00.652616 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-26 23:10:10.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 16:23:00.652616 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-27 00:03:37.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-27 02:16:34.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-27 15:03:46.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4921 2023-07-26 22:31:47.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230727.1162300/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-27 16:23:00.652616 testflows.github.runners-1.2.230727.1162300/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    38494 2023-07-27 16:23:00.000000 testflows.github.runners-1.2.230727.1162300/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-27 16:23:00.000000 testflows.github.runners-1.2.230727.1162300/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-27 16:23:00.000000 testflows.github.runners-1.2.230727.1162300/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230727.1162300/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-27 16:23:00.000000 testflows.github.runners-1.2.230727.1162300/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-27 16:23:00.000000 testflows.github.runners-1.2.230727.1162300/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230727.1151550/LICENSE` & `testflows.github.runners-1.2.230727.1162300/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/PKG-INFO` & `testflows.github.runners-1.2.230727.1162300/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230727.1151550
+Version: 1.2.230727.1162300
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -238,26 +238,26 @@
 
 You can specify custom runner server setup script using the **--setup-script** option.
 
 For example,
 
 :custom_setup.sh:
    .. code-block:: bash
-   
+
       #!/bin/bash
       set -x
       echo "Create and configure ubuntu user"
       adduser ubuntu --disabled-password --gecos ""
       echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
       addgroup wheel
       addgroup docker
       usermod -aG wheel ubuntu
       usermod -aG sudo ubuntu
       usermod -aG docker ubuntu
-      # custom setup 
+      # custom setup
       apt-get -y update
       apt-get -y install ca-certificates curl gnupg lsb-release python3-pip git unzip
 
 :command:
    .. code-block:: bash
 
       github-runners --setup-script ./custom_setup.sh
@@ -489,14 +489,22 @@
 
    export GITHUB_TOKEN=ghp_...
    export GITHUB_REPOSITORY=testflows/github-runners
    export HETZNER_TOKEN=GJzdc...
 
    github-runners deploy
 
+You can specify the version of the package to be installed using the **--version** option. By default, the current local package
+version will be installed on the cloud service server. You can also pass *latest* as the value to install the latest available
+version.
+
+.. code-block:: bash
+
+   github-runners deploy --version latest
+
 The **deploy** command will use the following default values:
 
 :location:
    *ash*
 :type:
    *cpx11*
 :image:
@@ -552,14 +560,30 @@
 
 Using x64 Instance
 ++++++++++++++++++
 
 By default, the **cpx11** AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used. If you want to use
 a different x64 instance then specify desired type using the **--type** option.
 
+Redeploying Cloud Service
+=========================
+
+You can change cloud service configuration or cloud service package version without deleting the existing cloud service server
+using the **cloud redeploy** command.
+
+.. code-block:: bash
+
+   github-runners <options> cloud redeploy
+
+:✋ Note:
+   The options that are passed to the **github-runners <options> cloud redeploy** command
+   will be the same options with which the service will be executed.
+
+You can specify the version of the package to be installed using the **--version** option.
+
 Cloud Service Logs
 ===================
 
 You can check logs for the **github-runners** service running on a cloud instance using the **github-runners cloud logs** command.
 Specify **-f, --follow** if you want to follow the logs journal.
 
 For example,
@@ -572,15 +596,14 @@
 
 :follow the logs journal:
 
    .. code-block:: bash
 
       github-runners cloud logs -f
 
-
 Cloud Service Status
 =====================
 
 You can check the status of the **github-runners** service running on a cloud instance using the **github-runners cloud status** command.
 
 For example,
 
@@ -631,16 +654,16 @@
 You can manually force uninstallation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud uninstall** command.
 
 .. code-block:: bash
 
    github-runners cloud uninstall
 
-Upgrading Cloud Service
-========================
+Upgrading Cloud Service Package
+===============================
 
 You can manually upgrade the **github-runners** service package running on a cloud instance using
 the **github-runners cloud upgrade** command.
 
 If specific '--version' is specified then the *testflows.github.runners* package is upgraded to
 the specified version otherwise the version is upgraded to the latest available.
 
@@ -649,14 +672,42 @@
    Instead, it is stopped before the upgrade and then started back up
    after the package upgrade is complete.
 
 .. code-block:: bash
 
    github-runners cloud upgrade --version <version>
 
+The service is not re-installed during the package upgrade process.
+Instead, it is stopped before the upgrade and then started back up
+
+Changing Cloud Service Options
+==============================
+
+If you need to change cloud service options such as the **--setup-script** or the **--max-runners** etc.,
+you can keep the existing server and use **cloud redeploy** command.
+
+.. code-block:: bash
+
+   github-runners <options> cloud redeploy --version latest
+
+When needed, you can also SSH into the cloud service manually and perform changes manually.
+
+You can do complete service teardown using the **cloud delete** and then the **cloud deploy** commands.
+
+.. code-block:: bash
+
+   github-runners cloud delete
+   github-runners <options> cloud deploy --version latest
+
+:✋ Note:
+   Complete teardown will not affect any current jobs as the service is designed to
+   be restartable. However, some servers might be left in an unfinished state
+   but they will be cleaned up when the service is restarted.
+
+
 Deleting Cloud Service
 ======================
 
 You can delete the **github-runners** cloud service and the cloud instance that is running on using
 the **github-runners cloud delete** command.
 
 The **cloud delete** command, deletes the cloud service by first stopping the service and then deleting the server instance.
@@ -673,14 +724,36 @@
       github-runners cloud delete
 
 :custom name:
    .. code-block:: bash
 
       github-runners cloud --name <custom_name> delete
 
+SSH in to Cloud Service
+==============================
+
+You can open SSH client to the cloud service using the **cloud ssh** command. For example,
+
+.. code-block:: bash
+
+   github-runners cloud ssh
+
+You can also manually SSH in to the cloud service using the **ssh** utility. For convenience, you can
+retrieve the SSH client command using the **cloud ssh command** command. For example,
+
+.. code-block:: bash
+
+   github-runners cloud ssh command
+
+The output will contain the full **ssh** command including the IP address of the cloud service server.
+
+::
+
+   ssh -q -o "StrictHostKeyChecking no" root@5.161.87.21
+
 ------------------
 Scaling Up Runners
 ------------------
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
@@ -962,28 +1035,39 @@
 
       * **deploy**
         deploy cloud service
 
         * **-f, --force**
           force deployment if already exist
 
+        * **--version number|latest**
+          service package version to deploy, either version number or 'latest',
+          default: current package version
+
         * **-l name, --location name**
           deployment server location, default: *ash*
 
         * **-t name, --type name**
           deployment server type, default: *cpx11*
 
         * **-i type:name_or_description, --image type:name_or_description**
           deployment server image type and name or description,
           where the type is either: 'system','snapshot','backup','app',
           default: *system:ubuntu-22.04*
 
         * **--setup-script path**
           path to custom deployment server setup script
 
+      * **redeploy**
+        redeploy on the same cloud service server
+
+        * **--version number|latest**
+          service package version to deploy, either version number or 'latest',
+          default: current package version
+
       * **logs**
         get cloud service logs
 
         * **-f, --follow**
           follow logs journal, default: *False*
 
       * **status**
```

### Comparing `testflows.github.runners-1.2.230727.1151550/README.rst` & `testflows.github.runners-1.2.230727.1162300/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -221,26 +221,26 @@
 
 You can specify custom runner server setup script using the **--setup-script** option.
 
 For example,
 
 :custom_setup.sh:
    .. code-block:: bash
-   
+
       #!/bin/bash
       set -x
       echo "Create and configure ubuntu user"
       adduser ubuntu --disabled-password --gecos ""
       echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
       addgroup wheel
       addgroup docker
       usermod -aG wheel ubuntu
       usermod -aG sudo ubuntu
       usermod -aG docker ubuntu
-      # custom setup 
+      # custom setup
       apt-get -y update
       apt-get -y install ca-certificates curl gnupg lsb-release python3-pip git unzip
 
 :command:
    .. code-block:: bash
 
       github-runners --setup-script ./custom_setup.sh
@@ -472,14 +472,22 @@
 
    export GITHUB_TOKEN=ghp_...
    export GITHUB_REPOSITORY=testflows/github-runners
    export HETZNER_TOKEN=GJzdc...
 
    github-runners deploy
 
+You can specify the version of the package to be installed using the **--version** option. By default, the current local package
+version will be installed on the cloud service server. You can also pass *latest* as the value to install the latest available
+version.
+
+.. code-block:: bash
+
+   github-runners deploy --version latest
+
 The **deploy** command will use the following default values:
 
 :location:
    *ash*
 :type:
    *cpx11*
 :image:
@@ -535,14 +543,30 @@
 
 Using x64 Instance
 ++++++++++++++++++
 
 By default, the **cpx11** AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used. If you want to use
 a different x64 instance then specify desired type using the **--type** option.
 
+Redeploying Cloud Service
+=========================
+
+You can change cloud service configuration or cloud service package version without deleting the existing cloud service server
+using the **cloud redeploy** command.
+
+.. code-block:: bash
+
+   github-runners <options> cloud redeploy
+
+:✋ Note:
+   The options that are passed to the **github-runners <options> cloud redeploy** command
+   will be the same options with which the service will be executed.
+
+You can specify the version of the package to be installed using the **--version** option.
+
 Cloud Service Logs
 ===================
 
 You can check logs for the **github-runners** service running on a cloud instance using the **github-runners cloud logs** command.
 Specify **-f, --follow** if you want to follow the logs journal.
 
 For example,
@@ -555,15 +579,14 @@
 
 :follow the logs journal:
 
    .. code-block:: bash
 
       github-runners cloud logs -f
 
-
 Cloud Service Status
 =====================
 
 You can check the status of the **github-runners** service running on a cloud instance using the **github-runners cloud status** command.
 
 For example,
 
@@ -614,16 +637,16 @@
 You can manually force uninstallation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud uninstall** command.
 
 .. code-block:: bash
 
    github-runners cloud uninstall
 
-Upgrading Cloud Service
-========================
+Upgrading Cloud Service Package
+===============================
 
 You can manually upgrade the **github-runners** service package running on a cloud instance using
 the **github-runners cloud upgrade** command.
 
 If specific '--version' is specified then the *testflows.github.runners* package is upgraded to
 the specified version otherwise the version is upgraded to the latest available.
 
@@ -632,14 +655,42 @@
    Instead, it is stopped before the upgrade and then started back up
    after the package upgrade is complete.
 
 .. code-block:: bash
 
    github-runners cloud upgrade --version <version>
 
+The service is not re-installed during the package upgrade process.
+Instead, it is stopped before the upgrade and then started back up
+
+Changing Cloud Service Options
+==============================
+
+If you need to change cloud service options such as the **--setup-script** or the **--max-runners** etc.,
+you can keep the existing server and use **cloud redeploy** command.
+
+.. code-block:: bash
+
+   github-runners <options> cloud redeploy --version latest
+
+When needed, you can also SSH into the cloud service manually and perform changes manually.
+
+You can do complete service teardown using the **cloud delete** and then the **cloud deploy** commands.
+
+.. code-block:: bash
+
+   github-runners cloud delete
+   github-runners <options> cloud deploy --version latest
+
+:✋ Note:
+   Complete teardown will not affect any current jobs as the service is designed to
+   be restartable. However, some servers might be left in an unfinished state
+   but they will be cleaned up when the service is restarted.
+
+
 Deleting Cloud Service
 ======================
 
 You can delete the **github-runners** cloud service and the cloud instance that is running on using
 the **github-runners cloud delete** command.
 
 The **cloud delete** command, deletes the cloud service by first stopping the service and then deleting the server instance.
@@ -656,14 +707,36 @@
       github-runners cloud delete
 
 :custom name:
    .. code-block:: bash
 
       github-runners cloud --name <custom_name> delete
 
+SSH in to Cloud Service
+==============================
+
+You can open SSH client to the cloud service using the **cloud ssh** command. For example,
+
+.. code-block:: bash
+
+   github-runners cloud ssh
+
+You can also manually SSH in to the cloud service using the **ssh** utility. For convenience, you can
+retrieve the SSH client command using the **cloud ssh command** command. For example,
+
+.. code-block:: bash
+
+   github-runners cloud ssh command
+
+The output will contain the full **ssh** command including the IP address of the cloud service server.
+
+::
+
+   ssh -q -o "StrictHostKeyChecking no" root@5.161.87.21
+
 ------------------
 Scaling Up Runners
 ------------------
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
@@ -945,28 +1018,39 @@
 
       * **deploy**
         deploy cloud service
 
         * **-f, --force**
           force deployment if already exist
 
+        * **--version number|latest**
+          service package version to deploy, either version number or 'latest',
+          default: current package version
+
         * **-l name, --location name**
           deployment server location, default: *ash*
 
         * **-t name, --type name**
           deployment server type, default: *cpx11*
 
         * **-i type:name_or_description, --image type:name_or_description**
           deployment server image type and name or description,
           where the type is either: 'system','snapshot','backup','app',
           default: *system:ubuntu-22.04*
 
         * **--setup-script path**
           path to custom deployment server setup script
 
+      * **redeploy**
+        redeploy on the same cloud service server
+
+        * **--version number|latest**
+          service package version to deploy, either version number or 'latest',
+          default: current package version
+
       * **logs**
         get cloud service logs
 
         * **-f, --follow**
           follow logs journal, default: *False*
 
       * **status**
```

### Comparing `testflows.github.runners-1.2.230727.1151550/setup.py` & `testflows.github.runners-1.2.230727.1162300/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230727.1151550",
+    version="1.2.230727.1162300",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/__init__.py`

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
-__version__ = "1.2.230727.1151550"
+__version__ = "1.2.230727.1162300"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/bin/github-runners`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,24 @@
         "-f",
         "--force",
         action="store_true",
         help="force deployment if already exist",
     )
 
     deploy_cloud_parser.add_argument(
+        "--version",
+        metavar="number|latest",
+        type=str,
+        help=(
+            f"service package version to deploy, either version number or 'latest',\n"
+            f"default: this version {__version__}"
+        ),
+    )
+
+    deploy_cloud_parser.add_argument(
         "-l",
         "--location",
         metavar="name",
         type=args.location_type,
         help="deployment server location, default: ash",
         default="ash",
     )
@@ -312,14 +322,33 @@
         dest="deploy_setup_script",
         type=args.path_type,
         help="path to custom deployment server setup script",
     )
 
     deploy_cloud_parser.set_defaults(func=cloud.deploy)
 
+    redeploy_cloud_parser = cloud_commands.add_parser(
+        "redeploy",
+        help="redeploy on the same cloud service server",
+        description="Redeploy application as a service on the existing server instance.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    redeploy_cloud_parser.add_argument(
+        "--version",
+        metavar="number|latest",
+        type=str,
+        help=(
+            f"service package version to deploy, either version number or 'latest',\n"
+            f"default: this version {__version__}"
+        ),
+    )
+
+    redeploy_cloud_parser.set_defaults(func=cloud.redeploy)
+
     logs_cloud_parser = cloud_commands.add_parser(
         "logs",
         help="get cloud service logs",
         description="Get cloud service logs.",
         formatter_class=RawTextHelpFormatter,
     )
```

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/cloud.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,78 +30,97 @@
 from .service import command_options
 
 current_dir = os.path.dirname(__file__)
 deploy_scripts_folder = "/home/ubuntu/.github-runners/scripts/"
 deploy_configs_folder = "/home/ubuntu/.github-runners/configs/"
 
 
-def deploy(args):
-    """Deploy github-runners as a service to a
+def deploy(args, redeploy=False):
+    """Deploy or redeploy github-runners as a service to a
     new Hetzner server instance."""
     check(args)
 
+    version = args.version or __version__
+
     server_name = args.server_name
     deploy_setup_script = args.deploy_setup_script or os.path.join(
         current_dir, "scripts", "deploy", "setup.sh"
     )
 
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=args.hetzner_token)
 
-    if args.force:
-        with Action(
-            f"Checking if server {server_name} already exists", ignore_fail=True
-        ):
+    if redeploy:
+        with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
-            with Action(f"Deleting server {server_name}"):
-                server.delete()
 
-    with Action("Checking if default image exists"):
-        args.default_image = check_image(client=client, image=args.default_image)
+        uninstall(server=server)
+
+        with Action("Cleaning copied scripts"):
+            ssh(server, f"rm -rf {deploy_scripts_folder}*")
+
+        with Action("Cleaning copied configs"):
+            ssh(server, f"rm -rf {deploy_configs_folder}*")
+
+    else:
+        if args.force:
+            with Action(
+                f"Checking if server {server_name} already exists", ignore_fail=True
+            ):
+                server: BoundServer = client.servers.get_by_name(server_name)
+                with Action(f"Deleting server {server_name}"):
+                    server.delete()
+
+        with Action("Checking if default image exists"):
+            args.default_image = check_image(client=client, image=args.default_image)
+
+        with Action("Checking if server image exists"):
+            args.image = check_image(client=client, image=args.image)
+
+        with Action(f"Checking if SSH key exists"):
+            with open(args.ssh_key, "r", encoding="utf-8") as ssh_key_file:
+                public_key = ssh_key_file.read()
+            key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
+            ssh_key = SSHKey(name=key_name, public_key=public_key)
+
+            if not client.ssh_keys.get_by_name(name=ssh_key.name):
+                with Action(f"Creating SSH key {ssh_key.name}"):
+                    client.ssh_keys.create(name=ssh_key.name, public_key=ssh_key.public_key)
+
+        with Action(f"Creating new server"):
+            response = client.servers.create(
+                name=server_name,
+                server_type=args.type,
+                image=args.image,
+                location=args.location,
+                ssh_keys=[ssh_key],
+            )
+            server: BoundServer = response.server
 
-    with Action("Checking if server image exists"):
-        args.image = check_image(client=client, image=args.image)
+        with Action(f"Waiting for server to be ready") as action:
+            wait_ready(server=server, timeout=args.max_server_ready_time, action=action)
 
-    with Action(f"Checking if SSH key exists"):
-        with open(args.ssh_key, "r", encoding="utf-8") as ssh_key_file:
-            public_key = ssh_key_file.read()
-        key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
-        ssh_key = SSHKey(name=key_name, public_key=public_key)
-
-        if not client.ssh_keys.get_by_name(name=ssh_key.name):
-            with Action(f"Creating SSH key {ssh_key.name}"):
-                client.ssh_keys.create(name=ssh_key.name, public_key=ssh_key.public_key)
-
-    with Action(f"Creating new server"):
-        response = client.servers.create(
-            name=server_name,
-            server_type=args.type,
-            image=args.image,
-            location=args.location,
-            ssh_keys=[ssh_key],
-        )
-        server: BoundServer = response.server
-
-    with Action(f"Waiting for server to be ready") as action:
-        wait_ready(server=server, timeout=args.max_server_ready_time, action=action)
-
-    with Action("Wait for SSH connection to be ready"):
-        wait_ssh(server=server, timeout=args.max_server_ready_time)
-
-    with Action("Executing setup.sh script"):
-        ssh(
-            server,
-            f"bash -s  < {deploy_setup_script}",
-        )
-
-    with Action("Installing github-runners"):
-        ssh(
-            server,
-            f"'sudo -u ubuntu pip3 install testflows.github.runners=={__version__}'",
-        )
+        with Action("Wait for SSH connection to be ready"):
+            wait_ssh(server=server, timeout=args.max_server_ready_time)
+
+        with Action("Executing setup.sh script"):
+            ssh(
+                server,
+                f"bash -s  < {deploy_setup_script}",
+            )
+
+    with Action(f"Installing github-runners {version}"):
+        command = f"'sudo -u ubuntu pip3 install testflows.github.runners=={version}'"
+
+        if version.strip().lower() == "latest":
+            command = f"'sudo -u ubuntu pip3 install testflows.github.runners'"
+            if redeploy:
+                command.replace("pip3 install", "pip3 install --upgrade")
+
+        ssh(server, command)
 
     with Action("Copying any custom scripts"):
         ip = ip_address(server)
 
         if args.setup_script:
             with Action(f"Copying custom setup script {args.setup_script}"):
                 scp(
@@ -151,14 +170,19 @@
 
     with Action("Fixing ownership of any copied configs"):
         ssh(server, f"chown -R ubuntu:ubuntu {deploy_configs_folder}")
 
     install(args, server=server)
 
 
+def redeploy(args, server: BoundServer = None):
+    """Redeploy service on a existing cloud instance."""
+    deploy(args=args, server=server, redeploy=True)
+
+
 def install(args, server: BoundServer = None):
     """Install service on a cloud instance."""
     if server is None:
         check(args)
 
         server_name = args.server_name
 
@@ -177,39 +201,44 @@
         command += "github-runners"
         command += command_options(args)
         command += " service install -f'\""
 
         ssh(server, command)
 
 
-def upgrade(args):
+def upgrade_package(server, version=None):
+    """Upgrade github-runners application package on a cloud instance."""
+    if version:
+        with Action(f"Upgrading github-runners to version {version}"):
+            ssh(
+                server,
+                f"'sudo -u ubuntu pip3 install testflows.github.runners=={version}'",
+            )
+    else:
+        with Action(f"Upgrading github-runners the latest version"):
+            ssh(
+                server,
+                f"'sudo -u ubuntu pip3 install --upgrade testflows.github.runners'",
+            )
+
+
+def upgrade(args, install_service=False):
     """Upgrade github-runners application on a cloud instance."""
     server_name = args.server_name
     upgrade_version = args.upgrade_version
 
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=args.hetzner_token)
 
     with Action(f"Getting server {server_name}"):
         server: BoundServer = client.servers.get_by_name(server_name)
 
     stop(args, server=server)
 
-    if upgrade_version:
-        with Action(f"Upgrading github-runners to version {upgrade_version}"):
-            ssh(
-                server,
-                f"'sudo -u ubuntu pip3 install testflows.github.runners=={upgrade_version}'",
-            )
-    else:
-        with Action(f"Upgrading github-runners the latest version"):
-            ssh(
-                server,
-                f"'sudo -u ubuntu pip3 install --upgrade testflows.github.runners'",
-            )
+    upgrade_package(server=server, version=upgrade_version)
 
     start(args, server=server)
 
 
 def uninstall(args):
     """Uninstall github-runners service from a cloud instance."""
     server_name = args.server_name
```

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230727.1162300/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230727.1162300/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230727.1151550
+Version: 1.2.230727.1162300
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -238,26 +238,26 @@
 
 You can specify custom runner server setup script using the **--setup-script** option.
 
 For example,
 
 :custom_setup.sh:
    .. code-block:: bash
-   
+
       #!/bin/bash
       set -x
       echo "Create and configure ubuntu user"
       adduser ubuntu --disabled-password --gecos ""
       echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
       addgroup wheel
       addgroup docker
       usermod -aG wheel ubuntu
       usermod -aG sudo ubuntu
       usermod -aG docker ubuntu
-      # custom setup 
+      # custom setup
       apt-get -y update
       apt-get -y install ca-certificates curl gnupg lsb-release python3-pip git unzip
 
 :command:
    .. code-block:: bash
 
       github-runners --setup-script ./custom_setup.sh
@@ -489,14 +489,22 @@
 
    export GITHUB_TOKEN=ghp_...
    export GITHUB_REPOSITORY=testflows/github-runners
    export HETZNER_TOKEN=GJzdc...
 
    github-runners deploy
 
+You can specify the version of the package to be installed using the **--version** option. By default, the current local package
+version will be installed on the cloud service server. You can also pass *latest* as the value to install the latest available
+version.
+
+.. code-block:: bash
+
+   github-runners deploy --version latest
+
 The **deploy** command will use the following default values:
 
 :location:
    *ash*
 :type:
    *cpx11*
 :image:
@@ -552,14 +560,30 @@
 
 Using x64 Instance
 ++++++++++++++++++
 
 By default, the **cpx11** AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used. If you want to use
 a different x64 instance then specify desired type using the **--type** option.
 
+Redeploying Cloud Service
+=========================
+
+You can change cloud service configuration or cloud service package version without deleting the existing cloud service server
+using the **cloud redeploy** command.
+
+.. code-block:: bash
+
+   github-runners <options> cloud redeploy
+
+:✋ Note:
+   The options that are passed to the **github-runners <options> cloud redeploy** command
+   will be the same options with which the service will be executed.
+
+You can specify the version of the package to be installed using the **--version** option.
+
 Cloud Service Logs
 ===================
 
 You can check logs for the **github-runners** service running on a cloud instance using the **github-runners cloud logs** command.
 Specify **-f, --follow** if you want to follow the logs journal.
 
 For example,
@@ -572,15 +596,14 @@
 
 :follow the logs journal:
 
    .. code-block:: bash
 
       github-runners cloud logs -f
 
-
 Cloud Service Status
 =====================
 
 You can check the status of the **github-runners** service running on a cloud instance using the **github-runners cloud status** command.
 
 For example,
 
@@ -631,16 +654,16 @@
 You can manually force uninstallation of the **github-runners** service running on a cloud instance using
 the **github-runners cloud uninstall** command.
 
 .. code-block:: bash
 
    github-runners cloud uninstall
 
-Upgrading Cloud Service
-========================
+Upgrading Cloud Service Package
+===============================
 
 You can manually upgrade the **github-runners** service package running on a cloud instance using
 the **github-runners cloud upgrade** command.
 
 If specific '--version' is specified then the *testflows.github.runners* package is upgraded to
 the specified version otherwise the version is upgraded to the latest available.
 
@@ -649,14 +672,42 @@
    Instead, it is stopped before the upgrade and then started back up
    after the package upgrade is complete.
 
 .. code-block:: bash
 
    github-runners cloud upgrade --version <version>
 
+The service is not re-installed during the package upgrade process.
+Instead, it is stopped before the upgrade and then started back up
+
+Changing Cloud Service Options
+==============================
+
+If you need to change cloud service options such as the **--setup-script** or the **--max-runners** etc.,
+you can keep the existing server and use **cloud redeploy** command.
+
+.. code-block:: bash
+
+   github-runners <options> cloud redeploy --version latest
+
+When needed, you can also SSH into the cloud service manually and perform changes manually.
+
+You can do complete service teardown using the **cloud delete** and then the **cloud deploy** commands.
+
+.. code-block:: bash
+
+   github-runners cloud delete
+   github-runners <options> cloud deploy --version latest
+
+:✋ Note:
+   Complete teardown will not affect any current jobs as the service is designed to
+   be restartable. However, some servers might be left in an unfinished state
+   but they will be cleaned up when the service is restarted.
+
+
 Deleting Cloud Service
 ======================
 
 You can delete the **github-runners** cloud service and the cloud instance that is running on using
 the **github-runners cloud delete** command.
 
 The **cloud delete** command, deletes the cloud service by first stopping the service and then deleting the server instance.
@@ -673,14 +724,36 @@
       github-runners cloud delete
 
 :custom name:
    .. code-block:: bash
 
       github-runners cloud --name <custom_name> delete
 
+SSH in to Cloud Service
+==============================
+
+You can open SSH client to the cloud service using the **cloud ssh** command. For example,
+
+.. code-block:: bash
+
+   github-runners cloud ssh
+
+You can also manually SSH in to the cloud service using the **ssh** utility. For convenience, you can
+retrieve the SSH client command using the **cloud ssh command** command. For example,
+
+.. code-block:: bash
+
+   github-runners cloud ssh command
+
+The output will contain the full **ssh** command including the IP address of the cloud service server.
+
+::
+
+   ssh -q -o "StrictHostKeyChecking no" root@5.161.87.21
+
 ------------------
 Scaling Up Runners
 ------------------
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
@@ -962,28 +1035,39 @@
 
       * **deploy**
         deploy cloud service
 
         * **-f, --force**
           force deployment if already exist
 
+        * **--version number|latest**
+          service package version to deploy, either version number or 'latest',
+          default: current package version
+
         * **-l name, --location name**
           deployment server location, default: *ash*
 
         * **-t name, --type name**
           deployment server type, default: *cpx11*
 
         * **-i type:name_or_description, --image type:name_or_description**
           deployment server image type and name or description,
           where the type is either: 'system','snapshot','backup','app',
           default: *system:ubuntu-22.04*
 
         * **--setup-script path**
           path to custom deployment server setup script
 
+      * **redeploy**
+        redeploy on the same cloud service server
+
+        * **--version number|latest**
+          service package version to deploy, either version number or 'latest',
+          default: current package version
+
       * **logs**
         get cloud service logs
 
         * **-f, --follow**
           follow logs journal, default: *False*
 
       * **status**
```

### Comparing `testflows.github.runners-1.2.230727.1151550/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230727.1162300/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

