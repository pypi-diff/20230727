# Comparing `tmp/aws-parallelcluster-3.6.1.tar.gz` & `tmp/aws-parallelcluster-3.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-parallelcluster-3.6.1.tar", last modified: Wed Jul  5 14:14:49 2023, max compression
+gzip compressed data, was "aws-parallelcluster-3.7.0b1.tar", last modified: Thu Jul 27 19:22:53 2023, max compression
```

## Comparing `aws-parallelcluster-3.6.1.tar` & `aws-parallelcluster-3.7.0b1.tar`

### file list

```diff
@@ -1,264 +1,270 @@
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.235465 aws-parallelcluster-3.6.1/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      114 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/MANIFEST.in
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1850 2023-07-05 14:14:49.235465 aws-parallelcluster-3.6.1/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      787 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/README
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       38 2023-07-05 14:14:49.235465 aws-parallelcluster-3.6.1/setup.cfg
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3443 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/setup.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.195465 aws-parallelcluster-3.6.1/src/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.195465 aws-parallelcluster-3.6.1/src/aws_parallelcluster.egg-info/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1850 2023-07-05 14:14:49.000000 aws-parallelcluster-3.6.1/src/aws_parallelcluster.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10677 2023-07-05 14:14:49.000000 aws-parallelcluster-3.6.1/src/aws_parallelcluster.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2023-07-05 14:14:49.000000 aws-parallelcluster-3.6.1/src/aws_parallelcluster.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      147 2023-07-05 14:14:49.000000 aws-parallelcluster-3.6.1/src/aws_parallelcluster.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2023-07-05 14:14:49.000000 aws-parallelcluster-3.6.1/src/aws_parallelcluster.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      641 2023-07-05 14:14:49.000000 aws-parallelcluster-3.6.1/src/aws_parallelcluster.egg-info/requires.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       36 2023-07-05 14:14:49.000000 aws-parallelcluster-3.6.1/src/aws_parallelcluster.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.195465 aws-parallelcluster-3.6.1/src/pcluster/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      559 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.199465 aws-parallelcluster-3.6.1/src/pcluster/api/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.199465 aws-parallelcluster-3.6.1/src/pcluster/api/awslambda/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/awslambda/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2659 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/awslambda/entrypoint.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11252 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/awslambda/serverless_wsgi.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.199465 aws-parallelcluster-3.6.1/src/pcluster/api/controllers/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      548 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/controllers/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4019 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/controllers/cluster_compute_fleet_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4192 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/controllers/cluster_instances_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7167 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/controllers/cluster_logs_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    19236 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/controllers/cluster_operations_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7697 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/controllers/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6289 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/controllers/image_logs_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    15354 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/controllers/image_operations_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4143 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/converters.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1536 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/encoder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5812 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/errors.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7657 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/flask_app.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.211465 aws-parallelcluster-3.6.1/src/pcluster/api/models/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6121 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4682 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/ami_info.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2128 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2428 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/base_model_.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3757 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/build_image_bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3652 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/build_image_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3639 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/build_image_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3369 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/change.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1717 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/cloud_formation_resource_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1775 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/cloud_formation_stack_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2103 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/cluster_configuration_structure.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9207 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/cluster_info_summary.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8637 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/cluster_instance.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2106 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/cluster_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1879 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/cluster_status_filtering_option.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1630 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/compute_fleet_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4053 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/config_validation_message.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2106 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/conflict_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3813 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3875 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/create_cluster_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3751 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/create_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2302 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/delete_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2220 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/delete_image_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3397 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/describe_cluster_instances_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    17460 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/describe_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3802 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/describe_compute_fleet_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    19464 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/describe_image_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4859 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/dryrun_operation_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6209 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/ec2_ami_info.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2185 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/ec2_ami_info_summary.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1488 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/ec2_ami_state.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6566 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/ec2_instance.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2451 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/failure.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3660 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/get_cluster_log_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2791 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/get_cluster_stack_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3618 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/get_image_log_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2759 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/get_image_stack_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1576 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/image_build_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1678 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/image_builder_image_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2053 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/image_configuration_structure.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8609 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/image_info_summary.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1615 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/image_status_filtering_option.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1484 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/instance_state.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2183 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/internal_service_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2161 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/limit_exceeded_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3024 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/list_cluster_log_streams_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3200 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/list_clusters_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2992 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/list_image_log_streams_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3108 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/list_images_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2315 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/list_official_images_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2373 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/log_event.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8592 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/log_stream.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2418 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/metadata.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1348 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/node_type.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2106 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/not_found_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1532 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/requested_compute_fleet_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2656 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/scheduler.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12343 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/stack_event.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2286 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/tag.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2172 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/unauthorized_client_error_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6155 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2594 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/update_cluster_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4944 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/update_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2377 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/update_compute_fleet_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3274 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/update_compute_fleet_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4087 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/update_error.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1394 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/models/validation_level.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.211465 aws-parallelcluster-3.6.1/src/pcluster/api/openapi/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/openapi/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   114697 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/openapi/openapi.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1388 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/typing_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8594 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/api/util.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.215465 aws-parallelcluster-3.6.1/src/pcluster/aws/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5634 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/aws_api.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    15716 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/aws_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5430 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/batch.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7832 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/cfn.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8480 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2234 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/dynamo.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    21619 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/ec2.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3313 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/efs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3795 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/fsx.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1351 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/iam.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      949 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/imagebuilder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      907 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/kms.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5687 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/logs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1801 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/resource_groups.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2097 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/route53.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7491 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/s3.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2656 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/s3_resource.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1067 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/secretsmanager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1003 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/ssm.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      959 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/aws/sts.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.215465 aws-parallelcluster-3.6.1/src/pcluster/cli/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.219465 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4361 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/cluster_logs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      975 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/commands.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5361 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/common.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.219465 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/configure/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/configure/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1486 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/configure/command.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    20483 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/configure/easyconfig.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10146 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/configure/networking.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5959 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/configure/subnet_computation.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8348 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/configure/utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6742 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/dcv_connect.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      896 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/dcv_util.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3571 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/image_logs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3968 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/ssh.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1434 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/commands/version.py
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)    11369 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/entrypoint.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1116 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/exceptions.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3002 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/logger.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4586 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/middleware.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7601 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/cli/model.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.219465 aws-parallelcluster-3.6.1/src/pcluster/config/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/config/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   134628 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/config/cluster_config.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    16981 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/config/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12981 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/config/config_patch.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11611 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/config/imagebuilder_config.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    21758 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/config/update_policy.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11286 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/constants.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2624 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/imagebuilder_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2302 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/launch_template_utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.219465 aws-parallelcluster-3.6.1/src/pcluster/lib/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      963 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/lib/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3558 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/lib/lib.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.223465 aws-parallelcluster-3.6.1/src/pcluster/models/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/models/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    58732 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/models/cluster.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12099 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/models/cluster_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13929 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/models/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12602 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/models/compute_fleet_status_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    35260 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/models/imagebuilder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5037 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/models/imagebuilder_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    16902 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/models/s3_bucket.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.223465 aws-parallelcluster-3.6.1/src/pcluster/networking/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      559 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/networking/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3769 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/networking/vpc_factory.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.195465 aws-parallelcluster-3.6.1/src/pcluster/resources/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.195465 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.223465 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.223465 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/alinux2/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1816 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/alinux2/Dockerfile
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     1139 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/build-docker-images.sh
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      535 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/buildspec.yml
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.223465 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/scripts/
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     1599 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/scripts/entrypoint.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     5466 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     1954 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     2882 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/scripts/mount_efs.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     2457 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)      856 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/upload-docker-images.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.223465 aws-parallelcluster-3.6.1/src/pcluster/resources/compute_node/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10135 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/compute_node/user_data.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.195465 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.223465 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7610 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.227465 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10142 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       96 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/NOTICE
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       81 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2701 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13195 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1842 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3545 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3369 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2763 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.227465 aws-parallelcluster-3.6.1/src/pcluster/resources/head_node/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6348 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/head_node/user_data.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.227465 aws-parallelcluster-3.6.1/src/pcluster/resources/imagebuilder/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1919 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/imagebuilder/custom_script.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10585 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/imagebuilder/parallelcluster.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8732 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12214 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    15874 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7391 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/resources/imagebuilder/update_and_reboot.yaml
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.227465 aws-parallelcluster-3.6.1/src/pcluster/schemas/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/schemas/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    86365 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/schemas/cluster_schema.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10601 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/schemas/common_schema.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7968 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/schemas/imagebuilder_schema.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.231465 aws-parallelcluster-3.6.1/src/pcluster/templates/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/templates/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    38565 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/templates/awsbatch_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5999 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/templates/cdk_artifacts_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3232 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/templates/cdk_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    40959 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/templates/cdk_builder_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    62398 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/templates/cluster_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5807 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/templates/compute_fleet_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    36443 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/templates/cw_dashboard_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    44224 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/templates/imagebuilder_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      682 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/templates/import_cdk.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    17335 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/templates/queues_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13562 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/templates/slurm_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    19351 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.235465 aws-parallelcluster-3.6.1/src/pcluster/validators/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8763 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/awsbatch_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    64949 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/cluster_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5233 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3528 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/database_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7588 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/directory_service_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12873 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/ebs_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    25736 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/ec2_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1212 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/efs_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1202 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/feature_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9186 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/fsx_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4000 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/iam_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2361 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/imagebuilder_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12556 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/instances_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1414 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/kms_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1858 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/monitoring_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9288 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/networking_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6760 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/s3_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7690 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/scheduler_plugin_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5470 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/slurm_settings_validator.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4081 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/tags_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      825 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster/validators/utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-05 14:14:49.235465 aws-parallelcluster-3.6.1/src/pcluster3_config_converter/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster3_config_converter/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    52964 2023-07-05 10:19:11.000000 aws-parallelcluster-3.6.1/src/pcluster3_config_converter/pcluster3_config_converter.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.517386 aws-parallelcluster-3.7.0b1/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      114 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/MANIFEST.in
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1852 2023-07-27 19:22:53.517386 aws-parallelcluster-3.7.0b1/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      787 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/README
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       38 2023-07-27 19:22:53.517386 aws-parallelcluster-3.7.0b1/setup.cfg
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3447 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/setup.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.473386 aws-parallelcluster-3.7.0b1/src/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.473386 aws-parallelcluster-3.7.0b1/src/aws_parallelcluster.egg-info/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1852 2023-07-27 19:22:53.000000 aws-parallelcluster-3.7.0b1/src/aws_parallelcluster.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10868 2023-07-27 19:22:53.000000 aws-parallelcluster-3.7.0b1/src/aws_parallelcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2023-07-27 19:22:53.000000 aws-parallelcluster-3.7.0b1/src/aws_parallelcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      147 2023-07-27 19:22:53.000000 aws-parallelcluster-3.7.0b1/src/aws_parallelcluster.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2023-07-27 19:22:53.000000 aws-parallelcluster-3.7.0b1/src/aws_parallelcluster.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      643 2023-07-27 19:22:53.000000 aws-parallelcluster-3.7.0b1/src/aws_parallelcluster.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       36 2023-07-27 19:22:53.000000 aws-parallelcluster-3.7.0b1/src/aws_parallelcluster.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.473386 aws-parallelcluster-3.7.0b1/src/pcluster/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      559 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.477386 aws-parallelcluster-3.7.0b1/src/pcluster/api/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.477386 aws-parallelcluster-3.7.0b1/src/pcluster/api/awslambda/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/awslambda/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2659 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/awslambda/entrypoint.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11252 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/awslambda/serverless_wsgi.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.477386 aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      548 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4019 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/cluster_compute_fleet_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4326 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/cluster_instances_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7167 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/cluster_logs_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    20246 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/cluster_operations_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7697 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6289 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/image_logs_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    15354 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/image_operations_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4218 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/converters.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1536 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/encoder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5812 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/errors.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7657 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/flask_app.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.489386 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6251 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4682 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/ami_info.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2128 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2428 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/base_model_.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3757 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/build_image_bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3652 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/build_image_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3639 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/build_image_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3369 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/change.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1717 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cloud_formation_resource_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1775 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cloud_formation_stack_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2103 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cluster_configuration_structure.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9207 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cluster_info_summary.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8637 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cluster_instance.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2106 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cluster_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1879 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cluster_status_filtering_option.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1630 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/compute_fleet_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4053 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/config_validation_message.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2106 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/conflict_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3813 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3875 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/create_cluster_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3751 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/create_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2302 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/delete_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2220 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/delete_image_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3397 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/describe_cluster_instances_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    18397 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/describe_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3802 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/describe_compute_fleet_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    19464 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/describe_image_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4859 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/dryrun_operation_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6209 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/ec2_ami_info.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2185 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/ec2_ami_info_summary.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1488 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/ec2_ami_state.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6566 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/ec2_instance.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2451 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/failure.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3660 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/get_cluster_log_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2791 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/get_cluster_stack_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3618 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/get_image_log_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2759 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/get_image_stack_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1576 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/image_build_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1678 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/image_builder_image_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2053 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/image_configuration_structure.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8609 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/image_info_summary.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1615 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/image_status_filtering_option.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1484 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/instance_state.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2183 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/internal_service_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2161 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/limit_exceeded_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3024 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/list_cluster_log_streams_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3200 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/list_clusters_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2992 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/list_image_log_streams_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3108 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/list_images_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2315 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/list_official_images_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2373 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/log_event.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8592 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/log_stream.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5231 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/login_nodes_pool.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1537 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/login_nodes_state.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2418 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/metadata.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1376 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/node_type.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2106 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/not_found_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1532 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/requested_compute_fleet_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2656 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/scheduler.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12343 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/stack_event.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2286 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/tag.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2172 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/unauthorized_client_error_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6155 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2594 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/update_cluster_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4944 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/update_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2377 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/update_compute_fleet_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3274 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/update_compute_fleet_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4087 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/update_error.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1394 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/models/validation_level.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.493386 aws-parallelcluster-3.7.0b1/src/pcluster/api/openapi/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/openapi/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   115718 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/openapi/openapi.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1388 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/typing_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8594 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/api/util.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.497386 aws-parallelcluster-3.7.0b1/src/pcluster/aws/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5845 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/aws_api.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    16065 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/aws_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5430 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/batch.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7832 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/cfn.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8480 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2234 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/dynamo.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    24057 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/ec2.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3313 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/efs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2879 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/elb.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4655 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/fsx.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1351 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/iam.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      949 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/imagebuilder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      907 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/kms.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5687 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/logs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1801 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/resource_groups.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2097 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/route53.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7491 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/s3.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2656 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/s3_resource.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1067 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/secretsmanager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1003 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/ssm.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      959 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/aws/sts.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.497386 aws-parallelcluster-3.7.0b1/src/pcluster/cli/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.497386 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4361 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/cluster_logs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      975 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/commands.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5361 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/common.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.497386 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/configure/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/configure/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1486 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/configure/command.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    20483 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/configure/easyconfig.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10146 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/configure/networking.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5959 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/configure/subnet_computation.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8348 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/configure/utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6742 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/dcv_connect.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      882 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/dcv_util.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3571 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/image_logs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3968 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/ssh.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1434 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/version.py
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)    11369 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/entrypoint.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1116 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/exceptions.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3002 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/logger.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4586 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/middleware.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7601 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/cli/model.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.501386 aws-parallelcluster-3.7.0b1/src/pcluster/config/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/config/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   123363 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/config/cluster_config.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    16981 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/config/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12981 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/config/config_patch.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11611 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/config/imagebuilder_config.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    24176 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/config/update_policy.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11866 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/constants.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2624 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/imagebuilder_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2302 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/launch_template_utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.501386 aws-parallelcluster-3.7.0b1/src/pcluster/lib/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      963 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/lib/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3558 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/lib/lib.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.501386 aws-parallelcluster-3.7.0b1/src/pcluster/models/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/models/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    51319 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/models/cluster.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12259 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/models/cluster_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13929 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/models/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12565 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/models/compute_fleet_status_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    35260 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/models/imagebuilder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5037 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/models/imagebuilder_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6294 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/models/login_nodes_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    16902 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/models/s3_bucket.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.501386 aws-parallelcluster-3.7.0b1/src/pcluster/networking/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      559 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/networking/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3769 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/networking/vpc_factory.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.473386 aws-parallelcluster-3.7.0b1/src/pcluster/resources/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.473386 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.501386 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.505386 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/alinux2/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1816 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/alinux2/Dockerfile
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     1139 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/build-docker-images.sh
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      535 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/buildspec.yml
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.505386 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/scripts/
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     1599 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/scripts/entrypoint.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     5466 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     1954 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     2882 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/scripts/mount_efs.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     2457 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)      856 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/upload-docker-images.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.505386 aws-parallelcluster-3.7.0b1/src/pcluster/resources/compute_node/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11174 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/compute_node/user_data.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.473386 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.505386 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7610 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.505386 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10142 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       96 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/NOTICE
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       81 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2701 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13195 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1842 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3545 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3369 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2763 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.505386 aws-parallelcluster-3.7.0b1/src/pcluster/resources/head_node/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6348 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/head_node/user_data.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.509386 aws-parallelcluster-3.7.0b1/src/pcluster/resources/imagebuilder/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1919 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/imagebuilder/custom_script.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10597 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/imagebuilder/parallelcluster.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8732 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6443 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    16543 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7345 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/imagebuilder/update_and_reboot.yaml
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.509386 aws-parallelcluster-3.7.0b1/src/pcluster/resources/login_node/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9758 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/resources/login_node/user_data.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.509386 aws-parallelcluster-3.7.0b1/src/pcluster/schemas/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/schemas/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    71914 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/schemas/cluster_schema.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10618 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/schemas/common_schema.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8026 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/schemas/imagebuilder_schema.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.509386 aws-parallelcluster-3.7.0b1/src/pcluster/templates/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    38565 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/awsbatch_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5999 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/cdk_artifacts_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3232 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/cdk_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    42294 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/cdk_builder_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    68857 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/cluster_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5807 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/compute_fleet_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    36652 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/cw_dashboard_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    44224 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/imagebuilder_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      682 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/import_cdk.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    16791 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/login_nodes_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    17656 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/queues_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13562 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/templates/slurm_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    19599 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.513386 aws-parallelcluster-3.7.0b1/src/pcluster/validators/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8783 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/awsbatch_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    65875 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/cluster_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5233 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3528 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/database_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7588 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/directory_service_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12873 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/ebs_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    25736 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/ec2_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1212 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/efs_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1202 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/feature_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9186 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/fsx_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4000 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/iam_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2361 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/imagebuilder_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13754 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/instances_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1414 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/kms_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1858 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/monitoring_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9288 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/networking_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6760 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/s3_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7496 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/slurm_settings_validator.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4081 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/tags_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      825 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster/validators/utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2023-07-27 19:22:53.517386 aws-parallelcluster-3.7.0b1/src/pcluster3_config_converter/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster3_config_converter/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    52964 2023-07-27 14:47:07.000000 aws-parallelcluster-3.7.0b1/src/pcluster3_config_converter/pcluster3_config_converter.py
```

### Comparing `aws-parallelcluster-3.6.1/PKG-INFO` & `aws-parallelcluster-3.7.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster
-Version: 3.6.1
+Version: 3.7.0b1
 Summary: AWS ParallelCluster is an AWS supported Open Source cluster management tool to deploy and manage HPC clusters in the AWS cloud.
 Home-page: https://github.com/aws/aws-parallelcluster
 Author: Amazon Web Services
 License: Apache License 2.0
 Project-URL: Changelog, https://github.com/aws/aws-parallelcluster/blob/develop/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/aws/aws-parallelcluster/issues
 Project-URL: Documentation, https://docs.aws.amazon.com/parallelcluster/
```

### Comparing `aws-parallelcluster-3.6.1/README` & `aws-parallelcluster-3.7.0b1/README`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/setup.py` & `aws-parallelcluster-3.7.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 
 def readme():
     """Read the README file and use it as long description."""
     with open(os.path.join(os.path.dirname(__file__), "README"), encoding="utf-8") as f:
         return f.read()
 
 
-VERSION = "3.6.1"
+VERSION = "3.7.0b1"
 CDK_VERSION = "1.164"
 REQUIRES = [
     "setuptools",
     "boto3>=1.16.14",
     "tabulate>=0.8.8,<=0.8.10",
-    "PyYAML~=5.3",
+    "PyYAML==5.3.1",
     "jinja2~=3.0",
     "marshmallow~=3.10",
     "aws-cdk.core~=" + CDK_VERSION,
     "aws-cdk.aws-batch~=" + CDK_VERSION,
     "aws_cdk.aws-cloudwatch~=" + CDK_VERSION,
     "aws-cdk.aws-codebuild~=" + CDK_VERSION,
     "aws-cdk.aws-dynamodb~=" + CDK_VERSION,
```

### Comparing `aws-parallelcluster-3.6.1/src/aws_parallelcluster.egg-info/PKG-INFO` & `aws-parallelcluster-3.7.0b1/src/aws_parallelcluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster
-Version: 3.6.1
+Version: 3.7.0b1
 Summary: AWS ParallelCluster is an AWS supported Open Source cluster management tool to deploy and manage HPC clusters in the AWS cloud.
 Home-page: https://github.com/aws/aws-parallelcluster
 Author: Amazon Web Services
 License: Apache License 2.0
 Project-URL: Changelog, https://github.com/aws/aws-parallelcluster/blob/develop/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/aws/aws-parallelcluster/issues
 Project-URL: Documentation, https://docs.aws.amazon.com/parallelcluster/
```

### Comparing `aws-parallelcluster-3.6.1/src/aws_parallelcluster.egg-info/SOURCES.txt` & `aws-parallelcluster-3.7.0b1/src/aws_parallelcluster.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 src/pcluster/api/models/list_cluster_log_streams_response_content.py
 src/pcluster/api/models/list_clusters_response_content.py
 src/pcluster/api/models/list_image_log_streams_response_content.py
 src/pcluster/api/models/list_images_response_content.py
 src/pcluster/api/models/list_official_images_response_content.py
 src/pcluster/api/models/log_event.py
 src/pcluster/api/models/log_stream.py
+src/pcluster/api/models/login_nodes_pool.py
+src/pcluster/api/models/login_nodes_state.py
 src/pcluster/api/models/metadata.py
 src/pcluster/api/models/node_type.py
 src/pcluster/api/models/not_found_exception_response_content.py
 src/pcluster/api/models/requested_compute_fleet_status.py
 src/pcluster/api/models/scheduler.py
 src/pcluster/api/models/stack_event.py
 src/pcluster/api/models/tag.py
@@ -105,14 +107,15 @@
 src/pcluster/aws/aws_resources.py
 src/pcluster/aws/batch.py
 src/pcluster/aws/cfn.py
 src/pcluster/aws/common.py
 src/pcluster/aws/dynamo.py
 src/pcluster/aws/ec2.py
 src/pcluster/aws/efs.py
+src/pcluster/aws/elb.py
 src/pcluster/aws/fsx.py
 src/pcluster/aws/iam.py
 src/pcluster/aws/imagebuilder.py
 src/pcluster/aws/kms.py
 src/pcluster/aws/logs.py
 src/pcluster/aws/resource_groups.py
 src/pcluster/aws/route53.py
@@ -153,14 +156,15 @@
 src/pcluster/models/__init__.py
 src/pcluster/models/cluster.py
 src/pcluster/models/cluster_resources.py
 src/pcluster/models/common.py
 src/pcluster/models/compute_fleet_status_manager.py
 src/pcluster/models/imagebuilder.py
 src/pcluster/models/imagebuilder_resources.py
+src/pcluster/models/login_nodes_status.py
 src/pcluster/models/s3_bucket.py
 src/pcluster/networking/__init__.py
 src/pcluster/networking/vpc_factory.py
 src/pcluster/resources/batch/docker/build-docker-images.sh
 src/pcluster/resources/batch/docker/buildspec.yml
 src/pcluster/resources/batch/docker/upload-docker-images.sh
 src/pcluster/resources/batch/docker/alinux2/Dockerfile
@@ -184,28 +188,30 @@
 src/pcluster/resources/head_node/user_data.sh
 src/pcluster/resources/imagebuilder/custom_script.yaml
 src/pcluster/resources/imagebuilder/parallelcluster.yaml
 src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml
 src/pcluster/resources/imagebuilder/parallelcluster_test.yaml
 src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml
 src/pcluster/resources/imagebuilder/update_and_reboot.yaml
+src/pcluster/resources/login_node/user_data.sh
 src/pcluster/schemas/__init__.py
 src/pcluster/schemas/cluster_schema.py
 src/pcluster/schemas/common_schema.py
 src/pcluster/schemas/imagebuilder_schema.py
 src/pcluster/templates/__init__.py
 src/pcluster/templates/awsbatch_builder.py
 src/pcluster/templates/cdk_artifacts_manager.py
 src/pcluster/templates/cdk_builder.py
 src/pcluster/templates/cdk_builder_utils.py
 src/pcluster/templates/cluster_stack.py
 src/pcluster/templates/compute_fleet_stack.py
 src/pcluster/templates/cw_dashboard_builder.py
 src/pcluster/templates/imagebuilder_stack.py
 src/pcluster/templates/import_cdk.py
+src/pcluster/templates/login_nodes_stack.py
 src/pcluster/templates/queues_stack.py
 src/pcluster/templates/slurm_builder.py
 src/pcluster/validators/__init__.py
 src/pcluster/validators/awsbatch_validators.py
 src/pcluster/validators/cluster_validators.py
 src/pcluster/validators/common.py
 src/pcluster/validators/database_validators.py
@@ -218,13 +224,12 @@
 src/pcluster/validators/iam_validators.py
 src/pcluster/validators/imagebuilder_validators.py
 src/pcluster/validators/instances_validators.py
 src/pcluster/validators/kms_validators.py
 src/pcluster/validators/monitoring_validators.py
 src/pcluster/validators/networking_validators.py
 src/pcluster/validators/s3_validators.py
-src/pcluster/validators/scheduler_plugin_validators.py
 src/pcluster/validators/slurm_settings_validator.py
 src/pcluster/validators/tags_validators.py
 src/pcluster/validators/utils.py
 src/pcluster3_config_converter/__init__.py
 src/pcluster3_config_converter/pcluster3_config_converter.py
```

### Comparing `aws-parallelcluster-3.6.1/src/aws_parallelcluster.egg-info/requires.txt` & `aws-parallelcluster-3.7.0b1/src/aws_parallelcluster.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 setuptools
 boto3>=1.16.14
 tabulate<=0.8.10,>=0.8.8
-PyYAML~=5.3
+PyYAML==5.3.1
 jinja2~=3.0
 marshmallow~=3.10
 aws-cdk.core~=1.164
 aws-cdk.aws-batch~=1.164
 aws_cdk.aws-cloudwatch~=1.164
 aws-cdk.aws-codebuild~=1.164
 aws-cdk.aws-dynamodb~=1.164
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/awslambda/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/awslambda/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/awslambda/entrypoint.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/awslambda/entrypoint.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/awslambda/serverless_wsgi.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/awslambda/serverless_wsgi.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/controllers/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/controllers/cluster_compute_fleet_controller.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/cluster_compute_fleet_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/controllers/cluster_instances_controller.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/cluster_instances_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,22 +78,25 @@
     cluster = Cluster(cluster_name)
     node_type = api_node_type_to_cluster_node_type(node_type)
     instances, next_token = cluster.describe_instances(
         next_token=next_token, node_type=node_type, queue_name=queue_name
     )
     ec2_instances = []
     for instance in instances:
+        node_type = ApiNodeType.COMPUTENODE
+        if instance.node_type == NodeType.HEAD_NODE.value:
+            node_type = ApiNodeType.HEADNODE
+        elif instance.node_type == NodeType.LOGIN_NODE.value:
+            node_type = ApiNodeType.LOGINNODE
         ec2_instances.append(
             ClusterInstance(
                 instance_id=instance.id,
                 launch_time=to_utc_datetime(instance.launch_time),
                 public_ip_address=instance.public_ip,
                 instance_type=instance.instance_type,
                 state=instance.state,
                 private_ip_address=instance.private_ip,
-                node_type=ApiNodeType.HEADNODE
-                if instance.node_type == NodeType.HEAD_NODE.value
-                else ApiNodeType.COMPUTENODE,
+                node_type=node_type,
                 queue_name=instance.queue_name,
             )
         )
     return DescribeClusterInstancesResponseContent(instances=ec2_instances, next_token=next_token)
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/controllers/cluster_logs_controller.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/cluster_logs_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/controllers/cluster_operations_controller.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/cluster_operations_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     CreateClusterResponseContent,
     DeleteClusterResponseContent,
     DescribeClusterResponseContent,
     EC2Instance,
     Failure,
     InstanceState,
     ListClustersResponseContent,
+    LoginNodesPool,
+    LoginNodesState,
     Scheduler,
     Tag,
     UpdateClusterBadRequestExceptionResponseContent,
     UpdateClusterRequestContent,
     UpdateClusterResponseContent,
     UpdateError,
     ValidationLevel,
@@ -63,14 +65,15 @@
     Cluster,
     ClusterActionError,
     ClusterUpdateError,
     ConfigValidationError,
     NotFoundClusterActionError,
 )
 from pcluster.models.cluster_resources import ClusterStack
+from pcluster.models.login_nodes_status import LoginNodesPoolState
 from pcluster.utils import get_installed_version, to_utc_datetime
 from pcluster.validators.common import FailureLevel
 
 LOGGER = logging.getLogger(__name__)
 
 
 @convert_errors()
@@ -116,15 +119,15 @@
         raise BadRequestException("configuration is required and cannot be empty")
 
     try:
         cluster = Cluster(create_cluster_request_content.cluster_name, cluster_config)
 
         if dryrun:
             ignored_validation_failures = cluster.validate_create_request(
-                get_validator_suppressors(suppress_validators), FailureLevel[validation_failure_level], dry_run=dryrun
+                get_validator_suppressors(suppress_validators), FailureLevel[validation_failure_level]
             )
             validation_messages = validation_results_to_config_validation_errors(ignored_validation_failures)
             raise DryrunOperationException(validation_messages=validation_messages or None)
 
         stack_id, ignored_validation_failures = cluster.create(
             disable_rollback=not rollback_on_failure,
             validator_suppressors=get_validator_suppressors(suppress_validators),
@@ -231,35 +234,56 @@
         cloud_formation_stack_status=cfn_stack.status,
         cluster_name=cluster_name,
         compute_fleet_status=fleet_status.value,
         cloudformation_stack_arn=cfn_stack.id,
         last_updated_time=to_utc_datetime(cfn_stack.last_updated_time),
         region=os.environ.get("AWS_DEFAULT_REGION"),
         cluster_status=cluster_status,
-        scheduler=Scheduler(type=cluster.stack.scheduler, metadata=cluster.get_plugin_metadata()),
+        scheduler=Scheduler(type=cluster.stack.scheduler),
         failures=_get_creation_failures(cluster_status, cfn_stack),
     )
 
     try:
         head_node = cluster.head_node_instance
         response.head_node = EC2Instance(
             instance_id=head_node.id,
             launch_time=to_utc_datetime(head_node.launch_time),
             public_ip_address=head_node.public_ip,
             instance_type=head_node.instance_type,
             state=InstanceState.from_dict(head_node.state),
             private_ip_address=head_node.private_ip,
         )
+        login_nodes = _get_login_nodes(cluster)
+        if login_nodes:
+            response.login_nodes = login_nodes
     except ClusterActionError as e:
-        # This should not be treated as a failure cause head node might not be running in some cases
+        # This should not be treated as a failure cause head node and login node might not be running in some cases.
+        # e.g. when the cluster is in DELETE_IN_PROGRESS
         LOGGER.info(e)
 
     return response
 
 
+def _get_login_nodes(cluster):
+    login_nodes_status = cluster.login_nodes_status
+    if login_nodes_status.get_login_nodes_pool_available():
+        status = LoginNodesState.FAILED
+        if login_nodes_status.get_status() == LoginNodesPoolState.ACTIVE:
+            status = LoginNodesState.ACTIVE
+        elif login_nodes_status.get_status() == LoginNodesPoolState.PENDING:
+            status = LoginNodesState.PENDING
+        login_nodes = LoginNodesPool(status=status)
+        login_nodes.address = login_nodes_status.get_address()
+        login_nodes.scheme = login_nodes_status.get_scheme()
+        login_nodes.healthy_nodes = login_nodes_status.get_healthy_nodes()
+        login_nodes.unhealthy_nodes = login_nodes_status.get_unhealthy_nodes()
+        return login_nodes
+    return None
+
+
 @configure_aws_region()
 @convert_errors()
 def list_clusters(region=None, next_token=None, cluster_status=None):
     """
     Retrieve the list of existing clusters managed by the API. Deleted clusters are not listed by default.
 
     :param region: List clusters deployed to a given AWS Region.
@@ -349,15 +373,14 @@
 
         if dryrun:
             _, changes, ignored_validation_failures = cluster.validate_update_request(
                 target_source_config=cluster_config,
                 force=force_update,
                 validator_suppressors=get_validator_suppressors(suppress_validators),
                 validation_failure_level=FailureLevel[validation_failure_level],
-                dry_run=dryrun,
             )
             change_set, _ = _analyze_changes(changes)
             validation_messages = validation_results_to_config_validation_errors(ignored_validation_failures)
             raise DryrunOperationException(change_set=change_set, validation_messages=validation_messages or None)
 
         changes, ignored_validation_failures = cluster.update(
             target_source_config=cluster_config,
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/controllers/common.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/controllers/image_logs_controller.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/image_logs_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/controllers/image_operations_controller.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/controllers/image_operations_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/converters.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,9 +63,13 @@
                     type=failure.validator_type,
                 )
             )
     return configuration_validation_messages
 
 
 def api_node_type_to_cluster_node_type(node_type: ApiNodeType):
-    mapping = {ApiNodeType.HEADNODE: NodeType.HEAD_NODE, ApiNodeType.COMPUTENODE: NodeType.COMPUTE}
+    mapping = {
+        ApiNodeType.HEADNODE: NodeType.HEAD_NODE,
+        ApiNodeType.COMPUTENODE: NodeType.COMPUTE,
+        ApiNodeType.LOGINNODE: NodeType.LOGIN_NODE,
+    }
     return mapping.get(node_type)
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/encoder.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/encoder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/errors.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/errors.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/flask_app.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/flask_app.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 from pcluster.api.models.list_cluster_log_streams_response_content import ListClusterLogStreamsResponseContent
 from pcluster.api.models.list_clusters_response_content import ListClustersResponseContent
 from pcluster.api.models.list_image_log_streams_response_content import ListImageLogStreamsResponseContent
 from pcluster.api.models.list_images_response_content import ListImagesResponseContent
 from pcluster.api.models.list_official_images_response_content import ListOfficialImagesResponseContent
 from pcluster.api.models.log_event import LogEvent
 from pcluster.api.models.log_stream import LogStream
+from pcluster.api.models.login_nodes_pool import LoginNodesPool
+from pcluster.api.models.login_nodes_state import LoginNodesState
 from pcluster.api.models.metadata import Metadata
 from pcluster.api.models.node_type import NodeType
 from pcluster.api.models.not_found_exception_response_content import NotFoundExceptionResponseContent
 from pcluster.api.models.requested_compute_fleet_status import RequestedComputeFleetStatus
 from pcluster.api.models.scheduler import Scheduler
 from pcluster.api.models.stack_event import StackEvent
 from pcluster.api.models.tag import Tag
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/ami_info.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/ami_info.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/bad_request_exception_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/base_model_.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/build_image_bad_request_exception_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/build_image_bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/build_image_request_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/build_image_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/build_image_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/build_image_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/change.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/change.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/cloud_formation_resource_status.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cloud_formation_resource_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/cloud_formation_stack_status.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cloud_formation_stack_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/cluster_configuration_structure.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cluster_configuration_structure.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/cluster_info_summary.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cluster_info_summary.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/cluster_instance.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cluster_instance.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/cluster_status.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cluster_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/cluster_status_filtering_option.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/cluster_status_filtering_option.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/compute_fleet_status.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/compute_fleet_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/config_validation_message.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/config_validation_message.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/conflict_exception_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/conflict_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/create_cluster_request_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/create_cluster_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/create_cluster_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/create_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/delete_cluster_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/delete_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/delete_image_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/delete_image_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/describe_cluster_instances_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/describe_cluster_instances_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/describe_cluster_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/describe_cluster_response_content.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pcluster.api.models.base_model_ import Model
 from pcluster.api.models.cloud_formation_stack_status import CloudFormationStackStatus
 from pcluster.api.models.cluster_configuration_structure import ClusterConfigurationStructure
 from pcluster.api.models.cluster_status import ClusterStatus
 from pcluster.api.models.compute_fleet_status import ComputeFleetStatus
 from pcluster.api.models.ec2_instance import EC2Instance
 from pcluster.api.models.failure import Failure
+from pcluster.api.models.login_nodes_pool import LoginNodesPool
 from pcluster.api.models.scheduler import Scheduler
 from pcluster.api.models.tag import Tag
 
 
 class DescribeClusterResponseContent(Model):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
@@ -42,14 +43,15 @@
         cluster_name=None,
         compute_fleet_status=None,
         cloudformation_stack_arn=None,
         last_updated_time=None,
         region=None,
         cluster_status=None,
         scheduler=None,
+        login_nodes=None,
         failures=None,
     ):
         """DescribeClusterResponseContent - a model defined in OpenAPI
 
         :param creation_time: The creation_time of this DescribeClusterResponseContent.
         :type creation_time: datetime
         :param head_node: The head_node of this DescribeClusterResponseContent.
@@ -72,14 +74,16 @@
         :type last_updated_time: datetime
         :param region: The region of this DescribeClusterResponseContent.
         :type region: str
         :param cluster_status: The cluster_status of this DescribeClusterResponseContent.
         :type cluster_status: ClusterStatus
         :param scheduler: The scheduler of this DescribeClusterResponseContent.  # noqa: E501
         :type scheduler: Scheduler
+        :param login_nodes: The login_nodes of this DescribeClusterResponseContent.  # noqa: E501
+        :type login_nodes: LoginNodesPool
         :type failures: List[Failure]
         """
         self.openapi_types = {
             "creation_time": datetime,
             "head_node": EC2Instance,
             "version": str,
             "cluster_configuration": ClusterConfigurationStructure,
@@ -88,14 +92,15 @@
             "cluster_name": str,
             "compute_fleet_status": ComputeFleetStatus,
             "cloudformation_stack_arn": str,
             "last_updated_time": datetime,
             "region": str,
             "cluster_status": ClusterStatus,
             "scheduler": Scheduler,
+            "login_nodes": LoginNodesPool,
             "failures": List[Failure],
         }
 
         self.attribute_map = {
             "creation_time": "creationTime",
             "head_node": "headNode",
             "version": "version",
@@ -105,14 +110,15 @@
             "cluster_name": "clusterName",
             "compute_fleet_status": "computeFleetStatus",
             "cloudformation_stack_arn": "cloudformationStackArn",
             "last_updated_time": "lastUpdatedTime",
             "region": "region",
             "cluster_status": "clusterStatus",
             "scheduler": "scheduler",
+            "login_nodes": "loginNodes",
             "failures": "failures",
         }
 
         self._creation_time = creation_time
         self._version = version
         self._cluster_configuration = cluster_configuration
         self._tags = tags
@@ -121,14 +127,15 @@
         self._compute_fleet_status = compute_fleet_status
         self._failures = failures
         self._cloudformation_stack_arn = cloudformation_stack_arn
         self._last_updated_time = last_updated_time
         self._region = region
         self._cluster_status = cluster_status
         self._head_node = head_node
+        self._login_nodes = login_nodes
         self._scheduler = scheduler
 
     @classmethod
     def from_dict(cls, dikt) -> "DescribeClusterResponseContent":
         """Returns the dict as a model
 
         :param dikt: A dict.
@@ -452,14 +459,35 @@
         """
         if cluster_status is None:
             raise ValueError("Invalid value for `cluster_status`, must not be `None`")
 
         self._cluster_status = cluster_status
 
     @property
+    def login_nodes(self):
+        """Gets the login_nodes of this DescribeClusterResponseContent.
+
+
+        :return: The login_nodes of this DescribeClusterResponseContent.
+        :rtype: LoginNodesPool
+        """
+        return self._login_nodes
+
+    @login_nodes.setter
+    def login_nodes(self, login_nodes):
+        """Sets the login_nodes of this DescribeClusterResponseContent.
+
+
+        :param login_nodes: The login_nodes of this DescribeClusterResponseContent.
+        :type login_nodes: LoginNodesPool
+        """
+
+        self._login_nodes = login_nodes
+
+    @property
     def failures(self):
         """Gets the failures of this DescribeClusterResponseContent.
 
         Failures reason and code when the stack is in CREATE_FAILED status.  # noqa: E501
 
         :return: The failures of this DescribeClusterResponseContent.
         :rtype: List[Failure]
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/describe_compute_fleet_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/describe_compute_fleet_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/describe_image_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/describe_image_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/dryrun_operation_exception_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/dryrun_operation_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/ec2_ami_info.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/ec2_ami_info.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/ec2_ami_info_summary.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/ec2_ami_info_summary.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/ec2_ami_state.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/ec2_ami_state.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/ec2_instance.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/ec2_instance.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/failure.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/failure.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/get_cluster_log_events_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/get_cluster_log_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/get_cluster_stack_events_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/get_cluster_stack_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/get_image_log_events_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/get_image_log_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/get_image_stack_events_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/get_image_stack_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/image_build_status.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/image_build_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/image_builder_image_status.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/image_builder_image_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/image_configuration_structure.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/image_configuration_structure.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/image_info_summary.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/image_info_summary.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/image_status_filtering_option.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/image_status_filtering_option.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/instance_state.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/instance_state.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/internal_service_exception_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/internal_service_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/limit_exceeded_exception_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/limit_exceeded_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/list_cluster_log_streams_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/list_cluster_log_streams_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/list_clusters_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/list_clusters_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/list_image_log_streams_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/list_image_log_streams_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/list_images_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/list_images_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/list_official_images_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/list_official_images_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/log_event.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/log_event.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/log_stream.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/log_stream.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/metadata.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/metadata.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/node_type.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/node_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     """
 
     """
     allowed enum values
     """
     HEADNODE = "HeadNode"
     COMPUTENODE = "ComputeNode"
+    LOGINNODE = "LoginNode"
 
     def __init__(self):
         """NodeType - a model defined in OpenAPI"""
         self.openapi_types = {}
 
         self.attribute_map = {}
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/not_found_exception_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/not_found_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/requested_compute_fleet_status.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/requested_compute_fleet_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/scheduler.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/scheduler.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/stack_event.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/stack_event.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/tag.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/tag.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/unauthorized_client_error_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/unauthorized_client_error_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/update_cluster_request_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/update_cluster_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/update_cluster_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/update_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/update_compute_fleet_request_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/update_compute_fleet_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/update_compute_fleet_response_content.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/update_compute_fleet_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/update_error.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/update_error.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/models/validation_level.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/models/validation_level.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/openapi/openapi.yaml` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/openapi/openapi.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 openapi: 3.0.2
 info:
   description: ParallelCluster API
   title: ParallelCluster
-  version: 3.6.1
+  version: 3.7.0
 servers:
 - url: /
 # override: auth is defined the the API GW level
 # security:
 # - aws.auth.sigv4: []
 paths:
   /v3/clusters:
@@ -2345,14 +2345,20 @@
       required:
       - instances
       title: DescribeClusterInstancesResponseContent
       type: object
     DescribeClusterResponseContent:
       example:
         creationTime: 2000-01-23T04:56:07.000+00:00
+        loginNodes:
+          unhealthyNodes: 6
+          address: address
+          scheme: scheme
+          healthyNodes: 0
+          status: null
         version: version
         clusterConfiguration:
           url: url
         tags:
         - value: value
           key: key
         - value: value
@@ -2419,14 +2425,16 @@
           description: Tags associated with the cluster.
           items:
             $ref: '#/components/schemas/Tag'
           title: tags
           type: array
         headNode:
           $ref: '#/components/schemas/EC2Instance'
+        loginNodes:
+          $ref: '#/components/schemas/LoginNodesPool'
         failureReason:
           description: "Reason of the failure when the stack is in CREATE_FAILED,\
             \ UPDATE_FAILED or DELETE_FAILED status."
           title: failureReason
           type: string
       required:
       - cloudFormationStackStatus
@@ -3139,14 +3147,49 @@
       - lastEventTimestamp
       - lastIngestionTime
       - logStreamArn
       - logStreamName
       - uploadSequenceToken
       title: LogStream
       type: object
+    LoginNodesPool:
+      example:
+        unhealthyNodes: 6
+        address: address
+        scheme: scheme
+        healthyNodes: 0
+        status: null
+      properties:
+        status:
+          $ref: '#/components/schemas/LoginNodesState'
+        address:
+          title: address
+          type: string
+        scheme:
+          title: scheme
+          type: string
+        healthyNodes:
+          format: int32
+          title: healthyNodes
+          type: integer
+        unhealthyNodes:
+          format: int32
+          title: unhealthyNodes
+          type: integer
+      required:
+      - status
+      title: LoginNodesPool
+      type: object
+    LoginNodesState:
+      enum:
+      - pending
+      - active
+      - failed
+      title: LoginNodesState
+      type: string
     Metadata:
       example:
         name: name
         version: version
       properties:
         name:
           title: name
@@ -3156,14 +3199,15 @@
           type: string
       title: Metadata
       type: object
     NodeType:
       enum:
       - HeadNode
       - ComputeNode
+      - LoginNode
       title: NodeType
       type: string
     NotFoundExceptionResponseContent:
       description: This exception is thrown when the requested entity is not found.
       properties:
         message:
           title: message
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/typing_utils.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/typing_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/api/util.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/api/util.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/aws_api.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/aws_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import os
 
 from pcluster.aws.batch import BatchClient
 from pcluster.aws.cfn import CfnClient
 from pcluster.aws.dynamo import DynamoResource
 from pcluster.aws.ec2 import Ec2Client
 from pcluster.aws.efs import EfsClient
+from pcluster.aws.elb import ElbClient
 from pcluster.aws.fsx import FSxClient
 from pcluster.aws.iam import IamClient
 from pcluster.aws.imagebuilder import ImageBuilderClient
 from pcluster.aws.kms import KmsClient
 from pcluster.aws.logs import LogsClient
 from pcluster.aws.resource_groups import ResourceGroupsClient
 from pcluster.aws.route53 import Route53Client
@@ -43,14 +44,15 @@
     def __init__(self):
         self.aws_region = os.environ.get("AWS_DEFAULT_REGION")
 
         self._batch = None
         self._cfn = None
         self._ec2 = None
         self._efs = None
+        self._elb = None
         self._fsx = None
         self._dynamodb = None
         self._s3 = None  # pylint: disable=C0103
         self._kms = None
         self._imagebuilder = None
         self._sts = None
         self._s3_resource = None
@@ -87,14 +89,21 @@
     def efs(self):
         """EFS client."""
         if not self._efs:
             self._efs = EfsClient(ec2_client=self.ec2)
         return self._efs
 
     @property
+    def elb(self):
+        """ELB client."""
+        if not self._elb:
+            self._elb = ElbClient()
+        return self._elb
+
+    @property
     def fsx(self):
         """FSX client."""
         if not self._fsx:
             self._fsx = FSxClient()
         return self._fsx
 
     @property
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/aws_resources.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/aws_resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -284,60 +284,71 @@
         return supported_classes
 
     def ec2memory_size_in_mib(self):
         """Return the amount of memory in MiB."""
         return self.instance_type_data.get("MemoryInfo", {}).get("SizeInMiB")
 
 
-class FsxFileSystemInfo:
-    """Data object wrapping the result of a describe_file_systems call."""
+class FsxStorageInfo:
+    """Data object wrapping the result of a describe_file_systems and describe_file_caches call."""
 
-    def __init__(self, file_system_data):
-        self.file_system_data = file_system_data
+    def __init__(self, file_storage_info):
+        self.file_storage_info = file_storage_info
 
     @property
-    def file_system_type(self):
+    def file_storage_type(self):
         """Return the type of FSx file system (LUSTRE, WINDOWS, ONTAP, or OPENZFS). WINDOWS is not supported."""
-        return self.file_system_data.get("FileSystemType")
+        return (
+            self.file_storage_info.get("FileSystemType")
+            if self.file_storage_info.get("FileSystemType")
+            else self.file_storage_info.get("FileCacheType")
+        )
 
     @property
     def mount_name(self):
         """Return MountName of the FSx Lustre file system."""
         return (
-            self.file_system_data.get("LustreConfiguration").get("MountName") if self.file_system_type == LUSTRE else ""
+            self.file_storage_info.get("LustreConfiguration").get("MountName")
+            if self.file_storage_type == LUSTRE
+            else ""
         )
 
     @property
     def dns_name(self):
         """
         Return DNSName of the file system.
 
         Lustre, OpenZFS have DNS name on file systems. Ontap has DNS name on storage virtual machines.
         """
-        return self.file_system_data.get("DNSName") if self.file_system_type in [LUSTRE, OPENZFS] else ""
+        return self.file_storage_info.get("DNSName") if self.file_storage_type in [LUSTRE, OPENZFS] else ""
 
     @property
     def file_system_id(self):
         """Return id of the file system."""
-        return self.file_system_data.get("FileSystemId")
+        return self.file_storage_info.get("FileSystemId")
+
+    @property
+    def file_cache_id(self):
+        """Return id of the file caches."""
+        return self.file_storage_info.get("FileCacheId")
 
     @property
     def vpc_id(self):
         """Return VPC id of the file system."""
-        return self.file_system_data.get("VpcId")
+        return self.file_storage_info.get("VpcId")
 
     @property
     def network_interface_ids(self):
         """Return network interface ids of the file system."""
-        return self.file_system_data.get("NetworkInterfaceIds")
+        return self.file_storage_info.get("NetworkInterfaceIds")
 
     @property
     def subnet_ids(self):
         """Return subnet ids of the file system."""
-        return self.file_system_data.get("SubnetIds")
+        return self.file_storage_info.get("SubnetIds")
 
 
 class ImageInfo:
     """Object to store Ec2 Image information, initialized with the describe_image or describe_images in ec2 client."""
 
     def __init__(self, image_data: dict):
         self._image_data = image_data
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/batch.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/batch.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/cfn.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/cfn.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/common.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/dynamo.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/dynamo.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/ec2.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/ec2.py`

 * *Files 4% similar despite different names*

```diff
@@ -483,7 +483,69 @@
     def run_instances(self, **kwargs):
         """Run instances."""
         try:
             self._client.run_instances(**kwargs)
         except ClientError as e:
             if e.response.get("Error").get("Code") != "DryRunOperation":
                 raise
+
+    @AWSExceptionHandler.handle_client_exception
+    def describe_route_tables(self, filters=None):
+        """
+        Describe EC2 route tables.
+
+        sample output:
+        [
+            {
+                "Associations": [
+                    {
+                        "Main": False,
+                        "RouteTableAssociationId": "rtbassoc-12345678901234567",
+                        "RouteTableId": "rtb-12345678901234567",
+                        "SubnetId": "subnet-12345678901234567",
+                        "AssociationState": {"State": "associated"},
+                    }
+                ],
+                "PropagatingVgws": [],
+                "RouteTableId": "rtb-12345678901234567",
+                "Routes": [
+                    {
+                        "DestinationCidrBlock": "10.0.0.0/16",
+                        "GatewayId": "local",
+                        "Origin": "CreateRouteTable",
+                        "State": "active",
+                    },
+                    {
+                        "DestinationCidrBlock": "0.0.0.0/0",
+                        "GatewayId": "igw-12345678901234567",
+                        "Origin": "CreateRoute",
+                        "State": "active",
+                    },
+                ],
+                "Tags": [
+                    {"Key": "aws:cloudformation:logical-id", "Value": "RouteTablePublic"},
+                    ...
+                ],
+                "VpcId": "vpc-12345678901234567",
+                "OwnerId": "123456789012"
+            }
+        ]
+        :param filters: The filters to apply when describing the route tables.
+        :return: The route tables that match the filters.
+        """
+        kwargs = {"Filters": filters} if filters else {}
+        return list(self._paginate_results(self._client.describe_route_tables, **kwargs))
+
+    @AWSExceptionHandler.handle_client_exception
+    def is_subnet_public(self, subnet_id):
+        """Check if a subnet is public."""
+        route_tables = self.describe_route_tables(filters=[{"Name": "association.subnet-id", "Values": [subnet_id]}])
+        if not route_tables:
+            raise Exception("No route tables found. The subnet configuration may be incorrect.")
+
+        route_table = route_tables[0]
+
+        for route in route_table.get("Routes", []):
+            if "GatewayId" in route and route["GatewayId"].startswith("igw-"):
+                return True
+
+        return False
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/efs.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/efs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/fsx.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/fsx.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 # with the License. A copy of the License is located at
 #
 # http://aws.amazon.com/apache2.0/
 #
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
-from pcluster.aws.aws_resources import FsxFileSystemInfo
+from pcluster.aws.aws_resources import FsxStorageInfo
 from pcluster.aws.common import AWSExceptionHandler, Boto3Client
 
 
 class FSxClient(Boto3Client):
     """S3 Boto3 client."""
 
     def __init__(self):
         super().__init__("fsx")
         self.cache = {}
         self.svm_cache = {}
         self.volume_cache = {}
+        self.fc_cache = {}
 
     @AWSExceptionHandler.handle_client_exception
     def get_file_systems_info(self, fsx_fs_ids):
         """
         Return FSx file systems info.
 
         :param fsx_fs_ids: a list of FSx file system Id
@@ -36,15 +37,15 @@
             if cached_data:
                 result.append(cached_data)
             else:
                 missed_fsx_fs_ids.append(file_system_id)
         if missed_fsx_fs_ids:
             response = list(self._paginate_results(self._client.describe_file_systems, FileSystemIds=missed_fsx_fs_ids))
             for file_system in response:
-                file_system_info = FsxFileSystemInfo(file_system)
+                file_system_info = FsxStorageInfo(file_system)
                 self.cache[file_system_info.file_system_id] = file_system_info
                 result.append(file_system_info)
         return result
 
     @AWSExceptionHandler.handle_client_exception
     def describe_storage_virtual_machines(self, storage_virtual_machine_ids):
         """Describe storage virtual machines."""
@@ -83,7 +84,26 @@
                 result.append(volume)
         return result
 
     @AWSExceptionHandler.handle_client_exception
     def describe_backup(self, backup_id):
         """Describe backup."""
         return self._client.describe_backups(BackupIds=[backup_id]).get("Backups")[0]
+
+    @AWSExceptionHandler.handle_client_exception
+    def describe_file_caches(self, file_cache_ids):
+        """Describe FSx File cache."""
+        result = []
+        missed_file_cache_ids = []
+        for file_cache_id in file_cache_ids:
+            cached_data = self.fc_cache.get(file_cache_id)
+            if cached_data:
+                result.append(cached_data)
+            else:
+                missed_file_cache_ids.append(file_cache_id)
+        if missed_file_cache_ids:
+            response = self._client.describe_file_caches(FileCacheIds=missed_file_cache_ids)["FileCaches"]
+            for file_cache in response:
+                file_cache_info = FsxStorageInfo(file_cache)
+                self.fc_cache[file_cache.get("FileCacheId")] = file_cache_info
+                result.append(file_cache_info)
+        return result
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/iam.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/iam.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/imagebuilder.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/imagebuilder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/kms.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/kms.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/logs.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/logs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/resource_groups.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/resource_groups.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/route53.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/route53.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/s3.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/s3.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/s3_resource.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/s3_resource.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/secretsmanager.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/ssm.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/aws/sts.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/aws/sts.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/cluster_logs.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/cluster_logs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/commands.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/commands.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/common.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/configure/command.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/configure/command.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/configure/easyconfig.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/configure/easyconfig.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/configure/networking.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/configure/networking.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/configure/subnet_computation.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/configure/subnet_computation.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/configure/utils.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/configure/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/dcv_connect.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/dcv_connect.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/dcv_util.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/dcv_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 from pcluster.constants import SUPPORTED_OSES
 
 
 def get_supported_dcv_os(architecture):
     """Return a list of all the operating system supported by DCV."""
     architectures_dict = {
         "x86_64": SUPPORTED_OSES,
-        "arm64": ["ubuntu1804", "alinux2", "centos7", "rhel8"],
+        "arm64": ["alinux2", "centos7", "rhel8"],
     }
     return architectures_dict.get(architecture, [])
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/image_logs.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/image_logs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/ssh.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/ssh.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/commands/version.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/entrypoint.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/exceptions.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/logger.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/logger.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/middleware.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/middleware.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/cli/model.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/cli/model.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/config/cluster_config.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/config/cluster_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,39 +37,28 @@
     DEFAULT_MIN_COUNT,
     DELETE_POLICY,
     DETAILED_MONITORING_ENABLED_DEFAULT,
     EBS_VOLUME_SIZE_DEFAULT,
     EBS_VOLUME_TYPE_DEFAULT,
     EBS_VOLUME_TYPE_DEFAULT_US_ISO,
     EBS_VOLUME_TYPE_IOPS_DEFAULT,
+    FILECACHE,
     LUSTRE,
     MAX_COMPUTE_RESOURCES_PER_QUEUE,
     MAX_EBS_COUNT,
     MAX_EXISTING_STORAGE_COUNT,
     MAX_NEW_STORAGE_COUNT,
     MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER,
     MAX_NUMBER_OF_QUEUES,
     NODE_BOOTSTRAP_TIMEOUT,
     ONTAP,
     OPENZFS,
-    SCHEDULER_PLUGIN_INTERFACE_VERSION,
-    SCHEDULER_PLUGIN_INTERFACE_VERSION_LOW_RANGE,
-    SCHEDULER_PLUGIN_MAX_NUMBER_OF_COMPUTE_RESOURCES,
-    SCHEDULER_PLUGIN_MAX_NUMBER_OF_QUEUES,
-    SUPPORTED_OSES,
     Feature,
 )
-from pcluster.utils import (
-    get_attr,
-    get_installed_version,
-    get_partition,
-    get_resource_name_from_resource_arn,
-    replace_url_parameters,
-    to_snake_case,
-)
+from pcluster.utils import get_partition, get_resource_name_from_resource_arn, to_snake_case
 from pcluster.validators.awsbatch_validators import (
     AwsBatchComputeInstanceTypeValidator,
     AwsBatchComputeResourceSizeValidator,
     AwsBatchFsxValidator,
     AwsBatchInstancesArchitectureCompatibilityValidator,
 )
 from pcluster.validators.cluster_validators import (
@@ -92,14 +81,15 @@
     FsxArchitectureOsValidator,
     HeadNodeImdsValidator,
     HeadNodeLaunchTemplateValidator,
     HostedZoneValidator,
     InstanceArchitectureCompatibilityValidator,
     IntelHpcArchitectureValidator,
     IntelHpcOsValidator,
+    LoginNodesSchedulerValidator,
     ManagedFsxMultiAzValidator,
     MaxCountValidator,
     MixedSecurityGroupOverwriteValidator,
     MultiNetworkInterfacesInstancesValidator,
     NameValidator,
     NumberOfStorageValidator,
     OverlappingMountDirValidator,
@@ -164,15 +154,15 @@
     RoleValidator,
 )
 from pcluster.validators.instances_validators import (
     InstancesAcceleratorsValidator,
     InstancesAllocationStrategyValidator,
     InstancesCPUValidator,
     InstancesEFAValidator,
-    InstancesMemorySchedulingValidator,
+    InstancesMemorySchedulingWarningValidator,
     InstancesNetworkingValidator,
 )
 from pcluster.validators.kms_validators import KmsKeyIdEncryptedValidator, KmsKeyValidator
 from pcluster.validators.monitoring_validators import DetailedMonitoringValidator, LogRotationValidator
 from pcluster.validators.networking_validators import (
     ElasticIpValidator,
     MultiAzPlacementGroupValidator,
@@ -183,29 +173,21 @@
 )
 from pcluster.validators.s3_validators import (
     S3BucketRegionValidator,
     S3BucketUriValidator,
     S3BucketValidator,
     UrlValidator,
 )
-from pcluster.validators.scheduler_plugin_validators import (
-    GrantSudoPrivilegesValidator,
-    PluginInterfaceVersionValidator,
-    SchedulerPluginOsArchitectureValidator,
-    SchedulerPluginRegionValidator,
-    SudoPrivilegesValidator,
-    SupportedVersionsValidator,
-    UserNameValidator,
-)
 from pcluster.validators.slurm_settings_validator import (
     SLURM_SETTINGS_DENY_LIST,
     CustomSlurmNodeNamesValidator,
     CustomSlurmSettingLevel,
     CustomSlurmSettingsIncludeFileOnlyValidator,
     CustomSlurmSettingsValidator,
+    SlurmNodePrioritiesWarningValidator,
 )
 from pcluster.validators.tags_validators import ComputeResourceTagsValidator
 
 LOGGER = logging.getLogger(__name__)
 
 # pylint: disable=C0302
 
@@ -610,14 +592,34 @@
     def existing_dns_name(self):
         """Return DNSName of the SVM of existing FSx filesystem."""
         return AWSApi.instance().fsx.describe_storage_virtual_machines([self.storage_virtual_machine_id])[0][
             "Endpoints"
         ]["Nfs"]["DNSName"]
 
 
+class ExistingFsxFileCache(BaseSharedFsx):
+    """Represent the shared FSX FileCache resource."""
+
+    def __init__(self, file_cache_id: str, **kwargs):
+        super().__init__(**kwargs)
+        self.file_cache_id = file_cache_id
+        self.file_system_id = file_cache_id
+        self.file_system_type = FILECACHE
+
+    @property
+    def existing_dns_name(self):
+        """Return DNSName of the existing FSx File Cache."""
+        return AWSApi.instance().fsx.describe_file_caches([self.file_cache_id])[0].dns_name
+
+    @property
+    def file_cache_mount_name(self):
+        """Return Mount Name of the existing FSx File Cache."""
+        return AWSApi.instance().fsx.describe_file_caches([self.file_cache_id])[0].mount_name
+
+
 # ---------------------- Networking ---------------------- #
 
 
 class Proxy(Resource):
     """Represent the proxy."""
 
     def __init__(self, http_proxy_address: str = None):
@@ -634,14 +636,41 @@
         self.additional_security_groups = Resource.init_param(additional_security_groups)
 
     def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
         self._register_validator(SecurityGroupsValidator, security_group_ids=self.security_groups)
         self._register_validator(SecurityGroupsValidator, security_group_ids=self.additional_security_groups)
 
 
+class SubnetsMixin:
+    """Represent Mixin class for networking functionality."""
+
+    def __init__(self, subnet_ids: List[str], **kwargs):
+        self.subnet_ids = Resource.init_param(subnet_ids)
+        self._az_subnet_ids_mapping = None
+
+    @property
+    def subnet_id_az_mapping(self):
+        """Map subnet ids to availability zones."""
+        return AWSApi.instance().ec2.get_subnets_az_mapping(self.subnet_ids)
+
+    @property
+    def az_subnet_ids_mapping(self):
+        """Map subnet ids to availability zones."""
+        if not self._az_subnet_ids_mapping:
+            self._az_subnet_ids_mapping = defaultdict(set)
+            for subnet_id, _az in self.subnet_id_az_mapping.items():
+                self._az_subnet_ids_mapping[_az].add(subnet_id)
+        return self._az_subnet_ids_mapping
+
+    @property
+    def az_list(self):
+        """Get availability zones list."""
+        return list(self.az_subnet_ids_mapping.keys())
+
+
 class HeadNodeNetworking(_BaseNetworking):
     """Represent the networking configuration for the head node."""
 
     def __init__(self, subnet_id: str, elastic_ip: Union[str, bool] = None, proxy: Proxy = None, **kwargs):
         super().__init__(**kwargs)
         self.subnet_id = Resource.init_param(subnet_id)
         self.elastic_ip = Resource.init_param(elastic_ip)
@@ -694,40 +723,21 @@
     """Represent the networking configuration for the compute resource."""
 
     def __init__(self, placement_group: PlacementGroup = None, **kwargs):
         super().__init__(**kwargs)
         self.placement_group = placement_group or PlacementGroup(implied=True)
 
 
-class _QueueNetworking(_BaseNetworking):
+class _QueueNetworking(_BaseNetworking, SubnetsMixin):
     """Represent the networking configuration for the Queue."""
 
     def __init__(self, subnet_ids: List[str], assign_public_ip: str = None, **kwargs):
-        super().__init__(**kwargs)
+        _BaseNetworking.__init__(self, **kwargs)
+        SubnetsMixin.__init__(self, subnet_ids, **kwargs)
         self.assign_public_ip = Resource.init_param(assign_public_ip)
-        self.subnet_ids = Resource.init_param(subnet_ids)
-        self._az_subnet_ids_mapping = None
-
-    @property
-    def subnet_id_az_mapping(self):
-        """Map queue subnet ids to availability zones."""
-        return AWSApi.instance().ec2.get_subnets_az_mapping(self.subnet_ids)
-
-    @property
-    def az_subnet_ids_mapping(self):
-        """Map queue subnet ids to availability zones."""
-        if not self._az_subnet_ids_mapping:
-            self._az_subnet_ids_mapping = defaultdict(set)
-            for subnet_id, _az in self.subnet_id_az_mapping.items():
-                self._az_subnet_ids_mapping[_az].add(subnet_id)
-        return self._az_subnet_ids_mapping
-
-    @property
-    def az_list(self):
-        return list(self.az_subnet_ids_mapping.keys())
 
 
 class SlurmQueueNetworking(_QueueNetworking):
     """Represent the networking configuration for the slurm Queue."""
 
     def __init__(self, placement_group: PlacementGroup = None, proxy: Proxy = None, **kwargs):
         super().__init__(**kwargs)
@@ -738,32 +748,33 @@
 class AwsBatchQueueNetworking(_QueueNetworking):
     """Represent the networking configuration for the aws batch Queue."""
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 
-class SchedulerPluginQueueNetworking(SlurmQueueNetworking):
-    """Represent the networking configuration for the Scheduler Plugin Queue."""
-
-    pass
-
-
-class Ssh(Resource):
-    """Represent the SSH configuration for a node."""
+class _BaseSsh(Resource):
+    """Represent the base SSH configuration, with the fields in common between all the Ssh."""
 
-    def __init__(self, key_name: str = None, allowed_ips: str = None, **kwargs):
+    def __init__(self, key_name: str = None, **kwargs):
         super().__init__(**kwargs)
         self.key_name = Resource.init_param(key_name)
-        self.allowed_ips = Resource.init_param(allowed_ips, default=CIDR_ALL_IPS)
 
     def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
         self._register_validator(KeyPairValidator, key_name=self.key_name)
 
 
+class HeadNodeSsh(_BaseSsh):
+    """Represent the SSH configuration for HeadNode."""
+
+    def __init__(self, allowed_ips: str = None, **kwargs):
+        super().__init__(**kwargs)
+        self.allowed_ips = Resource.init_param(allowed_ips, default=CIDR_ALL_IPS)
+
+
 class Dcv(Resource):
     """Represent the DCV configuration."""
 
     def __init__(self, enabled: bool, port: int = None, allowed_ips: str = None):
         super().__init__()
         self.enabled = Resource.init_param(enabled)
         self.port = Resource.init_param(port, default=8443)
@@ -896,27 +907,25 @@
         """Resource regex to be added in IAM policies."""
         if self.key_name:  # If bucket name and key name are specified, we combine them directly
             return [f"{self.bucket_name}/{self.key_name}"]
         else:  # If only bucket name is specified, we add two resources (the bucket and the contents in the bucket).
             return [self.bucket_name, f"{self.bucket_name}/*"]
 
 
-class Iam(Resource):
-    """Represent the IAM configuration for HeadNode and Queue."""
+class _BaseIam(Resource):
+    """Represent the base IAM configuration, with the fields in common between all the Iams."""
 
     def __init__(
         self,
-        s3_access: List[S3Access] = None,
         additional_iam_policies: List[AdditionalIamPolicy] = (),
         instance_role: str = None,
         instance_profile: str = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
-        self.s3_access = s3_access
         self.additional_iam_policies = additional_iam_policies
         self.instance_role = Resource.init_param(instance_role)
         self.instance_profile = Resource.init_param(instance_profile)
 
     @property
     def additional_iam_policy_arns(self) -> List[str]:
         """Get list of arn strings from the list of policy objects."""
@@ -955,14 +964,36 @@
     def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
         if self.instance_role:
             self._register_validator(RoleValidator, role_arn=self.instance_role)
         elif self.instance_profile:
             self._register_validator(InstanceProfileValidator, instance_profile_arn=self.instance_profile)
 
 
+class Iam(_BaseIam):
+    """Represent the IAM configuration for HeadNode and Queue."""
+
+    def __init__(
+        self,
+        s3_access: List[S3Access] = None,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+        self.s3_access = s3_access
+
+
+class LoginNodesIam(_BaseIam):
+    """Represent the IAM configuration for LoginNodes."""
+
+    def __init__(
+        self,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+
+
 class Imds(Resource):
     """Represent the IMDS configuration."""
 
     def __init__(self, secured: bool = None, **kwargs):
         super().__init__(**kwargs)
         self.secured = Resource.init_param(secured, default=True)
 
@@ -1085,21 +1116,25 @@
 
     def __init__(
         self,
         cluster_template: str = None,
         ami_search_filters: AmiSearchFilters = None,
         instance_types_data: str = None,
         timeouts: Timeouts = None,
+        compute_startup_time_metric_enabled: bool = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.cluster_template = Resource.init_param(cluster_template)
         self.ami_search_filters = Resource.init_param(ami_search_filters)
         self.instance_types_data = Resource.init_param(instance_types_data)
         self.timeouts = Resource.init_param(timeouts)
+        self.compute_startup_time_metric_enabled = Resource.init_param(
+            compute_startup_time_metric_enabled, default=False
+        )
 
     def _register_validators(self, context: ValidatorContext = None):
         super()._register_validators(context)
         if self.cluster_template:
             self._register_validator(UrlValidator, url=self.cluster_template)
 
 
@@ -1167,37 +1202,122 @@
     ):
         super().__init__()
         self.on_node_start = Resource.init_param(on_node_start)
         self.on_node_configured = Resource.init_param(on_node_configured)
         self.on_node_updated = Resource.init_param(on_node_updated)
 
 
+class LoginNodesImage(Resource):
+    """Represent the Image configuration of LoginNodes."""
+
+    def __init__(self, custom_ami: str):
+        super().__init__()
+        self.custom_ami = Resource.init_param(custom_ami)
+
+    def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
+        if self.custom_ami:
+            self._register_validator(CustomAmiTagValidator, custom_ami=self.custom_ami)
+
+
+class LoginNodesSsh(_BaseSsh):
+    """Represent the SSH configuration for LoginNodes."""
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+
+class LoginNodesNetworking(_BaseNetworking, SubnetsMixin):
+    """Represent the networking configuration for LoginNodes."""
+
+    def __init__(self, subnet_ids: List[str], proxy: Proxy = None, **kwargs):
+        _BaseNetworking.__init__(self, **kwargs)
+        SubnetsMixin.__init__(self, subnet_ids, **kwargs)
+        self.proxy = proxy
+
+    @property
+    def is_subnet_public(self):
+        """Get if the subnet is public or private."""
+        return AWSApi.instance().ec2.is_subnet_public(self.subnet_ids[0])
+
+
+class LoginNodesPool(Resource):
+    """Represent the configuration of a LoginNodesPool."""
+
+    def __init__(
+        self,
+        name: str,
+        instance_type: str,
+        image: LoginNodesImage = None,
+        networking: LoginNodesNetworking = None,
+        count: int = None,
+        ssh: LoginNodesSsh = None,
+        iam: LoginNodesIam = None,
+        gracetime_period: int = None,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+        self.name = Resource.init_param(name)
+        self.instance_type = Resource.init_param(instance_type)
+        self.image = image
+        self.networking = networking
+        self.count = Resource.init_param(count, default=1)
+        self.ssh = ssh
+        self.iam = iam or LoginNodesIam(implied=True)
+        self.gracetime_period = Resource.init_param(gracetime_period, default=60)
+
+    @property
+    def instance_profile(self):
+        """Return the IAM instance profile for login nodes, if set."""
+        return self.iam.instance_profile if self.iam else None
+
+    @property
+    def instance_role(self):
+        """Return the IAM role for login nodes, if set."""
+        return self.iam.instance_role if self.iam else None
+
+    def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
+        self._register_validator(InstanceTypeValidator, instance_type=self.instance_type)
+        self._register_validator(NameValidator, name=self.name)
+
+
+class LoginNodes(Resource):
+    """Represent the configuration of LoginNodes."""
+
+    def __init__(
+        self,
+        pools: List[LoginNodesPool],
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+        self.pools = pools
+
+
 class HeadNode(Resource):
     """Represent the Head Node resource."""
 
     def __init__(
         self,
         instance_type: str,
         networking: HeadNodeNetworking,
-        ssh: Ssh = None,
+        ssh: HeadNodeSsh = None,
         disable_simultaneous_multithreading: bool = None,
         local_storage: LocalStorage = None,
         dcv: Dcv = None,
         custom_actions: CustomActions = None,
         iam: Iam = None,
         imds: Imds = None,
         image: HeadNodeImage = None,
     ):
         super().__init__()
         self.instance_type = Resource.init_param(instance_type)
         self.disable_simultaneous_multithreading = Resource.init_param(
             disable_simultaneous_multithreading, default=False
         )
         self.networking = networking
-        self.ssh = ssh or Ssh(implied=True)
+        self.ssh = ssh or HeadNodeSsh(implied=True)
         self.local_storage = local_storage or LocalStorage(implied=True)
         self.dcv = dcv
         self.custom_actions = custom_actions
         self.iam = iam or Iam(implied=True)
         self.imds = imds or Imds(implied=True)
         self.image = image
         self.__instance_type_info = None
@@ -1331,15 +1451,15 @@
         self.additional_resources = Resource.init_param(additional_resources)
         self.dev_settings = dev_settings
         self.cluster_template_body = None
         self.source_config = None
         self.config_version = ""
         self.original_config_version = ""
         self._official_ami = None
-        self.imds = imds or TopLevelImds(implied="v1.0")
+        self.imds = imds or TopLevelImds(implied="v2.0")
         self.deployment_settings = deployment_settings
         self.managed_head_node_security_group = None
         self.managed_compute_security_group = None
 
     def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
         self._register_validator(RegionValidator, region=self.region)
         self._register_validator(ClusterNameValidator, name=self.cluster_name, scheduling=self.scheduling)
@@ -1356,18 +1476,15 @@
                 instance_type=self.head_node.instance_type,
                 image=self.head_node_ami,
             )
         if self.head_node.image and self.head_node.image.custom_ami:
             self._register_validator(
                 AmiOsCompatibleValidator, os=self.image.os, image_id=self.head_node.image.custom_ami
             )
-        # Check that all subnets in the cluster (head node subnet included) are in the same VPC and support DNS.
-        self._register_validator(
-            SubnetsValidator, subnet_ids=self.compute_subnet_ids + [self.head_node.networking.subnet_id]
-        )
+
         self._register_storage_validators()
         self._register_validator(
             HeadNodeLaunchTemplateValidator,
             head_node=self.head_node,
             root_volume_device_name=AWSApi.instance().ec2.describe_image(self.head_node_ami).device_name,
             ami_id=self.head_node_ami,
             tags=self.get_tags(),
@@ -1456,14 +1573,18 @@
                     existing_storage_count["fsx"] += 1
                     existing_fsx.add(storage.file_system_id)
                     self._register_validator(FeatureRegionValidator, feature=Feature.FSX_OPENZFS, region=self.region)
                 elif isinstance(storage, ExistingFsxOntap):
                     existing_storage_count["fsx"] += 1
                     existing_fsx.add(storage.file_system_id)
                     self._register_validator(FeatureRegionValidator, feature=Feature.FSX_ONTAP, region=self.region)
+                elif isinstance(storage, ExistingFsxFileCache):
+                    existing_storage_count["fsx"] += 1
+                    existing_fsx.add(storage.file_cache_id)
+                    self._register_validator(FeatureRegionValidator, feature=Feature.FSX_FILE_CACHE, region=self.region)
                 elif isinstance(storage, SharedEbs):
                     if storage.raid:
                         new_storage_count["raid"] += 1
                     else:
                         ebs_count += 1
                 elif isinstance(storage, SharedEfs):
                     if storage.file_system_id:
@@ -1474,19 +1595,18 @@
                             avail_zones_mapping=self.availability_zones_subnets_mapping,
                             security_groups_by_nodes=self.security_groups_by_nodes,
                         )
                     else:
                         new_storage_count["efs"] += 1
             self._register_validator(
                 ExistingFsxNetworkingValidator,
-                file_system_ids=list(existing_fsx),
+                file_storage_ids=list(existing_fsx),
                 subnet_ids=[self.head_node.networking.subnet_id] + self.compute_subnet_ids,
                 security_groups_by_nodes=self.security_groups_by_nodes,
             )
-
             self._validate_max_storage_count(ebs_count, existing_storage_count, new_storage_count)
             self._validate_new_storage_multiple_subnets(
                 self.scheduling.queues, self.compute_subnet_ids, new_storage_count
             )
 
         self._validate_mount_dirs()
 
@@ -1595,15 +1715,15 @@
             mount_dir_instance_types_dict[
                 self.head_node.local_storage.ephemeral_volume.mount_dir
                 if self.head_node.local_storage.ephemeral_volume
                 else DEFAULT_EPHEMERAL_DIR
             ].add(self.head_node.instance_type)
 
         scheduling = self.scheduling
-        if isinstance(scheduling, (SchedulerPluginScheduling, SlurmScheduling)):
+        if isinstance(scheduling, SlurmScheduling):
             for queue in scheduling.queues:
                 instance_types_with_instance_storage = queue.instance_types_with_instance_storage
                 if instance_types_with_instance_storage:
                     mount_dir_instance_types_dict[
                         queue.compute_settings.local_storage.ephemeral_volume.mount_dir
                         if queue.compute_settings.local_storage.ephemeral_volume
                         else DEFAULT_EPHEMERAL_DIR
@@ -1618,27 +1738,28 @@
         if self.shared_storage:
             for storage in self.shared_storage:
                 storage_id = None
                 if isinstance(storage, (SharedEfs, SharedFsxLustre)):
                     storage_id = storage.file_system_id
                 elif isinstance(storage, (SharedEbs, ExistingFsxOpenZfs, ExistingFsxOntap)):
                     storage_id = storage.volume_id
+                elif isinstance(storage, ExistingFsxFileCache):
+                    storage_id = storage.file_cache_id
                 if storage_id:
                     storage_id_list.append(storage_id)
         return storage_id_list
 
     @property
     def compute_subnet_ids(self):
         """Return the list of all compute subnet ids in the cluster."""
-        subnet_ids_list = []
+        subnet_ids_set = set()
         for queue in self.scheduling.queues:
             for subnet_id in queue.networking.subnet_ids:
-                if subnet_id not in subnet_ids_list:
-                    subnet_ids_list.append(subnet_id)
-        return subnet_ids_list
+                subnet_ids_set.add(subnet_id)
+        return list(subnet_ids_set)
 
     @property
     def availability_zones_subnets_mapping(self):
         """Retrieve the mapping of availability zone and cluster subnets."""
         mapping = {self.head_node.networking.availability_zone: {self.head_node.networking.subnet_id}}
         for subnet_id in self.compute_subnet_ids:
             mapping.setdefault(AWSApi.instance().ec2.get_subnet_avail_zone(subnet_id), set()).add(subnet_id)
@@ -1886,14 +2007,18 @@
         self.scheduling = scheduling
 
     def _register_validators(self, context: ValidatorContext = None):
         super()._register_validators(context)
         self._register_validator(FeatureRegionValidator, feature=Feature.BATCH, region=self.region)
         # TODO add InstanceTypesBaseAMICompatibleValidator
 
+        # Check that all subnets in the cluster (head node subnet included) are in the same VPC and support DNS.
+        self._register_validator(
+            SubnetsValidator, subnet_ids=self.compute_subnet_ids + [self.head_node.networking.subnet_id]
+        )
         if self.shared_storage:
             for storage in self.shared_storage:
                 if isinstance(storage, BaseSharedFsx):
                     self._register_validator(AwsBatchFsxValidator)
 
         for queue in self.scheduling.queues:
             for compute_resource in queue.compute_resources:
@@ -1921,14 +2046,16 @@
         disable_simultaneous_multithreading: bool = None,
         schedulable_memory: int = None,
         capacity_reservation_target: CapacityReservationTarget = None,
         networking: SlurmComputeResourceNetworking = None,
         health_checks: HealthChecks = None,
         custom_slurm_settings: Dict = None,
         tags: List[Tag] = None,
+        static_node_priority: int = None,
+        dynamic_node_priority: int = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.max_count = Resource.init_param(max_count, default=DEFAULT_MAX_COUNT)
         self.min_count = Resource.init_param(min_count, default=DEFAULT_MIN_COUNT)
         self.spot_price = Resource.init_param(spot_price)
         self.disable_simultaneous_multithreading = Resource.init_param(
@@ -1939,14 +2066,16 @@
         self.capacity_reservation_target = capacity_reservation_target
         self._instance_types_with_instance_storage = []
         self._instance_type_info_map = {}
         self.networking = networking or SlurmComputeResourceNetworking(implied=True)
         self.health_checks = health_checks or HealthChecks(implied=True)
         self.custom_slurm_settings = Resource.init_param(custom_slurm_settings, default={})
         self.tags = tags
+        self.static_node_priority = Resource.init_param(static_node_priority, default=1)
+        self.dynamic_node_priority = Resource.init_param(dynamic_node_priority, default=1000)
 
     @staticmethod
     def fetch_instance_type_info(instance_type) -> InstanceTypeInfo:
         """Return instance type information."""
         return AWSApi.instance().ec2.get_instance_type_info(instance_type)
 
     @property
@@ -2021,14 +2150,29 @@
     def instance_types(self) -> List[str]:
         """Return list of instance type names in this compute resource."""
         return [
             flexible_instance_type.instance_type
             for flexible_instance_type in self.instances  # pylint: disable=not-an-iterable
         ]
 
+    def _min_schedulable_memory_and_instance_type(self):
+        instances_and_memory = {t: info.ec2memory_size_in_mib() for t, info in self.instance_type_info_map.items()}
+        smallest_type = min(instances_and_memory, key=instances_and_memory.get)
+        return smallest_type, instances_and_memory[smallest_type]
+
+    def _register_validators(self, context: ValidatorContext = None):
+        super()._register_validators(context)
+        smallest_type, min_memory = self._min_schedulable_memory_and_instance_type()
+        self._register_validator(
+            SchedulableMemoryValidator,
+            schedulable_memory=self.schedulable_memory,
+            ec2memory=min_memory,
+            instance_type=smallest_type,
+        )
+
     @property
     def disable_simultaneous_multithreading_manually(self) -> bool:
         """Return true if simultaneous multithreading must be disabled with a cookbook script."""
         return self.disable_simultaneous_multithreading
 
     @property
     def max_network_interface_count(self) -> int:
@@ -2103,33 +2247,21 @@
 
     @property
     def disable_simultaneous_multithreading_manually(self) -> bool:
         """Return true if simultaneous multithreading must be disabled with a cookbook script."""
         return self.disable_simultaneous_multithreading and self.instance_type_info.default_threads_per_core() > 1
 
 
-class SchedulerPluginComputeResource(SlurmComputeResource):
-    """Represent the Scheduler Plugin Compute Resource."""
-
-    def __init__(
-        self,
-        custom_settings: Dict = None,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.custom_settings = custom_settings
-
-
 class _CommonQueue(BaseQueue):
-    """Represent the Common Queue resource between Slurm and Scheduler Plugin."""
+    """Represent the Common Queue resource between Slurm and future scheduler implementation."""
 
     def __init__(
         self,
-        compute_resources: List[Union[_BaseSlurmComputeResource, SchedulerPluginComputeResource]],
-        networking: Union[SlurmQueueNetworking, SchedulerPluginQueueNetworking],
+        compute_resources: List[_BaseSlurmComputeResource],
+        networking: SlurmQueueNetworking,
         compute_settings: ComputeSettings = None,
         custom_actions: CustomActions = None,
         iam: Iam = None,
         image: QueueImage = None,
         capacity_reservation_target: CapacityReservationTarget = None,
         **kwargs,
     ):
@@ -2174,33 +2306,31 @@
         for compute_resource in self.compute_resources:
             placement_group_setting = self.get_placement_group_settings_for_compute_resource(compute_resource)
             if placement_group_setting.get("is_managed"):
                 managed_placement_group_keys.append(placement_group_setting.get("key"))
         return managed_placement_group_keys
 
     def get_placement_group_settings_for_compute_resource(
-        self, compute_resource: Union[_BaseSlurmComputeResource, SchedulerPluginComputeResource]
+        self, compute_resource: _BaseSlurmComputeResource
     ) -> Dict[str, bool]:
         # Placement Group key is None and not managed by default
         placement_group_key, managed = None, False
         # prefer compute level groups over queue level groups
         chosen_pg = self.get_chosen_placement_group_setting_for_compute_resource(compute_resource)
         if chosen_pg.assignment:
             placement_group_key, managed = chosen_pg.assignment, False
         elif chosen_pg.enabled:
             placement_group_key, managed = f"{self.name}-{compute_resource.name}", True
         return {"key": placement_group_key, "is_managed": managed}
 
-    def is_placement_group_enabled_for_compute_resource(
-        self, compute_resource: Union[_BaseSlurmComputeResource, SchedulerPluginComputeResource]
-    ) -> bool:
+    def is_placement_group_enabled_for_compute_resource(self, compute_resource: _BaseSlurmComputeResource) -> bool:
         return self.get_placement_group_settings_for_compute_resource(compute_resource).get("key") is not None
 
     def get_chosen_placement_group_setting_for_compute_resource(
-        self, compute_resource: Union[_BaseSlurmComputeResource, SchedulerPluginComputeResource]
+        self, compute_resource: _BaseSlurmComputeResource
     ) -> PlacementGroup:
         """Handle logic that the Placement Group on compute resource level overrides queue level."""
         return (
             compute_resource.networking.placement_group
             if not compute_resource.networking.placement_group.implied
             else self.networking.placement_group
         )
@@ -2245,20 +2375,22 @@
     """Represents a Slurm Queue that has Compute Resources with both Single and Multiple Instance Types."""
 
     def __init__(
         self,
         allocation_strategy: str = None,
         custom_slurm_settings: Dict = None,
         health_checks: HealthChecks = None,
+        job_exclusive_allocation: bool = None,
         tags: List[Tag] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.health_checks = health_checks or HealthChecks(implied=True)
         self.custom_slurm_settings = Resource.init_param(custom_slurm_settings, default={})
+        self.job_exclusive_allocation = Resource.init_param(job_exclusive_allocation, default=False)
         self.tags = tags
         if any(
             isinstance(compute_resource, SlurmFlexibleComputeResource) for compute_resource in self.compute_resources
         ):
             self.allocation_strategy = (
                 AllocationStrategy[to_snake_case(allocation_strategy).upper()]
                 if allocation_strategy
@@ -2300,14 +2432,19 @@
         )
         self._register_validator(
             QueueSubnetsValidator,
             queue_name=self.name,
             subnet_ids=self.networking.subnet_ids,
             az_subnet_ids_mapping=self.networking.az_subnet_ids_mapping,
         )
+        self._register_validator(
+            SlurmNodePrioritiesWarningValidator,
+            queue_name=self.name,
+            compute_resources=self.compute_resources,
+        )
         if any(isinstance(compute_resource, SlurmComputeResource) for compute_resource in self.compute_resources):
             self._register_validator(
                 SingleInstanceTypeSubnetValidator,
                 queue_name=self.name,
                 subnet_ids=self.networking.subnet_ids,
             )
         if self.custom_slurm_settings:
@@ -2477,401 +2614,139 @@
             MaxCountValidator,
             resources_length=sum(len(queue.compute_resources) for queue in self.queues),
             max_length=MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER,
             resource_name="ComputeResources per Cluster",
         )
 
 
-class SchedulerPluginQueue(_CommonQueue):
-    """Represent the Scheduler Plugin queue."""
-
-    def __init__(
-        self,
-        custom_settings: Dict = None,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.custom_settings = custom_settings
-
-    def _register_validators(self, context: ValidatorContext = None):
-        super()._register_validators(context)
-        self._register_validator(
-            DuplicateNameValidator,
-            name_list=[compute_resource.name for compute_resource in self.compute_resources],
-            resource_name="Compute resource",
-        )
-        self._register_validator(
-            MaxCountValidator,
-            resources_length=len(self.compute_resources),
-            max_length=SCHEDULER_PLUGIN_MAX_NUMBER_OF_COMPUTE_RESOURCES,
-            resource_name="ComputeResources per Queue",
-        )
-        self._register_validator(
-            QueueSubnetsValidator,
-            queue_name=self.name,
-            subnet_ids=self.networking.subnet_ids,
-            az_subnet_ids_mapping=self.networking.az_subnet_ids_mapping,
-        )
-        if any(isinstance(compute_resource, SlurmComputeResource) for compute_resource in self.compute_resources):
-            self._register_validator(
-                SingleInstanceTypeSubnetValidator,
-                queue_name=self.name,
-                subnet_ids=self.networking.subnet_ids,
-            )
-        for compute_resource in self.compute_resources:
-            self._register_validator(
-                CapacityTypeValidator, capacity_type=self.capacity_type, instance_type=compute_resource.instance_type
-            )
-            self._register_validator(
-                EfaSecurityGroupValidator,
-                efa_enabled=compute_resource.efa.enabled,
-                security_groups=self.networking.security_groups,
-                additional_security_groups=self.networking.additional_security_groups,
-            )
-            self._register_validator(
-                EfaPlacementGroupValidator,
-                efa_enabled=compute_resource.efa.enabled,
-                placement_group_key=self.get_placement_group_settings_for_compute_resource(compute_resource).get("key"),
-                placement_group_disabled=self.get_chosen_placement_group_setting_for_compute_resource(
-                    compute_resource
-                ).enabled
-                is False,
-                multi_az_enabled=self.multi_az_enabled,
-            )
-
-    @property
-    def instance_type_list(self):
-        """Return the list of instance types associated to the Queue."""
-        return [compute_resource.instance_type for compute_resource in self.compute_resources]
-
-    @property
-    def instance_types_with_instance_storage(self):
-        """Return a set of instance types in the queue that have instance store."""
-        result = set()
-        for compute_resource in self.compute_resources:
-            if compute_resource.instance_type_info.instance_storage_supported():
-                result.add(compute_resource.instance_type)
-        return result
-
-
-class SchedulerPluginSupportedDistros(Resource):
-    """Represent the Supported Distros for a Scheduler Plugin."""
-
-    def __init__(self, x86: List[str] = None, arm64: List[str] = None, **kwargs):
-        super().__init__(**kwargs)
-        self.x86 = Resource.init_param(x86, default=SUPPORTED_OSES)
-        self.arm64 = Resource.init_param(arm64, default=SUPPORTED_OSES)
-
-
-class SchedulerPluginQueueConstraints(Resource):
-    """Represent the Queue Constraints for a Scheduler Plugin."""
-
-    def __init__(self, max_count: int = None, **kwargs):
-        super().__init__(**kwargs)
-        self.max_count = Resource.init_param(max_count, default=SCHEDULER_PLUGIN_MAX_NUMBER_OF_QUEUES)
-
-
-class SchedulerPluginComputeResourceConstraints(Resource):
-    """Represent the Compute Resource Constraints for a Scheduler Plugin."""
-
-    def __init__(self, max_count: int = None, **kwargs):
-        super().__init__(**kwargs)
-        self.max_count = Resource.init_param(max_count, default=SCHEDULER_PLUGIN_MAX_NUMBER_OF_COMPUTE_RESOURCES)
-
-
-class SchedulerPluginRequirements(Resource):
-    """Represent the Requirements for a Scheduler Plugin."""
-
-    def __init__(
-        self,
-        supported_distros: SchedulerPluginSupportedDistros = None,
-        supported_regions: List[str] = None,
-        queue_constraints: SchedulerPluginQueueConstraints = None,
-        compute_resource_constraints: SchedulerPluginComputeResourceConstraints = None,
-        requires_sudo_privileges: bool = None,
-        supports_cluster_update: bool = None,
-        supported_parallel_cluster_versions: str = None,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.supported_distros = supported_distros
-        self.supported_regions = supported_regions
-        self.queue_constraints = queue_constraints
-        self.compute_resource_constraints = compute_resource_constraints
-        self.requires_sudo_privileges = Resource.init_param(requires_sudo_privileges, default=False)
-        self.supports_cluster_update = Resource.init_param(supports_cluster_update, default=True)
-        self.supported_parallel_cluster_versions = supported_parallel_cluster_versions
-
-    def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
-        if self.supported_parallel_cluster_versions:
-            self._register_validator(
-                SupportedVersionsValidator,
-                installed_version=get_installed_version(),
-                supported_versions_string=self.supported_parallel_cluster_versions,
-            )
-
-
-class SchedulerPluginCloudFormationInfrastructure(Resource):
-    """Represent the CloudFormation infrastructure for a Scheduler Plugin."""
-
-    def __init__(self, template: str, s3_bucket_owner: str = None, checksum: str = None, **kwargs):
-        super().__init__(**kwargs)
-        self.template = replace_url_parameters(template)
-        self.s3_bucket_owner = s3_bucket_owner
-        self.checksum = checksum
-
-    def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
-        self._register_validator(
-            UrlValidator,
-            url=self.template,
-            fail_on_https_error=True,
-            fail_on_s3_error=True,
-            expected_bucket_owner=self.s3_bucket_owner,
-        )
-
-
-class SchedulerPluginClusterInfrastructure(Resource):
-    """Represent the ClusterInfastructure config for a Scheduler Plugin."""
-
-    def __init__(self, cloud_formation: SchedulerPluginCloudFormationInfrastructure = None, **kwargs):
-        super().__init__(**kwargs)
-        self.cloud_formation = cloud_formation
-
-
-class SchedulerPluginClusterSharedArtifact(Resource):
-    """Represent the ClusterSharedArtifact config for a Scheduler Plugin."""
-
-    def __init__(self, source: str, s3_bucket_owner: str = None, checksum: str = None, **kwargs):
-        super().__init__(**kwargs)
-        self.source = replace_url_parameters(source)
-        self.s3_bucket_owner = s3_bucket_owner
-        self.checksum = checksum
-
-    def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
-        self._register_validator(UrlValidator, url=self.source, expected_bucket_owner=self.s3_bucket_owner)
-
-
-class SchedulerPluginPluginResources(Resource):
-    """Represent the PluginResources config for a Scheduler Plugin."""
-
-    def __init__(self, cluster_shared_artifacts: [SchedulerPluginClusterSharedArtifact], **kwargs):
-        super().__init__(**kwargs)
-        self.cluster_shared_artifacts = cluster_shared_artifacts
-
-
-class SchedulerPluginExecuteCommand(Resource):
-    """Represent the ExecuteCommand for a Scheduler Plugin."""
-
-    def __init__(self, command: str, **kwargs):
-        super().__init__(**kwargs)
-        self.command = command
-
-
-class SchedulerPluginEvent(Resource):
-    """Represent the Event config for a Scheduler Plugin."""
-
-    def __init__(self, execute_command: SchedulerPluginExecuteCommand, **kwargs):
-        super().__init__(**kwargs)
-        self.execute_command = execute_command
-
-
-class SchedulerPluginEvents(Resource):
-    """Represent the Events config for a Scheduler Plugin."""
-
-    def __init__(
-        self,
-        head_init: SchedulerPluginEvent = None,
-        head_configure: SchedulerPluginEvent = None,
-        head_finalize: SchedulerPluginEvent = None,
-        compute_init: SchedulerPluginEvent = None,
-        compute_configure: SchedulerPluginEvent = None,
-        compute_finalize: SchedulerPluginEvent = None,
-        head_cluster_update: SchedulerPluginEvent = None,
-        head_compute_fleet_update: SchedulerPluginEvent = None,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.head_init = head_init
-        self.head_configure = head_configure
-        self.head_finalize = head_finalize
-        self.compute_init = compute_init
-        self.compute_configure = compute_configure
-        self.compute_finalize = compute_finalize
-        self.head_cluster_update = head_cluster_update
-        self.head_compute_fleet_update = head_compute_fleet_update
-
-
-class SchedulerPluginFile(Resource):
-    """Represent the Scheduler Plugin file resource."""
-
-    def __init__(
-        self, file_path: str, log_stream_name: str, node_type: str = None, timestamp_format: str = None, **kwargs
-    ):
-        super().__init__(**kwargs)
-        self.file_path = file_path
-        self.timestamp_format = Resource.init_param(timestamp_format, default="%Y-%m-%dT%H:%M:%S%z")
-        self.node_type = Resource.init_param(node_type, default="ALL")
-        self.log_stream_name = log_stream_name
-
-
-class SchedulerPluginLogs(Resource):
-    """Represent the Scheduler Plugin logs resource."""
-
-    def __init__(self, files: [SchedulerPluginFile], **kwargs):
-        super().__init__(**kwargs)
-        self.files = files
-
-
-class SchedulerPluginMonitoring(Resource):
-    """Represent the Scheduler Plugin monitoring resource."""
-
-    def __init__(self, logs: SchedulerPluginLogs, **kwargs):
-        super().__init__(**kwargs)
-        self.logs = logs
-
-
 class SudoerConfiguration(Resource):
     """Represent the SudoerConfiguration resource."""
 
     def __init__(self, commands: str, run_as: str, **kwargs):
         super().__init__(**kwargs)
         self.commands = commands
         self.run_as = run_as
 
 
-class SchedulerPluginUser(Resource):
-    """Represent the Scheduler Plugin user resource."""
-
-    def __init__(
-        self, name: str, enable_imds: bool = None, sudoer_configuration: List[SudoerConfiguration] = (), **kwargs
-    ):
-        super().__init__(**kwargs)
-        self.name = name
-        self.enable_imds = Resource.init_param(enable_imds, default=False)
-        self.sudoer_configuration = sudoer_configuration
-
-    def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
-        self._register_validator(
-            UserNameValidator,
-            user_name=self.name,
-        )
-
-
-class SchedulerPluginDefinition(Resource):
-    """Represent the Scheduler Plugin scheduler definition."""
+class SlurmClusterConfig(BaseClusterConfig):
+    """Represent the full Slurm Cluster configuration."""
 
     def __init__(
         self,
-        plugin_interface_version: str,
-        events: SchedulerPluginEvents,
-        metadata: Dict = None,
-        requirements: SchedulerPluginRequirements = None,
-        cluster_infrastructure: SchedulerPluginClusterInfrastructure = None,
-        plugin_resources: SchedulerPluginPluginResources = None,
-        monitoring: SchedulerPluginMonitoring = None,
-        system_users: [SchedulerPluginUser] = None,
-        tags: List[Tag] = None,
+        cluster_name: str,
+        scheduling: SlurmScheduling,
+        login_nodes: LoginNodes = None,
         **kwargs,
     ):
-        super().__init__(**kwargs)
-        self.plugin_interface_version = plugin_interface_version
-        self.metadata = metadata
-        self.requirements = requirements
-        self.cluster_infrastructure = cluster_infrastructure
-        self.plugin_resources = plugin_resources
-        self.events = events
-        self.monitoring = monitoring
-        self.system_users = system_users
-        self.tags = tags
-
-    def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
-        self._register_validator(
-            PluginInterfaceVersionValidator,
-            plugin_version=self.plugin_interface_version,
-            support_version_low_range=SCHEDULER_PLUGIN_INTERFACE_VERSION_LOW_RANGE,
-            support_version_high_range=SCHEDULER_PLUGIN_INTERFACE_VERSION,
-        )
+        super().__init__(cluster_name, **kwargs)
+        self.scheduling = scheduling
+        self.login_nodes = login_nodes
+        if self.login_nodes:
+            for pool in self.login_nodes.pools:
+                if pool.ssh and not pool.ssh.key_name:
+                    pool.ssh.key_name = self.head_node.ssh.key_name
+                elif not pool.ssh:
+                    pool.ssh = LoginNodesSsh(key_name=self.head_node.ssh.key_name)
+        self.__image_dict = None
+        # Cache capacity reservations information together to reduce number of boto3 calls.
+        # Since this cache is only used for validation, if AWSClientError happens
+        # (e.g insufficient IAM permissions to describe the capacity reservations), we catch the exception to avoid
+        # blocking CLI execution if the user want to suppress the validation.
+        try:
+            AWSApi.instance().ec2.describe_capacity_reservations(self.all_relevant_capacity_reservation_ids)
+        except AWSClientError:
+            logging.warning("Unable to cache describe_capacity_reservations results for all capacity reservation ids.")
 
+    def get_instance_types_data(self):
+        """Get instance type infos for all instance types used in the configuration file."""
+        result = {}
+        instance_type_info = self.head_node.instance_type_info
+        result[instance_type_info.instance_type()] = instance_type_info.instance_type_data
+        for queue in self.scheduling.queues:
+            for compute_resource in queue.compute_resources:
+                for instance_type in compute_resource.instance_types:
+                    instance_type_info = compute_resource.instance_type_info_map[instance_type]
+                    result[instance_type] = instance_type_info.instance_type_data
+        return result
 
-class SchedulerPluginSettings(Resource):
-    """Represent the Scheduler Plugin settings."""
+    @property
+    def login_nodes_ami(self):
+        """Get the image id of the LoginNodes."""
+        login_nodes_ami_dict = {}
+        if self.login_nodes:
+            for pool in self.login_nodes.pools:
+                if pool.image and pool.image.custom_ami:
+                    login_nodes_ami_dict[pool.name] = pool.image.custom_ami
+                elif self.image.custom_ami:
+                    login_nodes_ami_dict[pool.name] = self.image.custom_ami
+                else:
+                    login_nodes_ami_dict[pool.name] = self.official_ami
+        return login_nodes_ami_dict
 
-    def __init__(
-        self,
-        scheduler_definition: SchedulerPluginDefinition,
-        grant_sudo_privileges: bool = None,
-        custom_settings: Dict = None,
-        scheduler_definition_s3_bucket_owner: str = None,
-        scheduler_definition_checksum: str = None,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.scheduler_definition = scheduler_definition
-        self.grant_sudo_privileges = Resource.init_param(grant_sudo_privileges, default=False)
-        self.custom_settings = custom_settings
-        self.scheduler_definition_s3_bucket_owner = scheduler_definition_s3_bucket_owner
-        self.scheduler_definition_checksum = scheduler_definition_checksum
+    @property
+    def has_gpu_health_checks_enabled(self):
+        """Return True if an queue or compute resources has GPU health checking enabled."""
+        for queue in self.scheduling.queues:
+            if queue.health_checks.gpu.enabled:
+                return True
+            for compute_resource in queue.compute_resources:
+                if compute_resource.health_checks.gpu.enabled:
+                    return True
+        return False
 
-    def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
-        self._register_validator(
-            SudoPrivilegesValidator,
-            grant_sudo_privileges=self.grant_sudo_privileges,
-            requires_sudo_privileges=self.scheduler_definition.requirements.requires_sudo_privileges
-            if self.scheduler_definition.requirements
-            else None,
-        )
+    @property
+    def login_nodes_subnet_ids(self):
+        """Return the list of all LoginNodes subnet ids in the cluster."""
+        subnet_ids_set = set()
+        for pool in self.login_nodes.pools:
+            for subnet_id in pool.networking.subnet_ids:
+                subnet_ids_set.add(subnet_id)
+        return list(subnet_ids_set)
 
+    def _register_validators(self, context: ValidatorContext = None):  # noqa: C901
+        super()._register_validators(context)
         self._register_validator(
-            GrantSudoPrivilegesValidator,
-            grant_sudo_privileges=self.grant_sudo_privileges,
-            system_users=get_attr(self.scheduler_definition, "system_users"),
+            MixedSecurityGroupOverwriteValidator,
+            head_node_security_groups=self.head_node.networking.security_groups,
+            queues=self.scheduling.queues,
         )
 
+        # Check if all subnets(head node, Login nodes, compute nodes) are in the same VPC and support DNS.
+        if self.login_nodes:
+            self._register_validator(
+                SubnetsValidator,
+                subnet_ids=self.login_nodes_subnet_ids
+                + self.compute_subnet_ids
+                + [self.head_node.networking.subnet_id],
+            )
+
+        if self.login_nodes:
+            self._register_validator(LoginNodesSchedulerValidator, scheduler=self.scheduling.scheduler)
+
+        # Check the LoginNodes CustomAMI must be an ami of the same os family and the same arch.
+        if self.login_nodes:
+            for pool in self.login_nodes.pools:
+                if pool.image and pool.image.custom_ami:
+                    self._register_validator(AmiOsCompatibleValidator, os=self.image.os, image_id=pool.image.custom_ami)
+                    self._register_validator(
+                        InstanceTypeBaseAMICompatibleValidator,
+                        instance_type=pool.instance_type,
+                        image=self.login_nodes_ami[pool.name],
+                    )
 
-class SchedulerPluginScheduling(Resource):
-    """Represent a Scheduler Plugin Scheduling resource."""
-
-    def __init__(self, queues: List[SchedulerPluginQueue], settings: SchedulerPluginSettings, **kwargs):
-        super().__init__(**kwargs)
-        self.scheduler = "plugin"
-        self.queues = queues
-        self.settings = settings
-
-    def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
-        self._register_validator(
-            DuplicateNameValidator, name_list=[queue.name for queue in self.queues], resource_name="Queue"
-        )
-        self._register_validator(
-            MaxCountValidator,
-            resources_length=len(self.queues),
-            max_length=get_attr(
-                self.settings.scheduler_definition,
-                "requirements.queue_constraints.max_count",
-                default=SCHEDULER_PLUGIN_MAX_NUMBER_OF_QUEUES,
-            ),
-            resource_name="SchedulerQueues",
-        )
-        for queue in self.queues:
-            self._register_validator(
-                MaxCountValidator,
-                resources_length=len(queue.compute_resources),
-                max_length=get_attr(
-                    self.settings.scheduler_definition,
-                    "requirements.compute_resource_constraints.max_count",
-                    default=SCHEDULER_PLUGIN_MAX_NUMBER_OF_COMPUTE_RESOURCES,
-                ),
-                resource_name="ComputeResources",
+        if self.scheduling.settings and self.scheduling.settings.dns and self.scheduling.settings.dns.hosted_zone_id:
+            self._register_validator(
+                HostedZoneValidator,
+                hosted_zone_id=self.scheduling.settings.dns.hosted_zone_id,
+                cluster_vpc=self.vpc_id,
+                cluster_name=self.cluster_name,
             )
 
-
-class CommonSchedulerClusterConfig(BaseClusterConfig):
-    """Represent the common Cluster configuration between Slurm Config and Scheduler Plugin Config."""
-
-    def _register_validators(self, context: ValidatorContext = None):
-        super()._register_validators(context)
+        instance_types_data = self.get_instance_types_data()
+        self._register_validator(MultiNetworkInterfacesInstancesValidator, queues=self.scheduling.queues)
         checked_images = []
         for index, queue in enumerate(self.scheduling.queues):
             queue_image = self.image_dict[queue.name]
             if index == 0:
                 # Execute LaunchTemplateValidator only for the first queue
                 self._register_validator(
                     ComputeResourceLaunchTemplateValidator,
@@ -2883,37 +2758,29 @@
                 )
             ami_volume_size = AWSApi.instance().ec2.describe_image(queue_image).volume_size
             root_volume = queue.compute_settings.local_storage.root_volume
             root_volume_size = root_volume.size
             if root_volume_size is None:  # If root volume size is not specified, it will be the size of the AMI.
                 root_volume_size = ami_volume_size
             self._register_validator(
-                RootVolumeSizeValidator,
-                root_volume_size=root_volume_size,
-                ami_volume_size=ami_volume_size,
+                RootVolumeSizeValidator, root_volume_size=root_volume_size, ami_volume_size=ami_volume_size
             )
             self._register_validator(
                 EbsVolumeTypeSizeValidator, volume_type=root_volume.volume_type, volume_size=root_volume_size
             )
             self._register_validator(
                 EbsVolumeIopsValidator,
                 volume_type=root_volume.volume_type,
                 volume_size=root_volume_size,
                 volume_iops=root_volume.iops,
             )
             if queue_image not in checked_images and queue.queue_ami:
                 checked_images.append(queue_image)
                 self._register_validator(AmiOsCompatibleValidator, os=self.image.os, image_id=queue_image)
             for compute_resource in queue.compute_resources:
-                for instance_type in compute_resource.instance_types:
-                    self._register_validator(
-                        InstanceTypeBaseAMICompatibleValidator,
-                        instance_type=instance_type,
-                        image=queue_image,
-                    )
                 self._register_validator(
                     InstanceArchitectureCompatibilityValidator,
                     instance_type_info_list=list(compute_resource.instance_type_info_map.values()),
                     architecture=self.head_node.architecture,
                 )
                 self._register_validator(
                     EfaOsArchitectureValidator,
@@ -2946,14 +2813,80 @@
                         ),
                         odcr=cr_target,
                         subnet=queue.networking.subnet_ids[0],
                         instance_types=compute_resource.instance_types,
                         multi_az_enabled=queue.multi_az_enabled,
                         subnet_id_az_mapping=queue.networking.subnet_id_az_mapping,
                     )
+                for instance_type in compute_resource.instance_types:
+                    if self.scheduling.settings.enable_memory_based_scheduling:
+                        self._register_validator(
+                            InstanceTypeMemoryInfoValidator,
+                            instance_type=instance_type,
+                            instance_type_data=instance_types_data[instance_type],
+                        )
+                    self._register_validator(
+                        InstanceTypeBaseAMICompatibleValidator,
+                        instance_type=instance_type,
+                        image=queue_image,
+                    )
+                    self._register_validator(
+                        InstanceTypeAcceleratorManufacturerValidator,
+                        instance_type=instance_type,
+                        instance_type_data=instance_types_data[instance_type],
+                    )
+                    self._register_validator(
+                        InstanceTypePlacementGroupValidator,
+                        instance_type=instance_type,
+                        instance_type_data=instance_types_data[instance_type],
+                        placement_group_enabled=queue.is_placement_group_enabled_for_compute_resource(compute_resource),
+                    )
+                if isinstance(compute_resource, SlurmFlexibleComputeResource):
+                    validator_args = dict(
+                        queue_name=queue.name,
+                        multiaz_queue=queue.multi_az_enabled,
+                        capacity_type=queue.capacity_type,
+                        allocation_strategy=queue.allocation_strategy,
+                        compute_resource_name=compute_resource.name,
+                        instance_types_info=compute_resource.instance_type_info_map,
+                        disable_simultaneous_multithreading=compute_resource.disable_simultaneous_multithreading,
+                        efa_enabled=compute_resource.efa and compute_resource.efa.enabled,
+                        placement_group_enabled=queue.is_placement_group_enabled_for_compute_resource(compute_resource),
+                        memory_scheduling_enabled=self.scheduling.settings.enable_memory_based_scheduling,
+                    )
+                    flexible_instance_types_validators = [
+                        InstancesCPUValidator,
+                        InstancesAcceleratorsValidator,
+                        InstancesEFAValidator,
+                        InstancesNetworkingValidator,
+                        InstancesAllocationStrategyValidator,
+                        InstancesMemorySchedulingWarningValidator,
+                    ]
+                    for validator in flexible_instance_types_validators:
+                        self._register_validator(validator, **validator_args)
+                self._register_validator(
+                    ComputeResourceTagsValidator,
+                    queue_name=queue.name,
+                    compute_resource_name=compute_resource.name,
+                    cluster_tags=self.get_tags(),
+                    queue_tags=queue.get_tags(),
+                    compute_resource_tags=compute_resource.get_tags(),
+                )
+
+    @property
+    def image_dict(self):
+        """Return image dict of queues, key is queue name, value is image id."""
+        if self.__image_dict:
+            return self.__image_dict
+        self.__image_dict = {}
+
+        for queue in self.scheduling.queues:
+            self.__image_dict[queue.name] = queue.queue_ami or self.image.custom_ami or self.official_ami
+
+        return self.__image_dict
 
     @property
     def _capacity_reservation_targets(self):
         """Return a list of capacity reservation targets from all queues and compute resources with the section."""
         capacity_reservation_targets_list = []
         for queue in self.scheduling.queues:
             if queue.capacity_reservation_target:
@@ -3006,193 +2939,7 @@
     @property
     def has_custom_actions_in_queue(self):
         """Return True if any queues have custom scripts."""
         for queue in self.scheduling.queues:
             if queue.custom_actions:
                 return True
         return False
-
-
-class SchedulerPluginClusterConfig(CommonSchedulerClusterConfig):
-    """Represent the full Scheduler Plugin Cluster configuration."""
-
-    def __init__(self, cluster_name: str, scheduling: SchedulerPluginScheduling, **kwargs):
-        super().__init__(cluster_name, **kwargs)
-        self.scheduling = scheduling
-        self.__image_dict = None
-        # Cache capacity reservations information together to reduce number of boto3 calls.
-        # Since this cache is only used for validation, if AWSClientError happens
-        # (e.g insufficient IAM permissions to describe the capacity reservations), we catch the exception to avoid
-        # blocking CLI execution if the user want to suppress the validation.
-        try:
-            AWSApi.instance().ec2.describe_capacity_reservations(self.all_relevant_capacity_reservation_ids)
-        except AWSClientError:
-            logging.warning("Unable to cache describe_capacity_reservations results for all capacity reservation ids.")
-
-    def get_instance_types_data(self):
-        """Get instance type infos for all instance types used in the configuration file."""
-        result = {}
-        instance_type_info = self.head_node.instance_type_info
-        result[instance_type_info.instance_type()] = instance_type_info.instance_type_data
-        for queue in self.scheduling.queues:
-            for compute_resource in queue.compute_resources:
-                instance_type_info = compute_resource.instance_type_info
-                result[instance_type_info.instance_type()] = instance_type_info.instance_type_data
-        return result
-
-    def get_tags(self):
-        """Return tags configured in the root of the cluster config and under scheduler definition."""
-        return (self.tags if self.tags else []) + get_attr(
-            self.scheduling, "settings.scheduler_definition.tags", default=[]
-        )
-
-    def _register_validators(self, context: ValidatorContext = None):
-        super()._register_validators(context)
-        scheduler_definition = self.scheduling.settings.scheduler_definition
-        self._register_validator(
-            SchedulerPluginOsArchitectureValidator,
-            os=self.image.os,
-            architecture=self.head_node.architecture,
-            supported_x86=get_attr(scheduler_definition, "requirements.supported_distros.x86", default=SUPPORTED_OSES),
-            supported_arm64=get_attr(
-                scheduler_definition, "requirements.supported_distros.arm64", default=SUPPORTED_OSES
-            ),
-        )
-        self._register_validator(
-            SchedulerPluginRegionValidator,
-            region=self.region,
-            supported_regions=get_attr(scheduler_definition, "requirements.supported_regions"),
-        )
-
-    @property
-    def image_dict(self):
-        """Return image dict of queues, key is queue name, value is image id."""
-        if self.__image_dict:
-            return self.__image_dict
-        self.__image_dict = {}
-
-        for queue in self.scheduling.queues:
-            self.__image_dict[queue.name] = queue.queue_ami or self.image.custom_ami or self.official_ami
-
-        return self.__image_dict
-
-
-class SlurmClusterConfig(CommonSchedulerClusterConfig):
-    """Represent the full Slurm Cluster configuration."""
-
-    def __init__(self, cluster_name: str, scheduling: SlurmScheduling, **kwargs):
-        super().__init__(cluster_name, **kwargs)
-        self.scheduling = scheduling
-        self.__image_dict = None
-        # Cache capacity reservations information together to reduce number of boto3 calls.
-        # Since this cache is only used for validation, if AWSClientError happens
-        # (e.g insufficient IAM permissions to describe the capacity reservations), we catch the exception to avoid
-        # blocking CLI execution if the user want to suppress the validation.
-        try:
-            AWSApi.instance().ec2.describe_capacity_reservations(self.all_relevant_capacity_reservation_ids)
-        except AWSClientError:
-            logging.warning("Unable to cache describe_capacity_reservations results for all capacity reservation ids.")
-
-    def get_instance_types_data(self):
-        """Get instance type infos for all instance types used in the configuration file."""
-        result = {}
-        instance_type_info = self.head_node.instance_type_info
-        result[instance_type_info.instance_type()] = instance_type_info.instance_type_data
-        for queue in self.scheduling.queues:
-            for compute_resource in queue.compute_resources:
-                for instance_type in compute_resource.instance_types:
-                    instance_type_info = compute_resource.instance_type_info_map[instance_type]
-                    result[instance_type] = instance_type_info.instance_type_data
-        return result
-
-    @property
-    def has_gpu_health_checks_enabled(self):
-        """Return True if an queue or compute resources has GPU health checking enabled."""
-        for queue in self.scheduling.queues:
-            if queue.health_checks.gpu.enabled:
-                return True
-            for compute_resource in queue.compute_resources:
-                if compute_resource.health_checks.gpu.enabled:
-                    return True
-        return False
-
-    def _register_validators(self, context: ValidatorContext = None):
-        super()._register_validators(context)
-        self._register_validator(
-            MixedSecurityGroupOverwriteValidator,
-            head_node_security_groups=self.head_node.networking.security_groups,
-            queues=self.scheduling.queues,
-        )
-        if self.scheduling.settings and self.scheduling.settings.dns and self.scheduling.settings.dns.hosted_zone_id:
-            self._register_validator(
-                HostedZoneValidator,
-                hosted_zone_id=self.scheduling.settings.dns.hosted_zone_id,
-                cluster_vpc=self.vpc_id,
-                cluster_name=self.cluster_name,
-            )
-
-        instance_types_data = self.get_instance_types_data()
-        self._register_validator(MultiNetworkInterfacesInstancesValidator, queues=self.scheduling.queues)
-        for queue in self.scheduling.queues:
-            for compute_resource in queue.compute_resources:
-                if self.scheduling.settings.enable_memory_based_scheduling:
-                    for instance_type in compute_resource.instance_types:
-                        self._register_validator(
-                            InstanceTypeMemoryInfoValidator,
-                            instance_type=instance_type,
-                            instance_type_data=instance_types_data[instance_type],
-                        )
-                for instance_type in compute_resource.instance_types:
-                    self._register_validator(
-                        InstanceTypeAcceleratorManufacturerValidator,
-                        instance_type=instance_type,
-                        instance_type_data=instance_types_data[instance_type],
-                    )
-                    self._register_validator(
-                        InstanceTypePlacementGroupValidator,
-                        instance_type=instance_type,
-                        instance_type_data=instance_types_data[instance_type],
-                        placement_group_enabled=queue.is_placement_group_enabled_for_compute_resource(compute_resource),
-                    )
-                if isinstance(compute_resource, SlurmFlexibleComputeResource):
-                    validator_args = dict(
-                        queue_name=queue.name,
-                        multiaz_queue=queue.multi_az_enabled,
-                        capacity_type=queue.capacity_type,
-                        allocation_strategy=queue.allocation_strategy,
-                        compute_resource_name=compute_resource.name,
-                        instance_types_info=compute_resource.instance_type_info_map,
-                        disable_simultaneous_multithreading=compute_resource.disable_simultaneous_multithreading,
-                        efa_enabled=compute_resource.efa and compute_resource.efa.enabled,
-                        placement_group_enabled=queue.is_placement_group_enabled_for_compute_resource(compute_resource),
-                        memory_scheduling_enabled=self.scheduling.settings.enable_memory_based_scheduling,
-                    )
-                    flexible_instance_types_validators = [
-                        InstancesCPUValidator,
-                        InstancesAcceleratorsValidator,
-                        InstancesEFAValidator,
-                        InstancesNetworkingValidator,
-                        InstancesAllocationStrategyValidator,
-                        InstancesMemorySchedulingValidator,
-                    ]
-                    for validator in flexible_instance_types_validators:
-                        self._register_validator(validator, **validator_args)
-                self._register_validator(
-                    ComputeResourceTagsValidator,
-                    queue_name=queue.name,
-                    compute_resource_name=compute_resource.name,
-                    cluster_tags=self.get_tags(),
-                    queue_tags=queue.get_tags(),
-                    compute_resource_tags=compute_resource.get_tags(),
-                )
-
-    @property
-    def image_dict(self):
-        """Return image dict of queues, key is queue name, value is image id."""
-        if self.__image_dict:
-            return self.__image_dict
-        self.__image_dict = {}
-
-        for queue in self.scheduling.queues:
-            self.__image_dict[queue.name] = queue.queue_ami or self.image.custom_ami or self.official_ami
-
-        return self.__image_dict
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/config/common.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/config/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,15 @@
 
     It represents the Imds element that can be either at top level in the cluster config file,
     or in the Build section of the build image config file.
     """
 
     def __init__(self, imds_support: str = None, **kwargs):
         super().__init__(**kwargs)
-        self.imds_support = Resource.init_param(imds_support, default="v1.0")
+        self.imds_support = Resource.init_param(imds_support, default="v2.0")
 
 
 class DeploymentSettings(Resource):
     """
     Represent the settings related to PCluster deployment, i.e. Lambda Functions for custom resources.
 
     This structure is common to both the cluster and build image configuration files, as the build image
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/config/config_patch.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/config/config_patch.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/config/imagebuilder_config.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/config/imagebuilder_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         self.parent_image = Resource.init_param(parent_image)
         self.iam = iam
         self.tags = tags
         self.subnet_id = Resource.init_param(subnet_id)
         self.security_group_ids = security_group_ids
         self.components = components
         self.update_os_packages = update_os_packages
-        self.imds = imds or Imds(implied="v1.0")
+        self.imds = imds or Imds(implied="v2.0")
 
     def _register_validators(self, context: ValidatorContext = None):  # noqa: D102 #pylint: disable=unused-argument
         self._register_validator(
             InstanceTypeBaseAMICompatibleValidator,
             instance_type=self.instance_type,
             image=self.parent_image,
         )
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/config/update_policy.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/config/update_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         return True
     return False
 
 
 def fail_reason_shared_storage_update_policy(change, patch):
     if is_awsbatch_scheduler(change, patch):
         return f"Update actions are not currently supported for the '{change.key}' parameter"
-    reason = "All compute nodes must be stopped"
+    reason = "All login and compute nodes must be stopped"
     # QueueUpdateStrategy can override UpdatePolicy of parameters under SlurmQueues
     if not is_stop_required_for_shared_storage(change) and is_slurm_scheduler(patch):
         reason += " or QueueUpdateStrategy must be set"
 
     return reason
 
 
@@ -324,14 +324,15 @@
             if change.old_value is not None
             else "{0} the parameter '{1}'".format("Restore" if change.is_list else "Remove", change.key)
             + ". If you need this change, please consider creating a new cluster instead of updating the existing one."
         )
     actions = "Stop the compute fleet with the pcluster update-compute-fleet command"
     if not is_stop_required_for_shared_storage(change) and is_slurm_scheduler(patch):
         actions += ", or set QueueUpdateStrategy in the configuration used for the 'update-cluster' operation"
+    actions += f". {UpdatePolicy.ACTIONS_NEEDED['login_nodes_stop'](change, patch)}"
 
     return actions
 
 
 def actions_needed_managed_fsx(change, patch):
     fsx_lustre_names = unchanged_managed_fsx_lustre_names(change, patch)
     if fsx_lustre_names:
@@ -343,49 +344,72 @@
         return actions_needed_queue_update_strategy(change, patch)
 
 
 def condition_checker_shared_storage_update_policy(change, patch):
     """
     Check different requirements for different schedulers.
 
-    Compute fleet stop is required for plugin scheduler.
+    Compute and login fleet stop is required for plugin scheduler.
     Update for awsbatch scheduler is not supported.
     QueueUpdateStrategy can override UpdatePolicy of parameters under SlurmQueues for slurm scheduler.
     """
     if is_awsbatch_scheduler(change, patch):
         return False
+    if patch.cluster.has_running_login_nodes():
+        return False
     result = not patch.cluster.has_running_capacity()
     if is_slurm_scheduler(patch) and not is_stop_required_for_shared_storage(change):
         result = result or is_queue_update_strategy_set(patch)
 
     return result
 
 
+def condition_checker_login_nodes_pools_policy(change, _):
+    """Login fleet stop is required when a login pool is removed."""
+    return not is_login_pool_removed(change)
+
+
+def is_login_pool_removed(change):
+    return change.is_list and change.key == "Pools" and change.old_value is not None and change.new_value is None
+
+
+def condition_checker_login_nodes_stop_policy(_, patch):
+    return not patch.cluster.has_running_login_nodes()
+
+
 # Common fail_reason messages
 UpdatePolicy.FAIL_REASONS = {
     "ebs_volume_resize": "Updating the file system after a resize operation requires commands specific to your "
     "operating system.",
     "cookbook_update": lambda change, patch: (
         "Updating cookbook related parameter is not supported because it only "
         "applies updates to compute nodes. If you still want to proceed, first stop the compute fleet with the "
         "pcluster update-compute-fleet command and then run an update with the --force-update flag"
     ),
+    "login_nodes_running": lambda change, patch: "The update is not supported when login nodes are running",
+    "compute_or_login_nodes_running": lambda change, patch: (
+        "The update is not supported when compute or login nodes are running"
+    ),
 }
 
 # Common action_needed messages
 UpdatePolicy.ACTIONS_NEEDED = {
     "ebs_volume_update": "Follow the instructions at {0}#{1} to modify your volume from AWS Console.".format(
         "https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/requesting-ebs-volume-modifications.html",
         "modify-ebs-volume",
     ),
     "pcluster_stop": lambda change, patch: "Stop the compute fleet with the pcluster update-compute-fleet command",
     "pcluster_stop_conditional": actions_needed_queue_update_strategy,
     "managed_placement_group": actions_needed_managed_placement_group,
     "shared_storage_update_conditional": actions_needed_shared_storage_update,
     "managed_fsx": actions_needed_managed_fsx,
+    "login_nodes_stop": lambda change, patch: (
+        "Stop the login nodes by setting Count parameter to 0 "
+        "and update the cluster with the pcluster update-cluster command"
+    ),
 }
 
 # Base policies
 
 # Update is ignored
 UpdatePolicy.IGNORED = UpdatePolicy(
     name="IGNORED",
@@ -522,7 +546,42 @@
 UpdatePolicy.MANAGED_FSX = UpdatePolicy(
     name="MANAGED_FSX",
     level=6,
     fail_reason=fail_reason_managed_fsx,
     action_needed=UpdatePolicy.ACTIONS_NEEDED["managed_fsx"],
     condition_checker=condition_checker_managed_fsx,
 )
+
+
+# Update policy for updating LoginNodes / Pools
+UpdatePolicy.LOGIN_NODES_POOLS = UpdatePolicy(
+    name="LOGIN_NODES_POOLS_UPDATE_POLICY",
+    level=6,
+    condition_checker=condition_checker_login_nodes_pools_policy,
+    fail_reason=UpdatePolicy.FAIL_REASONS["login_nodes_running"],
+    action_needed=UpdatePolicy.ACTIONS_NEEDED["login_nodes_stop"],
+)
+
+# Update supported only with all login nodes down
+UpdatePolicy.LOGIN_NODES_STOP = UpdatePolicy(
+    name="LOGIN_NODES_STOP",
+    level=10,
+    condition_checker=condition_checker_login_nodes_stop_policy,
+    fail_reason=UpdatePolicy.FAIL_REASONS["login_nodes_running"],
+    action_needed=UpdatePolicy.ACTIONS_NEEDED["login_nodes_stop"],
+)
+
+
+# Update supported only with all computre and login nodes down
+UpdatePolicy.COMPUTE_AND_LOGIN_NODES_STOP = UpdatePolicy(
+    name="COMPUTE_AND_LOGIN_NODES_STOP",
+    level=10,
+    condition_checker=lambda change, patch: (
+        UpdatePolicy.COMPUTE_FLEET_STOP.condition_checker(change, patch)
+        and UpdatePolicy.LOGIN_NODES_STOP.condition_checker(change, patch)
+    ),
+    fail_reason=UpdatePolicy.FAIL_REASONS["compute_or_login_nodes_running"],
+    action_needed=lambda change, patch: "{}. {}".format(
+        UpdatePolicy.COMPUTE_FLEET_STOP.action_needed(change, patch),
+        UpdatePolicy.LOGIN_NODES_STOP.action_needed(change, patch),
+    ),
+)
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/constants.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,52 +6,51 @@
 # http://aws.amazon.com/apache2.0/
 #
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 from enum import Enum
 
-from pkg_resources import packaging
-
 PCLUSTER_NAME_MAX_LENGTH = 60
 # When Slurm accounting is enabled, Slurm creates database tables with the format 'cluster_name' + 'suffix'.
 # MySQL and MariaDB have a maximum table name length of 64 characters.
 # The longest suffix used by Slurm is 24 chars, therefore the cluster name must be at most 40 chars long.
 PCLUSTER_NAME_MAX_LENGTH_SLURM_ACCOUNTING = 40
 PCLUSTER_NAME_REGEX = r"^([a-zA-Z][a-zA-Z0-9-]{0,%d})$"
 PCLUSTER_ISSUES_LINK = "https://github.com/aws/aws-parallelcluster/issues"
+PCLUSTER_AMI_ID_REGEX = r"^ami-[0-9a-z]{8}$|^ami-[0-9a-z]{17}$"
 
 CIDR_ALL_IPS = "0.0.0.0/0"
 
 SUPPORTED_SCHEDULERS = ["slurm", "awsbatch"]
-SCHEDULERS_SUPPORTING_IMDS_SECURED = ["slurm", "plugin"]
-SUPPORTED_OSES = ["alinux2", "centos7", "ubuntu1804", "ubuntu2004", "rhel8"]
-SUPPORTED_OSES_FOR_SCHEDULER = {"slurm": SUPPORTED_OSES, "plugin": SUPPORTED_OSES, "awsbatch": ["alinux2"]}
+SCHEDULERS_SUPPORTING_IMDS_SECURED = ["slurm"]
+SUPPORTED_OSES = ["alinux2", "centos7", "ubuntu2004", "ubuntu2204", "rhel8"]
+SUPPORTED_OSES_FOR_SCHEDULER = {"slurm": SUPPORTED_OSES, "awsbatch": ["alinux2"]}
 DELETE_POLICY = "Delete"
 RETAIN_POLICY = "Retain"
 DELETION_POLICIES = [DELETE_POLICY, RETAIN_POLICY]
 DELETION_POLICIES_WITH_SNAPSHOT = DELETION_POLICIES + ["Snapshot"]
 SUPPORTED_ARCHITECTURES = ["x86_64", "arm64"]
 SUPPORTED_OSES_FOR_ARCHITECTURE = {"x86_64": SUPPORTED_OSES, "arm64": SUPPORTED_OSES}
 SLURM = "slurm"
 AWSBATCH = "awsbatch"
 
 OS_MAPPING = {
     "centos7": {"user": "centos"},
     "alinux2": {"user": "ec2-user"},
-    "ubuntu1804": {"user": "ubuntu"},
     "ubuntu2004": {"user": "ubuntu"},
+    "ubuntu2204": {"user": "ubuntu"},
     "rhel8": {"user": "ec2-user"},
 }
 
 OS_TO_IMAGE_NAME_PART_MAP = {
     "alinux2": "amzn2-hvm",
     "centos7": "centos7-hvm",
-    "ubuntu1804": "ubuntu-1804-lts-hvm",
     "ubuntu2004": "ubuntu-2004-lts-hvm",
+    "ubuntu2204": "ubuntu-2204-lts-hvm",
     "rhel8": "rhel8-hvm",
 }
 
 IMAGE_NAME_PART_TO_OS_MAP = {value: key for key, value in OS_TO_IMAGE_NAME_PART_MAP.items()}
 
 # Describe the list of requirements to be satisfied by the Pcluster AWS Batch CLI to manage the cluster.
 # It must be in the form <package-name><comparison-operator><version>
@@ -62,57 +61,68 @@
 
 FSX_SSD_THROUGHPUT = {"PERSISTENT_1": [50, 100, 200], "PERSISTENT_2": [125, 250, 500, 1000]}
 FSX_HDD_THROUGHPUT = [12, 40]
 
 LUSTRE = "LUSTRE"
 OPENZFS = "OPENZFS"
 ONTAP = "ONTAP"
+FILECACHE = "FILECACHE"
 
 FSX_LUSTRE = "FsxLustre"
 FSX_OPENZFS = "FsxOpenZfs"
 FSX_ONTAP = "FsxOntap"
+FSX_FILE_CACHE = "FsxFileCache"
 
 # https://docs.aws.amazon.com/fsx/latest/APIReference/API_DescribeVolumes.html#FSx-DescribeVolumes-request-VolumeIds.
 FSX_VOLUME_ID_REGEX = r"^fsvol-[0-9a-f]{17}$"
+# https://docs.aws.amazon.com/fsx/latest/APIReference/API_FileCacheCreating.html#FSx-Type-FileCacheCreating-FileCacheId:~:text=Pattern%3A-,%5E(fc%2D%5B0%2D9a%2Df%5D%7B8%2C%7D)%24,-Required%3A%20No
+FSX_FILE_CACHE_ID_REGEX = r"^(fc-[0-9a-f]{8,18})$"
 
 FSX_PORTS = {
     # Lustre Security group: https://docs.aws.amazon.com/fsx/latest/LustreGuide/limit-access-security-groups.html
     LUSTRE: {"tcp": [988]},
     # OpenZFS Security group: https://docs.aws.amazon.com/fsx/latest/OpenZFSGuide/limit-access-security-groups.html
     OPENZFS: {"tcp": [111, 2049, 20001, 20002, 20003], "udp": [111, 2049, 20001, 20002, 20003]},
     # Ontap Security group: https://docs.aws.amazon.com/fsx/latest/ONTAPGuide/limit-access-security-groups.html
     ONTAP: {"tcp": [111, 635, 2049, 4046], "udp": [111, 635, 2049, 4046]},
 }
 
+ALL_PORTS_RANGE = (0, 65535)
+SLURM_PORTS_RANGE = (6819, 6829)
+NFS_PORT = 2049
 EFS_PORT = 2049
 
 EBS_VOLUME_TYPE_IOPS_DEFAULT = {
     "io1": 100,
     "io2": 100,
     "gp3": 3000,
 }
 EBS_VOLUME_SIZE_DEFAULT = 35
 EBS_VOLUME_TYPE_DEFAULT = "gp3"
 EBS_VOLUME_TYPE_DEFAULT_US_ISO = "gp2"
 
 DEFAULT_MAX_COUNT = 10
 DEFAULT_MIN_COUNT = 0
 MAX_NUMBER_OF_QUEUES = 50
-SCHEDULER_PLUGIN_MAX_NUMBER_OF_QUEUES = 10
-SCHEDULER_PLUGIN_MAX_NUMBER_OF_COMPUTE_RESOURCES = 5
 # Allow for flexibility in how compute resources are distributed in the cluster
 MAX_NUMBER_OF_COMPUTE_RESOURCES_PER_CLUSTER = MAX_COMPUTE_RESOURCES_PER_QUEUE = 50
+MIN_SLURM_NODE_PRIORITY = 1
+MAX_SLURM_NODE_PRIORITY = 2**32 - 1  # max value of uint32_t
+
+# Thresholds used to trigger a warning if Memory Based Scheduling and Flexible Instance Types are used together
+MIN_MEMORY_ABSOLUTE_DIFFERENCE = 4096
+MIN_MEMORY_PRECENTAGE_DIFFERENCE = 0.20
 
 MAX_EBS_COUNT = 5
 MAX_NEW_STORAGE_COUNT = {"efs": 1, "fsx": 1, "raid": 1}
 MAX_EXISTING_STORAGE_COUNT = {"efs": 20, "fsx": 20, "raid": 0}
 
 COOKBOOK_PACKAGES_VERSIONS = {
-    "parallelcluster": "3.6.1",
-    "cookbook": "aws-parallelcluster-cookbook-3.6.1",
+    "parallelcluster": "3.7.0b1",
+    "cookbook": "aws-parallelcluster-cookbook-3.7.0b1",
     "chef": "17.2.29",
     "berkshelf": "7.2.0",
     "ami": "dev",
 }
 
 CW_DASHBOARD_ENABLED_DEFAULT = True
 CW_LOGS_ENABLED_DEFAULT = True
@@ -147,23 +157,23 @@
 # PCLUSTER_CLUSTER_NAME_TAG needs to be the same as the hard coded strings in node package
 # and in cleanup_resource.py used by Lambda function
 PCLUSTER_CLUSTER_NAME_TAG = f"{PCLUSTER_PREFIX}cluster-name"
 # PCLUSTER_NODE_TYPE_TAG needs to be the same as the hard coded strings in node package
 PCLUSTER_NODE_TYPE_TAG = f"{PCLUSTER_PREFIX}node-type"
 PCLUSTER_QUEUE_NAME_TAG = f"{PCLUSTER_PREFIX}queue-name"
 PCLUSTER_COMPUTE_RESOURCE_NAME_TAG = f"{PCLUSTER_PREFIX}compute-resource-name"
+PCLUSTER_LOGIN_NODES_POOL_NAME_TAG = f"{PCLUSTER_PREFIX}login-nodes-pool-name"
 IMAGEBUILDER_ARN_TAG = "Ec2ImageBuilderArn"
 PCLUSTER_S3_ARTIFACTS_DICT = {
     "root_directory": "parallelcluster",
     "root_cluster_directory": "clusters",
     "source_config_name": "cluster-config.yaml",
     "image_config_name": "image-config.yaml",
     "config_name": "cluster-config-with-implied-values.yaml",
     "template_name": "aws-parallelcluster.cfn.yaml",
-    "scheduler_plugin_template_name": "scheduler-plugin-substack.cfn",
     "instance_types_data_name": "instance-types-data.json",
     "custom_artifacts_name": "artifacts.zip",
     "scheduler_resources_name": "scheduler_resources.zip",
     "change_set_name": "change-set.json",
 }
 
 PCLUSTER_TAG_VALUE_REGEX = r"^([\w\+\-\=\.\_\:\@/]{0,256})$"
@@ -199,25 +209,20 @@
     "us-isob-east-1",
     "us-gov-east-1",
     "us-gov-west-1",
     "us-west-1",
     "us-west-2",
 ]
 
-SCHEDULER_PLUGIN_MAX_NUMBER_OF_USERS = 10
-
 # see https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html
 NODEJS_MIN_VERSION = "10.13.0"
 NODEJS_INCOMPATIBLE_VERSION_RANGE = ["13.0.0", "13.6.0"]
 
 NODE_BOOTSTRAP_TIMEOUT = 1800
 
-SCHEDULER_PLUGIN_INTERFACE_VERSION = packaging.version.Version("1.0")
-SCHEDULER_PLUGIN_INTERFACE_VERSION_LOW_RANGE = packaging.version.Version("1.0")
-
 # DirectoryService
 DIRECTORY_SERVICE_RESERVED_SETTINGS = {"id_provider": "ldap"}
 
 DEFAULT_EPHEMERAL_DIR = "/scratch"
 
 LAMBDA_VPC_ACCESS_MANAGED_POLICY = "arn:${AWS::Partition}:iam::aws:policy/service-role/AWSLambdaVPCAccessExecutionRole"
 
@@ -236,24 +241,26 @@
     We do not expect this enumeration to list all the features,
     but at least those that are considered for feature flagging.
     """
 
     BATCH = "AWS Batch scheduler"
     DCV = "NICE DCV"
     FSX_LUSTRE = "FSx Lustre"
+    FSX_FILE_CACHE = "FSx FileCache"
     FSX_ONTAP = "FSx ONTAP"
     FSX_OPENZFS = "FSx OpenZfs"
     SLURM_DATABASE = "SLURM Database"
     CLUSTER_HEALTH_METRICS = "Cluster Health Metrics"
 
 
 UNSUPPORTED_FEATURES_MAP = {
     Feature.BATCH: ["ap-northeast-3", "us-iso"],
     Feature.DCV: ["us-iso"],
     Feature.FSX_LUSTRE: ["us-iso"],
+    Feature.FSX_FILE_CACHE: ["us-iso"],
     Feature.FSX_ONTAP: ["us-iso"],
     Feature.FSX_OPENZFS: ["us-iso"],
     Feature.SLURM_DATABASE: [],
     Feature.CLUSTER_HEALTH_METRICS: ["us-iso"],
 }
 
 
@@ -305,7 +312,11 @@
     Operation.EXPORT_IMAGE_LOGS: ["us-iso"],
     Operation.GET_IMAGE_LOG_EVENTS: ["us-iso"],
     Operation.GET_IMAGE_STACK_EVENTS: ["us-iso"],
     Operation.LIST_IMAGE_LOG_STREAMS: ["us-iso"],
 }
 
 MAX_TAGS_COUNT = 40  # Tags are limited to 50, reserve some tags for parallelcluster specified tags
+
+IAM_ROLE_REGEX = "^arn:.*:role/"
+IAM_INSTANCE_PROFILE_REGEX = "^arn:.*:instance-profile/"
+IAM_POLICY_REGEX = "^arn:.*:policy/"
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/imagebuilder_utils.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/imagebuilder_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/launch_template_utils.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/launch_template_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/lib/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/lib/lib.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/lib/lib.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/models/cluster.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/models/cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,30 @@
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # This module contains all the classes representing the Resources objects.
 # These objects are obtained from the configuration file through a conversion based on the Schema classes.
 #
-import hashlib
 import json
 import logging
 import os
 import tempfile
 import time
 from copy import deepcopy
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Set, Tuple
-from urllib.request import urlopen
 
 import pkg_resources
-from jinja2 import BaseLoader
-from jinja2.sandbox import SandboxedEnvironment
 from marshmallow import ValidationError
 
-from pcluster.api.models import Metadata
 from pcluster.aws.aws_api import AWSApi
 from pcluster.aws.common import AWSClientError, BadRequestError, LimitExceededError, StackNotFoundError, get_region
-from pcluster.config.cluster_config import BaseClusterConfig, SchedulerPluginScheduling, Tag
+from pcluster.config.cluster_config import BaseClusterConfig, Tag
 from pcluster.config.common import ValidatorSuppressor
 from pcluster.config.config_patch import ConfigPatch
 from pcluster.constants import (
     PCLUSTER_CLUSTER_NAME_TAG,
     PCLUSTER_NODE_TYPE_TAG,
     PCLUSTER_QUEUE_NAME_TAG,
     PCLUSTER_S3_ARTIFACTS_DICT,
@@ -59,22 +54,22 @@
     NotFound,
     create_logs_archive,
     export_stack_events,
     parse_config,
     upload_archive,
 )
 from pcluster.models.compute_fleet_status_manager import ComputeFleetStatus, ComputeFleetStatusManager
-from pcluster.models.s3_bucket import S3Bucket, S3BucketFactory, S3FileFormat, create_s3_presigned_url, parse_bucket_url
+from pcluster.models.login_nodes_status import LoginNodesStatus
+from pcluster.models.s3_bucket import S3Bucket, S3BucketFactory, S3FileFormat, create_s3_presigned_url
 from pcluster.schemas.cluster_schema import ClusterSchema
 from pcluster.templates.cdk_builder import CDKTemplateBuilder
 from pcluster.templates.import_cdk import start as start_cdk_import
 from pcluster.utils import (
     datetime_to_epoch,
     generate_random_name_with_prefix,
-    get_attr,
     get_installed_version,
     grouper,
     yaml_load,
 )
 from pcluster.validators.common import FailureLevel, ValidationResult, ValidatorContext
 
 # pylint: disable=C0302
@@ -85,14 +80,15 @@
 
 
 class NodeType(Enum):
     """Enum that identifies the cluster node type."""
 
     HEAD_NODE = "HeadNode"
     COMPUTE = "Compute"
+    LOGIN_NODE = "LoginNode"
 
     def __str__(self):
         return str(self.value)
 
 
 class ClusterActionError(Exception):
     """Represent an error during the execution of an action on the cluster."""
@@ -172,14 +168,15 @@
         self.__bucket = None
         self.template_body = None
         self.__config = None
         self.__s3_artifact_dir = None
         self.__official_ami = None
         self.__has_running_capacity = None
         self.__running_capacity = None
+        self.__has_running_login_nodes = None
 
     @property
     def stack(self):
         """Return the ClusterStack object."""
         if not self.__stack:
             self.__stack = ClusterStack(AWSApi.instance().cfn.describe_stack(self.stack_name))
             self.__official_ami = self.__stack.official_ami
@@ -199,15 +196,15 @@
         if self.__s3_artifact_dir is None:
             self._get_artifact_dir()
         return self.__s3_artifact_dir
 
     @property
     def compute_fleet_status_manager(self) -> ComputeFleetStatusManager:
         """Return compute fleet status manager."""
-        return ComputeFleetStatusManager.get_manager(self.name, self.stack.version, self.stack.scheduler)
+        return ComputeFleetStatusManager.get_manager(self.name, self.stack.version)
 
     def _get_artifact_dir(self):
         """Get artifact directory in S3 bucket by stack output."""
         try:
             self.__s3_artifact_dir = self.stack.s3_artifact_directory
             if self.__s3_artifact_dir is None:
                 raise AWSClientError(
@@ -282,14 +279,24 @@
     @property
     def compute_fleet_status(self) -> ComputeFleetStatus:
         """Status of the cluster compute fleet."""
         status, _ = self.compute_fleet_status_with_last_updated_time
         return status
 
     @property
+    def login_nodes_status(self):
+        """Status of the login nodes pool."""
+        login_nodes_status = LoginNodesStatus(self.stack_name)
+        if self.stack.scheduler == "slurm" and self.config.login_nodes:
+            # This approach works since by design we have now only one pool.
+            # We should fix this if we want to add more than a login nodes pool per cluster.
+            login_nodes_status.retrieve_data(self.config.login_nodes.pools[0].name)
+        return login_nodes_status
+
+    @property
     def compute_fleet_status_with_last_updated_time(self) -> Tuple[ComputeFleetStatus, str]:
         """Status of the cluster compute fleet and the last compute fleet status updated time."""
         if self.stack.is_working_status or self.stack.status == "UPDATE_IN_PROGRESS":
             if self.stack.scheduler == "awsbatch":
                 status = ComputeFleetStatus(
                     AWSApi.instance().batch.get_compute_environment_state(self.stack.batch_compute_environment)
                 )
@@ -449,24 +456,22 @@
             return ClusterSchema(cluster_name=self.name).load(cluster_config)
         except ValidationError as e:
             # syntactic failure
             data = str(sorted(e.messages.items()) if isinstance(e.messages, dict) else e)
             validation_failures = [ValidationResult(data, FailureLevel.ERROR, validator_type="ConfigSchemaValidator")]
             raise ConfigValidationError("Invalid cluster configuration.", validation_failures=validation_failures)
 
-    def validate_create_request(self, validator_suppressors, validation_failure_level, dry_run=False):
+    def validate_create_request(self, validator_suppressors, validation_failure_level):
         """Validate a create cluster request."""
         self._validate_no_existing_stack()
         self.config, ignored_validation_failures = self._validate_and_parse_config(
             validator_suppressors=validator_suppressors,
             validation_failure_level=validation_failure_level,
             context=ValidatorContext(),
         )
-        if dry_run and isinstance(self.config.scheduling, SchedulerPluginScheduling):
-            self._render_and_upload_scheduler_plugin_template(dry_run=dry_run)
         return ignored_validation_failures
 
     def _validate_no_existing_stack(self):
         if AWSApi.instance().cfn.stack_exists(self.stack_name):
             raise BadRequestClusterActionError(f"Cluster {self.name} already exists.")
 
     def _validate_and_parse_config(
@@ -580,87 +585,22 @@
             # upload instance types data
             self.bucket.upload_config(
                 self.config.get_instance_types_data(),
                 PCLUSTER_S3_ARTIFACTS_DICT.get("instance_types_data_name"),
                 format=S3FileFormat.JSON,
             )
 
-            if isinstance(self.config.scheduling, SchedulerPluginScheduling):
-                self._render_and_upload_scheduler_plugin_template()
             LOGGER.info("Cluster artifacts uploaded correctly.")
         except BadRequestClusterActionError:
             raise
         except Exception as e:
             message = f"Unable to upload cluster resources to the S3 bucket {self.bucket.name} due to exception: {e}"
             LOGGER.error(message)
             raise _cluster_error_mapper(e, message)
 
-    def _render_and_upload_scheduler_plugin_template(self, dry_run=False):
-        scheduler_plugin_template = get_attr(
-            self.config, "scheduling.settings.scheduler_definition.cluster_infrastructure.cloud_formation.template"
-        )
-        if not scheduler_plugin_template:
-            return
-
-        try:
-            LOGGER.info("Downloading scheduler plugin CloudFormation template from %s", scheduler_plugin_template)
-            if scheduler_plugin_template.startswith("s3"):
-                bucket_parsing_result = parse_bucket_url(scheduler_plugin_template)
-                result = AWSApi.instance().s3.get_object(
-                    bucket_name=bucket_parsing_result["bucket_name"],
-                    key=bucket_parsing_result["object_key"],
-                    expected_bucket_owner=get_attr(
-                        self.config,
-                        "scheduling.settings.scheduler_definition.cluster_infrastructure.cloud_formation."
-                        "s3_bucket_owner",
-                    ),
-                )
-                file_content = result["Body"].read().decode("utf-8")
-            else:
-                # A nosec comment is appended to the following line in order to disable the B310 check.
-                # The urlopen argument is properly validated
-                # [B310:blacklist] Audit url open for permitted schemes.
-                with urlopen(scheduler_plugin_template) as f:  # nosec B310 nosemgrep
-                    file_content = f.read().decode("utf-8")
-        except Exception as e:
-            raise BadRequestClusterActionError(
-                f"Error while downloading scheduler plugin artifacts from '{scheduler_plugin_template}': {str(e)}"
-            ) from e
-
-        # checksum
-        self.validate_scheduler_plugin_template_checksum(file_content, scheduler_plugin_template)
-
-        # jinja rendering
-        try:
-            LOGGER.info("Rendering the following scheduler plugin CloudFormation template:\n%s", file_content)
-            environment = SandboxedEnvironment(loader=BaseLoader)
-            environment.filters["hash"] = (
-                # A nosec comment is appended to the following line in order to disable the B324 checks.
-                # The sha1 is used just as a hashing function.
-                # [B324:hashlib] Use of weak MD4, MD5, or SHA1 hash for security. Consider usedforsecurity=False
-                # [B303:blacklist] Use of insecure MD2, MD4, MD5, or SHA1 hash function
-                lambda value: hashlib.sha1(value.encode())  # nosec nosemgrep
-                .hexdigest()[0:16]
-                .capitalize()
-            )
-            template = environment.from_string(file_content)
-            rendered_template = template.render(
-                cluster_configuration=ClusterSchema(cluster_name=self.name).dump(deepcopy(self.config)),
-                cluster_name=self.name,
-                instance_types_info=self.config.get_instance_types_data(),
-            )
-        except Exception as e:
-            raise BadRequestClusterActionError(
-                f"Error while rendering scheduler plugin template '{scheduler_plugin_template}': {str(e)}"
-            ) from e
-        if not dry_run:
-            self.bucket.upload_cfn_template(
-                rendered_template, PCLUSTER_S3_ARTIFACTS_DICT["scheduler_plugin_template_name"], S3FileFormat.TEXT
-            )
-
     def delete(self, keep_logs: bool = True):
         """Delete cluster preserving log groups."""
         try:
             if keep_logs:
                 self._persist_cloudwatch_log_groups()
             self.stack.delete()
             self.__stack = ClusterStack(AWSApi.instance().cfn.describe_stack(self.stack_name))
@@ -790,14 +730,24 @@
                 self.__has_running_capacity = self.get_running_capacity() > 0
             else:
                 self.__has_running_capacity = (
                     self.compute_fleet_status_manager.get_status() != ComputeFleetStatus.STOPPED
                 )
         return self.__has_running_capacity
 
+    def has_running_login_nodes(self, updated_value: bool = False) -> bool:
+        """Return True if the cluster has running login nodes. Note: the value will be cached."""
+        if self.__has_running_login_nodes is None or updated_value:
+            self.__has_running_login_nodes = (
+                self.login_nodes_status.get_healthy_nodes() is not None
+                and self.login_nodes_status.get_unhealthy_nodes() is not None
+                and self.login_nodes_status.get_healthy_nodes() + self.login_nodes_status.get_unhealthy_nodes() != 0
+            )
+        return self.__has_running_login_nodes
+
     def get_running_capacity(self, updated_value: bool = False):
         """Return the number of instances or desired capacity. Note: the value will be cached."""
         if self.__running_capacity is None or updated_value:
             if self.stack.scheduler == "slurm":
                 self.__running_capacity = len(self.compute_instances)
             elif self.stack.scheduler == "awsbatch":
                 self.__running_capacity = AWSApi.instance().batch.get_compute_environment_capacity(
@@ -884,32 +834,26 @@
 
     def validate_update_request(
         self,
         target_source_config: str,
         validator_suppressors: Set[ValidatorSuppressor] = None,
         validation_failure_level: FailureLevel = FailureLevel.ERROR,
         force: bool = False,
-        dry_run: bool = False,
     ):
         """Validate a cluster update request."""
         self._validate_cluster_exists()
         self._validate_stack_status_not_in_progress()
         target_config, ignored_validation_failures = self._validate_and_parse_config(
             validator_suppressors=validator_suppressors,
             validation_failure_level=validation_failure_level,
             config_text=target_source_config,
             context=ValidatorContext(head_node_instance_id=self.head_node_instance.id, during_update=True),
         )
         changes = self._validate_patch(force, target_config)
 
-        self._validate_scheduling_update(changes, target_config)
-
-        if dry_run and isinstance(self.config.scheduling, SchedulerPluginScheduling):
-            self._render_and_upload_scheduler_plugin_template(dry_run=dry_run)
-
         return target_config, changes, ignored_validation_failures
 
     def _validate_patch(self, force, target_config):
         patch = ConfigPatch(
             cluster=self, base_config=self.config.source_config, target_config=target_config.source_config
         )
         patch_allowed, update_changes = patch.check()
@@ -1011,19 +955,14 @@
 
         # Add the tags
         self.config.tags += [Tag(key=tag_key, value=tag_value) for tag_key, tag_value in tags.items()]
 
     def _get_cfn_tags(self):
         """Return tag list in the format expected by CFN."""
         cluster_tags = [{"Key": tag.key, "Value": tag.value} for tag in self.config.tags]
-        if self.config.scheduling.scheduler == "plugin":
-            scheduler_plugin_tags = get_attr(self.config, "scheduling.settings.scheduler_definition.tags")
-            if scheduler_plugin_tags:
-                custom_scheduler_plugin_tags = [{"Key": tag.key, "Value": tag.value} for tag in scheduler_plugin_tags]
-                cluster_tags += custom_scheduler_plugin_tags
         return cluster_tags
 
     def export_logs(
         self,
         bucket: str,
         bucket_prefix: str = None,
         keep_s3_objects: bool = False,
@@ -1214,89 +1153,7 @@
                 raise NotFoundClusterActionError(f"The specified log stream {log_stream_name} does not exist.")
             raise _cluster_error_mapper(e, f"Unexpected error when retrieving log events: {e}.")
 
     @property
     def _stack_events_stream_name(self):
         """Return the name of the stack events log stream."""
         return STACK_EVENTS_LOG_STREAM_NAME_FORMAT.format(self.stack_name)
-
-    def _validate_scheduling_update(self, changes, target_config):
-        """Update of Scheduling is not supported when SupportsClusterUpdate of the scheduler plugin is set to false."""
-        # target_config.source_config.get("Scheduling") != self.config.source_config.get("Scheduling") doesn't mean
-        # there's changes in the config, if queue list in the scheduling dict has different order, target_config dict
-        # and original config dict may be different.
-        if (
-            self.config.scheduling.scheduler == "plugin"
-            and get_attr(self.config, "scheduling.settings.scheduler_definition.requirements.supports_cluster_update")
-            is False
-            and target_config.source_config.get("Scheduling") != self.config.source_config.get("Scheduling")
-        ):
-            scheduling_changes = []
-            # Example format of changes:
-            # changes = [
-            #     ["param_path", "parameter", "old value", "new value", "check", "reason", "action_needed"],
-            #     [
-            #         ["HeadNode", "Iam"],
-            #         "AdditionalIamPolicies",
-            #         None,
-            #         {"Policy": "arn:aws:iam::aws:policy/FakePolicy"},
-            #         "SUCCEEDED",
-            #         "-",
-            #         None,
-            #     ],
-            #     [
-            #         ["HeadNode", "Iam"],
-            #         "AdditionalIamPolicies",
-            #         {"Policy": "arn:aws:iam::aws:policy/AmazonS3ReadOnlyAccess"},
-            #         None,
-            #         "SUCCEEDED",
-            #         "-",
-            #         None,
-            #     ],
-            #     [
-            #         ["Scheduling", "SchedulerQueues[queue1]", "ComputeResources[compute-resource1]"],
-            #         "InstanceType",
-            #         "c5.2xlarge",
-            #         "c5.xlarge",
-            #         "SUCCEEDED",
-            #         "-",
-            #         None,
-            #     ],
-            # ]
-
-            # The first element of changes is:
-            # ["param_path", "parameter", "old value", "new value", "check", "reason", "action_needed"]
-            for change in changes[1:]:
-                if change[0][0] == "Scheduling":  # check if the param_path of the change start from Scheduling
-                    scheduling_changes.append(change)
-            if len(scheduling_changes) >= 1:
-                raise ClusterUpdateError(
-                    "Update failure: The scheduler plugin used for this cluster does not support updating the "
-                    "scheduling configuration.",
-                    [changes[0]] + scheduling_changes,
-                )
-
-    def validate_scheduler_plugin_template_checksum(self, file_content, scheduler_plugin_template):
-        """Validate scheduler plugin template checksum match the expected checksum."""
-        checksum = get_attr(
-            self.config, "scheduling.settings.scheduler_definition.cluster_infrastructure.cloud_formation.checksum"
-        )
-        if checksum:
-            actual_checksum = hashlib.sha256(file_content.encode()).hexdigest()
-            if actual_checksum != checksum:
-                raise BadRequestClusterActionError(
-                    f"Error when validating scheduler plugin template '{scheduler_plugin_template}': "
-                    f"checksum: {actual_checksum} does not match expected one: {checksum}"
-                )
-
-    def get_plugin_metadata(self):
-        """Get the metadata name and version used for the response of DescribeCluster when the scheduler is plugin."""
-        try:
-            full_metadata = get_attr(self.config, "scheduling.settings.scheduler_definition.metadata")
-            return (
-                Metadata(name=full_metadata.get("Name"), version=full_metadata.get("Version"))
-                if full_metadata
-                else None
-            )
-        except ClusterActionError:
-            LOGGER.warning("Unable to retrieve scheduler metadata from cluster configuration.")
-            return None
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/models/cluster_resources.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/models/cluster_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,30 +149,32 @@
                 "OnNodeStartFailure", "Failed to run OnNodeStart script.", "Failed to run OnNodeStart script"
             ),
             ClusterCreationFailure("EbsMountFailure", "Failed to mount EBS volume.", "Failed to mount EBS volume"),
             ClusterCreationFailure("EfsMountFailure", "Failed to mount EFS.", "Failed to mount EFS"),
             ClusterCreationFailure("FsxMountFailure", "Failed to mount FSX.", "Failed to mount FSX"),
             ClusterCreationFailure("RaidMountFailure", "Failed to mount RAID array.", "Failed to mount RAID array"),
             ClusterCreationFailure(
-                "HeadNodeBootstrapFailure", "Failed to set up the head node.", "configured scheduler plugin"
-            ),
-            ClusterCreationFailure(
                 "HeadNodeBootstrapFailure", "Failed to set up the head node.", "Failed to run chef recipe"
             ),
             ClusterCreationFailure(
                 "HeadNodeBootstrapFailure", "Failed to bootstrap the head node.", "Failed to bootstrap the head node"
             ),
             ClusterCreationFailure(
                 "ResourceCreationFailure",
                 "Failed to create resources for head node bootstrap.",
                 "Resource creation cancelled",
             ),
             ClusterCreationFailure(
                 "HeadNodeBootstrapFailure", "Cluster creation timed out.", "WaitCondition timed out"
             ),
+            ClusterCreationFailure(
+                "StaticNodeBootstrapFailure",
+                "Cluster has been set to PROTECTED mode due to failures detected in static node provisioning.",
+                "Cluster has been set to PROTECTED mode due to failures detected in static node provisioning",
+            ),
         ]
 
         general_failure = failure = ClusterCreationFailure(
             "ClusterCreationFailure", "Failed to create the cluster.", ""
         )
         cfn_failure_reason = self._get_failure_reason()
         if cfn_failure_reason:
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/models/common.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/models/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/models/compute_fleet_status_manager.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/models/compute_fleet_status_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,17 +140,17 @@
     def get_status_with_last_updated_time(
         self, status_fallback=ComputeFleetStatus.UNKNOWN, last_updated_time_fallback=None
     ):
         """Get compute fleet status and the last compute fleet status updated time."""
         pass
 
     @staticmethod
-    def get_manager(cluster_name, version, scheduler):
+    def get_manager(cluster_name, version):
         """Return compute fleet status manager based on version and plugin."""
-        if packaging.version.parse(version) < packaging.version.parse("3.2.0a0") and scheduler != "plugin":
+        if packaging.version.parse(version) < packaging.version.parse("3.2.0a0"):
             return PlainTextComputeFleetStatusManager(cluster_name)
         else:
             return JsonComputeFleetStatusManager(cluster_name)
 
     @staticmethod
     def _timeout_expired(start_time, timeout):
         return (time.time() - start_time) > timeout
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/models/imagebuilder.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/models/imagebuilder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/models/imagebuilder_resources.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/models/imagebuilder_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/models/s3_bucket.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/models/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/networking/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/networking/vpc_factory.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/networking/vpc_factory.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/alinux2/Dockerfile` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/alinux2/Dockerfile`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/build-docker-images.sh` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/build-docker-images.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/buildspec.yml` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/buildspec.yml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/scripts/entrypoint.sh` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/scripts/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/scripts/mount_efs.sh` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/scripts/mount_efs.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/batch/docker/upload-docker-images.sh` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/batch/docker/upload-docker-images.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/compute_node/user_data.sh` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/compute_node/user_data.sh`

 * *Files 6% similar despite different names*

```diff
@@ -140,14 +140,28 @@
         export HOME="/tmp"
         for d in `ls /tmp/cookbooks`; do
           cd /tmp/cookbooks/$d
           LANG=en_US.UTF-8 /opt/cinc/embedded/bin/berks vendor /etc/chef/cookbooks --delete || error_exit 'Vendoring cookbook failed.'
         done;
         export HOME="${!HOME_BAK}"
       }
+
+      function publish_startup_time
+      {
+        start_time=$1
+        end_time=$2
+        # Only put the startup time data if the scheduler is slurm
+        slurm_node_path=/etc/parallelcluster/slurm_plugin/slurm_node_spec.json
+        if test -f "$slurm_node_path"; then
+            INSTANCE_ID=$(cat $slurm_node_path | jq -r .instance_id)
+            INSTANCE_TYPE=$(cat $slurm_node_path | jq -r .'compute."instance-type"')
+            aws cloudwatch put-metric-data --namespace "ParallelCluster" --metric-name "StartupTime" --value $(($end_time-$start_time)) --dimensions "InstanceID=${!INSTANCE_ID},InstanceType=${!INSTANCE_TYPE},ClusterName=${ClusterName}" --region "${AWS::Region}"
+        fi
+      }
+
       [ -f /etc/profile.d/proxy.sh ] && . /etc/profile.d/proxy.sh
 
       # Configure AWS CLI using the expected overrides, if any.
       [ -f /etc/profile.d/aws-cli-default-config.sh ] && . /etc/profile.d/aws-cli-default-config.sh
 
       custom_cookbook=${CustomChefCookbook}
       export _region=${AWS::Region}
@@ -189,29 +203,40 @@
         curl --retry 3 -v -L -o /etc/chef/aws-parallelcluster-cookbook.tgz ${!cookbook_url}
         vendor_cookbook
       fi
       cd /tmp
 
       mkdir -p /etc/chef/ohai/hints
       touch /etc/chef/ohai/hints/ec2.json
+
+      # measure start time
+      start=$(date +%s)
+
       jq --argfile f1 /tmp/dna.json --argfile f2 /tmp/extra.json -n '$f1 * $f2' > /etc/chef/dna.json || ( echo "jq not installed or invalid extra_json"; cp /tmp/dna.json /etc/chef/dna.json)
       {
         pushd /etc/chef &&
-        cinc-client --local-mode --config /etc/chef/client.rb --log_level info --force-formatter --no-color --chef-zero-port 8889 --json-attributes /etc/chef/dna.json --override-runlist aws-parallelcluster::init &&
+        cinc-client --local-mode --config /etc/chef/client.rb --log_level info --force-formatter --no-color --chef-zero-port 8889 --json-attributes /etc/chef/dna.json --override-runlist aws-parallelcluster-entrypoints::init &&
         /opt/parallelcluster/scripts/fetch_and_run -preinstall &&
-        cinc-client --local-mode --config /etc/chef/client.rb --log_level info --force-formatter --no-color --chef-zero-port 8889 --json-attributes /etc/chef/dna.json --override-runlist aws-parallelcluster::config &&
+        cinc-client --local-mode --config /etc/chef/client.rb --log_level info --force-formatter --no-color --chef-zero-port 8889 --json-attributes /etc/chef/dna.json --override-runlist aws-parallelcluster-entrypoints::config &&
         /opt/parallelcluster/scripts/fetch_and_run -postinstall &&
-        cinc-client --local-mode --config /etc/chef/client.rb --log_level info --force-formatter --no-color --chef-zero-port 8889 --json-attributes /etc/chef/dna.json --override-runlist aws-parallelcluster::finalize &&
+        cinc-client --local-mode --config /etc/chef/client.rb --log_level info --force-formatter --no-color --chef-zero-port 8889 --json-attributes /etc/chef/dna.json --override-runlist aws-parallelcluster-entrypoints::finalize &&
         popd
       } || error_exit 'Failed to run bootstrap recipes. If --norollback was specified, check /var/log/cfn-init.log and /var/log/cloud-init-output.log.'
 
       if [ ! -f /opt/parallelcluster/.bootstrapped ]; then
         echo ${!cookbook_version} | tee /opt/parallelcluster/.bootstrapped
       fi
 
+      # measure end time
+      end=$(date +%s)
+
+      if [ "${ComputeStartupTimeMetricEnabled}" = "True" ]; then
+        publish_startup_time $start $end || echo "[WARNING] failed to push the StartupTime metric to CloudWatch."
+      fi
+
 --==BOUNDARY==
 Content-Type: text/x-shellscript; charset="us-ascii"
 MIME-Version: 1.0
 
 #!/bin/bash -x
 
 function error_exit
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/head_node/user_data.sh` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/head_node/user_data.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/imagebuilder/custom_script.yaml` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/imagebuilder/custom_script.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/imagebuilder/parallelcluster.yaml` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/imagebuilder/parallelcluster.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
           commands:
             - |
               set -v
               CINC_URL="https://${AWS::Region}-aws-parallelcluster.s3.${AWS::Region}.${AWS::URLSuffix}/archives/cinc/cinc-install-1.1.0.sh"
               [ -n "${CfnParamCincInstaller}" ] && CINC_URL="${CfnParamCincInstaller}"
               echo "${!CINC_URL}"
 
-      # Check input base AMI OS and get OS information, the output should be like centos.7 | amzn.2 | ubuntu.18.04 | ubuntu.20.04 | rhel.8.7
+      # Check input base AMI OS and get OS information, the output should be like centos.7 | amzn.2 | ubuntu.20.04 | ubuntu.22.04 | rhel.8.7
       - name: OperatingSystemRelease
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               FILE=/etc/os-release
@@ -82,18 +82,18 @@
               set -v
               RELEASE='{{ build.OperatingSystemRelease.outputs.stdout }}'
 
               if [ `echo "${!RELEASE}" | grep -w '^amzn\.2'` ]; then
                 OS='alinux2'
               elif [ `echo "${!RELEASE}" | grep '^centos\.7'` ]; then
                 OS='centos7'
-              elif [ `echo "${!RELEASE}" | grep '^ubuntu\.18'` ]; then
-                OS='ubuntu1804'
               elif [ `echo "${!RELEASE}" | grep '^ubuntu\.20'` ]; then
                 OS='ubuntu2004'
+              elif [ `echo "${!RELEASE}" | grep '^ubuntu\.22'` ]; then
+                OS='ubuntu2204'
               elif [ `echo "${!RELEASE}" | grep '^rhel\.8'` ]; then
                 OS='rhel8'
               else
                 echo "Operating System '${!RELEASE}' is not supported. Failing build."
                 exit {{ FailExitCode }}
               fi
 
@@ -147,18 +147,18 @@
               if [ ${CfnParamUpdateOsAndReboot} == false ]; then
                 RELEASE='{{ build.OperatingSystemRelease.outputs.stdout }}'
                 if [ `echo "${!RELEASE}" | grep -Ev '^(amzn|centos|ubuntu|rhel)'` ]; then
                   echo "This component does not support '${!RELEASE}'. Failing build."
                   exit {{ FailExitCode }}
                 fi
 
-                # This component only supports aarch64 CPUs on Amazon Linux 2, Ubuntu1804, Ubuntu2004, Centos7 and RHEL8
+                # This component only supports aarch64 CPUs on Amazon Linux 2, Ubuntu2004, Ubuntu2204, Centos7 and RHEL8
                 ARCH=$(uname -m)
                 if [[ `echo ${!ARCH}` == 'aarch64' ]]; then
-                  if [ `echo "${!RELEASE}" | grep -Ev '^(amzn\.2|centos\.7|ubuntu\.18\.04|ubuntu\.20\.04|rhel\.8)'` ]; then
+                  if [ `echo "${!RELEASE}" | grep -Ev '^(amzn\.2|centos\.7|ubuntu\.20\.04|ubuntu\.22\.04|rhel\.8)'` ]; then
                     echo "This component does not support '${!RELEASE}' on ARM64 CPUs. Failing build."
                     exit {{ FailExitCode }}
                   fi
                 fi
               fi
 
       # Install prerequisite OS packages
@@ -257,15 +257,15 @@
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               echo "Calling chef-client with /etc/parallelcluster/image_dna.json"
               cat /etc/parallelcluster/image_dna.json
-              cinc-client --local-mode --config /etc/chef/client.rb --log_level info --force-formatter --no-color --chef-zero-port 8889 --json-attributes /etc/parallelcluster/image_dna.json --override-runlist aws-parallelcluster::default
+              cinc-client --local-mode --config /etc/chef/client.rb --log_level info --force-formatter --no-color --chef-zero-port 8889 --json-attributes /etc/parallelcluster/image_dna.json --override-runlist aws-parallelcluster-entrypoints::install
 
       - name: CreateBootstrapFile
         action: CreateFile
         inputs:
           - path: /opt/parallelcluster/.bootstrapped
             content: |
               {{ build.PClusterCookbookVersionName.outputs.stdout }}
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -45,18 +45,18 @@
                 RELEASE="${ID}${VERSION_ID:+.${VERSION_ID}}"
               fi
 
               if [ $(echo "${RELEASE}" | grep -w '^amzn\.2') ]; then
                 OS='alinux2'
               elif [ $(echo "${RELEASE}" | grep '^centos\.7') ]; then
                 OS='centos7'
-              elif [ $(echo "${RELEASE}" | grep '^ubuntu\.18') ]; then
-                OS='ubuntu1804'
               elif [ $(echo "${RELEASE}" | grep '^ubuntu\.20') ]; then
                 OS='ubuntu2004'
+              elif [ $(echo "${RELEASE}" | grep '^ubuntu\.22') ]; then
+                OS='ubuntu2204'
               elif [ $(echo "${RELEASE}" | grep '^rhel\.8') ]; then
                 OS='rhel8'
               fi
 
               echo ${OS}
 
       - name: ParallelClusterTag
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -34,18 +34,18 @@
               set -v
               RELEASE='{{ validate.OperatingSystemRelease.outputs.stdout }}'
 
               if [ `echo "${RELEASE}" | grep -w '^amzn\.2'` ]; then
                 OS='alinux2'
               elif [ `echo "${RELEASE}" | grep '^centos\.7'` ]; then
                 OS='centos7'
-              elif [ `echo "${RELEASE}" | grep '^ubuntu\.18'` ]; then
-                OS='ubuntu1804'
               elif [ `echo "${RELEASE}" | grep '^ubuntu\.20'` ]; then
                 OS='ubuntu2004'
+              elif [ `echo "${RELEASE}" | grep '^ubuntu\.22'` ]; then
+                OS='ubuntu2204'
               elif [ `echo "${RELEASE}" | grep '^rhel\.8'` ]; then
                 OS='rhel8'
               else
                 echo "Operating System '${RELEASE}' is not supported. Failing build." && exit 1
               fi
 
               echo ${OS}
@@ -104,22 +104,14 @@
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} != 'arm64' ]] && echo "true" || echo "false"
 
-      - name: ArmPLSupported
-        action: ExecuteBash
-        inputs:
-          commands:
-            - |
-              set -v
-              [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} == 'arm64' ]] && echo "true" || echo "false"
-
       - name: FabricManagerSupported
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               [[ {{ validate.OperatingSystemArchitecture.outputs.stdout }} == 'arm64' ]] && echo "false" || echo "true"
@@ -128,15 +120,15 @@
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               ARCHITECTURE='{{ validate.OperatingSystemArchitecture.outputs.stdout }}'
               OS='{{ validate.OperatingSystemName.outputs.stdout }}'
-              if [ ${ARCHITECTURE} == 'arm64' ] && [[ ${OS} =~ ^(ubuntu(18|20)04|alinux2|rhel8)$ ]] || [ ${ARCHITECTURE} == 'x86_64' ]; then
+              if [ ${ARCHITECTURE} == 'arm64' ] && [[ ${OS} =~ ^(ubuntu(20|22)04|alinux2|rhel8)$ ]] || [ ${ARCHITECTURE} == 'x86_64' ]; then
                 echo "true"
               else
                 echo "false"
               fi
 
       ### versions ###
       - name: MungeVersion
@@ -195,39 +187,24 @@
                 PATTERN=$(jq '.default.cluster.nvidia.cuda_samples_version' {{ CookbookDefaultFile }})
                 VERSION=$(echo ${PATTERN} | tr -d '\n' | cut -d = -f 2 | xargs)
                 echo cuda-samples-${VERSION}/bin
               else
                 echo cuda-${cuda_ver}/samples/bin
               fi
 
-      - name: ArmPLVersion
+      ### utils ###
+      - name: PatchInSpecProfiles
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
-              PATTERN=$(jq '.default.cluster.armpl.major_minor_version' {{ CookbookDefaultFile }})
-              MAJOR_MINOR_VERSION=$(echo ${PATTERN} | tr -d '\n' | cut -d = -f 2 | xargs)
-              VERSION+="${MAJOR_MINOR_VERSION}."
-              PATTERN=$(jq '.default.cluster.armpl.patch_version' {{ CookbookDefaultFile }})
-              PATCH_VERSION=$(echo ${PATTERN} | tr -d '\n' | cut -d = -f 2 | xargs)
-              VERSION+="${PATCH_VERSION}"
-              echo ${VERSION}
+              sed -Ei "s#path: cookbooks/aws-parallelcluster#path: /etc/chef/cookbooks/aws-parallelcluster#g" /etc/chef/cookbooks/aws-parallelcluster-*/test/inspec.yml
+              echo "InSpec profiles patched"
 
-      - name: ArmPLGCCVersion
-        action: ExecuteBash
-        inputs:
-          commands:
-            - |
-              set -v
-              PATTERN=$(jq '.default.cluster.armpl.gcc.major_minor_version' {{ CookbookDefaultFile }})
-              VERSION=$(echo ${PATTERN} | tr -d '\n' | cut -d = -f 2 | xargs)
-              echo ${VERSION}
-
-      ### utils ###
       - name: NvidiaEnabled
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               NVIDIA_ENABLED=$(cat /etc/parallelcluster/image_dna.json | jq -r '.cluster.nvidia.enabled')
@@ -343,43 +320,19 @@
               set -vx
               OS='{{ validate.OperatingSystemName.outputs.stdout }}'
 
               if [ {{ validate.LustreSupported.outputs.stdout }} == true ]; then
                 echo "Checking for Lustre client..."
                 if [ ${OS} == centos7 ]; then
                   rpm -qa | grep lustre-client
-                elif [ ${OS} == ubuntu1804 ]; then
-                  dpkg -l | grep lustre
                 fi
               fi
               [[ $? -ne 0 ]] && echo "Check for Lustre client failed" && exit 1
               echo "FSx Lustre test passed"
 
-      - name: ArmPL
-        action: ExecuteBash
-        inputs:
-          commands:
-            - |
-              set -vx
-              if [ {{ validate.ArmPLSupported.outputs.stdout }} == true ]; then
-                echo "Checking gcc version and module loaded..."
-                unset MODULEPATH
-                source /etc/profile.d/modules.sh
-                (module avail)2>&1 | grep armpl/{{ validate.ArmPLVersion.outputs.stdout }}
-                [[ $? -ne 0 ]] && echo "Check armpl version failed" && exit 1
-                module load armpl/{{ validate.ArmPLVersion.outputs.stdout }}
-                gcc --version | grep {{ validate.ArmPLGCCVersion.outputs.stdout }}
-                [[ $? -ne 0 ]] && echo "Check gcc version for armpl failed" && exit 1
-                (module list)2>&1 | grep armpl/{{ validate.ArmPLVersion.outputs.stdout }}_gcc-{{ validate.ArmPLGCCVersion.outputs.stdout }}
-                [[ $? -ne 0 ]] && echo "Check armpl module failed" && exit 1
-                (module list)2>&1 | grep armpl/gcc-{{ validate.ArmPLGCCVersion.outputs.stdout }}
-                [[ $? -ne 0 ]] && echo "Check gcc module failed" && exit 1
-                echo "ArmPL test passed"
-              fi
-
       - name: Python
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -vx
               echo "Checking python3 installed..."
@@ -397,15 +350,79 @@
               if [ ${PLATFORM} != DEBIAN ]; then
                 echo "Checking dpkg is not installed on non-debian OS..."
                 if command -v dpkg &> /dev/null; then
                   echo "ERROR: dpkg found on non-Debian system" && exit 1
                 fi
                 echo "dpkg test passed"
               fi
-      - name: ChefValidations
+
+      - name: InSpecValidationsForAwsBatch
+        action: ExecuteBash
+        inputs:
+          commands:
+            - |
+              set -vx
+              echo "Performing InSpec validation for AwsBatch on the AMI..."
+              cd /etc/chef/cookbooks/aws-parallelcluster-awsbatch
+              inspec exec test --profiles-path . --controls /tag:install/ --no-distinct-exit
+              [[ $? -ne 0 ]] && echo "InSpec validation for AwsBatch failed" && exit 1
+              echo "InSpec validation for AwsBatch passed"
+
+      - name: InSpecValidationsForPlatform
+        action: ExecuteBash
+        inputs:
+          commands:
+            - |
+              set -vx
+              echo "Performing InSpec validation for platform on the AMI..."
+              cd /etc/chef/cookbooks/aws-parallelcluster-platform
+              inspec exec test --profiles-path . --controls /tag:install/ --no-distinct-exit
+              [[ $? -ne 0 ]] && echo "InSpec validation for platform failed" && exit 1
+              echo "InSpec validation for platform passed"
+
+      - name: InSpecValidationsForEnvironment
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -vx
+              echo "Performing InSpec validation for environment on the AMI..."
+              cd /etc/chef/cookbooks/aws-parallelcluster-environment
+              inspec exec test --profiles-path . --controls /tag:install/ --no-distinct-exit
+              [[ $? -ne 0 ]] && echo "InSpec validation for environment failed" && exit 1
+              echo "InSpec validation for environment passed"
 
-              cinc-client --local-mode --config /etc/chef/client.rb --log_level info --force-formatter --no-color --chef-zero-port 8889 --json-attributes /etc/parallelcluster/image_dna.json --override-runlist aws-parallelcluster::validations
+      - name: InSpecValidationsForComputeFleet
+        action: ExecuteBash
+        inputs:
+          commands:
+            - |
+              set -vx
+              echo "Performing InSpec validation for compute fleet on the AMI..."
+              cd /etc/chef/cookbooks/aws-parallelcluster-computefleet
+              inspec exec test --profiles-path . --controls /tag:install/ --no-distinct-exit
+              [[ $? -ne 0 ]] && echo "InSpec validation for compute fleet failed" && exit 1
+              echo "InSpec validation for compute fleet passed"
+
+      - name: InSpecValidationsForShared
+        action: ExecuteBash
+        inputs:
+          commands:
+            - |
+              set -vx
+              echo "Performing InSpec validation for shared cookbook on the AMI..."
+              cd /etc/chef/cookbooks/aws-parallelcluster-shared
+              inspec exec test --profiles-path . --controls /tag:install/ --no-distinct-exit
+              [[ $? -ne 0 ]] && echo "InSpec validation for shared cookbook failed" && exit 1
+              echo "InSpec validation for shared cookbook passed"
+
+      - name: InSpecValidationsForSlurm
+        action: ExecuteBash
+        inputs:
+          commands:
+            - |
+              set -vx
+              echo "Performing InSpec validation for Slurm on the AMI..."
+              cd /etc/chef/cookbooks/aws-parallelcluster-slurm
+              inspec exec test --profiles-path . --controls /tag:install/ --no-distinct-exit
+              [[ $? -ne 0 ]] && echo "InSpec validation for Slurm failed" && exit 1
+              echo "InSpec validation for slurm passed"
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/resources/imagebuilder/update_and_reboot.yaml` & `aws-parallelcluster-3.7.0b1/src/pcluster/resources/imagebuilder/update_and_reboot.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   - FailExitCode:
       type: string
       value: 1
 
 phases:
   - name: build
     steps:
-      # Check input base AMI OS and get OS information, the output should be like centos.7 | amzn.2 | ubuntu.18.04 | ubuntu.20.04 | rhel.8.7
+      # Check input base AMI OS and get OS information, the output should be like centos.7 | amzn.2 | ubuntu.20.04 | ubuntu.22.04 | rhel.8.7
       - name: OperatingSystemRelease
         action: ExecuteBash
         inputs:
           commands:
             - |
               set -v
               FILE=/etc/os-release
@@ -35,18 +35,18 @@
               set -v
               RELEASE='{{ build.OperatingSystemRelease.outputs.stdout }}'
 
               if [ `echo "${!RELEASE}" | grep -w '^amzn\.2'` ]; then
                 OS='alinux2'
               elif [ `echo "${!RELEASE}" | grep '^centos\.7'` ]; then
                 OS='centos7'
-              elif [ `echo "${!RELEASE}" | grep '^ubuntu\.18'` ]; then
-                OS='ubuntu1804'
               elif [ `echo "${!RELEASE}" | grep '^ubuntu\.20'` ]; then
                 OS='ubuntu2004'
+              elif [ `echo "${!RELEASE}" | grep '^ubuntu\.22'` ]; then
+                OS='ubuntu2204'
               elif [ `echo "${!RELEASE}" | grep '^rhel\.8'` ]; then
                 OS='rhel8'
               else
                 echo "Operating System '${!RELEASE}' is not supported. Failing build."
                 exit {{ FailExitCode }}
               fi
 
@@ -78,18 +78,18 @@
               set -v
               RELEASE='{{ build.OperatingSystemRelease.outputs.stdout }}'
               if [ `echo "${!RELEASE}" | grep -Ev '^(amzn|centos|ubuntu|rhel)'` ]; then
                 echo "This component does not support '${!RELEASE}'. Failing build."
                 exit {{ FailExitCode }}
               fi
 
-              # This component only supports aarch64 CPUs on Amazon Linux 2, Ubuntu1804, Ubuntu2004, Centos7 and RHEL 8
+              # This component only supports aarch64 CPUs on Amazon Linux 2, Ubuntu2004, Ubuntu2204, Centos7 and RHEL 8
               ARCH=$(uname -m)
               if [[ `echo ${!ARCH}` == 'aarch64' ]]; then
-                if [ `echo "${!RELEASE}" | grep -Ev '^(amzn\.2|centos\.7|ubuntu\.18\.04|ubuntu\.20\.04|rhel\.8)'` ]; then
+                if [ `echo "${!RELEASE}" | grep -Ev '^(amzn\.2|centos\.7|ubuntu\.20\.04|ubuntu\.22\.04|rhel\.8)'` ]; then
                   echo "This component does not support '${!RELEASE}' on ARM64 CPUs. Failing build."
                   exit {{ FailExitCode }}
                 fi
               fi
 
       - name: DisableNouveau
         action: ExecuteBash
@@ -125,25 +125,25 @@
             - |
               set -v
               OS='{{ build.OperatingSystemName.outputs.stdout }}'
               PLATFORM='{{ build.PlatformName.outputs.stdout }}'
 
               if [[ ${!PLATFORM} == RHEL ]]; then
                 yum -y update
-              
+
                 if [[ ${!OS} != "rhel8" ]]; then
                   package-cleanup -y --oldkernels --count=1
                 else
                   # package-cleanup has changed in RHEL8 and it works differently
                   # RHEL8 keeps at least 2 kernel for fallback reason https://access.redhat.com/solutions/1227
                   # The kernel cleanup should be performed manually
-              
+
                   # get the default kernel for the next boot
                   LAST_KERNEL_VERSION=$(grubby --default-kernel | sed -e "s/.*-\(4.18.0-.*\).$(uname -m)/\1/g")
-                  
+
                   # get all the installed kernel versions except the one for the next boot
                   KERNEL_VERSIONS_CLEANUP=$(rpm -q --qf "%{VERSION}-%{RELEASE}\n" kernel | grep -v "$LAST_KERNEL_VERSION")
                   for VERSION in $KERNEL_VERSIONS_CLEANUP; do
                     echo "Removing kernel-$VERSION kernel-core-$VERSION kernel-modules-$VERSION"
                     rpm -e kernel-$VERSION kernel-core-$VERSION kernel-modules-$VERSION;
                   done
                 fi
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/schemas/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/schemas/cluster_schema.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/schemas/cluster_schema.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,25 +11,20 @@
 
 #
 # This module contains all the classes representing the Schema of the configuration file.
 # These classes are created by following marshmallow syntax.
 #
 
 import copy
-import hashlib
 import logging
 import re
 from typing import List
-from urllib.request import urlopen
 
-from marshmallow import ValidationError, fields, post_load, pre_dump, pre_load, validate, validates, validates_schema
-from yaml import YAMLError
+from marshmallow import ValidationError, fields, post_load, pre_dump, validate, validates, validates_schema
 
-from pcluster.aws.aws_api import AWSApi
-from pcluster.aws.common import AWSClientError
 from pcluster.config.cluster_config import (
     AdditionalPackages,
     AllocationStrategy,
     AmiSearchFilters,
     AwsBatchClusterConfig,
     AwsBatchComputeResource,
     AwsBatchQueue,
@@ -48,105 +43,95 @@
     Dashboards,
     Database,
     Dcv,
     DirectoryService,
     Dns,
     Efa,
     EphemeralVolume,
+    ExistingFsxFileCache,
     ExistingFsxOntap,
     ExistingFsxOpenZfs,
     FlexibleInstanceType,
     GpuHealthCheck,
     HeadNode,
     HeadNodeImage,
     HeadNodeNetworking,
+    HeadNodeSsh,
     HealthChecks,
     Iam,
     Image,
     Imds,
     IntelSoftware,
     LocalStorage,
+    LoginNodes,
+    LoginNodesIam,
+    LoginNodesImage,
+    LoginNodesNetworking,
+    LoginNodesPool,
+    LoginNodesSsh,
     LogRotation,
     Logs,
     Monitoring,
     PlacementGroup,
     Proxy,
     QueueImage,
     QueueUpdateStrategy,
     Raid,
     Roles,
     RootVolume,
     S3Access,
-    SchedulerPluginCloudFormationInfrastructure,
-    SchedulerPluginClusterConfig,
-    SchedulerPluginClusterInfrastructure,
-    SchedulerPluginClusterSharedArtifact,
-    SchedulerPluginComputeResource,
-    SchedulerPluginComputeResourceConstraints,
-    SchedulerPluginDefinition,
-    SchedulerPluginEvent,
-    SchedulerPluginEvents,
-    SchedulerPluginExecuteCommand,
-    SchedulerPluginFile,
-    SchedulerPluginLogs,
-    SchedulerPluginMonitoring,
-    SchedulerPluginPluginResources,
-    SchedulerPluginQueue,
-    SchedulerPluginQueueConstraints,
-    SchedulerPluginQueueNetworking,
-    SchedulerPluginRequirements,
-    SchedulerPluginScheduling,
-    SchedulerPluginSettings,
-    SchedulerPluginSupportedDistros,
-    SchedulerPluginUser,
     SharedEbs,
     SharedEfs,
     SharedFsxLustre,
     SlurmClusterConfig,
     SlurmComputeResource,
     SlurmComputeResourceNetworking,
     SlurmFlexibleComputeResource,
     SlurmQueue,
     SlurmQueueNetworking,
     SlurmScheduling,
     SlurmSettings,
-    Ssh,
-    SudoerConfiguration,
     Timeouts,
 )
 from pcluster.config.common import BaseTag
 from pcluster.config.update_policy import UpdatePolicy
 from pcluster.constants import (
     DELETION_POLICIES,
     DELETION_POLICIES_WITH_SNAPSHOT,
+    FILECACHE,
+    FSX_FILE_CACHE,
+    FSX_FILE_CACHE_ID_REGEX,
     FSX_LUSTRE,
     FSX_ONTAP,
     FSX_OPENZFS,
     FSX_VOLUME_ID_REGEX,
+    IAM_INSTANCE_PROFILE_REGEX,
+    IAM_POLICY_REGEX,
+    IAM_ROLE_REGEX,
     LUSTRE,
+    MAX_SLURM_NODE_PRIORITY,
+    MIN_SLURM_NODE_PRIORITY,
     ONTAP,
     OPENZFS,
-    SCHEDULER_PLUGIN_MAX_NUMBER_OF_USERS,
+    PCLUSTER_AMI_ID_REGEX,
     SUPPORTED_OSES,
 )
-from pcluster.models.s3_bucket import parse_bucket_url
 from pcluster.schemas.common_schema import (
     AdditionalIamPolicySchema,
     BaseDevSettingsSchema,
     BaseSchema,
     DeploymentSettingsSchema,
 )
 from pcluster.schemas.common_schema import ImdsSchema as TopLevelImdsSchema
 from pcluster.schemas.common_schema import (
     TagSchema,
     get_field_validator,
     validate_no_duplicate_tag,
     validate_no_reserved_tag,
 )
-from pcluster.utils import yaml_load
 from pcluster.validators.cluster_validators import EFS_MESSAGES, FSX_MESSAGES
 
 # pylint: disable=C0302
 
 
 LOGGER = logging.getLogger(__name__)
 
@@ -475,55 +460,76 @@
     volume_id = fields.Str(
         required=True,
         validate=validate.Regexp(FSX_VOLUME_ID_REGEX),
         metadata={"update_policy": UpdatePolicy.UNSUPPORTED},
     )
 
 
+class FsxFileCacheSettingsSchema(BaseSchema):
+    """Represent the FSX File Cache schema."""
+
+    file_cache_id = fields.Str(
+        required=True,
+        validate=validate.Regexp(FSX_FILE_CACHE_ID_REGEX),
+        metadata={"update_policy": UpdatePolicy.UNSUPPORTED},
+    )
+
+
 class SharedStorageSchema(BaseSchema):
     """Represent the generic SharedStorage schema."""
 
     mount_dir = fields.Str(
         required=True,
         validate=get_field_validator("file_path"),
         metadata={"update_policy": UpdatePolicy.SHARED_STORAGE_UPDATE_POLICY},
     )
     name = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     storage_type = fields.Str(
         required=True,
-        validate=validate.OneOf(["Ebs", FSX_LUSTRE, FSX_OPENZFS, FSX_ONTAP, "Efs"]),
+        validate=validate.OneOf(["Ebs", FSX_LUSTRE, FSX_OPENZFS, FSX_ONTAP, "Efs", FSX_FILE_CACHE]),
         metadata={"update_policy": UpdatePolicy.UNSUPPORTED},
     )
     ebs_settings = fields.Nested(EbsSettingsSchema, metadata={"update_policy": UpdatePolicy.IGNORED})
     efs_settings = fields.Nested(EfsSettingsSchema, metadata={"update_policy": UpdatePolicy.IGNORED})
     fsx_lustre_settings = fields.Nested(FsxLustreSettingsSchema, metadata={"update_policy": UpdatePolicy.IGNORED})
     fsx_open_zfs_settings = fields.Nested(
         FsxOpenZfsSettingsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
     )
     fsx_ontap_settings = fields.Nested(FsxOntapSettingsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
+    fsx_file_cache_settings = fields.Nested(
+        FsxFileCacheSettingsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
+    )
 
     @validates_schema
     def no_coexist_storage_settings(self, data, **kwargs):
         """Validate that *_settings for different storage types do not co-exist."""
         if self.fields_coexist(
             data,
-            ["ebs_settings", "efs_settings", "fsx_lustre_settings", "fsx_open_zfs_settings", "fsx_ontap_settings"],
+            [
+                "ebs_settings",
+                "efs_settings",
+                "fsx_lustre_settings",
+                "fsx_open_zfs_settings",
+                "fsx_ontap_settings",
+                "fsx_file_cache_settings",
+            ],
             **kwargs,
         ):
             raise ValidationError("Multiple *Settings sections cannot be specified in the SharedStorage items.")
 
     @validates_schema
     def right_storage_settings(self, data, **kwargs):
         """Validate that *_settings param is associated to the right storage type."""
         for storage_type, settings in [
             ("Ebs", "ebs_settings"),
             ("Efs", "efs_settings"),
             (FSX_LUSTRE, "fsx_lustre_settings"),
             (FSX_OPENZFS, "fsx_open_zfs_settings"),
             (FSX_ONTAP, "fsx_ontap_settings"),
+            (FSX_FILE_CACHE, "fsx_file_cache_settings"),
         ]:
             # Verify the settings section is associated to the right storage type
             if data.get(settings, None) and storage_type != data.get("storage_type"):
                 raise ValidationError(
                     "SharedStorage > *Settings section is not appropriate to the "
                     f"StorageType {data.get('storage_type')}."
                 )
@@ -535,45 +541,53 @@
         shared_volume_attributes = {"mount_dir": data.get("mount_dir"), "name": data.get("name")}
         settings = (
             data.get("efs_settings", None)
             or data.get("ebs_settings", None)
             or data.get("fsx_lustre_settings", None)
             or data.get("fsx_open_zfs_settings", None)
             or data.get("fsx_ontap_settings", None)
+            or data.get("fsx_file_cache_settings", None)
         )
         if settings:
             shared_volume_attributes.update(**settings)
         if storage_type == "Efs":
             return SharedEfs(**shared_volume_attributes)
         elif storage_type == "Ebs":
             return SharedEbs(**shared_volume_attributes)
         elif storage_type == FSX_LUSTRE:
             return SharedFsxLustre(**shared_volume_attributes)
         elif storage_type == FSX_OPENZFS:
             return ExistingFsxOpenZfs(**shared_volume_attributes)
         elif storage_type == FSX_ONTAP:
             return ExistingFsxOntap(**shared_volume_attributes)
+        elif storage_type == FSX_FILE_CACHE:
+            return ExistingFsxFileCache(**shared_volume_attributes)
         return None
 
     @pre_dump
     def restore_child(self, data, **kwargs):
         """Restore back the child in the schema."""
         adapted_data = copy.deepcopy(data)
         # Move SharedXxx as a child to be automatically managed by marshmallow, see post_load action
         if adapted_data.shared_storage_type == "efs":
             storage_type = "efs"
         elif adapted_data.shared_storage_type == "fsx":
-            mapping = {LUSTRE: "fsx_lustre", OPENZFS: "fsx_open_zfs", ONTAP: "fsx_ontap"}
+            mapping = {
+                LUSTRE: "fsx_lustre",
+                OPENZFS: "fsx_open_zfs",
+                ONTAP: "fsx_ontap",
+                FILECACHE: "fsx_file_cache_settings",
+            }
             storage_type = mapping.get(adapted_data.file_system_type)
         else:  # "raid", "ebs"
             storage_type = "ebs"
         setattr(adapted_data, f"{storage_type}_settings", copy.copy(adapted_data))
         # Restore storage type attribute
         if adapted_data.shared_storage_type == "fsx":
-            mapping = {LUSTRE: FSX_LUSTRE, OPENZFS: FSX_OPENZFS, ONTAP: FSX_ONTAP}
+            mapping = {LUSTRE: FSX_LUSTRE, OPENZFS: FSX_OPENZFS, ONTAP: FSX_ONTAP, FILECACHE: FSX_FILE_CACHE}
             adapted_data.storage_type = mapping.get(adapted_data.file_system_type)
         else:
             adapted_data.storage_type = storage_type.capitalize()
         return adapted_data
 
     @validates("mount_dir")
     def shared_dir_validator(self, value):
@@ -607,16 +621,27 @@
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return Proxy(**data)
 
 
+class LoginNodeProxySchema(BaseSchema):
+    """Represent the schema of proxy for a Login Node."""
+
+    http_proxy_address = fields.Str(metadata={"update_policy": UpdatePolicy.SUPPORTED})
+
+    @post_load
+    def make_resource(self, data, **kwargs):
+        """Generate resource."""
+        return Proxy(**data)
+
+
 class BaseNetworkingSchema(BaseSchema):
-    """Represent the schema of common networking parameters used by head and compute nodes."""
+    """Represent the schema of common networking parameters used by head, compute and login nodes."""
 
     additional_security_groups = fields.List(
         fields.Str(validate=get_field_validator("security_group_id")),
         metadata={"update_policy": UpdatePolicy.SUPPORTED},
     )
     security_groups = fields.List(
         fields.Str(validate=get_field_validator("security_group_id")),
@@ -696,33 +721,29 @@
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return AwsBatchQueueNetworking(**data)
 
 
-class SchedulerPluginQueueNetworkingSchema(SlurmQueueNetworkingSchema):
-    """Represent the schema of the Networking, child of Scheduler Plugin Queue."""
+class BaseSshSchema(BaseSchema):
+    """Represent the schema of common Ssh parameters used by head and login nodes."""
 
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginQueueNetworking(**data)
+    key_name = fields.Str(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
 
 
-class SshSchema(BaseSchema):
-    """Represent the schema of the SSH."""
+class HeadNodeSshSchema(BaseSshSchema):
+    """Represent the schema of the HeadNodeSsh."""
 
-    key_name = fields.Str(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     allowed_ips = fields.Str(validate=get_field_validator("cidr"), metadata={"update_policy": UpdatePolicy.SUPPORTED})
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
-        return Ssh(**data)
+        return HeadNodeSsh(**data)
 
 
 class DcvSchema(BaseSchema):
     """Represent the schema of DCV."""
 
     enabled = fields.Bool(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     port = fields.Int(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
@@ -857,46 +878,51 @@
 
 
 class ClusterIamSchema(BaseSchema):
     """Represent the schema of IAM for Cluster."""
 
     roles = fields.Nested(RolesSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
     permissions_boundary = fields.Str(
-        metadata={"update_policy": UpdatePolicy.SUPPORTED}, validate=validate.Regexp("^arn:.*:policy/")
+        metadata={"update_policy": UpdatePolicy.SUPPORTED}, validate=validate.Regexp(IAM_POLICY_REGEX)
     )
 
     resource_prefix = fields.Str(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return ClusterIam(**data)
 
 
-class IamSchema(BaseSchema):
-    """Common schema of IAM for HeadNode and Queue."""
+class BaseIamSchema(BaseSchema):
+    """Represent the schema of common Iam parameters used by head, queue and login nodes."""
 
     instance_role = fields.Str(
-        metadata={"update_policy": UpdatePolicy.SUPPORTED}, validate=validate.Regexp("^arn:.*:role/")
-    )
-    s3_access = fields.Nested(
-        S3AccessSchema, many=True, metadata={"update_policy": UpdatePolicy.SUPPORTED, "update_key": "BucketName"}
+        metadata={"update_policy": UpdatePolicy.SUPPORTED}, validate=validate.Regexp(IAM_ROLE_REGEX)
     )
     additional_iam_policies = fields.Nested(
         AdditionalIamPolicySchema, many=True, metadata={"update_policy": UpdatePolicy.SUPPORTED, "update_key": "Policy"}
     )
 
     @validates_schema
     def no_coexist_role_policies(self, data, **kwargs):
         """Validate that instance_role, instance_profile or additional_iam_policies do not co-exist."""
         if self.fields_coexist(data, ["instance_role", "instance_profile", "additional_iam_policies"], **kwargs):
             raise ValidationError(
                 "InstanceProfile, InstanceRole or AdditionalIamPolicies can not be configured together."
             )
 
+
+class IamSchema(BaseIamSchema):
+    """Common schema of IAM for HeadNode and Queue."""
+
+    s3_access = fields.Nested(
+        S3AccessSchema, many=True, metadata={"update_policy": UpdatePolicy.SUPPORTED, "update_key": "BucketName"}
+    )
+
     @validates_schema
     def no_coexist_s3_access(self, data, **kwargs):
         """Validate that instance_role, instance_profile or additional_iam_policies do not co-exist."""
         if self.fields_coexist(data, ["instance_role", "s3_access"], **kwargs):
             raise ValidationError("S3Access can not be configured when InstanceRole is set.")
         if self.fields_coexist(data, ["instance_profile", "s3_access"], **kwargs):
             raise ValidationError("S3Access can not be configured when InstanceProfile is set.")
@@ -907,26 +933,49 @@
         return Iam(**data)
 
 
 class HeadNodeIamSchema(IamSchema):
     """Represent the schema of IAM for HeadNode."""
 
     instance_profile = fields.Str(
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED}, validate=validate.Regexp("^arn:.*:instance-profile/")
+        metadata={"update_policy": UpdatePolicy.UNSUPPORTED}, validate=validate.Regexp(IAM_INSTANCE_PROFILE_REGEX)
     )
 
 
 class QueueIamSchema(IamSchema):
     """Represent the schema of IAM for Queue."""
 
     instance_profile = fields.Str(
         metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP},
-        validate=validate.Regexp("^arn:.*:instance-profile/"),
+        validate=validate.Regexp(IAM_INSTANCE_PROFILE_REGEX),
+    )
+
+
+class LoginNodesIamSchema(BaseIamSchema):
+    """Represent the IAM schema of LoginNodes."""
+
+    instance_role = fields.Str(
+        metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP}, validate=validate.Regexp(IAM_ROLE_REGEX)
+    )
+
+    additional_iam_policies = fields.Nested(
+        AdditionalIamPolicySchema,
+        many=True,
+        metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP, "update_key": "Policy"},
+    )
+
+    instance_profile = fields.Str(
+        metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP}, validate=validate.Regexp(IAM_INSTANCE_PROFILE_REGEX)
     )
 
+    @post_load
+    def make_resource(self, data, **kwargs):
+        """Generate resource."""
+        return LoginNodesIam(**data)
+
 
 class ImdsSchema(BaseSchema):
     """Represent the schema of IMDS for HeadNode."""
 
     secured = fields.Bool(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
 
     @post_load
@@ -1016,14 +1065,15 @@
 class ClusterDevSettingsSchema(BaseDevSettingsSchema):
     """Represent the schema of Dev Setting."""
 
     cluster_template = fields.Str(metadata={"update_policy": UpdatePolicy.SUPPORTED})
     ami_search_filters = fields.Nested(AmiSearchFiltersSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     instance_types_data = fields.Str(metadata={"update_policy": UpdatePolicy.SUPPORTED})
     timeouts = fields.Nested(TimeoutsSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
+    compute_startup_time_metric_enabled = fields.Bool(metadata={"update_policy": UpdatePolicy.SUPPORTED})
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return ClusterDevSettings(**data)
 
 
@@ -1058,43 +1108,43 @@
 class ImageSchema(BaseSchema):
     """Represent the schema of the Image."""
 
     os = fields.Str(
         required=True, validate=validate.OneOf(SUPPORTED_OSES), metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
     )
     custom_ami = fields.Str(
-        validate=validate.Regexp(r"^ami-[0-9a-z]{8}$|^ami-[0-9a-z]{17}$"),
+        validate=validate.Regexp(PCLUSTER_AMI_ID_REGEX),
         metadata={"update_policy": UpdatePolicy.UNSUPPORTED},
     )
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return Image(**data)
 
 
 class HeadNodeImageSchema(BaseSchema):
     """Represent the schema of the HeadNode Image."""
 
     custom_ami = fields.Str(
-        validate=validate.Regexp(r"^ami-[0-9a-z]{8}$|^ami-[0-9a-z]{17}$"),
+        validate=validate.Regexp(PCLUSTER_AMI_ID_REGEX),
         metadata={"update_policy": UpdatePolicy.UNSUPPORTED},
     )
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return HeadNodeImage(**data)
 
 
 class QueueImageSchema(BaseSchema):
     """Represent the schema of the Queue Image."""
 
     custom_ami = fields.Str(
-        validate=validate.Regexp(r"^ami-[0-9a-z]{8}$|^ami-[0-9a-z]{17}$"),
+        validate=validate.Regexp(PCLUSTER_AMI_ID_REGEX),
         metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY},
     )
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return QueueImage(**data)
@@ -1204,28 +1254,128 @@
     """Represent the schema of the HeadNode."""
 
     instance_type = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     disable_simultaneous_multithreading = fields.Bool(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     networking = fields.Nested(
         HeadNodeNetworkingSchema, required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
     )
-    ssh = fields.Nested(SshSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
+    ssh = fields.Nested(HeadNodeSshSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
     local_storage = fields.Nested(HeadNodeStorageSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
     dcv = fields.Nested(DcvSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     custom_actions = fields.Nested(HeadNodeCustomActionsSchema, metadata={"update_policy": UpdatePolicy.IGNORED})
     iam = fields.Nested(HeadNodeIamSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
     imds = fields.Nested(ImdsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     image = fields.Nested(HeadNodeImageSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
 
     @post_load()
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return HeadNode(**data)
 
 
+class LoginNodesImageSchema(BaseSchema):
+    """Represent the Image schema of LoginNodes."""
+
+    custom_ami = fields.Str(
+        validate=validate.Regexp(PCLUSTER_AMI_ID_REGEX),
+        metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP},
+    )
+
+    @post_load
+    def make_resource(self, data, **kwargs):
+        """Generate resource."""
+        return LoginNodesImage(**data)
+
+
+class LoginNodesSshSchema(BaseSshSchema):
+    """Represent the Ssh schema of LoginNodes."""
+
+    key_name = fields.Str(metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP})
+
+    @post_load
+    def make_resource(self, data, **kwargs):
+        """Generate resource."""
+        return LoginNodesSsh(**data)
+
+
+class LoginNodesNetworkingSchema(BaseNetworkingSchema):
+    """Represent the networking schema of LoginNodes."""
+
+    subnet_ids = fields.List(
+        fields.Str(validate=get_field_validator("subnet_id")),
+        required=True,
+        validate=validate.Length(equal=1, error="Only one subnet can be associated with a login node pool."),
+        metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP},
+    )
+    additional_security_groups = fields.List(
+        fields.Str(validate=get_field_validator("security_group_id")),
+        metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP},
+    )
+    security_groups = fields.List(
+        fields.Str(validate=get_field_validator("security_group_id")),
+        metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP},
+    )
+
+    proxy = fields.Nested(LoginNodeProxySchema, metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP})
+
+    @post_load
+    def make_resource(self, data, **kwargs):
+        """Generate resource."""
+        return LoginNodesNetworking(**data)
+
+
+class LoginNodesPoolSchema(BaseSchema):
+    """Represent the schema of the LoginNodesPool."""
+
+    name = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP})
+    instance_type = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP})
+    image = fields.Nested(LoginNodesImageSchema, metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP})
+    networking = fields.Nested(
+        LoginNodesNetworkingSchema, required=True, metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP}
+    )
+    count = fields.Int(
+        required=True,
+        validate=validate.Range(
+            min=0,
+            error="The count for LoginNodes Pool must be greater than or equal to 0.",
+        ),
+        metadata={"update_policy": UpdatePolicy.SUPPORTED},
+    )
+    ssh = fields.Nested(LoginNodesSshSchema, metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP})
+    iam = fields.Nested(LoginNodesIamSchema, metadata={"update_policy": UpdatePolicy.LOGIN_NODES_STOP})
+    gracetime_period = fields.Int(
+        validate=validate.Range(
+            min=1, max=120, error="The gracetime period for LoginNodes Pool must be an interger from 1 to 120."
+        ),
+        metadata={"update_policy": UpdatePolicy.SUPPORTED},
+    )
+
+    @post_load
+    def make_resource(self, data, **kwargs):
+        """Generate resource."""
+        return LoginNodesPool(**data)
+
+
+class LoginNodesSchema(BaseSchema):
+    """Represent the schema of LoginNodes."""
+
+    pools = fields.Nested(
+        LoginNodesPoolSchema,
+        many=True,
+        required=True,
+        validate=validate.Length(equal=1, error="Only one pool can be specified when using login nodes."),
+        metadata={"update_policy": UpdatePolicy(UpdatePolicy.LOGIN_NODES_POOLS), "update_key": "Name"},
+    )
+
+    @post_load()
+    def make_resource(self, data, **kwargs):
+        """Generate resource."""
+        return LoginNodes(**data)
+
+
 class _ComputeResourceSchema(BaseSchema):
     """Represent the schema of the ComputeResource."""
 
     name = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
 
 
 class SlurmComputeResourceNetworkingSchema(BaseSchema):
@@ -1285,14 +1435,22 @@
         SlurmComputeResourceNetworkingSchema, metadata={"update_policy": UpdatePolicy.MANAGED_PLACEMENT_GROUP}
     )
     health_checks = fields.Nested(HealthChecksSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
     custom_slurm_settings = fields.Dict(metadata={"update_policy": UpdatePolicy.SUPPORTED})
     tags = fields.Nested(
         QueueTagSchema, many=True, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY, "update_key": "Key"}
     )
+    static_node_priority = fields.Int(
+        validate=validate.Range(min=MIN_SLURM_NODE_PRIORITY, max=MAX_SLURM_NODE_PRIORITY),
+        metadata={"update_policy": UpdatePolicy.SUPPORTED},
+    )
+    dynamic_node_priority = fields.Int(
+        validate=validate.Range(min=MIN_SLURM_NODE_PRIORITY, max=MAX_SLURM_NODE_PRIORITY),
+        metadata={"update_policy": UpdatePolicy.SUPPORTED},
+    )
 
     @validates_schema
     def no_coexist_instance_type_flexibility(self, data, **kwargs):
         """Validate that 'instance_type' and 'instances' do not co-exist."""
         if self.fields_coexist(
             data,
             ["instance_type", "instances"],
@@ -1351,25 +1509,14 @@
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return AwsBatchComputeResource(**data)
 
 
-class SchedulerPluginComputeResourceSchema(SlurmComputeResourceSchema):
-    """Represent the schema of the Scheduler Plugin ComputeResource."""
-
-    custom_settings = fields.Dict(metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginComputeResource(**data)
-
-
 class ComputeSettingsSchema(BaseSchema):
     """Represent the schema of the compute_settings schedulers queues."""
 
     local_storage = fields.Nested(QueueStorageSchema, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY})
 
     @post_load()
     def make_resource(self, data, **kwargs):
@@ -1384,15 +1531,15 @@
     capacity_type = fields.Str(
         validate=validate.OneOf([event.value for event in CapacityType]),
         metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY},
     )
 
 
 class _CommonQueueSchema(BaseQueueSchema):
-    """Represent the schema of common part between Slurm and Scheduler Plugin Queue."""
+    """Represent the schema of common part between Slurm and future scheduler Queue."""
 
     compute_settings = fields.Nested(
         ComputeSettingsSchema, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY}
     )
     custom_actions = fields.Nested(
         QueueCustomActionsSchema, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY}
     )
@@ -1419,14 +1566,15 @@
         SlurmQueueNetworkingSchema, required=True, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY}
     )
     health_checks = fields.Nested(HealthChecksSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
     custom_slurm_settings = fields.Dict(metadata={"update_policy": UpdatePolicy.SUPPORTED})
     tags = fields.Nested(
         QueueTagSchema, many=True, metadata={"update_policy": UpdatePolicy.QUEUE_UPDATE_STRATEGY, "update_key": "Key"}
     )
+    job_exclusive_allocation = fields.Bool(metadata={"update_policy": UpdatePolicy.SUPPORTED})
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return SlurmQueue(**data)
 
     @validates("tags")
@@ -1451,33 +1599,14 @@
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return AwsBatchQueue(**data)
 
 
-class SchedulerPluginQueueSchema(_CommonQueueSchema):
-    """Represent the schema of a Scheduler Plugin Queue."""
-
-    compute_resources = fields.Nested(
-        SchedulerPluginComputeResourceSchema,
-        many=True,
-        metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP, "update_key": "Name"},
-    )
-    networking = fields.Nested(
-        SchedulerPluginQueueNetworkingSchema, required=True, metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP}
-    )
-    custom_settings = fields.Dict(metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginQueue(**data)
-
-
 class DnsSchema(BaseSchema):
     """Represent the schema of Dns Settings."""
 
     disable_managed_dns = fields.Bool(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     hosted_zone_id = fields.Str(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     use_ec2_hostnames = fields.Bool(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
 
@@ -1503,15 +1632,18 @@
         """Generate resource."""
         return Database(**data)
 
 
 class SlurmSettingsSchema(BaseSchema):
     """Represent the schema of the Scheduling Settings."""
 
-    scaledown_idletime = fields.Int(metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
+    scaledown_idletime = fields.Int(
+        validate=validate.Range(min=-1),
+        metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP},
+    )
     dns = fields.Nested(DnsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     queue_update_strategy = fields.Str(
         validate=validate.OneOf([strategy.value for strategy in QueueUpdateStrategy]),
         metadata={"update_policy": UpdatePolicy.IGNORED},
     )
     enable_memory_based_scheduling = fields.Bool(metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
     database = fields.Nested(DatabaseSchema, metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
@@ -1529,435 +1661,20 @@
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return AwsBatchSettings(**data)
 
 
-class SchedulerPluginSupportedDistrosSchema(BaseSchema):
-    """Represent the schema for SupportedDistros in a Scheduler Plugin."""
-
-    x86 = fields.List(fields.Str(), metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    arm64 = fields.List(fields.Str(), metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginSupportedDistros(**data)
-
-
-class SchedulerPluginQueueConstraintsSchema(BaseSchema):
-    """Represent the schema for QueueConstraints in a Scheduler Plugin."""
-
-    max_count = fields.Int(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginQueueConstraints(**data)
-
-
-class SchedulerPluginComputeResourceConstraintsSchema(BaseSchema):
-    """Represent the schema for ComputeResourceConstraints in a Scheduler Plugin."""
-
-    max_count = fields.Int(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginComputeResourceConstraints(**data)
-
-
-class SchedulerPluginRequirementsSchema(BaseSchema):
-    """Represent the schema for Requirements in a Scheduler Plugin."""
-
-    supported_distros = fields.Nested(
-        SchedulerPluginSupportedDistrosSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
-    )
-    supported_regions = fields.List(fields.Str(), metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    queue_constraints = fields.Nested(
-        SchedulerPluginQueueConstraintsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
-    )
-    compute_resource_constraints = fields.Nested(
-        SchedulerPluginComputeResourceConstraintsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
-    )
-    requires_sudo_privileges = fields.Bool(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    supports_cluster_update = fields.Bool(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    supported_parallel_cluster_versions = fields.Str(
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED},
-        validate=validate.Regexp(
-            r"^((>|<|>=|<=)?[0-9]+\.[0-9]+\.[0-9]+([a-z][0-9]+)?,\s*)*(>|<|>=|<=)?[0-9]+\.[0-9]+\.[0-9]+([a-z][0-9]+)?$"
-        ),
-    )
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginRequirements(**data)
-
-
-class SchedulerPluginCloudFormationClusterInfrastructureSchema(BaseSchema):
-    """Represent the CloudFormation section of the Scheduler Plugin ClusterInfrastructure schema."""
-
-    template = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    s3_bucket_owner = fields.Str(
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED}, validate=validate.Regexp(r"^\d{12}$")
-    )
-    checksum = fields.Str(
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED}, validate=validate.Regexp(r"^[A-Fa-f0-9]{64}$")
-    )
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginCloudFormationInfrastructure(**data)
-
-
-class SchedulerPluginClusterInfrastructureSchema(BaseSchema):
-    """Represent the schema for ClusterInfrastructure schema in a Scheduler Plugin."""
-
-    cloud_formation = fields.Nested(
-        SchedulerPluginCloudFormationClusterInfrastructureSchema,
-        required=True,
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED},
-    )
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginClusterInfrastructure(**data)
-
-
-class SchedulerPluginClusterSharedArtifactSchema(BaseSchema):
-    """Represent the schema for Cluster Shared Artifact in a Scheduler Plugin."""
-
-    source = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    s3_bucket_owner = fields.Str(
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED}, validate=validate.Regexp(r"^\d{12}$")
-    )
-    checksum = fields.Str(
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED}, validate=validate.Regexp(r"^[A-Fa-f0-9]{64}$")
-    )
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginClusterSharedArtifact(**data)
-
-
-class SchedulerPluginResourcesSchema(BaseSchema):
-    """Represent the schema for Plugin Resouces in a Scheduler Plugin."""
-
-    cluster_shared_artifacts = fields.Nested(
-        SchedulerPluginClusterSharedArtifactSchema,
-        many=True,
-        required=True,
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED, "update_key": "Source"},
-    )
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginPluginResources(**data)
-
-
-class SchedulerPluginExecuteCommandSchema(BaseSchema):
-    """Represent the schema for ExecuteCommand in a Scheduler Plugin."""
-
-    command = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginExecuteCommand(**data)
-
-
-class SchedulerPluginEventSchema(BaseSchema):
-    """Represent the schema for Event in a Scheduler Plugin."""
-
-    execute_command = fields.Nested(
-        SchedulerPluginExecuteCommandSchema, required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
-    )
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginEvent(**data)
-
-
-class SchedulerPluginEventsSchema(BaseSchema):
-    """Represent the schema for Events in a Scheduler Plugin."""
-
-    head_init = fields.Nested(SchedulerPluginEventSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    head_configure = fields.Nested(SchedulerPluginEventSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    head_finalize = fields.Nested(SchedulerPluginEventSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    compute_init = fields.Nested(SchedulerPluginEventSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    compute_configure = fields.Nested(SchedulerPluginEventSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    compute_finalize = fields.Nested(SchedulerPluginEventSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    head_cluster_update = fields.Nested(
-        SchedulerPluginEventSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
-    )
-    head_compute_fleet_update = fields.Nested(
-        SchedulerPluginEventSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
-    )
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginEvents(**data)
-
-
-class SchedulerPluginFileSchema(BaseSchema):
-    """Represent the schema of the Scheduler Plugin."""
-
-    file_path = fields.Str(
-        required=True, validate=get_field_validator("file_path"), metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
-    )
-    timestamp_format = fields.Str(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    node_type = fields.Str(
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED}, validate=validate.OneOf(["HEAD", "COMPUTE", "ALL"])
-    )
-    log_stream_name = fields.Str(
-        required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}, validate=validate.Regexp(r"^[^:*]*$")
-    )
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginFile(**data)
-
-
-class SchedulerPluginLogsSchema(BaseSchema):
-    """Represent the schema of the Scheduler Plugin Logs."""
-
-    files = fields.Nested(
-        SchedulerPluginFileSchema,
-        required=True,
-        many=True,
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED, "update_key": "FilePath"},
-    )
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginLogs(**data)
-
-
-class SchedulerPluginMonitoringSchema(BaseSchema):
-    """Represent the schema of the Scheduler plugin Monitoring."""
-
-    logs = fields.Nested(SchedulerPluginLogsSchema, required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginMonitoring(**data)
-
-
-class SudoerConfigurationSchema(BaseSchema):
-    """Represent the SudoerConfiguration for scheduler plugin SystemUsers declared in the SchedulerDefinition."""
-
-    commands = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    run_as = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SudoerConfiguration(**data)
-
-
-class SchedulerPluginUserSchema(BaseSchema):
-    """Represent the schema of the Scheduler Plugin."""
-
-    name = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    enable_imds = fields.Bool(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    sudoer_configuration = fields.Nested(
-        SudoerConfigurationSchema, many=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED, "update_key": "Name"}
-    )
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginUser(**data)
-
-
-class SchedulerPluginDefinitionSchema(BaseSchema):
-    """Represent the schema of the Scheduler Plugin SchedulerDefinition."""
-
-    plugin_interface_version = fields.Str(
-        required=True,
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED},
-        validate=validate.Regexp(r"^[0-9]+\.[0-9]+$"),
-    )
-    metadata = fields.Dict(metadata={"update_policy": UpdatePolicy.UNSUPPORTED}, required=True)
-    requirements = fields.Nested(
-        SchedulerPluginRequirementsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
-    )
-    cluster_infrastructure = fields.Nested(
-        SchedulerPluginClusterInfrastructureSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
-    )
-    plugin_resources = fields.Nested(
-        SchedulerPluginResourcesSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
-    )
-    events = fields.Nested(
-        SchedulerPluginEventsSchema, required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
-    )
-    monitoring = fields.Nested(SchedulerPluginMonitoringSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    system_users = fields.Nested(
-        SchedulerPluginUserSchema,
-        many=True,
-        validate=validate.Length(max=SCHEDULER_PLUGIN_MAX_NUMBER_OF_USERS),
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED, "update_key": "Name"},
-    )
-    tags = fields.Nested(
-        TagSchema, many=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED, "update_key": "Key"}
-    )
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginDefinition(**data)
-
-    @validates("metadata")
-    def validate_metadata(self, value):
-        """Validate metadata contains fieds 'name' and 'version'."""
-        for key in ["Name", "Version"]:
-            if key not in value.keys():
-                raise ValidationError(f"{key} is required for scheduler plugin Metadata.")
-
-
-class SchedulerPluginSettingsSchema(BaseSchema):
-    """Represent the schema of the Scheduling Settings."""
-
-    scheduler_definition = fields.Nested(
-        SchedulerPluginDefinitionSchema, required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED}
-    )
-    grant_sudo_privileges = fields.Bool(metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
-    custom_settings = fields.Dict(metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
-    scheduler_definition_s3_bucket_owner = fields.Str(
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED}, validate=validate.Regexp(r"^\d{12}$")
-    )
-    scheduler_definition_checksum = fields.Str(
-        metadata={"update_policy": UpdatePolicy.UNSUPPORTED}, validate=validate.Regexp(r"^[A-Fa-f0-9]{64}$")
-    )
-
-    def _verify_checksum(self, file_content, original_definition, expected_checksum):
-        if expected_checksum:
-            actual_checksum = hashlib.sha256(file_content.encode()).hexdigest()
-            if actual_checksum != expected_checksum:
-                raise ValidationError(
-                    f"Error when validating SchedulerDefinition '{original_definition}': "
-                    f"checksum ({actual_checksum}) does not match expected one ({expected_checksum})"
-                )
-
-    def _fetch_scheduler_definition_from_s3(self, original_scheduler_definition, s3_bucket_owner):
-        try:
-            bucket_parsing_result = parse_bucket_url(original_scheduler_definition)
-            result = AWSApi.instance().s3.get_object(
-                bucket_name=bucket_parsing_result["bucket_name"],
-                key=bucket_parsing_result["object_key"],
-                expected_bucket_owner=s3_bucket_owner,
-            )
-            scheduler_definition = result["Body"].read().decode("utf-8")
-            return scheduler_definition
-        except AWSClientError as e:
-            error_message = (
-                f"Error while downloading scheduler definition from {original_scheduler_definition}: {str(e)}"
-            )
-            if s3_bucket_owner and e.error_code == "AccessDenied":
-                error_message = (
-                    f"{error_message}. This can be due to bucket owner not matching the expected "
-                    f"one '{s3_bucket_owner}'"
-                )
-            raise ValidationError(error_message) from e
-        except Exception as e:
-            raise ValidationError(
-                f"Error while downloading scheduler definition from {original_scheduler_definition}: {str(e)}"
-            ) from e
-
-    def _fetch_scheduler_definition_from_https(self, original_scheduler_definition):
-        try:
-            # A nosec comment is appended to the following line in order to disable the B310 check.
-            # The urlopen argument is properly validated
-            # [B310:blacklist] Audit url open for permitted schemes.
-            with urlopen(original_scheduler_definition) as f:  # nosec B310 nosemgrep
-                scheduler_definition = f.read().decode("utf-8")
-                return scheduler_definition
-        except Exception:
-            error_message = (
-                f"Error while downloading scheduler definition from {original_scheduler_definition}: "
-                "The provided URL is invalid or unavailable."
-            )
-            raise ValidationError(error_message)
-
-    def _validate_scheduler_definition_url(self, original_scheduler_definition, s3_bucket_owner):
-        """Validate SchedulerDefinition url is valid."""
-        if not original_scheduler_definition.startswith("s3") and not original_scheduler_definition.startswith("https"):
-            raise ValidationError(
-                f"Error while downloading scheduler definition from {original_scheduler_definition}: The provided value"
-                " for SchedulerDefinition is invalid. You can specify this as an S3 URL, HTTPS URL or as an inline "
-                "YAML object."
-            )
-        if original_scheduler_definition.startswith("https") and s3_bucket_owner:
-            raise ValidationError(
-                f"Error while downloading scheduler definition from {original_scheduler_definition}: "
-                "SchedulerDefinitionS3BucketOwner can only be specified when SchedulerDefinition is S3 URL."
-            )
-
-    def _fetch_scheduler_definition_from_url(
-        self, original_scheduler_definition, s3_bucket_owner, scheduler_definition_checksum, data
-    ):
-        LOGGER.info("Downloading scheduler plugin definition from %s", original_scheduler_definition)
-        if original_scheduler_definition.startswith("s3"):
-            scheduler_definition = self._fetch_scheduler_definition_from_s3(
-                original_scheduler_definition, s3_bucket_owner
-            )
-        elif original_scheduler_definition.startswith("https"):
-            scheduler_definition = self._fetch_scheduler_definition_from_https(original_scheduler_definition)
-
-        self._verify_checksum(scheduler_definition, original_scheduler_definition, scheduler_definition_checksum)
-
-        LOGGER.info("Using the following scheduler plugin definition:\n%s", scheduler_definition)
-        try:
-            data["SchedulerDefinition"] = yaml_load(scheduler_definition)
-        except YAMLError as e:
-            raise ValidationError(
-                f"The retrieved SchedulerDefinition ({original_scheduler_definition}) is not a valid YAML."
-            ) from e
-
-    @post_load
-    def make_resource(self, data, **kwargs):
-        """Generate resource."""
-        return SchedulerPluginSettings(**data)
-
-    @pre_load
-    def fetch_scheduler_definition(self, data, **kwargs):
-        """Fetch scheduler definition if it is s3 or https url."""
-        original_scheduler_definition = data["SchedulerDefinition"]
-        s3_bucket_owner = data.get("SchedulerDefinitionS3BucketOwner", None)
-        scheduler_definition_checksum = data.get("SchedulerDefinitionChecksum", None)
-        if isinstance(original_scheduler_definition, str):
-            self._validate_scheduler_definition_url(original_scheduler_definition, s3_bucket_owner)
-            self._fetch_scheduler_definition_from_url(
-                original_scheduler_definition, s3_bucket_owner, scheduler_definition_checksum, data
-            )
-        elif s3_bucket_owner or scheduler_definition_checksum:
-            raise ValidationError(
-                "SchedulerDefinitionS3BucketOwner or SchedulerDefinitionChecksum can only specified when "
-                "SchedulerDefinition is a URL."
-            )
-        return data
-
-
 class SchedulingSchema(BaseSchema):
     """Represent the schema of the Scheduling."""
 
     scheduler = fields.Str(
         required=True,
-        validate=validate.OneOf(["slurm", "awsbatch", "plugin"]),
+        validate=validate.OneOf(["slurm", "awsbatch"]),
         metadata={"update_policy": UpdatePolicy.UNSUPPORTED},
     )
     # Slurm schema
     slurm_settings = fields.Nested(SlurmSettingsSchema, metadata={"update_policy": UpdatePolicy.IGNORED})
     slurm_queues = fields.Nested(
         SlurmQueueSchema,
         many=True,
@@ -1969,48 +1686,34 @@
         many=True,
         validate=validate.Length(equal=1),
         metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP, "update_key": "Name"},
     )
     aws_batch_settings = fields.Nested(
         AwsBatchSettingsSchema, metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP}
     )
-    # Scheduler Plugin
-    scheduler_settings = fields.Nested(
-        SchedulerPluginSettingsSchema, metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP}
-    )
-    scheduler_queues = fields.Nested(
-        SchedulerPluginQueueSchema,
-        many=True,
-        metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP, "update_key": "Name"},
-    )
 
     @validates_schema
     def no_coexist_schedulers(self, data, **kwargs):
         """Validate that *_settings and *_queues for different schedulers do not co-exist."""
         scheduler = data.get("scheduler")
-        if self.fields_coexist(data, ["aws_batch_settings", "slurm_settings", "scheduler_settings"], **kwargs):
+        if self.fields_coexist(data, ["aws_batch_settings", "slurm_settings"], **kwargs):
             raise ValidationError("Multiple *Settings sections cannot be specified in the Scheduling section.")
-        if self.fields_coexist(
-            data, ["aws_batch_queues", "slurm_queues", "scheduler_queues"], one_required=True, **kwargs
-        ):
+        if self.fields_coexist(data, ["aws_batch_queues", "slurm_queues"], one_required=True, **kwargs):
             if scheduler == "awsbatch":
                 scheduler_prefix = "AwsBatch"
-            elif scheduler == "plugin":
-                scheduler_prefix = "Scheduler"
             else:
                 scheduler_prefix = scheduler.capitalize()
             raise ValidationError(f"{scheduler_prefix}Queues section must be specified in the Scheduling section.")
 
     @validates_schema
     def right_scheduler_schema(self, data, **kwargs):
         """Validate that *_settings field is associated to the right scheduler."""
         for scheduler, settings, queues in [
             ("awsbatch", "aws_batch_settings", "aws_batch_queues"),
             ("slurm", "slurm_settings", "slurm_queues"),
-            ("plugin", "scheduler_settings", "scheduler_queues"),
         ]:
             # Verify the settings section is associated to the right scheduler type
             configured_scheduler = data.get("scheduler")
             if settings in data and scheduler != configured_scheduler:
                 raise ValidationError(
                     f"Scheduling > *Settings section is not appropriate to the Scheduler: {configured_scheduler}."
                 )
@@ -2021,68 +1724,65 @@
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate the right type of scheduling according to the child type (Slurm vs AwsBatch vs Custom)."""
         scheduler = data.get("scheduler")
         if scheduler == "slurm":
             return SlurmScheduling(queues=data.get("slurm_queues"), settings=data.get("slurm_settings", None))
-        if scheduler == "plugin":
-            return SchedulerPluginScheduling(
-                queues=data.get("scheduler_queues"), settings=data.get("scheduler_settings", None)
-            )
         if scheduler == "awsbatch":
             return AwsBatchScheduling(
                 queues=data.get("aws_batch_queues"), settings=data.get("aws_batch_settings", None)
             )
         return None
 
     @pre_dump
     def restore_child(self, data, **kwargs):
         """Restore back the child in the schema, see post_load action."""
         adapted_data = copy.deepcopy(data)
         if adapted_data.scheduler == "awsbatch":
             scheduler_prefix = "aws_batch"
-        elif adapted_data.scheduler == "plugin":
-            scheduler_prefix = "scheduler"
         else:
             scheduler_prefix = adapted_data.scheduler
         setattr(adapted_data, f"{scheduler_prefix}_queues", copy.copy(getattr(adapted_data, "queues", None)))
         setattr(adapted_data, f"{scheduler_prefix}_settings", copy.copy(getattr(adapted_data, "settings", None)))
         return adapted_data
 
 
 class DirectoryServiceSchema(BaseSchema):
     """Represent the schema of the DirectoryService."""
 
-    domain_name = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
-    domain_addr = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
+    domain_name = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.COMPUTE_AND_LOGIN_NODES_STOP})
+    domain_addr = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.COMPUTE_AND_LOGIN_NODES_STOP})
     password_secret_arn = fields.Str(
         required=True,
         validate=validate.Regexp(r"^arn:.*:(secretsmanager:.*:.*:secret:|ssm:.*:.*:parameter\/).*$"),
-        metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP},
+        metadata={"update_policy": UpdatePolicy.COMPUTE_AND_LOGIN_NODES_STOP},
     )
-    domain_read_only_user = fields.Str(required=True, metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
-    ldap_tls_ca_cert = fields.Str(metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
+    domain_read_only_user = fields.Str(
+        required=True, metadata={"update_policy": UpdatePolicy.COMPUTE_AND_LOGIN_NODES_STOP}
+    )
+    ldap_tls_ca_cert = fields.Str(metadata={"update_policy": UpdatePolicy.COMPUTE_AND_LOGIN_NODES_STOP})
     ldap_tls_req_cert = fields.Str(
         validate=validate.OneOf(["never", "allow", "try", "demand", "hard"]),
-        metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP},
+        metadata={"update_policy": UpdatePolicy.COMPUTE_AND_LOGIN_NODES_STOP},
     )
-    ldap_access_filter = fields.Str(metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
-    generate_ssh_keys_for_users = fields.Bool(metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
-    additional_sssd_configs = fields.Dict(metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP})
+    ldap_access_filter = fields.Str(metadata={"update_policy": UpdatePolicy.COMPUTE_AND_LOGIN_NODES_STOP})
+    generate_ssh_keys_for_users = fields.Bool(metadata={"update_policy": UpdatePolicy.COMPUTE_AND_LOGIN_NODES_STOP})
+    additional_sssd_configs = fields.Dict(metadata={"update_policy": UpdatePolicy.COMPUTE_AND_LOGIN_NODES_STOP})
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return DirectoryService(**data)
 
 
 class ClusterSchema(BaseSchema):
     """Represent the schema of the Cluster."""
 
+    login_nodes = fields.Nested(LoginNodesSchema, many=False, metadata={"update_policy": UpdatePolicy.SUPPORTED})
     image = fields.Nested(ImageSchema, required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     head_node = fields.Nested(HeadNodeSchema, required=True, metadata={"update_policy": UpdatePolicy.SUPPORTED})
     scheduling = fields.Nested(SchedulingSchema, required=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     shared_storage = fields.Nested(
         SharedStorageSchema,
         many=True,
         metadata={
@@ -2094,15 +1794,15 @@
     monitoring = fields.Nested(MonitoringSchema, metadata={"update_policy": UpdatePolicy.IGNORED})
     additional_packages = fields.Nested(AdditionalPackagesSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     tags = fields.Nested(
         TagSchema, many=True, metadata={"update_policy": UpdatePolicy.UNSUPPORTED, "update_key": "Key"}
     )
     iam = fields.Nested(ClusterIamSchema, metadata={"update_policy": UpdatePolicy.IGNORED})
     directory_service = fields.Nested(
-        DirectoryServiceSchema, metadata={"update_policy": UpdatePolicy.COMPUTE_FLEET_STOP}
+        DirectoryServiceSchema, metadata={"update_policy": UpdatePolicy.COMPUTE_AND_LOGIN_NODES_STOP}
     )
     config_region = fields.Str(data_key="Region", metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     imds = fields.Nested(TopLevelImdsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
     custom_s3_bucket = fields.Str(metadata={"update_policy": UpdatePolicy.READ_ONLY_RESOURCE_BUCKET})
     additional_resources = fields.Str(metadata={"update_policy": UpdatePolicy.SUPPORTED})
     dev_settings = fields.Nested(ClusterDevSettingsSchema, metadata={"update_policy": UpdatePolicy.SUPPORTED})
     deployment_settings = fields.Nested(DeploymentSettingsSchema, metadata={"update_policy": UpdatePolicy.UNSUPPORTED})
@@ -2140,14 +1840,12 @@
     def make_resource(self, data, original_data, **kwargs):
         """Generate cluster according to the scheduler. Save original configuration."""
         scheduler = data.get("scheduling").scheduler
         if scheduler == "slurm":
             cluster = SlurmClusterConfig(cluster_name=self.cluster_name, **data)
         elif scheduler == "awsbatch":
             cluster = AwsBatchClusterConfig(cluster_name=self.cluster_name, **data)
-        elif scheduler == "plugin":
-            cluster = SchedulerPluginClusterConfig(cluster_name=self.cluster_name, **data)
         else:
             raise ValidationError(f"Unsupported scheduler {scheduler}.")
 
         cluster.source_config = original_data
         return cluster
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/schemas/common_schema.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/schemas/common_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import json
 
 from marshmallow import Schema, ValidationError, fields, post_dump, post_load, pre_dump, validate, validates
 
 from pcluster.config.cluster_config import BaseTag
 from pcluster.config.common import AdditionalIamPolicy, Cookbook, DeploymentSettings, Imds, LambdaFunctionsVpcConfig
 from pcluster.config.update_policy import UpdatePolicy
-from pcluster.constants import PCLUSTER_PREFIX, SUPPORTED_ARCHITECTURES
+from pcluster.constants import IAM_POLICY_REGEX, PCLUSTER_PREFIX, SUPPORTED_ARCHITECTURES
 from pcluster.utils import to_pascal_case
 
 ALLOWED_VALUES = {
     "cidr": r"^(([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])\.){3}"
     r"([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])"
     r"(\/([0-9]|[1-2][0-9]|3[0-2]))$",
     "file_path": r"^\/?[^\/.\\][^\/\\]*(\/[^\/.\\][^\/]*)*$",
@@ -181,15 +181,15 @@
         return BaseTag(**data)
 
 
 class AdditionalIamPolicySchema(BaseSchema):
     """Represent the schema of Additional IAM policy."""
 
     policy = fields.Str(
-        required=True, metadata={"update_policy": UpdatePolicy.SUPPORTED}, validate=validate.Regexp("^arn:.*:policy/")
+        required=True, metadata={"update_policy": UpdatePolicy.SUPPORTED}, validate=validate.Regexp(IAM_POLICY_REGEX)
     )
 
     @post_load
     def make_resource(self, data, **kwargs):
         """Generate resource."""
         return AdditionalIamPolicy(**data)
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/schemas/imagebuilder_schema.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/schemas/imagebuilder_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Iam,
     Image,
     ImageBuilderConfig,
     ImagebuilderDevSettings,
     UpdateOsPackages,
     Volume,
 )
-from pcluster.constants import PCLUSTER_IMAGE_NAME_REGEX
+from pcluster.constants import IAM_INSTANCE_PROFILE_REGEX, IAM_POLICY_REGEX, IAM_ROLE_REGEX, PCLUSTER_IMAGE_NAME_REGEX
 from pcluster.imagebuilder_utils import AMI_NAME_REQUIRED_SUBSTRING
 from pcluster.schemas.common_schema import (
     ALLOWED_VALUES,
     AdditionalIamPolicySchema,
     BaseDevSettingsSchema,
     BaseSchema,
     DeploymentSettingsSchema,
@@ -131,19 +131,19 @@
         if value and not validate_json_format(value):
             raise ValidationError(message="'{0}' is invalid".format(value))
 
 
 class IamSchema(BaseSchema):
     """Represent the schema of the ImageBuilder IAM."""
 
-    instance_role = fields.Str(validate=validate.Regexp("^arn:.*:role/"))
-    instance_profile = fields.Str(validate=validate.Regexp("^arn:.*:instance-profile/"))
-    cleanup_lambda_role = fields.Str(validate=validate.Regexp("^arn:.*:role/"))
+    instance_role = fields.Str(validate=validate.Regexp(IAM_ROLE_REGEX))
+    instance_profile = fields.Str(validate=validate.Regexp(IAM_INSTANCE_PROFILE_REGEX))
+    cleanup_lambda_role = fields.Str(validate=validate.Regexp(IAM_ROLE_REGEX))
     additional_iam_policies = fields.Nested(AdditionalIamPolicySchema, many=True)
-    permissions_boundary = fields.Str(validate=validate.Regexp("^arn:.*:policy/"))
+    permissions_boundary = fields.Str(validate=validate.Regexp(IAM_POLICY_REGEX))
 
     @validates_schema
     def no_coexist_role_policies(self, data, **kwargs):
         """Validate that instance_role, instance_profile or additional_iam_policies do not co-exist."""
         if self.fields_coexist(data, ["instance_role", "instance_profile", "additional_iam_policies"], **kwargs):
             raise ValidationError(
                 "InstanceProfile, InstanceRole or AdditionalIamPolicies can not be configured together."
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/templates/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/templates/awsbatch_builder.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/templates/awsbatch_builder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/templates/cdk_artifacts_manager.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/templates/cdk_artifacts_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/templates/cdk_builder.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/templates/cdk_builder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/templates/cdk_builder_utils.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/templates/cdk_builder_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # with the License. A copy of the License is located at
 #
 # http://aws.amazon.com/apache2.0/
 #
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
+
+# pylint: disable=too-many-lines
 import abc
 import hashlib
 from hashlib import sha1
 from typing import List, Union
 
 import pkg_resources
 from aws_cdk import aws_ec2 as ec2
@@ -22,14 +24,15 @@
 from aws_cdk.core import Arn, ArnFormat, CfnDeletionPolicy, CfnTag, Construct, Fn, Stack
 
 from pcluster.config.cluster_config import (
     BaseClusterConfig,
     BaseComputeResource,
     BaseQueue,
     HeadNode,
+    LoginNodesPool,
     SharedStorageType,
     SlurmClusterConfig,
     SlurmComputeResource,
     SlurmQueue,
 )
 from pcluster.constants import (
     COOKBOOK_PACKAGES_VERSIONS,
@@ -39,18 +42,16 @@
     PCLUSTER_CLUSTER_NAME_TAG,
     PCLUSTER_DYNAMODB_PREFIX,
     PCLUSTER_NODE_TYPE_TAG,
 )
 from pcluster.launch_template_utils import _LaunchTemplateBuilder
 from pcluster.models.s3_bucket import S3Bucket, parse_bucket_url
 from pcluster.utils import (
-    get_attr,
     get_installed_version,
     get_resource_name_from_resource_arn,
-    get_url_scheme,
     policy_name_to_arn,
     split_resource_prefix,
 )
 
 PCLUSTER_LAMBDA_PREFIX = "pcluster-"
 
 
@@ -70,15 +71,15 @@
     """Retrieve user data content."""
     user_data_file_path = pkg_resources.resource_filename(__name__, user_data_path)
     with open(user_data_file_path, "r", encoding="utf-8") as user_data_file:
         user_data_content = user_data_file.read()
     return user_data_content
 
 
-def get_common_user_data_env(node: Union[HeadNode, SlurmQueue], config: BaseClusterConfig) -> dict:
+def get_common_user_data_env(node: Union[HeadNode, SlurmQueue, LoginNodesPool], config: BaseClusterConfig) -> dict:
     """Return a dict containing the common env variables to be replaced in user data."""
     return {
         "YumProxy": node.networking.proxy.http_proxy_address if node.networking.proxy else "_none_",
         "DnfProxy": node.networking.proxy.http_proxy_address if node.networking.proxy else "",
         "AptProxy": node.networking.proxy.http_proxy_address if node.networking.proxy else "false",
         "ProxyServer": node.networking.proxy.http_proxy_address if node.networking.proxy else "NONE",
         "CustomChefCookbook": config.custom_chef_cookbook or "NONE",
@@ -152,15 +153,15 @@
     tags = {tag.key: tag.value for tag in custom_tags} if custom_tags else {}
     return tags if raw_dict else dict_to_cfn_tags(tags)
 
 
 def get_default_instance_tags(
     stack_name: str,
     config: BaseClusterConfig,
-    node: Union[HeadNode, BaseComputeResource],
+    node: Union[HeadNode, LoginNodesPool, BaseComputeResource],
     node_type: str,
     shared_storage_infos: dict,
     raw_dict: bool = False,
 ):
     """Return a list of default tags to be used for instances."""
     tags = {
         **get_cluster_tags(stack_name, raw_dict=True),
@@ -255,14 +256,34 @@
     # Additional security groups
     if queue.networking.additional_security_groups:
         queue_security_groups.extend(queue.networking.additional_security_groups)
 
     return queue_security_groups
 
 
+def get_login_nodes_security_groups_full(
+    managed_login_security_group: ec2.CfnSecurityGroup,
+    pool: LoginNodesPool,
+):
+    """Return full security groups to be used for the login node, default plus additional ones."""
+    login_nodes_security_groups = []
+
+    # Default security groups, created by us or provided by the user
+    if pool.networking.security_groups:
+        login_nodes_security_groups.extend(pool.networking.security_groups)
+    else:
+        login_nodes_security_groups.append(managed_login_security_group.ref)
+
+    # Additional security groups
+    if pool.networking.additional_security_groups:
+        login_nodes_security_groups.extend(pool.networking.additional_security_groups)
+
+    return login_nodes_security_groups
+
+
 def add_cluster_iam_resource_prefix(stack_name, config, name: str, iam_type: str):
     """Return a path and Name prefix from the Resource prefix config option."""
     full_resource_path = None
     full_resource_name = None
     if config.iam and config.iam.resource_prefix:
         iam_path, iam_name_prefix = split_resource_prefix(config.iam.resource_prefix)
         if iam_name_prefix:
@@ -333,25 +354,30 @@
     """Abstract construct defining IAM resources for a cluster node."""
 
     def __init__(
         self,
         scope: Construct,
         id: str,
         config: BaseClusterConfig,
-        node: Union[HeadNode, BaseQueue],
+        node: Union[HeadNode, BaseQueue, LoginNodesPool],
         shared_storage_infos: dict,
         name: str,
     ):
         super().__init__(scope, id)
         self._config = config
         self.instance_role = None
 
         self._add_role_and_policies(node, shared_storage_infos, name)
 
-    def _add_role_and_policies(self, node: Union[HeadNode, BaseQueue], shared_storage_infos: dict, name: str):
+    def _add_role_and_policies(
+        self,
+        node: Union[HeadNode, BaseQueue, LoginNodesPool],
+        shared_storage_infos: dict,
+        name: str,
+    ):
         """Create role and policies for the given node/queue."""
         suffix = create_hash_suffix(name)
         if node.instance_profile:
             # If existing InstanceProfile provided, do not create InstanceRole
             self.instance_profile = get_resource_name_from_resource_arn(node.instance_profile)
         elif node.instance_role:
             node_role_ref = get_resource_name_from_resource_arn(node.instance_role)
@@ -365,15 +391,15 @@
             )
 
             # Custom Cookbook S3 url policy
             if self._condition_custom_cookbook_with_s3_url():
                 self._add_custom_cookbook_policies_to_role(self.instance_role.ref, f"CustomCookbookPolicies{suffix}")
 
             # S3 Access Policies
-            if self._condition_create_s3_access_policies(node):
+            if isinstance(node, (BaseQueue, HeadNode)) and self._condition_create_s3_access_policies(node):
                 self._add_s3_access_policies_to_role(node, self.instance_role.ref, f"S3AccessPolicies{suffix}")
 
             # Head node Instance Profile
             self.instance_profile = self._add_instance_profile(self.instance_role.ref, f"InstanceProfile{suffix}")
 
     def _add_instance_profile(self, role_ref: str, name: str):
         instance_profile_path, instance_profile_name = add_cluster_iam_resource_prefix(
@@ -383,15 +409,15 @@
             Stack.of(self),
             name,
             roles=[role_ref],
             path=self._cluster_scoped_iam_path(iam_path=instance_profile_path),
             instance_profile_name=instance_profile_name,
         ).ref
 
-    def _add_node_role(self, node: Union[HeadNode, BaseQueue], name: str):
+    def _add_node_role(self, node: Union[HeadNode, BaseQueue, LoginNodesPool], name: str):
         role_path, role_name = add_cluster_iam_resource_prefix(
             self._config.cluster_name, self._config, name, iam_type="AWS::IAM::Role"
         )
         additional_iam_policies = set(node.iam.additional_iam_policy_arns)
         if self._config.monitoring.logs.cloud_watch.enabled:
             additional_iam_policies.add(policy_name_to_arn("CloudWatchAgentServerPolicy"))
         return iam.CfnRole(
@@ -445,15 +471,15 @@
 
     def _condition_custom_cookbook_with_s3_url(self):
         try:
             return self._config.dev_settings.cookbook.chef_cookbook.startswith("s3://")
         except AttributeError:
             return False
 
-    def _condition_create_s3_access_policies(self, node: Union[HeadNode, BaseQueue]):
+    def _condition_create_s3_access_policies(self, node: Union[HeadNode, BaseQueue, LoginNodesPool]):
         return node.iam and node.iam.s3_access
 
     def _add_custom_cookbook_policies_to_role(self, role_ref: str, name: str):
         bucket_info = parse_bucket_url(self._config.dev_settings.cookbook.chef_cookbook)
         bucket_name = bucket_info.get("bucket_name")
         object_key = bucket_info.get("object_key")
         iam.CfnPolicy(
@@ -477,15 +503,17 @@
                         resources=[self._format_arn(service="s3", resource=bucket_name, region="", account="")],
                     ),
                 ]
             ),
             roles=[role_ref],
         )
 
-    def _add_s3_access_policies_to_role(self, node: Union[HeadNode, BaseQueue], role_ref: str, name: str):
+    def _add_s3_access_policies_to_role(
+        self, node: Union[HeadNode, BaseQueue, LoginNodesPool], role_ref: str, name: str
+    ):
         """Attach S3 policies to given role."""
         read_only_s3_resources = []
         read_write_s3_resources = []
         for s3_access in node.iam.s3_access:
             for resource in s3_access.resource_regex:
                 arn = self._format_arn(service="s3", resource=resource, region="", account="")
                 if s3_access.enable_write_access:
@@ -540,15 +568,15 @@
     """Construct defining IAM resources for the head node."""
 
     def __init__(
         self,
         scope: Construct,
         id: str,
         config: BaseClusterConfig,
-        node: Union[HeadNode, BaseQueue],
+        node: Union[HeadNode, BaseQueue, LoginNodesPool],
         shared_storage_infos: dict,
         name: str,
         cluster_bucket: S3Bucket,
     ):
         self._cluster_bucket = cluster_bucket
         super().__init__(scope, id, config, node, shared_storage_infos, name)
 
@@ -724,42 +752,14 @@
                             actions=["ec2:RunInstances", "ec2:CreateFleet", "resource-groups:ListGroupResources"],
                             effect=iam.Effect.ALLOW,
                             resources=capacity_reservation_resource_group_arns,
                         )
                     ]
                 )
 
-        if self._config.scheduling.scheduler == "plugin":
-            cluster_shared_artifacts = get_attr(
-                self._config, "scheduling.settings.scheduler_definition.plugin_resources.cluster_shared_artifacts"
-            )
-            if cluster_shared_artifacts:
-                for artifacts in cluster_shared_artifacts:
-                    if get_url_scheme(artifacts.source) == "s3":
-                        bucket_info = parse_bucket_url(artifacts.source)
-                        bucket_name = bucket_info.get("bucket_name")
-                        object_key = bucket_info.get("object_key")
-                        policy.extend(
-                            [
-                                iam.PolicyStatement(
-                                    actions=["s3:GetObject"],
-                                    effect=iam.Effect.ALLOW,
-                                    resources=[
-                                        self._format_arn(
-                                            region="",
-                                            service="s3",
-                                            account="",
-                                            resource=bucket_name,
-                                            resource_name=object_key,
-                                        )
-                                    ],
-                                ),
-                            ]
-                        )
-
         if self._config.directory_service:
             password_secret_arn = Arn.split(
                 self._config.directory_service.password_secret_arn, ArnFormat.COLON_RESOURCE_NAME
             )
             policy.append(
                 iam.PolicyStatement(
                     sid="AllowGettingDirectorySecretValue",
@@ -833,23 +833,76 @@
             if any(queues_without_custom_roles):
                 pass_role_resources.add(default_pass_role_resource)
         else:
             pass_role_resources = {default_pass_role_resource}
         return list(pass_role_resources)
 
 
+class LoginNodesIamResources(NodeIamResourcesBase):
+    """Construct defining IAM resources for a login node."""
+
+    def __init__(
+        self,
+        scope: Construct,
+        id: str,
+        config: BaseClusterConfig,
+        node: Union[HeadNode, BaseQueue, LoginNodesPool],
+        shared_storage_infos: dict,
+        name: str,
+        auto_scaling_group_name: str,
+    ):
+        self._auto_scaling_group_name = auto_scaling_group_name
+        super().__init__(scope, id, config, node, shared_storage_infos, name)
+
+    def _build_policy(self) -> List[iam.PolicyStatement]:
+        return [
+            iam.PolicyStatement(
+                sid="Ec2",
+                actions=["ec2:DescribeInstanceAttribute"],
+                effect=iam.Effect.ALLOW,
+                resources=["*"],
+            ),
+            iam.PolicyStatement(
+                sid="S3GetObj",
+                actions=["s3:GetObject"],
+                effect=iam.Effect.ALLOW,
+                resources=[
+                    self._format_arn(
+                        service="s3",
+                        resource="{0}-aws-parallelcluster/*".format(Stack.of(self).region),
+                        region="",
+                        account="",
+                    )
+                ],
+            ),
+            iam.PolicyStatement(
+                sid="Autoscaling",
+                actions=[
+                    "autoscaling:CompleteLifecycleAction",
+                ],
+                effect=iam.Effect.ALLOW,
+                resources=[
+                    self._format_arn(
+                        service="autoscaling",
+                        resource=f"autoScalingGroupName/{self._auto_scaling_group_name}",
+                    )
+                ],
+            ),
+        ]
+
+
 class ComputeNodeIamResources(NodeIamResourcesBase):
     """Construct defining IAM resources for a compute node."""
 
     def __init__(
         self,
         scope: Construct,
         id: str,
         config: BaseClusterConfig,
-        node: Union[HeadNode, BaseQueue],
+        node: Union[HeadNode, BaseQueue, LoginNodesPool],
         shared_storage_infos: dict,
         name: str,
     ):
         super().__init__(scope, id, config, node, shared_storage_infos, name)
 
     def _build_policy(self) -> List[iam.PolicyStatement]:
         return [
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/templates/cluster_stack.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/templates/cluster_stack.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 #
 # or in the "LICENSE.txt" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint: disable=too-many-lines
 
+import collections.abc
+
 #
 # This module contains all the classes required to convert a Cluster into a CFN template by using CDK.
 #
 import json
 from collections import defaultdict, namedtuple
 from datetime import datetime
 from typing import Union
@@ -34,54 +36,60 @@
     CfnStack,
     CfnTag,
     Construct,
     CustomResource,
     Duration,
     Fn,
     Stack,
+    Tags,
 )
 
 from pcluster.aws.aws_api import AWSApi
 from pcluster.aws.common import AWSClientError
 from pcluster.config.cluster_config import (
     AwsBatchClusterConfig,
     BaseSharedFsx,
+    ExistingFsxFileCache,
     ExistingFsxOntap,
     ExistingFsxOpenZfs,
     SharedEbs,
     SharedEfs,
     SharedFsxLustre,
     SharedStorageType,
     SlurmClusterConfig,
 )
 from pcluster.constants import (
+    ALL_PORTS_RANGE,
     CW_ALARM_DATAPOINTS_TO_ALARM_DEFAULT,
     CW_ALARM_EVALUATION_PERIODS_DEFAULT,
     CW_ALARM_PERCENT_THRESHOLD_DEFAULT,
     CW_ALARM_PERIOD_DEFAULT,
     CW_LOG_GROUP_NAME_PREFIX,
     CW_LOGS_CFN_PARAM_NAME,
     DEFAULT_EPHEMERAL_DIR,
+    EFS_PORT,
+    FSX_PORTS,
     LUSTRE,
+    NFS_PORT,
     NODE_BOOTSTRAP_TIMEOUT,
     OS_MAPPING,
     PCLUSTER_DYNAMODB_PREFIX,
     PCLUSTER_S3_ARTIFACTS_DICT,
+    SLURM_PORTS_RANGE,
 )
 from pcluster.models.s3_bucket import S3Bucket
 from pcluster.templates.awsbatch_builder import AwsBatchConstruct
 from pcluster.templates.cdk_builder_utils import (
     CdkLaunchTemplateBuilder,
     HeadNodeIamResources,
     PclusterLambdaConstruct,
     add_lambda_cfn_role,
     apply_permissions_boundary,
     convert_deletion_policy,
     create_hash_suffix,
-    generate_launch_template_version_cfn_parameter_hash,
     get_cloud_watch_logs_policy_statement,
     get_cloud_watch_logs_retention_days,
     get_common_user_data_env,
     get_custom_tags,
     get_default_instance_tags,
     get_default_volume_tags,
     get_directory_service_dna_json_for_head_node,
@@ -90,14 +98,15 @@
     get_shared_storage_ids_by_type,
     get_slurm_specific_dna_json_for_head_node,
     get_user_data_content,
     to_comma_separated_string,
 )
 from pcluster.templates.compute_fleet_stack import ComputeFleetConstruct
 from pcluster.templates.cw_dashboard_builder import CWDashboardConstruct
+from pcluster.templates.login_nodes_stack import LoginNodesStack
 from pcluster.templates.slurm_builder import SlurmConstruct
 from pcluster.utils import get_attr, get_http_tokens_setting, get_service_endpoint
 
 StorageInfo = namedtuple("StorageInfo", ["id", "config"])
 
 
 class ClusterCdkStack:
@@ -167,27 +176,31 @@
         """Return list of security groups to be used for the compute, created by us AND provided by the user."""
         compute_group_set = self.config.compute_security_groups
         if self._compute_security_group:
             compute_group_set.append(self._compute_security_group.ref)
 
         return compute_group_set
 
-    def _generate_compute_fleet_role_names_cfn_parameter(self):
-        """
-        Generate compute fleet role names.
-
-        Return a comma separate string for compute fleet role names cfn parameter
-        in Scheduler Plugin cfn substack template.
-        """
-        role_list = []
-        for _, instance_role in self.compute_fleet_resources.managed_compute_instance_roles.items():
-            if instance_role is None:
-                continue
-            role_list.append(instance_role)
-        return ",".join([instance_role.ref for instance_role in role_list])
+    def _get_login_security_groups(self):
+        """Return list of security groups to be used for the login nodes, created by us AND provided by the user."""
+        login_security_groups = (
+            [
+                security_group
+                for pool in self.config.login_nodes.pools
+                if pool.networking.security_groups
+                for security_group in pool.networking.security_groups
+            ]
+            if isinstance(self.config, SlurmClusterConfig) and self.config.login_nodes
+            else []
+        )
+
+        if self._login_security_group:
+            login_security_groups.append(self._login_security_group.ref)
+
+        return login_security_groups
 
     # -- Parameters -------------------------------------------------------------------------------------------------- #
 
     def _add_parameters(self):
         CfnParameter(
             self.stack,
             "ClusterUser",
@@ -234,16 +247,19 @@
     def _add_resources(self):
         # Cloud Watch Logs
         self.log_group = None
         if self.config.is_cw_logging_enabled:
             self.log_group = self._add_cluster_log_group()
 
         # Managed security groups
-        self._head_security_group, self._compute_security_group = self._add_security_groups()
-
+        (
+            self._head_security_group,
+            self._compute_security_group,
+            self._login_security_group,
+        ) = self._add_security_groups()
         # Head Node ENI
         self._head_eni = self._add_head_eni()
 
         if self.config.shared_storage:
             for storage in self.config.shared_storage:
                 self._add_shared_storage(storage)
 
@@ -263,14 +279,17 @@
 
         # Head Node
         self.head_node_instance = self._add_head_node()
         # Add a dependency to the cleanup Route53 resource, so that Route53 Hosted Zone is cleaned after node is deleted
         if self._condition_is_slurm() and hasattr(self.scheduler_resources, "cleanup_route53_custom_resource"):
             self.head_node_instance.add_depends_on(self.scheduler_resources.cleanup_route53_custom_resource)
 
+        # Initialize Login Nodes
+        self._add_login_nodes_resources()
+
         # AWS Batch related resources
         if self._condition_is_batch():
             self.scheduler_resources = AwsBatchConstruct(
                 scope=self.stack,
                 id="AwsBatch",
                 stack_name=self._stack_name,
                 cluster_config=self.config,
@@ -399,15 +418,39 @@
                 shared_storage_mount_dirs=self.shared_storage_mount_dirs,
                 shared_storage_attributes=self.shared_storage_attributes,
                 cluster_hosted_zone=self.scheduler_resources.cluster_hosted_zone if self.scheduler_resources else None,
                 dynamodb_table=self.scheduler_resources.dynamodb_table if self.scheduler_resources else None,
                 head_eni=self._head_eni,
                 slurm_construct=self.scheduler_resources,
             )
-        self._add_scheduler_plugin_substack()
+
+    def _add_login_nodes_resources(self):
+        """Add Login Nodes related resources."""
+        self.login_nodes_stack = None
+        if self._condition_is_slurm() and self.config.login_nodes:
+            self.login_nodes_stack = LoginNodesStack(
+                scope=self.stack,
+                id="LoginNodes",
+                cluster_config=self.config,
+                log_group=self.log_group,
+                shared_storage_infos=self.shared_storage_infos,
+                shared_storage_mount_dirs=self.shared_storage_mount_dirs,
+                shared_storage_attributes=self.shared_storage_attributes,
+                login_security_group=self._login_security_group,
+                head_eni=self._head_eni,
+                cluster_hosted_zone=self.scheduler_resources.cluster_hosted_zone if self.scheduler_resources else None,
+            )
+            Tags.of(self.login_nodes_stack).add(
+                # This approach works since by design we have now only one pool.
+                # We should fix this if we want to add more than a login nodes pool per cluster.
+                "parallelcluster:login-nodes-pool",
+                self.config.login_nodes.pools[0].name,
+            )
+            # Add dependency on the Head Node construct
+            self.login_nodes_stack.node.add_dependency(self.head_node_instance)
 
     def _add_cleanup_resources_lambda(self):
         """Create Lambda cleanup resources function and its role."""
         cleanup_resources_lambda_role = None
         if self._condition_create_lambda_iam_role():
             s3_policy_actions = ["s3:DeleteObject", "s3:DeleteObjectVersion", "s3:ListBucket", "s3:ListBucketVersions"]
 
@@ -491,84 +534,198 @@
             ec2.CfnEIPAssociation(
                 self.stack, "AssociateEIP", allocation_id=allocation_id, network_interface_id=head_eni.ref
             )
 
         return head_eni
 
     def _add_security_groups(self):
-        """Associate security group to Head node and queues."""
-        # Head Node Security Group
+        head_node_security_groups, managed_head_security_group = self._head_security_groups()
+        (
+            login_security_groups,
+            managed_login_security_group,
+            custom_login_security_groups,
+        ) = self._login_security_groups()
+        (
+            compute_security_groups,
+            managed_compute_security_group,
+            custom_compute_security_groups,
+        ) = self._compute_security_groups()
+
+        self._add_inbounds_to_managed_security_groups(
+            compute_security_groups,
+            custom_compute_security_groups,
+            head_node_security_groups,
+            login_security_groups,
+            custom_login_security_groups,
+            managed_compute_security_group,
+            managed_head_security_group,
+            managed_login_security_group,
+        )
+
+        return managed_head_security_group, managed_compute_security_group, managed_login_security_group
+
+    def _head_security_groups(self):
         managed_head_security_group = None
         custom_head_security_groups = self.config.head_node.networking.security_groups or []
         if not custom_head_security_groups:
             managed_head_security_group = self._add_head_security_group()
             head_node_security_groups = [managed_head_security_group.ref]
         else:
             head_node_security_groups = custom_head_security_groups
+        return head_node_security_groups, managed_head_security_group
 
-        # Compute Security Groups
+    def _login_security_groups(self):
+        managed_login_security_group = None
+        custom_login_security_groups = set()
+        managed_login_security_group_required = False
+        if self._condition_is_slurm() and self.config.login_nodes:
+            for pool in self.config.login_nodes.pools:
+                pool_security_groups = pool.networking.security_groups
+                if pool_security_groups:
+                    for security_group in pool_security_groups:
+                        custom_login_security_groups.add(security_group)
+                else:
+                    managed_login_security_group_required = True
+        login_security_groups = list(custom_login_security_groups)
+        if managed_login_security_group_required:
+            managed_login_security_group = self._add_login_nodes_security_group()
+            login_security_groups.append(managed_login_security_group.ref)
+        return login_security_groups, managed_login_security_group, custom_login_security_groups
+
+    def _compute_security_groups(self):
         managed_compute_security_group = None
         custom_compute_security_groups = set()
         managed_compute_security_group_required = False
         for queue in self.config.scheduling.queues:
             queue_security_groups = queue.networking.security_groups
             if queue_security_groups:
                 for security_group in queue_security_groups:
                     custom_compute_security_groups.add(security_group)
             else:
                 managed_compute_security_group_required = True
         compute_security_groups = list(custom_compute_security_groups)
         if managed_compute_security_group_required:
             managed_compute_security_group = self._add_compute_security_group()
             compute_security_groups.append(managed_compute_security_group.ref)
-
-        self._add_inbounds_to_managed_security_groups(
-            compute_security_groups,
-            custom_compute_security_groups,
-            head_node_security_groups,
-            managed_compute_security_group,
-            managed_head_security_group,
-        )
-
-        return managed_head_security_group, managed_compute_security_group
+        return compute_security_groups, managed_compute_security_group, custom_compute_security_groups
 
     def _add_inbounds_to_managed_security_groups(
         self,
         compute_security_groups,
         custom_compute_security_groups,
         head_node_security_groups,
+        login_security_groups,
+        custom_login_security_groups,
         managed_compute_security_group,
         managed_head_security_group,
+        managed_login_security_group,
+    ):
+        self._add_inbounds_to_managed_head_security_group(
+            compute_security_groups, login_security_groups, managed_head_security_group
+        )
+
+        self._add_inbounds_to_managed_login_security_group(
+            head_node_security_groups,
+            compute_security_groups,
+            custom_login_security_groups,
+            managed_login_security_group,
+        )
+
+        self._add_inbounds_to_managed_compute_security_group(
+            head_node_security_groups,
+            login_security_groups,
+            custom_compute_security_groups,
+            managed_compute_security_group,
+        )
+
+    def _add_inbounds_to_managed_head_security_group(
+        self, compute_security_groups, login_security_groups, managed_head_security_group
     ):
         if managed_head_security_group:
             for index, security_group in enumerate(compute_security_groups):
                 # Access to head node from compute nodes
                 self._allow_all_ingress(
                     f"HeadNodeSecurityGroupComputeIngress{index}", security_group, managed_head_security_group.ref
                 )
+            for index, security_group in enumerate(login_security_groups):
+                # Access to head node from login nodes
+                self._allow_all_ingress(
+                    f"HeadNodeSecurityGroupLoginSlurmIngress{index}",
+                    security_group,
+                    managed_head_security_group.ref,
+                    ip_protocol="tcp",
+                    port=SLURM_PORTS_RANGE,
+                )
+                self._allow_all_ingress(
+                    f"HeadNodeSecurityGroupLoginNfsIngress{index}",
+                    security_group,
+                    managed_head_security_group.ref,
+                    ip_protocol="tcp",
+                    port=NFS_PORT,
+                )
+
+    def _add_inbounds_to_managed_login_security_group(
+        self,
+        head_node_security_groups,
+        compute_security_groups,
+        custom_login_security_groups,
+        managed_login_security_group,
+    ):
+        if managed_login_security_group:
+            # Access to login nodes from head node and compute nodes
+            for index, security_group in enumerate(head_node_security_groups):
+                self._allow_all_ingress(
+                    f"LoginSecurityGroupHeadNodeIngress{index}", security_group, managed_login_security_group.ref
+                )
+            for index, security_group in enumerate(compute_security_groups):
+                self._allow_all_ingress(
+                    f"LoginSecurityGroupComputeIngress{index}", security_group, managed_login_security_group.ref
+                )
+            for index, security_group in enumerate(custom_login_security_groups):
+                self._allow_all_ingress(
+                    f"LoginSecurityGroupCustomLoginSecurityGroupIngress{index}",
+                    security_group,
+                    managed_login_security_group.ref,
+                )
+
+    def _add_inbounds_to_managed_compute_security_group(
+        self,
+        head_node_security_groups,
+        login_security_groups,
+        custom_compute_security_groups,
+        managed_compute_security_group,
+    ):
         if managed_compute_security_group:
-            # Access to compute nodes from head node
+            # Access to compute nodes from head node and login nodes
             for index, security_group in enumerate(head_node_security_groups):
                 self._allow_all_ingress(
-                    f"ComputeSecurityGroupHeadNodeIngress{index}", security_group, managed_compute_security_group.ref
+                    f"ComputeSecurityGroupHeadNodeIngress{index}",
+                    security_group,
+                    managed_compute_security_group.ref,
+                )
+            for index, security_group in enumerate(login_security_groups):
+                self._allow_all_ingress(
+                    f"ComputeSecurityGroupLoginIngress{index}",
+                    security_group,
+                    managed_compute_security_group.ref,
                 )
             for index, security_group in enumerate(custom_compute_security_groups):
                 self._allow_all_ingress(
                     f"ComputeSecurityGroupCustomComputeSecurityGroupIngress{index}",
                     security_group,
                     managed_compute_security_group.ref,
                 )
 
-    def _allow_all_ingress(self, description, source_security_group_id, group_id):
+    def _allow_all_ingress(self, description, source_security_group_id, group_id, ip_protocol="-1", port=(0, 65535)):
         return ec2.CfnSecurityGroupIngress(
             self.stack,
             description,
-            ip_protocol="-1",
-            from_port=0,
-            to_port=65535,
+            ip_protocol=ip_protocol,
+            from_port=port[0] if isinstance(port, collections.abc.Sequence) else port,
+            to_port=port[1] if isinstance(port, collections.abc.Sequence) else port,
             source_security_group_id=source_security_group_id,
             group_id=group_id,
         )
 
     def _allow_all_egress(self, description, destination_security_group_id, group_id):
         return ec2.CfnSecurityGroupEgress(
             self.stack,
@@ -592,23 +749,37 @@
         storage_security_group.cfn_options.deletion_policy = (
             storage_security_group.cfn_options.update_replace_policy
         ) = storage_deletion_policy
 
         target_security_groups = {
             "Head": self._get_head_node_security_groups(),
             "Compute": self._get_compute_security_groups(),
+            "Login": self._get_login_security_groups(),
             "Storage": [storage_security_group.ref],
         }
 
         for sg_type, sg_refs in target_security_groups.items():
             for sg_ref_id, sg_ref in enumerate(sg_refs):
+                # TODO Scope down ingress rules to allow only traffic on the strictly necessary ports.
+                #      Currently scoped down only on Login nodes to limit blast radius.
+                ingress_protocol = "-1"
+                ingress_port = ALL_PORTS_RANGE
+                if sg_type == "Login":
+                    if storage_type == SharedStorageType.EFS:
+                        ingress_protocol = "tcp"
+                        ingress_port = EFS_PORT
+                    elif storage_type == SharedStorageType.FSX:
+                        ingress_protocol = "tcp"
+                        ingress_port = FSX_PORTS[LUSTRE]["tcp"][0]
                 ingress_rule = self._allow_all_ingress(
                     description=f"{storage_cfn_id}SecurityGroup{sg_type}Ingress{sg_ref_id}",
                     source_security_group_id=sg_ref,
                     group_id=storage_security_group.ref,
+                    ip_protocol=ingress_protocol,
+                    port=ingress_port,
                 )
 
                 egress_rule = self._allow_all_egress(
                     description=f"{storage_cfn_id}SecurityGroup{sg_type}Egress{sg_ref_id}",
                     destination_security_group_id=sg_ref,
                     group_id=storage_security_group.ref,
                 )
@@ -665,14 +836,32 @@
             to_port=65535,
             source_security_group_id=compute_security_group.ref,
             group_id=compute_security_group.ref,
         )
 
         return compute_security_group
 
+    def _add_login_nodes_security_group(self):
+        login_nodes_security_group_ingress = [
+            # SSH access
+            ec2.CfnSecurityGroup.IngressProperty(
+                ip_protocol="tcp",
+                from_port=22,
+                to_port=22,
+                cidr_ip="0.0.0.0/0",
+            )
+        ]
+        return ec2.CfnSecurityGroup(
+            self.stack,
+            "LoginNodesSecurityGroup",
+            group_description="Enable access to the login nodes",
+            vpc_id=self.config.vpc_id,
+            security_group_ingress=login_nodes_security_group_ingress,
+        )
+
     def _add_head_security_group(self):
         head_security_group_ingress = [
             # SSH access
             ec2.CfnSecurityGroup.IngressProperty(
                 ip_protocol="tcp", from_port=22, to_port=22, cidr_ip=self.config.head_node.ssh.allowed_ips
             )
         ]
@@ -707,26 +896,33 @@
             storage_list.append(StorageInfo(self._add_efs_storage(cfn_resource_id, storage), storage))
         elif storage.shared_storage_type == SharedStorageType.RAID:
             storage_list.extend(self._add_raid_volume(cfn_resource_id, storage))
         self.shared_storage_mount_dirs[storage.shared_storage_type].append(storage.mount_dir)
 
     def _add_fsx_storage(self, id: str, shared_fsx: BaseSharedFsx):
         """Add specific Cfn Resources to map the FSX storage."""
-        fsx_id = shared_fsx.file_system_id if isinstance(shared_fsx, SharedFsxLustre) else shared_fsx.volume_id
+        if isinstance(shared_fsx, SharedFsxLustre):
+            fsx_id = shared_fsx.file_system_id
+        elif isinstance(shared_fsx, ExistingFsxFileCache):
+            fsx_id = shared_fsx.file_cache_id
+        else:
+            fsx_id = shared_fsx.volume_id
         mount_name = ""
         dns_name = ""
         volume_junction_path = ""
         if fsx_id:
             dns_name = shared_fsx.existing_dns_name
             if isinstance(shared_fsx, ExistingFsxOntap):
                 volume_junction_path = shared_fsx.junction_path
             if isinstance(shared_fsx, ExistingFsxOpenZfs):
                 volume_junction_path = shared_fsx.volume_path
             if isinstance(shared_fsx, SharedFsxLustre):
                 mount_name = shared_fsx.existing_mount_name
+            if isinstance(shared_fsx, ExistingFsxFileCache):
+                mount_name = shared_fsx.file_cache_mount_name
         else:
             # Drive cache type must be set for HDD (Either "NONE" or "READ"), and must not be set for SDD (None).
             drive_cache_type = None
             if shared_fsx.fsx_storage_type == "HDD":
                 if shared_fsx.drive_cache_type:
                     drive_cache_type = shared_fsx.drive_cache_type
                 else:
@@ -898,16 +1094,14 @@
             id="HeadNodeWaitCondition" + self.timestamp,
             count=1,
             handle=wait_condition_handle.ref,
             timeout=str(
                 get_attr(self.config, "dev_settings.timeouts.head_node_bootstrap_timeout", NODE_BOOTSTRAP_TIMEOUT)
             ),
         )
-        if self.scheduler_plugin_stack:
-            wait_condition.add_depends_on(self.scheduler_plugin_stack)
         return wait_condition, wait_condition_handle
 
     def _add_head_node(self):
         head_node = self.config.head_node
         head_lt_security_groups = self._get_head_node_security_groups_full()
 
         # LT network interfaces
@@ -977,17 +1171,14 @@
         # CloudFormation::Init metadata
 
         dna_json = json.dumps(
             {
                 "cluster": {
                     "stack_name": self._stack_name,
                     "stack_arn": self.stack.stack_id,
-                    "scheduler_plugin_substack_arn": self.scheduler_plugin_stack.ref
-                    if self.scheduler_plugin_stack
-                    else "",
                     "raid_vol_ids": get_shared_storage_ids_by_type(self.shared_storage_infos, SharedStorageType.RAID),
                     "raid_shared_dir": to_comma_separated_string(
                         self.shared_storage_mount_dirs[SharedStorageType.RAID]
                     ),
                     "raid_type": to_comma_separated_string(
                         self.shared_storage_attributes[SharedStorageType.RAID]["Type"]
                     ),
@@ -1170,15 +1361,15 @@
             "chefPrepEnv": {
                 "commands": {
                     "chef": {
                         "command": (
                             "cinc-client --local-mode --config /etc/chef/client.rb --log_level info "
                             "--logfile /var/log/chef-client.log --force-formatter --no-color "
                             "--chef-zero-port 8889 --json-attributes /etc/chef/dna.json "
-                            "--override-runlist aws-parallelcluster::init"
+                            "--override-runlist aws-parallelcluster-entrypoints::init"
                         ),
                         "cwd": "/etc/chef",
                     }
                 }
             },
             "shellRunPreInstall": {
                 "commands": {"runpreinstall": {"command": "/opt/parallelcluster/scripts/fetch_and_run -preinstall"}}
@@ -1186,15 +1377,15 @@
             "chefConfig": {
                 "commands": {
                     "chef": {
                         "command": (
                             "cinc-client --local-mode --config /etc/chef/client.rb --log_level info "
                             "--logfile /var/log/chef-client.log --force-formatter --no-color "
                             "--chef-zero-port 8889 --json-attributes /etc/chef/dna.json "
-                            "--override-runlist aws-parallelcluster::config"
+                            "--override-runlist aws-parallelcluster-entrypoints::config"
                         ),
                         "cwd": "/etc/chef",
                     }
                 }
             },
             "shellRunPostInstall": {
                 "commands": {"runpostinstall": {"command": "/opt/parallelcluster/scripts/fetch_and_run -postinstall"}}
@@ -1202,15 +1393,15 @@
             "chefFinalize": {
                 "commands": {
                     "chef": {
                         "command": (
                             "cinc-client --local-mode --config /etc/chef/client.rb --log_level info "
                             "--logfile /var/log/chef-client.log --force-formatter --no-color "
                             "--chef-zero-port 8889 --json-attributes /etc/chef/dna.json "
-                            "--override-runlist aws-parallelcluster::finalize"
+                            "--override-runlist aws-parallelcluster-entrypoints::finalize"
                         ),
                         "cwd": "/etc/chef",
                     },
                     "bootstrap": {
                         "command": (
                             "[ ! -f /opt/parallelcluster/.bootstrapped ] && echo ${cookbook_version} "
                             "| tee /opt/parallelcluster/.bootstrapped || exit 0"
@@ -1222,15 +1413,15 @@
                 "commands": {
                     "chef": {
                         "command": (
                             ". /etc/profile.d/pcluster.sh; "
                             "cinc-client --local-mode --config /etc/chef/client.rb --log_level info"
                             " --logfile /var/log/chef-client.log --force-formatter --no-color"
                             " --chef-zero-port 8889 --json-attributes /etc/chef/dna.json"
-                            " --override-runlist aws-parallelcluster::update &&"
+                            " --override-runlist aws-parallelcluster-entrypoints::update &&"
                             " /opt/parallelcluster/scripts/fetch_and_run -postupdate &&"
                             f" cfn-signal --exit-code=0 --reason='Update complete'"
                             f" --region {self.stack.region} --url {cloudformation_url}"
                             f" '{self.wait_condition_handle.ref}' ||"
                             f" cfn-signal --exit-code=1 --reason='Update failed'"
                             f" --region {self.stack.region} --url {cloudformation_url}"
                             f" '{self.wait_condition_handle.ref}'"
@@ -1261,17 +1452,14 @@
                 self._stack_name, self.config, head_node, "HeadNode", self.shared_storage_infos
             )
             + get_custom_tags(self.config),
         )
         if not self._condition_is_batch():
             head_node_instance.node.add_dependency(self.compute_fleet_resources)
 
-        if self._condition_is_scheduler_plugin() and self.scheduler_plugin_stack:
-            head_node_instance.add_depends_on(self.scheduler_plugin_stack)
-
         return head_node_instance
 
     def _get_launch_templates_config(self):
         if not self.compute_fleet_resources:
             return None
 
         lt_config = {"Queues": {}}
@@ -1280,64 +1468,27 @@
             for compute_resource, launch_template in compute_resources.items():
                 lt_config["Queues"][queue]["ComputeResources"][compute_resource] = {
                     "LaunchTemplate": {"Id": launch_template.ref, "Version": launch_template.attr_latest_version_number}
                 }
 
         return lt_config
 
-    def _add_scheduler_plugin_substack(self):
-        self.scheduler_plugin_stack = None
-        if not self._condition_is_scheduler_plugin() or not get_attr(
-            self.config, "scheduling.settings.scheduler_definition.cluster_infrastructure.cloud_formation.template"
-        ):
-            return
-
-        template_url = self.bucket.get_cfn_template_url(
-            template_name=PCLUSTER_S3_ARTIFACTS_DICT.get("scheduler_plugin_template_name")
-        )
-
-        parameters = {
-            "ClusterName": self._stack_name,
-            "ParallelClusterStackId": self.stack.stack_id,
-            "VpcId": self.config.vpc_id,
-            # Empty if passed in config and not created by pclsuter
-            "HeadNodeRoleName": self._managed_head_node_instance_role.ref
-            if self._managed_head_node_instance_role
-            else "",
-            # Comma separated list of compute_fleet roles that are created by pcluster not the ones passed in config
-            "ComputeFleetRoleNames": self._generate_compute_fleet_role_names_cfn_parameter(),
-        }
-
-        for queue_name, queue in self._get_launch_templates_config()["Queues"].items():
-            for compute_resource_name, compute_resource in queue["ComputeResources"].items():
-                parameters[
-                    f"LaunchTemplate"
-                    f"{generate_launch_template_version_cfn_parameter_hash(queue_name, compute_resource_name)}Version"
-                ] = compute_resource["LaunchTemplate"]["Version"]
-
-        self.scheduler_plugin_stack = CfnStack(
-            self.stack, "SchedulerPluginStack", template_url=template_url, parameters=parameters
-        )
-
     # -- Conditions -------------------------------------------------------------------------------------------------- #
 
     def _condition_create_lambda_iam_role(self):
         return (
             not self.config.iam
             or not self.config.iam.roles
             or not self.config.iam.roles.lambda_functions_role
             or self.config.iam.roles.get_param("lambda_functions_role").implied
         )
 
     def _condition_is_slurm(self):
         return self.config.scheduling.scheduler == "slurm"
 
-    def _condition_is_scheduler_plugin(self):
-        return self.config.scheduling.scheduler == "plugin"
-
     def _condition_is_batch(self):
         return self.config.scheduling.scheduler == "awsbatch"
 
     # -- Outputs ----------------------------------------------------------------------------------------------------- #
 
     def _add_outputs(self):
         # Storage filesystem Ids
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/templates/compute_fleet_stack.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/templates/compute_fleet_stack.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/templates/cw_dashboard_builder.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/templates/cw_dashboard_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import Iterable
 
 from aws_cdk import aws_cloudwatch as cloudwatch
 from aws_cdk import aws_ec2 as ec2
 from aws_cdk import aws_logs as logs
 from aws_cdk.core import Construct, Duration, Stack
 
-from pcluster.config.cluster_config import BaseClusterConfig, SharedFsxLustre, SharedStorageType
+from pcluster.config.cluster_config import BaseClusterConfig, ExistingFsxFileCache, SharedFsxLustre, SharedStorageType
 from pcluster.constants import Feature
 from pcluster.utils import is_feature_supported
 
 MAX_WIDTH = 24
 
 
 class Coord:
@@ -465,14 +465,17 @@
         ]
         namespace = "AWS/FSx"
         metric_graphs = defaultdict(list)
         for index, storage in enumerate(storages_list):
             if isinstance(storage.config, SharedFsxLustre):
                 metrics = lustre_metrics
                 dimensions_map = {"FileSystemId": storage.id}
+            elif isinstance(storage.config, ExistingFsxFileCache):
+                metrics = lustre_metrics
+                dimensions_map = {"FileCacheId": storage.config.file_cache_id}
             else:
                 metrics = common_metrics
                 dimensions_map = {"FileSystemId": storage.config.file_system_id, "VolumeId": storage.id}
 
                 # FSx Ontap/OpenZFS do not provide free capacity metric. The code below generates the metric using math.
                 free_capacity_metric = cloudwatch.MathExpression(
                     label=f"{storage.id} FreeDataStorageCapacity",
@@ -703,15 +706,15 @@
                     self._new_cw_log_widget(
                         title="system-messages",
                         conditions=[Condition(["alinux2", "centos7", "rhel8"], base_os)],
                         filters=[self._new_filter(pattern=f"{head_private_ip}.*system-messages")],
                     ),
                     self._new_cw_log_widget(
                         title="syslog",
-                        conditions=[Condition(["ubuntu1804", "ubuntu2004"], base_os)],
+                        conditions=[Condition(["ubuntu2004", "ubuntu2204"], base_os)],
                         filters=[self._new_filter(pattern=f"{head_private_ip}.*syslog")],
                     ),
                     self._new_cw_log_widget(
                         title="cfn-init",
                         filters=[self._new_filter(pattern=f"{head_private_ip}.*cfn-init")],
                     ),
                     self._new_cw_log_widget(
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/templates/imagebuilder_stack.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/templates/imagebuilder_stack.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/templates/import_cdk.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/templates/import_cdk.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/templates/queues_stack.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/templates/queues_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,15 @@
 
 from aws_cdk import aws_ec2 as ec2
 from aws_cdk import aws_logs as logs
 from aws_cdk.core import CfnTag, Fn, NestedStack, Stack
 from constructs import Construct
 
 from pcluster.aws.aws_api import AWSApi
-from pcluster.config.cluster_config import (
-    SchedulerPluginQueue,
-    SharedStorageType,
-    SlurmClusterConfig,
-    SlurmComputeResource,
-    SlurmQueue,
-)
+from pcluster.config.cluster_config import SharedStorageType, SlurmClusterConfig, SlurmComputeResource, SlurmQueue
 from pcluster.constants import (
     DEFAULT_EPHEMERAL_DIR,
     NODE_BOOTSTRAP_TIMEOUT,
     OS_MAPPING,
     PCLUSTER_COMPUTE_RESOURCE_NAME_TAG,
     PCLUSTER_QUEUE_NAME_TAG,
 )
@@ -258,15 +252,15 @@
                                     self._shared_storage_attributes[SharedStorageType.FSX]["FileSystemTypes"]
                                 ),
                                 "FSXSharedDirs": to_comma_separated_string(
                                     self._shared_storage_mount_dirs[SharedStorageType.FSX]
                                 ),
                                 "Scheduler": self._config.scheduling.scheduler,
                                 "EphemeralDir": queue.compute_settings.local_storage.ephemeral_volume.mount_dir
-                                if isinstance(queue, (SlurmQueue, SchedulerPluginQueue))
+                                if isinstance(queue, SlurmQueue)
                                 and queue.compute_settings.local_storage.ephemeral_volume
                                 else DEFAULT_EPHEMERAL_DIR,
                                 "EbsSharedDirs": to_comma_separated_string(
                                     self._shared_storage_mount_dirs[SharedStorageType.EBS]
                                 ),
                                 "ClusterDNSDomain": str(self._cluster_hosted_zone.name)
                                 if self._cluster_hosted_zone
@@ -299,14 +293,21 @@
                                 "Timeout": str(
                                     get_attr(
                                         self._config,
                                         "dev_settings.timeouts.compute_node_bootstrap_timeout",
                                         NODE_BOOTSTRAP_TIMEOUT,
                                     )
                                 ),
+                                "ComputeStartupTimeMetricEnabled": str(
+                                    get_attr(
+                                        self._config,
+                                        "dev_settings.compute_startup_time_metric_enabled",
+                                        default=False,
+                                    )
+                                ),
                             },
                             **get_common_user_data_env(queue, self._config),
                         },
                     )
                 ),
                 monitoring=ec2.CfnLaunchTemplate.MonitoringProperty(enabled=is_detailed_monitoring_enabled),
                 tag_specifications=[
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/templates/slurm_builder.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/templates/slurm_builder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/utils.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,14 +425,20 @@
 
 
 def remove_none_values(original_dictionary):
     """Return a dictionary without entries with None value."""
     return {key: value for key, value in original_dictionary.items() if value is not None}
 
 
+def get_chunks(input_lst, desired_size=20):
+    """Get a list of lists splitting the input list in chunks with a specific length."""
+    for i in range(0, len(input_lst), desired_size):
+        yield input_lst[i : i + desired_size]  # noqa: E203
+
+
 def batch_by_property_callback(items, property_callback: Callable[..., int], batch_size):
     """
     Group a list of items into batches based on a property of each item and the specified `batch_size`.
 
     The property of each item is obtained using the property_callback function. This way the caller of
     `batch_by_property_size` defines which property to use for each item.
     Example: (With batch_size of 2 and property_callback=lambda item: len(item.property))
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/awsbatch_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/awsbatch_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,12 +184,12 @@
         return re.search(r"^([a-z0-9\-]+)\.", candidate) is not None
 
 
 class AwsBatchFsxValidator(Validator):
     """
     Validator for FSx and AWS Batch scheduler.
 
-    Fail if using AWS Batch and FSx for Lustre, not supported yet.
+    Fail if using AWS Batch and FSx for Lustre, ONTAP, OpenZFS, File Cache are not supported yet.
     """
 
     def _validate(self):
-        self._add_failure("FSx for Lustre is not supported when using AWS Batch as scheduler.", FailureLevel.ERROR)
+        self._add_failure("FSx is not supported when using AWS Batch as scheduler.", FailureLevel.ERROR)
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/cluster_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/cluster_validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -563,58 +563,64 @@
             network_interfaces_data = {}
             for network_interface in response:
                 network_interfaces_data[network_interface["NetworkInterfaceId"]] = network_interface
             return network_interfaces_data
         else:
             return {}
 
-    def _validate(self, file_system_ids, subnet_ids, security_groups_by_nodes):
+    def _validate(self, file_storage_ids, subnet_ids, security_groups_by_nodes):
         try:
-            file_systems = AWSApi.instance().fsx.get_file_systems_info(file_system_ids)
-            self._check_file_systems(security_groups_by_nodes, file_systems, subnet_ids)
+            file_cache_ids = [file_cache_id for file_cache_id in file_storage_ids if file_cache_id.startswith("fc-")]
+            if file_cache_ids:
+                file_storage_ids = [id for id in file_storage_ids if id not in file_cache_ids]
+                file_caches = AWSApi.instance().fsx.describe_file_caches(file_cache_ids)
+                self._check_file_storage(security_groups_by_nodes, file_caches, subnet_ids)
+
+            file_systems = AWSApi.instance().fsx.get_file_systems_info(file_storage_ids)
+            self._check_file_storage(security_groups_by_nodes, file_systems, subnet_ids)
         except AWSClientError as e:
             self._add_failure(str(e), FailureLevel.ERROR)
 
-    def _check_file_systems(self, security_groups_by_nodes, file_systems, subnet_ids):
+    def _check_file_storage(self, security_groups_by_nodes, file_storages, subnet_ids):
         vpc_id = AWSApi.instance().ec2.get_subnet_vpc(subnet_ids[0])
-        network_interfaces_data = self._describe_network_interfaces(file_systems)
-        for file_system in file_systems:
+        network_interfaces_data = self._describe_network_interfaces(file_storages)
+        for file_storage in file_storages:
             # Check to see if fs is in the same VPC as the stack
-            file_system_id = file_system.file_system_id
-            if file_system.vpc_id != vpc_id:
+            file_storage_id = file_storage.file_system_id if file_storage.file_system_id else file_storage.file_cache_id
+            if file_storage.vpc_id != vpc_id:
                 self._add_failure(
-                    "Currently only support using FSx file system that is in the same VPC as the cluster. "
-                    f"The file system {file_system_id} is in {file_system.vpc_id}.",
+                    "Currently only support using FSx file storage that is in the same VPC as the cluster. "
+                    f"The file system {file_storage_id} is in {file_storage.vpc_id}.",
                     FailureLevel.ERROR,
                 )
 
             # If there is an existing mt in the az, check the inbound and outbound rules of the security groups
-            network_interface_ids = file_system.network_interface_ids
+            network_interface_ids = file_storage.network_interface_ids
             if not network_interface_ids:
                 self._add_failure(
-                    f"Unable to validate FSx security groups. The given FSx file system '{file_system_id}'"
+                    f"Unable to validate FSx security groups. The given FSx file storage '{file_storage_id}'"
                     " doesn't have Elastic Network Interfaces attached to it.",
                     FailureLevel.ERROR,
                 )
             else:
                 network_interface_responses = []
                 for network_interface_id in network_interface_ids:
                     network_interface_responses.append(network_interfaces_data[network_interface_id])
 
                 network_interfaces = [ni for ni in network_interface_responses if ni.get("VpcId") == vpc_id]
 
-                for protocol, ports in FSX_PORTS[file_system.file_system_type].items():
+                for protocol, ports in FSX_PORTS[file_storage.file_storage_type].items():
                     missing_ports = self._get_missing_ports(
                         security_groups_by_nodes, subnet_ids, network_interfaces, ports, protocol
                     )
 
                     if missing_ports:
                         self._add_failure(
-                            f"The current security group settings on file system '{file_system_id}' does not"
-                            " satisfy mounting requirement. The file system must be associated to a security group"
+                            f"The current security group settings on file storage '{file_storage_id}' does not"
+                            " satisfy mounting requirement. The file storage must be associated to a security group"
                             f" that allows inbound and outbound {protocol.upper()} traffic through ports {ports}. "
                             f"Missing ports: {missing_ports}",
                             FailureLevel.ERROR,
                         )
 
     def _get_missing_ports(self, security_groups_by_nodes, subnet_ids, network_interfaces, ports, protocol):
         missing_ports = []
@@ -1462,7 +1468,19 @@
             if queue_subnets_with_public_ips:
                 self._add_failure(
                     f"The queue {queue.name} contains an instance type with multiple network interfaces however the "
                     f"subnets {queue_subnets_with_public_ips} is configured to automatically assign public IPs. AWS "
                     f"public IPs can only be assigned to instances launched with a single network interface.",
                     FailureLevel.ERROR,
                 )
+
+
+class LoginNodesSchedulerValidator(Validator):
+    """Verify that when using LoginNodes, the scheduler must be slurm."""
+
+    def _validate(self, scheduler):
+        if scheduler != "slurm":
+            self._add_failure(
+                "When using LoginNodes, the configured scheduler must be set to Slurm. "
+                "Please set the scheduler to Slurm.",
+                FailureLevel.ERROR,
+            )
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/common.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/database_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/database_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/directory_service_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/directory_service_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/ebs_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/ebs_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/ec2_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/ec2_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/efs_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/efs_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/feature_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/feature_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/fsx_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/fsx_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/iam_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/iam_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/imagebuilder_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/imagebuilder_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/instances_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/instances_validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # OR CONDITIONS OF ANY KIND, express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 from enum import Enum
 from typing import Callable, Dict
 
 from pcluster.aws.aws_resources import InstanceTypeInfo
 from pcluster.config import cluster_config
+from pcluster.constants import MIN_MEMORY_ABSOLUTE_DIFFERENCE, MIN_MEMORY_PRECENTAGE_DIFFERENCE
 from pcluster.validators.common import FailureLevel, Validator
 
 
 class _FlexibleInstanceTypesValidatorMixin:
     def validate_property_homogeneity(
         self,
         instance_types_info: Dict[str, InstanceTypeInfo],
@@ -229,25 +230,47 @@
                 f"Compute Resource {compute_resource_name} is using an OnDemand CapacityType but the Allocation "
                 f"Strategy specified is {allocation_strategy.value}. OnDemand CapacityType can only use '"
                 f"{cluster_config.AllocationStrategy.LOWEST_PRICE.value}' allocation strategy.",
                 FailureLevel.ERROR,
             )
 
 
-class InstancesMemorySchedulingValidator(Validator, _FlexibleInstanceTypesValidatorMixin):
-    """Validate support for Memory-based Scheduling when using Flexible Instance Types."""
+class InstancesMemorySchedulingWarningValidator(Validator):
+    """
+    Memory-based Scheduling Warning Validator.
+
+    This validator checks if Memory-based Scheduling is enabled when also using Flexible Instance Types.
+    In this case warns the customer about possible unused resources due to the differences in the instance types.
+    """
 
     def _validate(
         self,
         compute_resource_name: str,
         instance_types_info: Dict[str, InstanceTypeInfo],
         memory_scheduling_enabled: bool,
         **kwargs,
     ):
-        """Memory-based scheduling is NOT supported for Compute Resources with multiple instance types."""
-        if memory_scheduling_enabled and len(instance_types_info.items()) > 1:
+        if (
+            memory_scheduling_enabled
+            and len(instance_types_info.items()) > 1
+            and self.memory_difference_exceeds_thresholds(instance_types_info)
+        ):
             self._add_failure(
-                "Memory-based scheduling is only supported for Compute Resources using either 'InstanceType' or "
-                f"'Instances' with one instance type. Compute Resource {compute_resource_name} has more than "
-                "one instance type specified.",
-                FailureLevel.ERROR,
+                f'Enabling Memory-based scheduling when a Compute Resource ("{compute_resource_name}") has more than'
+                " one instance type specified may lead to unused resources since only the minimum available memory"
+                " across all instance-types can be specified in the Slurm node definition.",
+                FailureLevel.WARNING,
             )
+
+    def memory_difference_exceeds_thresholds(self, instance_types_info: Dict[str, InstanceTypeInfo]):
+        """Return True only if both thresholds are exceeded."""
+        min_memory, max_memory = self._min_max_memory(instance_types_info)
+        absolute_diff = max_memory - min_memory
+        percent_diff = absolute_diff / min_memory
+
+        return absolute_diff > MIN_MEMORY_ABSOLUTE_DIFFERENCE and percent_diff > MIN_MEMORY_PRECENTAGE_DIFFERENCE
+
+    def _min_max_memory(self, instance_types_info: Dict[str, InstanceTypeInfo]):
+        available_memory = [item.ec2memory_size_in_mib() for _, item in instance_types_info.items()]
+        # EC2 API should return valid values, but since it's really cheap better add a check
+        available_memory = [value for value in available_memory if value is not None]
+        return min(available_memory), max(available_memory)
```

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/kms_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/kms_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/monitoring_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/monitoring_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/networking_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/networking_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/s3_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/s3_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/tags_validators.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/tags_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster/validators/utils.py` & `aws-parallelcluster-3.7.0b1/src/pcluster/validators/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster3_config_converter/__init__.py` & `aws-parallelcluster-3.7.0b1/src/pcluster3_config_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.6.1/src/pcluster3_config_converter/pcluster3_config_converter.py` & `aws-parallelcluster-3.7.0b1/src/pcluster3_config_converter/pcluster3_config_converter.py`

 * *Files identical despite different names*

