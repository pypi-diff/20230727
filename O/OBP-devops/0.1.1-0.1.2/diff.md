# Comparing `tmp/OBP_devops-0.1.1.tar.gz` & `tmp/OBP_devops-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_devops-0.1.1.tar", last modified: Thu Jul 20 08:24:13 2023, max compression
+gzip compressed data, was "OBP_devops-0.1.2.tar", last modified: Thu Jul 27 17:49:33 2023, max compression
```

## Comparing `OBP_devops-0.1.1.tar` & `OBP_devops-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 08:24:13.863257 OBP_devops-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-07-20 08:24:13.850132 OBP_devops-0.1.1/OBP_devops/
--rw-rw-rw-   0        0        0     7180 2023-07-20 08:22:47.000000 OBP_devops-0.1.1/OBP_devops/__init__.py
--rw-rw-rw-   0        0        0     2600 2023-01-27 06:22:26.000000 OBP_devops-0.1.1/OBP_devops/cloudformation.py
--rw-rw-rw-   0        0        0     9072 2023-01-27 06:22:26.000000 OBP_devops-0.1.1/OBP_devops/codebuild.py
--rw-rw-rw-   0        0        0     2632 2023-05-31 12:31:36.000000 OBP_devops-0.1.1/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py
--rw-rw-rw-   0        0        0     3016 2023-05-31 12:31:35.000000 OBP_devops-0.1.1/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py
--rw-rw-rw-   0        0        0     2480 2023-05-31 12:31:35.000000 OBP_devops-0.1.1/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py
--rw-rw-rw-   0        0        0     2365 2023-01-27 05:16:17.000000 OBP_devops-0.1.1/OBP_devops/codepipeline.py
--rw-rw-rw-   0        0        0     4336 2023-01-27 06:22:27.000000 OBP_devops-0.1.1/OBP_devops/ecr.py
--rw-rw-rw-   0        0        0     1906 2023-05-31 12:31:36.000000 OBP_devops-0.1.1/OBP_devops/ecr_private_tag_immutability_enabled.py
--rw-rw-rw-   0        0        0     1849 2023-05-31 12:31:36.000000 OBP_devops-0.1.1/OBP_devops/ecs_container_insights_enabled.py
--rw-rw-rw-   0        0        0     1926 2023-07-20 07:08:22.000000 OBP_devops-0.1.1/OBP_devops/ecs_containers_non_privileged.py
--rw-rw-rw-   0        0        0     2000 2023-07-20 07:58:07.000000 OBP_devops-0.1.1/OBP_devops/ecs_containers_read_only_access.py
--rw-rw-rw-   0        0        0     2058 2023-05-31 12:31:35.000000 OBP_devops-0.1.1/OBP_devops/ecs_fargate_latest_platform_version.py
--rw-rw-rw-   0        0        0     1951 2023-07-20 07:58:07.000000 OBP_devops-0.1.1/OBP_devops/ecs_task_definition_memory_hard_limit.py
--rw-rw-rw-   0        0        0     2060 2023-07-20 07:58:07.000000 OBP_devops-0.1.1/OBP_devops/ecs_task_definition_nonroot_user.py
--rw-rw-rw-   0        0        0     1957 2023-07-20 07:58:07.000000 OBP_devops-0.1.1/OBP_devops/ecs_task_definition_pid_mode_check.py
--rw-rw-rw-   0        0        0     2156 2023-07-20 07:58:07.000000 OBP_devops-0.1.1/OBP_devops/ecs_task_definition_user_for_host_mode_check.py
--rw-rw-rw-   0        0        0     4711 2023-01-27 06:22:27.000000 OBP_devops-0.1.1/OBP_devops/eks.py
--rw-rw-rw-   0        0        0     3326 2023-01-30 07:27:29.000000 OBP_devops-0.1.1/OBP_devops/elastic_beanstalk.py
--rw-rw-rw-   0        0        0     6477 2023-05-31 12:13:47.000000 OBP_devops-0.1.1/OBP_devops/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:24:13.860259 OBP_devops-0.1.1/OBP_devops.egg-info/
--rw-rw-rw-   0        0        0      369 2023-07-20 08:24:13.000000 OBP_devops-0.1.1/OBP_devops.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      976 2023-07-20 08:24:13.000000 OBP_devops-0.1.1/OBP_devops.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 08:24:13.000000 OBP_devops-0.1.1/OBP_devops.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-20 08:24:13.000000 OBP_devops-0.1.1/OBP_devops.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      369 2023-07-20 08:24:13.862258 OBP_devops-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_devops-0.1.1/README.md
--rw-rw-rw-   0        0        0      550 2023-07-20 08:22:47.000000 OBP_devops-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 08:24:13.864257 OBP_devops-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 17:49:33.961032 OBP_devops-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-07-27 17:49:33.940811 OBP_devops-0.1.2/OBP_devops/
+-rw-rw-rw-   0        0        0     7208 2023-07-27 17:49:00.000000 OBP_devops-0.1.2/OBP_devops/__init__.py
+-rw-rw-rw-   0        0        0     2600 2023-01-27 06:22:26.000000 OBP_devops-0.1.2/OBP_devops/cloudformation.py
+-rw-rw-rw-   0        0        0     9072 2023-01-27 06:22:26.000000 OBP_devops-0.1.2/OBP_devops/codebuild.py
+-rw-rw-rw-   0        0        0     2632 2023-05-31 12:31:36.000000 OBP_devops-0.1.2/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py
+-rw-rw-rw-   0        0        0     3016 2023-05-31 12:31:35.000000 OBP_devops-0.1.2/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py
+-rw-rw-rw-   0        0        0     2480 2023-05-31 12:31:35.000000 OBP_devops-0.1.2/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py
+-rw-rw-rw-   0        0        0     2365 2023-01-27 05:16:17.000000 OBP_devops-0.1.2/OBP_devops/codepipeline.py
+-rw-rw-rw-   0        0        0     4336 2023-01-27 06:22:27.000000 OBP_devops-0.1.2/OBP_devops/ecr.py
+-rw-rw-rw-   0        0        0     1906 2023-05-31 12:31:36.000000 OBP_devops-0.1.2/OBP_devops/ecr_private_tag_immutability_enabled.py
+-rw-rw-rw-   0        0        0     1849 2023-05-31 12:31:36.000000 OBP_devops-0.1.2/OBP_devops/ecs_container_insights_enabled.py
+-rw-rw-rw-   0        0        0     1926 2023-07-20 07:08:22.000000 OBP_devops-0.1.2/OBP_devops/ecs_containers_non_privileged.py
+-rw-rw-rw-   0        0        0     2000 2023-07-20 07:58:07.000000 OBP_devops-0.1.2/OBP_devops/ecs_containers_read_only_access.py
+-rw-rw-rw-   0        0        0     2058 2023-05-31 12:31:35.000000 OBP_devops-0.1.2/OBP_devops/ecs_fargate_latest_platform_version.py
+-rw-rw-rw-   0        0        0     1951 2023-07-20 07:58:07.000000 OBP_devops-0.1.2/OBP_devops/ecs_task_definition_memory_hard_limit.py
+-rw-rw-rw-   0        0        0     2060 2023-07-20 07:58:07.000000 OBP_devops-0.1.2/OBP_devops/ecs_task_definition_nonroot_user.py
+-rw-rw-rw-   0        0        0     1957 2023-07-20 07:58:07.000000 OBP_devops-0.1.2/OBP_devops/ecs_task_definition_pid_mode_check.py
+-rw-rw-rw-   0        0        0     2156 2023-07-20 07:58:07.000000 OBP_devops-0.1.2/OBP_devops/ecs_task_definition_user_for_host_mode_check.py
+-rw-rw-rw-   0        0        0     4711 2023-01-27 06:22:27.000000 OBP_devops-0.1.2/OBP_devops/eks.py
+-rw-rw-rw-   0        0        0     3326 2023-01-30 07:27:29.000000 OBP_devops-0.1.2/OBP_devops/elastic_beanstalk.py
+-rw-rw-rw-   0        0        0     6477 2023-05-31 12:13:47.000000 OBP_devops-0.1.2/OBP_devops/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:49:33.955032 OBP_devops-0.1.2/OBP_devops.egg-info/
+-rw-rw-rw-   0        0        0      369 2023-07-27 17:49:33.000000 OBP_devops-0.1.2/OBP_devops.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2023-07-27 17:49:33.000000 OBP_devops-0.1.2/OBP_devops.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 17:49:33.000000 OBP_devops-0.1.2/OBP_devops.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 17:49:33.000000 OBP_devops-0.1.2/OBP_devops.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      369 2023-07-27 17:49:33.960030 OBP_devops-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_devops-0.1.2/README.md
+-rw-rw-rw-   0        0        0      550 2023-07-27 17:49:00.000000 OBP_devops-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 17:49:33.962030 OBP_devops-0.1.2/setup.cfg
```

### Comparing `OBP_devops-0.1.1/OBP_devops/__init__.py` & `OBP_devops-0.1.2/OBP_devops/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from botocore.exceptions import ClientError
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Klera DevOps'
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 
 
 class aws_client:
     def __init__(self, **kwargs):
         if 'aws_access_key_id' in kwargs.keys() and 'aws_secret_access_key' in kwargs.keys():
             self.session = session.Session(
                 aws_access_key_id=kwargs['aws_access_key_id'],
@@ -49,28 +49,28 @@
         regions = self.get_regions()
         eb_envs = self.list_elastic_beanstalk_envs(regions=regions)
         # print("eb envs" + str(eb_envs))
         task_definitions = self.list_task_definitions(regions)
 
         compliance = [
             # self.enhanced_health_reporting_enabled(eb_envs),
-            self.managed_updates_enabled(environments=eb_envs),
-            self.stack_notification_check(regions),
-            self.ecr_private_tag_immutability_enabled(regions),
-            self.ecs_container_insights_enabled(regions),
-            self.ecs_containers_non_privileged(task_definitions),
-            self.ecs_containers_read_only_access(task_definitions),
-            self.ecs_task_definition_nonroot_user(task_definitions),
-            self.ecs_task_definition_pid_mode_check(task_definitions),
-            self.ecs_task_definition_user_for_host_mode_check(task_definitions),
-            self.ecs_task_definition_memory_hard_limit(task_definitions),
-            self.ecs_fargate_latest_platform_version(regions),
-            self.codedeploy_auto_rollback_monitor_enabled(regions),
-            self.codedeploy_ec2_minimum_healthy_hosts_configured(regions),
-            self.codedeploy_lambda_allatonce_traffic_shift_disabled(regions)
+            # self.managed_updates_enabled(environments=eb_envs),
+            # self.stack_notification_check(regions),
+            # self.ecr_private_tag_immutability_enabled(regions),
+            # self.ecs_container_insights_enabled(regions),
+            # self.ecs_containers_non_privileged(task_definitions),
+            # self.ecs_containers_read_only_access(task_definitions),
+            # self.ecs_task_definition_nonroot_user(task_definitions),
+            # self.ecs_task_definition_pid_mode_check(task_definitions),
+            # self.ecs_task_definition_user_for_host_mode_check(task_definitions),
+            # self.ecs_task_definition_memory_hard_limit(task_definitions),
+            # self.ecs_fargate_latest_platform_version(regions),
+            # self.codedeploy_auto_rollback_monitor_enabled(regions),
+            # self.codedeploy_ec2_minimum_healthy_hosts_configured(regions),
+            # self.codedeploy_lambda_allatonce_traffic_shift_disabled(regions)
         ]
 
         # calling the compliance methods for eks
         try:
             eks_clusters = self.list_eks_clusters(regions)
             # print("eks clusters" + str(eks_clusters))
         except ClientError as e:
```

### Comparing `OBP_devops-0.1.1/OBP_devops/cloudformation.py` & `OBP_devops-0.1.2/OBP_devops/cloudformation.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/codebuild.py` & `OBP_devops-0.1.2/OBP_devops/codebuild.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py` & `OBP_devops-0.1.2/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py` & `OBP_devops-0.1.2/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py` & `OBP_devops-0.1.2/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/codepipeline.py` & `OBP_devops-0.1.2/OBP_devops/codepipeline.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/ecr.py` & `OBP_devops-0.1.2/OBP_devops/ecr.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/ecr_private_tag_immutability_enabled.py` & `OBP_devops-0.1.2/OBP_devops/ecr_private_tag_immutability_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/ecs_container_insights_enabled.py` & `OBP_devops-0.1.2/OBP_devops/ecs_container_insights_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/ecs_containers_non_privileged.py` & `OBP_devops-0.1.2/OBP_devops/ecs_containers_non_privileged.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/ecs_containers_read_only_access.py` & `OBP_devops-0.1.2/OBP_devops/ecs_containers_read_only_access.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/ecs_fargate_latest_platform_version.py` & `OBP_devops-0.1.2/OBP_devops/ecs_fargate_latest_platform_version.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/ecs_task_definition_memory_hard_limit.py` & `OBP_devops-0.1.2/OBP_devops/ecs_task_definition_memory_hard_limit.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/ecs_task_definition_nonroot_user.py` & `OBP_devops-0.1.2/OBP_devops/ecs_task_definition_nonroot_user.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/ecs_task_definition_pid_mode_check.py` & `OBP_devops-0.1.2/OBP_devops/ecs_task_definition_pid_mode_check.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/ecs_task_definition_user_for_host_mode_check.py` & `OBP_devops-0.1.2/OBP_devops/ecs_task_definition_user_for_host_mode_check.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/eks.py` & `OBP_devops-0.1.2/OBP_devops/eks.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/elastic_beanstalk.py` & `OBP_devops-0.1.2/OBP_devops/elastic_beanstalk.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops/utils.py` & `OBP_devops-0.1.2/OBP_devops/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/OBP_devops.egg-info/SOURCES.txt` & `OBP_devops-0.1.2/OBP_devops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.1/pyproject.toml` & `OBP_devops-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "OBP_devops"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="dheeraj.banodha", email="dheeraj.banodha@impetus.com" },
   { name="ravish.sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
```

