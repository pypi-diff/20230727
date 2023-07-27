# Comparing `tmp/aws_obp_1-0.0.2.tar.gz` & `tmp/aws_obp_1-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_obp_1-0.0.2.tar", last modified: Mon Feb 13 13:47:01 2023, max compression
+gzip compressed data, was "aws_obp_1-0.0.3.tar", last modified: Thu Jul 27 17:04:01 2023, max compression
```

## Comparing `aws_obp_1-0.0.2.tar` & `aws_obp_1-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 13:47:01.550187 aws_obp_1-0.0.2/
--rw-rw-rw-   0        0        0      368 2023-02-13 13:47:01.544847 aws_obp_1-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 05:16:17.000000 aws_obp_1-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-13 13:47:01.514477 aws_obp_1-0.0.2/aws_obp_1/
--rw-rw-rw-   0        0        0     5907 2023-02-13 12:50:32.000000 aws_obp_1-0.0.2/aws_obp_1/__init__.py
--rw-rw-rw-   0        0        0     6203 2023-02-08 05:28:25.000000 aws_obp_1-0.0.2/aws_obp_1/auto_scaling.py
--rw-rw-rw-   0        0        0     5991 2023-02-06 12:39:33.000000 aws_obp_1-0.0.2/aws_obp_1/ec2.py
--rw-rw-rw-   0        0        0     2478 2023-02-06 11:39:53.000000 aws_obp_1-0.0.2/aws_obp_1/lambda_fn.py
--rw-rw-rw-   0        0        0    13805 2023-02-13 13:45:26.000000 aws_obp_1-0.0.2/aws_obp_1/lb.py
--rw-rw-rw-   0        0        0     1831 2023-02-03 13:02:14.000000 aws_obp_1-0.0.2/aws_obp_1/rds.py
--rw-rw-rw-   0        0        0     4461 2023-02-06 11:00:44.000000 aws_obp_1-0.0.2/aws_obp_1/s3.py
--rw-rw-rw-   0        0        0     8969 2023-02-13 05:50:37.000000 aws_obp_1-0.0.2/aws_obp_1/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-13 13:47:01.538151 aws_obp_1-0.0.2/aws_obp_1.egg-info/
--rw-rw-rw-   0        0        0      368 2023-02-13 13:47:01.000000 aws_obp_1-0.0.2/aws_obp_1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-02-13 13:47:01.000000 aws_obp_1-0.0.2/aws_obp_1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 13:47:01.000000 aws_obp_1-0.0.2/aws_obp_1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-02-13 13:47:01.000000 aws_obp_1-0.0.2/aws_obp_1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      549 2023-02-13 13:46:23.000000 aws_obp_1-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-13 13:47:01.550187 aws_obp_1-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 17:04:01.818030 aws_obp_1-0.0.3/
+-rw-rw-rw-   0        0        0      368 2023-07-27 17:04:01.817031 aws_obp_1-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 05:16:17.000000 aws_obp_1-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 17:04:01.804845 aws_obp_1-0.0.3/aws_obp_1/
+-rw-rw-rw-   0        0        0     6263 2023-07-27 16:59:10.000000 aws_obp_1-0.0.3/aws_obp_1/__init__.py
+-rw-rw-rw-   0        0        0     6203 2023-03-24 12:23:56.000000 aws_obp_1-0.0.3/aws_obp_1/auto_scaling.py
+-rw-rw-rw-   0        0        0     5991 2023-03-24 12:23:56.000000 aws_obp_1-0.0.3/aws_obp_1/ec2.py
+-rw-rw-rw-   0        0        0     2478 2023-03-24 12:23:56.000000 aws_obp_1-0.0.3/aws_obp_1/lambda_fn.py
+-rw-rw-rw-   0        0        0    13805 2023-03-24 12:23:56.000000 aws_obp_1-0.0.3/aws_obp_1/lb.py
+-rw-rw-rw-   0        0        0     1831 2023-03-24 12:23:56.000000 aws_obp_1-0.0.3/aws_obp_1/rds.py
+-rw-rw-rw-   0        0        0     4895 2023-07-27 16:59:10.000000 aws_obp_1-0.0.3/aws_obp_1/s3.py
+-rw-rw-rw-   0        0        0     8969 2023-03-24 12:23:56.000000 aws_obp_1-0.0.3/aws_obp_1/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 17:04:01.815030 aws_obp_1-0.0.3/aws_obp_1.egg-info/
+-rw-rw-rw-   0        0        0      368 2023-07-27 17:04:01.000000 aws_obp_1-0.0.3/aws_obp_1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-27 17:04:01.000000 aws_obp_1-0.0.3/aws_obp_1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 17:04:01.000000 aws_obp_1-0.0.3/aws_obp_1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 17:04:01.000000 aws_obp_1-0.0.3/aws_obp_1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      549 2023-07-27 16:59:10.000000 aws_obp_1-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 17:04:01.819030 aws_obp_1-0.0.3/setup.cfg
```

### Comparing `aws_obp_1-0.0.2/aws_obp_1/__init__.py` & `aws_obp_1-0.0.3/aws_obp_1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from botocore.exceptions import ClientError
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Klera DevOps'
-__version__ = '0.0.1'
+__version__ = '0.0.3'
 
 
 class aws_client:
     def __init__(self, **kwargs):
         if 'aws_access_key_id' in kwargs.keys() and 'aws_secret_access_key' in kwargs.keys():
             self.session = session.Session(
                 aws_access_key_id=kwargs['aws_access_key_id'],
@@ -63,16 +63,23 @@
             sg_lst = self.list_security_groups(regions=regions)
         except ClientError as e:
             compliance.append(self.ec2_security_group_attached_to_eni(
                 exception=True, exception_text=e.response['Error']['Code']))
         else:
             compliance.append(self.ec2_security_group_attached_to_eni(eni_lst=eni_lst, sg_lst=sg_lst))
 
-        compliance.append(self.alarm_s3_bucket_policy_change(regions=regions))
-        compliance.append(self.s3_lifecycle_policy_check())
+        try:
+            compliance.append(self.alarm_s3_bucket_policy_change(regions=regions))
+        except ClientError as e:
+            compliance.append(self.alarm_s3_bucket_policy_change(exception=True, exception_text=e.response['Error']['Code']))
+
+        try:
+            compliance.append(self.s3_lifecycle_policy_check())
+        except ClientError as e:
+            compliance.append(self.s3_lifecycle_policy_check(exception=True, exception_text=e.response['Error']['Code']))
 
         try:
             lambda_list = self.list_lambda_functions(regions=regions)
         except ClientError as e:
             compliance.append(self.lambda_function_settings_check(
                 exception=True, exception_text=e.response['Error']['Code']
             ))
```

### Comparing `aws_obp_1-0.0.2/aws_obp_1/auto_scaling.py` & `aws_obp_1-0.0.3/aws_obp_1/auto_scaling.py`

 * *Files identical despite different names*

### Comparing `aws_obp_1-0.0.2/aws_obp_1/ec2.py` & `aws_obp_1-0.0.3/aws_obp_1/ec2.py`

 * *Files identical despite different names*

### Comparing `aws_obp_1-0.0.2/aws_obp_1/lambda_fn.py` & `aws_obp_1-0.0.3/aws_obp_1/lambda_fn.py`

 * *Files identical despite different names*

### Comparing `aws_obp_1-0.0.2/aws_obp_1/lb.py` & `aws_obp_1-0.0.3/aws_obp_1/lb.py`

 * *Files identical despite different names*

### Comparing `aws_obp_1-0.0.2/aws_obp_1/rds.py` & `aws_obp_1-0.0.3/aws_obp_1/rds.py`

 * *Files identical despite different names*

### Comparing `aws_obp_1-0.0.2/aws_obp_1/s3.py` & `aws_obp_1-0.0.3/aws_obp_1/s3.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         'Description': description,
         'Risk Level': risk_level,
         'ControlId': control_id
     }
 
 
 # Checks compliance for s3 lifecycle policy check
-def s3_lifecycle_policy_check(self) -> dict:
+def s3_lifecycle_policy_check(self, **kwargs) -> dict:
     """
     :param self:
     :return:
     """
     logger.info(" ---Inside s3 :: s3_lifecycle_policy_check()--- ")
 
     result = True
@@ -77,14 +77,26 @@
     compliance_type = 'S3 lifecycle policy check'
     description = "Checks if a lifecycle rule is configured for an Amazon Simple Storage Service (Amazon S3) bucket. " \
                   "The rule is NON_COMPLIANT if there is no active lifecycle configuration rules or the " \
                   "configuration does not match with the parameter values."
     resource_type = 'S3'
     risk_level = 'Low'
 
+    if 'exception' in kwargs.keys() and kwargs['exception']:
+        return {
+            'Result': False,
+            'failReason': kwargs['exception_text'],
+            'resource_type': resource_type,
+            'Offenders': offenders,
+            'Compliance_type': compliance_type,
+            'Description': description,
+            'Risk Level': risk_level,
+            'ControlId': control_id
+        }
+
     client = self.session.client('s3')
     buckets_response = client.list_buckets()
 
     for bucket in buckets_response['Buckets']:
         try:
             config_response = client.get_bucket_lifecycle_configuration(
                 Bucket=bucket['Name']
```

### Comparing `aws_obp_1-0.0.2/aws_obp_1/utils.py` & `aws_obp_1-0.0.3/aws_obp_1/utils.py`

 * *Files identical despite different names*

### Comparing `aws_obp_1-0.0.2/pyproject.toml` & `aws_obp_1-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aws_obp_1"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="dheeraj.banodha", email="dheeraj.banodha@impetus.com" },
   { name="ravish.sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
```

