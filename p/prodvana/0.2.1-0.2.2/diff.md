# Comparing `tmp/prodvana-0.2.1.tar.gz` & `tmp/prodvana-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodvana-0.2.1.tar", max compression
+gzip compressed data, was "prodvana-0.2.2.tar", max compression
```

## Comparing `prodvana-0.2.1.tar` & `prodvana-0.2.2.tar`

### file list

```diff
@@ -1,329 +1,329 @@
--rw-r--r--   0        0        0       81 2023-07-07 23:25:26.643463 prodvana-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-07-07 23:25:26.643463 prodvana-0.2.1/prodvana/__init__.py
--rw-r--r--   0        0        0     3529 2023-07-07 23:25:26.643463 prodvana-0.2.1/prodvana/client.py
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.788471 prodvana-0.2.1/prodvana/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.788471 prodvana-0.2.1/prodvana/proto/prodvana/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/agent/__init__.py
--rw-r--r--   0        0        0     9562 2023-07-26 18:43:18.520471 prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
--rw-r--r--   0        0        0    19141 2023-07-26 18:43:18.664471 prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
--rw-r--r--   0        0        0    22573 2023-07-26 18:43:18.520471 prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
--rw-r--r--   0        0        0     6760 2023-07-26 18:43:18.660471 prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.808471 prodvana-0.2.1/prodvana/proto/prodvana/application/__init__.py
--rw-r--r--   0        0        0     3521 2023-07-26 18:43:18.624471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_config_pb2.py
--rw-r--r--   0        0        0     3485 2023-07-26 18:43:18.768471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.628471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.768471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    15907 2023-07-26 18:43:18.624471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2.py
--rw-r--r--   0        0        0    16830 2023-07-26 18:43:18.764471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2.pyi
--rw-r--r--   0        0        0    22241 2023-07-26 18:43:18.632471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6755 2023-07-26 18:43:18.764471 prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2235 2023-07-26 18:43:18.628471 prodvana-0.2.1/prodvana/proto/prodvana/application/object_pb2.py
--rw-r--r--   0        0        0     2184 2023-07-26 18:43:18.768471 prodvana-0.2.1/prodvana/proto/prodvana/application/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.628471 prodvana-0.2.1/prodvana/proto/prodvana/application/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.764471 prodvana-0.2.1/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2011 2023-07-26 18:43:18.628471 prodvana-0.2.1/prodvana/proto/prodvana/application/user_metadata_pb2.py
--rw-r--r--   0        0        0     1670 2023-07-26 18:43:18.768471 prodvana-0.2.1/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.628471 prodvana-0.2.1/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.768471 prodvana-0.2.1/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/auth/__init__.py
--rw-r--r--   0        0        0     8480 2023-07-26 18:43:18.608471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2.py
--rw-r--r--   0        0        0    10206 2023-07-26 18:43:18.748471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
--rw-r--r--   0        0        0    18631 2023-07-26 18:43:18.608471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6767 2023-07-26 18:43:18.748471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3181 2023-07-26 18:43:18.608471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_pb2.py
--rw-r--r--   0        0        0     5515 2023-07-26 18:43:18.748471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.608471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.744471 prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/blobs/__init__.py
--rw-r--r--   0        0        0     2285 2023-07-26 18:43:18.548471 prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
--rw-r--r--   0        0        0     1129 2023-07-26 18:43:18.688471 prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
--rw-r--r--   0        0        0     2704 2023-07-26 18:43:18.548471 prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
--rw-r--r--   0        0        0      895 2023-07-26 18:43:18.688471 prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.792471 prodvana-0.2.1/prodvana/proto/prodvana/capability/__init__.py
--rw-r--r--   0        0        0     4830 2023-07-26 18:43:18.516471 prodvana-0.2.1/prodvana/proto/prodvana/capability/capability_pb2.py
--rw-r--r--   0        0        0     5455 2023-07-26 18:43:18.656471 prodvana-0.2.1/prodvana/proto/prodvana/capability/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.516471 prodvana-0.2.1/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.656471 prodvana-0.2.1/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/__init__.py
--rw-r--r--   0        0        0     1988 2023-07-26 18:43:18.572471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/constants_pb2.py
--rw-r--r--   0        0        0     1667 2023-07-26 18:43:18.700471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/constants_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.556471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/constants_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.696471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/constants_pb2_grpc.pyi
--rw-r--r--   0        0        0     1366 2023-07-26 18:43:18.552471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
--rw-r--r--   0        0        0      869 2023-07-26 18:43:18.696471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.552471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.704471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
--rw-r--r--   0        0        0     2864 2023-07-26 18:43:18.556471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/env_pb2.py
--rw-r--r--   0        0        0     2933 2023-07-26 18:43:18.704471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/env_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.568471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.712471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
--rw-r--r--   0        0        0     4272 2023-07-26 18:43:18.552471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/helm_pb2.py
--rw-r--r--   0        0        0     5454 2023-07-26 18:43:18.708471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/helm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.560471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.700471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
--rw-r--r--   0        0        0     3013 2023-07-26 18:43:18.572471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
--rw-r--r--   0        0        0     4537 2023-07-26 18:43:18.708471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.560471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.692471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     1738 2023-07-26 18:43:18.564471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/links_pb2.py
--rw-r--r--   0        0        0      846 2023-07-26 18:43:18.704471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/links_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.552471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.712471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
--rw-r--r--   0        0        0     1338 2023-07-26 18:43:18.564471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/maturity_pb2.py
--rw-r--r--   0        0        0     1103 2023-07-26 18:43:18.692471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.572471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.700471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
--rw-r--r--   0        0        0     1838 2023-07-26 18:43:18.568471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/meta_pb2.py
--rw-r--r--   0        0        0     2531 2023-07-26 18:43:18.696471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.564471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.700471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0     1866 2023-07-26 18:43:18.560471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/notification_pb2.py
--rw-r--r--   0        0        0     1337 2023-07-26 18:43:18.696471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.548471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.692471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
--rw-r--r--   0        0        0     7815 2023-07-26 18:43:18.556471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/parameters_pb2.py
--rw-r--r--   0        0        0    10735 2023-07-26 18:43:18.696471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.568471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.712471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0     9143 2023-07-26 18:43:18.568471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/program_pb2.py
--rw-r--r--   0        0        0    15928 2023-07-26 18:43:18.708471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/program_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.564471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.692471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
--rw-r--r--   0        0        0     2686 2023-07-26 18:43:18.560471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/retry_pb2.py
--rw-r--r--   0        0        0     2757 2023-07-26 18:43:18.712471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/retry_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.556471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.708471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
--rw-r--r--   0        0        0     2804 2023-07-26 18:43:18.556471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/task_pb2.py
--rw-r--r--   0        0        0     3946 2023-07-26 18:43:18.704471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.572471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.688471 prodvana-0.2.1/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.792471 prodvana-0.2.1/prodvana/proto/prodvana/config_file/__init__.py
--rw-r--r--   0        0        0     3685 2023-07-26 18:43:18.516471 prodvana-0.2.1/prodvana/proto/prodvana/config_file/config_pb2.py
--rw-r--r--   0        0        0     4656 2023-07-26 18:43:18.660471 prodvana-0.2.1/prodvana/proto/prodvana/config_file/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.516471 prodvana-0.2.1/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.660471 prodvana-0.2.1/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/__init__.py
--rw-r--r--   0        0        0     1388 2023-07-26 18:43:18.604471 prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
--rw-r--r--   0        0        0     1131 2023-07-26 18:43:18.744471 prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.604471 prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.740471 prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.792471 prodvana-0.2.1/prodvana/proto/prodvana/delivery/__init__.py
--rw-r--r--   0        0        0     2079 2023-07-26 18:43:18.508471 prodvana-0.2.1/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
--rw-r--r--   0        0        0     2294 2023-07-26 18:43:18.652471 prodvana-0.2.1/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.508471 prodvana-0.2.1/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.648471 prodvana-0.2.1/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/__init__.py
--rw-r--r--   0        0        0     6161 2023-07-26 18:43:18.528471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/config_pb2.py
--rw-r--r--   0        0        0     8052 2023-07-26 18:43:18.668471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.532471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.672471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
--rw-r--r--   0        0        0     9291 2023-07-26 18:43:18.528471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
--rw-r--r--   0        0        0     8986 2023-07-26 18:43:18.672471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
--rw-r--r--   0        0        0    13097 2023-07-26 18:43:18.528471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3909 2023-07-26 18:43:18.672471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2015 2023-07-26 18:43:18.528471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/object_pb2.py
--rw-r--r--   0        0        0     1862 2023-07-26 18:43:18.668471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.532471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.668471 prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/__init__.py
--rw-r--r--   0        0        0    21535 2023-07-26 18:43:18.540471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2.py
--rw-r--r--   0        0        0    29180 2023-07-26 18:43:18.680471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
--rw-r--r--   0        0        0    20037 2023-07-26 18:43:18.536471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
--rw-r--r--   0        0        0     5752 2023-07-26 18:43:18.676471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/__init__.py
--rw-r--r--   0        0        0    27197 2023-07-26 18:43:18.532471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
--rw-r--r--   0        0        0    77697 2023-07-26 18:43:18.672471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.536471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.676471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
--rw-r--r--   0        0        0     3601 2023-07-26 22:01:30.060842 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
--rw-r--r--   0        0        0     8499 2023-07-26 22:01:30.060842 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.536471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.676471 prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.808471 prodvana-0.2.1/prodvana/proto/prodvana/environment/__init__.py
--rw-r--r--   0        0        0    16774 2023-07-26 18:43:18.632471 prodvana-0.2.1/prodvana/proto/prodvana/environment/clusters_pb2.py
--rw-r--r--   0        0        0    37710 2023-07-26 18:43:18.776471 prodvana-0.2.1/prodvana/proto/prodvana/environment/clusters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.636471 prodvana-0.2.1/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.772471 prodvana-0.2.1/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
--rw-r--r--   0        0        0    12870 2023-07-26 18:43:18.636471 prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2.py
--rw-r--r--   0        0        0    18334 2023-07-26 18:43:18.772471 prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
--rw-r--r--   0        0        0    21499 2023-07-26 18:43:18.632471 prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6311 2023-07-26 18:43:18.772471 prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.808471 prodvana-0.2.1/prodvana/proto/prodvana/events/__init__.py
--rw-r--r--   0        0        0     4801 2023-07-26 18:43:18.640471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2.py
--rw-r--r--   0        0        0     5547 2023-07-26 18:43:18.784471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2.pyi
--rw-r--r--   0        0        0     2714 2023-07-26 18:43:18.644471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
--rw-r--r--   0        0        0      853 2023-07-26 18:43:18.784471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2688 2023-07-26 18:43:18.640471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_pb2.py
--rw-r--r--   0        0        0     4131 2023-07-26 18:43:18.780471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.644471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.780471 prodvana-0.2.1/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
--rw-r--r--   0        0        0    10353 2023-07-26 18:43:18.644471 prodvana-0.2.1/prodvana/proto/prodvana/events/types_pb2.py
--rw-r--r--   0        0        0    30800 2023-07-26 18:43:18.784471 prodvana-0.2.1/prodvana/proto/prodvana/events/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.644471 prodvana-0.2.1/prodvana/proto/prodvana/events/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.780471 prodvana-0.2.1/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.808471 prodvana-0.2.1/prodvana/proto/prodvana/insights/__init__.py
--rw-r--r--   0        0        0     2205 2023-07-26 18:43:18.624471 prodvana-0.2.1/prodvana/proto/prodvana/insights/insights_pb2.py
--rw-r--r--   0        0        0     3508 2023-07-26 18:43:18.760471 prodvana-0.2.1/prodvana/proto/prodvana/insights/insights_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.620471 prodvana-0.2.1/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.764471 prodvana-0.2.1/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/__init__.py
--rw-r--r--   0        0        0     8344 2023-07-26 18:43:18.592471 prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2.py
--rw-r--r--   0        0        0    13338 2023-07-26 18:43:18.732471 prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
--rw-r--r--   0        0        0    12065 2023-07-26 18:43:18.592471 prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3657 2023-07-26 18:43:18.732471 prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/metrics/__init__.py
--rw-r--r--   0        0        0     3762 2023-07-26 18:43:18.524471 prodvana-0.2.1/prodvana/proto/prodvana/metrics/metrics_pb2.py
--rw-r--r--   0        0        0     8746 2023-07-26 18:43:18.668471 prodvana-0.2.1/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.524471 prodvana-0.2.1/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.668471 prodvana-0.2.1/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/object/__init__.py
--rw-r--r--   0        0        0     1657 2023-07-26 18:43:18.544471 prodvana-0.2.1/prodvana/proto/prodvana/object/meta_pb2.py
--rw-r--r--   0        0        0     1957 2023-07-26 18:43:18.684471 prodvana-0.2.1/prodvana/proto/prodvana/object/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.544471 prodvana-0.2.1/prodvana/proto/prodvana/object/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.684471 prodvana-0.2.1/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/organization/__init__.py
--rw-r--r--   0        0        0     9808 2023-07-26 18:43:18.544471 prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2.py
--rw-r--r--   0        0        0     9762 2023-07-26 18:43:18.684471 prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
--rw-r--r--   0        0        0    14668 2023-07-26 18:43:18.540471 prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4779 2023-07-26 18:43:18.680471 prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2568 2023-07-26 18:43:18.540471 prodvana-0.2.1/prodvana/proto/prodvana/organization/user_metadata_pb2.py
--rw-r--r--   0        0        0     1972 2023-07-26 18:43:18.680471 prodvana-0.2.1/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.540471 prodvana-0.2.1/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.684471 prodvana-0.2.1/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/__init__.py
--rw-r--r--   0        0        0     2038 2023-07-26 18:43:18.596471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/object_pb2.py
--rw-r--r--   0        0        0     2595 2023-07-26 18:43:18.736471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.596471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.732471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     6748 2023-07-26 18:43:18.596471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
--rw-r--r--   0        0        0    11698 2023-07-26 18:43:18.736471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.596471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.736471 prodvana-0.2.1/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.808471 prodvana-0.2.1/prodvana/proto/prodvana/protection/__init__.py
--rw-r--r--   0        0        0     2777 2023-07-26 18:43:18.620471 prodvana-0.2.1/prodvana/proto/prodvana/protection/attachments_pb2.py
--rw-r--r--   0        0        0     2860 2023-07-26 18:43:18.760471 prodvana-0.2.1/prodvana/proto/prodvana/protection/attachments_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.620471 prodvana-0.2.1/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.752471 prodvana-0.2.1/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
--rw-r--r--   0        0        0     1716 2023-07-26 18:43:18.616471 prodvana-0.2.1/prodvana/proto/prodvana/protection/object_pb2.py
--rw-r--r--   0        0        0     1545 2023-07-26 18:43:18.760471 prodvana-0.2.1/prodvana/proto/prodvana/protection/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.620471 prodvana-0.2.1/prodvana/proto/prodvana/protection/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.752471 prodvana-0.2.1/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     6615 2023-07-26 18:43:18.620471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_config_pb2.py
--rw-r--r--   0        0        0    10041 2023-07-26 18:43:18.760471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.616471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.756471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     8167 2023-07-26 18:43:18.616471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2.py
--rw-r--r--   0        0        0     8325 2023-07-26 18:43:18.752471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
--rw-r--r--   0        0        0    12468 2023-07-26 18:43:18.612471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
--rw-r--r--   0        0        0     3716 2023-07-26 18:43:18.756471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3938 2023-07-26 18:43:18.616471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_reference_pb2.py
--rw-r--r--   0        0        0     4997 2023-07-26 18:43:18.756471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.612471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.756471 prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/__init__.py
--rw-r--r--   0        0        0     2453 2023-07-26 18:43:18.588471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/object_pb2.py
--rw-r--r--   0        0        0     3325 2023-07-26 18:43:18.728471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.588471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.724471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     7193 2023-07-26 18:43:18.588471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
--rw-r--r--   0        0        0    12716 2023-07-26 18:43:18.728471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.584471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.728471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    10119 2023-07-26 18:43:18.584471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
--rw-r--r--   0        0        0    11055 2023-07-26 18:43:18.724471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
--rw-r--r--   0        0        0    15129 2023-07-26 18:43:18.588471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4757 2023-07-26 18:43:18.728471 prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/repo/__init__.py
--rw-r--r--   0        0        0     1701 2023-07-26 18:43:18.548471 prodvana-0.2.1/prodvana/proto/prodvana/repo/repo_pb2.py
--rw-r--r--   0        0        0     2315 2023-07-26 18:43:18.688471 prodvana-0.2.1/prodvana/proto/prodvana/repo/repo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.544471 prodvana-0.2.1/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.684471 prodvana-0.2.1/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/__init__.py
--rw-r--r--   0        0        0     1434 2023-07-26 18:43:18.600471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/features_pb2.py
--rw-r--r--   0        0        0     1320 2023-07-26 18:43:18.740471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/features_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.600471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.740471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
--rw-r--r--   0        0        0     4579 2023-07-26 18:43:18.600471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
--rw-r--r--   0        0        0     6995 2023-07-26 18:43:18.736471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.600471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.740471 prodvana-0.2.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.796471 prodvana-0.2.1/prodvana/proto/prodvana/scm/__init__.py
--rw-r--r--   0        0        0     1229 2023-07-26 18:43:18.524471 prodvana-0.2.1/prodvana/proto/prodvana/scm/types_pb2.py
--rw-r--r--   0        0        0      914 2023-07-26 18:43:18.664471 prodvana-0.2.1/prodvana/proto/prodvana/scm/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.524471 prodvana-0.2.1/prodvana/proto/prodvana/scm/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.664471 prodvana-0.2.1/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.792471 prodvana-0.2.1/prodvana/proto/prodvana/secrets/__init__.py
--rw-r--r--   0        0        0     6361 2023-07-26 18:43:18.520471 prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
--rw-r--r--   0        0        0     4586 2023-07-26 18:43:18.660471 prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
--rw-r--r--   0        0        0     9936 2023-07-26 18:43:18.520471 prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
--rw-r--r--   0        0        0     2847 2023-07-26 18:43:18.660471 prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/service/__init__.py
--rw-r--r--   0        0        0     4358 2023-07-26 18:43:18.576471 prodvana-0.2.1/prodvana/proto/prodvana/service/object_pb2.py
--rw-r--r--   0        0        0     7117 2023-07-26 18:43:18.720471 prodvana-0.2.1/prodvana/proto/prodvana/service/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.584471 prodvana-0.2.1/prodvana/proto/prodvana/service/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.712471 prodvana-0.2.1/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     1908 2023-07-26 18:43:18.576471 prodvana-0.2.1/prodvana/proto/prodvana/service/parameters_pb2.py
--rw-r--r--   0        0        0     2424 2023-07-26 18:43:18.716471 prodvana-0.2.1/prodvana/proto/prodvana/service/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.580471 prodvana-0.2.1/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.724471 prodvana-0.2.1/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    26309 2023-07-26 18:43:18.580471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_config_pb2.py
--rw-r--r--   0        0        0    54314 2023-07-26 18:43:18.716471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.584471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.724471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    31947 2023-07-26 18:43:18.580471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2.py
--rw-r--r--   0        0        0    38013 2023-07-26 18:43:18.720471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2.pyi
--rw-r--r--   0        0        0    33828 2023-07-26 18:43:18.580471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
--rw-r--r--   0        0        0     9674 2023-07-26 18:43:18.720471 prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2198 2023-07-26 18:43:18.576471 prodvana-0.2.1/prodvana/proto/prodvana/service/user_metadata_pb2.py
--rw-r--r--   0        0        0     2106 2023-07-26 18:43:18.716471 prodvana-0.2.1/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.576471 prodvana-0.2.1/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.720471 prodvana-0.2.1/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/settings/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/__init__.py
--rw-r--r--   0        0        0     5019 2023-07-26 18:43:18.604471 prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2.py
--rw-r--r--   0        0        0     5677 2023-07-26 18:43:18.744471 prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
--rw-r--r--   0        0        0     8214 2023-07-26 18:43:18.604471 prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
--rw-r--r--   0        0        0     2318 2023-07-26 18:43:18.744471 prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.792471 prodvana-0.2.1/prodvana/proto/prodvana/stat/__init__.py
--rw-r--r--   0        0        0     1317 2023-07-26 18:43:18.512471 prodvana-0.2.1/prodvana/proto/prodvana/stat/efficiency_pb2.py
--rw-r--r--   0        0        0     1156 2023-07-26 18:43:18.652471 prodvana-0.2.1/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.512471 prodvana-0.2.1/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.652471 prodvana-0.2.1/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.804471 prodvana-0.2.1/prodvana/proto/prodvana/users/__init__.py
--rw-r--r--   0        0        0     1361 2023-07-26 18:43:18.612471 prodvana-0.2.1/prodvana/proto/prodvana/users/users_pb2.py
--rw-r--r--   0        0        0     1451 2023-07-26 18:43:18.748471 prodvana-0.2.1/prodvana/proto/prodvana/users/users_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.612471 prodvana-0.2.1/prodvana/proto/prodvana/users/users_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.752471 prodvana-0.2.1/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.792471 prodvana-0.2.1/prodvana/proto/prodvana/version/__init__.py
--rw-r--r--   0        0        0     1723 2023-07-26 18:43:18.512471 prodvana-0.2.1/prodvana/proto/prodvana/version/source_metadata_pb2.py
--rw-r--r--   0        0        0     2817 2023-07-26 18:43:18.652471 prodvana-0.2.1/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.512471 prodvana-0.2.1/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.656471 prodvana-0.2.1/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.800471 prodvana-0.2.1/prodvana/proto/prodvana/volumes/__init__.py
--rw-r--r--   0        0        0     3089 2023-07-26 18:43:18.592471 prodvana-0.2.1/prodvana/proto/prodvana/volumes/volumes_pb2.py
--rw-r--r--   0        0        0     4793 2023-07-26 18:43:18.732471 prodvana-0.2.1/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.592471 prodvana-0.2.1/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.732471 prodvana-0.2.1/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.808471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/__init__.py
--rw-r--r--   0        0        0     3274 2023-07-26 18:43:18.636471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/integration_config_pb2.py
--rw-r--r--   0        0        0     4328 2023-07-26 18:43:18.776471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.640471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.780471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    36604 2023-07-26 18:43:18.636471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
--rw-r--r--   0        0        0    52034 2023-07-26 18:43:18.776471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
--rw-r--r--   0        0        0    57702 2023-07-26 18:43:18.640471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
--rw-r--r--   0        0        0    16676 2023-07-26 18:43:18.776471 prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-26 18:43:18.812471 prodvana-0.2.1/prodvana/proto/validate/__init__.py
--rw-r--r--   0        0        0    13684 2023-07-26 18:43:18.648471 prodvana-0.2.1/prodvana/proto/validate/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-07-26 18:43:18.784471 prodvana-0.2.1/prodvana/proto/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-07-26 18:43:18.648471 prodvana-0.2.1/prodvana/proto/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-07-26 18:43:18.788471 prodvana-0.2.1/prodvana/proto/validate/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-07-07 23:25:26.663462 prodvana-0.2.1/prodvana/py.typed
--rw-r--r--   0        0        0        0 2023-07-07 23:25:26.663462 prodvana-0.2.1/prodvana/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-07-07 23:25:26.663462 prodvana-0.2.1/prodvana/utils/desired_states.py
--rw-r--r--   0        0        0     1434 2023-07-20 20:38:16.234138 prodvana-0.2.1/prodvana/utils/parameters.py
--rw-r--r--   0        0        0     1731 2023-07-20 20:38:16.234138 prodvana-0.2.1/prodvana/utils/protections.py
--rw-r--r--   0        0        0     4079 2023-07-07 23:25:26.663462 prodvana-0.2.1/prodvana/utils/service_config.py
--rw-r--r--   0        0        0     7140 2023-07-07 23:25:26.663462 prodvana-0.2.1/prodvana/utils/tests/test_service_config.py
--rw-r--r--   0        0        0      746 2023-07-26 22:08:49.976855 prodvana-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       81 2023-05-30 15:25:51.905500 prodvana-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 15:25:51.913500 prodvana-0.2.2/prodvana/__init__.py
+-rw-r--r--   0        0        0     3529 2023-05-30 15:25:51.913500 prodvana-0.2.2/prodvana/client.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.311867 prodvana-0.2.2/prodvana/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.311867 prodvana-0.2.2/prodvana/proto/prodvana/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.315867 prodvana-0.2.2/prodvana/proto/prodvana/agent/__init__.py
+-rw-r--r--   0        0        0     9562 2023-07-12 14:36:38.985104 prodvana-0.2.2/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
+-rw-r--r--   0        0        0    19141 2023-07-12 14:36:38.985104 prodvana-0.2.2/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
+-rw-r--r--   0        0        0    22573 2023-07-09 22:25:55.035867 prodvana-0.2.2/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
+-rw-r--r--   0        0        0     6760 2023-07-09 22:25:55.175867 prodvana-0.2.2/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.327867 prodvana-0.2.2/prodvana/proto/prodvana/application/__init__.py
+-rw-r--r--   0        0        0     3521 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/application/application_config_pb2.py
+-rw-r--r--   0        0        0     3485 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/application/application_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.115867 prodvana-0.2.2/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.259867 prodvana-0.2.2/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15907 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/application/application_manager_pb2.py
+-rw-r--r--   0        0        0    16830 2023-07-09 22:25:55.259867 prodvana-0.2.2/prodvana/proto/prodvana/application/application_manager_pb2.pyi
+-rw-r--r--   0        0        0    22241 2023-07-09 22:25:55.115867 prodvana-0.2.2/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6755 2023-07-09 22:25:55.255867 prodvana-0.2.2/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2235 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/application/object_pb2.py
+-rw-r--r--   0        0        0     2184 2023-07-09 22:25:55.259867 prodvana-0.2.2/prodvana/proto/prodvana/application/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.119867 prodvana-0.2.2/prodvana/proto/prodvana/application/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.251867 prodvana-0.2.2/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2011 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/application/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1670 2023-07-09 22:25:55.255867 prodvana-0.2.2/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.119867 prodvana-0.2.2/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.255867 prodvana-0.2.2/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.331867 prodvana-0.2.2/prodvana/proto/prodvana/auth/__init__.py
+-rw-r--r--   0        0        0     8480 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_manager_pb2.py
+-rw-r--r--   0        0        0    10206 2023-07-09 22:25:55.299867 prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
+-rw-r--r--   0        0        0    18631 2023-07-09 22:25:55.159867 prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6767 2023-07-09 22:25:55.295867 prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3181 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_pb2.py
+-rw-r--r--   0        0        0     5515 2023-07-09 22:25:55.299867 prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.155867 prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.299867 prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.331867 prodvana-0.2.2/prodvana/proto/prodvana/blobs/__init__.py
+-rw-r--r--   0        0        0     2285 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
+-rw-r--r--   0        0        0     1129 2023-07-09 22:25:55.291867 prodvana-0.2.2/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
+-rw-r--r--   0        0        0     2704 2023-07-09 22:25:55.151867 prodvana-0.2.2/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      895 2023-07-09 22:25:55.295867 prodvana-0.2.2/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.323867 prodvana-0.2.2/prodvana/proto/prodvana/capability/__init__.py
+-rw-r--r--   0        0        0     4830 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/capability/capability_pb2.py
+-rw-r--r--   0        0        0     5455 2023-07-09 22:25:55.243867 prodvana-0.2.2/prodvana/proto/prodvana/capability/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.103867 prodvana-0.2.2/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.247867 prodvana-0.2.2/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.319867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/__init__.py
+-rw-r--r--   0        0        0     1988 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/common_config/constants_pb2.py
+-rw-r--r--   0        0        0     1667 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/common_config/constants_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/common_config/constants_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/common_config/constants_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1366 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
+-rw-r--r--   0        0        0      869 2023-07-09 22:25:55.211867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.055867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.215867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2864 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/common_config/env_pb2.py
+-rw-r--r--   0        0        0     2933 2023-07-09 22:25:55.195867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/env_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.063867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.207867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4272 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/common_config/helm_pb2.py
+-rw-r--r--   0        0        0     5454 2023-07-09 22:25:55.215867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/helm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.059867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.199867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3013 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
+-rw-r--r--   0        0        0     4537 2023-07-09 22:25:55.195867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.063867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.211867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1738 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/common_config/links_pb2.py
+-rw-r--r--   0        0        0      846 2023-07-09 22:25:55.195867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/links_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.071867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.199867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1338 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/common_config/maturity_pb2.py
+-rw-r--r--   0        0        0     1103 2023-07-09 22:25:55.215867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.055867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.203867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1838 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/common_config/meta_pb2.py
+-rw-r--r--   0        0        0     2531 2023-07-09 22:25:55.203867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.067867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.195867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1866 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/common_config/notification_pb2.py
+-rw-r--r--   0        0        0     1337 2023-07-09 22:25:55.199867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.071867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.211867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7815 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/common_config/parameters_pb2.py
+-rw-r--r--   0        0        0    10735 2023-07-09 22:25:55.207867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.059867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.203867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9143 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/common_config/program_pb2.py
+-rw-r--r--   0        0        0    15928 2023-07-09 22:25:55.199867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/program_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.067867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.191867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2686 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/common_config/retry_pb2.py
+-rw-r--r--   0        0        0     2757 2023-07-09 22:25:55.199867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/retry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.055867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.207867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2804 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/common_config/task_pb2.py
+-rw-r--r--   0        0        0     3946 2023-07-09 22:25:55.191867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.067867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.207867 prodvana-0.2.2/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.331867 prodvana-0.2.2/prodvana/proto/prodvana/config_file/__init__.py
+-rw-r--r--   0        0        0     3685 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/config_file/config_pb2.py
+-rw-r--r--   0        0        0     4656 2023-07-09 22:25:55.295867 prodvana-0.2.2/prodvana/proto/prodvana/config_file/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.155867 prodvana-0.2.2/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.295867 prodvana-0.2.2/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.319867 prodvana-0.2.2/prodvana/proto/prodvana/config_writeback/__init__.py
+-rw-r--r--   0        0        0     1388 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
+-rw-r--r--   0        0        0     1131 2023-07-09 22:25:55.223867 prodvana-0.2.2/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.083867 prodvana-0.2.2/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.223867 prodvana-0.2.2/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.315867 prodvana-0.2.2/prodvana/proto/prodvana/delivery/__init__.py
+-rw-r--r--   0        0        0     2079 2023-07-10 19:20:51.973585 prodvana-0.2.2/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
+-rw-r--r--   0        0        0     2294 2023-07-09 22:25:55.179867 prodvana-0.2.2/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.039867 prodvana-0.2.2/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.179867 prodvana-0.2.2/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.323867 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/__init__.py
+-rw-r--r--   0        0        0     6161 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/config_pb2.py
+-rw-r--r--   0        0        0     8052 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.087867 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.231867 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9291 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
+-rw-r--r--   0        0        0     8986 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
+-rw-r--r--   0        0        0    13097 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3909 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2015 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/object_pb2.py
+-rw-r--r--   0        0        0     1862 2023-07-09 22:25:55.231867 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.087867 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.227867 prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.319867 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/__init__.py
+-rw-r--r--   0        0        0    21535 2023-07-25 19:56:35.186371 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/manager_pb2.py
+-rw-r--r--   0        0        0    29180 2023-07-25 19:56:35.186371 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
+-rw-r--r--   0        0        0    20037 2023-07-25 19:56:35.186371 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5752 2023-07-25 19:56:35.186371 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.319867 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/__init__.py
+-rw-r--r--   0        0        0    27537 2023-07-27 15:24:23.619268 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
+-rw-r--r--   0        0        0    78899 2023-07-27 15:24:23.619268 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.079867 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.219867 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3601 2023-07-27 15:24:23.619268 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
+-rw-r--r--   0        0        0     8499 2023-07-27 15:24:23.619268 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.079867 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.219867 prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.315867 prodvana-0.2.2/prodvana/proto/prodvana/environment/__init__.py
+-rw-r--r--   0        0        0    16774 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/environment/clusters_pb2.py
+-rw-r--r--   0        0        0    37710 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/environment/clusters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.039867 prodvana-0.2.2/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.183867 prodvana-0.2.2/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12870 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/environment/environment_manager_pb2.py
+-rw-r--r--   0        0        0    18334 2023-07-09 22:25:55.183867 prodvana-0.2.2/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
+-rw-r--r--   0        0        0    21499 2023-07-09 22:25:55.043867 prodvana-0.2.2/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6311 2023-07-09 22:25:55.183867 prodvana-0.2.2/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.327867 prodvana-0.2.2/prodvana/proto/prodvana/events/__init__.py
+-rw-r--r--   0        0        0     4801 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/events/events_manager_pb2.py
+-rw-r--r--   0        0        0     5547 2023-07-09 22:25:55.267867 prodvana-0.2.2/prodvana/proto/prodvana/events/events_manager_pb2.pyi
+-rw-r--r--   0        0        0     2714 2023-07-09 22:25:55.127867 prodvana-0.2.2/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      853 2023-07-09 22:25:55.271867 prodvana-0.2.2/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2688 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/events/events_pb2.py
+-rw-r--r--   0        0        0     4131 2023-07-09 22:25:55.271867 prodvana-0.2.2/prodvana/proto/prodvana/events/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.131867 prodvana-0.2.2/prodvana/proto/prodvana/events/events_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.271867 prodvana-0.2.2/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10353 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/events/types_pb2.py
+-rw-r--r--   0        0        0    30800 2023-07-09 22:25:55.267867 prodvana-0.2.2/prodvana/proto/prodvana/events/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.127867 prodvana-0.2.2/prodvana/proto/prodvana/events/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.271867 prodvana-0.2.2/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.323867 prodvana-0.2.2/prodvana/proto/prodvana/insights/__init__.py
+-rw-r--r--   0        0        0     2205 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/insights/insights_pb2.py
+-rw-r--r--   0        0        0     3508 2023-07-09 22:25:55.247867 prodvana-0.2.2/prodvana/proto/prodvana/insights/insights_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.107867 prodvana-0.2.2/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.251867 prodvana-0.2.2/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.331867 prodvana-0.2.2/prodvana/proto/prodvana/managed_resource/__init__.py
+-rw-r--r--   0        0        0     8344 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/managed_resource/manager_pb2.py
+-rw-r--r--   0        0        0    13338 2023-07-09 22:25:55.303867 prodvana-0.2.2/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
+-rw-r--r--   0        0        0    12065 2023-07-09 22:25:55.159867 prodvana-0.2.2/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3657 2023-07-09 22:25:55.299867 prodvana-0.2.2/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.327867 prodvana-0.2.2/prodvana/proto/prodvana/metrics/__init__.py
+-rw-r--r--   0        0        0     3762 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/metrics/metrics_pb2.py
+-rw-r--r--   0        0        0     8746 2023-07-09 22:25:55.251867 prodvana-0.2.2/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.111867 prodvana-0.2.2/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.251867 prodvana-0.2.2/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.315867 prodvana-0.2.2/prodvana/proto/prodvana/object/__init__.py
+-rw-r--r--   0        0        0     1657 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/object/meta_pb2.py
+-rw-r--r--   0        0        0     1957 2023-07-09 22:25:55.187867 prodvana-0.2.2/prodvana/proto/prodvana/object/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.043867 prodvana-0.2.2/prodvana/proto/prodvana/object/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.187867 prodvana-0.2.2/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.331867 prodvana-0.2.2/prodvana/proto/prodvana/organization/__init__.py
+-rw-r--r--   0        0        0     9808 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/organization/organization_manager_pb2.py
+-rw-r--r--   0        0        0     9762 2023-07-09 22:25:55.291867 prodvana-0.2.2/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
+-rw-r--r--   0        0        0    14668 2023-07-09 22:25:55.151867 prodvana-0.2.2/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4779 2023-07-09 22:25:55.291867 prodvana-0.2.2/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2568 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/organization/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1972 2023-07-09 22:25:55.287867 prodvana-0.2.2/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.151867 prodvana-0.2.2/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.291867 prodvana-0.2.2/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.331867 prodvana-0.2.2/prodvana/proto/prodvana/pipelines/__init__.py
+-rw-r--r--   0        0        0     2038 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/pipelines/object_pb2.py
+-rw-r--r--   0        0        0     2595 2023-07-09 22:25:55.303867 prodvana-0.2.2/prodvana/proto/prodvana/pipelines/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.163867 prodvana-0.2.2/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.303867 prodvana-0.2.2/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6748 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
+-rw-r--r--   0        0        0    11698 2023-07-09 22:25:55.303867 prodvana-0.2.2/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.167867 prodvana-0.2.2/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.307867 prodvana-0.2.2/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.327867 prodvana-0.2.2/prodvana/proto/prodvana/protection/__init__.py
+-rw-r--r--   0        0        0     2777 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/protection/attachments_pb2.py
+-rw-r--r--   0        0        0     2860 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/protection/attachments_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.139867 prodvana-0.2.2/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.283867 prodvana-0.2.2/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1716 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/protection/object_pb2.py
+-rw-r--r--   0        0        0     1545 2023-07-09 22:25:55.279867 prodvana-0.2.2/prodvana/proto/prodvana/protection/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.139867 prodvana-0.2.2/prodvana/proto/prodvana/protection/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.275867 prodvana-0.2.2/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6615 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_config_pb2.py
+-rw-r--r--   0        0        0    10041 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.139867 prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.279867 prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8167 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_manager_pb2.py
+-rw-r--r--   0        0        0     8325 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
+-rw-r--r--   0        0        0    12468 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3716 2023-07-20 14:30:22.146988 prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3938 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_reference_pb2.py
+-rw-r--r--   0        0        0     4997 2023-07-09 22:25:55.279867 prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.135867 prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.275867 prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.327867 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/__init__.py
+-rw-r--r--   0        0        0     2453 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/object_pb2.py
+-rw-r--r--   0        0        0     3325 2023-07-09 22:25:55.283867 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.147867 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.283867 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7237 2023-07-27 15:24:23.619268 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
+-rw-r--r--   0        0        0    12880 2023-07-27 15:24:23.619268 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.143867 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.287867 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10119 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
+-rw-r--r--   0        0        0    11055 2023-07-09 22:25:55.283867 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
+-rw-r--r--   0        0        0    15129 2023-07-09 22:25:55.143867 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4757 2023-07-09 22:25:55.287867 prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.319867 prodvana-0.2.2/prodvana/proto/prodvana/repo/__init__.py
+-rw-r--r--   0        0        0     1701 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/repo/repo_pb2.py
+-rw-r--r--   0        0        0     2315 2023-07-09 22:25:55.227867 prodvana-0.2.2/prodvana/proto/prodvana/repo/repo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.083867 prodvana-0.2.2/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.223867 prodvana-0.2.2/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.327867 prodvana-0.2.2/prodvana/proto/prodvana/runtimes/__init__.py
+-rw-r--r--   0        0        0     1434 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/runtimes/features_pb2.py
+-rw-r--r--   0        0        0     1320 2023-07-09 22:25:55.259867 prodvana-0.2.2/prodvana/proto/prodvana/runtimes/features_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.119867 prodvana-0.2.2/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.263867 prodvana-0.2.2/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4579 2023-07-10 19:20:51.977585 prodvana-0.2.2/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
+-rw-r--r--   0        0        0     6995 2023-07-09 22:25:55.259867 prodvana-0.2.2/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.123867 prodvana-0.2.2/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.263867 prodvana-0.2.2/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.315867 prodvana-0.2.2/prodvana/proto/prodvana/scm/__init__.py
+-rw-r--r--   0        0        0     1229 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/prodvana/scm/types_pb2.py
+-rw-r--r--   0        0        0      914 2023-07-09 22:25:55.175867 prodvana-0.2.2/prodvana/proto/prodvana/scm/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.031867 prodvana-0.2.2/prodvana/proto/prodvana/scm/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.175867 prodvana-0.2.2/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.323867 prodvana-0.2.2/prodvana/proto/prodvana/secrets/__init__.py
+-rw-r--r--   0        0        0     6361 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
+-rw-r--r--   0        0        0     4586 2023-07-09 22:25:55.235867 prodvana-0.2.2/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
+-rw-r--r--   0        0        0     9936 2023-07-09 22:25:55.091867 prodvana-0.2.2/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     2847 2023-07-09 22:25:55.231867 prodvana-0.2.2/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.323867 prodvana-0.2.2/prodvana/proto/prodvana/service/__init__.py
+-rw-r--r--   0        0        0     4358 2023-07-20 14:30:22.150988 prodvana-0.2.2/prodvana/proto/prodvana/service/object_pb2.py
+-rw-r--r--   0        0        0     7117 2023-07-20 14:30:22.150988 prodvana-0.2.2/prodvana/proto/prodvana/service/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.099867 prodvana-0.2.2/prodvana/proto/prodvana/service/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.235867 prodvana-0.2.2/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1908 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/prodvana/service/parameters_pb2.py
+-rw-r--r--   0        0        0     2424 2023-07-09 22:25:55.239867 prodvana-0.2.2/prodvana/proto/prodvana/service/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.095867 prodvana-0.2.2/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.239867 prodvana-0.2.2/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    26420 2023-07-27 15:24:23.619268 prodvana-0.2.2/prodvana/proto/prodvana/service/service_config_pb2.py
+-rw-r--r--   0        0        0    54994 2023-07-27 15:24:23.619268 prodvana-0.2.2/prodvana/proto/prodvana/service/service_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.095867 prodvana-0.2.2/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.243867 prodvana-0.2.2/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    31947 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/prodvana/service/service_manager_pb2.py
+-rw-r--r--   0        0        0    38013 2023-07-09 22:25:55.235867 prodvana-0.2.2/prodvana/proto/prodvana/service/service_manager_pb2.pyi
+-rw-r--r--   0        0        0    33828 2023-07-09 22:25:55.099867 prodvana-0.2.2/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     9674 2023-07-09 22:25:55.239867 prodvana-0.2.2/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2198 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/prodvana/service/user_metadata_pb2.py
+-rw-r--r--   0        0        0     2106 2023-07-09 22:25:55.235867 prodvana-0.2.2/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.103867 prodvana-0.2.2/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.239867 prodvana-0.2.2/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.323867 prodvana-0.2.2/prodvana/proto/prodvana/settings/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.323867 prodvana-0.2.2/prodvana/proto/prodvana/settings/organization/__init__.py
+-rw-r--r--   0        0        0     5019 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/prodvana/settings/organization/users_pb2.py
+-rw-r--r--   0        0        0     5677 2023-07-09 22:25:55.247867 prodvana-0.2.2/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
+-rw-r--r--   0        0        0     8214 2023-07-09 22:25:55.107867 prodvana-0.2.2/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
+-rw-r--r--   0        0        0     2318 2023-07-09 22:25:55.247867 prodvana-0.2.2/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.311867 prodvana-0.2.2/prodvana/proto/prodvana/stat/__init__.py
+-rw-r--r--   0        0        0     1317 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/prodvana/stat/efficiency_pb2.py
+-rw-r--r--   0        0        0     1156 2023-07-09 22:25:55.171867 prodvana-0.2.2/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.031867 prodvana-0.2.2/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.171867 prodvana-0.2.2/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.331867 prodvana-0.2.2/prodvana/proto/prodvana/users/__init__.py
+-rw-r--r--   0        0        0     1361 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/prodvana/users/users_pb2.py
+-rw-r--r--   0        0        0     1451 2023-07-09 22:25:55.307867 prodvana-0.2.2/prodvana/proto/prodvana/users/users_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.167867 prodvana-0.2.2/prodvana/proto/prodvana/users/users_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.307867 prodvana-0.2.2/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.319867 prodvana-0.2.2/prodvana/proto/prodvana/version/__init__.py
+-rw-r--r--   0        0        0     1723 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/prodvana/version/source_metadata_pb2.py
+-rw-r--r--   0        0        0     2817 2023-07-09 22:25:55.187867 prodvana-0.2.2/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.047867 prodvana-0.2.2/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.187867 prodvana-0.2.2/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.319867 prodvana-0.2.2/prodvana/proto/prodvana/volumes/__init__.py
+-rw-r--r--   0        0        0     3089 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/prodvana/volumes/volumes_pb2.py
+-rw-r--r--   0        0        0     4793 2023-07-09 22:25:55.191867 prodvana-0.2.2/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.051867 prodvana-0.2.2/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.191867 prodvana-0.2.2/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.327867 prodvana-0.2.2/prodvana/proto/prodvana/workflow/__init__.py
+-rw-r--r--   0        0        0     3274 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/prodvana/workflow/integration_config_pb2.py
+-rw-r--r--   0        0        0     4328 2023-07-09 22:25:55.263867 prodvana-0.2.2/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.123867 prodvana-0.2.2/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.263867 prodvana-0.2.2/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    36604 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
+-rw-r--r--   0        0        0    52034 2023-07-09 22:25:55.267867 prodvana-0.2.2/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
+-rw-r--r--   0        0        0    57702 2023-07-09 22:25:55.123867 prodvana-0.2.2/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
+-rw-r--r--   0        0        0    16676 2023-07-09 22:25:55.267867 prodvana-0.2.2/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-07-09 22:25:55.335867 prodvana-0.2.2/prodvana/proto/validate/__init__.py
+-rw-r--r--   0        0        0    13684 2023-07-10 19:20:51.981585 prodvana-0.2.2/prodvana/proto/validate/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-07-09 22:25:55.307867 prodvana-0.2.2/prodvana/proto/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-07-09 22:25:55.167867 prodvana-0.2.2/prodvana/proto/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-07-09 22:25:55.311867 prodvana-0.2.2/prodvana/proto/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-30 15:25:51.913500 prodvana-0.2.2/prodvana/py.typed
+-rw-r--r--   0        0        0        0 2023-05-30 15:25:51.913500 prodvana-0.2.2/prodvana/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-05-30 15:25:51.913500 prodvana-0.2.2/prodvana/utils/desired_states.py
+-rw-r--r--   0        0        0     1434 2023-07-20 22:00:45.520554 prodvana-0.2.2/prodvana/utils/parameters.py
+-rw-r--r--   0        0        0     1731 2023-07-20 22:00:45.520554 prodvana-0.2.2/prodvana/utils/protections.py
+-rw-r--r--   0        0        0     4079 2023-05-30 15:25:51.913500 prodvana-0.2.2/prodvana/utils/service_config.py
+-rw-r--r--   0        0        0     7140 2023-05-30 15:25:51.913500 prodvana-0.2.2/prodvana/utils/tests/test_service_config.py
+-rw-r--r--   0        0        0      746 2023-07-27 15:28:25.559280 prodvana-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.2.2/PKG-INFO
```

### Comparing `prodvana-0.2.1/prodvana/client.py` & `prodvana-0.2.2/prodvana/client.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/agent/agent_interaction_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/application/application_config_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/application/application_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/application/application_config_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/application/application_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/application/application_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/application/application_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/application/object_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/application/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/application/object_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/application/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/application/user_metadata_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/application/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/application/user_metadata_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/application/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/auth/auth_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/auth/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/capability/capability_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/capability/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/capability/capability_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/capability/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/constants_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/constants_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/constants_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/constants_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/env_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/env_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/env_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/env_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/helm_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/helm_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/helm_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/helm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/links_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/links_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/links_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/maturity_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/maturity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/maturity_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/maturity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/meta_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/meta_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/notification_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/notification_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/parameters_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/parameters_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/program_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/program_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/program_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/program_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/retry_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/retry_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/retry_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/retry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/task_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/task_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/common_config/task_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/common_config/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/config_file/config_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/config_file/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/config_file/config_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/config_file/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/writeback_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/config_writeback/writeback_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/delivery/delivery_config_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/delivery/delivery_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/config_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/object_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/desired_state/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/desired_state/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from prodvana.proto.prodvana.common_config import program_pb2 as prodvana_dot_common__config_dot_program__pb2
 from prodvana.proto.prodvana.common_config import retry_pb2 as prodvana_dot_common__config_dot_retry__pb2
 from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
 from prodvana.proto.prodvana.environment import clusters_pb2 as prodvana_dot_environment_dot_clusters__pb2
 from prodvana.proto.prodvana.protection import protection_reference_pb2 as prodvana_dot_protection_dot_protection__reference__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0prodvana/desired_state/model/desired_state.proto\x12\x1cprodvana.desired_state.model\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a!prodvana/common_config/task.proto\x1a#prodvana/environment/clusters.proto\x1a.prodvana/protection/protection_reference.proto\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xa8\x06\n\tCondition\x12X\n\x07rc_cond\x18\x01 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.ReleaseChannelStableConditionH\x00\x12Q\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x36.prodvana.desired_state.model.Condition.ManualApprovalH\x00\x12\\\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.CustomTaskSuccessfulConditionH\x00\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x1a\xa7\x01\n\x1dReleaseChannelStableCondition\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x0f\n\x07service\x18\x02 \x01(\t\x12\x12\n\nservice_id\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x05 \x01(\t\x12\x17\n\x0fservice_version\x18\x06 \x01(\t\x1a\x34\n\x0eManualApproval\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x1a\x88\x02\n\x1d\x43ustomTaskSuccessfulCondition\x12\x18\n\x10\x63ustom_task_name\x18\x01 \x01(\t\x12\x66\n\nprotection\x18\x02 \x01(\x0b\x32P.prodvana.desired_state.model.Condition.CustomTaskSuccessfulCondition.ProtectionH\x00\x1a[\n\nProtection\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\ttask_type\x18\x03 \x01(\x0e\x32,.prodvana.desired_state.model.CustomTaskTypeB\x08\n\x06sourceB\x0b\n\tcondition\"\xa0\x01\n\x11\x44\x65liveryExtension\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\x12\x38\n\tlifecycle\x18\x02 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\x12<\n\nreferences\x18\x03 \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\"L\n\nIdentifier\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".prodvana.desired_state.model.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xc5\x03\n\x08Metadata\x12>\n\rpreconditions\x18\x01 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12;\n\ninvariants\x18\x02 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12\x36\n\x04self\x18\x03 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x46\n\x10protection_links\x18\x06 \x03(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12L\n\x13\x64\x65livery_extensions\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.DeliveryExtension\x12\"\n\x1atarget_state_set_by_parent\x18\t \x01(\x08J\x04\x08\x07\x10\x08R\x0bprotections\"\xad\x01\n\x11StatusExplanation\x12\x39\n\x07subject\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\x06reason\x18\x02 \x01(\x0e\x32*.prodvana.desired_state.model.StatusReason\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x10\n\x08messages\x18\x04 \x03(\t\"\x8b\x01\n\x11\x41\x63tionExplanation\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x0b\x61\x63tion_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.ActionType\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xde\x01\n\x07Version\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08replicas\x18\x02 \x01(\x05\x12\x1a\n\x12\x61vailable_replicas\x18\x08 \x01(\x05\x12\x32\n\x0epush_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12\x17\n\x0ftarget_replicas\x18\x06 \x01(\x05\x12\r\n\x05\x64irty\x18\t \x01(\x08J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08R\tunhealthyR\x11unhealthy_reasons\"\x86\x03\n\x14ServiceInstanceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x12\n\nservice_id\x18\x08 \x01(\t\x12\x1a\n\x12release_channel_id\x18\t \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12?\n\x10rollback_version\x18\x06 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12\x10\n\x08rollback\x18\x07 \x01(\x08\x12=\n\x08\x64\x65livery\x18\n \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\"\xf0\x02\n\x0cServiceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x12\n\nservice_id\x18\x05 \x01(\t\x12L\n\x10release_channels\x18\x06 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\x12\x43\n\x0c\x63ustom_tasks\x18\x07 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskState\x12Q\n\x13\x64\x65livery_extensions\x18\t \x03(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"\xa5\x02\n\x11ServiceGroupState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12<\n\x08services\x18\x02 \x03(\x0b\x32*.prodvana.desired_state.model.ServiceState\x12\x43\n\x0c\x63ustom_tasks\x18\x03 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskState\x12Q\n\x13\x64\x65livery_extensions\x18\x05 \x03(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateJ\x04\x08\x04\x10\x05\"\xa8\x02\n\x13\x43\x61naryProgressState\x12H\n\x06status\x18\x01 \x01(\x0e\x32\x38.prodvana.desired_state.model.CanaryProgressState.Status\x12 \n\rcanary_weight\x18\x02 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x15pause_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\r\n\tCOMPLETED\x10\x03\"\x94\x03\n\rDeliveryState\x12\x18\n\x10\x64\x65sired_state_id\x18\x0c \x01(\t\x12\x42\n\x06status\x18\x08 \x01(\x0e\x32\x32.prodvana.desired_state.model.DeliveryState.Status\x12\x0f\n\x07message\x18\x06 \x01(\t\x12J\n\x0f\x63\x61nary_progress\x18\x0b \x03(\x0b\x32\x31.prodvana.desired_state.model.CanaryProgressState\x12\x11\n\tfirst_run\x18\r \x01(\x08\x12\x12\n\ngeneration\x18\x0e \x01(\t\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_PROGRESSING\x10\x01\x12\x11\n\rSTATUS_PAUSED\x10\x02\x12\x12\n\x0eSTATUS_HEALTHY\x10\x03\x12\x14\n\x10STATUS_UNHEALTHY\x10\x04J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"=\n\x1bRuntimeExtensionFetchOutput\x12\r\n\x05\x64irty\x18\x01 \x01(\x08\x12\x0f\n\x07message\x18\x02 \x01(\t\"\xda\n\n\rRuntimeObject\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0bobject_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x42\n\x06status\x18\x06 \x01(\x0e\x32\x32.prodvana.desired_state.model.RuntimeObject.Status\x12?\n\x10rollback_version\x18\x07 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12=\n\x08\x64\x65livery\x18\x08 \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\x12\x18\n\x10version_agnostic\x18\n \x01(\x08\x12\"\n\x1a\x64\x65sired_version_dirty_only\x18\x14 \x01(\x08\x12\x0f\n\x07message\x18\x0c \x01(\t\x12W\n\x11runtime_extension\x18\r \x01(\x0b\x32<.prodvana.desired_state.model.RuntimeObject.RuntimeExtension\x12+\n\x08interval\x18\x0f \x01(\x0b\x32\x19.google.protobuf.Duration\x12*\n\x07timeout\x18\x10 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x17\n\x0foutput_blob_ids\x18\x12 \x03(\t\x12\x12\n\nexit_codes\x18\x13 \x03(\x05\x12%\n\x1drequire_approval_before_apply\x18\x15 \x01(\x08\x12G\n\x10missing_approval\x18\x16 \x01(\x0b\x32-.prodvana.desired_state.model.MissingApproval\x1a\xdb\x03\n\x10RuntimeExtension\x12=\n\x05\x61pply\x18\x03 \x01(\x0b\x32..prodvana.environment.CompiledExtensionCommand\x12=\n\x05\x66\x65tch\x18\x01 \x01(\x0b\x32..prodvana.environment.CompiledExtensionCommand\x12\x31\n\x0e\x66\x65tch_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x30\n\rfetch_timeout\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x12\n\nservice_id\x18\x02 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x06 \x01(\t\x12?\n\nparameters\x18\x07 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x08 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x31\n\x04type\x18\t \x01(\x0e\x32#.prodvana.environment.ExtensionType\"0\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\r\n\tSUCCEEDED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0e\x10\x0fJ\x04\x08\x11\x10\x12R\x0eunhealthy_podsR\nstate_hash\"O\n\x0e\x43onditionState\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xd6\x03\n\x0c\x43ontrolState\x12\x10\n\x08rollback\x18\x01 \x01(\x08\x12I\n\x13precondition_states\x18\x02 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x46\n\x10invariant_states\x18\x03 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x0e\n\x06paused\x18\x04 \x01(\x08\x12L\n\x13status_explanations\x18\x05 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12K\n\x12\x61\x63tion_explanation\x18\x06 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\x12:\n\x16last_fetched_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_applied_timestamp\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xb3\x01\n\x13ManualApprovalState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.prodvana.desired_state.model.ManualApprovalStatus\x12\r\n\x05topic\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\"\xc1\x05\n\x05State\x12=\n\x07service\x18\x01 \x01(\x0b\x32*.prodvana.desired_state.model.ServiceStateH\x00\x12N\n\x10service_instance\x18\x02 \x01(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceStateH\x00\x12H\n\rservice_group\x18\x03 \x01(\x0b\x32/.prodvana.desired_state.model.ServiceGroupStateH\x00\x12\x45\n\x0eruntime_object\x18\x04 \x01(\x0b\x32+.prodvana.desired_state.model.RuntimeObjectH\x00\x12L\n\x0fmanual_approval\x18\x05 \x01(\x0b\x32\x31.prodvana.desired_state.model.ManualApprovalStateH\x00\x12\x44\n\x0b\x63ustom_task\x18\x06 \x01(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateH\x00\x12S\n\x15protection_attachment\x18\x07 \x01(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachmentH\x00\x12L\n\x0fprotection_link\x18\x08 \x01(\x0b\x32\x31.prodvana.desired_state.model.ProtectionLinkStateH\x00\x12R\n\x12\x64\x65livery_extension\x18\t \x01(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateH\x00\x42\r\n\x0bstate_oneof\"\x82\x01\n\x0b\x41nnotations\x12I\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32\x34.prodvana.desired_state.model.Annotations.Annotation\x1a(\n\nAnnotation\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xae\x01\n\x18\x43ustomTaskExecutionState\x12>\n\x06status\x18\x01 \x01(\x0e\x32..prodvana.desired_state.model.CustomTaskStatus\x12\x10\n\x08\x61ttempts\x18\x02 \x01(\x03\x12@\n\x1clatest_attempt_end_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xce\x03\n\x0f\x43ustomTaskState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1c\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x04 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x05 \x01(\t\x12\x17\n\x0frelease_channel\x18\x06 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x07 \x01(\t\x12@\n\x07program\x18\t \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\ntask_state\x18\x0c \x01(\x0b\x32\x36.prodvana.desired_state.model.CustomTaskExecutionState\x12\x39\n\x0cretry_config\x18\r \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12\x13\n\x0bservice_ids\x18\x0e \x03(\tJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xeb\x04\n\x13ProtectionLinkState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12=\n\x06status\x18\x02 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\x12:\n\x04link\x18\x03 \x01(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12\x35\n\x11started_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11stopped_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0estopped_reason\x18\x06 \x01(\x0e\x32<.prodvana.desired_state.model.ProtectionLinkState.StopReason\x12;\n\x17\x66irst_success_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa1\x01\n\nStopReason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x17\n\x13LIFECYCLE_COMPLETED\x10\x01\x12\x12\n\x0eSUCCEEDED_ONCE\x10\x02\x12\x1a\n\x16SUCCEEDED_FOR_DURATION\x10\x03\x12\r\n\tTIMED_OUT\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x44\x45LETED\x10\x06\x12\x15\n\x11MANUALLY_BYPASSED\x10\x07\"\x89\x04\n\x14ProtectionAttachment\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x46\n\x17last_completed_versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12\x15\n\rprotection_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\x81\x05\n\x16\x44\x65liveryExtensionState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x14\n\x0c\x65xtension_id\x18\x03 \x01(\t\x12\x1d\n\x15\x65xtension_instance_id\x18\n \x01(\t\x12\x38\n\tlifecycle\x18\x0b \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12<\n\nreferences\x18\x0c \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\x12=\n\x06status\x18\r \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\x86\x04\n\x06Signal\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\x12Z\n\x12\x64\x65livery_promotion\x18\x02 \x01(\x0b\x32<.prodvana.desired_state.model.Signal.DeliveryPromotionConfigH\x00\x12R\n\x11protection_bypass\x18\x03 \x01(\x0b\x32\x35.prodvana.desired_state.model.Signal.ProtectionBypassH\x00\x12\x63\n\x1aruntime_extension_approval\x18\x04 \x01(\x0b\x32=.prodvana.desired_state.model.Signal.RuntimeExtensionApprovalH\x00\x1a\x36\n\x17\x44\x65liveryPromotionConfig\x12\r\n\x05stage\x18\x01 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x02 \x01(\x08\x1a\x12\n\x10ProtectionBypass\x1aY\n\x18RuntimeExtensionApproval\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06reject\x18\x02 \x01(\x08\x42\x08\n\x06\x63onfig\"?\n\x08\x44\x65\x62ugLog\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03log\x18\x02 \x01(\t\"j\n\x0fMissingApproval\x12\x18\n\x10\x64\x65sired_state_id\x18\x01 \x01(\t\x12=\n\x0bsignal_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType*\xcb\x01\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x14\n\x10SERVICE_INSTANCE\x10\x02\x12\x11\n\rSERVICE_GROUP\x10\x03\x12\x12\n\x0eRUNTIME_OBJECT\x10\x04\x12\x13\n\x0fMANUAL_APPROVAL\x10\x05\x12\x0f\n\x0b\x43USTOM_TASK\x10\x06\x12\x19\n\x15PROTECTION_ATTACHMENT\x10\x07\x12\x13\n\x0fPROTECTION_LINK\x10\x08\x12\x16\n\x12\x44\x45LIVERY_EXTENSION\x10\t*\x9a\x01\n\x0e\x43ustomTaskType\x12\x1c\n\x18\x43USTOM_TASK_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11PRE_APPROVAL_TASK\x10\x01\x12\x0c\n\x08\x41PPROVAL\x10\x02\x12\x16\n\x12POST_APPROVAL_TASK\x10\x03\x12\x13\n\x0f\x44\x45PLOYMENT_TASK\x10\x04\x12\x18\n\x14POST_DEPLOYMENT_TASK\x10\x05*\xf0\x01\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0e\n\nCONVERGING\x10\x01\x12\r\n\tCONVERGED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x10\n\x0cROLLING_BACK\x10\x04\x12\x0f\n\x0bROLLED_BACK\x10\x05\x12\x13\n\x0f\x46\x41ILED_ROLLBACK\x10\x0c\x12\n\n\x06PAUSED\x10\x06\x12\x10\n\x0c\x43HILD_PAUSED\x10\x07\x12\x19\n\x15WAITING_PRECONDITIONS\x10\x08\x12\x0c\n\x08REPLACED\x10\t\x12\x1b\n\x17WAITING_MANUAL_APPROVAL\x10\n\x12\x0b\n\x07\x44\x45LETED\x10\x0b*o\n\x0cSimpleStatus\x12\x0e\n\nSS_UNKNOWN\x10\x00\x12\x11\n\rSS_CONVERGING\x10\x01\x12\x10\n\x0cSS_CONVERGED\x10\x02\x12\r\n\tSS_FAILED\x10\x03\x12\x1b\n\x17SS_WAITING_FOR_APPROVAL\x10\x04*\xff\x01\n\x0cStatusReason\x12\x12\n\x0eREASON_UNKNOWN\x10\x00\x12\x14\n\x10NO_CURRENT_STATE\x10\x01\x12\x10\n\x0c\x41PPLY_FAILED\x10\x02\x12\x12\n\x0eUNHEALTHY_PODS\x10\x03\x12\x11\n\rUPDATING_PODS\x10\x04\x12\x14\n\x10VERSION_MISMATCH\x10\x05\x12\x19\n\x15RUNTIME_OBJECT_FAILED\x10\x06\x12\x18\n\x14PRECONDITIONS_FAILED\x10\x07\x12\x1c\n\x18MANUAL_APPROVAL_REJECTED\x10\x08\x12\x10\n\x0cSTUCK_ENTITY\x10\t\x12\x11\n\rVERSION_DIRTY\x10\n*r\n\nActionType\x12\x17\n\x13\x41\x43TION_TYPE_UNKNOWN\x10\x00\x12\x18\n\x14\x41\x43TION_TYPE_APPLYING\x10\x01\x12\x17\n\x13\x41\x43TION_TYPE_APPLIED\x10\x02\x12\x18\n\x14\x41\x43TION_TYPE_COMPLETE\x10\x03*\x96\x01\n\x0f\x43onditionStatus\x12\x1c\n\x18\x43ONDITION_UNKNOWN_STATUS\x10\x00\x12\x15\n\x11\x43ONDITION_PENDING\x10\x01\x12\x17\n\x13\x43ONDITION_SATISFIED\x10\x02\x12\x1f\n\x1b\x43ONDITION_MANUALLY_BYPASSED\x10\x03\x12\x14\n\x10\x43ONDITION_FAILED\x10\x04*?\n\x14ManualApprovalStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x41PPROVED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02*\x85\x01\n\x10\x43ustomTaskStatus\x12\x17\n\x13\x43USTOM_TASK_PENDING\x10\x00\x12\x1a\n\x16\x43USTOM_TASK_SUCCESSFUL\x10\x01\x12!\n\x1d\x43USTOM_TASK_RETRIES_EXHAUSTED\x10\x02\x12\x19\n\x15\x43USTOM_TASK_TIMED_OUT\x10\x03*\x8b\x01\n\nSignalType\x12\x12\n\x0eSIGNAL_UNKNOWN\x10\x00\x12\x16\n\x12\x44\x45LIVERY_PROMOTION\x10\x01\x12\x15\n\x11PROTECTION_BYPASS\x10\x02\x12\x1e\n\x1aRUNTIME_EXTENSION_APPROVAL\x10\x03\x12\x1a\n\x16SIGNAL_MANUAL_APPROVAL\x10\x04\x42XZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0prodvana/desired_state/model/desired_state.proto\x12\x1cprodvana.desired_state.model\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a!prodvana/common_config/task.proto\x1a#prodvana/environment/clusters.proto\x1a.prodvana/protection/protection_reference.proto\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xa8\x06\n\tCondition\x12X\n\x07rc_cond\x18\x01 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.ReleaseChannelStableConditionH\x00\x12Q\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x36.prodvana.desired_state.model.Condition.ManualApprovalH\x00\x12\\\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.CustomTaskSuccessfulConditionH\x00\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x1a\xa7\x01\n\x1dReleaseChannelStableCondition\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x0f\n\x07service\x18\x02 \x01(\t\x12\x12\n\nservice_id\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x05 \x01(\t\x12\x17\n\x0fservice_version\x18\x06 \x01(\t\x1a\x34\n\x0eManualApproval\x12\r\n\x05topic\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x1a\x88\x02\n\x1d\x43ustomTaskSuccessfulCondition\x12\x18\n\x10\x63ustom_task_name\x18\x01 \x01(\t\x12\x66\n\nprotection\x18\x02 \x01(\x0b\x32P.prodvana.desired_state.model.Condition.CustomTaskSuccessfulCondition.ProtectionH\x00\x1a[\n\nProtection\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\ttask_type\x18\x03 \x01(\x0e\x32,.prodvana.desired_state.model.CustomTaskTypeB\x08\n\x06sourceB\x0b\n\tcondition\"\xa0\x01\n\x11\x44\x65liveryExtension\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\x12\x38\n\tlifecycle\x18\x02 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\x12<\n\nreferences\x18\x03 \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\"L\n\nIdentifier\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".prodvana.desired_state.model.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xec\x03\n\x08Metadata\x12>\n\rpreconditions\x18\x01 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12;\n\ninvariants\x18\x02 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12\x36\n\x04self\x18\x03 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x46\n\x10protection_links\x18\x06 \x03(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12L\n\x13\x64\x65livery_extensions\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.DeliveryExtension\x12\"\n\x1atarget_state_set_by_parent\x18\t \x01(\x08\x12%\n\x1drequire_approval_before_apply\x18\n \x01(\x08J\x04\x08\x07\x10\x08R\x0bprotections\"\xad\x01\n\x11StatusExplanation\x12\x39\n\x07subject\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\x06reason\x18\x02 \x01(\x0e\x32*.prodvana.desired_state.model.StatusReason\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x10\n\x08messages\x18\x04 \x03(\t\"\x8b\x01\n\x11\x41\x63tionExplanation\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x0b\x61\x63tion_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.ActionType\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xde\x01\n\x07Version\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08replicas\x18\x02 \x01(\x05\x12\x1a\n\x12\x61vailable_replicas\x18\x08 \x01(\x05\x12\x32\n\x0epush_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12\x17\n\x0ftarget_replicas\x18\x06 \x01(\x05\x12\r\n\x05\x64irty\x18\t \x01(\x08J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08R\tunhealthyR\x11unhealthy_reasons\"\x86\x03\n\x14ServiceInstanceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x12\n\nservice_id\x18\x08 \x01(\t\x12\x1a\n\x12release_channel_id\x18\t \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12?\n\x10rollback_version\x18\x06 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12\x10\n\x08rollback\x18\x07 \x01(\x08\x12=\n\x08\x64\x65livery\x18\n \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\"\xf0\x02\n\x0cServiceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x12\n\nservice_id\x18\x05 \x01(\t\x12L\n\x10release_channels\x18\x06 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\x12\x43\n\x0c\x63ustom_tasks\x18\x07 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskState\x12Q\n\x13\x64\x65livery_extensions\x18\t \x03(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"\xa5\x02\n\x11ServiceGroupState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12<\n\x08services\x18\x02 \x03(\x0b\x32*.prodvana.desired_state.model.ServiceState\x12\x43\n\x0c\x63ustom_tasks\x18\x03 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskState\x12Q\n\x13\x64\x65livery_extensions\x18\x05 \x03(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateJ\x04\x08\x04\x10\x05\"\xa8\x02\n\x13\x43\x61naryProgressState\x12H\n\x06status\x18\x01 \x01(\x0e\x32\x38.prodvana.desired_state.model.CanaryProgressState.Status\x12 \n\rcanary_weight\x18\x02 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x15pause_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\r\n\tCOMPLETED\x10\x03\"\x94\x03\n\rDeliveryState\x12\x18\n\x10\x64\x65sired_state_id\x18\x0c \x01(\t\x12\x42\n\x06status\x18\x08 \x01(\x0e\x32\x32.prodvana.desired_state.model.DeliveryState.Status\x12\x0f\n\x07message\x18\x06 \x01(\t\x12J\n\x0f\x63\x61nary_progress\x18\x0b \x03(\x0b\x32\x31.prodvana.desired_state.model.CanaryProgressState\x12\x11\n\tfirst_run\x18\r \x01(\x08\x12\x12\n\ngeneration\x18\x0e \x01(\t\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_PROGRESSING\x10\x01\x12\x11\n\rSTATUS_PAUSED\x10\x02\x12\x12\n\x0eSTATUS_HEALTHY\x10\x03\x12\x14\n\x10STATUS_UNHEALTHY\x10\x04J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"=\n\x1bRuntimeExtensionFetchOutput\x12\r\n\x05\x64irty\x18\x01 \x01(\x08\x12\x0f\n\x07message\x18\x02 \x01(\t\"\xa9\n\n\rRuntimeObject\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0bobject_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x42\n\x06status\x18\x06 \x01(\x0e\x32\x32.prodvana.desired_state.model.RuntimeObject.Status\x12?\n\x10rollback_version\x18\x07 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12=\n\x08\x64\x65livery\x18\x08 \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\x12\x18\n\x10version_agnostic\x18\n \x01(\x08\x12\"\n\x1a\x64\x65sired_version_dirty_only\x18\x14 \x01(\x08\x12\x0f\n\x07message\x18\x0c \x01(\t\x12W\n\x11runtime_extension\x18\r \x01(\x0b\x32<.prodvana.desired_state.model.RuntimeObject.RuntimeExtension\x12+\n\x08interval\x18\x0f \x01(\x0b\x32\x19.google.protobuf.Duration\x12*\n\x07timeout\x18\x10 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x17\n\x0foutput_blob_ids\x18\x12 \x03(\t\x12\x12\n\nexit_codes\x18\x13 \x03(\x05\x12%\n\x1drequire_approval_before_apply\x18\x15 \x01(\x08\x1a\xdb\x03\n\x10RuntimeExtension\x12=\n\x05\x61pply\x18\x03 \x01(\x0b\x32..prodvana.environment.CompiledExtensionCommand\x12=\n\x05\x66\x65tch\x18\x01 \x01(\x0b\x32..prodvana.environment.CompiledExtensionCommand\x12\x31\n\x0e\x66\x65tch_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x30\n\rfetch_timeout\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x12\n\nservice_id\x18\x02 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x06 \x01(\t\x12?\n\nparameters\x18\x07 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x08 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x31\n\x04type\x18\t \x01(\x0e\x32#.prodvana.environment.ExtensionType\"0\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\r\n\tSUCCEEDED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0e\x10\x0fJ\x04\x08\x11\x10\x12J\x04\x08\x16\x10\x17R\x0eunhealthy_podsR\nstate_hashR\x10missing_approval\"O\n\x0e\x43onditionState\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\x9f\x04\n\x0c\x43ontrolState\x12\x10\n\x08rollback\x18\x01 \x01(\x08\x12I\n\x13precondition_states\x18\x02 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x46\n\x10invariant_states\x18\x03 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x0e\n\x06paused\x18\x04 \x01(\x08\x12L\n\x13status_explanations\x18\x05 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12K\n\x12\x61\x63tion_explanation\x18\x06 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\x12:\n\x16last_fetched_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_applied_timestamp\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12G\n\x10missing_approval\x18\t \x01(\x0b\x32-.prodvana.desired_state.model.MissingApproval\"\xb3\x01\n\x13ManualApprovalState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.prodvana.desired_state.model.ManualApprovalStatus\x12\r\n\x05topic\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\"\xc1\x05\n\x05State\x12=\n\x07service\x18\x01 \x01(\x0b\x32*.prodvana.desired_state.model.ServiceStateH\x00\x12N\n\x10service_instance\x18\x02 \x01(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceStateH\x00\x12H\n\rservice_group\x18\x03 \x01(\x0b\x32/.prodvana.desired_state.model.ServiceGroupStateH\x00\x12\x45\n\x0eruntime_object\x18\x04 \x01(\x0b\x32+.prodvana.desired_state.model.RuntimeObjectH\x00\x12L\n\x0fmanual_approval\x18\x05 \x01(\x0b\x32\x31.prodvana.desired_state.model.ManualApprovalStateH\x00\x12\x44\n\x0b\x63ustom_task\x18\x06 \x01(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateH\x00\x12S\n\x15protection_attachment\x18\x07 \x01(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachmentH\x00\x12L\n\x0fprotection_link\x18\x08 \x01(\x0b\x32\x31.prodvana.desired_state.model.ProtectionLinkStateH\x00\x12R\n\x12\x64\x65livery_extension\x18\t \x01(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateH\x00\x42\r\n\x0bstate_oneof\"\x82\x01\n\x0b\x41nnotations\x12I\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32\x34.prodvana.desired_state.model.Annotations.Annotation\x1a(\n\nAnnotation\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xae\x01\n\x18\x43ustomTaskExecutionState\x12>\n\x06status\x18\x01 \x01(\x0e\x32..prodvana.desired_state.model.CustomTaskStatus\x12\x10\n\x08\x61ttempts\x18\x02 \x01(\x03\x12@\n\x1clatest_attempt_end_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xce\x03\n\x0f\x43ustomTaskState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1c\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x04 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x05 \x01(\t\x12\x17\n\x0frelease_channel\x18\x06 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x07 \x01(\t\x12@\n\x07program\x18\t \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\ntask_state\x18\x0c \x01(\x0b\x32\x36.prodvana.desired_state.model.CustomTaskExecutionState\x12\x39\n\x0cretry_config\x18\r \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12\x13\n\x0bservice_ids\x18\x0e \x03(\tJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xeb\x04\n\x13ProtectionLinkState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12=\n\x06status\x18\x02 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\x12:\n\x04link\x18\x03 \x01(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12\x35\n\x11started_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11stopped_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0estopped_reason\x18\x06 \x01(\x0e\x32<.prodvana.desired_state.model.ProtectionLinkState.StopReason\x12;\n\x17\x66irst_success_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa1\x01\n\nStopReason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x17\n\x13LIFECYCLE_COMPLETED\x10\x01\x12\x12\n\x0eSUCCEEDED_ONCE\x10\x02\x12\x1a\n\x16SUCCEEDED_FOR_DURATION\x10\x03\x12\r\n\tTIMED_OUT\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x44\x45LETED\x10\x06\x12\x15\n\x11MANUALLY_BYPASSED\x10\x07\"\x89\x04\n\x14ProtectionAttachment\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x46\n\x17last_completed_versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12\x15\n\rprotection_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\x81\x05\n\x16\x44\x65liveryExtensionState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x14\n\x0c\x65xtension_id\x18\x03 \x01(\t\x12\x1d\n\x15\x65xtension_instance_id\x18\n \x01(\t\x12\x38\n\tlifecycle\x18\x0b \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12<\n\nreferences\x18\x0c \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\x12=\n\x06status\x18\r \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\x86\x04\n\x06Signal\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\x12Z\n\x12\x64\x65livery_promotion\x18\x02 \x01(\x0b\x32<.prodvana.desired_state.model.Signal.DeliveryPromotionConfigH\x00\x12R\n\x11protection_bypass\x18\x03 \x01(\x0b\x32\x35.prodvana.desired_state.model.Signal.ProtectionBypassH\x00\x12\x63\n\x1aruntime_extension_approval\x18\x04 \x01(\x0b\x32=.prodvana.desired_state.model.Signal.RuntimeExtensionApprovalH\x00\x1a\x36\n\x17\x44\x65liveryPromotionConfig\x12\r\n\x05stage\x18\x01 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x02 \x01(\x08\x1a\x12\n\x10ProtectionBypass\x1aY\n\x18RuntimeExtensionApproval\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06reject\x18\x02 \x01(\x08\x42\x08\n\x06\x63onfig\"?\n\x08\x44\x65\x62ugLog\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03log\x18\x02 \x01(\t\"j\n\x0fMissingApproval\x12\x18\n\x10\x64\x65sired_state_id\x18\x01 \x01(\t\x12=\n\x0bsignal_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\"d\n\rApplyRejected\x12I\n\x10missing_approval\x18\x01 \x01(\x0b\x32-.prodvana.desired_state.model.MissingApprovalH\x00\x42\x08\n\x06reason*\xcb\x01\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x14\n\x10SERVICE_INSTANCE\x10\x02\x12\x11\n\rSERVICE_GROUP\x10\x03\x12\x12\n\x0eRUNTIME_OBJECT\x10\x04\x12\x13\n\x0fMANUAL_APPROVAL\x10\x05\x12\x0f\n\x0b\x43USTOM_TASK\x10\x06\x12\x19\n\x15PROTECTION_ATTACHMENT\x10\x07\x12\x13\n\x0fPROTECTION_LINK\x10\x08\x12\x16\n\x12\x44\x45LIVERY_EXTENSION\x10\t*\x9a\x01\n\x0e\x43ustomTaskType\x12\x1c\n\x18\x43USTOM_TASK_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11PRE_APPROVAL_TASK\x10\x01\x12\x0c\n\x08\x41PPROVAL\x10\x02\x12\x16\n\x12POST_APPROVAL_TASK\x10\x03\x12\x13\n\x0f\x44\x45PLOYMENT_TASK\x10\x04\x12\x18\n\x14POST_DEPLOYMENT_TASK\x10\x05*\xf0\x01\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0e\n\nCONVERGING\x10\x01\x12\r\n\tCONVERGED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x10\n\x0cROLLING_BACK\x10\x04\x12\x0f\n\x0bROLLED_BACK\x10\x05\x12\x13\n\x0f\x46\x41ILED_ROLLBACK\x10\x0c\x12\n\n\x06PAUSED\x10\x06\x12\x10\n\x0c\x43HILD_PAUSED\x10\x07\x12\x19\n\x15WAITING_PRECONDITIONS\x10\x08\x12\x0c\n\x08REPLACED\x10\t\x12\x1b\n\x17WAITING_MANUAL_APPROVAL\x10\n\x12\x0b\n\x07\x44\x45LETED\x10\x0b*o\n\x0cSimpleStatus\x12\x0e\n\nSS_UNKNOWN\x10\x00\x12\x11\n\rSS_CONVERGING\x10\x01\x12\x10\n\x0cSS_CONVERGED\x10\x02\x12\r\n\tSS_FAILED\x10\x03\x12\x1b\n\x17SS_WAITING_FOR_APPROVAL\x10\x04*\xff\x01\n\x0cStatusReason\x12\x12\n\x0eREASON_UNKNOWN\x10\x00\x12\x14\n\x10NO_CURRENT_STATE\x10\x01\x12\x10\n\x0c\x41PPLY_FAILED\x10\x02\x12\x12\n\x0eUNHEALTHY_PODS\x10\x03\x12\x11\n\rUPDATING_PODS\x10\x04\x12\x14\n\x10VERSION_MISMATCH\x10\x05\x12\x19\n\x15RUNTIME_OBJECT_FAILED\x10\x06\x12\x18\n\x14PRECONDITIONS_FAILED\x10\x07\x12\x1c\n\x18MANUAL_APPROVAL_REJECTED\x10\x08\x12\x10\n\x0cSTUCK_ENTITY\x10\t\x12\x11\n\rVERSION_DIRTY\x10\n*r\n\nActionType\x12\x17\n\x13\x41\x43TION_TYPE_UNKNOWN\x10\x00\x12\x18\n\x14\x41\x43TION_TYPE_APPLYING\x10\x01\x12\x17\n\x13\x41\x43TION_TYPE_APPLIED\x10\x02\x12\x18\n\x14\x41\x43TION_TYPE_COMPLETE\x10\x03*\x96\x01\n\x0f\x43onditionStatus\x12\x1c\n\x18\x43ONDITION_UNKNOWN_STATUS\x10\x00\x12\x15\n\x11\x43ONDITION_PENDING\x10\x01\x12\x17\n\x13\x43ONDITION_SATISFIED\x10\x02\x12\x1f\n\x1b\x43ONDITION_MANUALLY_BYPASSED\x10\x03\x12\x14\n\x10\x43ONDITION_FAILED\x10\x04*?\n\x14ManualApprovalStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x41PPROVED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02*\x85\x01\n\x10\x43ustomTaskStatus\x12\x17\n\x13\x43USTOM_TASK_PENDING\x10\x00\x12\x1a\n\x16\x43USTOM_TASK_SUCCESSFUL\x10\x01\x12!\n\x1d\x43USTOM_TASK_RETRIES_EXHAUSTED\x10\x02\x12\x19\n\x15\x43USTOM_TASK_TIMED_OUT\x10\x03*\x8b\x01\n\nSignalType\x12\x12\n\x0eSIGNAL_UNKNOWN\x10\x00\x12\x16\n\x12\x44\x45LIVERY_PROMOTION\x10\x01\x12\x15\n\x11PROTECTION_BYPASS\x10\x02\x12\x1e\n\x1aRUNTIME_EXTENSION_APPROVAL\x10\x03\x12\x1a\n\x16SIGNAL_MANUAL_APPROVAL\x10\x04\x42XZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
 
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
-  _globals['_TYPE']._serialized_start=10478
-  _globals['_TYPE']._serialized_end=10681
-  _globals['_CUSTOMTASKTYPE']._serialized_start=10684
-  _globals['_CUSTOMTASKTYPE']._serialized_end=10838
-  _globals['_STATUS']._serialized_start=10841
-  _globals['_STATUS']._serialized_end=11081
-  _globals['_SIMPLESTATUS']._serialized_start=11083
-  _globals['_SIMPLESTATUS']._serialized_end=11194
-  _globals['_STATUSREASON']._serialized_start=11197
-  _globals['_STATUSREASON']._serialized_end=11452
-  _globals['_ACTIONTYPE']._serialized_start=11454
-  _globals['_ACTIONTYPE']._serialized_end=11568
-  _globals['_CONDITIONSTATUS']._serialized_start=11571
-  _globals['_CONDITIONSTATUS']._serialized_end=11721
-  _globals['_MANUALAPPROVALSTATUS']._serialized_start=11723
-  _globals['_MANUALAPPROVALSTATUS']._serialized_end=11786
-  _globals['_CUSTOMTASKSTATUS']._serialized_start=11789
-  _globals['_CUSTOMTASKSTATUS']._serialized_end=11922
-  _globals['_SIGNALTYPE']._serialized_start=11925
-  _globals['_SIGNALTYPE']._serialized_end=12064
+  _globals['_TYPE']._serialized_start=10643
+  _globals['_TYPE']._serialized_end=10846
+  _globals['_CUSTOMTASKTYPE']._serialized_start=10849
+  _globals['_CUSTOMTASKTYPE']._serialized_end=11003
+  _globals['_STATUS']._serialized_start=11006
+  _globals['_STATUS']._serialized_end=11246
+  _globals['_SIMPLESTATUS']._serialized_start=11248
+  _globals['_SIMPLESTATUS']._serialized_end=11359
+  _globals['_STATUSREASON']._serialized_start=11362
+  _globals['_STATUSREASON']._serialized_end=11617
+  _globals['_ACTIONTYPE']._serialized_start=11619
+  _globals['_ACTIONTYPE']._serialized_end=11733
+  _globals['_CONDITIONSTATUS']._serialized_start=11736
+  _globals['_CONDITIONSTATUS']._serialized_end=11886
+  _globals['_MANUALAPPROVALSTATUS']._serialized_start=11888
+  _globals['_MANUALAPPROVALSTATUS']._serialized_end=11951
+  _globals['_CUSTOMTASKSTATUS']._serialized_start=11954
+  _globals['_CUSTOMTASKSTATUS']._serialized_end=12087
+  _globals['_SIGNALTYPE']._serialized_start=12090
+  _globals['_SIGNALTYPE']._serialized_end=12229
   _globals['_PROTECTIONLINK']._serialized_start=407
   _globals['_PROTECTIONLINK']._serialized_end=519
   _globals['_CONDITION']._serialized_start=522
   _globals['_CONDITION']._serialized_end=1330
   _globals['_CONDITION_RELEASECHANNELSTABLECONDITION']._serialized_start=829
   _globals['_CONDITION_RELEASECHANNELSTABLECONDITION']._serialized_end=996
   _globals['_CONDITION_MANUALAPPROVAL']._serialized_start=998
@@ -72,73 +72,75 @@
   _globals['_CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION']._serialized_start=1216
   _globals['_CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION']._serialized_end=1307
   _globals['_DELIVERYEXTENSION']._serialized_start=1333
   _globals['_DELIVERYEXTENSION']._serialized_end=1493
   _globals['_IDENTIFIER']._serialized_start=1495
   _globals['_IDENTIFIER']._serialized_end=1571
   _globals['_METADATA']._serialized_start=1574
-  _globals['_METADATA']._serialized_end=2027
-  _globals['_STATUSEXPLANATION']._serialized_start=2030
-  _globals['_STATUSEXPLANATION']._serialized_end=2203
-  _globals['_ACTIONEXPLANATION']._serialized_start=2206
-  _globals['_ACTIONEXPLANATION']._serialized_end=2345
-  _globals['_VERSION']._serialized_start=2348
-  _globals['_VERSION']._serialized_end=2570
-  _globals['_SERVICEINSTANCESTATE']._serialized_start=2573
-  _globals['_SERVICEINSTANCESTATE']._serialized_end=2963
-  _globals['_SERVICESTATE']._serialized_start=2966
-  _globals['_SERVICESTATE']._serialized_end=3334
-  _globals['_SERVICEGROUPSTATE']._serialized_start=3337
-  _globals['_SERVICEGROUPSTATE']._serialized_end=3630
-  _globals['_CANARYPROGRESSSTATE']._serialized_start=3633
-  _globals['_CANARYPROGRESSSTATE']._serialized_end=3929
-  _globals['_CANARYPROGRESSSTATE_STATUS']._serialized_start=3868
-  _globals['_CANARYPROGRESSSTATE_STATUS']._serialized_end=3929
-  _globals['_DELIVERYSTATE']._serialized_start=3932
-  _globals['_DELIVERYSTATE']._serialized_end=4336
-  _globals['_DELIVERYSTATE_STATUS']._serialized_start=4175
-  _globals['_DELIVERYSTATE_STATUS']._serialized_end=4288
-  _globals['_RUNTIMEEXTENSIONFETCHOUTPUT']._serialized_start=4338
-  _globals['_RUNTIMEEXTENSIONFETCHOUTPUT']._serialized_end=4399
-  _globals['_RUNTIMEOBJECT']._serialized_start=4402
-  _globals['_RUNTIMEOBJECT']._serialized_end=5772
-  _globals['_RUNTIMEOBJECT_RUNTIMEEXTENSION']._serialized_start=5195
-  _globals['_RUNTIMEOBJECT_RUNTIMEEXTENSION']._serialized_end=5670
-  _globals['_RUNTIMEOBJECT_STATUS']._serialized_start=5672
-  _globals['_RUNTIMEOBJECT_STATUS']._serialized_end=5720
-  _globals['_CONDITIONSTATE']._serialized_start=5774
-  _globals['_CONDITIONSTATE']._serialized_end=5853
-  _globals['_CONTROLSTATE']._serialized_start=5856
-  _globals['_CONTROLSTATE']._serialized_end=6326
-  _globals['_MANUALAPPROVALSTATE']._serialized_start=6329
-  _globals['_MANUALAPPROVALSTATE']._serialized_end=6508
-  _globals['_STATE']._serialized_start=6511
-  _globals['_STATE']._serialized_end=7216
-  _globals['_ANNOTATIONS']._serialized_start=7219
-  _globals['_ANNOTATIONS']._serialized_end=7349
-  _globals['_ANNOTATIONS_ANNOTATION']._serialized_start=7309
-  _globals['_ANNOTATIONS_ANNOTATION']._serialized_end=7349
-  _globals['_CUSTOMTASKEXECUTIONSTATE']._serialized_start=7352
-  _globals['_CUSTOMTASKEXECUTIONSTATE']._serialized_end=7526
-  _globals['_CUSTOMTASKSTATE']._serialized_start=7529
-  _globals['_CUSTOMTASKSTATE']._serialized_end=7991
-  _globals['_PROTECTIONLINKSTATE']._serialized_start=7994
-  _globals['_PROTECTIONLINKSTATE']._serialized_end=8613
-  _globals['_PROTECTIONLINKSTATE_STOPREASON']._serialized_start=8452
-  _globals['_PROTECTIONLINKSTATE_STOPREASON']._serialized_end=8613
-  _globals['_PROTECTIONATTACHMENT']._serialized_start=8616
-  _globals['_PROTECTIONATTACHMENT']._serialized_end=9137
-  _globals['_DELIVERYEXTENSIONSTATE']._serialized_start=9140
-  _globals['_DELIVERYEXTENSIONSTATE']._serialized_end=9781
-  _globals['_SIGNAL']._serialized_start=9784
-  _globals['_SIGNAL']._serialized_end=10302
-  _globals['_SIGNAL_DELIVERYPROMOTIONCONFIG']._serialized_start=10127
-  _globals['_SIGNAL_DELIVERYPROMOTIONCONFIG']._serialized_end=10181
-  _globals['_SIGNAL_PROTECTIONBYPASS']._serialized_start=10183
-  _globals['_SIGNAL_PROTECTIONBYPASS']._serialized_end=10201
-  _globals['_SIGNAL_RUNTIMEEXTENSIONAPPROVAL']._serialized_start=10203
-  _globals['_SIGNAL_RUNTIMEEXTENSIONAPPROVAL']._serialized_end=10292
-  _globals['_DEBUGLOG']._serialized_start=10304
-  _globals['_DEBUGLOG']._serialized_end=10367
-  _globals['_MISSINGAPPROVAL']._serialized_start=10369
-  _globals['_MISSINGAPPROVAL']._serialized_end=10475
+  _globals['_METADATA']._serialized_end=2066
+  _globals['_STATUSEXPLANATION']._serialized_start=2069
+  _globals['_STATUSEXPLANATION']._serialized_end=2242
+  _globals['_ACTIONEXPLANATION']._serialized_start=2245
+  _globals['_ACTIONEXPLANATION']._serialized_end=2384
+  _globals['_VERSION']._serialized_start=2387
+  _globals['_VERSION']._serialized_end=2609
+  _globals['_SERVICEINSTANCESTATE']._serialized_start=2612
+  _globals['_SERVICEINSTANCESTATE']._serialized_end=3002
+  _globals['_SERVICESTATE']._serialized_start=3005
+  _globals['_SERVICESTATE']._serialized_end=3373
+  _globals['_SERVICEGROUPSTATE']._serialized_start=3376
+  _globals['_SERVICEGROUPSTATE']._serialized_end=3669
+  _globals['_CANARYPROGRESSSTATE']._serialized_start=3672
+  _globals['_CANARYPROGRESSSTATE']._serialized_end=3968
+  _globals['_CANARYPROGRESSSTATE_STATUS']._serialized_start=3907
+  _globals['_CANARYPROGRESSSTATE_STATUS']._serialized_end=3968
+  _globals['_DELIVERYSTATE']._serialized_start=3971
+  _globals['_DELIVERYSTATE']._serialized_end=4375
+  _globals['_DELIVERYSTATE_STATUS']._serialized_start=4214
+  _globals['_DELIVERYSTATE_STATUS']._serialized_end=4327
+  _globals['_RUNTIMEEXTENSIONFETCHOUTPUT']._serialized_start=4377
+  _globals['_RUNTIMEEXTENSIONFETCHOUTPUT']._serialized_end=4438
+  _globals['_RUNTIMEOBJECT']._serialized_start=4441
+  _globals['_RUNTIMEOBJECT']._serialized_end=5762
+  _globals['_RUNTIMEOBJECT_RUNTIMEEXTENSION']._serialized_start=5161
+  _globals['_RUNTIMEOBJECT_RUNTIMEEXTENSION']._serialized_end=5636
+  _globals['_RUNTIMEOBJECT_STATUS']._serialized_start=5638
+  _globals['_RUNTIMEOBJECT_STATUS']._serialized_end=5686
+  _globals['_CONDITIONSTATE']._serialized_start=5764
+  _globals['_CONDITIONSTATE']._serialized_end=5843
+  _globals['_CONTROLSTATE']._serialized_start=5846
+  _globals['_CONTROLSTATE']._serialized_end=6389
+  _globals['_MANUALAPPROVALSTATE']._serialized_start=6392
+  _globals['_MANUALAPPROVALSTATE']._serialized_end=6571
+  _globals['_STATE']._serialized_start=6574
+  _globals['_STATE']._serialized_end=7279
+  _globals['_ANNOTATIONS']._serialized_start=7282
+  _globals['_ANNOTATIONS']._serialized_end=7412
+  _globals['_ANNOTATIONS_ANNOTATION']._serialized_start=7372
+  _globals['_ANNOTATIONS_ANNOTATION']._serialized_end=7412
+  _globals['_CUSTOMTASKEXECUTIONSTATE']._serialized_start=7415
+  _globals['_CUSTOMTASKEXECUTIONSTATE']._serialized_end=7589
+  _globals['_CUSTOMTASKSTATE']._serialized_start=7592
+  _globals['_CUSTOMTASKSTATE']._serialized_end=8054
+  _globals['_PROTECTIONLINKSTATE']._serialized_start=8057
+  _globals['_PROTECTIONLINKSTATE']._serialized_end=8676
+  _globals['_PROTECTIONLINKSTATE_STOPREASON']._serialized_start=8515
+  _globals['_PROTECTIONLINKSTATE_STOPREASON']._serialized_end=8676
+  _globals['_PROTECTIONATTACHMENT']._serialized_start=8679
+  _globals['_PROTECTIONATTACHMENT']._serialized_end=9200
+  _globals['_DELIVERYEXTENSIONSTATE']._serialized_start=9203
+  _globals['_DELIVERYEXTENSIONSTATE']._serialized_end=9844
+  _globals['_SIGNAL']._serialized_start=9847
+  _globals['_SIGNAL']._serialized_end=10365
+  _globals['_SIGNAL_DELIVERYPROMOTIONCONFIG']._serialized_start=10190
+  _globals['_SIGNAL_DELIVERYPROMOTIONCONFIG']._serialized_end=10244
+  _globals['_SIGNAL_PROTECTIONBYPASS']._serialized_start=10246
+  _globals['_SIGNAL_PROTECTIONBYPASS']._serialized_end=10264
+  _globals['_SIGNAL_RUNTIMEEXTENSIONAPPROVAL']._serialized_start=10266
+  _globals['_SIGNAL_RUNTIMEEXTENSIONAPPROVAL']._serialized_end=10355
+  _globals['_DEBUGLOG']._serialized_start=10367
+  _globals['_DEBUGLOG']._serialized_end=10430
+  _globals['_MISSINGAPPROVAL']._serialized_start=10432
+  _globals['_MISSINGAPPROVAL']._serialized_end=10538
+  _globals['_APPLYREJECTED']._serialized_start=10540
+  _globals['_APPLYREJECTED']._serialized_end=10640
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -487,43 +487,46 @@
     INVARIANTS_FIELD_NUMBER: builtins.int
     SELF_FIELD_NUMBER: builtins.int
     DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
     ROOT_DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
     PROTECTION_LINKS_FIELD_NUMBER: builtins.int
     DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
     TARGET_STATE_SET_BY_PARENT_FIELD_NUMBER: builtins.int
+    REQUIRE_APPROVAL_BEFORE_APPLY_FIELD_NUMBER: builtins.int
     @property
     def preconditions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Condition]: ...
     @property
     def invariants(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Condition]: ...
     @property
     def self(self) -> global___Identifier: ...
     desired_state_id: builtins.str
     root_desired_state_id: builtins.str
     @property
     def protection_links(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ProtectionLink]: ...
     @property
     def delivery_extensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtension]: ...
     target_state_set_by_parent: builtins.bool
     """if true, the entity does not set its own target state. instead, the target state will be set when the parent decides to set target state."""
+    require_approval_before_apply: builtins.bool
     def __init__(
         # pyright: reportSelfClsParameterName=false
         self_,
         *,
         preconditions: collections.abc.Iterable[global___Condition] | None = ...,
         invariants: collections.abc.Iterable[global___Condition] | None = ...,
         self: global___Identifier | None = ...,
         desired_state_id: builtins.str = ...,
         root_desired_state_id: builtins.str = ...,
         protection_links: collections.abc.Iterable[global___ProtectionLink] | None = ...,
         delivery_extensions: collections.abc.Iterable[global___DeliveryExtension] | None = ...,
         target_state_set_by_parent: builtins.bool = ...,
+        require_approval_before_apply: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["self", b"self"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["delivery_extensions", b"delivery_extensions", "desired_state_id", b"desired_state_id", "invariants", b"invariants", "preconditions", b"preconditions", "protection_links", b"protection_links", "root_desired_state_id", b"root_desired_state_id", "self", b"self", "target_state_set_by_parent", b"target_state_set_by_parent"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery_extensions", b"delivery_extensions", "desired_state_id", b"desired_state_id", "invariants", b"invariants", "preconditions", b"preconditions", "protection_links", b"protection_links", "require_approval_before_apply", b"require_approval_before_apply", "root_desired_state_id", b"root_desired_state_id", "self", b"self", "target_state_set_by_parent", b"target_state_set_by_parent"]) -> None: ...
 
 global___Metadata = Metadata
 
 class StatusExplanation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUBJECT_FIELD_NUMBER: builtins.int
@@ -931,15 +934,14 @@
     MESSAGE_FIELD_NUMBER: builtins.int
     RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
     INTERVAL_FIELD_NUMBER: builtins.int
     TIMEOUT_FIELD_NUMBER: builtins.int
     OUTPUT_BLOB_IDS_FIELD_NUMBER: builtins.int
     EXIT_CODES_FIELD_NUMBER: builtins.int
     REQUIRE_APPROVAL_BEFORE_APPLY_FIELD_NUMBER: builtins.int
-    MISSING_APPROVAL_FIELD_NUMBER: builtins.int
     @property
     def meta(self) -> global___Metadata: ...
     object_type: builtins.str
     namespace: builtins.str
     name: builtins.str
     @property
     def versions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Version]: ...
@@ -968,16 +970,14 @@
         """output_blob_ids and exit_codes are in the same order, assuming output is saved
         if output is saved, this is the ID of the blob to retrieve it, only for run-to-completion objects.
         """
     @property
     def exit_codes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """exit codes, only for run-to-completion objects like jobs"""
     require_approval_before_apply: builtins.bool
-    @property
-    def missing_approval(self) -> global___MissingApproval: ...
     def __init__(
         self,
         *,
         meta: global___Metadata | None = ...,
         object_type: builtins.str = ...,
         namespace: builtins.str = ...,
         name: builtins.str = ...,
@@ -990,18 +990,17 @@
         message: builtins.str = ...,
         runtime_extension: global___RuntimeObject.RuntimeExtension | None = ...,
         interval: google.protobuf.duration_pb2.Duration | None = ...,
         timeout: google.protobuf.duration_pb2.Duration | None = ...,
         output_blob_ids: collections.abc.Iterable[builtins.str] | None = ...,
         exit_codes: collections.abc.Iterable[builtins.int] | None = ...,
         require_approval_before_apply: builtins.bool = ...,
-        missing_approval: global___MissingApproval | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "interval", b"interval", "meta", b"meta", "missing_approval", b"missing_approval", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "timeout", b"timeout"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "desired_version_dirty_only", b"desired_version_dirty_only", "exit_codes", b"exit_codes", "interval", b"interval", "message", b"message", "meta", b"meta", "missing_approval", b"missing_approval", "name", b"name", "namespace", b"namespace", "object_type", b"object_type", "output_blob_ids", b"output_blob_ids", "require_approval_before_apply", b"require_approval_before_apply", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "status", b"status", "timeout", b"timeout", "version_agnostic", b"version_agnostic", "versions", b"versions"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "interval", b"interval", "meta", b"meta", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "timeout", b"timeout"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery", b"delivery", "desired_version_dirty_only", b"desired_version_dirty_only", "exit_codes", b"exit_codes", "interval", b"interval", "message", b"message", "meta", b"meta", "name", b"name", "namespace", b"namespace", "object_type", b"object_type", "output_blob_ids", b"output_blob_ids", "require_approval_before_apply", b"require_approval_before_apply", "rollback_version", b"rollback_version", "runtime_extension", b"runtime_extension", "status", b"status", "timeout", b"timeout", "version_agnostic", b"version_agnostic", "versions", b"versions"]) -> None: ...
 
 global___RuntimeObject = RuntimeObject
 
 class ConditionState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STATUS_FIELD_NUMBER: builtins.int
@@ -1022,14 +1021,15 @@
     PRECONDITION_STATES_FIELD_NUMBER: builtins.int
     INVARIANT_STATES_FIELD_NUMBER: builtins.int
     PAUSED_FIELD_NUMBER: builtins.int
     STATUS_EXPLANATIONS_FIELD_NUMBER: builtins.int
     ACTION_EXPLANATION_FIELD_NUMBER: builtins.int
     LAST_FETCHED_TIMESTAMP_FIELD_NUMBER: builtins.int
     LAST_APPLIED_TIMESTAMP_FIELD_NUMBER: builtins.int
+    MISSING_APPROVAL_FIELD_NUMBER: builtins.int
     rollback: builtins.bool
     @property
     def precondition_states(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ConditionState]: ...
     @property
     def invariant_states(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ConditionState]: ...
     paused: builtins.bool
     """An entity is paused if itself or any of its ancestors have paused field set.
@@ -1043,28 +1043,31 @@
     @property
     def action_explanation(self) -> global___ActionExplanation:
         """What is DD doing now?"""
     @property
     def last_fetched_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     @property
     def last_applied_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    @property
+    def missing_approval(self) -> global___MissingApproval: ...
     def __init__(
         self,
         *,
         rollback: builtins.bool = ...,
         precondition_states: collections.abc.Iterable[global___ConditionState] | None = ...,
         invariant_states: collections.abc.Iterable[global___ConditionState] | None = ...,
         paused: builtins.bool = ...,
         status_explanations: collections.abc.Iterable[global___StatusExplanation] | None = ...,
         action_explanation: global___ActionExplanation | None = ...,
         last_fetched_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         last_applied_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        missing_approval: global___MissingApproval | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "last_applied_timestamp", b"last_applied_timestamp", "last_fetched_timestamp", b"last_fetched_timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "invariant_states", b"invariant_states", "last_applied_timestamp", b"last_applied_timestamp", "last_fetched_timestamp", b"last_fetched_timestamp", "paused", b"paused", "precondition_states", b"precondition_states", "rollback", b"rollback", "status_explanations", b"status_explanations"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "last_applied_timestamp", b"last_applied_timestamp", "last_fetched_timestamp", b"last_fetched_timestamp", "missing_approval", b"missing_approval"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "invariant_states", b"invariant_states", "last_applied_timestamp", b"last_applied_timestamp", "last_fetched_timestamp", b"last_fetched_timestamp", "missing_approval", b"missing_approval", "paused", b"paused", "precondition_states", b"precondition_states", "rollback", b"rollback", "status_explanations", b"status_explanations"]) -> None: ...
 
 global___ControlState = ControlState
 
 class ManualApprovalState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     META_FIELD_NUMBER: builtins.int
@@ -1512,7 +1515,27 @@
         *,
         desired_state_id: builtins.str = ...,
         signal_type: global___SignalType.ValueType = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["desired_state_id", b"desired_state_id", "signal_type", b"signal_type"]) -> None: ...
 
 global___MissingApproval = MissingApproval
+
+class ApplyRejected(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    MISSING_APPROVAL_FIELD_NUMBER: builtins.int
+    @property
+    def missing_approval(self) -> global___MissingApproval:
+        """Cannot apply because this entity requires additional approval.
+        TODO: Add reasons like paused entities.
+        """
+    def __init__(
+        self,
+        *,
+        missing_approval: global___MissingApproval | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["missing_approval", b"missing_approval", "reason", b"reason"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["missing_approval", b"missing_approval", "reason", b"reason"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["reason", b"reason"]) -> typing_extensions.Literal["missing_approval"] | None: ...
+
+global___ApplyRejected = ApplyRejected
```

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/entity_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/environment/clusters_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/environment/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/environment/clusters_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/environment/clusters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/environment/environment_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/events/events_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/events/events_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/events/events_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/events/events_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/events/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/events/types_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/events/types_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/events/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/insights/insights_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/insights/insights_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/insights/insights_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/insights/insights_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/managed_resource/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/metrics/metrics_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/metrics/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/metrics/metrics_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/metrics/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/object/meta_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/object/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/object/meta_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/object/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/organization/organization_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/organization/user_metadata_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/organization/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/pipelines/object_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/pipelines/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/pipelines/object_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/pipelines/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/pipelines/pipelines_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/pipelines/pipelines_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/protection/attachments_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/protection/attachments_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/protection/attachments_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/protection/attachments_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/protection/object_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/protection/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/protection/object_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/protection/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_config_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_config_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_reference_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_reference_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/object_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/release_channel/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/object_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/release_channel/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from prodvana.proto.prodvana.pipelines import pipelines_pb2 as prodvana_dot_pipelines_dot_pipelines__pb2
 from prodvana.proto.prodvana.protection import attachments_pb2 as prodvana_dot_protection_dot_attachments__pb2
 from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 from prodvana.proto.prodvana.workflow import integration_config_pb2 as prodvana_dot_workflow_dot_integration__config__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5prodvana/release_channel/release_channel_config.proto\x12\x18prodvana.release_channel\x1a\x1egoogle/protobuf/duration.proto\x1a&prodvana/common_config/constants.proto\x1a prodvana/common_config/env.proto\x1a%prodvana/common_config/maturity.proto\x1a\"prodvana/pipelines/pipelines.proto\x1a%prodvana/protection/attachments.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a\x17validate/validate.proto\"\xcd\x01\n\x06Policy\x12n\n\x0b\x64\x65\x66\x61ult_env\x18\x01 \x03(\x0b\x32\x30.prodvana.release_channel.Policy.DefaultEnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aS\n\x0f\x44\x65\x66\x61ultEnvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\"\xb4\x05\n\x14ReleaseChannelConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\r\n\x05order\x18\x02 \x01(\x03\x12\x32\n\x08maturity\x18\x03 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x30\n\x06policy\x18\x04 \x01(\x0b\x32 .prodvana.release_channel.Policy\x12G\n\x08runtimes\x18\x05 \x03(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12@\n\x12\x64\x65ploy_annotations\x18\x06 \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12=\n\rpreconditions\x18\x07 \x03(\x0b\x32&.prodvana.release_channel.Precondition\x12\x44\n\x0bprotections\x18\x08 \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12P\n\x17\x63onvergence_protections\x18\t \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12U\n\x1cservice_instance_protections\x18\x0b \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12\x33\n\tconstants\x18\n \x03(\x0b\x32 .prodvana.common_config.Constant\"\x94\x04\n\x0cPrecondition\x12]\n\x16release_channel_stable\x18\x01 \x01(\x0b\x32;.prodvana.release_channel.Precondition.ReleaseChannelStableH\x00\x12P\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x35.prodvana.release_channel.Precondition.ManualApprovalH\x00\x12H\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x31.prodvana.release_channel.Precondition.CustomTaskH\x00\x1a\\\n\x14ReleaseChannelStable\x12\x17\n\x0frelease_channel\x18\x01 \x01(\t\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x1a\x33\n\x0eManualApproval\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x1aT\n\nCustomTask\x12\x11\n\ttask_name\x18\x01 \x01(\t\x12\x33\n\x0b\x63ustom_task\x18\x02 \x01(\x0b\x32\x1e.prodvana.pipelines.CustomTaskB\x0e\n\x0cpreconditionJ\x04\x08\x04\x10\x05R\nprotection\"\xb9\x02\n\x1bReleaseChannelRuntimeConfig\x12<\n\x07runtime\x18\x02 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\x04name\x18\x03 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12S\n\x17\x63ontainer_orchestration\x18\x01 \x01(\x0b\x32\x30.prodvana.runtimes.ContainerOrchestrationRuntimeH\x00\x12=\n\x04type\x18\x04 \x01(\x0e\x32/.prodvana.release_channel.RuntimeConnectionTypeB\x0c\n\ncapability*V\n\x15RuntimeConnectionType\x12\x16\n\x12UNKNOWN_CONNECTION\x10\x00\x12\x16\n\x12LONG_LIVED_COMPUTE\x10\x01\x12\r\n\tEXTENSION\x10\x02\x42TZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/release_channelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5prodvana/release_channel/release_channel_config.proto\x12\x18prodvana.release_channel\x1a\x1egoogle/protobuf/duration.proto\x1a&prodvana/common_config/constants.proto\x1a prodvana/common_config/env.proto\x1a%prodvana/common_config/maturity.proto\x1a\"prodvana/pipelines/pipelines.proto\x1a%prodvana/protection/attachments.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a\x17validate/validate.proto\"\xcd\x01\n\x06Policy\x12n\n\x0b\x64\x65\x66\x61ult_env\x18\x01 \x03(\x0b\x32\x30.prodvana.release_channel.Policy.DefaultEnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aS\n\x0f\x44\x65\x66\x61ultEnvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\"\xb4\x05\n\x14ReleaseChannelConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\r\n\x05order\x18\x02 \x01(\x03\x12\x32\n\x08maturity\x18\x03 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x30\n\x06policy\x18\x04 \x01(\x0b\x32 .prodvana.release_channel.Policy\x12G\n\x08runtimes\x18\x05 \x03(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12@\n\x12\x64\x65ploy_annotations\x18\x06 \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12=\n\rpreconditions\x18\x07 \x03(\x0b\x32&.prodvana.release_channel.Precondition\x12\x44\n\x0bprotections\x18\x08 \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12P\n\x17\x63onvergence_protections\x18\t \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12U\n\x1cservice_instance_protections\x18\x0b \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12\x33\n\tconstants\x18\n \x03(\x0b\x32 .prodvana.common_config.Constant\"\xaa\x04\n\x0cPrecondition\x12]\n\x16release_channel_stable\x18\x01 \x01(\x0b\x32;.prodvana.release_channel.Precondition.ReleaseChannelStableH\x00\x12P\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x35.prodvana.release_channel.Precondition.ManualApprovalH\x00\x12H\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x31.prodvana.release_channel.Precondition.CustomTaskH\x00\x1a\\\n\x14ReleaseChannelStable\x12\x17\n\x0frelease_channel\x18\x01 \x01(\t\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x1aI\n\x0eManualApproval\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x14\n\x0c\x65very_action\x18\x03 \x01(\x08\x1aT\n\nCustomTask\x12\x11\n\ttask_name\x18\x01 \x01(\t\x12\x33\n\x0b\x63ustom_task\x18\x02 \x01(\x0b\x32\x1e.prodvana.pipelines.CustomTaskB\x0e\n\x0cpreconditionJ\x04\x08\x04\x10\x05R\nprotection\"\xb9\x02\n\x1bReleaseChannelRuntimeConfig\x12<\n\x07runtime\x18\x02 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\x04name\x18\x03 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12S\n\x17\x63ontainer_orchestration\x18\x01 \x01(\x0b\x32\x30.prodvana.runtimes.ContainerOrchestrationRuntimeH\x00\x12=\n\x04type\x18\x04 \x01(\x0e\x32/.prodvana.release_channel.RuntimeConnectionTypeB\x0c\n\ncapability*V\n\x15RuntimeConnectionType\x12\x16\n\x12UNKNOWN_CONNECTION\x10\x00\x12\x16\n\x12LONG_LIVED_COMPUTE\x10\x01\x12\r\n\tEXTENSION\x10\x02\x42TZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/release_channelb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.release_channel.release_channel_config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -37,26 +37,26 @@
   _POLICY.fields_by_name['default_env']._serialized_options = b'\372B$\232\001!\030\001\"\035r\0332\031^[a-zA-Z_]+[a-zA-Z0-9_]*$'
   _RELEASECHANNELCONFIG.fields_by_name['name']._options = None
   _RELEASECHANNELCONFIG.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
   _RELEASECHANNELRUNTIMECONFIG.fields_by_name['runtime']._options = None
   _RELEASECHANNELRUNTIMECONFIG.fields_by_name['runtime']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
   _RELEASECHANNELRUNTIMECONFIG.fields_by_name['name']._options = None
   _RELEASECHANNELRUNTIMECONFIG.fields_by_name['name']._serialized_options = b'\372B)r\'\020\000\030?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$'
-  _globals['_RUNTIMECONNECTIONTYPE']._serialized_start=2167
-  _globals['_RUNTIMECONNECTIONTYPE']._serialized_end=2253
+  _globals['_RUNTIMECONNECTIONTYPE']._serialized_start=2189
+  _globals['_RUNTIMECONNECTIONTYPE']._serialized_end=2275
   _globals['_POLICY']._serialized_start=414
   _globals['_POLICY']._serialized_end=619
   _globals['_POLICY_DEFAULTENVENTRY']._serialized_start=536
   _globals['_POLICY_DEFAULTENVENTRY']._serialized_end=619
   _globals['_RELEASECHANNELCONFIG']._serialized_start=622
   _globals['_RELEASECHANNELCONFIG']._serialized_end=1314
   _globals['_PRECONDITION']._serialized_start=1317
-  _globals['_PRECONDITION']._serialized_end=1849
+  _globals['_PRECONDITION']._serialized_end=1871
   _globals['_PRECONDITION_RELEASECHANNELSTABLE']._serialized_start=1584
   _globals['_PRECONDITION_RELEASECHANNELSTABLE']._serialized_end=1676
   _globals['_PRECONDITION_MANUALAPPROVAL']._serialized_start=1678
-  _globals['_PRECONDITION_MANUALAPPROVAL']._serialized_end=1729
-  _globals['_PRECONDITION_CUSTOMTASK']._serialized_start=1731
-  _globals['_PRECONDITION_CUSTOMTASK']._serialized_end=1815
-  _globals['_RELEASECHANNELRUNTIMECONFIG']._serialized_start=1852
-  _globals['_RELEASECHANNELRUNTIMECONFIG']._serialized_end=2165
+  _globals['_PRECONDITION_MANUALAPPROVAL']._serialized_end=1751
+  _globals['_PRECONDITION_CUSTOMTASK']._serialized_start=1753
+  _globals['_PRECONDITION_CUSTOMTASK']._serialized_end=1837
+  _globals['_RELEASECHANNELRUNTIMECONFIG']._serialized_start=1874
+  _globals['_RELEASECHANNELRUNTIMECONFIG']._serialized_end=2187
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -153,23 +153,26 @@
         def ClearField(self, field_name: typing_extensions.Literal["duration", b"duration", "release_channel", b"release_channel"]) -> None: ...
 
     class ManualApproval(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         NAME_FIELD_NUMBER: builtins.int
         DESCRIPTION_FIELD_NUMBER: builtins.int
+        EVERY_ACTION_FIELD_NUMBER: builtins.int
         name: builtins.str
         description: builtins.str
+        every_action: builtins.bool
         def __init__(
             self,
             *,
             name: builtins.str = ...,
             description: builtins.str = ...,
+            every_action: builtins.bool = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "name", b"name"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "every_action", b"every_action", "name", b"name"]) -> None: ...
 
     class CustomTask(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TASK_NAME_FIELD_NUMBER: builtins.int
         CUSTOM_TASK_FIELD_NUMBER: builtins.int
         task_name: builtins.str
```

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/repo/repo_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/repo/repo_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/repo/repo_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/repo/repo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/runtimes/features_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/runtimes/features_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/runtimes/features_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/runtimes/features_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/scm/types_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/scm/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/scm/types_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/scm/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/service/object_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/service/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/service/object_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/service/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/service/parameters_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/service/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/service/parameters_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/service/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/service/service_config_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/service/service_config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 from prodvana.proto.prodvana.workflow import integration_config_pb2 as prodvana_dot_workflow_dot_integration__config__pb2
 from prodvana.proto.prodvana.service import parameters_pb2 as prodvana_dot_service_dot_parameters__pb2
 from prodvana.proto.prodvana.volumes import volumes_pb2 as prodvana_dot_volumes_dot_volumes__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/service/service_config.proto\x12\x10prodvana.service\x1a\x1egoogle/protobuf/duration.proto\x1a$prodvana/capability/capability.proto\x1a&prodvana/common_config/constants.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a!prodvana/common_config/helm.proto\x1a%prodvana/common_config/maturity.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a!prodvana/common_config/task.proto\x1a\'prodvana/delivery/delivery_config.proto\x1a(prodvana/delivery_extension/config.proto\x1a%prodvana/protection/attachments.proto\x1a.prodvana/protection/protection_reference.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a!prodvana/service/parameters.proto\x1a\x1eprodvana/volumes/volumes.proto\x1a\x17validate/validate.proto\"1\n\x0eReplicasConfig\x12\x0f\n\x05\x66ixed\x18\x01 \x01(\x05H\x00\x42\x0e\n\x0c\x63onfig_oneof\"\xaa\x02\n\x0eMetricAnalysis\x12J\n\x0csuccess_rate\x18\x02 \x01(\x0b\x32\x32.prodvana.service.MetricAnalysis.SuccessRateConfigH\x00\x12\x45\n\x0blatency_p95\x18\x03 \x01(\x0b\x32..prodvana.service.MetricAnalysis.LatencyConfigH\x00\x1a\x32\n\x11SuccessRateConfig\x12\x1d\n\x15min_threshold_percent\x18\x01 \x01(\x01\x1a?\n\rLatencyConfig\x12.\n\x0bmax_latency\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x10\n\x0e\x61nalysis_oneof\"\xb7\x02\n\x15ReleaseStrategyConfig\x12<\n\x19individual_stage_deadline\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1a\x61utomated_testing_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12:\n\x10metrics_analysis\x18\x03 \x03(\x0b\x32 .prodvana.service.MetricAnalysis\x12\x17\n\x0fmanual_approval\x18\x04 \x01(\x08\x12\x31\n\x0e\x63heck_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x66\x61ilure_threshold\x18\x06 \x01(\x05\"f\n\tTLSSecret\x12\x14\n\nraw_secret\x18\x03 \x01(\tH\x00\x12\x30\n\x06secret\x18\x04 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x11\n\ntls_secret\x12\x03\xf8\x42\x01\"\x81\x01\n\x0eTLSCertificate\x12\x37\n\x08tls_cert\x18\x01 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x36\n\x07tls_key\x18\x02 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"j\n\x0b\x43\x65rtificate\x12/\n\x03tls\x18\x01 \x01(\x0b\x32 .prodvana.service.TLSCertificateH\x00\x12\x16\n\x0c\x61ws_acm_cert\x18\x02 \x01(\tH\x00\x42\x12\n\x0b\x63\x65rtificate\x12\x03\xf8\x42\x01\"\xea\t\n\x17PerReleaseChannelConfig\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12&\n\x10\x63ustom_hostnames\x18\x02 \x03(\tB\x0c\xfa\x42\t\x92\x01\x06\"\x04r\x02h\x01\x12W\n\x08programs\x18\x05 \x03(\x0b\x32\x36.prodvana.common_config.PerReleaseChannelProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12+\n\x04\x63\x65rt\x18\x06 \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12:\n\x0f\x64\x65livery_config\x18\x07 \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x08 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\t \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x43\n\x0epre_push_tasks\x18\n \x03(\x0b\x32\x1c.prodvana.service.TaskConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12U\n\x13\x64\x65livery_extensions\x18\x12 \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x41\n\x10runtime_specific\x18\x0b \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x11 \x01(\t\x12\x45\n\x11runtime_extension\x18\r \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x0e \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x10 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x0f \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12h\n\x03\x65nv\x18\x13 \x03(\x0b\x32\x32.prodvana.service.PerReleaseChannelConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12\x33\n\tconstants\x18\x14 \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x44\n\x0bprotections\x18\x15 \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x0c\x10\r\",\n\x13\x43\x61pabilityReference\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x18\x43ompiledCapabilityConfig\x12\x39\n\ncapability\x18\x01 \x01(\x0b\x32%.prodvana.capability.CapabilityConfig\".\n\x10ProgramReference\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"6\n\rTaskReference\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"\xf1\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x0c\x62\x61se_program\x18\x02 \x01(\x0b\x32\".prodvana.service.ProgramReference\x12\x39\n\x0cretry_config\x18\x03 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12,\n\x03ref\x18\x04 \x01(\x0b\x32\x1f.prodvana.service.TaskReference\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xa2\x02\n\x17\x44\x65liveryExtensionConfig\x12G\n\x07inlined\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12\x1b\n\x08instance\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12H\n\x03ref\x18\x04 \x01(\x0b\x32\x39.prodvana.delivery_extension.DeliveryExtensionInstanceRefH\x00\x12\x44\n\tlifecycle\x18\x02 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycleB\n\xfa\x42\x07\x82\x01\x04 \x00 \x01\x42\x11\n\ndefinition\x12\x03\xf8\x42\x01\"\x9e\x02\n\x19\x44\x65liveryExtensionInstance\x12G\n\x07inlined\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12H\n\x03ref\x18\x03 \x01(\x0b\x32\x39.prodvana.delivery_extension.DeliveryExtensionInstanceRefH\x00\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x44\n\tlifecycle\x18\x04 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycleB\n\xfa\x42\x07\x82\x01\x04 \x00 \x01\x42\x11\n\ndefinition\x12\x03\xf8\x42\x01\"\x9c\x02\n\x15RuntimeSpecificConfig\x12@\n\x03k8s\x18\x01 \x01(\x0b\x32\x31.prodvana.service.RuntimeSpecificConfig.K8SConfigH\x00\x1a\xae\x01\n\tK8SConfig\x12\x66\n\x13service_annotations\x18\x01 \x03(\x0b\x32I.prodvana.service.RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry\x1a\x39\n\x17ServiceAnnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0eruntime_config\"Z\n\x16RuntimeExtensionConfig\x12@\n\x10parameter_values\x18\x01 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"&\n\x12\x41utoRollbackConfig\x12\x10\n\x08\x64isabled\x18\x01 \x01(\x08\"\xd3\x0f\n\rServiceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x13\n\x0b\x61pplication\x18\x14 \x01(\t\x12\x46\n\x08programs\x18\x02 \x03(\x0b\x32%.prodvana.common_config.ProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x41\n\x10release_strategy\x18\x05 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12U\n\x13per_release_channel\x18\t \x03(\x0b\x32).prodvana.service.PerReleaseChannelConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\x0c\x63\x61pabilities\x18\n \x03(\x0b\x32%.prodvana.service.CapabilityReferenceB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12:\n\x0f\x64\x65livery_config\x18\x0b \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0c \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\r \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x34\n\x0epre_push_tasks\x18\x0f \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1d \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12Q\n\x1c\x64\x65livery_extension_instances\x18\x1e \x03(\x0b\x32+.prodvana.service.DeliveryExtensionInstance\x12\x41\n\x10runtime_specific\x18\x10 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x1c \x01(\t\x12N\n\nparameters\x18\x15 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x42\n\x10parameter_values\x18\x16 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12\x33\n\tconstants\x18! \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x34\n\x11progress_deadline\x18\x18 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x12 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x13 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x1b \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1a \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12M\n\x12parameters_autogen\x18\x17 \x01(\x0e\x32\x31.prodvana.service.ServiceConfig.ParametersAutogen\x12;\n\rauto_rollback\x18\x19 \x01(\x0b\x32$.prodvana.service.AutoRollbackConfig\x12\x1c\n\x14no_cleanup_on_delete\x18\x1f \x01(\x08\x12^\n\x03\x65nv\x18  \x03(\x0b\x32(.prodvana.service.ServiceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\"M\n\x11ParametersAutogen\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05IMAGE\x10\x02\x12\x16\n\x12IMAGE_AND_REPLICAS\x10\x03\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\x0e\x10\x0fJ\x04\x08\x11\x10\x12R\x08\x65xternalR\x10image_repositoryR\rbase_templateR\x15\x63ontainer_registry_idR\x0bprotections\"\xc2\x0e\n\x1d\x43ompiledServiceInstanceConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x12 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x32\n\x08maturity\x18\x05 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x41\n\x10release_strategy\x18\x06 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12\x18\n\x10\x63ustom_hostnames\x18\x07 \x03(\t\x12+\n\x04\x63\x65rt\x18\n \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12\x46\n\x07runtime\x18\x0b \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x1b \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12@\n\x0c\x63\x61pabilities\x18\x0c \x03(\x0b\x32*.prodvana.service.CompiledCapabilityConfig\x12:\n\x0f\x64\x65livery_config\x18\r \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0e \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\x0f \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x34\n\x0epre_push_tasks\x18\x11 \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1e \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12Q\n\x1c\x64\x65livery_extension_instances\x18\x1f \x03(\x0b\x32+.prodvana.service.DeliveryExtensionInstance\x12\x41\n\x10runtime_specific\x18\x13 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12?\n\nparameters\x18\x18 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x19 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x33\n\tconstants\x18! \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x34\n\x11progress_deadline\x18\x1a \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x16 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x17 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1d \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12n\n\x03\x65nv\x18\x1c \x03(\x0b\x32\x38.prodvana.service.CompiledServiceInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12\x1c\n\x14no_cleanup_on_delete\x18  \x01(\x08\x12\x44\n\x0bprotections\x18\" \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\x10\x10\x11J\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16R\rbase_templateR\x0cruntime_type\"\x88\x02\n\x11\x43ompiledJobConfig\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x46\n\x07runtime\x18\x04 \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x05 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/service/service_config.proto\x12\x10prodvana.service\x1a\x1egoogle/protobuf/duration.proto\x1a$prodvana/capability/capability.proto\x1a&prodvana/common_config/constants.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a!prodvana/common_config/helm.proto\x1a%prodvana/common_config/maturity.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a!prodvana/common_config/task.proto\x1a\'prodvana/delivery/delivery_config.proto\x1a(prodvana/delivery_extension/config.proto\x1a%prodvana/protection/attachments.proto\x1a.prodvana/protection/protection_reference.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a!prodvana/service/parameters.proto\x1a\x1eprodvana/volumes/volumes.proto\x1a\x17validate/validate.proto\"1\n\x0eReplicasConfig\x12\x0f\n\x05\x66ixed\x18\x01 \x01(\x05H\x00\x42\x0e\n\x0c\x63onfig_oneof\"\xaa\x02\n\x0eMetricAnalysis\x12J\n\x0csuccess_rate\x18\x02 \x01(\x0b\x32\x32.prodvana.service.MetricAnalysis.SuccessRateConfigH\x00\x12\x45\n\x0blatency_p95\x18\x03 \x01(\x0b\x32..prodvana.service.MetricAnalysis.LatencyConfigH\x00\x1a\x32\n\x11SuccessRateConfig\x12\x1d\n\x15min_threshold_percent\x18\x01 \x01(\x01\x1a?\n\rLatencyConfig\x12.\n\x0bmax_latency\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x10\n\x0e\x61nalysis_oneof\"\xb7\x02\n\x15ReleaseStrategyConfig\x12<\n\x19individual_stage_deadline\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1a\x61utomated_testing_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12:\n\x10metrics_analysis\x18\x03 \x03(\x0b\x32 .prodvana.service.MetricAnalysis\x12\x17\n\x0fmanual_approval\x18\x04 \x01(\x08\x12\x31\n\x0e\x63heck_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x66\x61ilure_threshold\x18\x06 \x01(\x05\"f\n\tTLSSecret\x12\x14\n\nraw_secret\x18\x03 \x01(\tH\x00\x12\x30\n\x06secret\x18\x04 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x11\n\ntls_secret\x12\x03\xf8\x42\x01\"\x81\x01\n\x0eTLSCertificate\x12\x37\n\x08tls_cert\x18\x01 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x36\n\x07tls_key\x18\x02 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"j\n\x0b\x43\x65rtificate\x12/\n\x03tls\x18\x01 \x01(\x0b\x32 .prodvana.service.TLSCertificateH\x00\x12\x16\n\x0c\x61ws_acm_cert\x18\x02 \x01(\tH\x00\x42\x12\n\x0b\x63\x65rtificate\x12\x03\xf8\x42\x01\"\xea\t\n\x17PerReleaseChannelConfig\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12&\n\x10\x63ustom_hostnames\x18\x02 \x03(\tB\x0c\xfa\x42\t\x92\x01\x06\"\x04r\x02h\x01\x12W\n\x08programs\x18\x05 \x03(\x0b\x32\x36.prodvana.common_config.PerReleaseChannelProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12+\n\x04\x63\x65rt\x18\x06 \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12:\n\x0f\x64\x65livery_config\x18\x07 \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x08 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\t \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x43\n\x0epre_push_tasks\x18\n \x03(\x0b\x32\x1c.prodvana.service.TaskConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12U\n\x13\x64\x65livery_extensions\x18\x12 \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x41\n\x10runtime_specific\x18\x0b \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x11 \x01(\t\x12\x45\n\x11runtime_extension\x18\r \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x0e \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x10 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x0f \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12h\n\x03\x65nv\x18\x13 \x03(\x0b\x32\x32.prodvana.service.PerReleaseChannelConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12\x33\n\tconstants\x18\x14 \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x44\n\x0bprotections\x18\x15 \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x0c\x10\r\",\n\x13\x43\x61pabilityReference\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x18\x43ompiledCapabilityConfig\x12\x39\n\ncapability\x18\x01 \x01(\x0b\x32%.prodvana.capability.CapabilityConfig\".\n\x10ProgramReference\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"6\n\rTaskReference\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"\xf1\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x0c\x62\x61se_program\x18\x02 \x01(\x0b\x32\".prodvana.service.ProgramReference\x12\x39\n\x0cretry_config\x18\x03 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12,\n\x03ref\x18\x04 \x01(\x0b\x32\x1f.prodvana.service.TaskReference\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xa2\x02\n\x17\x44\x65liveryExtensionConfig\x12G\n\x07inlined\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12\x1b\n\x08instance\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12H\n\x03ref\x18\x04 \x01(\x0b\x32\x39.prodvana.delivery_extension.DeliveryExtensionInstanceRefH\x00\x12\x44\n\tlifecycle\x18\x02 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycleB\n\xfa\x42\x07\x82\x01\x04 \x00 \x01\x42\x11\n\ndefinition\x12\x03\xf8\x42\x01\"\x9e\x02\n\x19\x44\x65liveryExtensionInstance\x12G\n\x07inlined\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12H\n\x03ref\x18\x03 \x01(\x0b\x32\x39.prodvana.delivery_extension.DeliveryExtensionInstanceRefH\x00\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x44\n\tlifecycle\x18\x04 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycleB\n\xfa\x42\x07\x82\x01\x04 \x00 \x01\x42\x11\n\ndefinition\x12\x03\xf8\x42\x01\"\x9c\x02\n\x15RuntimeSpecificConfig\x12@\n\x03k8s\x18\x01 \x01(\x0b\x32\x31.prodvana.service.RuntimeSpecificConfig.K8SConfigH\x00\x1a\xae\x01\n\tK8SConfig\x12\x66\n\x13service_annotations\x18\x01 \x03(\x0b\x32I.prodvana.service.RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry\x1a\x39\n\x17ServiceAnnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0eruntime_config\"Z\n\x16RuntimeExtensionConfig\x12@\n\x10parameter_values\x18\x01 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"&\n\x12\x41utoRollbackConfig\x12\x10\n\x08\x64isabled\x18\x01 \x01(\x08\"\xd3\x0f\n\rServiceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x13\n\x0b\x61pplication\x18\x14 \x01(\t\x12\x46\n\x08programs\x18\x02 \x03(\x0b\x32%.prodvana.common_config.ProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x41\n\x10release_strategy\x18\x05 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12U\n\x13per_release_channel\x18\t \x03(\x0b\x32).prodvana.service.PerReleaseChannelConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\x0c\x63\x61pabilities\x18\n \x03(\x0b\x32%.prodvana.service.CapabilityReferenceB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12:\n\x0f\x64\x65livery_config\x18\x0b \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0c \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\r \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x34\n\x0epre_push_tasks\x18\x0f \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1d \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12Q\n\x1c\x64\x65livery_extension_instances\x18\x1e \x03(\x0b\x32+.prodvana.service.DeliveryExtensionInstance\x12\x41\n\x10runtime_specific\x18\x10 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x1c \x01(\t\x12N\n\nparameters\x18\x15 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x42\n\x10parameter_values\x18\x16 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12\x33\n\tconstants\x18! \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x34\n\x11progress_deadline\x18\x18 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x12 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x13 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x1b \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1a \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12M\n\x12parameters_autogen\x18\x17 \x01(\x0e\x32\x31.prodvana.service.ServiceConfig.ParametersAutogen\x12;\n\rauto_rollback\x18\x19 \x01(\x0b\x32$.prodvana.service.AutoRollbackConfig\x12\x1c\n\x14no_cleanup_on_delete\x18\x1f \x01(\x08\x12^\n\x03\x65nv\x18  \x03(\x0b\x32(.prodvana.service.ServiceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\"M\n\x11ParametersAutogen\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05IMAGE\x10\x02\x12\x16\n\x12IMAGE_AND_REPLICAS\x10\x03\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\x0e\x10\x0fJ\x04\x08\x11\x10\x12R\x08\x65xternalR\x10image_repositoryR\rbase_templateR\x15\x63ontainer_registry_idR\x0bprotections\"\x97\x0f\n\x1d\x43ompiledServiceInstanceConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x12 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x32\n\x08maturity\x18\x05 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x41\n\x10release_strategy\x18\x06 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12\x18\n\x10\x63ustom_hostnames\x18\x07 \x03(\t\x12+\n\x04\x63\x65rt\x18\n \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12\x46\n\x07runtime\x18\x0b \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x1b \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12@\n\x0c\x63\x61pabilities\x18\x0c \x03(\x0b\x32*.prodvana.service.CompiledCapabilityConfig\x12:\n\x0f\x64\x65livery_config\x18\r \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0e \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\x0f \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x34\n\x0epre_push_tasks\x18\x11 \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1e \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12Q\n\x1c\x64\x65livery_extension_instances\x18\x1f \x03(\x0b\x32+.prodvana.service.DeliveryExtensionInstance\x12\x41\n\x10runtime_specific\x18\x13 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12?\n\nparameters\x18\x18 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x19 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x33\n\tconstants\x18! \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x34\n\x11progress_deadline\x18\x1a \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x16 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x17 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1d \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12n\n\x03\x65nv\x18\x1c \x03(\x0b\x32\x38.prodvana.service.CompiledServiceInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12\x1c\n\x14no_cleanup_on_delete\x18  \x01(\x08\x12\x44\n\x0bprotections\x18\" \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12(\n has_at_least_one_manual_approval\x18# \x01(\x08\x12)\n!requires_approval_for_every_apply\x18$ \x01(\x08\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\x10\x10\x11J\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16R\rbase_templateR\x0cruntime_type\"\x88\x02\n\x11\x43ompiledJobConfig\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x46\n\x07runtime\x18\x04 \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x05 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.service.service_config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -160,13 +160,13 @@
   _globals['_SERVICECONFIG']._serialized_start=4745
   _globals['_SERVICECONFIG']._serialized_end=6748
   _globals['_SERVICECONFIG_ENVENTRY']._serialized_start=3036
   _globals['_SERVICECONFIG_ENVENTRY']._serialized_end=3112
   _globals['_SERVICECONFIG_PARAMETERSAUTOGEN']._serialized_start=6546
   _globals['_SERVICECONFIG_PARAMETERSAUTOGEN']._serialized_end=6623
   _globals['_COMPILEDSERVICEINSTANCECONFIG']._serialized_start=6751
-  _globals['_COMPILEDSERVICEINSTANCECONFIG']._serialized_end=8609
+  _globals['_COMPILEDSERVICEINSTANCECONFIG']._serialized_end=8694
   _globals['_COMPILEDSERVICEINSTANCECONFIG_ENVENTRY']._serialized_start=3036
   _globals['_COMPILEDSERVICEINSTANCECONFIG_ENVENTRY']._serialized_end=3112
-  _globals['_COMPILEDJOBCONFIG']._serialized_start=8612
-  _globals['_COMPILEDJOBCONFIG']._serialized_end=8876
+  _globals['_COMPILEDJOBCONFIG']._serialized_start=8697
+  _globals['_COMPILEDJOBCONFIG']._serialized_end=8961
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/service/service_config_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/service/service_config_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -790,14 +790,16 @@
     PROGRESS_DEADLINE_FIELD_NUMBER: builtins.int
     RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     HELM_FIELD_NUMBER: builtins.int
     ENV_FIELD_NUMBER: builtins.int
     NO_CLEANUP_ON_DELETE_FIELD_NUMBER: builtins.int
     PROTECTIONS_FIELD_NUMBER: builtins.int
+    HAS_AT_LEAST_ONE_MANUAL_APPROVAL_FIELD_NUMBER: builtins.int
+    REQUIRES_APPROVAL_FOR_EVERY_APPLY_FIELD_NUMBER: builtins.int
     service: builtins.str
     application: builtins.str
     release_channel: builtins.str
     @property
     def programs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig]: ...
     @property
     def replicas(self) -> global___ReplicasConfig: ...
@@ -849,14 +851,18 @@
     def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
         """The compiled environment for this instance's context, e.g.  Release Channel.
         This is used to inject these values into external configs.
         """
     no_cleanup_on_delete: builtins.bool
     @property
     def protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig]: ...
+    has_at_least_one_manual_approval: builtins.bool
+    """Does this service instance have at least one manual approval configured?"""
+    requires_approval_for_every_apply: builtins.bool
+    """Does this service instance require manual approval on each push/apply action?"""
     def __init__(
         self,
         *,
         service: builtins.str = ...,
         application: builtins.str = ...,
         release_channel: builtins.str = ...,
         programs: collections.abc.Iterable[prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig] | None = ...,
@@ -881,17 +887,19 @@
         progress_deadline: google.protobuf.duration_pb2.Duration | None = ...,
         runtime_extension: global___RuntimeExtensionConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
         env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
         no_cleanup_on_delete: builtins.bool = ...,
         protections: collections.abc.Iterable[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig] | None = ...,
+        has_at_least_one_manual_approval: builtins.bool = ...,
+        requires_approval_for_every_apply: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "capabilities", b"capabilities", "cert", b"cert", "config_oneof", b"config_oneof", "constants", b"constants", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "delivery_extension_instances", b"delivery_extension_instances", "delivery_extensions", b"delivery_extensions", "deploy_annotations", b"deploy_annotations", "env", b"env", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "maturity", b"maturity", "no_cleanup_on_delete", b"no_cleanup_on_delete", "parameter_values", b"parameter_values", "parameters", b"parameters", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "protections", b"protections", "release_channel", b"release_channel", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "service", b"service", "volumes", b"volumes"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "capabilities", b"capabilities", "cert", b"cert", "config_oneof", b"config_oneof", "constants", b"constants", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "delivery_extension_instances", b"delivery_extension_instances", "delivery_extensions", b"delivery_extensions", "deploy_annotations", b"deploy_annotations", "env", b"env", "has_at_least_one_manual_approval", b"has_at_least_one_manual_approval", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "maturity", b"maturity", "no_cleanup_on_delete", b"no_cleanup_on_delete", "parameter_values", b"parameter_values", "parameters", b"parameters", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "protections", b"protections", "release_channel", b"release_channel", "release_strategy", b"release_strategy", "replicas", b"replicas", "requires_approval_for_every_apply", b"requires_approval_for_every_apply", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "service", b"service", "volumes", b"volumes"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["runtime_extension", "kubernetes_config", "helm"] | None: ...
 
 global___CompiledServiceInstanceConfig = CompiledServiceInstanceConfig
 
 class CompiledJobConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/service/service_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/service/service_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/service/user_metadata_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/service/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/service/user_metadata_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/service/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/settings/organization/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/settings/organization/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/stat/efficiency_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/stat/efficiency_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/stat/efficiency_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/stat/efficiency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/users/users_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/users/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/users/users_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/users/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/version/source_metadata_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/version/source_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/version/source_metadata_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/version/source_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/volumes/volumes_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/volumes/volumes_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/volumes/volumes_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/volumes/volumes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/workflow/integration_config_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/workflow/integration_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py` & `prodvana-0.2.2/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py` & `prodvana-0.2.2/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi` & `prodvana-0.2.2/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/validate/validate_pb2.py` & `prodvana-0.2.2/prodvana/proto/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/proto/validate/validate_pb2.pyi` & `prodvana-0.2.2/prodvana/proto/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/utils/desired_states.py` & `prodvana-0.2.2/prodvana/utils/desired_states.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/utils/parameters.py` & `prodvana-0.2.2/prodvana/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/utils/protections.py` & `prodvana-0.2.2/prodvana/utils/protections.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/utils/service_config.py` & `prodvana-0.2.2/prodvana/utils/service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/prodvana/utils/tests/test_service_config.py` & `prodvana-0.2.2/prodvana/utils/tests/test_service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.2.1/pyproject.toml` & `prodvana-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodvana"
-version = "0.2.1"
+version = "0.2.2"
 description = "Prodvana's client libraries"
 readme = "README.md"
 authors = []
 homepage = "https://prodvana.io"
 documentation = "https://docs.prodvana.io"
 repository = "https://github.com/prodvana/prodvana-public"
 exclude = ["examples"]
```

### Comparing `prodvana-0.2.1/PKG-INFO` & `prodvana-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodvana
-Version: 0.2.1
+Version: 0.2.2
 Summary: Prodvana's client libraries
 Home-page: https://prodvana.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-api-python-client (>=2.58.0,<3.0)
```

