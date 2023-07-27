# Comparing `tmp/aws-parallelcluster-node-3.6.1.tar.gz` & `tmp/aws-parallelcluster-node-3.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-parallelcluster-node-3.6.1.tar", last modified: Wed Jul  5 14:13:50 2023, max compression
+gzip compressed data, was "aws-parallelcluster-node-3.7.0b1.tar", last modified: Thu Jul 27 19:22:07 2023, max compression
```

## Comparing `aws-parallelcluster-node-3.6.1.tar` & `aws-parallelcluster-node-3.7.0b1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:13:50.743219 aws-parallelcluster-node-3.6.1/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11358 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/LICENSE.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      102 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/NOTICE.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      732 2023-07-05 14:13:50.743219 aws-parallelcluster-node-3.6.1/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      748 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/README.md
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       38 2023-07-05 14:13:50.743219 aws-parallelcluster-node-3.6.1/setup.cfg
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2298 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/setup.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:13:50.735219 aws-parallelcluster-node-3.6.1/src/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:13:50.735219 aws-parallelcluster-node-3.6.1/src/aws_parallelcluster_node.egg-info/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      732 2023-07-05 14:13:50.000000 aws-parallelcluster-node-3.6.1/src/aws_parallelcluster_node.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1338 2023-07-05 14:13:50.000000 aws-parallelcluster-node-3.6.1/src/aws_parallelcluster_node.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2023-07-05 14:13:50.000000 aws-parallelcluster-node-3.6.1/src/aws_parallelcluster_node.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      257 2023-07-05 14:13:50.000000 aws-parallelcluster-node-3.6.1/src/aws_parallelcluster_node.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2023-07-05 14:13:50.000000 aws-parallelcluster-node-3.6.1/src/aws_parallelcluster_node.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       30 2023-07-05 14:13:50.000000 aws-parallelcluster-node-3.6.1/src/aws_parallelcluster_node.egg-info/requires.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       20 2023-07-05 14:13:50.000000 aws-parallelcluster-node-3.6.1/src/aws_parallelcluster_node.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:13:50.739219 aws-parallelcluster-node-3.6.1/src/common/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/common/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1284 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/common/ec2_utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:13:50.739219 aws-parallelcluster-node-3.6.1/src/common/schedulers/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/common/schedulers/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    16552 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/common/schedulers/slurm_commands.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      733 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/common/time_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11793 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/common/utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:13:50.739219 aws-parallelcluster-node-3.6.1/src/slurm_plugin/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    31297 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/cluster_event_publisher.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    63920 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/clustermgtd.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5071 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9891 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/computemgtd.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4232 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/console_logger.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    17504 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/fleet_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6565 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/fleet_status_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    22767 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/instance_manager.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:13:50.743219 aws-parallelcluster-node-3.6.1/src/slurm_plugin/logging/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1117 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      343 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/logging/parallelcluster_computemgtd_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      382 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/logging/parallelcluster_fleet_status_manager_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      710 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/logging/parallelcluster_resume_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      369 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/logging/parallelcluster_suspend_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11351 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/resume.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    25616 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/slurm_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3658 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/suspend.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3268 2023-07-05 10:19:12.000000 aws-parallelcluster-node-3.6.1/src/slurm_plugin/task_executor.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:07.921122 aws-parallelcluster-node-3.7.0b1/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11358 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/LICENSE.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      102 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/NOTICE.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      734 2023-07-27 19:22:07.921122 aws-parallelcluster-node-3.7.0b1/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      748 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/README.md
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       38 2023-07-27 19:22:07.921122 aws-parallelcluster-node-3.7.0b1/setup.cfg
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2300 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/setup.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:07.917122 aws-parallelcluster-node-3.7.0b1/src/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:07.917122 aws-parallelcluster-node-3.7.0b1/src/aws_parallelcluster_node.egg-info/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      734 2023-07-27 19:22:07.000000 aws-parallelcluster-node-3.7.0b1/src/aws_parallelcluster_node.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1338 2023-07-27 19:22:07.000000 aws-parallelcluster-node-3.7.0b1/src/aws_parallelcluster_node.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2023-07-27 19:22:07.000000 aws-parallelcluster-node-3.7.0b1/src/aws_parallelcluster_node.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      257 2023-07-27 19:22:07.000000 aws-parallelcluster-node-3.7.0b1/src/aws_parallelcluster_node.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2023-07-27 19:22:07.000000 aws-parallelcluster-node-3.7.0b1/src/aws_parallelcluster_node.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       30 2023-07-27 19:22:07.000000 aws-parallelcluster-node-3.7.0b1/src/aws_parallelcluster_node.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       20 2023-07-27 19:22:07.000000 aws-parallelcluster-node-3.7.0b1/src/aws_parallelcluster_node.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:07.917122 aws-parallelcluster-node-3.7.0b1/src/common/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/common/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1284 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/common/ec2_utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:07.917122 aws-parallelcluster-node-3.7.0b1/src/common/schedulers/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/common/schedulers/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    18692 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/common/schedulers/slurm_commands.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      733 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/common/time_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12674 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/common/utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:07.921122 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    31297 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/cluster_event_publisher.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    63914 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/clustermgtd.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5218 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9891 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/computemgtd.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4232 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/console_logger.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    18138 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/fleet_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6779 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/fleet_status_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    54847 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/instance_manager.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:07.921122 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/logging/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1117 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      343 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/logging/parallelcluster_computemgtd_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      382 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/logging/parallelcluster_fleet_status_manager_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      710 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/logging/parallelcluster_resume_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      369 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/logging/parallelcluster_suspend_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12607 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/resume.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    29145 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/slurm_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3658 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/suspend.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3268 2023-07-27 14:47:07.000000 aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/task_executor.py
```

### Comparing `aws-parallelcluster-node-3.6.1/LICENSE.txt` & `aws-parallelcluster-node-3.7.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/PKG-INFO` & `aws-parallelcluster-node-3.7.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster-node
-Version: 3.6.1
+Version: 3.7.0b1
 Summary: aws-parallelcluster-node provides the scripts for an AWS ParallelCluster node.
 Home-page: https://github.com/aws/aws-parallelcluster-node
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-parallelcluster-node-3.6.1/README.md` & `aws-parallelcluster-node-3.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/setup.py` & `aws-parallelcluster-node-3.7.0b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 console_scripts = [
     "slurm_resume = slurm_plugin.resume:main",
     "slurm_suspend = slurm_plugin.suspend:main",
     "slurm_fleet_status_manager = slurm_plugin.fleet_status_manager:main",
     "clustermgtd = slurm_plugin.clustermgtd:main",
     "computemgtd = slurm_plugin.computemgtd:main",
 ]
-version = "3.6.1"
+version = "3.7.0b1"
 requires = ["boto3>=1.7.55", "retrying>=1.3.3"]
 
 setup(
     name="aws-parallelcluster-node",
     version=version,
     author="Amazon Web Services",
     description="aws-parallelcluster-node provides the scripts for an AWS ParallelCluster node.",
```

### Comparing `aws-parallelcluster-node-3.6.1/src/aws_parallelcluster_node.egg-info/PKG-INFO` & `aws-parallelcluster-node-3.7.0b1/src/aws_parallelcluster_node.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster-node
-Version: 3.6.1
+Version: 3.7.0b1
 Summary: aws-parallelcluster-node provides the scripts for an AWS ParallelCluster node.
 Home-page: https://github.com/aws/aws-parallelcluster-node
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-parallelcluster-node-3.6.1/src/aws_parallelcluster_node.egg-info/SOURCES.txt` & `aws-parallelcluster-node-3.7.0b1/src/aws_parallelcluster_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/src/common/__init__.py` & `aws-parallelcluster-node-3.7.0b1/src/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/src/common/ec2_utils.py` & `aws-parallelcluster-node-3.7.0b1/src/common/ec2_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/src/common/schedulers/__init__.py` & `aws-parallelcluster-node-3.7.0b1/src/common/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/src/common/schedulers/slurm_commands.py` & `aws-parallelcluster-node-3.7.0b1/src/common/schedulers/slurm_commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 #
 # http://aws.amazon.com/apache2.0/
 #
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 
+import json
 import logging
 import os
 import re
 from datetime import datetime, timezone
-from typing import List
+from typing import Dict, List
 
 from common.utils import check_command_output, grouper, run_command, validate_subprocess_argument
 from retrying import retry
 from slurm_plugin.slurm_resources import (
     DynamicNode,
     InvalidNodenameError,
     PartitionStatus,
@@ -51,14 +52,15 @@
     "tres-per-job",
     "tres-per-task",
     "tres-per-node",
     "cpus-per-tres",
 ]
 SQUEUE_FIELD_STRING = ",".join([field + ":{size}" for field in _SQUEUE_FIELDS]).format(size=SQUEUE_FIELD_SIZE)
 SLURM_BINARIES_DIR = os.environ.get("SLURM_BINARIES_DIR", "/opt/slurm/bin")
+SLURM_CONF_DIR = os.path.join(os.path.split(SLURM_BINARIES_DIR)[0], "etc")
 SCONTROL = f"sudo {SLURM_BINARIES_DIR}/scontrol"
 SINFO = f"{SLURM_BINARIES_DIR}/sinfo"
 
 SCONTROL_OUTPUT_AWK_PARSER = (
     'awk \'BEGIN{{RS="\\n\\n" ; ORS="######\\n";}} {{print}}\' | '
     + "grep -oP '^(NodeName=\\S+)|(NodeAddr=\\S+)|(NodeHostName=\\S+)|(?<!Next)(State=\\S+)|"
     + "(Partitions=\\S+)|(SlurmdStartTime=\\S+)|(LastBusyTime=\\S+)|(Reason=.*)|(######)'"
@@ -66,14 +68,56 @@
 
 # Set default timeouts for running different slurm commands.
 # These timeouts might be needed when running on large scale
 DEFAULT_GET_INFO_COMMAND_TIMEOUT = 30
 DEFAULT_UPDATE_COMMAND_TIMEOUT = 60
 
 
+class PartitionNodelistMapping:
+    """
+    Singleton class to represent the partition-nodelist mapping between PC-managed partitions and PC-managed nodes.
+
+    The information contained in this singleton is used to make sure ParallelCluster only handles partitions and nodes
+    it is supposed to manage (via Slurm commands).
+    """
+
+    partition_nodelist_mapping: Dict[str, str]
+    _instance = None
+
+    def __init__(self):
+        self.partition_nodelist_mapping = {}
+
+    def get_partition_nodelist_mapping(self) -> Dict[str, str]:
+        """Retrieve partition-nodelist mapping from JSON file."""
+        if not self.partition_nodelist_mapping:
+            partition_nodelist_json = os.path.join(
+                SLURM_CONF_DIR,
+                "pcluster/parallelcluster_partition_nodelist_mapping.json",
+            )
+            with open(partition_nodelist_json, "r", encoding="utf-8") as file:
+                self.partition_nodelist_mapping = json.load(file)
+        return self.partition_nodelist_mapping
+
+    def get_partitions(self) -> List[str]:
+        """Retrieve partitions from JSON file."""
+        return list(self.get_partition_nodelist_mapping().keys())
+
+    @staticmethod
+    def instance():
+        """Return the singleton PartitionNodelistMapping instance."""
+        if not PartitionNodelistMapping._instance:
+            PartitionNodelistMapping._instance = PartitionNodelistMapping()
+        return PartitionNodelistMapping._instance
+
+    @staticmethod
+    def reset():
+        """Reset the instance to clear all caches."""
+        PartitionNodelistMapping._instance = None
+
+
 def is_static_node(nodename):
     """
     Check if the node is static or dynamic.
 
     Valid NodeName format: {queue_name}-{st/dy}-{instancetype}-{number}
     """
     _, node_type, _ = parse_nodename(nodename)
@@ -148,15 +192,15 @@
     return succeeded_partitions
 
 
 def update_all_partitions(state, reset_node_addrs_hostname):
     """Update partitions to a state and reset nodesaddr/nodehostname if needed."""
     try:
         # Get all nodes from partition as opposed to ignoring power_down nodes
-        partitions = get_partition_info(get_all_nodes=True)
+        partitions = get_partitions_info()
         partition_to_update = []
         for part in partitions:
             if PartitionStatus(part.state) != PartitionStatus(state):
                 log.info("Setting partition %s state from %s to %s", part.name, part.state, state)
                 if reset_node_addrs_hostname:
                     log.info("Resetting partition nodes %s", part.nodenames)
                     set_nodes_power_down(part.nodenames, reason="stopping cluster")
@@ -240,51 +284,79 @@
         # works: scontrol update nodename=c5.2xlarge-[1-2] nodeaddr="some ip","some ip"
         # fails: scontrol update nodename=c5.2xlarge-[1-2] nodeaddr="some ip"
         reset_nodes(nodes, state="resume", reason=reason, raise_on_error=False)
     else:
         update_nodes(nodes=nodes, state="resume", reason=reason, raise_on_error=False)
 
 
-def get_nodes_info(nodes="", command_timeout=DEFAULT_GET_INFO_COMMAND_TIMEOUT):
+def get_nodes_info(nodes: str = "", command_timeout=DEFAULT_GET_INFO_COMMAND_TIMEOUT) -> List[SlurmNode]:
     """
     Retrieve SlurmNode list from slurm nodelist notation.
 
     Sample slurm nodelist notation: queue1-dy-c5_xlarge-[1-3],queue2-st-t2_micro-5.
+    If no nodes argument is provided, this function considers only nodes in partitions managed by ParallelCluster.
+    It is responsibility of the caller to pass a nodes argument with only nodes in partitions managed by
+    ParallelCluster.
+
+    TODO: we can consider building a filter to be used in case a nodes argument is passed, in order to exclude nodes
+     not managed by ParallelCluster.
     """
+    if nodes == "":
+        nodes = _get_all_partition_nodes(",".join(PartitionNodelistMapping.instance().get_partitions()))
+
     # Validation to sanitize the input argument and make it safe to use the function affected by B604
     validate_subprocess_argument(nodes)
 
     # awk is used to replace the \n\n record separator with '######\n'
     # Note: In case the node does not belong to any partition the Partitions field is missing from Slurm output
     show_node_info_command = f"{SCONTROL} show nodes {nodes} | {SCONTROL_OUTPUT_AWK_PARSER}"
     nodeinfo_str = check_command_output(show_node_info_command, timeout=command_timeout, shell=True)  # nosec B604
 
     return _parse_nodes_info(nodeinfo_str)
 
 
-def get_partition_info(command_timeout=DEFAULT_GET_INFO_COMMAND_TIMEOUT, get_all_nodes=True):
-    """Retrieve slurm partition info from scontrol."""
-    show_partition_info_command = f'{SCONTROL} show partitions | grep -oP "^PartitionName=\\K(\\S+)| State=\\K(\\S+)"'
+def get_partitions_info(command_timeout=DEFAULT_GET_INFO_COMMAND_TIMEOUT) -> List[SlurmPartition]:
+    """
+    Retrieve slurm partition info from scontrol.
+
+    This function considers only partitions managed by ParallelCluster.
+    """
+    partitions = list(PartitionNodelistMapping.instance().get_partitions())
+    grep_filter = _get_partition_grep_filter(partitions)
+    show_partition_info_command = (
+        f"{SCONTROL} show partitions -o {grep_filter} " + '| grep -oP "^PartitionName=\\K(\\S+)| State=\\K(\\S+)"'
+    )
     # It's safe to use the function affected by B604 since the command is fully built in this code
     partition_info_str = check_command_output(
         show_partition_info_command, timeout=command_timeout, shell=True  # nosec B604
     )
     partitions_info = _parse_partition_name_and_state(partition_info_str)
     return [
         SlurmPartition(
             partition_name,
-            _get_all_partition_nodes(partition_name) if get_all_nodes else _get_partition_nodes(partition_name),
+            _get_all_partition_nodes(partition_name),
             partition_state,
         )
         for partition_name, partition_state in partitions_info
     ]
 
 
+def _get_partition_grep_filter(partitions: List[str]) -> str:
+    grep_filter = ""
+    if partitions:
+        grep_filter += " | grep"
+        for partition in partitions:
+            grep_filter += f' -e "PartitionName={partition}"'
+    return grep_filter
+
+
 def resume_powering_down_nodes():
     """Resume nodes that are powering_down so that are set in power state right away."""
+    # TODO: This function was added due to Slurm ticket 12915. The bug is not reproducible and the ticket was then
+    #  closed. This operation may now be useless: we need to check this.
     log.info("Resuming powering down nodes.")
     powering_down_nodes = _get_slurm_nodes(states="powering_down")
     update_nodes(nodes=powering_down_nodes, state="resume", raise_on_error=False)
 
 
 def _parse_partition_name_and_state(partition_info):
     """Parse partition name and state from scontrol output."""
@@ -298,41 +370,25 @@
 
     show_all_nodes_command = f"{SINFO} -h -p {partition_name} -o %N"
     return check_command_output(show_all_nodes_command, timeout=command_timeout, shell=True).strip()  # nosec B604
 
 
 def _get_slurm_nodes(states=None, partition_name=None, command_timeout=DEFAULT_GET_INFO_COMMAND_TIMEOUT):
     sinfo_command = f"{SINFO} -h -N -o %N"
-    if partition_name:
-        validate_subprocess_argument(partition_name)
-        sinfo_command += f" -p {partition_name}"
+    partition_name = partition_name or ",".join(PartitionNodelistMapping.instance().get_partitions())
+    validate_subprocess_argument(partition_name)
+    sinfo_command += f" -p {partition_name}"
     if states:
         validate_subprocess_argument(states)
         sinfo_command += f" -t {states}"
     # Every node is print on a separate line
     # It's safe to use the function affected by B604 since the command is fully built in this code
     return check_command_output(sinfo_command, timeout=command_timeout, shell=True).splitlines()  # nosec B604
 
 
-def _get_partition_nodes(partition_name, command_timeout=DEFAULT_GET_INFO_COMMAND_TIMEOUT):
-    """Get up nodes in a parition by querying sinfo, and filtering out power_down nodes."""
-    all_nodes = _get_slurm_nodes(partition_name=partition_name)
-    power_down_nodes = _get_slurm_nodes(partition_name=partition_name, states="power_down,powering_down")
-    down_nodes = _get_slurm_nodes(partition_name=partition_name, states="down")
-    nodes = []
-    for nodename in all_nodes:
-        # Always try to maintain the following nodes:
-        # Static nodes
-        # Any node in down
-        # Any node not in power_saving mode
-        if "-st-" in nodename or nodename in down_nodes or (nodename not in power_down_nodes and nodename != "n/a"):
-            nodes.append(nodename)
-    return ",".join(nodes)
-
-
 def _parse_nodes_info(slurm_node_info: str) -> List[SlurmNode]:
     """Parse slurm node info into SlurmNode objects."""
     # [ec2-user@ip-10-0-0-58 ~]$ /opt/slurm/bin/scontrol show nodes compute-dy-c5xlarge-[1-3],compute-dy-c5xlarge-50001\
     # | awk 'BEGIN{{RS="\n\n" ; ORS="######\n";}} {{print}}' | grep -oP "^(NodeName=\S+)|(NodeAddr=\S+)
     # |(NodeHostName=\S+)|(?<!Next)(State=\S+)|(Partitions=\S+)|(SlurmdStartTime=\S+)|(LastBusyTime=\\S+)|(Reason=.*)\
     # |(######)"
     # NodeName=compute-dy-c5xlarge-1
```

### Comparing `aws-parallelcluster-node-3.6.1/src/common/time_utils.py` & `aws-parallelcluster-node-3.7.0b1/src/common/time_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/src/common/utils.py` & `aws-parallelcluster-node-3.7.0b1/src/common/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # http://aws.amazon.com/apache2.0/
 #
 # or in the "LICENSE.txt" file accompanying this file.
 # This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, express or implied.
 # See the License for the specific language governing permissions and limitations under the License.
 
 import collections
+import contextlib
 import itertools
 import json
 import logging
 import os
 import pwd
 import shlex
 
@@ -316,7 +317,34 @@
     :param path: path to validate
     :raise: Exception if the path is not a valid absolute path
     :return: True if the path is a valid absolute path
     """
     if not os.path.isabs(path):
         raise ValueError(f"The path {path} is not a valid absolute path")
     return True
+
+
+@contextlib.contextmanager
+def setup_logging_filter(logger: logging.Logger, custom_field: str):
+    """Set up a custom logging filter and remove it at the end of the context."""
+
+    class CustomFilter(logging.Filter):
+        def __init__(self, custom_field: str):
+            super().__init__()
+            self.field = custom_field
+            self.value = None
+
+        def set_custom_value(self, custom_value: str):
+            self.value = custom_value
+
+        def filter(self, record: logging.LogRecord) -> bool:
+            if self.value:
+                record.msg = f"{self.field} {self.value} - {record.msg}"
+            return True
+
+    custom_filter = CustomFilter(custom_field)
+    logger.addFilter(custom_filter)
+    try:
+        yield custom_filter
+    finally:
+        # Remove the custom log filter
+        logger.removeFilter(custom_filter)
```

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/__init__.py` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/cluster_event_publisher.py` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/cluster_event_publisher.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/clustermgtd.py` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/clustermgtd.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,30 +23,31 @@
 # A nosec comment is appended to the following line in order to disable the B404 check.
 # In this file the input of the module subprocess is trusted.
 from subprocess import CalledProcessError  # nosec B404
 from typing import Dict, List
 
 from botocore.config import Config
 from common.schedulers.slurm_commands import (
+    PartitionNodelistMapping,
     get_nodes_info,
-    get_partition_info,
+    get_partitions_info,
     reset_nodes,
     set_nodes_down,
     set_nodes_drain,
     set_nodes_power_down,
     update_all_partitions,
     update_partitions,
 )
 from common.time_utils import seconds
 from common.utils import check_command_output, read_json, sleep_remaining_loop_time, time_is_up, wait_remaining_time
 from retrying import retry
 from slurm_plugin.cluster_event_publisher import ClusterEventPublisher
 from slurm_plugin.common import TIMESTAMP_FORMAT, log_exception, print_with_count
 from slurm_plugin.console_logger import ConsoleLogger
-from slurm_plugin.instance_manager import InstanceManager
+from slurm_plugin.instance_manager import InstanceManagerFactory
 from slurm_plugin.slurm_resources import (
     CONFIG_FILE_DIR,
     ComputeResourceFailureEvent,
     DynamicNode,
     EC2InstanceHealthState,
     PartitionStatus,
     SlurmNode,
@@ -376,14 +377,15 @@
         self._current_time = None
         self._config = None
         self._compute_fleet_status_manager = None
         self._instance_manager = None
         self._task_executor = None
         self._console_logger = None
         self._event_publisher = None
+        self._partition_nodelist_mapping_instance = None
         self.set_config(config)
 
     def set_config(self, config: ClustermgtdConfig):
         if self._config != config:
             log.info("Applying new clustermgtd config: %s", config)
 
             # If a new task executor is needed, the old one will be shutdown.
@@ -409,15 +411,15 @@
         if self._task_executor:
             self._task_executor.shutdown()
             self._task_executor = None
 
     @staticmethod
     def _initialize_instance_manager(config):
         """Initialize instance manager class that will be used to launch/terminate/describe instances."""
-        return InstanceManager(
+        return InstanceManagerFactory.get_manager(
             config.region,
             config.cluster_name,
             config.boto3_config,
             table_name=config.dynamodb_table,
             hosted_zone=config.hosted_zone,
             dns_domain=config.dns_domain,
             use_private_hostname=config.use_private_hostname,
@@ -489,14 +491,18 @@
 
         if not self._config.disable_all_cluster_management:
             if self._compute_fleet_status in {
                 None,
                 ComputeFleetStatus.RUNNING,
                 ComputeFleetStatus.PROTECTED,
             }:
+                # Get partition_nodelist_mapping between PC-managed Slurm partitions and PC-managed Slurm nodelists
+                # Initialize PartitionNodelistMapping singleton
+                self._partition_nodelist_mapping_instance = PartitionNodelistMapping.instance()
+
                 # Get node states for nodes in inactive and active partitions
                 # Initialize nodes
                 try:
                     log.info("Retrieving nodes info from the scheduler")
                     nodes = self._get_node_info_with_retry()
                     log.debug("Nodes: %s", nodes)
                     partitions_name_map, compute_resource_nodes_map = self._parse_scheduler_nodes_data(nodes)
@@ -550,16 +556,16 @@
     @staticmethod
     @retry(stop_max_attempt_number=2, wait_fixed=1000)
     def _get_node_info_with_retry(nodes=""):
         return get_nodes_info(nodes)
 
     @staticmethod
     @retry(stop_max_attempt_number=2, wait_fixed=1000)
-    def _get_partition_info_with_retry():
-        return {part.name: part for part in get_partition_info(get_all_nodes=True)}
+    def _get_partitions_info_with_retry() -> Dict[str, SlurmPartition]:
+        return {part.name: part for part in get_partitions_info()}
 
     def _clean_up_inactive_partition(self, partitions):
         """Terminate all other instances associated with nodes in INACTIVE partition directly through EC2."""
         inactive_instance_ids, inactive_nodes = ClusterManager._get_inactive_instances_and_nodes(partitions)
         if inactive_nodes:
             try:
                 log.info("Cleaning up INACTIVE partitions.")
@@ -735,22 +741,22 @@
             ice_compute_resources_and_nodes_map,
         )
 
     def _increase_partitions_protected_failure_count(self, bootstrap_failure_nodes):
         """Keep count of boostrap failures."""
         for node in bootstrap_failure_nodes:
             compute_resource = node.compute_resource_name
-            for p in node.partitions:
-                if p in self._partitions_protected_failure_count_map:
-                    self._partitions_protected_failure_count_map[p][compute_resource] = (
-                        self._partitions_protected_failure_count_map[p].get(compute_resource, 0) + 1
-                    )
-                else:
-                    self._partitions_protected_failure_count_map[p] = {}
-                    self._partitions_protected_failure_count_map[p][compute_resource] = 1
+            queue_name = node.queue_name
+            if queue_name in self._partitions_protected_failure_count_map:
+                self._partitions_protected_failure_count_map[queue_name][compute_resource] = (
+                    self._partitions_protected_failure_count_map[queue_name].get(compute_resource, 0) + 1
+                )
+            else:
+                self._partitions_protected_failure_count_map[queue_name] = {}
+                self._partitions_protected_failure_count_map[queue_name][compute_resource] = 1
 
     @log_exception(log, "maintaining unhealthy dynamic nodes", raise_on_error=False)
     def _handle_unhealthy_dynamic_nodes(self, unhealthy_dynamic_nodes):
         """
         Maintain any unhealthy dynamic node.
 
         Terminate instances backing dynamic nodes.
@@ -823,18 +829,18 @@
 
         if instances_to_terminate:
             log.info("Terminating instances backing unhealthy static nodes")
             self._instance_manager.delete_instances(
                 instances_to_terminate, terminate_batch_size=self._config.terminate_max_batch_size
             )
         log.info("Launching new instances for unhealthy static nodes")
-        self._instance_manager.add_instances_for_nodes(
-            node_list,
-            self._config.launch_max_batch_size,
-            self._config.update_node_address,
+        self._instance_manager.add_instances(
+            node_list=node_list,
+            launch_batch_size=self._config.launch_max_batch_size,
+            update_node_address=self._config.update_node_address,
         )
         # Add launched nodes to list of nodes being replaced, excluding any nodes that failed to launch
         failed_nodes = set().union(*self._instance_manager.failed_nodes.values())
         launched_nodes = set(node_list) - failed_nodes
         self._static_nodes_in_replacement |= launched_nodes
         log.info(
             "After node maintenance, following nodes are currently in replacement: %s",
@@ -1047,30 +1053,22 @@
             health_check_type=health_check_type,
         )
         self._handle_nodes_failing_health_check(nodes_failing_health_check, health_check_type)
 
     @staticmethod
     def _parse_scheduler_nodes_data(nodes):
         try:
-            ignored_nodes = []
             compute_resource_nodes_map = {}
-            partitions_name_map = ClusterManager._get_partition_info_with_retry()
+            partitions_name_map = ClusterManager._get_partitions_info_with_retry()
             log.debug("Partitions: %s", partitions_name_map)
             for node in nodes:
-                if not node.partitions or any(p not in partitions_name_map for p in node.partitions):
-                    # ignore nodes not belonging to any partition
-                    ignored_nodes.append(node)
-                else:
-                    for p in node.partitions:
-                        partitions_name_map[p].slurm_nodes.append(node)
-                    compute_resource_nodes_map.setdefault(node.queue_name, {}).setdefault(
-                        node.compute_resource_name, []
-                    ).append(node)
-            if ignored_nodes:
-                log.warning("Ignoring following nodes because they do not belong to any partition: %s", ignored_nodes)
+                partitions_name_map[node.queue_name].slurm_nodes.append(node)
+                compute_resource_nodes_map.setdefault(node.queue_name, {}).setdefault(
+                    node.compute_resource_name, []
+                ).append(node)
             return partitions_name_map, compute_resource_nodes_map
         except Exception as e:
             log.error("Failed when getting partition/node states from scheduler with exception %s", e)
             raise
 
     @staticmethod
     def _update_slurm_nodes_with_ec2_info(nodes, cluster_instances):
```

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/common.py` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,16 @@
         def wrapper(*args, **kwargs):
             try:
                 return function(*args, **kwargs)
             except catch_exception as e:
                 logger.log(log_level, "Failed when %s with exception %s, message: %s", action_desc, type(e).__name__, e)
                 if raise_on_error:
                     if exception_to_raise:
-                        raise exception_to_raise
+                        # preserve exception message if exception to raise is same of actual exception
+                        raise e if isinstance(e, exception_to_raise) else exception_to_raise
                     else:
                         raise
 
         return wrapper
 
     return _log_exception
```

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/computemgtd.py` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/computemgtd.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/console_logger.py` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/console_logger.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/fleet_manager.py` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/fleet_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 # the License. A copy of the License is located at
 #
 # http://aws.amazon.com/apache2.0/
 #
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
+import contextlib
 import copy
 import logging
 import time
 from abc import ABC, abstractmethod
 
 import boto3
 from botocore.exceptions import ClientError
 from common.ec2_utils import get_private_ip_address
+from common.utils import setup_logging_filter
 
 logger = logging.getLogger(__name__)
 
 
 class EC2Instance:
     def __init__(self, id, private_ip, hostname, launch_time):
         """Initialize slurm node with attributes."""
@@ -150,24 +152,30 @@
     def _evaluate_launch_params(self, count):
         pass
 
     @abstractmethod
     def _launch_instances(self, launch_params):
         pass
 
-    def launch_ec2_instances(self, count):
+    def launch_ec2_instances(self, count, job_id=None):
         """
         Launch EC2 instances.
 
         :raises ClientError in case of failures with Boto3 calls (run_instances, create_fleet, describe_instances)
         :raises FleetManagerException in case of missing required instance type info (e.g. private-ip) after 3 retries.
         """
-        launch_params = self._evaluate_launch_params(count)
-        assigned_nodes = self._launch_instances(launch_params)
-        logger.debug("Launched the following instances: %s", assigned_nodes.get("Instances"))
+        with contextlib.ExitStack() as stack:
+            if job_id:
+                job_id_logging_filter = stack.enter_context(setup_logging_filter(logger, "JobID"))
+                job_id_logging_filter.set_custom_value(job_id)
+
+            launch_params = self._evaluate_launch_params(count)
+            assigned_nodes = self._launch_instances(launch_params)
+            logger.debug("Launched the following instances: %s", assigned_nodes.get("Instances"))
+
         return [EC2Instance.from_describe_instance_data(instance_info) for instance_info in assigned_nodes["Instances"]]
 
 
 class Ec2RunInstancesManager(FleetManager):
     """Manager to create EC2 instances fleet using EC2 run_instances API."""
 
     def __init__(
@@ -370,47 +378,53 @@
 
         :raises ClientError in case of boto3 failure
         :return list of instances with complete information and list of IDs for instances with incomplete information
         """
         instances = []
         partial_instance_ids = instance_ids
 
-        retry = 3
+        retry = 4
+        # Wait for instances to be available in EC2
+        time.sleep(0.1)
         while retry > 0 and partial_instance_ids:
-            # Wait for instances to be available in EC2
-            time.sleep(5)
             complete_instances, partial_instance_ids = self._retrieve_instances_info_from_ec2(partial_instance_ids)
             instances.extend(complete_instances)
             retry = retry - 1
+            if retry > 0:
+                time.sleep(0.3)
 
         return instances, partial_instance_ids
 
     def _retrieve_instances_info_from_ec2(self, instance_ids: list):
         """
         Retrieve instance info from EC2 by Instance Ids and verify to have required info.
 
-        :raises ClientError in case of boto3 failure
         :return list of instances with complete information and list of IDs for instances with incomplete information
         """
         complete_instances = []
         partial_instance_ids = []
 
         if instance_ids:
-            ec2_client = boto3.client("ec2", region_name=self._region, config=self._boto3_config)
-            paginator = ec2_client.get_paginator("describe_instances")
-            response_iterator = paginator.paginate(InstanceIds=instance_ids)
-            filtered_iterator = response_iterator.search("Reservations[].Instances[]")
-
-            for instance_info in filtered_iterator:
-                try:
-                    # Try to build EC2Instance objects using all the required fields
-                    EC2Instance.from_describe_instance_data(instance_info)
-                    complete_instances.append(instance_info)
-                except KeyError:
-                    partial_instance_ids.append(instance_info["InstanceId"])
+            try:
+                ec2_client = boto3.client("ec2", region_name=self._region, config=self._boto3_config)
+                paginator = ec2_client.get_paginator("describe_instances")
+                response_iterator = paginator.paginate(InstanceIds=instance_ids)
+                filtered_iterator = response_iterator.search("Reservations[].Instances[]")
+
+                for instance_info in filtered_iterator:
+                    try:
+                        # Try to build EC2Instance objects using all the required fields
+                        EC2Instance.from_describe_instance_data(instance_info)
+                        complete_instances.append(instance_info)
+                    except KeyError as e:
+                        logger.debug("Unable to retrieve instance info: %s", e)
+                        partial_instance_ids.append(instance_info["InstanceId"])
+            except ClientError as e:
+                logger.debug("Unable to retrieve instance info: %s", e)
+                partial_instance_ids.extend(instance_ids)
 
         return complete_instances, partial_instance_ids
 
 
 def run_instances(region, boto3_config, run_instances_kwargs):
     """
     Check whether to override ec2 run_instances.
```

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/fleet_status_manager.py` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/fleet_status_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from configparser import ConfigParser
 from logging.config import fileConfig
 
 from botocore.config import Config
 from common.schedulers.slurm_commands import resume_powering_down_nodes, update_all_partitions
 from slurm_plugin.clustermgtd import ComputeFleetStatus, ComputeFleetStatusManager
 from slurm_plugin.common import log_exception
-from slurm_plugin.instance_manager import InstanceManager
+from slurm_plugin.instance_manager import InstanceManagerFactory
 from slurm_plugin.slurm_resources import CONFIG_FILE_DIR, PartitionStatus
 
 log = logging.getLogger(__name__)
 
 
 class SlurmFleetManagerConfig:
     DEFAULTS = {
@@ -88,21 +88,23 @@
     elif ComputeFleetStatus.is_start_requested(computefleet_status):
         _start_partitions()
 
 
 def _start_partitions():
     log.info("Setting slurm partitions to UP and resuming nodes...")
     update_all_partitions(PartitionStatus.UP, reset_node_addrs_hostname=False)
+    # TODO: This function was added due to Slurm ticket 12915. The bug is not reproducible and the ticket was then
+    #  closed. This operation may now be useless: we need to check this.
     resume_powering_down_nodes()
 
 
 def _stop_partitions(config):
     log.info("Setting slurm partitions to INACTIVE and terminating all compute nodes...")
     update_all_partitions(PartitionStatus.INACTIVE, reset_node_addrs_hostname=True)
-    instance_manager = InstanceManager(
+    instance_manager = InstanceManagerFactory.get_manager(
         config.region,
         config.cluster_name,
         config.boto3_config,
     )
     instance_manager.terminate_all_compute_nodes(config.terminate_max_batch_size)
```

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/logging/parallelcluster_resume_logging.conf` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/logging/parallelcluster_resume_logging.conf`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/resume.py` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/resume.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,36 +18,39 @@
 from logging.config import fileConfig
 
 from botocore.config import Config
 from common.schedulers.slurm_commands import get_nodes_info, set_nodes_down
 from common.utils import read_json
 from slurm_plugin.cluster_event_publisher import ClusterEventPublisher
 from slurm_plugin.common import is_clustermgtd_heartbeat_valid, print_with_count
-from slurm_plugin.instance_manager import InstanceManager
+from slurm_plugin.instance_manager import InstanceManagerFactory
 from slurm_plugin.slurm_resources import CONFIG_FILE_DIR
 
 log = logging.getLogger(__name__)
 event_logger = log.getChild("events")
 
 
 class SlurmResumeConfig:
     DEFAULTS = {
         "max_retry": 1,
-        "max_batch_size": 500,
+        "launch_max_batch_size": 500,
+        "assign_node_max_batch_size": 500,
+        "terminate_max_batch_size": 1000,
         "update_node_address": True,
         "clustermgtd_timeout": 300,
         "proxy": "NONE",
         "logging_config": os.path.join(os.path.dirname(__file__), "logging", "parallelcluster_resume_logging.conf"),
         "hosted_zone": None,
         "dns_domain": None,
         "use_private_hostname": False,
         "run_instances_overrides": "/opt/slurm/etc/pcluster/run_instances_overrides.json",
         "create_fleet_overrides": "/opt/slurm/etc/pcluster/create_fleet_overrides.json",
         "fleet_config_file": "/etc/parallelcluster/slurm_plugin/fleet-config.json",
         "all_or_nothing_batch": False,
+        "job_level_scaling": True,
     }
 
     def __init__(self, config_file_path):
         self._get_config(config_file_path)
 
     def __repr__(self):
         attrs = ", ".join(["{key}={value}".format(key=key, value=repr(value)) for key, value in self.__dict__.items()])
@@ -70,23 +73,32 @@
         self.hosted_zone = config.get("slurm_resume", "hosted_zone", fallback=self.DEFAULTS.get("hosted_zone"))
         self.dns_domain = config.get("slurm_resume", "dns_domain", fallback=self.DEFAULTS.get("dns_domain"))
         self.use_private_hostname = config.getboolean(
             "slurm_resume", "use_private_hostname", fallback=self.DEFAULTS.get("use_private_hostname")
         )
         self.head_node_private_ip = config.get("slurm_resume", "head_node_private_ip")
         self.head_node_hostname = config.get("slurm_resume", "head_node_hostname")
-        self.max_batch_size = config.getint(
-            "slurm_resume", "max_batch_size", fallback=self.DEFAULTS.get("max_batch_size")
+        self.launch_max_batch_size = config.getint(
+            "slurm_resume", "launch_max_batch_size", fallback=self.DEFAULTS.get("launch_max_batch_size")
+        )
+        self.assign_node_max_batch_size = config.getint(
+            "slurm_resume", "assign_node_max_batch_size", fallback=self.DEFAULTS.get("assign_node_max_batch_size")
+        )
+        self.terminate_max_batch_size = config.getint(
+            "slurm_resume", "terminate_max_batch_size", fallback=self.DEFAULTS.get("terminate_max_batch_size")
         )
         self.update_node_address = config.getboolean(
             "slurm_resume", "update_node_address", fallback=self.DEFAULTS.get("update_node_address")
         )
         self.all_or_nothing_batch = config.getboolean(
             "slurm_resume", "all_or_nothing_batch", fallback=self.DEFAULTS.get("all_or_nothing_batch")
         )
+        self.job_level_scaling = config.getboolean(
+            "slurm_resume", "job_level_scaling", fallback=self.DEFAULTS.get("job_level_scaling")
+        )
         fleet_config_file = config.get(
             "slurm_resume", "fleet_config_file", fallback=self.DEFAULTS.get("fleet_config_file")
         )
         self.fleet_config = read_json(fleet_config_file)
 
         # run_instances_overrides_file and create_fleet_overrides_file contain a json with the following format:
         # {
@@ -144,15 +156,15 @@
     try:
         log.info("Setting following failed nodes into DOWN state: %s", print_with_count(node_list))
         set_nodes_down(node_list, reason=reason)
     except Exception as e:
         log.error("Failed to place nodes %s into down with exception: %s", print_with_count(node_list), e)
 
 
-def _resume(arg_nodes, resume_config):
+def _resume(arg_nodes, resume_config, slurm_resume):
     """Launch new EC2 nodes according to nodes requested by slurm."""
     # Check heartbeat
     current_time = datetime.now(tz=timezone.utc)
     if not is_clustermgtd_heartbeat_valid(
         current_time, resume_config.clustermgtd_timeout, resume_config.clustermgtd_heartbeat_file_path
     ):
         log.error(
@@ -167,31 +179,35 @@
     node_list = []
     node_list_with_status = []
     for node in get_nodes_info(arg_nodes):
         node_list.append(node.name)
         node_list_with_status.append((node.name, node.state_string))
     log.info("Current state of Slurm nodes to resume: %s", node_list_with_status)
 
-    instance_manager = InstanceManager(
-        resume_config.region,
-        resume_config.cluster_name,
-        resume_config.boto3_config,
+    instance_manager = InstanceManagerFactory.get_manager(
+        region=resume_config.region,
+        cluster_name=resume_config.cluster_name,
+        boto3_config=resume_config.boto3_config,
         table_name=resume_config.dynamodb_table,
         hosted_zone=resume_config.hosted_zone,
         dns_domain=resume_config.dns_domain,
         use_private_hostname=resume_config.use_private_hostname,
         head_node_private_ip=resume_config.head_node_private_ip,
         head_node_hostname=resume_config.head_node_hostname,
         fleet_config=resume_config.fleet_config,
         run_instances_overrides=resume_config.run_instances_overrides,
         create_fleet_overrides=resume_config.create_fleet_overrides,
+        job_level_scaling=resume_config.job_level_scaling,
     )
-    instance_manager.add_instances_for_nodes(
+    instance_manager.add_instances(
+        slurm_resume=slurm_resume,
         node_list=node_list,
-        launch_batch_size=resume_config.max_batch_size,
+        launch_batch_size=resume_config.launch_max_batch_size,
+        assign_node_batch_size=resume_config.assign_node_max_batch_size,
+        terminate_batch_size=resume_config.terminate_max_batch_size,
         update_node_address=resume_config.update_node_address,
         all_or_nothing_batch=resume_config.all_or_nothing_batch,
     )
     failed_nodes = set().union(*instance_manager.failed_nodes.values())
     success_nodes = [node for node in node_list if node not in failed_nodes]
     log.info("Successfully launched nodes %s", print_with_count(success_nodes))
 
@@ -234,16 +250,24 @@
             log.warning(
                 "Unable to configure logging from %s, using default settings and writing to %s.\nException: %s",
                 resume_config.logging_config,
                 default_log_file,
                 e,
             )
         log.info("ResumeProgram config: %s", resume_config)
-        _resume(args.nodes, resume_config)
+
+        _resume(args.nodes, resume_config, _get_slurm_resume())
         log.info("ResumeProgram finished.")
     except Exception as e:
         log.exception("Encountered exception when requesting instances for %s: %s", args.nodes, e)
         _handle_failed_nodes(args.nodes)
 
 
+def _get_slurm_resume():
+    slurm_resume = read_json(os.environ.get("SLURM_RESUME_FILE"), default={})
+    log_level = logging.INFO if slurm_resume else logging.ERROR
+    log.log(log_level, "Slurm Resume File content: %s", slurm_resume)
+    return slurm_resume
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/slurm_resources.py` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/slurm_resources.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 
 import logging
 import re
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
+from typing import List
 
-from common.utils import time_is_up
+from common.utils import convert_range_to_list, time_is_up
 
 logger = logging.getLogger(__name__)
 
 # Possible ec2 health status: 'ok'|'impaired'|'insufficient-data'|'not-applicable'|'initializing'
 EC2_HEALTH_STATUS_UNHEALTHY_STATES = {"impaired"}
 # Possible instance states: 'pending'|'running'|'shutting-down'|'terminated'|'stopping'|'stopped'
 EC2_INSTANCE_HEALTHY_STATES = {"pending", "running"}
@@ -77,14 +78,96 @@
     def __eq__(self, other):
         """Compare 2 SlurmPartition objects."""
         if isinstance(other, SlurmPartition):
             return self.__dict__ == other.__dict__
         return False
 
 
+class JobOversubscribe(Enum):
+    YES = "YES"
+    NO = "NO"
+    USER = "USER"
+    MCS = "MCS"
+    OK = "OK"
+
+    @classmethod
+    # Default to OK when Oversubscribe value cannot be parsed
+    def _missing_(cls, value):
+        return cls.OK
+
+    def __str__(self):
+        return str(self.value)
+
+
+@dataclass
+class SlurmJob(metaclass=ABCMeta):
+    job_id: int
+
+
+class SlurmResumeJob(SlurmJob):
+    def __init__(
+        self,
+        job_id,
+        nodes_alloc,
+        nodes_resume,
+        oversubscribe,
+        partition="",
+        reservation="",
+        features="",
+        extra="",
+    ):
+        """Initialize Slurm job with attributes."""
+        super().__init__(
+            job_id,
+        )
+
+        self.nodes_alloc = get_node_list(nodes_alloc)
+        self.nodes_resume = get_node_list(nodes_resume)
+        self.oversubscribe = JobOversubscribe(oversubscribe)
+        self.partition = partition
+        self.reservation = reservation
+        self.features = features
+        self.extra = extra
+
+    def is_exclusive(self):
+        return self.oversubscribe == JobOversubscribe.NO
+
+    def __eq__(self, other):
+        """Compare 2 SlurmJob objects."""
+        if isinstance(other, SlurmJob):
+            return self.__dict__ == other.__dict__
+        return False
+
+    def __repr__(self):
+        attrs = ", ".join(["{key}={value}".format(key=key, value=repr(value)) for key, value in self.__dict__.items()])
+        return "{class_name}({attrs})".format(class_name=self.__class__.__name__, attrs=attrs)
+
+    def __str__(self):
+        return f"{self.job_id}"
+
+    def __hash__(self):
+        return hash(self.job_id)
+
+
+@dataclass
+class SlurmResumeData:
+    # List of exclusive job allocated to 1 node each
+    jobs_single_node_no_oversubscribe: List[SlurmResumeJob]
+    # List of exclusive job allocated to more than 1 node each
+    jobs_multi_node_no_oversubscribe: List[SlurmResumeJob]
+    # List of non-exclusive job
+    jobs_oversubscribe: List[SlurmResumeJob]
+    # List of node allocated to single node exclusive job
+    single_node_no_oversubscribe: List[str]
+    # List of node allocated to multiple node exclusive job
+    multi_node_no_oversubscribe: List[str]
+    # List of node allocated to non-exclusive job
+    nodes_oversubscribe: List[str]
+
+
 class SlurmNode(metaclass=ABCMeta):
     SLURM_SCONTROL_COMPLETING_STATE = "COMPLETING"
     SLURM_SCONTROL_BUSY_STATES = {"MIXED", "ALLOCATED", SLURM_SCONTROL_COMPLETING_STATE}
     SLURM_SCONTROL_IDLE_STATE = "IDLE"
     SLURM_SCONTROL_DOWN_STATE = "DOWN"
     SLURM_SCONTROL_DRAIN_STATE = "DRAIN"
     SLURM_SCONTROL_POWERING_DOWN_STATE = "POWERING_DOWN"
@@ -634,7 +717,38 @@
     """Parse queue_name, node_type (st vs dy) and instance_type from nodename."""
     nodename_capture = re.match(r"^([a-z0-9\-]+)-(st|dy)-([a-z0-9\-]+)-\d+$", nodename)
     if not nodename_capture:
         raise InvalidNodenameError
 
     queue_name, node_type, compute_resource_name = nodename_capture.groups()
     return queue_name, node_type, compute_resource_name
+
+
+def get_node_list(nodenames):
+    """
+    Convert nodenames to a list of nodes.
+
+    Example input nodenames: "queue1-st-c5xlarge-[1,3,4-5],queue1-st-c5large-20"
+    Example output [queue1-st-c5xlarge-1, queue1-st-c5xlarge-3, queue1-st-c5xlarge-4, queue1-st-c5xlarge-5,
+    queue1-st-c5large-20]
+    """
+    matches = []
+    if type(nodenames) is str:
+        matches = re.findall(r"((([a-z0-9\-]+)-(st|dy)-([a-z0-9\-]+)-)(\[[\d+,-]+\]|\d+))(,|$)", nodenames)
+        # [('queue1-st-c5xlarge-[1,3,4-5]', 'queue1-st-c5xlarge-', 'queue1', 'st', 'c5xlarge', '[1,3,4-5]'),
+        # ('queue1-st-c5large-20', 'queue1-st-c5large-', 'queue1', 'st', 'c5large', '20')]
+    node_list = []
+    if not matches:
+        raise InvalidNodenameError
+    for match in matches:
+        nodename, prefix, _, _, _, nodes, _ = match
+        if "[" not in nodes:
+            # Single nodename
+            node_list.append(nodename)
+        else:
+            # Multiple nodenames
+            try:
+                node_range = convert_range_to_list(nodes.strip("[]"))
+            except ValueError:
+                raise InvalidNodenameError
+            node_list += [prefix + str(n) for n in node_range]
+    return node_list
```

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/suspend.py` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/suspend.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.1/src/slurm_plugin/task_executor.py` & `aws-parallelcluster-node-3.7.0b1/src/slurm_plugin/task_executor.py`

 * *Files identical despite different names*

