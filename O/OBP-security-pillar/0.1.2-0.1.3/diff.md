# Comparing `tmp/OBP_security_pillar-0.1.2.tar.gz` & `tmp/OBP_security_pillar-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_security_pillar-0.1.2.tar", last modified: Tue Jul 18 05:06:53 2023, max compression
+gzip compressed data, was "OBP_security_pillar-0.1.3.tar", last modified: Thu Jul 27 16:47:54 2023, max compression
```

## Comparing `OBP_security_pillar-0.1.2.tar` & `OBP_security_pillar-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 05:06:53.018776 OBP_security_pillar-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.802776 OBP_security_pillar-0.1.2/OBP_security_pillar/
--rw-rw-rw-   0        0        0     3955 2023-07-18 05:06:22.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.825774 OBP_security_pillar-0.1.2/OBP_security_pillar/auto_scaling/
--rw-rw-rw-   0        0        0      475 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/auto_scaling/__init__.py
--rw-rw-rw-   0        0        0     2189 2023-01-27 08:23:40.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.840774 OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/
--rw-rw-rw-   0        0        0      724 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/__init__.py
--rw-rw-rw-   0        0        0     2509 2023-01-27 08:24:11.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py
--rw-rw-rw-   0        0        0     3124 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/driver.py
--rw-rw-rw-   0        0        0     1251 2023-01-27 07:29:08.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/compliance.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.855775 OBP_security_pillar-0.1.2/OBP_security_pillar/dynamodb/
--rw-rw-rw-   0        0        0      493 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/dynamodb/__init__.py
--rw-rw-rw-   0        0        0     2863 2023-01-27 08:24:38.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.936776 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/
--rw-rw-rw-   0        0        0     2214 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/Incoming_ssh_disabled.py
--rw-rw-rw-   0        0        0     2852 2023-05-25 10:19:42.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/__init__.py
--rw-rw-rw-   0        0        0     3275 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py
--rw-rw-rw-   0        0        0     1519 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py
--rw-rw-rw-   0        0        0     2105 2023-01-27 07:29:08.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_encrypted_volume.py
--rw-rw-rw-   0        0        0     1540 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_imdsv2_check.py
--rw-rw-rw-   0        0        0     3047 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py
--rw-rw-rw-   0        0        0     1431 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py
--rw-rw-rw-   0        0        0     1519 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_instance_profile_attached.py
--rw-rw-rw-   0        0        0     2088 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_volume_inuse_check.py
--rw-rw-rw-   0        0        0     2223 2023-01-27 08:28:22.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/instance_in_vpc.py
--rw-rw-rw-   0        0        0     2348 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py
--rw-rw-rw-   0        0        0     2793 2023-01-27 08:43:11.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/elb_logging_enabled.py
--rw-rw-rw-   0        0        0     2268 2023-01-27 08:43:27.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/elb_tls_https_listeners_only.py
--rw-rw-rw-   0        0        0     1969 2023-01-27 08:44:03.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/guard_duty_enabled.py
--rw-rw-rw-   0        0        0     2387 2023-01-27 08:44:27.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/lambda_inside_vpc.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.968775 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/
--rw-rw-rw-   0        0        0     2835 2023-05-25 09:38:15.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/__init__.py
--rw-rw-rw-   0        0        0     1554 2023-05-25 09:12:47.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
--rw-rw-rw-   0        0        0     1379 2023-05-25 09:12:47.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_instance_public_access_check.py
--rw-rw-rw-   0        0        0     1392 2023-05-25 09:23:36.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_snapshot_encrypted.py
--rw-rw-rw-   0        0        0     1901 2023-05-25 09:23:36.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py
--rw-rw-rw-   0        0        0     1401 2023-05-25 09:14:26.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_storage_encrypted.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:06:53.011778 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/
--rw-rw-rw-   0        0        0     1706 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/__init__.py
--rw-rw-rw-   0        0        0     1645 2023-07-18 05:06:22.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_logging_enabled.py
--rw-rw-rw-   0        0        0     2145 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py
--rw-rw-rw-   0        0        0     2147 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py
--rw-rw-rw-   0        0        0     1391 2023-05-25 09:38:15.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py
--rw-rw-rw-   0        0        0     2260 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py
--rw-rw-rw-   0        0        0     1954 2023-07-18 05:06:22.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py
--rw-rw-rw-   0        0        0     1817 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_default_encryption_kms.py
--rw-rw-rw-   0        0        0     1761 2023-01-04 11:06:48.000000 OBP_security_pillar-0.1.2/OBP_security_pillar/security_hub_enabled.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:06:52.812791 OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/
--rw-rw-rw-   0        0        0      797 2023-07-18 05:06:52.000000 OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2223 2023-07-18 05:06:52.000000 OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 05:06:52.000000 OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-18 05:06:52.000000 OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      797 2023-07-18 05:06:53.015780 OBP_security_pillar-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 OBP_security_pillar-0.1.2/README.md
--rw-rw-rw-   0        0        0      495 2023-07-18 05:06:22.000000 OBP_security_pillar-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 05:06:53.018776 OBP_security_pillar-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.808684 OBP_security_pillar-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.365058 OBP_security_pillar-0.1.3/OBP_security_pillar/
+-rw-rw-rw-   0        0        0     4065 2023-07-27 16:47:33.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.408467 OBP_security_pillar-0.1.3/OBP_security_pillar/auto_scaling/
+-rw-rw-rw-   0        0        0      475 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/auto_scaling/__init__.py
+-rw-rw-rw-   0        0        0     2189 2023-01-27 08:23:40.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.456988 OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/
+-rw-rw-rw-   0        0        0      724 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/__init__.py
+-rw-rw-rw-   0        0        0     2509 2023-01-27 08:24:11.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py
+-rw-rw-rw-   0        0        0     3124 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/driver.py
+-rw-rw-rw-   0        0        0     1251 2023-01-27 07:29:08.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/compliance.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.483314 OBP_security_pillar-0.1.3/OBP_security_pillar/dynamodb/
+-rw-rw-rw-   0        0        0      493 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0     2863 2023-01-27 08:24:38.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.638033 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/
+-rw-rw-rw-   0        0        0     2214 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/Incoming_ssh_disabled.py
+-rw-rw-rw-   0        0        0     2852 2023-05-25 10:19:42.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/__init__.py
+-rw-rw-rw-   0        0        0     3275 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py
+-rw-rw-rw-   0        0        0     1519 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py
+-rw-rw-rw-   0        0        0     2105 2023-01-27 07:29:08.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_encrypted_volume.py
+-rw-rw-rw-   0        0        0     1540 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_imdsv2_check.py
+-rw-rw-rw-   0        0        0     3047 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py
+-rw-rw-rw-   0        0        0     1431 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py
+-rw-rw-rw-   0        0        0     1519 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_instance_profile_attached.py
+-rw-rw-rw-   0        0        0     2088 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_volume_inuse_check.py
+-rw-rw-rw-   0        0        0     2223 2023-01-27 08:28:22.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/instance_in_vpc.py
+-rw-rw-rw-   0        0        0     2348 2023-05-25 10:01:21.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py
+-rw-rw-rw-   0        0        0     2793 2023-01-27 08:43:11.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/elb_logging_enabled.py
+-rw-rw-rw-   0        0        0     2268 2023-01-27 08:43:27.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/elb_tls_https_listeners_only.py
+-rw-rw-rw-   0        0        0     1969 2023-01-27 08:44:03.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/guard_duty_enabled.py
+-rw-rw-rw-   0        0        0     2387 2023-01-27 08:44:27.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/lambda_inside_vpc.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.709479 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/
+-rw-rw-rw-   0        0        0     2835 2023-05-25 09:38:15.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/__init__.py
+-rw-rw-rw-   0        0        0     1554 2023-05-25 09:12:47.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
+-rw-rw-rw-   0        0        0     1379 2023-05-25 09:12:47.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_instance_public_access_check.py
+-rw-rw-rw-   0        0        0     1392 2023-05-25 09:23:36.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_snapshot_encrypted.py
+-rw-rw-rw-   0        0        0     1901 2023-05-25 09:23:36.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py
+-rw-rw-rw-   0        0        0     1401 2023-05-25 09:14:26.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_storage_encrypted.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.805753 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/
+-rw-rw-rw-   0        0        0     1706 2023-05-25 10:12:07.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/__init__.py
+-rw-rw-rw-   0        0        0     1645 2023-07-18 05:06:22.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_logging_enabled.py
+-rw-rw-rw-   0        0        0     2145 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py
+-rw-rw-rw-   0        0        0     2147 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py
+-rw-rw-rw-   0        0        0     1391 2023-05-25 09:38:15.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py
+-rw-rw-rw-   0        0        0     2260 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py
+-rw-rw-rw-   0        0        0     1954 2023-07-18 05:06:22.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py
+-rw-rw-rw-   0        0        0     1817 2023-05-25 09:33:44.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_default_encryption_kms.py
+-rw-rw-rw-   0        0        0     1761 2023-01-04 11:06:48.000000 OBP_security_pillar-0.1.3/OBP_security_pillar/security_hub_enabled.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:47:54.376236 OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/
+-rw-rw-rw-   0        0        0      797 2023-07-27 16:47:54.000000 OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2223 2023-07-27 16:47:54.000000 OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 16:47:54.000000 OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-27 16:47:54.000000 OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      797 2023-07-27 16:47:54.807685 OBP_security_pillar-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 OBP_security_pillar-0.1.3/README.md
+-rw-rw-rw-   0        0        0      495 2023-07-27 16:47:33.000000 OBP_security_pillar-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-27 16:47:54.808684 OBP_security_pillar-0.1.3/setup.cfg
```

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/__init__.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 __author__ = 'Dheeraj Banodha'
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 
 class aws_client:
     def __init__(self, **kwargs):
         """
         @param str aws_access_key_id: AWS Access Key ID
         @param str aws_secret_access_key: AWS Secret Access Key
@@ -25,14 +25,16 @@
             self.session = session.Session(profile_name=kwargs['profile_name'])
 
     from .rds import rds_compliance, list_rds_instances, list_rds_snapshots
     from .s3 import s3_compliance, list_s3_buckets
     import OBP_security_pillar.s3 as s3
     import OBP_security_pillar.ec2 as ec2
     import OBP_security_pillar.rds as rds
+    import OBP_security_pillar.cloudtrail as cloudtrail
+    import OBP_security_pillar.dynamodb as dynamodb
     from .ec2 import ec2_compliance, list_ec2_instances
     from .auto_scaling import auto_scaling_compliance
     from .cloudtrail import cloudtrail_compliance
     from .dynamodb import dynamodb_compliance
     from .guard_duty_enabled import guard_duty_enabled
     from .lambda_inside_vpc import lambda_inside_vpc
     # from .security_hub_enabled import security_hub_enabled
```

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/__init__.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/cloudtrail/driver.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/cloudtrail/driver.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/compliance.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/compliance.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/Incoming_ssh_disabled.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/Incoming_ssh_disabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/__init__.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_encrypted_volume.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_encrypted_volume.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_imdsv2_check.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_imdsv2_check.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_instance_profile_attached.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_instance_profile_attached.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/ec2_volume_inuse_check.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/ec2_volume_inuse_check.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/instance_in_vpc.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/instance_in_vpc.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/elb_logging_enabled.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/elb_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/elb_tls_https_listeners_only.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/elb_tls_https_listeners_only.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/guard_duty_enabled.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/guard_duty_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/lambda_inside_vpc.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/lambda_inside_vpc.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/rds/__init__.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_instance_public_access_check.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_instance_public_access_check.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_snapshot_encrypted.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_snapshot_encrypted.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/rds/rds_storage_encrypted.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/rds/rds_storage_encrypted.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/__init__.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_logging_enabled.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/s3/s3_default_encryption_kms.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/s3/s3_default_encryption_kms.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar/security_hub_enabled.py` & `OBP_security_pillar-0.1.3/OBP_security_pillar/security_hub_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/PKG-INFO` & `OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OBP-security-pillar
-Version: 0.1.2
+Version: 0.1.3
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `OBP_security_pillar-0.1.2/OBP_security_pillar.egg-info/SOURCES.txt` & `OBP_security_pillar-0.1.3/OBP_security_pillar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.1.2/PKG-INFO` & `OBP_security_pillar-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OBP_security_pillar
-Version: 0.1.2
+Version: 0.1.3
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

