# Comparing `tmp/skypilot-nightly-1.0.0.dev20230725.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20230726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20230725.tar", last modified: Tue Jul 25 10:40:42 2023, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20230726.tar", last modified: Wed Jul 26 10:40:41 2023, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20230725.tar` & `skypilot-nightly-1.0.0.dev20230726.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.647769 skypilot-nightly-1.0.0.dev20230725/
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-25 10:40:42.647769 skypilot-nightly-1.0.0.dev20230725/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 10:40:42.647769 skypilot-nightly-1.0.0.dev20230725/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-25 10:40:35.000000 skypilot-nightly-1.0.0.dev20230725/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.627769 skypilot-nightly-1.0.0.dev20230725/sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-25 10:40:35.000000 skypilot-nightly-1.0.0.dev20230725/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.627769 skypilot-nightly-1.0.0.dev20230725/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631769 skypilot-nightly-1.0.0.dev20230725/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)   113020 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   202078 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631769 skypilot-nightly-1.0.0.dev20230725/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/backends/onprem_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631769 skypilot-nightly-1.0.0.dev20230725/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (123)   168564 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631769 skypilot-nightly-1.0.0.dev20230725/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41169 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    46375 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.631769 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.635769 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.635769 skypilot-nightly-1.0.0.dev20230725/sky/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    89763 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.635769 skypilot-nightly-1.0.0.dev20230725/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.635769 skypilot-nightly-1.0.0.dev20230725/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/provision/aws/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.635769 skypilot-nightly-1.0.0.dev20230725/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42860 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.635769 skypilot-nightly-1.0.0.dev20230725/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-25 10:40:35.000000 skypilot-nightly-1.0.0.dev20230725/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.635769 skypilot-nightly-1.0.0.dev20230725/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/log_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.623769 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.635769 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.639769 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/aws/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.639769 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.639769 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.639769 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.639769 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.639769 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/oci/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.639769 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/scp/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/scp/scp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.643769 skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/job_head.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.643769 skypilot-nightly-1.0.0.dev20230725/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.643769 skypilot-nightly-1.0.0.dev20230725/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.643769 skypilot-nightly-1.0.0.dev20230725/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.643769 skypilot-nightly-1.0.0.dev20230725/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.643769 skypilot-nightly-1.0.0.dev20230725/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/templates/gcp-tpu-create.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.643769 skypilot-nightly-1.0.0.dev20230725/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.647769 skypilot-nightly-1.0.0.dev20230725/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.647769 skypilot-nightly-1.0.0.dev20230725/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/env_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/tpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.647769 skypilot-nightly-1.0.0.dev20230725/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-25 10:40:42.000000 skypilot-nightly-1.0.0.dev20230725/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-25 10:40:42.000000 skypilot-nightly-1.0.0.dev20230725/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:40:42.000000 skypilot-nightly-1.0.0.dev20230725/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-25 10:40:42.000000 skypilot-nightly-1.0.0.dev20230725/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-25 10:40:42.000000 skypilot-nightly-1.0.0.dev20230725/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-25 10:40:42.000000 skypilot-nightly-1.0.0.dev20230725/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:40:42.647769 skypilot-nightly-1.0.0.dev20230725/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_onprem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_pycryptodome_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   126800 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 10:40:33.000000 skypilot-nightly-1.0.0.dev20230725/tests/test_wheels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.093694 skypilot-nightly-1.0.0.dev20230726/
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-26 10:40:41.093694 skypilot-nightly-1.0.0.dev20230726/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 10:40:41.093694 skypilot-nightly-1.0.0.dev20230726/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-26 10:40:33.000000 skypilot-nightly-1.0.0.dev20230726/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.065693 skypilot-nightly-1.0.0.dev20230726/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-26 10:40:33.000000 skypilot-nightly-1.0.0.dev20230726/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.065693 skypilot-nightly-1.0.0.dev20230726/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.065693 skypilot-nightly-1.0.0.dev20230726/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113020 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202355 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.065693 skypilot-nightly-1.0.0.dev20230726/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/backends/onprem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.065693 skypilot-nightly-1.0.0.dev20230726/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168564 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.069694 skypilot-nightly-1.0.0.dev20230726/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41169 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46375 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.073694 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.073694 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.077694 skypilot-nightly-1.0.0.dev20230726/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89763 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.077694 skypilot-nightly-1.0.0.dev20230726/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.077694 skypilot-nightly-1.0.0.dev20230726/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/provision/aws/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.077694 skypilot-nightly-1.0.0.dev20230726/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42860 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.077694 skypilot-nightly-1.0.0.dev20230726/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-26 10:40:33.000000 skypilot-nightly-1.0.0.dev20230726/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.077694 skypilot-nightly-1.0.0.dev20230726/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/log_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.061694 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.077694 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.077694 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.077694 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.081694 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.081694 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.081694 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.081694 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/oci/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.081694 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/scp/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/scp/scp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.081694 skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/job_head.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.085693 skypilot-nightly-1.0.0.dev20230726/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/spot/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.085693 skypilot-nightly-1.0.0.dev20230726/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.085693 skypilot-nightly-1.0.0.dev20230726/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.085693 skypilot-nightly-1.0.0.dev20230726/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.085693 skypilot-nightly-1.0.0.dev20230726/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.085693 skypilot-nightly-1.0.0.dev20230726/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.085693 skypilot-nightly-1.0.0.dev20230726/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.089694 skypilot-nightly-1.0.0.dev20230726/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/env_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/tpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.089694 skypilot-nightly-1.0.0.dev20230726/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-26 10:40:41.000000 skypilot-nightly-1.0.0.dev20230726/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-26 10:40:41.000000 skypilot-nightly-1.0.0.dev20230726/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 10:40:41.000000 skypilot-nightly-1.0.0.dev20230726/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 10:40:41.000000 skypilot-nightly-1.0.0.dev20230726/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-26 10:40:41.000000 skypilot-nightly-1.0.0.dev20230726/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 10:40:41.000000 skypilot-nightly-1.0.0.dev20230726/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:40:41.093694 skypilot-nightly-1.0.0.dev20230726/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_onprem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_pycryptodome_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126800 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-26 10:40:31.000000 skypilot-nightly-1.0.0.dev20230726/tests/test_wheels.py
```

### Comparing `skypilot-nightly-1.0.0.dev20230725/LICENSE` & `skypilot-nightly-1.0.0.dev20230726/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230726/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230726/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230725
+Version: 1.0.0.dev20230726
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230725
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230726
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230725/README.md` & `skypilot-nightly-1.0.0.dev20230726/README.md`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/pyproject.toml` & `skypilot-nightly-1.0.0.dev20230726/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/setup.py` & `skypilot-nightly-1.0.0.dev20230726/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20230726/sky/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
-__commit__ = '24a5622509639db09398c9624360a3119e38effb'
-__version__ = '1.0.0-dev20230725'
+__commit__ = '608d0c34ced75b881e5b35b36e416f56d2f685fc'
+__version__ = '1.0.0-dev20230726'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
```

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20230726/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20230726/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20230726/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/adaptors/docker.py` & `skypilot-nightly-1.0.0.dev20230726/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20230726/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20230726/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20230726/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20230726/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20230726/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20230726/sky/backends/cloud_vm_ray_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1783,14 +1783,20 @@
                 if result is not None:
                     # Retry. Unlikely will succeed if it's due to no capacity.
                     logger.info(
                         'Retrying due to the possibly flaky RESOURCE_NOT_FOUND '
                         'error.')
                     return True
 
+            if isinstance(to_provision_cloud, clouds.Lambda):
+                if 'Your API requests are being rate limited.' in stderr:
+                    logger.info(
+                        'Retrying due to Lambda API rate limit exceeded.')
+                    return True
+
             if 'rsync: command not found' in stderr:
                 logger.info('Skipping retry due to `rsync` not found in '
                             'the specified image.')
                 return False
 
             if ('Processing file mounts' in stdout and
                     'Running setup commands' not in stdout and
```

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20230726/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20230726/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/backends/onprem_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/backends/onprem_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20230726/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/check.py` & `skypilot-nightly-1.0.0.dev20230726/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/cli.py` & `skypilot-nightly-1.0.0.dev20230726/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20230726/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/local.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/local.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20230726/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/core.py` & `skypilot-nightly-1.0.0.dev20230726/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/dag.py` & `skypilot-nightly-1.0.0.dev20230726/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20230726/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20230726/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20230726/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/execution.py` & `skypilot-nightly-1.0.0.dev20230726/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20230726/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20230726/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20230726/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20230726/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/provision/gcp/instance.py` & `skypilot-nightly-1.0.0.dev20230726/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/provision/gcp/instance_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/resources.py` & `skypilot-nightly-1.0.0.dev20230726/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230726/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20230726/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20230726/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/aws/config.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/aws/node_provider.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/aws/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/aws/utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/gcp/config.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/gcp/node.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/gcp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 """Lambda Cloud helper functions."""
 import json
 import os
 import requests
+import time
 from typing import Any, Dict, List, Optional, Tuple
 
+from sky.utils import common_utils
+
 CREDENTIALS_PATH = '~/.lambda_cloud/lambda_keys'
 API_ENDPOINT = 'https://cloud.lambdalabs.com/api/v1'
+INITIAL_BACKOFF_SECONDS = 10
+MAX_BACKOFF_FACTOR = 10
+MAX_ATTEMPTS = 6
 
 
 class LambdaCloudError(Exception):
     pass
 
 
 class Metadata:
@@ -81,14 +87,36 @@
         code = resp_json.get('error', {}).get('code')
         message = resp_json.get('error', {}).get('message')
     except (KeyError, json.decoder.JSONDecodeError):
         raise LambdaCloudError(f'Unexpected error. Status code: {status_code}')
     raise LambdaCloudError(f'{code}: {message}')
 
 
+def _try_request_with_backoff(method: str,
+                              url: str,
+                              headers: Dict[str, str],
+                              data: Optional[str] = None):
+    backoff = common_utils.Backoff(initial_backoff=INITIAL_BACKOFF_SECONDS,
+                                   max_backoff_factor=MAX_BACKOFF_FACTOR)
+    for i in range(MAX_ATTEMPTS):
+        if method == 'get':
+            response = requests.get(url, headers=headers)
+        elif method == 'post':
+            response = requests.post(url, headers=headers, data=data)
+        else:
+            raise ValueError(f'Unsupported requests method: {method}')
+        # If rate limited, wait and try again
+        if response.status_code == 429 and i != MAX_ATTEMPTS - 1:
+            time.sleep(backoff.current_backoff())
+            continue
+        if response.status_code == 200:
+            return response
+        raise_lambda_error(response)
+
+
 class LambdaCloudClient:
     """Wrapper functions for Lambda Cloud API."""
 
     def __init__(self) -> None:
         self.credentials = os.path.expanduser(CREDENTIALS_PATH)
         assert os.path.exists(self.credentials), 'Credentials not found'
         with open(self.credentials, 'r') as f:
@@ -129,46 +157,47 @@
         data = json.dumps({
             'region_name': region,
             'instance_type_name': instance_type,
             'ssh_key_names': [ssh_key_name],
             'quantity': quantity,
             'name': name
         })
-        response = requests.post(f'{API_ENDPOINT}/instance-operations/launch',
-                                 data=data,
-                                 headers=self.headers)
-        raise_lambda_error(response)
+        response = _try_request_with_backoff(
+            'post',
+            f'{API_ENDPOINT}/instance-operations/launch',
+            data=data,
+            headers=self.headers)
         return response.json().get('data', []).get('instance_ids', [])
 
     def remove_instances(self, *instance_ids: str) -> Dict[str, Any]:
         """Terminate instances."""
         data = json.dumps({
             'instance_ids': [
                 instance_ids[0]  # TODO(ewzeng) don't hardcode
             ]
         })
-        response = requests.post(
+        response = _try_request_with_backoff(
+            'post',
             f'{API_ENDPOINT}/instance-operations/terminate',
             data=data,
             headers=self.headers)
-        raise_lambda_error(response)
         return response.json().get('data', []).get('terminated_instances', [])
 
     def list_instances(self) -> List[Dict[str, Any]]:
         """List existing instances."""
-        response = requests.get(f'{API_ENDPOINT}/instances',
-                                headers=self.headers)
-        raise_lambda_error(response)
+        response = _try_request_with_backoff('get',
+                                             f'{API_ENDPOINT}/instances',
+                                             headers=self.headers)
         return response.json().get('data', [])
 
     def list_ssh_keys(self) -> List[Dict[str, str]]:
         """List ssh keys."""
-        response = requests.get(f'{API_ENDPOINT}/ssh-keys',
-                                headers=self.headers)
-        raise_lambda_error(response)
+        response = _try_request_with_backoff('get',
+                                             f'{API_ENDPOINT}/ssh-keys',
+                                             headers=self.headers)
         return response.json().get('data', [])
 
     def get_unique_ssh_key_name(self, prefix: str,
                                 pub_key: str) -> Tuple[str, bool]:
         """Returns a ssh key name with the given prefix.
 
         If no names have given prefix, return prefix. If pub_key exists and
@@ -196,18 +225,18 @@
                     name[len(prefix) + 1:].isdigit()):
                 suffix_digits.append(int(name[len(prefix) + 1:]))
         return f'{prefix}-{max(suffix_digits) + 1}', False
 
     def register_ssh_key(self, name: str, pub_key: str) -> None:
         """Register ssh key with Lambda."""
         data = json.dumps({'name': name, 'public_key': pub_key})
-        response = requests.post(f'{API_ENDPOINT}/ssh-keys',
-                                 data=data,
-                                 headers=self.headers)
-        raise_lambda_error(response)
+        _try_request_with_backoff('post',
+                                  f'{API_ENDPOINT}/ssh-keys',
+                                  data=data,
+                                  headers=self.headers)
 
     def list_catalog(self) -> Dict[str, Any]:
         """List offered instances and their availability."""
-        response = requests.get(f'{API_ENDPOINT}/instance-types',
-                                headers=self.headers)
-        raise_lambda_error(response)
+        response = _try_request_with_backoff('get',
+                                             f'{API_ENDPOINT}/instance-types',
+                                             headers=self.headers)
         return response.json().get('data', [])
```

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/oci/config.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/oci/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/providers/scp/scp_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/providers/scp/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20230726/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20230726/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20230726/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20230726/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20230726/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20230726/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20230726/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20230726/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20230726/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20230726/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/task.py` & `skypilot-nightly-1.0.0.dev20230726/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230726/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230726/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230726/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230726/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230726/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230726/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230726/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230726/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20230726/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20230726/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20230726/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/cli_utils/status_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         StatusColumn('RESOURCES',
                      _get_resources,
                      trunc_length=70 if not show_all else 0),
         StatusColumn('REGION', _get_region, show_by_default=False),
         StatusColumn('ZONE', _get_zone, show_by_default=False),
         StatusColumn('STATUS', _get_status_colored),
         StatusColumn('AUTOSTOP', _get_autostop),
+        StatusColumn('HEAD_IP', _get_head_ip, show_by_default=False),
         StatusColumn('COMMAND',
                      _get_command,
                      trunc_length=COMMAND_TRUNC_LENGTH if not show_all else 0),
     ]
 
     columns = []
     for status_column in status_columns:
@@ -359,14 +360,23 @@
     if cluster_record['to_down']:
         autostop_str += f'{separation}(down)'
     if autostop_str == '':
         autostop_str = '-'
     return autostop_str
 
 
+def _get_head_ip(cluster_record: _ClusterRecord) -> str:
+    handle = cluster_record['handle']
+    if not isinstance(handle, backends.CloudVmRayResourceHandle):
+        return '-'
+    if handle.head_ip is None:
+        return '-'
+    return handle.head_ip
+
+
 def _is_pending_autostop(cluster_record: _ClusterRecord) -> bool:
     # autostop < 0 means nothing scheduled.
     return cluster_record['autostop'] >= 0 and _get_status(
         cluster_record) != status_lib.ClusterStatus.STOPPED
 
 
 # ---- 'sky cost-report' helper functions below ----
```

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/dag_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/tpu_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/tpu_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20230726/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230726/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230725
+Version: 1.0.0.dev20230726
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230725
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230726
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230725/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20230726/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20230726/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20230726/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20230726/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/tests/test_jobs.py` & `skypilot-nightly-1.0.0.dev20230726/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20230726/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/tests/test_onprem.py` & `skypilot-nightly-1.0.0.dev20230726/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20230726/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20230726/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20230726/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/tests/test_spot.py` & `skypilot-nightly-1.0.0.dev20230726/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20230726/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230725/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20230726/tests/test_wheels.py`

 * *Files identical despite different names*

