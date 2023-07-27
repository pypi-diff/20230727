# Comparing `tmp/OBP_monitoring_v2-0.0.3.tar.gz` & `tmp/OBP_monitoring_v2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_monitoring_v2-0.0.3.tar", last modified: Tue Jul 18 05:33:45 2023, max compression
+gzip compressed data, was "OBP_monitoring_v2-0.0.4.tar", last modified: Thu Jul 27 17:15:26 2023, max compression
```

## Comparing `OBP_monitoring_v2-0.0.3.tar` & `OBP_monitoring_v2-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 05:33:45.835538 OBP_monitoring_v2-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-07-18 05:33:45.796543 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/
--rw-rw-rw-   0        0        0     1771 2023-07-18 05:31:32.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/__init__.py
--rw-rw-rw-   0        0        0     2112 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/asg_elb_healthcheck_required.py
--rw-rw-rw-   0        0        0     2244 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/ec2_instance_detailed_monitoring_enabled.py
--rw-rw-rw-   0        0        0     1999 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/guard_duty_enabled.py
--rw-rw-rw-   0        0        0     2361 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/lambda_concurrency_check.py
--rw-rw-rw-   0        0        0     1950 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/lambda_dlq_check.py
--rw-rw-rw-   0        0        0     2137 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py
--rw-rw-rw-   0        0        0     1853 2023-07-18 05:31:32.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/s3_event_notifications_enabled.py
--rw-rw-rw-   0        0        0     1627 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:33:45.829548 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2.egg-info/
--rw-rw-rw-   0        0        0      376 2023-07-18 05:33:45.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-07-18 05:33:45.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 05:33:45.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-18 05:33:45.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      376 2023-07-18 05:33:45.834540 OBP_monitoring_v2-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_monitoring_v2-0.0.3/README.md
--rw-rw-rw-   0        0        0      557 2023-07-18 05:32:06.000000 OBP_monitoring_v2-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 05:33:45.836539 OBP_monitoring_v2-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 17:15:26.756410 OBP_monitoring_v2-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-07-27 17:15:26.738415 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/
+-rw-rw-rw-   0        0        0     1782 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/__init__.py
+-rw-rw-rw-   0        0        0     2133 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/asg_elb_healthcheck_required.py
+-rw-rw-rw-   0        0        0     2265 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/ec2_instance_detailed_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     1999 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/guard_duty_enabled.py
+-rw-rw-rw-   0        0        0     2384 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/lambda_concurrency_check.py
+-rw-rw-rw-   0        0        0     1950 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/lambda_dlq_check.py
+-rw-rw-rw-   0        0        0     2158 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     2079 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/s3_event_notifications_enabled.py
+-rw-rw-rw-   0        0        0     1627 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:15:26.752415 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-07-27 17:15:26.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-07-27 17:15:26.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 17:15:26.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-27 17:15:26.000000 OBP_monitoring_v2-0.0.4/OBP_monitoring_v2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      376 2023-07-27 17:15:26.755412 OBP_monitoring_v2-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_monitoring_v2-0.0.4/README.md
+-rw-rw-rw-   0        0        0      557 2023-07-27 17:14:44.000000 OBP_monitoring_v2-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 17:15:26.756410 OBP_monitoring_v2-0.0.4/setup.cfg
```

### Comparing `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/__init__.py` & `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 __author__ = 'Klera DevOps'
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 
 
 class aws_client:
     def __init__(self, **kwargs):
         if 'aws_access_key_id' in kwargs.keys() and 'aws_secret_access_key' in kwargs.keys():
             self.session = session.Session(
                 aws_access_key_id=kwargs['aws_access_key_id'],
@@ -24,19 +24,19 @@
     from .asg_elb_healthcheck_required import asg_elb_healthcheck_required
     from .ec2_instance_detailed_monitoring_enabled import ec2_instance_detailed_monitoring_enabled
     from .guard_duty_enabled import guard_duty_enabled
     from .lambda_dlq_check import lambda_dlq_check
     from .rds_enhanced_monitoring_enabled import rds_enhanced_monitoring_enabled
     from .utils import get_regions
 
-    def get_compliance(self) -> list:
+    def get_compliance(self, regions) -> list:
         """
         :return:
         """
-        regions = self.get_regions()
+        # regions = self.get_regions()
         compliance = [
             self.lambda_concurrency_check(regions),
             self.s3_event_notifications_enabled(),
             self.asg_elb_healthcheck_required(regions),
             self.ec2_instance_detailed_monitoring_enabled(regions),
             self.guard_duty_enabled(regions),
             self.lambda_dlq_check(regions),
```

### Comparing `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/asg_elb_healthcheck_required.py` & `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/asg_elb_healthcheck_required.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 def asg_elb_healthcheck_required(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return dict:
     """
     logger.info(" ---Inside autoscaling :: asg_elb_healthcheck_required()")
 
     result = True
     failReason = ''
```

### Comparing `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/ec2_instance_detailed_monitoring_enabled.py` & `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/ec2_instance_detailed_monitoring_enabled.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # checks compliance.py for ec2 instance detailed monitoring enabled
 def ec2_instance_detailed_monitoring_enabled(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside ec2 :: ec2_instance_detailed_monitoring_enabled")
 
     result = True
     failReason = ''
```

### Comparing `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/guard_duty_enabled.py` & `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/guard_duty_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/lambda_concurrency_check.py` & `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/lambda_concurrency_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # checks the compliance for lambda-inside-vpc
 def lambda_concurrency_check(self, regions) -> dict:
     """
+    :param regions:
     :param self:
     :return:
     """
     logger.info(" ---Inside OBP Monitoring :: lambda_concurrency_check()")
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id3.70'
     compliance_type = "lambda-concurrency-check"
     description = "Checks whether the AWS Lambda function is configured with function-level concurrent execution limit."
     resource_type = "AWS Lambda"
     risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('lambda')
+    # regions = self.session.get_available_regions('lambda')
 
     for region in regions:
         try:
             client = self.session.client('lambda', region_name=region)
             function_lst = list_lambda_functions(client)
 
             for function in function_lst:
```

### Comparing `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/lambda_dlq_check.py` & `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/lambda_dlq_check.py`

 * *Files identical despite different names*

### Comparing `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py` & `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 logger = logging.getLogger()
 
 
 # checks compliance.py for rds automatic minor version enabled
 def rds_enhanced_monitoring_enabled(self, regions) -> dict:
     """
 
+    :param regions:
     :param self:
     :return dict: rds enhanced monitoring enabled compliance.py details
     """
     logger.info(" ---Inside rds :: rds_enhanced_monitoring_enabled()")
 
     result = True
     failReason = ''
```

### Comparing `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/s3_event_notifications_enabled.py` & `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/s3_event_notifications_enabled.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,50 +9,55 @@
 # checks the compliance.py for s3 bucket versioning enabled
 def s3_event_notifications_enabled(self):
     """
 
     :param self:
     :return dict:
     """
-    logger.info(" ---Inside OBP MOnitoring :: s3_event_notificationsenabled()")
+    logger.info(" ---Inside OBP MMonitoring :: s3_event_notificationsenabled()")
 
     result = True
     failReason = ''
     offenders = []
     control_id = 'Id11.1'
     compliance_type = "S3 event notifications enabled"
     description = "Checks if Amazon S3 Events Notifications are enabled on an S3 bucket."
     resource_type = "S3 Buckets"
     risk_level = 'Medium'
 
     client = self.session.client('s3')
-    response = client.list_buckets()
-
-    for bucket in response['Buckets']:
-        bucket_name = bucket['Name']
-
-        try:
-            resp = client.get_bucket_notification_configuration(
-                Bucket=bucket_name,
-            )
-            #print(resp)
-            del resp['ResponseMetadata']
-            notifications_enabled = bool(resp)
-            if notifications_enabled == False:
-                raise KeyError
-            
-        except KeyError:
-            result = False
-            failReason = "Notifications are turned off for S3 buckets."
-            offenders.append(bucket_name)
-            continue
-        except ClientError:
-            result = False
-            failReason = "Access denied for get_bucket_logging api"
-            offenders.append(bucket_name)
+    try:
+        response = client.list_buckets()
+    except ClientError:
+        result = False
+        failReason = "Access denied for list buckets"
+        offenders.append('')
+    else:
+        for bucket in response['Buckets']:
+            bucket_name = bucket['Name']
+
+            try:
+                resp = client.get_bucket_notification_configuration(
+                    Bucket=bucket_name,
+                )
+                #print(resp)
+                del resp['ResponseMetadata']
+                notifications_enabled = bool(resp)
+                if notifications_enabled == False:
+                    raise KeyError
+
+            except KeyError:
+                result = False
+                failReason = "Notifications are turned off for S3 buckets."
+                offenders.append(bucket_name)
+                continue
+            except ClientError:
+                result = False
+                failReason = "Access denied for get_bucket_logging api"
+                offenders.append(bucket_name)
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
```

### Comparing `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/utils.py` & `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2.egg-info/SOURCES.txt` & `OBP_monitoring_v2-0.0.4/OBP_monitoring_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OBP_monitoring_v2-0.0.3/pyproject.toml` & `OBP_monitoring_v2-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "OBP_monitoring_v2"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="dheeraj.banodha", email="dheeraj.banodha@impetus.com" },
   { name="ravish.sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
```

