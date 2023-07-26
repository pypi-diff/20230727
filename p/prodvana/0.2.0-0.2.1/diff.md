# Comparing `tmp/prodvana-0.2.0.tar.gz` & `tmp/prodvana-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodvana-0.2.0.tar", max compression
+gzip compressed data, was "prodvana-0.2.1.tar", max compression
```

## Comparing `prodvana-0.2.0.tar` & `prodvana-0.2.1.tar`

### file list

```diff
@@ -1,329 +1,329 @@
--rw-r--r--   0        0        0       81 2023-07-07 23:25:26.643463 prodvana-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-07 23:25:26.643463 prodvana-0.2.0/prodvana/__init__.py
--rw-r--r--   0        0        0     3529 2023-07-07 23:25:26.643463 prodvana-0.2.0/prodvana/client.py
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.421700 prodvana-0.2.0/prodvana/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.421700 prodvana-0.2.0/prodvana/proto/prodvana/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.425700 prodvana-0.2.0/prodvana/proto/prodvana/agent/__init__.py
--rw-r--r--   0        0        0     9562 2023-07-19 21:15:42.121700 prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
--rw-r--r--   0        0        0    19141 2023-07-19 21:15:42.277700 prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
--rw-r--r--   0        0        0    22573 2023-07-19 21:15:42.121700 prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
--rw-r--r--   0        0        0     6760 2023-07-19 21:15:42.277700 prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.445700 prodvana-0.2.0/prodvana/proto/prodvana/application/__init__.py
--rw-r--r--   0        0        0     3521 2023-07-19 21:15:42.233700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_config_pb2.py
--rw-r--r--   0        0        0     3485 2023-07-19 21:15:42.401700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.241700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.397700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    15907 2023-07-19 21:15:42.237700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2.py
--rw-r--r--   0        0        0    16830 2023-07-19 21:15:42.393700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2.pyi
--rw-r--r--   0        0        0    22241 2023-07-19 21:15:42.241700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6755 2023-07-19 21:15:42.393700 prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2235 2023-07-19 21:15:42.241700 prodvana-0.2.0/prodvana/proto/prodvana/application/object_pb2.py
--rw-r--r--   0        0        0     2184 2023-07-19 21:15:42.397700 prodvana-0.2.0/prodvana/proto/prodvana/application/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.241700 prodvana-0.2.0/prodvana/proto/prodvana/application/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.393700 prodvana-0.2.0/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2011 2023-07-19 21:15:42.237700 prodvana-0.2.0/prodvana/proto/prodvana/application/user_metadata_pb2.py
--rw-r--r--   0        0        0     1670 2023-07-19 21:15:42.397700 prodvana-0.2.0/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.237700 prodvana-0.2.0/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.397700 prodvana-0.2.0/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.441700 prodvana-0.2.0/prodvana/proto/prodvana/auth/__init__.py
--rw-r--r--   0        0        0     8480 2023-07-19 21:15:42.213700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2.py
--rw-r--r--   0        0        0    10206 2023-07-19 21:15:42.373700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
--rw-r--r--   0        0        0    18631 2023-07-19 21:15:42.217700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6767 2023-07-19 21:15:42.373700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3181 2023-07-19 21:15:42.217700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_pb2.py
--rw-r--r--   0        0        0     5515 2023-07-19 21:15:42.377700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.213700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.373700 prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.433700 prodvana-0.2.0/prodvana/proto/prodvana/blobs/__init__.py
--rw-r--r--   0        0        0     2285 2023-07-19 21:15:42.149700 prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
--rw-r--r--   0        0        0     1129 2023-07-19 21:15:42.309700 prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
--rw-r--r--   0        0        0     2704 2023-07-19 21:15:42.149700 prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
--rw-r--r--   0        0        0      895 2023-07-19 21:15:42.305700 prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.425700 prodvana-0.2.0/prodvana/proto/prodvana/capability/__init__.py
--rw-r--r--   0        0        0     4830 2023-07-19 21:15:42.113700 prodvana-0.2.0/prodvana/proto/prodvana/capability/capability_pb2.py
--rw-r--r--   0        0        0     5455 2023-07-19 21:15:42.273700 prodvana-0.2.0/prodvana/proto/prodvana/capability/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.113700 prodvana-0.2.0/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.269700 prodvana-0.2.0/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.433700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/__init__.py
--rw-r--r--   0        0        0     1988 2023-07-19 21:15:42.177700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/constants_pb2.py
--rw-r--r--   0        0        0     1667 2023-07-19 21:15:42.321700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/constants_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.157700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/constants_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.317700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/constants_pb2_grpc.pyi
--rw-r--r--   0        0        0     1366 2023-07-19 21:15:42.157700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
--rw-r--r--   0        0        0      869 2023-07-19 21:15:42.317700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.153700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.325700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
--rw-r--r--   0        0        0     2864 2023-07-19 21:15:42.161700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/env_pb2.py
--rw-r--r--   0        0        0     2933 2023-07-19 21:15:42.325700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/env_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.173700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.337700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
--rw-r--r--   0        0        0     4272 2023-07-19 21:15:42.153700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/helm_pb2.py
--rw-r--r--   0        0        0     5454 2023-07-19 21:15:42.329700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/helm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.165700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.321700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
--rw-r--r--   0        0        0     3013 2023-07-19 21:15:42.177700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
--rw-r--r--   0        0        0     4537 2023-07-19 21:15:42.329700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.161700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.313700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     1738 2023-07-19 21:15:42.169700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/links_pb2.py
--rw-r--r--   0        0        0      846 2023-07-19 21:15:42.325700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/links_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.153700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.333700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
--rw-r--r--   0        0        0     1338 2023-07-19 21:15:42.169700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/maturity_pb2.py
--rw-r--r--   0        0        0     1103 2023-07-19 21:15:42.309700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.177700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.321700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
--rw-r--r--   0        0        0     1838 2023-07-19 21:15:42.173700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/meta_pb2.py
--rw-r--r--   0        0        0     2531 2023-07-19 21:15:42.317700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.169700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.321700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0     1866 2023-07-19 21:15:42.165700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/notification_pb2.py
--rw-r--r--   0        0        0     1337 2023-07-19 21:15:42.317700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.153700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.313700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
--rw-r--r--   0        0        0     7815 2023-07-19 21:15:42.161700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/parameters_pb2.py
--rw-r--r--   0        0        0    10735 2023-07-19 21:15:42.313700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.169700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.333700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0     9143 2023-07-19 21:15:42.173700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/program_pb2.py
--rw-r--r--   0        0        0    15928 2023-07-19 21:15:42.329700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/program_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.165700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.309700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
--rw-r--r--   0        0        0     2686 2023-07-19 21:15:42.165700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/retry_pb2.py
--rw-r--r--   0        0        0     2757 2023-07-19 21:15:42.333700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/retry_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.157700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.329700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
--rw-r--r--   0        0        0     2804 2023-07-19 21:15:42.157700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/task_pb2.py
--rw-r--r--   0        0        0     3946 2023-07-19 21:15:42.325700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.173700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.309700 prodvana-0.2.0/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.425700 prodvana-0.2.0/prodvana/proto/prodvana/config_file/__init__.py
--rw-r--r--   0        0        0     3685 2023-07-19 21:15:42.117700 prodvana-0.2.0/prodvana/proto/prodvana/config_file/config_pb2.py
--rw-r--r--   0        0        0     4656 2023-07-19 21:15:42.273700 prodvana-0.2.0/prodvana/proto/prodvana/config_file/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.117700 prodvana-0.2.0/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.273700 prodvana-0.2.0/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.437700 prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/__init__.py
--rw-r--r--   0        0        0     1388 2023-07-19 21:15:42.209700 prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
--rw-r--r--   0        0        0     1131 2023-07-19 21:15:42.369700 prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.209700 prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.369700 prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.421700 prodvana-0.2.0/prodvana/proto/prodvana/delivery/__init__.py
--rw-r--r--   0        0        0     2079 2023-07-19 21:15:42.109700 prodvana-0.2.0/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
--rw-r--r--   0        0        0     2294 2023-07-19 21:15:42.265700 prodvana-0.2.0/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.105700 prodvana-0.2.0/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.261700 prodvana-0.2.0/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.429700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/__init__.py
--rw-r--r--   0        0        0     6161 2023-07-19 21:15:42.125700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/config_pb2.py
--rw-r--r--   0        0        0     8052 2023-07-19 21:15:42.285700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.133700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.289700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
--rw-r--r--   0        0        0     9291 2023-07-19 21:15:42.129700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
--rw-r--r--   0        0        0     8986 2023-07-19 21:15:42.289700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
--rw-r--r--   0        0        0    13097 2023-07-19 21:15:42.129700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3909 2023-07-19 21:15:42.289700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2015 2023-07-19 21:15:42.129700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/object_pb2.py
--rw-r--r--   0        0        0     1862 2023-07-19 21:15:42.285700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.133700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.285700 prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.429700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/__init__.py
--rw-r--r--   0        0        0    22956 2023-07-20 18:34:42.993878 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2.py
--rw-r--r--   0        0        0    30187 2023-07-20 18:34:42.993878 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
--rw-r--r--   0        0        0    22004 2023-07-20 18:34:42.993878 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
--rw-r--r--   0        0        0     6317 2023-07-20 18:34:42.993878 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.429700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/__init__.py
--rw-r--r--   0        0        0    26696 2023-07-20 18:34:42.993878 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
--rw-r--r--   0        0        0    76423 2023-07-20 18:34:42.997877 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.137700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.293700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
--rw-r--r--   0        0        0     3517 2023-07-19 21:15:42.133700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
--rw-r--r--   0        0        0     7935 2023-07-19 21:15:42.293700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.137700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.293700 prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.445700 prodvana-0.2.0/prodvana/proto/prodvana/environment/__init__.py
--rw-r--r--   0        0        0    16774 2023-07-20 18:34:42.997877 prodvana-0.2.0/prodvana/proto/prodvana/environment/clusters_pb2.py
--rw-r--r--   0        0        0    37710 2023-07-20 18:34:42.997877 prodvana-0.2.0/prodvana/proto/prodvana/environment/clusters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.245700 prodvana-0.2.0/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.401700 prodvana-0.2.0/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
--rw-r--r--   0        0        0    12870 2023-07-19 21:15:42.245700 prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2.py
--rw-r--r--   0        0        0    18334 2023-07-19 21:15:42.401700 prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
--rw-r--r--   0        0        0    21499 2023-07-19 21:15:42.245700 prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6311 2023-07-19 21:15:42.401700 prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.445700 prodvana-0.2.0/prodvana/proto/prodvana/events/__init__.py
--rw-r--r--   0        0        0     4801 2023-07-19 21:15:42.253700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2.py
--rw-r--r--   0        0        0     5547 2023-07-19 21:15:42.417700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2.pyi
--rw-r--r--   0        0        0     2714 2023-07-19 21:15:42.257700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
--rw-r--r--   0        0        0      853 2023-07-19 21:15:42.417700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2688 2023-07-19 21:15:42.253700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_pb2.py
--rw-r--r--   0        0        0     4131 2023-07-19 21:15:42.409700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.257700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.413700 prodvana-0.2.0/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
--rw-r--r--   0        0        0    10353 2023-07-19 21:15:42.257700 prodvana-0.2.0/prodvana/proto/prodvana/events/types_pb2.py
--rw-r--r--   0        0        0    30800 2023-07-19 21:15:42.413700 prodvana-0.2.0/prodvana/proto/prodvana/events/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.257700 prodvana-0.2.0/prodvana/proto/prodvana/events/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.413700 prodvana-0.2.0/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.445700 prodvana-0.2.0/prodvana/proto/prodvana/insights/__init__.py
--rw-r--r--   0        0        0     2205 2023-07-19 21:15:42.233700 prodvana-0.2.0/prodvana/proto/prodvana/insights/insights_pb2.py
--rw-r--r--   0        0        0     3508 2023-07-19 21:15:42.389700 prodvana-0.2.0/prodvana/proto/prodvana/insights/insights_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.233700 prodvana-0.2.0/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.389700 prodvana-0.2.0/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.437700 prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/__init__.py
--rw-r--r--   0        0        0     8344 2023-07-19 21:15:42.201700 prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2.py
--rw-r--r--   0        0        0    13338 2023-07-19 21:15:42.357700 prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
--rw-r--r--   0        0        0    12065 2023-07-19 21:15:42.197700 prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3657 2023-07-19 21:15:42.357700 prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.429700 prodvana-0.2.0/prodvana/proto/prodvana/metrics/__init__.py
--rw-r--r--   0        0        0     3762 2023-07-19 21:15:42.125700 prodvana-0.2.0/prodvana/proto/prodvana/metrics/metrics_pb2.py
--rw-r--r--   0        0        0     8746 2023-07-19 21:15:42.281700 prodvana-0.2.0/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.125700 prodvana-0.2.0/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.281700 prodvana-0.2.0/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.433700 prodvana-0.2.0/prodvana/proto/prodvana/object/__init__.py
--rw-r--r--   0        0        0     1657 2023-07-19 21:15:42.145700 prodvana-0.2.0/prodvana/proto/prodvana/object/meta_pb2.py
--rw-r--r--   0        0        0     1957 2023-07-19 21:15:42.301700 prodvana-0.2.0/prodvana/proto/prodvana/object/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.145700 prodvana-0.2.0/prodvana/proto/prodvana/object/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.305700 prodvana-0.2.0/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.429700 prodvana-0.2.0/prodvana/proto/prodvana/organization/__init__.py
--rw-r--r--   0        0        0     9808 2023-07-19 21:15:42.145700 prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2.py
--rw-r--r--   0        0        0     9762 2023-07-19 21:15:42.301700 prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
--rw-r--r--   0        0        0    14668 2023-07-19 21:15:42.141700 prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4779 2023-07-19 21:15:42.301700 prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2568 2023-07-19 21:15:42.141700 prodvana-0.2.0/prodvana/proto/prodvana/organization/user_metadata_pb2.py
--rw-r--r--   0        0        0     1972 2023-07-19 21:15:42.297700 prodvana-0.2.0/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.141700 prodvana-0.2.0/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.301700 prodvana-0.2.0/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.437700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/__init__.py
--rw-r--r--   0        0        0     2038 2023-07-19 21:15:42.201700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/object_pb2.py
--rw-r--r--   0        0        0     2595 2023-07-19 21:15:42.361700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.201700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.361700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     6748 2023-07-19 21:15:42.205700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
--rw-r--r--   0        0        0    11698 2023-07-19 21:15:42.361700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.201700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.361700 prodvana-0.2.0/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.441700 prodvana-0.2.0/prodvana/proto/prodvana/protection/__init__.py
--rw-r--r--   0        0        0     2777 2023-07-19 21:15:42.225700 prodvana-0.2.0/prodvana/proto/prodvana/protection/attachments_pb2.py
--rw-r--r--   0        0        0     2860 2023-07-19 21:15:42.389700 prodvana-0.2.0/prodvana/proto/prodvana/protection/attachments_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.229700 prodvana-0.2.0/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.381700 prodvana-0.2.0/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
--rw-r--r--   0        0        0     1716 2023-07-19 21:15:42.225700 prodvana-0.2.0/prodvana/proto/prodvana/protection/object_pb2.py
--rw-r--r--   0        0        0     1545 2023-07-19 21:15:42.385700 prodvana-0.2.0/prodvana/proto/prodvana/protection/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.229700 prodvana-0.2.0/prodvana/proto/prodvana/protection/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.381700 prodvana-0.2.0/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     6615 2023-07-19 21:15:42.229700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_config_pb2.py
--rw-r--r--   0        0        0    10041 2023-07-19 21:15:42.389700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.225700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.385700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     8167 2023-07-19 21:15:42.225700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2.py
--rw-r--r--   0        0        0     8325 2023-07-19 21:15:42.381700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
--rw-r--r--   0        0        0    12468 2023-07-19 21:15:42.221700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
--rw-r--r--   0        0        0     3716 2023-07-19 21:15:42.381700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3938 2023-07-19 21:15:42.221700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_reference_pb2.py
--rw-r--r--   0        0        0     4997 2023-07-19 21:15:42.385700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.221700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.385700 prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.433700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/__init__.py
--rw-r--r--   0        0        0     2453 2023-07-19 21:15:42.193700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/object_pb2.py
--rw-r--r--   0        0        0     3325 2023-07-19 21:15:42.353700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.197700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.349700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     7193 2023-07-19 21:15:42.193700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
--rw-r--r--   0        0        0    12716 2023-07-19 21:15:42.353700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.189700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.349700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    10119 2023-07-19 21:15:42.189700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
--rw-r--r--   0        0        0    11055 2023-07-19 21:15:42.349700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
--rw-r--r--   0        0        0    15129 2023-07-19 21:15:42.193700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4757 2023-07-19 21:15:42.353700 prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.433700 prodvana-0.2.0/prodvana/proto/prodvana/repo/__init__.py
--rw-r--r--   0        0        0     1701 2023-07-19 21:15:42.149700 prodvana-0.2.0/prodvana/proto/prodvana/repo/repo_pb2.py
--rw-r--r--   0        0        0     2315 2023-07-19 21:15:42.305700 prodvana-0.2.0/prodvana/proto/prodvana/repo/repo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.145700 prodvana-0.2.0/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.305700 prodvana-0.2.0/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.437700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/__init__.py
--rw-r--r--   0        0        0     1434 2023-07-19 21:15:42.205700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/features_pb2.py
--rw-r--r--   0        0        0     1320 2023-07-19 21:15:42.369700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/features_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.209700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.365700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
--rw-r--r--   0        0        0     4579 2023-07-19 21:15:42.205700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
--rw-r--r--   0        0        0     6995 2023-07-19 21:15:42.365700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.205700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.365700 prodvana-0.2.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.429700 prodvana-0.2.0/prodvana/proto/prodvana/scm/__init__.py
--rw-r--r--   0        0        0     1229 2023-07-19 21:15:42.121700 prodvana-0.2.0/prodvana/proto/prodvana/scm/types_pb2.py
--rw-r--r--   0        0        0      914 2023-07-19 21:15:42.281700 prodvana-0.2.0/prodvana/proto/prodvana/scm/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.125700 prodvana-0.2.0/prodvana/proto/prodvana/scm/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.281700 prodvana-0.2.0/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.425700 prodvana-0.2.0/prodvana/proto/prodvana/secrets/__init__.py
--rw-r--r--   0        0        0     6361 2023-07-19 21:15:42.117700 prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
--rw-r--r--   0        0        0     4586 2023-07-19 21:15:42.273700 prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
--rw-r--r--   0        0        0     9936 2023-07-19 21:15:42.117700 prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
--rw-r--r--   0        0        0     2847 2023-07-19 21:15:42.277700 prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.433700 prodvana-0.2.0/prodvana/proto/prodvana/service/__init__.py
--rw-r--r--   0        0        0     4358 2023-07-20 18:34:42.997877 prodvana-0.2.0/prodvana/proto/prodvana/service/object_pb2.py
--rw-r--r--   0        0        0     7117 2023-07-20 18:34:42.997877 prodvana-0.2.0/prodvana/proto/prodvana/service/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.189700 prodvana-0.2.0/prodvana/proto/prodvana/service/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.337700 prodvana-0.2.0/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     1908 2023-07-19 21:15:42.181700 prodvana-0.2.0/prodvana/proto/prodvana/service/parameters_pb2.py
--rw-r--r--   0        0        0     2424 2023-07-19 21:15:42.337700 prodvana-0.2.0/prodvana/proto/prodvana/service/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.185700 prodvana-0.2.0/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.345700 prodvana-0.2.0/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    26309 2023-07-19 21:15:42.185700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_config_pb2.py
--rw-r--r--   0        0        0    54314 2023-07-19 21:15:42.341700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.189700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.345700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    31947 2023-07-19 21:15:42.185700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2.py
--rw-r--r--   0        0        0    38013 2023-07-19 21:15:42.341700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2.pyi
--rw-r--r--   0        0        0    33828 2023-07-19 21:15:42.185700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
--rw-r--r--   0        0        0     9674 2023-07-19 21:15:42.345700 prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2198 2023-07-19 21:15:42.181700 prodvana-0.2.0/prodvana/proto/prodvana/service/user_metadata_pb2.py
--rw-r--r--   0        0        0     2106 2023-07-19 21:15:42.337700 prodvana-0.2.0/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.181700 prodvana-0.2.0/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.341700 prodvana-0.2.0/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.441700 prodvana-0.2.0/prodvana/proto/prodvana/settings/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.441700 prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/__init__.py
--rw-r--r--   0        0        0     5019 2023-07-19 21:15:42.213700 prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2.py
--rw-r--r--   0        0        0     5677 2023-07-19 21:15:42.369700 prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
--rw-r--r--   0        0        0     8214 2023-07-19 21:15:42.213700 prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
--rw-r--r--   0        0        0     2318 2023-07-19 21:15:42.373700 prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.425700 prodvana-0.2.0/prodvana/proto/prodvana/stat/__init__.py
--rw-r--r--   0        0        0     1317 2023-07-19 21:15:42.109700 prodvana-0.2.0/prodvana/proto/prodvana/stat/efficiency_pb2.py
--rw-r--r--   0        0        0     1156 2023-07-19 21:15:42.265700 prodvana-0.2.0/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.109700 prodvana-0.2.0/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.265700 prodvana-0.2.0/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.441700 prodvana-0.2.0/prodvana/proto/prodvana/users/__init__.py
--rw-r--r--   0        0        0     1361 2023-07-19 21:15:42.221700 prodvana-0.2.0/prodvana/proto/prodvana/users/users_pb2.py
--rw-r--r--   0        0        0     1451 2023-07-19 21:15:42.377700 prodvana-0.2.0/prodvana/proto/prodvana/users/users_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.217700 prodvana-0.2.0/prodvana/proto/prodvana/users/users_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.377700 prodvana-0.2.0/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.425700 prodvana-0.2.0/prodvana/proto/prodvana/version/__init__.py
--rw-r--r--   0        0        0     1723 2023-07-19 21:15:42.113700 prodvana-0.2.0/prodvana/proto/prodvana/version/source_metadata_pb2.py
--rw-r--r--   0        0        0     2817 2023-07-19 21:15:42.269700 prodvana-0.2.0/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.109700 prodvana-0.2.0/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.269700 prodvana-0.2.0/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.437700 prodvana-0.2.0/prodvana/proto/prodvana/volumes/__init__.py
--rw-r--r--   0        0        0     3089 2023-07-19 21:15:42.197700 prodvana-0.2.0/prodvana/proto/prodvana/volumes/volumes_pb2.py
--rw-r--r--   0        0        0     4793 2023-07-19 21:15:42.357700 prodvana-0.2.0/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.197700 prodvana-0.2.0/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.357700 prodvana-0.2.0/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.445700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/__init__.py
--rw-r--r--   0        0        0     3274 2023-07-19 21:15:42.249700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/integration_config_pb2.py
--rw-r--r--   0        0        0     4328 2023-07-19 21:15:42.405700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.249700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.409700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    36604 2023-07-19 21:15:42.249700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
--rw-r--r--   0        0        0    52034 2023-07-19 21:15:42.409700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
--rw-r--r--   0        0        0    57702 2023-07-19 21:15:42.253700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
--rw-r--r--   0        0        0    16676 2023-07-19 21:15:42.405700 prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-19 21:15:42.449700 prodvana-0.2.0/prodvana/proto/validate/__init__.py
--rw-r--r--   0        0        0    13684 2023-07-19 21:15:42.261700 prodvana-0.2.0/prodvana/proto/validate/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-07-19 21:15:42.417700 prodvana-0.2.0/prodvana/proto/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-19 21:15:42.261700 prodvana-0.2.0/prodvana/proto/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-19 21:15:42.421700 prodvana-0.2.0/prodvana/proto/validate/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-07 23:25:26.663462 prodvana-0.2.0/prodvana/py.typed
--rw-r--r--   0        0        0        0 2023-07-07 23:25:26.663462 prodvana-0.2.0/prodvana/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-07-07 23:25:26.663462 prodvana-0.2.0/prodvana/utils/desired_states.py
--rw-r--r--   0        0        0     1434 2023-07-20 20:38:16.234138 prodvana-0.2.0/prodvana/utils/parameters.py
--rw-r--r--   0        0        0     1731 2023-07-20 20:38:16.234138 prodvana-0.2.0/prodvana/utils/protections.py
--rw-r--r--   0        0        0     4079 2023-07-07 23:25:26.663462 prodvana-0.2.0/prodvana/utils/service_config.py
--rw-r--r--   0        0        0     7140 2023-07-07 23:25:26.663462 prodvana-0.2.0/prodvana/utils/tests/test_service_config.py
--rw-r--r--   0        0        0      746 2023-07-22 13:46:43.126029 prodvana-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       81 2023-07-07 23:25:26.643463 prodvana-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-07 23:25:26.643463 prodvana-0.2.1/prodvana/__init__.py
+-rw-r--r--   0        0        0     3529 2023-07-07 23:25:26.643463 prodvana-0.2.1/prodvana/client.py
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.788471 prodvana-0.2.1/prodvana/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.788471 prodvana-0.2.1/prodvana/proto/prodvana/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/agent/__init__.py
+-rw-r--r--   0        0        0     9562 2023-07-26 18:43:18.520471 prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
+-rw-r--r--   0        0        0    19141 2023-07-26 18:43:18.664471 prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
+-rw-r--r--   0        0        0    22573 2023-07-26 18:43:18.520471 prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
+-rw-r--r--   0        0        0     6760 2023-07-26 18:43:18.660471 prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.808471 prodvana-0.2.1/prodvana/proto/prodvana/application/__init__.py
+-rw-r--r--   0        0        0     3521 2023-07-26 18:43:18.624471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_config_pb2.py
+-rw-r--r--   0        0        0     3485 2023-07-26 18:43:18.768471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.628471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.768471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15907 2023-07-26 18:43:18.624471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2.py
+-rw-r--r--   0        0        0    16830 2023-07-26 18:43:18.764471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2.pyi
+-rw-r--r--   0        0        0    22241 2023-07-26 18:43:18.632471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6755 2023-07-26 18:43:18.764471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2235 2023-07-26 18:43:18.628471 prodvana-0.2.1/prodvana/proto/prodvana/application/object_pb2.py
+-rw-r--r--   0        0        0     2184 2023-07-26 18:43:18.768471 prodvana-0.2.1/prodvana/proto/prodvana/application/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.628471 prodvana-0.2.1/prodvana/proto/prodvana/application/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.764471 prodvana-0.2.1/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2011 2023-07-26 18:43:18.628471 prodvana-0.2.1/prodvana/proto/prodvana/application/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1670 2023-07-26 18:43:18.768471 prodvana-0.2.1/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.628471 prodvana-0.2.1/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.768471 prodvana-0.2.1/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/auth/__init__.py
+-rw-r--r--   0        0        0     8480 2023-07-26 18:43:18.608471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2.py
+-rw-r--r--   0        0        0    10206 2023-07-26 18:43:18.748471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
+-rw-r--r--   0        0        0    18631 2023-07-26 18:43:18.608471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6767 2023-07-26 18:43:18.748471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3181 2023-07-26 18:43:18.608471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_pb2.py
+-rw-r--r--   0        0        0     5515 2023-07-26 18:43:18.748471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.608471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.744471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/blobs/__init__.py
+-rw-r--r--   0        0        0     2285 2023-07-26 18:43:18.548471 prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
+-rw-r--r--   0        0        0     1129 2023-07-26 18:43:18.688471 prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
+-rw-r--r--   0        0        0     2704 2023-07-26 18:43:18.548471 prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      895 2023-07-26 18:43:18.688471 prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.792471 prodvana-0.2.1/prodvana/proto/prodvana/capability/__init__.py
+-rw-r--r--   0        0        0     4830 2023-07-26 18:43:18.516471 prodvana-0.2.1/prodvana/proto/prodvana/capability/capability_pb2.py
+-rw-r--r--   0        0        0     5455 2023-07-26 18:43:18.656471 prodvana-0.2.1/prodvana/proto/prodvana/capability/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.516471 prodvana-0.2.1/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.656471 prodvana-0.2.1/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/__init__.py
+-rw-r--r--   0        0        0     1988 2023-07-26 18:43:18.572471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/constants_pb2.py
+-rw-r--r--   0        0        0     1667 2023-07-26 18:43:18.700471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/constants_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.556471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/constants_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.696471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/constants_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1366 2023-07-26 18:43:18.552471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
+-rw-r--r--   0        0        0      869 2023-07-26 18:43:18.696471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.552471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.704471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2864 2023-07-26 18:43:18.556471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/env_pb2.py
+-rw-r--r--   0        0        0     2933 2023-07-26 18:43:18.704471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/env_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.568471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.712471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4272 2023-07-26 18:43:18.552471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/helm_pb2.py
+-rw-r--r--   0        0        0     5454 2023-07-26 18:43:18.708471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/helm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.560471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.700471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3013 2023-07-26 18:43:18.572471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
+-rw-r--r--   0        0        0     4537 2023-07-26 18:43:18.708471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.560471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.692471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1738 2023-07-26 18:43:18.564471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/links_pb2.py
+-rw-r--r--   0        0        0      846 2023-07-26 18:43:18.704471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/links_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.552471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.712471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1338 2023-07-26 18:43:18.564471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/maturity_pb2.py
+-rw-r--r--   0        0        0     1103 2023-07-26 18:43:18.692471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.572471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.700471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1838 2023-07-26 18:43:18.568471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/meta_pb2.py
+-rw-r--r--   0        0        0     2531 2023-07-26 18:43:18.696471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.564471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.700471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1866 2023-07-26 18:43:18.560471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/notification_pb2.py
+-rw-r--r--   0        0        0     1337 2023-07-26 18:43:18.696471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.548471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.692471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7815 2023-07-26 18:43:18.556471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/parameters_pb2.py
+-rw-r--r--   0        0        0    10735 2023-07-26 18:43:18.696471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.568471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.712471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9143 2023-07-26 18:43:18.568471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/program_pb2.py
+-rw-r--r--   0        0        0    15928 2023-07-26 18:43:18.708471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/program_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.564471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.692471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2686 2023-07-26 18:43:18.560471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/retry_pb2.py
+-rw-r--r--   0        0        0     2757 2023-07-26 18:43:18.712471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/retry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.556471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.708471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2804 2023-07-26 18:43:18.556471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/task_pb2.py
+-rw-r--r--   0        0        0     3946 2023-07-26 18:43:18.704471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.572471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.688471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.792471 prodvana-0.2.1/prodvana/proto/prodvana/config_file/__init__.py
+-rw-r--r--   0        0        0     3685 2023-07-26 18:43:18.516471 prodvana-0.2.1/prodvana/proto/prodvana/config_file/config_pb2.py
+-rw-r--r--   0        0        0     4656 2023-07-26 18:43:18.660471 prodvana-0.2.1/prodvana/proto/prodvana/config_file/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.516471 prodvana-0.2.1/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.660471 prodvana-0.2.1/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/__init__.py
+-rw-r--r--   0        0        0     1388 2023-07-26 18:43:18.604471 prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
+-rw-r--r--   0        0        0     1131 2023-07-26 18:43:18.744471 prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.604471 prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.740471 prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.792471 prodvana-0.2.1/prodvana/proto/prodvana/delivery/__init__.py
+-rw-r--r--   0        0        0     2079 2023-07-26 18:43:18.508471 prodvana-0.2.1/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
+-rw-r--r--   0        0        0     2294 2023-07-26 18:43:18.652471 prodvana-0.2.1/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.508471 prodvana-0.2.1/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.648471 prodvana-0.2.1/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/__init__.py
+-rw-r--r--   0        0        0     6161 2023-07-26 18:43:18.528471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/config_pb2.py
+-rw-r--r--   0        0        0     8052 2023-07-26 18:43:18.668471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.532471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.672471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9291 2023-07-26 18:43:18.528471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
+-rw-r--r--   0        0        0     8986 2023-07-26 18:43:18.672471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
+-rw-r--r--   0        0        0    13097 2023-07-26 18:43:18.528471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3909 2023-07-26 18:43:18.672471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2015 2023-07-26 18:43:18.528471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/object_pb2.py
+-rw-r--r--   0        0        0     1862 2023-07-26 18:43:18.668471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.532471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.668471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/__init__.py
+-rw-r--r--   0        0        0    21535 2023-07-26 18:43:18.540471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2.py
+-rw-r--r--   0        0        0    29180 2023-07-26 18:43:18.680471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
+-rw-r--r--   0        0        0    20037 2023-07-26 18:43:18.536471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5752 2023-07-26 18:43:18.676471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/__init__.py
+-rw-r--r--   0        0        0    27197 2023-07-26 18:43:18.532471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
+-rw-r--r--   0        0        0    77697 2023-07-26 18:43:18.672471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.536471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.676471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3601 2023-07-26 22:01:30.060842 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
+-rw-r--r--   0        0        0     8499 2023-07-26 22:01:30.060842 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.536471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.676471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.808471 prodvana-0.2.1/prodvana/proto/prodvana/environment/__init__.py
+-rw-r--r--   0        0        0    16774 2023-07-26 18:43:18.632471 prodvana-0.2.1/prodvana/proto/prodvana/environment/clusters_pb2.py
+-rw-r--r--   0        0        0    37710 2023-07-26 18:43:18.776471 prodvana-0.2.1/prodvana/proto/prodvana/environment/clusters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.636471 prodvana-0.2.1/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.772471 prodvana-0.2.1/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12870 2023-07-26 18:43:18.636471 prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2.py
+-rw-r--r--   0        0        0    18334 2023-07-26 18:43:18.772471 prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
+-rw-r--r--   0        0        0    21499 2023-07-26 18:43:18.632471 prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6311 2023-07-26 18:43:18.772471 prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.808471 prodvana-0.2.1/prodvana/proto/prodvana/events/__init__.py
+-rw-r--r--   0        0        0     4801 2023-07-26 18:43:18.640471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2.py
+-rw-r--r--   0        0        0     5547 2023-07-26 18:43:18.784471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2.pyi
+-rw-r--r--   0        0        0     2714 2023-07-26 18:43:18.644471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      853 2023-07-26 18:43:18.784471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2688 2023-07-26 18:43:18.640471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_pb2.py
+-rw-r--r--   0        0        0     4131 2023-07-26 18:43:18.780471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.644471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.780471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10353 2023-07-26 18:43:18.644471 prodvana-0.2.1/prodvana/proto/prodvana/events/types_pb2.py
+-rw-r--r--   0        0        0    30800 2023-07-26 18:43:18.784471 prodvana-0.2.1/prodvana/proto/prodvana/events/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.644471 prodvana-0.2.1/prodvana/proto/prodvana/events/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.780471 prodvana-0.2.1/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.808471 prodvana-0.2.1/prodvana/proto/prodvana/insights/__init__.py
+-rw-r--r--   0        0        0     2205 2023-07-26 18:43:18.624471 prodvana-0.2.1/prodvana/proto/prodvana/insights/insights_pb2.py
+-rw-r--r--   0        0        0     3508 2023-07-26 18:43:18.760471 prodvana-0.2.1/prodvana/proto/prodvana/insights/insights_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.620471 prodvana-0.2.1/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.764471 prodvana-0.2.1/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/__init__.py
+-rw-r--r--   0        0        0     8344 2023-07-26 18:43:18.592471 prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2.py
+-rw-r--r--   0        0        0    13338 2023-07-26 18:43:18.732471 prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
+-rw-r--r--   0        0        0    12065 2023-07-26 18:43:18.592471 prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3657 2023-07-26 18:43:18.732471 prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/metrics/__init__.py
+-rw-r--r--   0        0        0     3762 2023-07-26 18:43:18.524471 prodvana-0.2.1/prodvana/proto/prodvana/metrics/metrics_pb2.py
+-rw-r--r--   0        0        0     8746 2023-07-26 18:43:18.668471 prodvana-0.2.1/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.524471 prodvana-0.2.1/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.668471 prodvana-0.2.1/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/object/__init__.py
+-rw-r--r--   0        0        0     1657 2023-07-26 18:43:18.544471 prodvana-0.2.1/prodvana/proto/prodvana/object/meta_pb2.py
+-rw-r--r--   0        0        0     1957 2023-07-26 18:43:18.684471 prodvana-0.2.1/prodvana/proto/prodvana/object/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.544471 prodvana-0.2.1/prodvana/proto/prodvana/object/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.684471 prodvana-0.2.1/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/organization/__init__.py
+-rw-r--r--   0        0        0     9808 2023-07-26 18:43:18.544471 prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2.py
+-rw-r--r--   0        0        0     9762 2023-07-26 18:43:18.684471 prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
+-rw-r--r--   0        0        0    14668 2023-07-26 18:43:18.540471 prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4779 2023-07-26 18:43:18.680471 prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2568 2023-07-26 18:43:18.540471 prodvana-0.2.1/prodvana/proto/prodvana/organization/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1972 2023-07-26 18:43:18.680471 prodvana-0.2.1/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.540471 prodvana-0.2.1/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.684471 prodvana-0.2.1/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/__init__.py
+-rw-r--r--   0        0        0     2038 2023-07-26 18:43:18.596471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/object_pb2.py
+-rw-r--r--   0        0        0     2595 2023-07-26 18:43:18.736471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.596471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.732471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6748 2023-07-26 18:43:18.596471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
+-rw-r--r--   0        0        0    11698 2023-07-26 18:43:18.736471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.596471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.736471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.808471 prodvana-0.2.1/prodvana/proto/prodvana/protection/__init__.py
+-rw-r--r--   0        0        0     2777 2023-07-26 18:43:18.620471 prodvana-0.2.1/prodvana/proto/prodvana/protection/attachments_pb2.py
+-rw-r--r--   0        0        0     2860 2023-07-26 18:43:18.760471 prodvana-0.2.1/prodvana/proto/prodvana/protection/attachments_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.620471 prodvana-0.2.1/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.752471 prodvana-0.2.1/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1716 2023-07-26 18:43:18.616471 prodvana-0.2.1/prodvana/proto/prodvana/protection/object_pb2.py
+-rw-r--r--   0        0        0     1545 2023-07-26 18:43:18.760471 prodvana-0.2.1/prodvana/proto/prodvana/protection/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.620471 prodvana-0.2.1/prodvana/proto/prodvana/protection/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.752471 prodvana-0.2.1/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6615 2023-07-26 18:43:18.620471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_config_pb2.py
+-rw-r--r--   0        0        0    10041 2023-07-26 18:43:18.760471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.616471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.756471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8167 2023-07-26 18:43:18.616471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2.py
+-rw-r--r--   0        0        0     8325 2023-07-26 18:43:18.752471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
+-rw-r--r--   0        0        0    12468 2023-07-26 18:43:18.612471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3716 2023-07-26 18:43:18.756471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3938 2023-07-26 18:43:18.616471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_reference_pb2.py
+-rw-r--r--   0        0        0     4997 2023-07-26 18:43:18.756471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.612471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.756471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/__init__.py
+-rw-r--r--   0        0        0     2453 2023-07-26 18:43:18.588471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/object_pb2.py
+-rw-r--r--   0        0        0     3325 2023-07-26 18:43:18.728471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.588471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.724471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7193 2023-07-26 18:43:18.588471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
+-rw-r--r--   0        0        0    12716 2023-07-26 18:43:18.728471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.584471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.728471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10119 2023-07-26 18:43:18.584471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
+-rw-r--r--   0        0        0    11055 2023-07-26 18:43:18.724471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
+-rw-r--r--   0        0        0    15129 2023-07-26 18:43:18.588471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4757 2023-07-26 18:43:18.728471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/repo/__init__.py
+-rw-r--r--   0        0        0     1701 2023-07-26 18:43:18.548471 prodvana-0.2.1/prodvana/proto/prodvana/repo/repo_pb2.py
+-rw-r--r--   0        0        0     2315 2023-07-26 18:43:18.688471 prodvana-0.2.1/prodvana/proto/prodvana/repo/repo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.544471 prodvana-0.2.1/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.684471 prodvana-0.2.1/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/__init__.py
+-rw-r--r--   0        0        0     1434 2023-07-26 18:43:18.600471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/features_pb2.py
+-rw-r--r--   0        0        0     1320 2023-07-26 18:43:18.740471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/features_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.600471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.740471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4579 2023-07-26 18:43:18.600471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
+-rw-r--r--   0        0        0     6995 2023-07-26 18:43:18.736471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.600471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.740471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/scm/__init__.py
+-rw-r--r--   0        0        0     1229 2023-07-26 18:43:18.524471 prodvana-0.2.1/prodvana/proto/prodvana/scm/types_pb2.py
+-rw-r--r--   0        0        0      914 2023-07-26 18:43:18.664471 prodvana-0.2.1/prodvana/proto/prodvana/scm/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.524471 prodvana-0.2.1/prodvana/proto/prodvana/scm/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.664471 prodvana-0.2.1/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.792471 prodvana-0.2.1/prodvana/proto/prodvana/secrets/__init__.py
+-rw-r--r--   0        0        0     6361 2023-07-26 18:43:18.520471 prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
+-rw-r--r--   0        0        0     4586 2023-07-26 18:43:18.660471 prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
+-rw-r--r--   0        0        0     9936 2023-07-26 18:43:18.520471 prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     2847 2023-07-26 18:43:18.660471 prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/service/__init__.py
+-rw-r--r--   0        0        0     4358 2023-07-26 18:43:18.576471 prodvana-0.2.1/prodvana/proto/prodvana/service/object_pb2.py
+-rw-r--r--   0        0        0     7117 2023-07-26 18:43:18.720471 prodvana-0.2.1/prodvana/proto/prodvana/service/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.584471 prodvana-0.2.1/prodvana/proto/prodvana/service/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.712471 prodvana-0.2.1/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1908 2023-07-26 18:43:18.576471 prodvana-0.2.1/prodvana/proto/prodvana/service/parameters_pb2.py
+-rw-r--r--   0        0        0     2424 2023-07-26 18:43:18.716471 prodvana-0.2.1/prodvana/proto/prodvana/service/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.580471 prodvana-0.2.1/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.724471 prodvana-0.2.1/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    26309 2023-07-26 18:43:18.580471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_config_pb2.py
+-rw-r--r--   0        0        0    54314 2023-07-26 18:43:18.716471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.584471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.724471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    31947 2023-07-26 18:43:18.580471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2.py
+-rw-r--r--   0        0        0    38013 2023-07-26 18:43:18.720471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2.pyi
+-rw-r--r--   0        0        0    33828 2023-07-26 18:43:18.580471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     9674 2023-07-26 18:43:18.720471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2198 2023-07-26 18:43:18.576471 prodvana-0.2.1/prodvana/proto/prodvana/service/user_metadata_pb2.py
+-rw-r--r--   0        0        0     2106 2023-07-26 18:43:18.716471 prodvana-0.2.1/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.576471 prodvana-0.2.1/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.720471 prodvana-0.2.1/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/settings/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/__init__.py
+-rw-r--r--   0        0        0     5019 2023-07-26 18:43:18.604471 prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2.py
+-rw-r--r--   0        0        0     5677 2023-07-26 18:43:18.744471 prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
+-rw-r--r--   0        0        0     8214 2023-07-26 18:43:18.604471 prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
+-rw-r--r--   0        0        0     2318 2023-07-26 18:43:18.744471 prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.792471 prodvana-0.2.1/prodvana/proto/prodvana/stat/__init__.py
+-rw-r--r--   0        0        0     1317 2023-07-26 18:43:18.512471 prodvana-0.2.1/prodvana/proto/prodvana/stat/efficiency_pb2.py
+-rw-r--r--   0        0        0     1156 2023-07-26 18:43:18.652471 prodvana-0.2.1/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.512471 prodvana-0.2.1/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.652471 prodvana-0.2.1/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/users/__init__.py
+-rw-r--r--   0        0        0     1361 2023-07-26 18:43:18.612471 prodvana-0.2.1/prodvana/proto/prodvana/users/users_pb2.py
+-rw-r--r--   0        0        0     1451 2023-07-26 18:43:18.748471 prodvana-0.2.1/prodvana/proto/prodvana/users/users_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.612471 prodvana-0.2.1/prodvana/proto/prodvana/users/users_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.752471 prodvana-0.2.1/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.792471 prodvana-0.2.1/prodvana/proto/prodvana/version/__init__.py
+-rw-r--r--   0        0        0     1723 2023-07-26 18:43:18.512471 prodvana-0.2.1/prodvana/proto/prodvana/version/source_metadata_pb2.py
+-rw-r--r--   0        0        0     2817 2023-07-26 18:43:18.652471 prodvana-0.2.1/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.512471 prodvana-0.2.1/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.656471 prodvana-0.2.1/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/volumes/__init__.py
+-rw-r--r--   0        0        0     3089 2023-07-26 18:43:18.592471 prodvana-0.2.1/prodvana/proto/prodvana/volumes/volumes_pb2.py
+-rw-r--r--   0        0        0     4793 2023-07-26 18:43:18.732471 prodvana-0.2.1/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.592471 prodvana-0.2.1/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.732471 prodvana-0.2.1/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.808471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/__init__.py
+-rw-r--r--   0        0        0     3274 2023-07-26 18:43:18.636471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/integration_config_pb2.py
+-rw-r--r--   0        0        0     4328 2023-07-26 18:43:18.776471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.640471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.780471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    36604 2023-07-26 18:43:18.636471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
+-rw-r--r--   0        0        0    52034 2023-07-26 18:43:18.776471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
+-rw-r--r--   0        0        0    57702 2023-07-26 18:43:18.640471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
+-rw-r--r--   0        0        0    16676 2023-07-26 18:43:18.776471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-26 18:43:18.812471 prodvana-0.2.1/prodvana/proto/validate/__init__.py
+-rw-r--r--   0        0        0    13684 2023-07-26 18:43:18.648471 prodvana-0.2.1/prodvana/proto/validate/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-07-26 18:43:18.784471 prodvana-0.2.1/prodvana/proto/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-26 18:43:18.648471 prodvana-0.2.1/prodvana/proto/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-26 18:43:18.788471 prodvana-0.2.1/prodvana/proto/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-07 23:25:26.663462 prodvana-0.2.1/prodvana/py.typed
+-rw-r--r--   0        0        0        0 2023-07-07 23:25:26.663462 prodvana-0.2.1/prodvana/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-07-07 23:25:26.663462 prodvana-0.2.1/prodvana/utils/desired_states.py
+-rw-r--r--   0        0        0     1434 2023-07-20 20:38:16.234138 prodvana-0.2.1/prodvana/utils/parameters.py
+-rw-r--r--   0        0        0     1731 2023-07-20 20:38:16.234138 prodvana-0.2.1/prodvana/utils/protections.py
+-rw-r--r--   0        0        0     4079 2023-07-07 23:25:26.663462 prodvana-0.2.1/prodvana/utils/service_config.py
+-rw-r--r--   0        0        0     7140 2023-07-07 23:25:26.663462 prodvana-0.2.1/prodvana/utils/tests/test_service_config.py
+-rw-r--r--   0        0        0      746 2023-07-26 22:08:49.976855 prodvana-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.2.1/PKG-INFO
```

### Comparing `prodvana-0.2.0/prodvana/client.py` & `prodvana-0.2.1/prodvana/client.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/application/application_config_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/application/application_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/application/application_config_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/application/application_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/application/object_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/application/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/application/object_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/application/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/application/user_metadata_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/application/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/application/user_metadata_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/application/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/auth/auth_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/capability/capability_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/capability/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/capability/capability_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/capability/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/constants_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/constants_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/constants_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/constants_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/env_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/env_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/env_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/env_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/helm_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/helm_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/helm_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/helm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/links_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/links_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/links_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/maturity_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/maturity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/maturity_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/maturity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/meta_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/meta_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/notification_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/notification_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/parameters_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/parameters_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/program_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/program_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/program_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/program_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/retry_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/retry_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/retry_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/retry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/task_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/task_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/common_config/task_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/common_config/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/config_file/config_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/config_file/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/config_file/config_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/config_file/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/writeback_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/writeback_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/delivery/delivery_config_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/delivery/delivery_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/config_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/object_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from prodvana.proto.prodvana.desired_state.model import desired_state_pb2 as prodvana_dot_desired__state_dot_model_dot_desired__state__pb2
 from prodvana.proto.prodvana.desired_state.model import entity_pb2 as prodvana_dot_desired__state_dot_model_dot_entity__pb2
 from prodvana.proto.prodvana.service import service_config_pb2 as prodvana_dot_service_dot_service__config__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$prodvana/desired_state/manager.proto\x12\x16prodvana.desired_state\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x30prodvana/desired_state/model/desired_state.proto\x1a)prodvana/desired_state/model/entity.proto\x1a%prodvana/service/service_config.proto\x1a\x17validate/validate.proto\"l\n\x12SetDesiredStateReq\x12\x44\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.StateB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x10\n\x08rollback\x18\x02 \x01(\x08\"\xc4\x01\n\x17ValidateDesiredStateReq\x12\x44\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.StateB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x10\n\x08rollback\x18\x02 \x01(\x08\x12Q\n\x18service_instance_configs\x18\x03 \x03(\x0b\x32/.prodvana.service.CompiledServiceInstanceConfig\"/\n\x13SetDesiredStateResp\x12\x18\n\x10\x64\x65sired_state_id\x18\x01 \x01(\t\"e\n+GetServiceDesiredStateConvergenceSummaryReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"b\n\x12StatusExplanations\x12L\n\x13status_explanations\x18\x01 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\"G\n\tDebugLogs\x12:\n\ndebug_logs\x18\x01 \x03(\x0b\x32&.prodvana.desired_state.model.DebugLog\"\xaf\x0f\n\x13\x44\x65siredStateSummary\x12?\n\x0c\x65ntity_graph\x18\x0f \x01(\x0b\x32).prodvana.desired_state.model.EntityGraph\x12\x36\n\x12\x63reation_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12replaced_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x0estarting_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12<\n\x0flast_seen_state\x18\x02 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12:\n\rdesired_state\x18\x03 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12K\n\x08statuses\x18\x04 \x03(\x0b\x32\x39.prodvana.desired_state.DesiredStateSummary.StatusesEntry\x12\x39\n\x15last_update_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x64\n\x15precondition_statuses\x18\x08 \x03(\x0b\x32\x45.prodvana.desired_state.DesiredStateSummary.PreconditionStatusesEntry\x12`\n\x13status_explanations\x18\t \x03(\x0b\x32\x43.prodvana.desired_state.DesiredStateSummary.StatusExplanationsEntry\x12N\n\ndebug_logs\x18\n \x03(\x0b\x32:.prodvana.desired_state.DesiredStateSummary.DebugLogsEntry\x12`\n\x13\x61\x63tion_explanations\x18\x0b \x03(\x0b\x32\x43.prodvana.desired_state.DesiredStateSummary.ActionExplanationsEntry\x12\x65\n\x16last_update_timestamps\x18\x0c \x03(\x0b\x32\x45.prodvana.desired_state.DesiredStateSummary.LastUpdateTimestampsEntry\x12g\n\x17last_fetched_timestamps\x18\r \x03(\x0b\x32\x46.prodvana.desired_state.DesiredStateSummary.LastFetchedTimestampsEntry\x12g\n\x17last_applied_timestamps\x18\x0e \x03(\x0b\x32\x46.prodvana.desired_state.DesiredStateSummary.LastAppliedTimestampsEntry\x1aU\n\rStatusesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0e\x32$.prodvana.desired_state.model.Status:\x02\x38\x01\x1ai\n\x19PreconditionStatusesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12;\n\x05value\x18\x02 \x01(\x0b\x32,.prodvana.desired_state.model.ConditionState:\x02\x38\x01\x1a\x65\n\x17StatusExplanationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32*.prodvana.desired_state.StatusExplanations:\x02\x38\x01\x1aS\n\x0e\x44\x65\x62ugLogsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32!.prodvana.desired_state.DebugLogs:\x02\x38\x01\x1aj\n\x17\x41\x63tionExplanationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12>\n\x05value\x18\x02 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation:\x02\x38\x01\x1aW\n\x19LastUpdateTimestampsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x38\x01\x1aX\n\x1aLastFetchedTimestampsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x38\x01\x1aX\n\x1aLastAppliedTimestampsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x38\x01\"B\n\x1dGetDesiredStateConvergenceReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"e\n%GetDesiredStateConvergenceSummaryResp\x12<\n\x07summary\x18\x01 \x01(\x0b\x32+.prodvana.desired_state.DesiredStateSummary\"l\n,GetServiceDesiredStateConvergenceSummaryResp\x12<\n\x07summary\x18\x01 \x01(\x0b\x32+.prodvana.desired_state.DesiredStateSummary\"Y\n\x1fGetServiceLastConvergedStateReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"w\n GetServiceLastConvergedStateResp\x12S\n\x17service_instance_states\x18\x01 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\"\x81\x01\n GetServiceDesiredStateHistoryReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\"\x81\x01\n!GetServiceDesiredStateHistoryResp\x12\x43\n\x0e\x64\x65sired_states\x18\x01 \x03(\x0b\x32+.prodvana.desired_state.DesiredStateSummary\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"7\n\x12GetDesiredStateReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\x96\x01\n\x13GetDesiredStateResp\x12:\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12\x43\n\x16\x63ompiled_desired_state\x18\x02 \x01(\x0b\x32#.prodvana.desired_state.model.State\"\x9b\x01\n\x18ValidateDesiredStateResp\x12:\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12\x43\n\x16\x63ompiled_desired_state\x18\x02 \x01(\x0b\x32#.prodvana.desired_state.model.State\"a\n\x14SetManualApprovalReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x16\n\x05topic\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x0e\n\x06reject\x18\x03 \x01(\x08\"\x17\n\x15SetManualApprovalResp\"m\n\x12PromoteDeliveryReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\r\n\x05stage\x18\x02 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x03 \x01(\x08\x12\x17\n\x06source\x18\x04 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\x15\n\x13PromoteDeliveryResp\"Q\n\x13\x42ypassProtectionReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x17\n\x06source\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\x16\n\x14\x42ypassProtectionResp\"\x95\x01\n\x1f\x41pproveRuntimeExtensionApplyReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x17\n\x06source\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x36\n\x12\x61pproval_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\"\n ApproveRuntimeExtensionApplyResp2\xc8\x10\n\x13\x44\x65siredStateManager\x12\x89\x01\n\x0fSetDesiredState\x12*.prodvana.desired_state.SetDesiredStateReq\x1a+.prodvana.desired_state.SetDesiredStateResp\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1/desired_states:\x01*\x12\x89\x02\n(GetServiceDesiredStateConvergenceSummary\x12\x43.prodvana.desired_state.GetServiceDesiredStateConvergenceSummaryReq\x1a\x44.prodvana.desired_state.GetServiceDesiredStateConvergenceSummaryResp\"R\x82\xd3\xe4\x93\x02L\x12J/v1/applications/{application=*}/services/{service=*}/latest_desired_state\x12\xe0\x01\n\x1dGetServiceLastConvergedStates\x12\x37.prodvana.desired_state.GetServiceLastConvergedStateReq\x1a\x38.prodvana.desired_state.GetServiceLastConvergedStateResp\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/v1/applications/{application=*}/services/{service=*}/last_converged\x12\xe2\x01\n\x1dGetServiceDesiredStateHistory\x12\x38.prodvana.desired_state.GetServiceDesiredStateHistoryReq\x1a\x39.prodvana.desired_state.GetServiceDesiredStateHistoryResp\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/v1/applications/{application=*}/services/{service=*}/desired_states\x12\x9b\x01\n\x0fGetDesiredState\x12*.prodvana.desired_state.GetDesiredStateReq\x1a+.prodvana.desired_state.GetDesiredStateResp\"/\x82\xd3\xe4\x93\x02)\x12\'/v1/desired_states/{desired_state_id=*}\x12\xd2\x01\n!GetDesiredStateConvergenceSummary\x12\x35.prodvana.desired_state.GetDesiredStateConvergenceReq\x1a=.prodvana.desired_state.GetDesiredStateConvergenceSummaryResp\"7\x82\xd3\xe4\x93\x02\x31\x12//v1/desired_states/{desired_state_id=*}/summary\x12\xa1\x01\n\x14ValidateDesiredState\x12/.prodvana.desired_state.ValidateDesiredStateReq\x1a\x30.prodvana.desired_state.ValidateDesiredStateResp\"&\x82\xd3\xe4\x93\x02 \"\x1b/v1/desired_states/validate:\x01*\x12\xa8\x01\n\x11SetManualApproval\x12,.prodvana.desired_state.SetManualApprovalReq\x1a-.prodvana.desired_state.SetManualApprovalResp\"6\x82\xd3\xe4\x93\x02\x30\"+/v1/desired_states/approve_manual_condition:\x01*\x12\x9a\x01\n\x0fPromoteDelivery\x12*.prodvana.desired_state.PromoteDeliveryReq\x1a+.prodvana.desired_state.PromoteDeliveryResp\".\x82\xd3\xe4\x93\x02(\"#/v1/desired_states/promote_delivery:\x01*\x12\x9e\x01\n\x10\x42ypassProtection\x12+.prodvana.desired_state.BypassProtectionReq\x1a,.prodvana.desired_state.BypassProtectionResp\"/\x82\xd3\xe4\x93\x02)\"$/v1/desired_states/bypass_protection:\x01*\x12\xd0\x01\n\x1c\x41pproveRuntimeExtensionApply\x12\x37.prodvana.desired_state.ApproveRuntimeExtensionApplyReq\x1a\x38.prodvana.desired_state.ApproveRuntimeExtensionApplyResp\"=\x82\xd3\xe4\x93\x02\x37\"2/v1/desired_states/approve_runtime_extension_apply:\x01*BRZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_stateb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$prodvana/desired_state/manager.proto\x12\x16prodvana.desired_state\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x30prodvana/desired_state/model/desired_state.proto\x1a)prodvana/desired_state/model/entity.proto\x1a%prodvana/service/service_config.proto\x1a\x17validate/validate.proto\"l\n\x12SetDesiredStateReq\x12\x44\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.StateB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x10\n\x08rollback\x18\x02 \x01(\x08\"\xc4\x01\n\x17ValidateDesiredStateReq\x12\x44\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.StateB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x10\n\x08rollback\x18\x02 \x01(\x08\x12Q\n\x18service_instance_configs\x18\x03 \x03(\x0b\x32/.prodvana.service.CompiledServiceInstanceConfig\"/\n\x13SetDesiredStateResp\x12\x18\n\x10\x64\x65sired_state_id\x18\x01 \x01(\t\"e\n+GetServiceDesiredStateConvergenceSummaryReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"b\n\x12StatusExplanations\x12L\n\x13status_explanations\x18\x01 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\"G\n\tDebugLogs\x12:\n\ndebug_logs\x18\x01 \x03(\x0b\x32&.prodvana.desired_state.model.DebugLog\"\xaf\x0f\n\x13\x44\x65siredStateSummary\x12?\n\x0c\x65ntity_graph\x18\x0f \x01(\x0b\x32).prodvana.desired_state.model.EntityGraph\x12\x36\n\x12\x63reation_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x12replaced_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x0estarting_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12<\n\x0flast_seen_state\x18\x02 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12:\n\rdesired_state\x18\x03 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12K\n\x08statuses\x18\x04 \x03(\x0b\x32\x39.prodvana.desired_state.DesiredStateSummary.StatusesEntry\x12\x39\n\x15last_update_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x64\n\x15precondition_statuses\x18\x08 \x03(\x0b\x32\x45.prodvana.desired_state.DesiredStateSummary.PreconditionStatusesEntry\x12`\n\x13status_explanations\x18\t \x03(\x0b\x32\x43.prodvana.desired_state.DesiredStateSummary.StatusExplanationsEntry\x12N\n\ndebug_logs\x18\n \x03(\x0b\x32:.prodvana.desired_state.DesiredStateSummary.DebugLogsEntry\x12`\n\x13\x61\x63tion_explanations\x18\x0b \x03(\x0b\x32\x43.prodvana.desired_state.DesiredStateSummary.ActionExplanationsEntry\x12\x65\n\x16last_update_timestamps\x18\x0c \x03(\x0b\x32\x45.prodvana.desired_state.DesiredStateSummary.LastUpdateTimestampsEntry\x12g\n\x17last_fetched_timestamps\x18\r \x03(\x0b\x32\x46.prodvana.desired_state.DesiredStateSummary.LastFetchedTimestampsEntry\x12g\n\x17last_applied_timestamps\x18\x0e \x03(\x0b\x32\x46.prodvana.desired_state.DesiredStateSummary.LastAppliedTimestampsEntry\x1aU\n\rStatusesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0e\x32$.prodvana.desired_state.model.Status:\x02\x38\x01\x1ai\n\x19PreconditionStatusesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12;\n\x05value\x18\x02 \x01(\x0b\x32,.prodvana.desired_state.model.ConditionState:\x02\x38\x01\x1a\x65\n\x17StatusExplanationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32*.prodvana.desired_state.StatusExplanations:\x02\x38\x01\x1aS\n\x0e\x44\x65\x62ugLogsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32!.prodvana.desired_state.DebugLogs:\x02\x38\x01\x1aj\n\x17\x41\x63tionExplanationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12>\n\x05value\x18\x02 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation:\x02\x38\x01\x1aW\n\x19LastUpdateTimestampsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x38\x01\x1aX\n\x1aLastFetchedTimestampsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x38\x01\x1aX\n\x1aLastAppliedTimestampsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x38\x01\"B\n\x1dGetDesiredStateConvergenceReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"e\n%GetDesiredStateConvergenceSummaryResp\x12<\n\x07summary\x18\x01 \x01(\x0b\x32+.prodvana.desired_state.DesiredStateSummary\"l\n,GetServiceDesiredStateConvergenceSummaryResp\x12<\n\x07summary\x18\x01 \x01(\x0b\x32+.prodvana.desired_state.DesiredStateSummary\"Y\n\x1fGetServiceLastConvergedStateReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"w\n GetServiceLastConvergedStateResp\x12S\n\x17service_instance_states\x18\x01 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\"\x81\x01\n GetServiceDesiredStateHistoryReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\"\x81\x01\n!GetServiceDesiredStateHistoryResp\x12\x43\n\x0e\x64\x65sired_states\x18\x01 \x03(\x0b\x32+.prodvana.desired_state.DesiredStateSummary\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"7\n\x12GetDesiredStateReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\x96\x01\n\x13GetDesiredStateResp\x12:\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12\x43\n\x16\x63ompiled_desired_state\x18\x02 \x01(\x0b\x32#.prodvana.desired_state.model.State\"\x9b\x01\n\x18ValidateDesiredStateResp\x12:\n\rdesired_state\x18\x01 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12\x43\n\x16\x63ompiled_desired_state\x18\x02 \x01(\x0b\x32#.prodvana.desired_state.model.State\"\xa0\x01\n\x14SetManualApprovalReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x16\n\x05topic\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x0e\n\x06reject\x18\x03 \x01(\x08\x12=\n\x0bsignal_type\x18\x04 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\"\x17\n\x15SetManualApprovalResp\"m\n\x12PromoteDeliveryReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\r\n\x05stage\x18\x02 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x03 \x01(\x08\x12\x17\n\x06source\x18\x04 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\x15\n\x13PromoteDeliveryResp\"Q\n\x13\x42ypassProtectionReq\x12!\n\x10\x64\x65sired_state_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x17\n\x06source\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\x16\n\x14\x42ypassProtectionResp2\xf5\x0e\n\x13\x44\x65siredStateManager\x12\x89\x01\n\x0fSetDesiredState\x12*.prodvana.desired_state.SetDesiredStateReq\x1a+.prodvana.desired_state.SetDesiredStateResp\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1/desired_states:\x01*\x12\x89\x02\n(GetServiceDesiredStateConvergenceSummary\x12\x43.prodvana.desired_state.GetServiceDesiredStateConvergenceSummaryReq\x1a\x44.prodvana.desired_state.GetServiceDesiredStateConvergenceSummaryResp\"R\x82\xd3\xe4\x93\x02L\x12J/v1/applications/{application=*}/services/{service=*}/latest_desired_state\x12\xe0\x01\n\x1dGetServiceLastConvergedStates\x12\x37.prodvana.desired_state.GetServiceLastConvergedStateReq\x1a\x38.prodvana.desired_state.GetServiceLastConvergedStateResp\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/v1/applications/{application=*}/services/{service=*}/last_converged\x12\xe2\x01\n\x1dGetServiceDesiredStateHistory\x12\x38.prodvana.desired_state.GetServiceDesiredStateHistoryReq\x1a\x39.prodvana.desired_state.GetServiceDesiredStateHistoryResp\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/v1/applications/{application=*}/services/{service=*}/desired_states\x12\x9b\x01\n\x0fGetDesiredState\x12*.prodvana.desired_state.GetDesiredStateReq\x1a+.prodvana.desired_state.GetDesiredStateResp\"/\x82\xd3\xe4\x93\x02)\x12\'/v1/desired_states/{desired_state_id=*}\x12\xd2\x01\n!GetDesiredStateConvergenceSummary\x12\x35.prodvana.desired_state.GetDesiredStateConvergenceReq\x1a=.prodvana.desired_state.GetDesiredStateConvergenceSummaryResp\"7\x82\xd3\xe4\x93\x02\x31\x12//v1/desired_states/{desired_state_id=*}/summary\x12\xa1\x01\n\x14ValidateDesiredState\x12/.prodvana.desired_state.ValidateDesiredStateReq\x1a\x30.prodvana.desired_state.ValidateDesiredStateResp\"&\x82\xd3\xe4\x93\x02 \"\x1b/v1/desired_states/validate:\x01*\x12\xa8\x01\n\x11SetManualApproval\x12,.prodvana.desired_state.SetManualApprovalReq\x1a-.prodvana.desired_state.SetManualApprovalResp\"6\x82\xd3\xe4\x93\x02\x30\"+/v1/desired_states/approve_manual_condition:\x01*\x12\x9a\x01\n\x0fPromoteDelivery\x12*.prodvana.desired_state.PromoteDeliveryReq\x1a+.prodvana.desired_state.PromoteDeliveryResp\".\x82\xd3\xe4\x93\x02(\"#/v1/desired_states/promote_delivery:\x01*\x12\x9e\x01\n\x10\x42ypassProtection\x12+.prodvana.desired_state.BypassProtectionReq\x1a,.prodvana.desired_state.BypassProtectionResp\"/\x82\xd3\xe4\x93\x02)\"$/v1/desired_states/bypass_protection:\x01*BRZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_stateb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.desired_state.manager_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -72,18 +72,14 @@
   _PROMOTEDELIVERYREQ.fields_by_name['desired_state_id']._serialized_options = b'\372B\004r\002\020\001'
   _PROMOTEDELIVERYREQ.fields_by_name['source']._options = None
   _PROMOTEDELIVERYREQ.fields_by_name['source']._serialized_options = b'\372B\004r\002\020\001'
   _BYPASSPROTECTIONREQ.fields_by_name['desired_state_id']._options = None
   _BYPASSPROTECTIONREQ.fields_by_name['desired_state_id']._serialized_options = b'\372B\004r\002\020\001'
   _BYPASSPROTECTIONREQ.fields_by_name['source']._options = None
   _BYPASSPROTECTIONREQ.fields_by_name['source']._serialized_options = b'\372B\004r\002\020\001'
-  _APPROVERUNTIMEEXTENSIONAPPLYREQ.fields_by_name['desired_state_id']._options = None
-  _APPROVERUNTIMEEXTENSIONAPPLYREQ.fields_by_name['desired_state_id']._serialized_options = b'\372B\004r\002\020\001'
-  _APPROVERUNTIMEEXTENSIONAPPLYREQ.fields_by_name['source']._options = None
-  _APPROVERUNTIMEEXTENSIONAPPLYREQ.fields_by_name['source']._serialized_options = b'\372B\004r\002\020\001'
   _DESIREDSTATEMANAGER.methods_by_name['SetDesiredState']._options = None
   _DESIREDSTATEMANAGER.methods_by_name['SetDesiredState']._serialized_options = b'\202\323\344\223\002\027\"\022/v1/desired_states:\001*'
   _DESIREDSTATEMANAGER.methods_by_name['GetServiceDesiredStateConvergenceSummary']._options = None
   _DESIREDSTATEMANAGER.methods_by_name['GetServiceDesiredStateConvergenceSummary']._serialized_options = b'\202\323\344\223\002L\022J/v1/applications/{application=*}/services/{service=*}/latest_desired_state'
   _DESIREDSTATEMANAGER.methods_by_name['GetServiceLastConvergedStates']._options = None
   _DESIREDSTATEMANAGER.methods_by_name['GetServiceLastConvergedStates']._serialized_options = b'\202\323\344\223\002F\022D/v1/applications/{application=*}/services/{service=*}/last_converged'
   _DESIREDSTATEMANAGER.methods_by_name['GetServiceDesiredStateHistory']._options = None
@@ -96,16 +92,14 @@
   _DESIREDSTATEMANAGER.methods_by_name['ValidateDesiredState']._serialized_options = b'\202\323\344\223\002 \"\033/v1/desired_states/validate:\001*'
   _DESIREDSTATEMANAGER.methods_by_name['SetManualApproval']._options = None
   _DESIREDSTATEMANAGER.methods_by_name['SetManualApproval']._serialized_options = b'\202\323\344\223\0020\"+/v1/desired_states/approve_manual_condition:\001*'
   _DESIREDSTATEMANAGER.methods_by_name['PromoteDelivery']._options = None
   _DESIREDSTATEMANAGER.methods_by_name['PromoteDelivery']._serialized_options = b'\202\323\344\223\002(\"#/v1/desired_states/promote_delivery:\001*'
   _DESIREDSTATEMANAGER.methods_by_name['BypassProtection']._options = None
   _DESIREDSTATEMANAGER.methods_by_name['BypassProtection']._serialized_options = b'\202\323\344\223\002)\"$/v1/desired_states/bypass_protection:\001*'
-  _DESIREDSTATEMANAGER.methods_by_name['ApproveRuntimeExtensionApply']._options = None
-  _DESIREDSTATEMANAGER.methods_by_name['ApproveRuntimeExtensionApply']._serialized_options = b'\202\323\344\223\0027\"2/v1/desired_states/approve_runtime_extension_apply:\001*'
   _globals['_SETDESIREDSTATEREQ']._serialized_start=284
   _globals['_SETDESIREDSTATEREQ']._serialized_end=392
   _globals['_VALIDATEDESIREDSTATEREQ']._serialized_start=395
   _globals['_VALIDATEDESIREDSTATEREQ']._serialized_end=591
   _globals['_SETDESIREDSTATERESP']._serialized_start=593
   _globals['_SETDESIREDSTATERESP']._serialized_end=640
   _globals['_GETSERVICEDESIREDSTATECONVERGENCESUMMARYREQ']._serialized_start=642
@@ -148,26 +142,22 @@
   _globals['_GETSERVICEDESIREDSTATEHISTORYRESP']._serialized_end=3643
   _globals['_GETDESIREDSTATEREQ']._serialized_start=3645
   _globals['_GETDESIREDSTATEREQ']._serialized_end=3700
   _globals['_GETDESIREDSTATERESP']._serialized_start=3703
   _globals['_GETDESIREDSTATERESP']._serialized_end=3853
   _globals['_VALIDATEDESIREDSTATERESP']._serialized_start=3856
   _globals['_VALIDATEDESIREDSTATERESP']._serialized_end=4011
-  _globals['_SETMANUALAPPROVALREQ']._serialized_start=4013
-  _globals['_SETMANUALAPPROVALREQ']._serialized_end=4110
-  _globals['_SETMANUALAPPROVALRESP']._serialized_start=4112
-  _globals['_SETMANUALAPPROVALRESP']._serialized_end=4135
-  _globals['_PROMOTEDELIVERYREQ']._serialized_start=4137
-  _globals['_PROMOTEDELIVERYREQ']._serialized_end=4246
-  _globals['_PROMOTEDELIVERYRESP']._serialized_start=4248
-  _globals['_PROMOTEDELIVERYRESP']._serialized_end=4269
-  _globals['_BYPASSPROTECTIONREQ']._serialized_start=4271
-  _globals['_BYPASSPROTECTIONREQ']._serialized_end=4352
-  _globals['_BYPASSPROTECTIONRESP']._serialized_start=4354
-  _globals['_BYPASSPROTECTIONRESP']._serialized_end=4376
-  _globals['_APPROVERUNTIMEEXTENSIONAPPLYREQ']._serialized_start=4379
-  _globals['_APPROVERUNTIMEEXTENSIONAPPLYREQ']._serialized_end=4528
-  _globals['_APPROVERUNTIMEEXTENSIONAPPLYRESP']._serialized_start=4530
-  _globals['_APPROVERUNTIMEEXTENSIONAPPLYRESP']._serialized_end=4564
-  _globals['_DESIREDSTATEMANAGER']._serialized_start=4567
-  _globals['_DESIREDSTATEMANAGER']._serialized_end=6687
+  _globals['_SETMANUALAPPROVALREQ']._serialized_start=4014
+  _globals['_SETMANUALAPPROVALREQ']._serialized_end=4174
+  _globals['_SETMANUALAPPROVALRESP']._serialized_start=4176
+  _globals['_SETMANUALAPPROVALRESP']._serialized_end=4199
+  _globals['_PROMOTEDELIVERYREQ']._serialized_start=4201
+  _globals['_PROMOTEDELIVERYREQ']._serialized_end=4310
+  _globals['_PROMOTEDELIVERYRESP']._serialized_start=4312
+  _globals['_PROMOTEDELIVERYRESP']._serialized_end=4333
+  _globals['_BYPASSPROTECTIONREQ']._serialized_start=4335
+  _globals['_BYPASSPROTECTIONREQ']._serialized_end=4416
+  _globals['_BYPASSPROTECTIONRESP']._serialized_start=4418
+  _globals['_BYPASSPROTECTIONRESP']._serialized_end=4440
+  _globals['_DESIREDSTATEMANAGER']._serialized_start=4443
+  _globals['_DESIREDSTATEMANAGER']._serialized_end=6352
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -515,29 +515,32 @@
 
 class SetManualApprovalReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
     TOPIC_FIELD_NUMBER: builtins.int
     REJECT_FIELD_NUMBER: builtins.int
+    SIGNAL_TYPE_FIELD_NUMBER: builtins.int
     desired_state_id: builtins.str
     topic: builtins.str
     """string application = 2 [(prodvana.proto.validate.rules).string.min_len = 1];
     string service = 3 [(prodvana.proto.validate.rules).string.min_len = 1];
     string release_channel = 4 [(prodvana.proto.validate.rules).string.min_len = 1];
     """
     reject: builtins.bool
+    signal_type: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.SignalType.ValueType
     def __init__(
         self,
         *,
         desired_state_id: builtins.str = ...,
         topic: builtins.str = ...,
         reject: builtins.bool = ...,
+        signal_type: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.SignalType.ValueType = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["desired_state_id", b"desired_state_id", "reject", b"reject", "topic", b"topic"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["desired_state_id", b"desired_state_id", "reject", b"reject", "signal_type", b"signal_type", "topic", b"topic"]) -> None: ...
 
 global___SetManualApprovalReq = SetManualApprovalReq
 
 class SetManualApprovalResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
@@ -599,38 +602,7 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___BypassProtectionResp = BypassProtectionResp
-
-class ApproveRuntimeExtensionApplyReq(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
-    SOURCE_FIELD_NUMBER: builtins.int
-    APPROVAL_TIMESTAMP_FIELD_NUMBER: builtins.int
-    desired_state_id: builtins.str
-    source: builtins.str
-    @property
-    def approval_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
-    def __init__(
-        self,
-        *,
-        desired_state_id: builtins.str = ...,
-        source: builtins.str = ...,
-        approval_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["approval_timestamp", b"approval_timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["approval_timestamp", b"approval_timestamp", "desired_state_id", b"desired_state_id", "source", b"source"]) -> None: ...
-
-global___ApproveRuntimeExtensionApplyReq = ApproveRuntimeExtensionApplyReq
-
-class ApproveRuntimeExtensionApplyResp(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    def __init__(
-        self,
-    ) -> None: ...
-
-global___ApproveRuntimeExtensionApplyResp = ApproveRuntimeExtensionApplyResp
```

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,14 @@
                 response_deserializer=prodvana_dot_desired__state_dot_manager__pb2.PromoteDeliveryResp.FromString,
                 )
         self.BypassProtection = channel.unary_unary(
                 '/prodvana.desired_state.DesiredStateManager/BypassProtection',
                 request_serializer=prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionReq.SerializeToString,
                 response_deserializer=prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionResp.FromString,
                 )
-        self.ApproveRuntimeExtensionApply = channel.unary_unary(
-                '/prodvana.desired_state.DesiredStateManager/ApproveRuntimeExtensionApply',
-                request_serializer=prodvana_dot_desired__state_dot_manager__pb2.ApproveRuntimeExtensionApplyReq.SerializeToString,
-                response_deserializer=prodvana_dot_desired__state_dot_manager__pb2.ApproveRuntimeExtensionApplyResp.FromString,
-                )
 
 
 class DesiredStateManagerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def SetDesiredState(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -130,20 +125,14 @@
 
     def BypassProtection(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ApproveRuntimeExtensionApply(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
 
 def add_DesiredStateManagerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'SetDesiredState': grpc.unary_unary_rpc_method_handler(
                     servicer.SetDesiredState,
                     request_deserializer=prodvana_dot_desired__state_dot_manager__pb2.SetDesiredStateReq.FromString,
                     response_serializer=prodvana_dot_desired__state_dot_manager__pb2.SetDesiredStateResp.SerializeToString,
@@ -189,19 +178,14 @@
                     response_serializer=prodvana_dot_desired__state_dot_manager__pb2.PromoteDeliveryResp.SerializeToString,
             ),
             'BypassProtection': grpc.unary_unary_rpc_method_handler(
                     servicer.BypassProtection,
                     request_deserializer=prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionReq.FromString,
                     response_serializer=prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionResp.SerializeToString,
             ),
-            'ApproveRuntimeExtensionApply': grpc.unary_unary_rpc_method_handler(
-                    servicer.ApproveRuntimeExtensionApply,
-                    request_deserializer=prodvana_dot_desired__state_dot_manager__pb2.ApproveRuntimeExtensionApplyReq.FromString,
-                    response_serializer=prodvana_dot_desired__state_dot_manager__pb2.ApproveRuntimeExtensionApplyResp.SerializeToString,
-            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'prodvana.desired_state.DesiredStateManager', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -373,24 +357,7 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/prodvana.desired_state.DesiredStateManager/BypassProtection',
             prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionReq.SerializeToString,
             prodvana_dot_desired__state_dot_manager__pb2.BypassProtectionResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def ApproveRuntimeExtensionApply(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/prodvana.desired_state.DesiredStateManager/ApproveRuntimeExtensionApply',
-            prodvana_dot_desired__state_dot_manager__pb2.ApproveRuntimeExtensionApplyReq.SerializeToString,
-            prodvana_dot_desired__state_dot_manager__pb2.ApproveRuntimeExtensionApplyResp.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -44,18 +44,14 @@
         prodvana.proto.prodvana.desired_state.manager_pb2.PromoteDeliveryReq,
         prodvana.proto.prodvana.desired_state.manager_pb2.PromoteDeliveryResp,
     ]
     BypassProtection: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.desired_state.manager_pb2.BypassProtectionReq,
         prodvana.proto.prodvana.desired_state.manager_pb2.BypassProtectionResp,
     ]
-    ApproveRuntimeExtensionApply: grpc.UnaryUnaryMultiCallable[
-        prodvana.proto.prodvana.desired_state.manager_pb2.ApproveRuntimeExtensionApplyReq,
-        prodvana.proto.prodvana.desired_state.manager_pb2.ApproveRuntimeExtensionApplyResp,
-    ]
 
 class DesiredStateManagerServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def SetDesiredState(
         self,
         request: prodvana.proto.prodvana.desired_state.manager_pb2.SetDesiredStateReq,
         context: grpc.ServicerContext,
@@ -110,15 +106,9 @@
     ) -> prodvana.proto.prodvana.desired_state.manager_pb2.PromoteDeliveryResp: ...
     @abc.abstractmethod
     def BypassProtection(
         self,
         request: prodvana.proto.prodvana.desired_state.manager_pb2.BypassProtectionReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.desired_state.manager_pb2.BypassProtectionResp: ...
-    @abc.abstractmethod
-    def ApproveRuntimeExtensionApply(
-        self,
-        request: prodvana.proto.prodvana.desired_state.manager_pb2.ApproveRuntimeExtensionApplyReq,
-        context: grpc.ServicerContext,
-    ) -> prodvana.proto.prodvana.desired_state.manager_pb2.ApproveRuntimeExtensionApplyResp: ...
 
 def add_DesiredStateManagerServicer_to_server(servicer: DesiredStateManagerServicer, server: grpc.Server) -> None: ...
```

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from prodvana.proto.prodvana.common_config import program_pb2 as prodvana_dot_common__config_dot_program__pb2
 from prodvana.proto.prodvana.common_config import retry_pb2 as prodvana_dot_common__config_dot_retry__pb2
 from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
 from prodvana.proto.prodvana.environment import clusters_pb2 as prodvana_dot_environment_dot_clusters__pb2
 from prodvana.proto.prodvana.protection import protection_reference_pb2 as prodvana_dot_protection_dot_protection__reference__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0prodvana/desired_state/model/desired_state.proto\x12\x1cprodvana.desired_state.model\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a!prodvana/common_config/task.proto\x1a#prodvana/environment/clusters.proto\x1a.prodvana/protection/protection_reference.proto\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xa8\x06\n\tCondition\x12X\n\x07rc_cond\x18\x01 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.ReleaseChannelStableConditionH\x00\x12Q\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x36.prodvana.desired_state.model.Condition.ManualApprovalH\x00\x12\\\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.CustomTaskSuccessfulConditionH\x00\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x1a\xa7\x01\n\x1dReleaseChannelStableCondition\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x0f\n\x07service\x18\x02 \x01(\t\x12\x12\n\nservice_id\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x05 \x01(\t\x12\x17\n\x0fservice_version\x18\x06 \x01(\t\x1a\x34\n\x0eManualApproval\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x1a\x88\x02\n\x1d\x43ustomTaskSuccessfulCondition\x12\x18\n\x10\x63ustom_task_name\x18\x01 \x01(\t\x12\x66\n\nprotection\x18\x02 \x01(\x0b\x32P.prodvana.desired_state.model.Condition.CustomTaskSuccessfulCondition.ProtectionH\x00\x1a[\n\nProtection\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\ttask_type\x18\x03 \x01(\x0e\x32,.prodvana.desired_state.model.CustomTaskTypeB\x08\n\x06sourceB\x0b\n\tcondition\"\xa0\x01\n\x11\x44\x65liveryExtension\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\x12\x38\n\tlifecycle\x18\x02 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\x12<\n\nreferences\x18\x03 \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\"L\n\nIdentifier\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".prodvana.desired_state.model.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xc5\x03\n\x08Metadata\x12>\n\rpreconditions\x18\x01 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12;\n\ninvariants\x18\x02 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12\x36\n\x04self\x18\x03 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x46\n\x10protection_links\x18\x06 \x03(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12L\n\x13\x64\x65livery_extensions\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.DeliveryExtension\x12\"\n\x1atarget_state_set_by_parent\x18\t \x01(\x08J\x04\x08\x07\x10\x08R\x0bprotections\"\xad\x01\n\x11StatusExplanation\x12\x39\n\x07subject\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\x06reason\x18\x02 \x01(\x0e\x32*.prodvana.desired_state.model.StatusReason\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x10\n\x08messages\x18\x04 \x03(\t\"\x8b\x01\n\x11\x41\x63tionExplanation\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x0b\x61\x63tion_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.ActionType\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xde\x01\n\x07Version\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08replicas\x18\x02 \x01(\x05\x12\x1a\n\x12\x61vailable_replicas\x18\x08 \x01(\x05\x12\x32\n\x0epush_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12\x17\n\x0ftarget_replicas\x18\x06 \x01(\x05\x12\r\n\x05\x64irty\x18\t \x01(\x08J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08R\tunhealthyR\x11unhealthy_reasons\"\x86\x03\n\x14ServiceInstanceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x12\n\nservice_id\x18\x08 \x01(\t\x12\x1a\n\x12release_channel_id\x18\t \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12?\n\x10rollback_version\x18\x06 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12\x10\n\x08rollback\x18\x07 \x01(\x08\x12=\n\x08\x64\x65livery\x18\n \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\"\xf0\x02\n\x0cServiceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x12\n\nservice_id\x18\x05 \x01(\t\x12L\n\x10release_channels\x18\x06 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\x12\x43\n\x0c\x63ustom_tasks\x18\x07 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskState\x12Q\n\x13\x64\x65livery_extensions\x18\t \x03(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"\xa5\x02\n\x11ServiceGroupState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12<\n\x08services\x18\x02 \x03(\x0b\x32*.prodvana.desired_state.model.ServiceState\x12\x43\n\x0c\x63ustom_tasks\x18\x03 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskState\x12Q\n\x13\x64\x65livery_extensions\x18\x05 \x03(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateJ\x04\x08\x04\x10\x05\"\xa8\x02\n\x13\x43\x61naryProgressState\x12H\n\x06status\x18\x01 \x01(\x0e\x32\x38.prodvana.desired_state.model.CanaryProgressState.Status\x12 \n\rcanary_weight\x18\x02 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x15pause_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\r\n\tCOMPLETED\x10\x03\"\x94\x03\n\rDeliveryState\x12\x18\n\x10\x64\x65sired_state_id\x18\x0c \x01(\t\x12\x42\n\x06status\x18\x08 \x01(\x0e\x32\x32.prodvana.desired_state.model.DeliveryState.Status\x12\x0f\n\x07message\x18\x06 \x01(\t\x12J\n\x0f\x63\x61nary_progress\x18\x0b \x03(\x0b\x32\x31.prodvana.desired_state.model.CanaryProgressState\x12\x11\n\tfirst_run\x18\r \x01(\x08\x12\x12\n\ngeneration\x18\x0e \x01(\t\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_PROGRESSING\x10\x01\x12\x11\n\rSTATUS_PAUSED\x10\x02\x12\x12\n\x0eSTATUS_HEALTHY\x10\x03\x12\x14\n\x10STATUS_UNHEALTHY\x10\x04J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"=\n\x1bRuntimeExtensionFetchOutput\x12\r\n\x05\x64irty\x18\x01 \x01(\x08\x12\x0f\n\x07message\x18\x02 \x01(\t\"\x91\n\n\rRuntimeObject\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0bobject_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x42\n\x06status\x18\x06 \x01(\x0e\x32\x32.prodvana.desired_state.model.RuntimeObject.Status\x12?\n\x10rollback_version\x18\x07 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12=\n\x08\x64\x65livery\x18\x08 \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\x12\x18\n\x10version_agnostic\x18\n \x01(\x08\x12\"\n\x1a\x64\x65sired_version_dirty_only\x18\x14 \x01(\x08\x12\x0f\n\x07message\x18\x0c \x01(\t\x12W\n\x11runtime_extension\x18\r \x01(\x0b\x32<.prodvana.desired_state.model.RuntimeObject.RuntimeExtension\x12+\n\x08interval\x18\x0f \x01(\x0b\x32\x19.google.protobuf.Duration\x12*\n\x07timeout\x18\x10 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x17\n\x0foutput_blob_ids\x18\x12 \x03(\t\x12\x12\n\nexit_codes\x18\x13 \x03(\x05\x12%\n\x1drequire_approval_before_apply\x18\x15 \x01(\x08\x1a\xdb\x03\n\x10RuntimeExtension\x12=\n\x05\x61pply\x18\x03 \x01(\x0b\x32..prodvana.environment.CompiledExtensionCommand\x12=\n\x05\x66\x65tch\x18\x01 \x01(\x0b\x32..prodvana.environment.CompiledExtensionCommand\x12\x31\n\x0e\x66\x65tch_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x30\n\rfetch_timeout\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x12\n\nservice_id\x18\x02 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x06 \x01(\t\x12?\n\nparameters\x18\x07 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x08 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x31\n\x04type\x18\t \x01(\x0e\x32#.prodvana.environment.ExtensionType\"0\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\r\n\tSUCCEEDED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0e\x10\x0fJ\x04\x08\x11\x10\x12R\x0eunhealthy_podsR\nstate_hash\"O\n\x0e\x43onditionState\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xd6\x03\n\x0c\x43ontrolState\x12\x10\n\x08rollback\x18\x01 \x01(\x08\x12I\n\x13precondition_states\x18\x02 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x46\n\x10invariant_states\x18\x03 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x0e\n\x06paused\x18\x04 \x01(\x08\x12L\n\x13status_explanations\x18\x05 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12K\n\x12\x61\x63tion_explanation\x18\x06 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\x12:\n\x16last_fetched_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_applied_timestamp\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb3\x01\n\x13ManualApprovalState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.prodvana.desired_state.model.ManualApprovalStatus\x12\r\n\x05topic\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\"\xc1\x05\n\x05State\x12=\n\x07service\x18\x01 \x01(\x0b\x32*.prodvana.desired_state.model.ServiceStateH\x00\x12N\n\x10service_instance\x18\x02 \x01(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceStateH\x00\x12H\n\rservice_group\x18\x03 \x01(\x0b\x32/.prodvana.desired_state.model.ServiceGroupStateH\x00\x12\x45\n\x0eruntime_object\x18\x04 \x01(\x0b\x32+.prodvana.desired_state.model.RuntimeObjectH\x00\x12L\n\x0fmanual_approval\x18\x05 \x01(\x0b\x32\x31.prodvana.desired_state.model.ManualApprovalStateH\x00\x12\x44\n\x0b\x63ustom_task\x18\x06 \x01(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateH\x00\x12S\n\x15protection_attachment\x18\x07 \x01(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachmentH\x00\x12L\n\x0fprotection_link\x18\x08 \x01(\x0b\x32\x31.prodvana.desired_state.model.ProtectionLinkStateH\x00\x12R\n\x12\x64\x65livery_extension\x18\t \x01(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateH\x00\x42\r\n\x0bstate_oneof\"\x82\x01\n\x0b\x41nnotations\x12I\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32\x34.prodvana.desired_state.model.Annotations.Annotation\x1a(\n\nAnnotation\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xae\x01\n\x18\x43ustomTaskExecutionState\x12>\n\x06status\x18\x01 \x01(\x0e\x32..prodvana.desired_state.model.CustomTaskStatus\x12\x10\n\x08\x61ttempts\x18\x02 \x01(\x03\x12@\n\x1clatest_attempt_end_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xce\x03\n\x0f\x43ustomTaskState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1c\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x04 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x05 \x01(\t\x12\x17\n\x0frelease_channel\x18\x06 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x07 \x01(\t\x12@\n\x07program\x18\t \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\ntask_state\x18\x0c \x01(\x0b\x32\x36.prodvana.desired_state.model.CustomTaskExecutionState\x12\x39\n\x0cretry_config\x18\r \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12\x13\n\x0bservice_ids\x18\x0e \x03(\tJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xeb\x04\n\x13ProtectionLinkState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12=\n\x06status\x18\x02 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\x12:\n\x04link\x18\x03 \x01(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12\x35\n\x11started_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11stopped_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0estopped_reason\x18\x06 \x01(\x0e\x32<.prodvana.desired_state.model.ProtectionLinkState.StopReason\x12;\n\x17\x66irst_success_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa1\x01\n\nStopReason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x17\n\x13LIFECYCLE_COMPLETED\x10\x01\x12\x12\n\x0eSUCCEEDED_ONCE\x10\x02\x12\x1a\n\x16SUCCEEDED_FOR_DURATION\x10\x03\x12\r\n\tTIMED_OUT\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x44\x45LETED\x10\x06\x12\x15\n\x11MANUALLY_BYPASSED\x10\x07\"\x89\x04\n\x14ProtectionAttachment\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x46\n\x17last_completed_versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12\x15\n\rprotection_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\x81\x05\n\x16\x44\x65liveryExtensionState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x14\n\x0c\x65xtension_id\x18\x03 \x01(\t\x12\x1d\n\x15\x65xtension_instance_id\x18\n \x01(\t\x12\x38\n\tlifecycle\x18\x0b \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12<\n\nreferences\x18\x0c \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\x12=\n\x06status\x18\r \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xf6\x03\n\x06Signal\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\x12Z\n\x12\x64\x65livery_promotion\x18\x02 \x01(\x0b\x32<.prodvana.desired_state.model.Signal.DeliveryPromotionConfigH\x00\x12R\n\x11protection_bypass\x18\x03 \x01(\x0b\x32\x35.prodvana.desired_state.model.Signal.ProtectionBypassH\x00\x12\x63\n\x1aruntime_extension_approval\x18\x04 \x01(\x0b\x32=.prodvana.desired_state.model.Signal.RuntimeExtensionApprovalH\x00\x1a\x36\n\x17\x44\x65liveryPromotionConfig\x12\r\n\x05stage\x18\x01 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x02 \x01(\x08\x1a\x12\n\x10ProtectionBypass\x1aI\n\x18RuntimeExtensionApproval\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\n\x06\x63onfig\"?\n\x08\x44\x65\x62ugLog\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03log\x18\x02 \x01(\t*\xcb\x01\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x14\n\x10SERVICE_INSTANCE\x10\x02\x12\x11\n\rSERVICE_GROUP\x10\x03\x12\x12\n\x0eRUNTIME_OBJECT\x10\x04\x12\x13\n\x0fMANUAL_APPROVAL\x10\x05\x12\x0f\n\x0b\x43USTOM_TASK\x10\x06\x12\x19\n\x15PROTECTION_ATTACHMENT\x10\x07\x12\x13\n\x0fPROTECTION_LINK\x10\x08\x12\x16\n\x12\x44\x45LIVERY_EXTENSION\x10\t*\x9a\x01\n\x0e\x43ustomTaskType\x12\x1c\n\x18\x43USTOM_TASK_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11PRE_APPROVAL_TASK\x10\x01\x12\x0c\n\x08\x41PPROVAL\x10\x02\x12\x16\n\x12POST_APPROVAL_TASK\x10\x03\x12\x13\n\x0f\x44\x45PLOYMENT_TASK\x10\x04\x12\x18\n\x14POST_DEPLOYMENT_TASK\x10\x05*\xf0\x01\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0e\n\nCONVERGING\x10\x01\x12\r\n\tCONVERGED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x10\n\x0cROLLING_BACK\x10\x04\x12\x0f\n\x0bROLLED_BACK\x10\x05\x12\x13\n\x0f\x46\x41ILED_ROLLBACK\x10\x0c\x12\n\n\x06PAUSED\x10\x06\x12\x10\n\x0c\x43HILD_PAUSED\x10\x07\x12\x19\n\x15WAITING_PRECONDITIONS\x10\x08\x12\x0c\n\x08REPLACED\x10\t\x12\x1b\n\x17WAITING_MANUAL_APPROVAL\x10\n\x12\x0b\n\x07\x44\x45LETED\x10\x0b*R\n\x0cSimpleStatus\x12\x0e\n\nSS_UNKNOWN\x10\x00\x12\x11\n\rSS_CONVERGING\x10\x01\x12\x10\n\x0cSS_CONVERGED\x10\x02\x12\r\n\tSS_FAILED\x10\x03*\xff\x01\n\x0cStatusReason\x12\x12\n\x0eREASON_UNKNOWN\x10\x00\x12\x14\n\x10NO_CURRENT_STATE\x10\x01\x12\x10\n\x0c\x41PPLY_FAILED\x10\x02\x12\x12\n\x0eUNHEALTHY_PODS\x10\x03\x12\x11\n\rUPDATING_PODS\x10\x04\x12\x14\n\x10VERSION_MISMATCH\x10\x05\x12\x19\n\x15RUNTIME_OBJECT_FAILED\x10\x06\x12\x18\n\x14PRECONDITIONS_FAILED\x10\x07\x12\x1c\n\x18MANUAL_APPROVAL_REJECTED\x10\x08\x12\x10\n\x0cSTUCK_ENTITY\x10\t\x12\x11\n\rVERSION_DIRTY\x10\n*r\n\nActionType\x12\x17\n\x13\x41\x43TION_TYPE_UNKNOWN\x10\x00\x12\x18\n\x14\x41\x43TION_TYPE_APPLYING\x10\x01\x12\x17\n\x13\x41\x43TION_TYPE_APPLIED\x10\x02\x12\x18\n\x14\x41\x43TION_TYPE_COMPLETE\x10\x03*\x96\x01\n\x0f\x43onditionStatus\x12\x1c\n\x18\x43ONDITION_UNKNOWN_STATUS\x10\x00\x12\x15\n\x11\x43ONDITION_PENDING\x10\x01\x12\x17\n\x13\x43ONDITION_SATISFIED\x10\x02\x12\x1f\n\x1b\x43ONDITION_MANUALLY_BYPASSED\x10\x03\x12\x14\n\x10\x43ONDITION_FAILED\x10\x04*?\n\x14ManualApprovalStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x41PPROVED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02*\x85\x01\n\x10\x43ustomTaskStatus\x12\x17\n\x13\x43USTOM_TASK_PENDING\x10\x00\x12\x1a\n\x16\x43USTOM_TASK_SUCCESSFUL\x10\x01\x12!\n\x1d\x43USTOM_TASK_RETRIES_EXHAUSTED\x10\x02\x12\x19\n\x15\x43USTOM_TASK_TIMED_OUT\x10\x03*o\n\nSignalType\x12\x12\n\x0eSIGNAL_UNKNOWN\x10\x00\x12\x16\n\x12\x44\x45LIVERY_PROMOTION\x10\x01\x12\x15\n\x11PROTECTION_BYPASS\x10\x02\x12\x1e\n\x1aRUNTIME_EXTENSION_APPROVAL\x10\x03\x42XZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0prodvana/desired_state/model/desired_state.proto\x12\x1cprodvana.desired_state.model\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a!prodvana/common_config/task.proto\x1a#prodvana/environment/clusters.proto\x1a.prodvana/protection/protection_reference.proto\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xa8\x06\n\tCondition\x12X\n\x07rc_cond\x18\x01 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.ReleaseChannelStableConditionH\x00\x12Q\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x36.prodvana.desired_state.model.Condition.ManualApprovalH\x00\x12\\\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.CustomTaskSuccessfulConditionH\x00\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x1a\xa7\x01\n\x1dReleaseChannelStableCondition\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x0f\n\x07service\x18\x02 \x01(\t\x12\x12\n\nservice_id\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x05 \x01(\t\x12\x17\n\x0fservice_version\x18\x06 \x01(\t\x1a\x34\n\x0eManualApproval\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x1a\x88\x02\n\x1d\x43ustomTaskSuccessfulCondition\x12\x18\n\x10\x63ustom_task_name\x18\x01 \x01(\t\x12\x66\n\nprotection\x18\x02 \x01(\x0b\x32P.prodvana.desired_state.model.Condition.CustomTaskSuccessfulCondition.ProtectionH\x00\x1a[\n\nProtection\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\ttask_type\x18\x03 \x01(\x0e\x32,.prodvana.desired_state.model.CustomTaskTypeB\x08\n\x06sourceB\x0b\n\tcondition\"\xa0\x01\n\x11\x44\x65liveryExtension\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\x12\x38\n\tlifecycle\x18\x02 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\x12<\n\nreferences\x18\x03 \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\"L\n\nIdentifier\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".prodvana.desired_state.model.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xc5\x03\n\x08Metadata\x12>\n\rpreconditions\x18\x01 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12;\n\ninvariants\x18\x02 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12\x36\n\x04self\x18\x03 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x46\n\x10protection_links\x18\x06 \x03(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12L\n\x13\x64\x65livery_extensions\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.DeliveryExtension\x12\"\n\x1atarget_state_set_by_parent\x18\t \x01(\x08J\x04\x08\x07\x10\x08R\x0bprotections\"\xad\x01\n\x11StatusExplanation\x12\x39\n\x07subject\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\x06reason\x18\x02 \x01(\x0e\x32*.prodvana.desired_state.model.StatusReason\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x10\n\x08messages\x18\x04 \x03(\t\"\x8b\x01\n\x11\x41\x63tionExplanation\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x0b\x61\x63tion_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.ActionType\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xde\x01\n\x07Version\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08replicas\x18\x02 \x01(\x05\x12\x1a\n\x12\x61vailable_replicas\x18\x08 \x01(\x05\x12\x32\n\x0epush_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12\x17\n\x0ftarget_replicas\x18\x06 \x01(\x05\x12\r\n\x05\x64irty\x18\t \x01(\x08J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08R\tunhealthyR\x11unhealthy_reasons\"\x86\x03\n\x14ServiceInstanceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x12\n\nservice_id\x18\x08 \x01(\t\x12\x1a\n\x12release_channel_id\x18\t \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12?\n\x10rollback_version\x18\x06 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12\x10\n\x08rollback\x18\x07 \x01(\x08\x12=\n\x08\x64\x65livery\x18\n \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\"\xf0\x02\n\x0cServiceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x12\n\nservice_id\x18\x05 \x01(\t\x12L\n\x10release_channels\x18\x06 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\x12\x43\n\x0c\x63ustom_tasks\x18\x07 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskState\x12Q\n\x13\x64\x65livery_extensions\x18\t \x03(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"\xa5\x02\n\x11ServiceGroupState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12<\n\x08services\x18\x02 \x03(\x0b\x32*.prodvana.desired_state.model.ServiceState\x12\x43\n\x0c\x63ustom_tasks\x18\x03 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskState\x12Q\n\x13\x64\x65livery_extensions\x18\x05 \x03(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateJ\x04\x08\x04\x10\x05\"\xa8\x02\n\x13\x43\x61naryProgressState\x12H\n\x06status\x18\x01 \x01(\x0e\x32\x38.prodvana.desired_state.model.CanaryProgressState.Status\x12 \n\rcanary_weight\x18\x02 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x15pause_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\r\n\tCOMPLETED\x10\x03\"\x94\x03\n\rDeliveryState\x12\x18\n\x10\x64\x65sired_state_id\x18\x0c \x01(\t\x12\x42\n\x06status\x18\x08 \x01(\x0e\x32\x32.prodvana.desired_state.model.DeliveryState.Status\x12\x0f\n\x07message\x18\x06 \x01(\t\x12J\n\x0f\x63\x61nary_progress\x18\x0b \x03(\x0b\x32\x31.prodvana.desired_state.model.CanaryProgressState\x12\x11\n\tfirst_run\x18\r \x01(\x08\x12\x12\n\ngeneration\x18\x0e \x01(\t\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_PROGRESSING\x10\x01\x12\x11\n\rSTATUS_PAUSED\x10\x02\x12\x12\n\x0eSTATUS_HEALTHY\x10\x03\x12\x14\n\x10STATUS_UNHEALTHY\x10\x04J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"=\n\x1bRuntimeExtensionFetchOutput\x12\r\n\x05\x64irty\x18\x01 \x01(\x08\x12\x0f\n\x07message\x18\x02 \x01(\t\"\xda\n\n\rRuntimeObject\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0bobject_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x42\n\x06status\x18\x06 \x01(\x0e\x32\x32.prodvana.desired_state.model.RuntimeObject.Status\x12?\n\x10rollback_version\x18\x07 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12=\n\x08\x64\x65livery\x18\x08 \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\x12\x18\n\x10version_agnostic\x18\n \x01(\x08\x12\"\n\x1a\x64\x65sired_version_dirty_only\x18\x14 \x01(\x08\x12\x0f\n\x07message\x18\x0c \x01(\t\x12W\n\x11runtime_extension\x18\r \x01(\x0b\x32<.prodvana.desired_state.model.RuntimeObject.RuntimeExtension\x12+\n\x08interval\x18\x0f \x01(\x0b\x32\x19.google.protobuf.Duration\x12*\n\x07timeout\x18\x10 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x17\n\x0foutput_blob_ids\x18\x12 \x03(\t\x12\x12\n\nexit_codes\x18\x13 \x03(\x05\x12%\n\x1drequire_approval_before_apply\x18\x15 \x01(\x08\x12G\n\x10missing_approval\x18\x16 \x01(\x0b\x32-.prodvana.desired_state.model.MissingApproval\x1a\xdb\x03\n\x10RuntimeExtension\x12=\n\x05\x61pply\x18\x03 \x01(\x0b\x32..prodvana.environment.CompiledExtensionCommand\x12=\n\x05\x66\x65tch\x18\x01 \x01(\x0b\x32..prodvana.environment.CompiledExtensionCommand\x12\x31\n\x0e\x66\x65tch_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x30\n\rfetch_timeout\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x12\n\nservice_id\x18\x02 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x06 \x01(\t\x12?\n\nparameters\x18\x07 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x08 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x31\n\x04type\x18\t \x01(\x0e\x32#.prodvana.environment.ExtensionType\"0\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\r\n\tSUCCEEDED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0e\x10\x0fJ\x04\x08\x11\x10\x12R\x0eunhealthy_podsR\nstate_hash\"O\n\x0e\x43onditionState\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xd6\x03\n\x0c\x43ontrolState\x12\x10\n\x08rollback\x18\x01 \x01(\x08\x12I\n\x13precondition_states\x18\x02 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x46\n\x10invariant_states\x18\x03 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x0e\n\x06paused\x18\x04 \x01(\x08\x12L\n\x13status_explanations\x18\x05 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12K\n\x12\x61\x63tion_explanation\x18\x06 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\x12:\n\x16last_fetched_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_applied_timestamp\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb3\x01\n\x13ManualApprovalState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.prodvana.desired_state.model.ManualApprovalStatus\x12\r\n\x05topic\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\"\xc1\x05\n\x05State\x12=\n\x07service\x18\x01 \x01(\x0b\x32*.prodvana.desired_state.model.ServiceStateH\x00\x12N\n\x10service_instance\x18\x02 \x01(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceStateH\x00\x12H\n\rservice_group\x18\x03 \x01(\x0b\x32/.prodvana.desired_state.model.ServiceGroupStateH\x00\x12\x45\n\x0eruntime_object\x18\x04 \x01(\x0b\x32+.prodvana.desired_state.model.RuntimeObjectH\x00\x12L\n\x0fmanual_approval\x18\x05 \x01(\x0b\x32\x31.prodvana.desired_state.model.ManualApprovalStateH\x00\x12\x44\n\x0b\x63ustom_task\x18\x06 \x01(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateH\x00\x12S\n\x15protection_attachment\x18\x07 \x01(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachmentH\x00\x12L\n\x0fprotection_link\x18\x08 \x01(\x0b\x32\x31.prodvana.desired_state.model.ProtectionLinkStateH\x00\x12R\n\x12\x64\x65livery_extension\x18\t \x01(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateH\x00\x42\r\n\x0bstate_oneof\"\x82\x01\n\x0b\x41nnotations\x12I\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32\x34.prodvana.desired_state.model.Annotations.Annotation\x1a(\n\nAnnotation\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xae\x01\n\x18\x43ustomTaskExecutionState\x12>\n\x06status\x18\x01 \x01(\x0e\x32..prodvana.desired_state.model.CustomTaskStatus\x12\x10\n\x08\x61ttempts\x18\x02 \x01(\x03\x12@\n\x1clatest_attempt_end_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xce\x03\n\x0f\x43ustomTaskState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1c\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x04 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x05 \x01(\t\x12\x17\n\x0frelease_channel\x18\x06 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x07 \x01(\t\x12@\n\x07program\x18\t \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\ntask_state\x18\x0c \x01(\x0b\x32\x36.prodvana.desired_state.model.CustomTaskExecutionState\x12\x39\n\x0cretry_config\x18\r \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12\x13\n\x0bservice_ids\x18\x0e \x03(\tJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xeb\x04\n\x13ProtectionLinkState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12=\n\x06status\x18\x02 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\x12:\n\x04link\x18\x03 \x01(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12\x35\n\x11started_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11stopped_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0estopped_reason\x18\x06 \x01(\x0e\x32<.prodvana.desired_state.model.ProtectionLinkState.StopReason\x12;\n\x17\x66irst_success_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa1\x01\n\nStopReason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x17\n\x13LIFECYCLE_COMPLETED\x10\x01\x12\x12\n\x0eSUCCEEDED_ONCE\x10\x02\x12\x1a\n\x16SUCCEEDED_FOR_DURATION\x10\x03\x12\r\n\tTIMED_OUT\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x44\x45LETED\x10\x06\x12\x15\n\x11MANUALLY_BYPASSED\x10\x07\"\x89\x04\n\x14ProtectionAttachment\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x46\n\x17last_completed_versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12\x15\n\rprotection_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\x81\x05\n\x16\x44\x65liveryExtensionState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x14\n\x0c\x65xtension_id\x18\x03 \x01(\t\x12\x1d\n\x15\x65xtension_instance_id\x18\n \x01(\t\x12\x38\n\tlifecycle\x18\x0b \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12<\n\nreferences\x18\x0c \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\x12=\n\x06status\x18\r \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\x86\x04\n\x06Signal\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\x12Z\n\x12\x64\x65livery_promotion\x18\x02 \x01(\x0b\x32<.prodvana.desired_state.model.Signal.DeliveryPromotionConfigH\x00\x12R\n\x11protection_bypass\x18\x03 \x01(\x0b\x32\x35.prodvana.desired_state.model.Signal.ProtectionBypassH\x00\x12\x63\n\x1aruntime_extension_approval\x18\x04 \x01(\x0b\x32=.prodvana.desired_state.model.Signal.RuntimeExtensionApprovalH\x00\x1a\x36\n\x17\x44\x65liveryPromotionConfig\x12\r\n\x05stage\x18\x01 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x02 \x01(\x08\x1a\x12\n\x10ProtectionBypass\x1aY\n\x18RuntimeExtensionApproval\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06reject\x18\x02 \x01(\x08\x42\x08\n\x06\x63onfig\"?\n\x08\x44\x65\x62ugLog\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03log\x18\x02 \x01(\t\"j\n\x0fMissingApproval\x12\x18\n\x10\x64\x65sired_state_id\x18\x01 \x01(\t\x12=\n\x0bsignal_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType*\xcb\x01\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x14\n\x10SERVICE_INSTANCE\x10\x02\x12\x11\n\rSERVICE_GROUP\x10\x03\x12\x12\n\x0eRUNTIME_OBJECT\x10\x04\x12\x13\n\x0fMANUAL_APPROVAL\x10\x05\x12\x0f\n\x0b\x43USTOM_TASK\x10\x06\x12\x19\n\x15PROTECTION_ATTACHMENT\x10\x07\x12\x13\n\x0fPROTECTION_LINK\x10\x08\x12\x16\n\x12\x44\x45LIVERY_EXTENSION\x10\t*\x9a\x01\n\x0e\x43ustomTaskType\x12\x1c\n\x18\x43USTOM_TASK_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11PRE_APPROVAL_TASK\x10\x01\x12\x0c\n\x08\x41PPROVAL\x10\x02\x12\x16\n\x12POST_APPROVAL_TASK\x10\x03\x12\x13\n\x0f\x44\x45PLOYMENT_TASK\x10\x04\x12\x18\n\x14POST_DEPLOYMENT_TASK\x10\x05*\xf0\x01\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0e\n\nCONVERGING\x10\x01\x12\r\n\tCONVERGED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x10\n\x0cROLLING_BACK\x10\x04\x12\x0f\n\x0bROLLED_BACK\x10\x05\x12\x13\n\x0f\x46\x41ILED_ROLLBACK\x10\x0c\x12\n\n\x06PAUSED\x10\x06\x12\x10\n\x0c\x43HILD_PAUSED\x10\x07\x12\x19\n\x15WAITING_PRECONDITIONS\x10\x08\x12\x0c\n\x08REPLACED\x10\t\x12\x1b\n\x17WAITING_MANUAL_APPROVAL\x10\n\x12\x0b\n\x07\x44\x45LETED\x10\x0b*o\n\x0cSimpleStatus\x12\x0e\n\nSS_UNKNOWN\x10\x00\x12\x11\n\rSS_CONVERGING\x10\x01\x12\x10\n\x0cSS_CONVERGED\x10\x02\x12\r\n\tSS_FAILED\x10\x03\x12\x1b\n\x17SS_WAITING_FOR_APPROVAL\x10\x04*\xff\x01\n\x0cStatusReason\x12\x12\n\x0eREASON_UNKNOWN\x10\x00\x12\x14\n\x10NO_CURRENT_STATE\x10\x01\x12\x10\n\x0c\x41PPLY_FAILED\x10\x02\x12\x12\n\x0eUNHEALTHY_PODS\x10\x03\x12\x11\n\rUPDATING_PODS\x10\x04\x12\x14\n\x10VERSION_MISMATCH\x10\x05\x12\x19\n\x15RUNTIME_OBJECT_FAILED\x10\x06\x12\x18\n\x14PRECONDITIONS_FAILED\x10\x07\x12\x1c\n\x18MANUAL_APPROVAL_REJECTED\x10\x08\x12\x10\n\x0cSTUCK_ENTITY\x10\t\x12\x11\n\rVERSION_DIRTY\x10\n*r\n\nActionType\x12\x17\n\x13\x41\x43TION_TYPE_UNKNOWN\x10\x00\x12\x18\n\x14\x41\x43TION_TYPE_APPLYING\x10\x01\x12\x17\n\x13\x41\x43TION_TYPE_APPLIED\x10\x02\x12\x18\n\x14\x41\x43TION_TYPE_COMPLETE\x10\x03*\x96\x01\n\x0f\x43onditionStatus\x12\x1c\n\x18\x43ONDITION_UNKNOWN_STATUS\x10\x00\x12\x15\n\x11\x43ONDITION_PENDING\x10\x01\x12\x17\n\x13\x43ONDITION_SATISFIED\x10\x02\x12\x1f\n\x1b\x43ONDITION_MANUALLY_BYPASSED\x10\x03\x12\x14\n\x10\x43ONDITION_FAILED\x10\x04*?\n\x14ManualApprovalStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x41PPROVED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02*\x85\x01\n\x10\x43ustomTaskStatus\x12\x17\n\x13\x43USTOM_TASK_PENDING\x10\x00\x12\x1a\n\x16\x43USTOM_TASK_SUCCESSFUL\x10\x01\x12!\n\x1d\x43USTOM_TASK_RETRIES_EXHAUSTED\x10\x02\x12\x19\n\x15\x43USTOM_TASK_TIMED_OUT\x10\x03*\x8b\x01\n\nSignalType\x12\x12\n\x0eSIGNAL_UNKNOWN\x10\x00\x12\x16\n\x12\x44\x45LIVERY_PROMOTION\x10\x01\x12\x15\n\x11PROTECTION_BYPASS\x10\x02\x12\x1e\n\x1aRUNTIME_EXTENSION_APPROVAL\x10\x03\x12\x1a\n\x16SIGNAL_MANUAL_APPROVAL\x10\x04\x42XZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.desired_state.model.desired_state_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -35,34 +35,34 @@
   _CANARYPROGRESSSTATE.fields_by_name['canary_weight']._serialized_options = b'\372B\006\032\004\030d(\000'
   _CUSTOMTASKSTATE.fields_by_name['name']._options = None
   _CUSTOMTASKSTATE.fields_by_name['name']._serialized_options = b'\372B\004r\002\020\001'
   _CUSTOMTASKSTATE.fields_by_name['description']._options = None
   _CUSTOMTASKSTATE.fields_by_name['description']._serialized_options = b'\372B\004r\002\020\001'
   _CUSTOMTASKSTATE.fields_by_name['program']._options = None
   _CUSTOMTASKSTATE.fields_by_name['program']._serialized_options = b'\372B\005\212\001\002\020\001'
-  _globals['_TYPE']._serialized_start=10281
-  _globals['_TYPE']._serialized_end=10484
-  _globals['_CUSTOMTASKTYPE']._serialized_start=10487
-  _globals['_CUSTOMTASKTYPE']._serialized_end=10641
-  _globals['_STATUS']._serialized_start=10644
-  _globals['_STATUS']._serialized_end=10884
-  _globals['_SIMPLESTATUS']._serialized_start=10886
-  _globals['_SIMPLESTATUS']._serialized_end=10968
-  _globals['_STATUSREASON']._serialized_start=10971
-  _globals['_STATUSREASON']._serialized_end=11226
-  _globals['_ACTIONTYPE']._serialized_start=11228
-  _globals['_ACTIONTYPE']._serialized_end=11342
-  _globals['_CONDITIONSTATUS']._serialized_start=11345
-  _globals['_CONDITIONSTATUS']._serialized_end=11495
-  _globals['_MANUALAPPROVALSTATUS']._serialized_start=11497
-  _globals['_MANUALAPPROVALSTATUS']._serialized_end=11560
-  _globals['_CUSTOMTASKSTATUS']._serialized_start=11563
-  _globals['_CUSTOMTASKSTATUS']._serialized_end=11696
-  _globals['_SIGNALTYPE']._serialized_start=11698
-  _globals['_SIGNALTYPE']._serialized_end=11809
+  _globals['_TYPE']._serialized_start=10478
+  _globals['_TYPE']._serialized_end=10681
+  _globals['_CUSTOMTASKTYPE']._serialized_start=10684
+  _globals['_CUSTOMTASKTYPE']._serialized_end=10838
+  _globals['_STATUS']._serialized_start=10841
+  _globals['_STATUS']._serialized_end=11081
+  _globals['_SIMPLESTATUS']._serialized_start=11083
+  _globals['_SIMPLESTATUS']._serialized_end=11194
+  _globals['_STATUSREASON']._serialized_start=11197
+  _globals['_STATUSREASON']._serialized_end=11452
+  _globals['_ACTIONTYPE']._serialized_start=11454
+  _globals['_ACTIONTYPE']._serialized_end=11568
+  _globals['_CONDITIONSTATUS']._serialized_start=11571
+  _globals['_CONDITIONSTATUS']._serialized_end=11721
+  _globals['_MANUALAPPROVALSTATUS']._serialized_start=11723
+  _globals['_MANUALAPPROVALSTATUS']._serialized_end=11786
+  _globals['_CUSTOMTASKSTATUS']._serialized_start=11789
+  _globals['_CUSTOMTASKSTATUS']._serialized_end=11922
+  _globals['_SIGNALTYPE']._serialized_start=11925
+  _globals['_SIGNALTYPE']._serialized_end=12064
   _globals['_PROTECTIONLINK']._serialized_start=407
   _globals['_PROTECTIONLINK']._serialized_end=519
   _globals['_CONDITION']._serialized_start=522
   _globals['_CONDITION']._serialized_end=1330
   _globals['_CONDITION_RELEASECHANNELSTABLECONDITION']._serialized_start=829
   _globals['_CONDITION_RELEASECHANNELSTABLECONDITION']._serialized_end=996
   _globals['_CONDITION_MANUALAPPROVAL']._serialized_start=998
@@ -96,47 +96,49 @@
   _globals['_DELIVERYSTATE']._serialized_start=3932
   _globals['_DELIVERYSTATE']._serialized_end=4336
   _globals['_DELIVERYSTATE_STATUS']._serialized_start=4175
   _globals['_DELIVERYSTATE_STATUS']._serialized_end=4288
   _globals['_RUNTIMEEXTENSIONFETCHOUTPUT']._serialized_start=4338
   _globals['_RUNTIMEEXTENSIONFETCHOUTPUT']._serialized_end=4399
   _globals['_RUNTIMEOBJECT']._serialized_start=4402
-  _globals['_RUNTIMEOBJECT']._serialized_end=5699
-  _globals['_RUNTIMEOBJECT_RUNTIMEEXTENSION']._serialized_start=5122
-  _globals['_RUNTIMEOBJECT_RUNTIMEEXTENSION']._serialized_end=5597
-  _globals['_RUNTIMEOBJECT_STATUS']._serialized_start=5599
-  _globals['_RUNTIMEOBJECT_STATUS']._serialized_end=5647
-  _globals['_CONDITIONSTATE']._serialized_start=5701
-  _globals['_CONDITIONSTATE']._serialized_end=5780
-  _globals['_CONTROLSTATE']._serialized_start=5783
-  _globals['_CONTROLSTATE']._serialized_end=6253
-  _globals['_MANUALAPPROVALSTATE']._serialized_start=6256
-  _globals['_MANUALAPPROVALSTATE']._serialized_end=6435
-  _globals['_STATE']._serialized_start=6438
-  _globals['_STATE']._serialized_end=7143
-  _globals['_ANNOTATIONS']._serialized_start=7146
-  _globals['_ANNOTATIONS']._serialized_end=7276
-  _globals['_ANNOTATIONS_ANNOTATION']._serialized_start=7236
-  _globals['_ANNOTATIONS_ANNOTATION']._serialized_end=7276
-  _globals['_CUSTOMTASKEXECUTIONSTATE']._serialized_start=7279
-  _globals['_CUSTOMTASKEXECUTIONSTATE']._serialized_end=7453
-  _globals['_CUSTOMTASKSTATE']._serialized_start=7456
-  _globals['_CUSTOMTASKSTATE']._serialized_end=7918
-  _globals['_PROTECTIONLINKSTATE']._serialized_start=7921
-  _globals['_PROTECTIONLINKSTATE']._serialized_end=8540
-  _globals['_PROTECTIONLINKSTATE_STOPREASON']._serialized_start=8379
-  _globals['_PROTECTIONLINKSTATE_STOPREASON']._serialized_end=8540
-  _globals['_PROTECTIONATTACHMENT']._serialized_start=8543
-  _globals['_PROTECTIONATTACHMENT']._serialized_end=9064
-  _globals['_DELIVERYEXTENSIONSTATE']._serialized_start=9067
-  _globals['_DELIVERYEXTENSIONSTATE']._serialized_end=9708
-  _globals['_SIGNAL']._serialized_start=9711
-  _globals['_SIGNAL']._serialized_end=10213
-  _globals['_SIGNAL_DELIVERYPROMOTIONCONFIG']._serialized_start=10054
-  _globals['_SIGNAL_DELIVERYPROMOTIONCONFIG']._serialized_end=10108
-  _globals['_SIGNAL_PROTECTIONBYPASS']._serialized_start=10110
-  _globals['_SIGNAL_PROTECTIONBYPASS']._serialized_end=10128
-  _globals['_SIGNAL_RUNTIMEEXTENSIONAPPROVAL']._serialized_start=10130
-  _globals['_SIGNAL_RUNTIMEEXTENSIONAPPROVAL']._serialized_end=10203
-  _globals['_DEBUGLOG']._serialized_start=10215
-  _globals['_DEBUGLOG']._serialized_end=10278
+  _globals['_RUNTIMEOBJECT']._serialized_end=5772
+  _globals['_RUNTIMEOBJECT_RUNTIMEEXTENSION']._serialized_start=5195
+  _globals['_RUNTIMEOBJECT_RUNTIMEEXTENSION']._serialized_end=5670
+  _globals['_RUNTIMEOBJECT_STATUS']._serialized_start=5672
+  _globals['_RUNTIMEOBJECT_STATUS']._serialized_end=5720
+  _globals['_CONDITIONSTATE']._serialized_start=5774
+  _globals['_CONDITIONSTATE']._serialized_end=5853
+  _globals['_CONTROLSTATE']._serialized_start=5856
+  _globals['_CONTROLSTATE']._serialized_end=6326
+  _globals['_MANUALAPPROVALSTATE']._serialized_start=6329
+  _globals['_MANUALAPPROVALSTATE']._serialized_end=6508
+  _globals['_STATE']._serialized_start=6511
+  _globals['_STATE']._serialized_end=7216
+  _globals['_ANNOTATIONS']._serialized_start=7219
+  _globals['_ANNOTATIONS']._serialized_end=7349
+  _globals['_ANNOTATIONS_ANNOTATION']._serialized_start=7309
+  _globals['_ANNOTATIONS_ANNOTATION']._serialized_end=7349
+  _globals['_CUSTOMTASKEXECUTIONSTATE']._serialized_start=7352
+  _globals['_CUSTOMTASKEXECUTIONSTATE']._serialized_end=7526
+  _globals['_CUSTOMTASKSTATE']._serialized_start=7529
+  _globals['_CUSTOMTASKSTATE']._serialized_end=7991
+  _globals['_PROTECTIONLINKSTATE']._serialized_start=7994
+  _globals['_PROTECTIONLINKSTATE']._serialized_end=8613
+  _globals['_PROTECTIONLINKSTATE_STOPREASON']._serialized_start=8452
+  _globals['_PROTECTIONLINKSTATE_STOPREASON']._serialized_end=8613
+  _globals['_PROTECTIONATTACHMENT']._serialized_start=8616
+  _globals['_PROTECTIONATTACHMENT']._serialized_end=9137
+  _globals['_DELIVERYEXTENSIONSTATE']._serialized_start=9140
+  _globals['_DELIVERYEXTENSIONSTATE']._serialized_end=9781
+  _globals['_SIGNAL']._serialized_start=9784
+  _globals['_SIGNAL']._serialized_end=10302
+  _globals['_SIGNAL_DELIVERYPROMOTIONCONFIG']._serialized_start=10127
+  _globals['_SIGNAL_DELIVERYPROMOTIONCONFIG']._serialized_end=10181
+  _globals['_SIGNAL_PROTECTIONBYPASS']._serialized_start=10183
+  _globals['_SIGNAL_PROTECTIONBYPASS']._serialized_end=10201
+  _globals['_SIGNAL_RUNTIMEEXTENSIONAPPROVAL']._serialized_start=10203
+  _globals['_SIGNAL_RUNTIMEEXTENSIONAPPROVAL']._serialized_end=10292
+  _globals['_DEBUGLOG']._serialized_start=10304
+  _globals['_DEBUGLOG']._serialized_end=10367
+  _globals['_MISSINGAPPROVAL']._serialized_start=10369
+  _globals['_MISSINGAPPROVAL']._serialized_end=10475
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -141,21 +141,23 @@
 
 class _SimpleStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SimpleStatus.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SS_UNKNOWN: _SimpleStatus.ValueType  # 0
     SS_CONVERGING: _SimpleStatus.ValueType  # 1
     SS_CONVERGED: _SimpleStatus.ValueType  # 2
     SS_FAILED: _SimpleStatus.ValueType  # 3
+    SS_WAITING_FOR_APPROVAL: _SimpleStatus.ValueType  # 4
 
 class SimpleStatus(_SimpleStatus, metaclass=_SimpleStatusEnumTypeWrapper): ...
 
 SS_UNKNOWN: SimpleStatus.ValueType  # 0
 SS_CONVERGING: SimpleStatus.ValueType  # 1
 SS_CONVERGED: SimpleStatus.ValueType  # 2
 SS_FAILED: SimpleStatus.ValueType  # 3
+SS_WAITING_FOR_APPROVAL: SimpleStatus.ValueType  # 4
 global___SimpleStatus = SimpleStatus
 
 class _StatusReason:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _StatusReasonEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_StatusReason.ValueType], builtins.type):  # noqa: F821
@@ -293,21 +295,23 @@
 
 class _SignalTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SignalType.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SIGNAL_UNKNOWN: _SignalType.ValueType  # 0
     DELIVERY_PROMOTION: _SignalType.ValueType  # 1
     PROTECTION_BYPASS: _SignalType.ValueType  # 2
     RUNTIME_EXTENSION_APPROVAL: _SignalType.ValueType  # 3
+    SIGNAL_MANUAL_APPROVAL: _SignalType.ValueType  # 4
 
 class SignalType(_SignalType, metaclass=_SignalTypeEnumTypeWrapper): ...
 
 SIGNAL_UNKNOWN: SignalType.ValueType  # 0
 DELIVERY_PROMOTION: SignalType.ValueType  # 1
 PROTECTION_BYPASS: SignalType.ValueType  # 2
 RUNTIME_EXTENSION_APPROVAL: SignalType.ValueType  # 3
+SIGNAL_MANUAL_APPROVAL: SignalType.ValueType  # 4
 global___SignalType = SignalType
 
 class ProtectionLink(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LIFECYCLE_FIELD_NUMBER: builtins.int
     ATTACHMENT_ID_FIELD_NUMBER: builtins.int
@@ -927,14 +931,15 @@
     MESSAGE_FIELD_NUMBER: builtins.int
     RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
     INTERVAL_FIELD_NUMBER: builtins.int
     TIMEOUT_FIELD_NUMBER: builtins.int
     OUTPUT_BLOB_IDS_FIELD_NUMBER: builtins.int
     EXIT_CODES_FIELD_NUMBER: builtins.int
     REQUIRE_APPROVAL_BEFORE_APPLY_FIELD_NUMBER: builtins.int
+    MISSING_APPROVAL_FIELD_NUMBER: builtins.int
     @property
     def meta(self) -> global___Metadata: ...
     object_type: builtins.str
     namespace: builtins.str
     name: builtins.str
     @property
     def versions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Version]: ...
@@ -963,14 +968,16 @@
         """output_blob_ids and exit_codes are in the same order, assuming output is saved
         if output is saved, this is the ID of the blob to retrieve it, only for run-to-completion objects.
         """
     @property
     def exit_codes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """exit codes, only for run-to-completion objects like jobs"""
     require_approval_before_apply: builtins.bool
+    @property
+    def missing_approval(self) -> global___MissingApproval: ...
     def __init__(
         self,
         *,
         meta: global___Metadata | None = ...,
         object_type: builtins.str = ...,
         namespace: builtins.str = ...,
         name: builtins.str = ...,
@@ -983,17 +990,18 @@
         message: builtins.str = ...,
         runtime_extension: global___RuntimeObject.RuntimeExtension | None = ...,
         interval: google.protobuf.duration_pb2.Duration | None = ...,
         timeout: google.protobuf.duration_pb2.Duration | None = ...,
         output_blob_ids: collections.abc.Iterable[builtins.str] | None = ...,
         exit_codes: collections.abc.Iterable[builtins.int] | None = ...,
         require_approval_before_apply: builtins.bool = ...,
+        missing_approval: global___MissingApproval | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "interval", b"interval", "meta", b"meta", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "timeout", b"timeout"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "desired_version_dirty_only", b"desired_version_dirty_only", "exit_codes", b"exit_codes", "interval", b"interval", "message", b"message", "meta", b"meta", "name", b"name", "namespace", b"namespace", "object_type", b"object_type", "output_blob_ids", b"output_blob_ids", "require_approval_before_apply", b"require_approval_before_apply", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "status", b"status", "timeout", b"timeout", "version_agnostic", b"version_agnostic", "versions", b"versions"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "interval", b"interval", "meta", b"meta", "missing_approval", b"missing_approval", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "timeout", b"timeout"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "desired_version_dirty_only", b"desired_version_dirty_only", "exit_codes", b"exit_codes", "interval", b"interval", "message", b"message", "meta", b"meta", "missing_approval", b"missing_approval", "name", b"name", "namespace", b"namespace", "object_type", b"object_type", "output_blob_ids", b"output_blob_ids", "require_approval_before_apply", b"require_approval_before_apply", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "status", b"status", "timeout", b"timeout", "version_agnostic", b"version_agnostic", "versions", b"versions"]) -> None: ...
 
 global___RuntimeObject = RuntimeObject
 
 class ConditionState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STATUS_FIELD_NUMBER: builtins.int
@@ -1425,28 +1433,32 @@
             self,
         ) -> None: ...
 
     class RuntimeExtensionApproval(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TIMESTAMP_FIELD_NUMBER: builtins.int
+        REJECT_FIELD_NUMBER: builtins.int
         @property
         def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
             """When was the approval issued?
             If this is after last run timestamp, apply can proceed.
-            TODO: Add actor info - who/what approved and how?
-            TODO: Add some kind of token derived from corresponding fetch which can be passed down to apply.
             """
+        reject: builtins.bool
+        """TODO: Add actor info - who/what approved and how?
+        TODO: Add some kind of token derived from corresponding fetch which can be passed down to apply.
+        """
         def __init__(
             self,
             *,
             timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+            reject: builtins.bool = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["reject", b"reject", "timestamp", b"timestamp"]) -> None: ...
 
     TYPE_FIELD_NUMBER: builtins.int
     DELIVERY_PROMOTION_FIELD_NUMBER: builtins.int
     PROTECTION_BYPASS_FIELD_NUMBER: builtins.int
     RUNTIME_EXTENSION_APPROVAL_FIELD_NUMBER: builtins.int
     type: global___SignalType.ValueType
     @property
@@ -1483,7 +1495,24 @@
         ts: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         log: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["ts", b"ts"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["log", b"log", "ts", b"ts"]) -> None: ...
 
 global___DebugLog = DebugLog
+
+class MissingApproval(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
+    SIGNAL_TYPE_FIELD_NUMBER: builtins.int
+    desired_state_id: builtins.str
+    signal_type: global___SignalType.ValueType
+    def __init__(
+        self,
+        *,
+        desired_state_id: builtins.str = ...,
+        signal_type: global___SignalType.ValueType = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["desired_state_id", b"desired_state_id", "signal_type", b"signal_type"]) -> None: ...
+
+global___MissingApproval = MissingApproval
```

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/entity_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/entity_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 
 
 from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
 from prodvana.proto.prodvana.desired_state.model import desired_state_pb2 as prodvana_dot_desired__state_dot_model_dot_desired__state__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/desired_state/model/entity.proto\x12\x1cprodvana.desired_state.model\x1a!prodvana/common_config/task.proto\x1a\x30prodvana/desired_state/model/desired_state.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xb2\x08\n\x06\x45ntity\x12\x34\n\x02id\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x02 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x03 \x01(\t\x12>\n\x0b\x61nnotations\x18\x04 \x01(\x0b\x32).prodvana.desired_state.model.Annotations\x12\x34\n\x06status\x18\x05 \x01(\x0e\x32$.prodvana.desired_state.model.Status\x12\x41\n\rsimple_status\x18\x11 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12;\n\x0estarting_state\x18\x06 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12<\n\x0flast_seen_state\x18\x07 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12:\n\rdesired_state\x18\x08 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12K\n\x15precondition_statuses\x18\t \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12L\n\x13status_explanations\x18\n \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12\x34\n\x04logs\x18\x0b \x03(\x0b\x32&.prodvana.desired_state.model.DebugLog\x12K\n\x12\x61\x63tion_explanation\x18\x0c \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\x12\x39\n\x15last_update_timestamp\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_fetched_timestamp\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_applied_timestamp\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x0c\x64\x65pendencies\x18\x10 \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x38\n\tlifecycle\x18\x12 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\"}\n\x0b\x45ntityGraph\x12\x36\n\x04root\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x36\n\x08\x65ntities\x18\x02 \x03(\x0b\x32$.prodvana.desired_state.model.EntityBXZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/desired_state/model/entity.proto\x12\x1cprodvana.desired_state.model\x1a!prodvana/common_config/task.proto\x1a\x30prodvana/desired_state/model/desired_state.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xed\x08\n\x06\x45ntity\x12\x34\n\x02id\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x02 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x03 \x01(\t\x12>\n\x0b\x61nnotations\x18\x04 \x01(\x0b\x32).prodvana.desired_state.model.Annotations\x12\x34\n\x06status\x18\x05 \x01(\x0e\x32$.prodvana.desired_state.model.Status\x12\x41\n\rsimple_status\x18\x11 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12;\n\x0estarting_state\x18\x06 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12<\n\x0flast_seen_state\x18\x07 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12:\n\rdesired_state\x18\x08 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12\x39\n\x0ctarget_state\x18\x13 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12K\n\x15precondition_statuses\x18\t \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12L\n\x13status_explanations\x18\n \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12\x34\n\x04logs\x18\x0b \x03(\x0b\x32&.prodvana.desired_state.model.DebugLog\x12K\n\x12\x61\x63tion_explanation\x18\x0c \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\x12\x39\n\x15last_update_timestamp\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_fetched_timestamp\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_applied_timestamp\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x0c\x64\x65pendencies\x18\x10 \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x38\n\tlifecycle\x18\x12 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\"}\n\x0b\x45ntityGraph\x12\x36\n\x04root\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x36\n\x08\x65ntities\x18\x02 \x03(\x0b\x32$.prodvana.desired_state.model.EntityBXZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.desired_state.model.entity_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/model'
   _globals['_ENTITY']._serialized_start=194
-  _globals['_ENTITY']._serialized_end=1268
-  _globals['_ENTITYGRAPH']._serialized_start=1270
-  _globals['_ENTITYGRAPH']._serialized_end=1395
+  _globals['_ENTITY']._serialized_end=1327
+  _globals['_ENTITYGRAPH']._serialized_start=1329
+  _globals['_ENTITYGRAPH']._serialized_end=1454
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     ROOT_DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
     ANNOTATIONS_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     SIMPLE_STATUS_FIELD_NUMBER: builtins.int
     STARTING_STATE_FIELD_NUMBER: builtins.int
     LAST_SEEN_STATE_FIELD_NUMBER: builtins.int
     DESIRED_STATE_FIELD_NUMBER: builtins.int
+    TARGET_STATE_FIELD_NUMBER: builtins.int
     PRECONDITION_STATUSES_FIELD_NUMBER: builtins.int
     STATUS_EXPLANATIONS_FIELD_NUMBER: builtins.int
     LOGS_FIELD_NUMBER: builtins.int
     ACTION_EXPLANATION_FIELD_NUMBER: builtins.int
     LAST_UPDATE_TIMESTAMP_FIELD_NUMBER: builtins.int
     LAST_FETCHED_TIMESTAMP_FIELD_NUMBER: builtins.int
     LAST_APPLIED_TIMESTAMP_FIELD_NUMBER: builtins.int
@@ -49,15 +50,19 @@
     status: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Status.ValueType
     simple_status: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.SimpleStatus.ValueType
     @property
     def starting_state(self) -> prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State: ...
     @property
     def last_seen_state(self) -> prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State: ...
     @property
-    def desired_state(self) -> prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State: ...
+    def desired_state(self) -> prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State:
+        """the state we want to get to before calling convergence complete"""
+    @property
+    def target_state(self) -> prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State:
+        """the state we are actually going to apply. when preconditions are met, target state = desired state, otherwise, target state = previous desired state"""
     @property
     def precondition_statuses(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.desired_state.model.desired_state_pb2.ConditionState]: ...
     @property
     def status_explanations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.desired_state.model.desired_state_pb2.StatusExplanation]: ...
     @property
     def logs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.desired_state.model.desired_state_pb2.DebugLog]: ...
     @property
@@ -70,39 +75,40 @@
         """when prodvana last fetched entity state, best effort"""
     @property
     def last_applied_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """when prodvana last applied state for this entity, best effort"""
     @property
     def dependencies(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Identifier]: ...
     lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType
-    """next tag: 19"""
+    """next tag: 20"""
     def __init__(
         self,
         *,
         id: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Identifier | None = ...,
         desired_state_id: builtins.str = ...,
         root_desired_state_id: builtins.str = ...,
         annotations: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Annotations | None = ...,
         status: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Status.ValueType = ...,
         simple_status: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.SimpleStatus.ValueType = ...,
         starting_state: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State | None = ...,
         last_seen_state: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State | None = ...,
         desired_state: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State | None = ...,
+        target_state: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.State | None = ...,
         precondition_statuses: collections.abc.Iterable[prodvana.proto.prodvana.desired_state.model.desired_state_pb2.ConditionState] | None = ...,
         status_explanations: collections.abc.Iterable[prodvana.proto.prodvana.desired_state.model.desired_state_pb2.StatusExplanation] | None = ...,
         logs: collections.abc.Iterable[prodvana.proto.prodvana.desired_state.model.desired_state_pb2.DebugLog] | None = ...,
         action_explanation: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.ActionExplanation | None = ...,
         last_update_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         last_fetched_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         last_applied_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         dependencies: collections.abc.Iterable[prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Identifier] | None = ...,
         lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "annotations", b"annotations", "desired_state", b"desired_state", "id", b"id", "last_applied_timestamp", b"last_applied_timestamp", "last_fetched_timestamp", b"last_fetched_timestamp", "last_seen_state", b"last_seen_state", "last_update_timestamp", b"last_update_timestamp", "starting_state", b"starting_state"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "annotations", b"annotations", "dependencies", b"dependencies", "desired_state", b"desired_state", "desired_state_id", b"desired_state_id", "id", b"id", "last_applied_timestamp", b"last_applied_timestamp", "last_fetched_timestamp", b"last_fetched_timestamp", "last_seen_state", b"last_seen_state", "last_update_timestamp", b"last_update_timestamp", "lifecycle", b"lifecycle", "logs", b"logs", "precondition_statuses", b"precondition_statuses", "root_desired_state_id", b"root_desired_state_id", "simple_status", b"simple_status", "starting_state", b"starting_state", "status", b"status", "status_explanations", b"status_explanations"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "annotations", b"annotations", "desired_state", b"desired_state", "id", b"id", "last_applied_timestamp", b"last_applied_timestamp", "last_fetched_timestamp", b"last_fetched_timestamp", "last_seen_state", b"last_seen_state", "last_update_timestamp", b"last_update_timestamp", "starting_state", b"starting_state", "target_state", b"target_state"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "annotations", b"annotations", "dependencies", b"dependencies", "desired_state", b"desired_state", "desired_state_id", b"desired_state_id", "id", b"id", "last_applied_timestamp", b"last_applied_timestamp", "last_fetched_timestamp", b"last_fetched_timestamp", "last_seen_state", b"last_seen_state", "last_update_timestamp", b"last_update_timestamp", "lifecycle", b"lifecycle", "logs", b"logs", "precondition_statuses", b"precondition_statuses", "root_desired_state_id", b"root_desired_state_id", "simple_status", b"simple_status", "starting_state", b"starting_state", "status", b"status", "status_explanations", b"status_explanations", "target_state", b"target_state"]) -> None: ...
 
 global___Entity = Entity
 
 class EntityGraph(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ROOT_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/environment/clusters_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/environment/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/environment/clusters_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/environment/clusters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/events/events_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/events/events_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/events/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/events/types_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/events/types_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/events/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/insights/insights_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/insights/insights_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/insights/insights_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/insights/insights_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/metrics/metrics_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/metrics/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/metrics/metrics_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/metrics/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/object/meta_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/object/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/object/meta_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/object/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/organization/user_metadata_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/organization/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/pipelines/object_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/pipelines/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/pipelines/object_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/pipelines/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/pipelines/pipelines_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/pipelines/pipelines_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/protection/attachments_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/protection/attachments_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/protection/attachments_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/protection/attachments_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/protection/object_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/protection/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/protection/object_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/protection/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_config_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_config_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_reference_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_reference_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/object_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/object_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/repo/repo_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/repo/repo_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/repo/repo_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/repo/repo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/runtimes/features_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/runtimes/features_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/runtimes/features_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/runtimes/features_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/scm/types_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/scm/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/scm/types_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/scm/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/service/object_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/service/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/service/object_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/service/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/service/parameters_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/service/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/service/parameters_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/service/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/service/service_config_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/service/service_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/service/service_config_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/service/service_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/service/user_metadata_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/service/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/service/user_metadata_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/service/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/stat/efficiency_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/stat/efficiency_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/stat/efficiency_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/stat/efficiency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/users/users_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/users/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/users/users_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/users/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/version/source_metadata_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/version/source_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/version/source_metadata_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/version/source_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/volumes/volumes_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/volumes/volumes_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/volumes/volumes_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/volumes/volumes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/workflow/integration_config_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/workflow/integration_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py` & `prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py` & `prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi` & `prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/validate/validate_pb2.py` & `prodvana-0.2.1/prodvana/proto/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/proto/validate/validate_pb2.pyi` & `prodvana-0.2.1/prodvana/proto/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/utils/desired_states.py` & `prodvana-0.2.1/prodvana/utils/desired_states.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/utils/parameters.py` & `prodvana-0.2.1/prodvana/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/utils/protections.py` & `prodvana-0.2.1/prodvana/utils/protections.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/utils/service_config.py` & `prodvana-0.2.1/prodvana/utils/service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/prodvana/utils/tests/test_service_config.py` & `prodvana-0.2.1/prodvana/utils/tests/test_service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.0/pyproject.toml` & `prodvana-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodvana"
-version = "0.2.0"
+version = "0.2.1"
 description = "Prodvana's client libraries"
 readme = "README.md"
 authors = []
 homepage = "https://prodvana.io"
 documentation = "https://docs.prodvana.io"
 repository = "https://github.com/prodvana/prodvana-public"
 exclude = ["examples"]
```

### Comparing `prodvana-0.2.0/PKG-INFO` & `prodvana-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodvana
-Version: 0.2.0
+Version: 0.2.1
 Summary: Prodvana's client libraries
 Home-page: https://prodvana.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-api-python-client (>=2.58.0,<3.0)
```

