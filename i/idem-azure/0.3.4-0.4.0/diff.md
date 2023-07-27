# Comparing `tmp/idem-azure-0.3.4.tar.gz` & `tmp/idem-azure-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-azure-0.3.4.tar", last modified: Thu Jun 15 13:50:35 2023, max compression
+gzip compressed data, was "idem-azure-0.4.0.tar", last modified: Thu Jul 27 13:38:44 2023, max compression
```

## Comparing `idem-azure-0.3.4.tar` & `idem-azure-0.4.0.tar`

### file list

```diff
@@ -1,148 +1,164 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-06-15 13:50:21.000000 idem-azure-0.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7784 2023-06-15 13:50:35.838512 idem-azure-0.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6904 2023-06-15 13:50:21.000000 idem-azure-0.3.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.830511 idem-azure-0.3.4/idem_azure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.830511 idem-azure-0.3.4/idem_azure/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/acct/azure/
--rw-r--r--   0 root         (0) root         (0)     1994 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/acct/azure/login.py
--rw-r--r--   0 root         (0) root         (0)      801 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/acct/azure/mock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/acct/metadata/
--rw-r--r--   0 root         (0) root         (0)      361 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/acct/metadata/azure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.830511 idem-azure-0.3.4/idem_azure/backup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/backup/virtual_networks/
--rw-r--r--   0 root         (0) root         (0)    10446 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/backup/virtual_networks/nat_gateways.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/backup/virtual_networks/public_ip_addresses.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/backup/virtual_networks/routes.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.830511 idem-azure-0.3.4/idem_azure/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/exec/azure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/exec/azure/authorization/
--rw-r--r--   0 root         (0) root         (0)     3940 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/authorization/role_assignments.py
--rw-r--r--   0 root         (0) root         (0)     4259 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/authorization/role_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/exec/azure/compute/
--rw-r--r--   0 root         (0) root         (0)     4226 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/compute/log_analytics_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4136 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/compute/virtual_machines.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/exec/azure/key_vault/
--rw-r--r--   0 root         (0) root         (0)     3819 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/key_vault/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/exec/azure/management_groups/
--rw-r--r--   0 root         (0) root         (0)     3779 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/management_groups/management_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/exec/azure/network/
--rw-r--r--   0 root         (0) root         (0)     3877 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/network/firewall.py
--rw-r--r--   0 root         (0) root         (0)     4133 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/network/firewall_policies.py
--rw-r--r--   0 root         (0) root         (0)     4030 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/network/network_interfaces.py
--rw-r--r--   0 root         (0) root         (0)     4221 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/network/network_security_groups.py
--rw-r--r--   0 root         (0) root         (0)     4082 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/network/public_ip_addresses.py
--rw-r--r--   0 root         (0) root         (0)     3946 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/network/route_tables.py
--rw-r--r--   0 root         (0) root         (0)     4372 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/network/routes.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/network/security_rules.py
--rw-r--r--   0 root         (0) root         (0)     4368 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/network/subnets.py
--rw-r--r--   0 root         (0) root         (0)     3995 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/network/virtual_networks.py
--rw-r--r--   0 root         (0) root         (0)     1252 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/permission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/exec/azure/policy/
--rw-r--r--   0 root         (0) root         (0)     3193 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/policy/policy_assignments.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/policy/policy_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/exec/azure/resource_management/
--rw-r--r--   0 root         (0) root         (0)     3948 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/resource_management/resource_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/exec/azure/storage_resource_provider/
--rw-r--r--   0 root         (0) root         (0)     4116 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/storage_resource_provider/storage_accounts.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/storage_resource_provider/storage_blob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/exec/azure/subscription/
--rw-r--r--   0 root         (0) root         (0)     4191 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/subscription/attach_subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     4405 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/exec/azure/subscription/subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.830511 idem-azure-0.3.4/idem_azure/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/pop_create/azure/
--rw-r--r--   0 root         (0) root         (0)     2572 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/pop_create/azure/api_reference.py
--rw-r--r--   0 root         (0) root         (0)     7272 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/pop_create/azure/api_spec.py
--rw-r--r--   0 root         (0) root         (0)     4737 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/pop_create/azure/init.py
--rw-r--r--   0 root         (0) root         (0)     5085 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/pop_create/azure/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1526 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/pop_create/azure/resource.py
--rw-r--r--   0 root         (0) root         (0)     4766 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/pop_create/azure/rest.py
--rw-r--r--   0 root         (0) root         (0)    11179 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/pop_create/azure/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.830511 idem-azure-0.3.4/idem_azure/reconcile/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/reconcile/pending/
--rw-r--r--   0 root         (0) root         (0)     1696 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/reconcile/pending/azure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.830511 idem-azure-0.3.4/idem_azure/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/states/azure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/states/azure/authorization/
--rw-r--r--   0 root         (0) root         (0)    10160 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/authorization/role_assignments.py
--rw-r--r--   0 root         (0) root         (0)    12622 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/authorization/role_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/states/azure/compute/
--rw-r--r--   0 root         (0) root         (0)    16304 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/compute/log_analytics_workspace.py
--rw-r--r--   0 root         (0) root         (0)    19615 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/compute/virtual_machines.py
--rw-r--r--   0 root         (0) root         (0)      372 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/states/azure/key_vault/
--rw-r--r--   0 root         (0) root         (0)    18648 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/key_vault/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure/states/azure/management_groups/
--rw-r--r--   0 root         (0) root         (0)    11659 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/management_groups/management_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/states/azure/network/
--rw-r--r--   0 root         (0) root         (0)    15838 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/network/firewall.py
--rw-r--r--   0 root         (0) root         (0)    14921 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/network/firewall_policies.py
--rw-r--r--   0 root         (0) root         (0)    15532 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/network/network_interfaces.py
--rw-r--r--   0 root         (0) root         (0)    15488 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/network/network_security_groups.py
--rw-r--r--   0 root         (0) root         (0)    16001 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/network/public_ip_addresses.py
--rw-r--r--   0 root         (0) root         (0)    13954 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/network/route_tables.py
--rw-r--r--   0 root         (0) root         (0)    12656 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/network/routes.py
--rw-r--r--   0 root         (0) root         (0)    17142 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/network/security_rules.py
--rw-r--r--   0 root         (0) root         (0)    15676 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/network/subnets.py
--rw-r--r--   0 root         (0) root         (0)    14926 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/network/virtual_networks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/states/azure/policy/
--rw-r--r--   0 root         (0) root         (0)    12283 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/policy/policy_assignments.py
--rw-r--r--   0 root         (0) root         (0)    13235 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/policy/policy_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/states/azure/resource_management/
--rw-r--r--   0 root         (0) root         (0)    11624 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/resource_management/resource_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/states/azure/storage_resource_provider/
--rw-r--r--   0 root         (0) root         (0)    29668 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/storage_resource_provider/storage_accounts.py
--rw-r--r--   0 root         (0) root         (0)    14447 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/storage_resource_provider/storage_blob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/states/azure/subscription/
--rw-r--r--   0 root         (0) root         (0)     8445 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/subscription/attach_subscriptions.py
--rw-r--r--   0 root         (0) root         (0)    11510 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/states/azure/subscription/subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.830511 idem-azure-0.3.4/idem_azure/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/tool/azure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/tool/azure/authorization/
--rw-r--r--   0 root         (0) root         (0)     2377 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/authorization/role_assignments.py
--rw-r--r--   0 root         (0) root         (0)     7362 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/authorization/role_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/tool/azure/compute/
--rw-r--r--   0 root         (0) root         (0)    16498 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/compute/log_analytics_workspace.py
--rw-r--r--   0 root         (0) root         (0)    31418 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/compute/virtual_machines.py
--rw-r--r--   0 root         (0) root         (0)     1999 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/tool/azure/key_vault/
--rw-r--r--   0 root         (0) root         (0)     9536 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/key_vault/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/tool/azure/management_groups/
--rw-r--r--   0 root         (0) root         (0)     4329 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/management_groups/management_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/tool/azure/network/
--rw-r--r--   0 root         (0) root         (0)     6983 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/network/firewall.py
--rw-r--r--   0 root         (0) root         (0)     7073 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/network/firewall_policies.py
--rw-r--r--   0 root         (0) root         (0)    10032 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/network/network_interfaces.py
--rw-r--r--   0 root         (0) root         (0)    10207 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/network/network_security_groups.py
--rw-r--r--   0 root         (0) root         (0)    14334 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/network/public_ip_addresses.py
--rw-r--r--   0 root         (0) root         (0)     8907 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/network/route_tables.py
--rw-r--r--   0 root         (0) root         (0)     4816 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/network/routes.py
--rw-r--r--   0 root         (0) root         (0)    12345 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/network/security_rules.py
--rw-r--r--   0 root         (0) root         (0)    13498 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/network/subnets.py
--rw-r--r--   0 root         (0) root         (0)    11127 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/network/virtual_networks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/tool/azure/policy/
--rw-r--r--   0 root         (0) root         (0)     3795 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/policy/policy_assignment.py
--rw-r--r--   0 root         (0) root         (0)     6870 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/policy/policy_definition.py
--rw-r--r--   0 root         (0) root         (0)     5513 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/tool/azure/resource_management/
--rw-r--r--   0 root         (0) root         (0)     3308 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/resource_management/resource_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/tool/azure/storage_resource_provider/
--rw-r--r--   0 root         (0) root         (0)    52455 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/storage_resource_provider/storage_accounts.py
--rw-r--r--   0 root         (0) root         (0)     9128 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/storage_resource_provider/storage_blob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/tool/azure/subscription/
--rw-r--r--   0 root         (0) root         (0)     3956 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/subscription/subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/test_state_utils.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/azure/uri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.838512 idem-azure-0.3.4/idem_azure/tool/validators/
--rw-r--r--   0 root         (0) root         (0)      744 2023-06-15 13:50:21.000000 idem-azure-0.3.4/idem_azure/tool/validators/http.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-15 13:50:35.000000 idem-azure-0.3.4/idem_azure/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:50:35.834511 idem-azure-0.3.4/idem_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7784 2023-06-15 13:50:35.000000 idem-azure-0.3.4/idem_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4687 2023-06-15 13:50:35.000000 idem-azure-0.3.4/idem_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 13:50:35.000000 idem-azure-0.3.4/idem_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-15 13:50:35.000000 idem-azure-0.3.4/idem_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-15 13:50:35.000000 idem-azure-0.3.4/idem_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-15 13:50:35.838512 idem-azure-0.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2792 2023-06-15 13:50:21.000000 idem-azure-0.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.920464 idem-azure-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-07-27 13:38:30.000000 idem-azure-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7784 2023-07-27 13:38:44.920464 idem-azure-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6904 2023-07-27 13:38:30.000000 idem-azure-0.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.908464 idem-azure-0.4.0/idem_azure/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/acct/azure/
+-rw-r--r--   0 root         (0) root         (0)     2643 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/acct/azure/login.py
+-rw-r--r--   0 root         (0) root         (0)      801 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/acct/azure/mock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/acct/metadata/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/acct/metadata/azure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.908464 idem-azure-0.4.0/idem_azure/backup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/backup/virtual_networks/
+-rw-r--r--   0 root         (0) root         (0)    10467 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/backup/virtual_networks/nat_gateways.py
+-rw-r--r--   0 root         (0) root         (0)    10725 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/backup/virtual_networks/public_ip_addresses.py
+-rw-r--r--   0 root         (0) root         (0)    10047 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/backup/virtual_networks/routes.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.908464 idem-azure-0.4.0/idem_azure/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/exec/azure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/exec/azure/authorization/
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/authorization/role_assignments.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/authorization/role_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/exec/azure/compute/
+-rw-r--r--   0 root         (0) root         (0)     4229 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/compute/log_analytics_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/compute/virtual_machines.py
+-rw-r--r--   0 root         (0) root         (0)      484 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/exec/azure/key_vault/
+-rw-r--r--   0 root         (0) root         (0)     3819 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/key_vault/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/exec/azure/management_groups/
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/management_groups/management_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/exec/azure/network/
+-rw-r--r--   0 root         (0) root         (0)     3877 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/network/firewall.py
+-rw-r--r--   0 root         (0) root         (0)     4136 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/network/firewall_policies.py
+-rw-r--r--   0 root         (0) root         (0)     4030 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/network/network_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     4227 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/network/network_security_groups.py
+-rw-r--r--   0 root         (0) root         (0)     4085 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/network/public_ip_addresses.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/network/route_tables.py
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/network/routes.py
+-rw-r--r--   0 root         (0) root         (0)     3506 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/network/security_rules.py
+-rw-r--r--   0 root         (0) root         (0)     4371 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/network/subnets.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/network/virtual_network_peerings.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/network/virtual_networks.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/permission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/exec/azure/policy/
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/policy/policy_assignments.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/policy/policy_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/exec/azure/resource_management/
+-rw-r--r--   0 root         (0) root         (0)     3951 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/resource_management/resource_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/exec/azure/sql_database/
+-rw-r--r--   0 root         (0) root         (0)     6050 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/sql_database/databases.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/exec/azure/storage_resource_provider/
+-rw-r--r--   0 root         (0) root         (0)     4119 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/storage_resource_provider/storage_accounts.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/storage_resource_provider/storage_blob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/exec/azure/subscription/
+-rw-r--r--   0 root         (0) root         (0)     4191 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/subscription/attach_subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     4405 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/exec/azure/subscription/subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.908464 idem-azure-0.4.0/idem_azure/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/pop_create/azure/
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/pop_create/azure/api_reference.py
+-rw-r--r--   0 root         (0) root         (0)     7272 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/pop_create/azure/api_spec.py
+-rw-r--r--   0 root         (0) root         (0)     4737 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/pop_create/azure/init.py
+-rw-r--r--   0 root         (0) root         (0)     5085 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/pop_create/azure/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/pop_create/azure/resource.py
+-rw-r--r--   0 root         (0) root         (0)     4766 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/pop_create/azure/rest.py
+-rw-r--r--   0 root         (0) root         (0)    11191 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/pop_create/azure/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.908464 idem-azure-0.4.0/idem_azure/reconcile/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/reconcile/pending/
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/reconcile/pending/azure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.908464 idem-azure-0.4.0/idem_azure/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/states/azure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure/states/azure/authorization/
+-rw-r--r--   0 root         (0) root         (0)    10160 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/authorization/role_assignments.py
+-rw-r--r--   0 root         (0) root         (0)    12622 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/authorization/role_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/states/azure/compute/
+-rw-r--r--   0 root         (0) root         (0)    16316 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/compute/log_analytics_workspace.py
+-rw-r--r--   0 root         (0) root         (0)    24487 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/compute/virtual_machines.py
+-rw-r--r--   0 root         (0) root         (0)      372 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/states/azure/key_vault/
+-rw-r--r--   0 root         (0) root         (0)    18648 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/key_vault/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/states/azure/management_groups/
+-rw-r--r--   0 root         (0) root         (0)    11659 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/management_groups/management_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/states/azure/network/
+-rw-r--r--   0 root         (0) root         (0)    15838 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/network/firewall.py
+-rw-r--r--   0 root         (0) root         (0)    14921 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/network/firewall_policies.py
+-rw-r--r--   0 root         (0) root         (0)    15532 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/network/network_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)    15497 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/network/network_security_groups.py
+-rw-r--r--   0 root         (0) root         (0)    16001 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/network/public_ip_addresses.py
+-rw-r--r--   0 root         (0) root         (0)    13954 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/network/route_tables.py
+-rw-r--r--   0 root         (0) root         (0)    12656 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/network/routes.py
+-rw-r--r--   0 root         (0) root         (0)    17151 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/network/security_rules.py
+-rw-r--r--   0 root         (0) root         (0)    15676 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/network/subnets.py
+-rw-r--r--   0 root         (0) root         (0)     7653 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/network/virtual_network_peerings.py
+-rw-r--r--   0 root         (0) root         (0)    17439 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/network/virtual_networks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/states/azure/policy/
+-rw-r--r--   0 root         (0) root         (0)    12283 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/policy/policy_assignments.py
+-rw-r--r--   0 root         (0) root         (0)    13235 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/policy/policy_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/states/azure/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)     2819 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/states/azure/resource_management/
+-rw-r--r--   0 root         (0) root         (0)    11624 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/resource_management/resource_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/states/azure/sql_database/
+-rw-r--r--   0 root         (0) root         (0)    27864 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/sql_database/databases.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/states/azure/storage_resource_provider/
+-rw-r--r--   0 root         (0) root         (0)    32277 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/storage_resource_provider/storage_accounts.py
+-rw-r--r--   0 root         (0) root         (0)    14461 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/storage_resource_provider/storage_blob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/states/azure/subscription/
+-rw-r--r--   0 root         (0) root         (0)     8445 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/subscription/attach_subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)    11510 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/states/azure/subscription/subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.908464 idem-azure-0.4.0/idem_azure/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/tool/azure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/tool/azure/authorization/
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/authorization/role_assignments.py
+-rw-r--r--   0 root         (0) root         (0)     7362 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/authorization/role_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     1758 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/tool/azure/compute/
+-rw-r--r--   0 root         (0) root         (0)    16498 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/compute/log_analytics_workspace.py
+-rw-r--r--   0 root         (0) root         (0)    35879 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/compute/virtual_machines.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/container.py
+-rw-r--r--   0 root         (0) root         (0)    17576 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/generic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/tool/azure/key_vault/
+-rw-r--r--   0 root         (0) root         (0)     9536 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/key_vault/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/tool/azure/management_groups/
+-rw-r--r--   0 root         (0) root         (0)     4329 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/management_groups/management_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.916464 idem-azure-0.4.0/idem_azure/tool/azure/network/
+-rw-r--r--   0 root         (0) root         (0)     6983 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/network/firewall.py
+-rw-r--r--   0 root         (0) root         (0)     7073 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/network/firewall_policies.py
+-rw-r--r--   0 root         (0) root         (0)    10032 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/network/network_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)    10207 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/network/network_security_groups.py
+-rw-r--r--   0 root         (0) root         (0)    14334 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/network/public_ip_addresses.py
+-rw-r--r--   0 root         (0) root         (0)     8907 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/network/route_tables.py
+-rw-r--r--   0 root         (0) root         (0)     4816 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/network/routes.py
+-rw-r--r--   0 root         (0) root         (0)    12345 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/network/security_rules.py
+-rw-r--r--   0 root         (0) root         (0)    13498 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/network/subnets.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/network/virtual_network_peerings.py
+-rw-r--r--   0 root         (0) root         (0)    15003 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/network/virtual_networks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.920464 idem-azure-0.4.0/idem_azure/tool/azure/policy/
+-rw-r--r--   0 root         (0) root         (0)     3795 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/policy/policy_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     6870 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/policy/policy_definition.py
+-rw-r--r--   0 root         (0) root         (0)     3989 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/polling.py
+-rw-r--r--   0 root         (0) root         (0)     5513 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.920464 idem-azure-0.4.0/idem_azure/tool/azure/resource_management/
+-rw-r--r--   0 root         (0) root         (0)     3308 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/resource_management/resource_groups.py
+-rw-r--r--   0 root         (0) root         (0)     2135 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/resource_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.920464 idem-azure-0.4.0/idem_azure/tool/azure/sql_database/
+-rw-r--r--   0 root         (0) root         (0)     9978 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/sql_database/databases.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.920464 idem-azure-0.4.0/idem_azure/tool/azure/storage_resource_provider/
+-rw-r--r--   0 root         (0) root         (0)    62655 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/storage_resource_provider/storage_accounts.py
+-rw-r--r--   0 root         (0) root         (0)     9128 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/storage_resource_provider/storage_blob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.920464 idem-azure-0.4.0/idem_azure/tool/azure/subscription/
+-rw-r--r--   0 root         (0) root         (0)     3956 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/subscription/subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/test_state_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/uri.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/azure/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.920464 idem-azure-0.4.0/idem_azure/tool/validators/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-27 13:38:30.000000 idem-azure-0.4.0/idem_azure/tool/validators/http.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-27 13:38:44.000000 idem-azure-0.4.0/idem_azure/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:38:44.912464 idem-azure-0.4.0/idem_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7784 2023-07-27 13:38:44.000000 idem-azure-0.4.0/idem_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-07-27 13:38:44.000000 idem-azure-0.4.0/idem_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 13:38:44.000000 idem-azure-0.4.0/idem_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-27 13:38:44.000000 idem-azure-0.4.0/idem_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-27 13:38:44.000000 idem-azure-0.4.0/idem_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 13:38:44.920464 idem-azure-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2792 2023-07-27 13:38:30.000000 idem-azure-0.4.0/setup.py
```

### Comparing `idem-azure-0.3.4/LICENSE` & `idem-azure-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/PKG-INFO` & `idem-azure-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-azure
-Version: 0.3.4
+Version: 0.4.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/vmware/idem/idem-azure
 Author: Yingzhi Hao
 Author-email: hyingzhi@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-azure-0.3.4/README.rst` & `idem-azure-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/acct/azure/mock.py` & `idem-azure-0.4.0/idem_azure/acct/azure/mock.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/backup/virtual_networks/nat_gateways.py` & `idem-azure-0.4.0/idem_azure/backup/virtual_networks/nat_gateways.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,28 +47,28 @@
     """
     if parameters is None:
         parameters = {}
 
     subscription_id = ctx.acct.subscription_id
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/natGateways/{nat_gateway_name}?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/natGateways/{nat_gateway_name}?api-version=2021-03-01",
         success_codes=[200],
     )
 
     if force_update:
         if ctx.get("test", False):
             return dict(
                 name=name,
                 result=True,
                 comment="Would force to update azure.virtual_networks.nat_gateways",
             )
         response_force_put = await hub.exec.request.json.put(
             ctx,
-            url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/natGateways/{nat_gateway_name}?api-version=2021-03-01",
+            url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/natGateways/{nat_gateway_name}?api-version=2021-03-01",
             success_codes=[200, 201],
             json=parameters,
         )
         if response_force_put["result"]:
             old_resource = response_get["ret"] if response_get["result"] else None
             return dict(
                 name=name,
@@ -96,15 +96,15 @@
                 comment="Would create azure.virtual_networks.nat_gateways",
             )
 
         if response_get["status"] == 404:
             # PUT operation to create a resource
             response_put = await hub.exec.request.json.put(
                 ctx,
-                url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/natGateways/{nat_gateway_name}?api-version=2021-03-01",
+                url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/natGateways/{nat_gateway_name}?api-version=2021-03-01",
                 success_codes=[200, 201],
                 json=parameters,
             )
 
             if not response_put["result"]:
                 hub.log.debug(
                     f"Could not create Nat Gateways {response_put['comment']} {response_put['ret']}"
@@ -154,15 +154,15 @@
                 old_state=existing_resource,
                 new_state=existing_resource,
                 comment=f"'{name}' has no property need to be updated.",
             )
 
         response_patch = await hub.exec.request.json.patch(
             ctx,
-            url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/natGateways/{nat_gateway_name}?api-version=2021-03-01",
+            url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/natGateways/{nat_gateway_name}?api-version=2021-03-01",
             success_codes=[200],
             json=new_parameters,
         )
 
         if not response_patch["result"]:
             hub.log.debug(
                 f"Could not update Nat Gateways {response_patch['comment']} {response_patch['ret']}"
@@ -209,29 +209,29 @@
                 - resource_group_name: value
                 - nat_gateway_name: value
     """
 
     subscription_id = ctx.acct.subscription_id
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/natGateways/{nat_gateway_name}?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/natGateways/{nat_gateway_name}?api-version=2021-03-01",
         success_codes=[200],
     )
     if response_get["result"]:
         if ctx.get("test", False):
             return dict(
                 name=name,
                 result=True,
                 comment="Would delete azure.virtual_networks.nat_gateways",
             )
 
         existing_resource = response_get["ret"]
         response_delete = await hub.exec.request.raw.delete(
             ctx,
-            url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/natGateways/{nat_gateway_name}?api-version=2021-03-01",
+            url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/natGateways/{nat_gateway_name}?api-version=2021-03-01",
             success_codes=[200, 202],
         )
 
         if not response_delete["result"]:
             hub.log.debug(
                 f"Could not delete Nat Gateways {response_delete['comment']} {response_delete['ret']}"
             )
@@ -296,15 +296,15 @@
         {
             "resourceGroups": "resource_group_name",
             "natGateways": "nat_gateway_name",
         }
     )
     async for page_result in hub.tool.azure.request.paginate(
         ctx,
-        url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/providers/Microsoft.Network/natGateways?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/providers/Microsoft.Network/natGateways?api-version=2021-03-01",
         success_codes=[200],
     ):
         resource_list = page_result.get("value", None)
         if resource_list:
             for resource in resource_list:
                 uri_parameter_values = hub.tool.azure.uri.get_parameter_value(
                     resource["id"], uri_parameters
```

### Comparing `idem-azure-0.3.4/idem_azure/backup/virtual_networks/public_ip_addresses.py` & `idem-azure-0.4.0/idem_azure/backup/virtual_networks/public_ip_addresses.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,28 +46,28 @@
     """
     if parameters is None:
         parameters = {}
 
     subscription_id = ctx.acct.subscription_id
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/publicIPAddresses/{public_ip_address_name}?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/publicIPAddresses/{public_ip_address_name}?api-version=2021-03-01",
         success_codes=[200],
     )
 
     if force_update:
         if ctx.get("test", False):
             return dict(
                 name=name,
                 result=True,
                 comment="Would force to update azure.virtual_networks.public_ip_addresses",
             )
         response_force_put = await hub.exec.request.json.put(
             ctx,
-            url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/publicIPAddresses/{public_ip_address_name}?api-version=2021-03-01",
+            url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/publicIPAddresses/{public_ip_address_name}?api-version=2021-03-01",
             success_codes=[200, 201],
             json=parameters,
         )
         if response_force_put["result"]:
             old_resource = response_get["ret"] if response_get["result"] else None
             return dict(
                 name=name,
@@ -95,15 +95,15 @@
                 comment="Would create azure.virtual_networks.public_ip_addresses",
             )
 
         if response_get["status"] == 404:
             # PUT operation to create a resource
             response_put = await hub.exec.request.json.put(
                 ctx,
-                url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/publicIPAddresses/{public_ip_address_name}?api-version=2021-03-01",
+                url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/publicIPAddresses/{public_ip_address_name}?api-version=2021-03-01",
                 success_codes=[200, 201],
                 json=parameters,
             )
 
             if not response_put["result"]:
                 hub.log.debug(
                     f"Could not create Public IP Addresses {response_put['comment']} {response_put['ret']}"
@@ -153,15 +153,15 @@
                 old_state=existing_resource,
                 new_state=existing_resource,
                 comment=f"'{name}' has no property need to be updated.",
             )
 
         response_patch = await hub.exec.request.json.patch(
             ctx,
-            url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/publicIPAddresses/{public_ip_address_name}?api-version=2021-03-01",
+            url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/publicIPAddresses/{public_ip_address_name}?api-version=2021-03-01",
             success_codes=[200],
             json=new_parameters,
         )
 
         if not response_patch["result"]:
             hub.log.debug(
                 f"Could not update Public IP Addresses {response_patch['comment']} {response_patch['ret']}"
@@ -208,29 +208,29 @@
                 - resource_group_name: value
                 - public_ip_address_name: value
     """
 
     subscription_id = ctx.acct.subscription_id
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/publicIPAddresses/{public_ip_address_name}?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/publicIPAddresses/{public_ip_address_name}?api-version=2021-03-01",
         success_codes=[200],
     )
     if response_get["result"]:
         if ctx.get("test", False):
             return dict(
                 name=name,
                 result=True,
                 comment="Would delete azure.virtual_networks.public_ip_addresses",
             )
 
         existing_resource = response_get["ret"]
         response_delete = await hub.exec.request.raw.delete(
             ctx,
-            url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/publicIPAddresses/{public_ip_address_name}?api-version=2021-03-01",
+            url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/publicIPAddresses/{public_ip_address_name}?api-version=2021-03-01",
             success_codes=[200, 202, 204],
         )
 
         if not response_delete["result"]:
             hub.log.debug(
                 f"Could not delete Public IP Addresses {response_delete['comment']} {response_delete['ret']}"
             )
@@ -295,15 +295,15 @@
         {
             "resourceGroups": "resource_group_name",
             "publicIPAddresses": "public_ip_address_name",
         }
     )
     async for page_result in hub.tool.azure.request.paginate(
         ctx,
-        url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/providers/Microsoft.Network/publicIPAddresses?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/providers/Microsoft.Network/publicIPAddresses?api-version=2021-03-01",
         success_codes=[200],
     ):
         resource_list = page_result.get("value", None)
         if resource_list:
             for resource in resource_list:
                 uri_parameter_values = hub.tool.azure.uri.get_parameter_value(
                     resource["id"], uri_parameters
```

### Comparing `idem-azure-0.3.4/idem_azure/backup/virtual_networks/routes.py` & `idem-azure-0.4.0/idem_azure/backup/virtual_networks/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,28 +50,28 @@
     """
     if parameters is None:
         parameters = {}
 
     subscription_id = ctx.acct.subscription_id
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/routeTables/{route_table_name}/routes/{route_name}?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/routeTables/{route_table_name}/routes/{route_name}?api-version=2021-03-01",
         success_codes=[200],
     )
 
     if force_update:
         if ctx.get("test", False):
             return dict(
                 name=name,
                 result=True,
                 comment="Would force to update azure.virtual_networks.routes",
             )
         response_force_put = await hub.exec.request.json.put(
             ctx,
-            url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/routeTables/{route_table_name}/routes/{route_name}?api-version=2021-03-01",
+            url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/routeTables/{route_table_name}/routes/{route_name}?api-version=2021-03-01",
             success_codes=[200, 201],
             json=parameters,
         )
         if response_force_put["result"]:
             old_resource = response_get["ret"] if response_get["result"] else None
             return dict(
                 name=name,
@@ -99,15 +99,15 @@
                 comment="Would create azure.virtual_networks.routes",
             )
 
         if response_get["status"] == 404:
             # PUT operation to create a resource
             response_put = await hub.exec.request.json.put(
                 ctx,
-                url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/routeTables/{route_table_name}/routes/{route_name}?api-version=2021-03-01",
+                url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/routeTables/{route_table_name}/routes/{route_name}?api-version=2021-03-01",
                 success_codes=[200, 201],
                 json=parameters,
             )
 
             if not response_put["result"]:
                 hub.log.debug(
                     f"Could not create Routes {response_put['comment']} {response_put['ret']}"
@@ -180,29 +180,29 @@
                 - route_table_name: value
                 - route_name: value
     """
 
     subscription_id = ctx.acct.subscription_id
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/routeTables/{route_table_name}/routes/{route_name}?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/routeTables/{route_table_name}/routes/{route_name}?api-version=2021-03-01",
         success_codes=[200],
     )
     if response_get["result"]:
         if ctx.get("test", False):
             return dict(
                 name=name,
                 result=True,
                 comment="Would delete azure.virtual_networks.routes",
             )
 
         existing_resource = response_get["ret"]
         response_delete = await hub.exec.request.raw.delete(
             ctx,
-            url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/routeTables/{route_table_name}/routes/{route_name}?api-version=2021-03-01",
+            url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/routeTables/{route_table_name}/routes/{route_name}?api-version=2021-03-01",
             success_codes=[200, 202, 204],
         )
 
         if not response_delete["result"]:
             hub.log.debug(
                 f"Could not delete Routes {response_delete['comment']} {response_delete['ret']}"
             )
@@ -268,21 +268,21 @@
             "resourceGroups": "resource_group_name",
             "routeTables": "route_table_name",
             "routes": "route_name",
         }
     )
     async for route_tables_page_result in hub.tool.azure.request.paginate(
         ctx,
-        url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/providers/Microsoft.Network/routeTables?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/providers/Microsoft.Network/routeTables?api-version=2021-03-01",
         success_codes=[200],
     ):
         route_tables_list = route_tables_page_result.get("value", None)
         if route_tables_list:
             for route_table in route_tables_list:
-                url = f"{hub.exec.azure.URL}/{route_table.get('id')}/routes?api-version=2021-03-01"
+                url = f"{ctx.acct.endpoint_url}/{route_table.get('id')}/routes?api-version=2021-03-01"
                 response_get = await hub.exec.request.json.get(
                     ctx,
                     url=url,
                     success_codes=[200],
                 )
                 if response_get["result"]:
                     resource_list = response_get["ret"].get("value", list())
```

### Comparing `idem-azure-0.3.4/idem_azure/conf.py` & `idem-azure-0.4.0/idem_azure/conf.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/authorization/role_assignments.py` & `idem-azure-0.4.0/idem_azure/exec/azure/authorization/role_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/authorization/role_definitions.py` & `idem-azure-0.4.0/idem_azure/exec/azure/authorization/role_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/compute/log_analytics_workspace.py` & `idem-azure-0.4.0/idem_azure/exec/azure/compute/log_analytics_workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             "resourceGroups": "resource_group_name",
             "workspaces": "workspace_name",
         }
     )
 
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-12-01-preview",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-12-01-preview",
         success_codes=[200],
     )
     if not response_get["result"]:
         if response_get["status"] != 404:
             result["result"] = False
         result["comment"] = response_get["comment"]
         return result
```

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/compute/virtual_machines.py` & `idem-azure-0.4.0/idem_azure/exec/azure/compute/virtual_machines.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             "resourceGroups": "resource_group_name",
             "virtualMachines": "virtual_machine_name",
         }
     )
 
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2022-03-01",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2022-03-01",
         success_codes=[200],
     )
     if not response_get["result"]:
         if response_get["status"] != 404:
             result["result"] = False
         result["comment"] = response_get["comment"]
         return result
```

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/key_vault/vault.py` & `idem-azure-0.4.0/idem_azure/exec/azure/key_vault/vault.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/management_groups/management_groups.py` & `idem-azure-0.4.0/idem_azure/exec/azure/management_groups/management_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/network/firewall.py` & `idem-azure-0.4.0/idem_azure/exec/azure/network/firewall.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/network/firewall_policies.py` & `idem-azure-0.4.0/idem_azure/exec/azure/network/firewall_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             "subscriptions": "subscription_id",
             "firewallPolicies": "firewall_policy_name",
         }
     )
 
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2022-07-01",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2022-07-01",
         success_codes=[200],
     )
     if not response_get["result"]:
         if response_get["status"] != 404:
             result["result"] = False
         result["comment"] = response_get["comment"]
         return result
```

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/network/network_interfaces.py` & `idem-azure-0.4.0/idem_azure/exec/azure/network/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/network/network_security_groups.py` & `idem-azure-0.4.0/idem_azure/exec/azure/network/network_security_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             "networkSecurityGroups": "network_security_group_name",
             "subscriptions": "subscription_id",
         }
     )
 
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2022-07-01",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2022-07-01",
         success_codes=[200],
     )
     if not response_get["result"]:
         if response_get["status"] != 404:
             result["result"] = False
         result["comment"] = response_get["comment"]
         return result
@@ -105,15 +105,15 @@
             "resourceGroups": "resource_group_name",
             "networkSecurityGroups": "network_security_group_name",
             "subscriptions": "subscription_id",
         }
     )
     async for page_result in hub.tool.azure.request.paginate(
         ctx,
-        url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/providers/Microsoft.Network/networkSecurityGroups?api-version=2022-07-01",
+        url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/providers/Microsoft.Network/networkSecurityGroups?api-version=2022-07-01",
         success_codes=[200],
     ):
         resource_list = page_result.get("value")
         if resource_list:
             for resource in resource_list:
                 resource_id = resource["id"]
                 uri_parameter_values = hub.tool.azure.uri.get_parameter_value_in_dict(
```

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/network/public_ip_addresses.py` & `idem-azure-0.4.0/idem_azure/exec/azure/network/public_ip_addresses.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             "resourceGroups": "resource_group_name",
             "publicIPAddresses": "public_ip_address_name",
         }
     )
 
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-03-01",
         success_codes=[200],
     )
 
     if not response_get["result"]:
         if response_get["status"] != 404:
             result["result"] = False
         result["comment"] = response_get["comment"]
```

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/network/route_tables.py` & `idem-azure-0.4.0/idem_azure/exec/azure/network/route_tables.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/network/routes.py` & `idem-azure-0.4.0/idem_azure/exec/azure/network/routes.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/network/security_rules.py` & `idem-azure-0.4.0/idem_azure/exec/azure/network/security_rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                     resource_id: "/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/networkSecurityGroups/{network_security_group_name}/securityRules/{security_rule_name}"
 
     """
     result = dict(comment=[], result=True, ret=None)
 
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2022-07-01",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2022-07-01",
         success_codes=[200],
     )
     if not response_get["result"]:
         if response_get["status"] != 404:
             result["result"] = False
         result["comment"] = response_get["comment"]
         return result
@@ -84,15 +84,15 @@
 
 
     """
     result = dict(comment=[], result=True, ret=[])
     subscription_id = ctx.acct.subscription_id
     async for nsg_page_result in hub.tool.azure.request.paginate(
         ctx,
-        url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/providers/Microsoft.Network/networkSecurityGroups?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/providers/Microsoft.Network/networkSecurityGroups?api-version=2021-03-01",
         success_codes=[200],
     ):
         nsg_resource_list = nsg_page_result.get("value")
         if nsg_resource_list:
             for nsg_resource in nsg_resource_list:
                 if nsg_resource.get("properties") and nsg_resource.get(
                     "properties"
```

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/network/subnets.py` & `idem-azure-0.4.0/idem_azure/exec/azure/network/subnets.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             "virtualNetworks": "virtual_network_name",
             "subnets": "subnet_name",
         }
     )
 
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-06-01",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-06-01",
         success_codes=[200, 201],
     )
     if not response_get["result"]:
         if response_get["status"] != 404:
             result["result"] = False
         result["comment"] = response_get["comment"]
         return result
```

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/network/virtual_networks.py` & `idem-azure-0.4.0/idem_azure/exec/azure/network/virtual_networks.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/permission.py` & `idem-azure-0.4.0/idem_azure/exec/azure/permission.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/policy/policy_assignments.py` & `idem-azure-0.4.0/idem_azure/exec/azure/policy/policy_assignments.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                     raw: False
 
     """
     result = dict(comment=[], result=True, ret=None)
 
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-06-01",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-06-01",
         success_codes=[200],
     )
     if not response_get["result"]:
         if response_get["status"] != 404:
             result["result"] = False
         result["comment"] = response_get["comment"]
         return result
```

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/policy/policy_definitions.py` & `idem-azure-0.4.0/idem_azure/exec/azure/policy/policy_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/resource_management/resource_groups.py` & `idem-azure-0.4.0/idem_azure/exec/azure/resource_management/resource_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                     resource_id: "/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}"
 
     """
     result = dict(comment=[], result=True, ret=None)
 
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-04-01",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-04-01",
         success_codes=[200],
     )
     if not response_get["result"]:
         if response_get["status"] != 404:
             result["result"] = False
         result["comment"] = response_get["comment"]
         return result
```

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/storage_resource_provider/storage_accounts.py` & `idem-azure-0.4.0/idem_azure/exec/azure/storage_resource_provider/storage_accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             "resourceGroups": "resource_group_name",
             "storageAccounts": "account_name",
         }
     )
 
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-04-01",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-04-01",
         success_codes=[200],
     )
     if not response_get["result"]:
         if response_get["status"] != 404:
             result["result"] = False
         result["comment"] = response_get["comment"]
         return result
```

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/storage_resource_provider/storage_blob.py` & `idem-azure-0.4.0/idem_azure/exec/azure/storage_resource_provider/storage_blob.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             "storageAccounts": "account_name",
             "containerName": "container_name",
         }
     )
 
     response_get = await hub.exec.request.json.get(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-04-01",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-04-01",
         success_codes=[200],
     )
     if not response_get["result"]:
         if response_get["status"] != 404:
             result["result"] = False
         result["comment"] = response_get["comment"]
         return result
```

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/subscription/attach_subscriptions.py` & `idem-azure-0.4.0/idem_azure/exec/azure/subscription/attach_subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/exec/azure/subscription/subscriptions.py` & `idem-azure-0.4.0/idem_azure/exec/azure/subscription/subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/pop_create/azure/api_reference.py` & `idem-azure-0.4.0/idem_azure/pop_create/azure/api_reference.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/pop_create/azure/api_spec.py` & `idem-azure-0.4.0/idem_azure/pop_create/azure/api_spec.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/pop_create/azure/init.py` & `idem-azure-0.4.0/idem_azure/pop_create/azure/init.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/pop_create/azure/plugin.py` & `idem-azure-0.4.0/idem_azure/pop_create/azure/plugin.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/pop_create/azure/resource.py` & `idem-azure-0.4.0/idem_azure/pop_create/azure/resource.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/pop_create/azure/rest.py` & `idem-azure-0.4.0/idem_azure/pop_create/azure/rest.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/pop_create/azure/template.py` & `idem-azure-0.4.0/idem_azure/pop_create/azure/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     subscription_id = ctx.acct.subscription_id
     if resource_id is None:
         # TODO: This resource_id is not correct and it needs to be manually fixed to the correct one
         resource_id = {{ function.hardcoded.get_function }}
     # TODO: double check if the api version here is correct or not.
     response_get = {{ function.hardcoded.get_function }}(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-03-01",
         success_codes=[200],
     )
 
     if not response_get["result"]:
         if ctx.get("test", False):
             # Return a proposed state by Idem state --test
             result["new_state"] = hub.tool.azure.test_state_utils.generate_test_state(
@@ -122,15 +122,15 @@
 
         if response_get["status"] == 404:
             # PUT operation to create a resource
             # TODO Populate payload, please refer to hub.tool.azure.virtual_networks.conversion_utils.convert_present_to_raw_virtual_network()
             payload = {}
             response_put = {{ function.hardcoded.create_function }}(
                 ctx,
-                url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-03-01",
+                url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-03-01",
                 success_codes=[200, 201],
                 json=payload,
             )
 
             if not response_put["result"]:
                 hub.log.debug(f"Could not create {{ function.hardcoded.resource_name }} {response_put['comment']} {response_put['ret']}")
                 result["comment"] = (response_put["comment"], response_put["ret"])
@@ -170,15 +170,15 @@
             result["comment"] = (
                 f"azure.{{ function.hardcoded.create_ref }} '{name}' has no property need to be updated.",
             )
             return result
         result["comment"] = result["comment"] + new_payload["comment"]
         response_put = await hub.exec.request.json.put(
             ctx,
-            url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-03-01",
+            url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-03-01",
             success_codes=[200],
             json=new_payload["ret"],
         )
 
         if not response_put["result"]:
             hub.log.debug(
                 f"Could not update azure.{{ function.hardcoded.create_ref }} '{name}' {response_put['comment']} {response_put['ret']}"
@@ -197,15 +197,15 @@
     result = dict(comment="", old_state=None, new_state=None, name=name, result=True)
     subscription_id = ctx.acct.subscription_id
     # TODO: This resource_id is not correct and it needs to be manually fixed to the correct one
     resource_id = {{ function.hardcoded.get_function }}
     # TODO: double check if the api version here is correct or not.
     response_get = {{ function.hardcoded.get_function }}(
         ctx,
-        url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-03-01",
+        url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-03-01",
         success_codes=[200],
     )
     if response_get["result"]:
         # TODO: Add conversion_util function here. Please refer to hub.tool.azure.virtual_networks.conversion_utils.convert_raw_virtual_network_to_present
         result["old_state"] = {}
         if ctx.get("test", False):
             result["comment"] = ("Would delete azure.{{ function.hardcoded.create_ref }} '{name}'",)
```

### Comparing `idem-azure-0.3.4/idem_azure/reconcile/pending/azure.py` & `idem-azure-0.4.0/idem_azure/reconcile/pending/azure.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/authorization/role_assignments.py` & `idem-azure-0.4.0/idem_azure/states/azure/authorization/role_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/authorization/role_definitions.py` & `idem-azure-0.4.0/idem_azure/states/azure/authorization/role_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/compute/log_analytics_workspace.py` & `idem-azure-0.4.0/idem_azure/states/azure/compute/log_analytics_workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                 features=features,
                 sku=sku,
                 location=location,
                 tags=tags,
             )
             response_put = await hub.exec.request.json.put(
                 ctx,
-                url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-12-01-preview",
+                url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-12-01-preview",
                 success_codes=[200, 201],
                 json=payload,
             )
 
             if not response_put["result"]:
                 hub.log.debug(
                     f"Could not create azure.compute.log_analytics {response_put['comment']} {response_put['ret']}"
@@ -227,15 +227,15 @@
             result["comment"].append(
                 f"azure.compute.log_analytics_workspace '{name}' has no property need to be updated."
             )
             return result
         result["comment"] += new_payload["comment"]
         response_put = await hub.exec.request.json.put(
             ctx,
-            url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-12-01-preview",
+            url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-12-01-preview",
             success_codes=[200],
             json=new_payload["ret"],
         )
 
         if not response_put["result"]:
             hub.log.debug(
                 f"Could not update azure.compute.log_analytics_workspace {response_put['comment']} {response_put['ret']}"
@@ -321,15 +321,15 @@
             result["comment"].append(
                 f"Would delete azure.compute.log_analytics_workspace '{name}'"
             )
             return result
 
         response_delete = await hub.exec.request.raw.delete(
             ctx,
-            url=f"{hub.exec.azure.URL}{resource_id}?api-version=2021-12-01-preview",
+            url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-12-01-preview",
             success_codes=[200, 202, 204],
         )
         if not response_delete["result"]:
             hub.log.debug(
                 f"Could not delete azure.compute.log_analytics_workspace {response_delete['comment']} {response_delete['ret']}"
             )
             result["result"] = False
@@ -369,15 +369,15 @@
             "resourceGroups": "resource_group_name",
             "resourcegroups": "resource_group_name",
             "workspaces": "workspace_name",
         }
     )
     async for page_result in hub.tool.azure.request.paginate(
         ctx,
-        url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}"
+        url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}"
         f"/providers/Microsoft.OperationalInsights/workspaces?api-version=2021-12-01-preview",
         success_codes=[200],
     ):
         resource_list = page_result.get("value", None)
         if resource_list:
             for resource in resource_list:
                 resource_id = resource["id"]
```

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/compute/virtual_machines.py` & `idem-azure-0.4.0/idem_azure/states/azure/compute/virtual_machines.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,142 +1,187 @@
 """State module for managing Compute Virtual Machine."""
 import copy
+from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
 __contracts__ = ["resource"]
 __reconcile_wait__ = {"static": {"wait_in_seconds": 20}}
 
 
 async def present(
     hub,
     ctx,
     name: str,
-    resource_group_name: str,
-    virtual_machine_name: str,
     location: str,
-    virtual_machine_size: str,
     network_interface_ids: List[str],
     os_profile: make_dataclass(
         "OsProfile",
         [
             ("computer_name", str),
             ("admin_username", str),
-            ("admin_password", str),
-        ],
-    ),
-    storage_image_reference: make_dataclass(
-        "OsProfile",
-        [
-            ("image_sku", str),
-            ("image_publisher", str),
-            ("image_version", str),
-            ("image_offer", str),
+            ("admin_password", str, field(default=None)),
         ],
     ),
     storage_os_disk: make_dataclass(
         "StorageOsDisk",
         [
             ("disk_name", str),
-            ("disk_size_in_GB", int),
             ("disk_caching", str),
             ("disk_create_option", str),
-            ("disk_delete_option", str),
-            ("disk_id", str),
             ("storage_account_type", str),
+            ("disk_delete_option", str, field(default=None)),
+            ("disk_size_in_GB", int, field(default=None)),
+            ("disk_id", str, field(default=None)),
+            ("disk_image_vhd_uri", str, field(default=None)),
+            ("disk_os_type", str, field(default=None)),
+            ("disk_vhd_uri", str, field(default=None)),
+            ("write_accelerator_enabled", bool, field(default=None)),
         ],
     ),
+    resource_id: str = None,
+    subscription_id: str = None,
+    resource_group_name: str = None,
+    virtual_machine_name: str = None,
+    virtual_machine_size: str = None,
+    storage_image_reference: make_dataclass(
+        "ImageReference",
+        [
+            ("image_sku", str, field(default=None)),
+            ("image_publisher", str, field(default=None)),
+            ("image_version", str, field(default=None)),
+            ("image_offer", str, field(default=None)),
+            ("image_id", str, field(default=None)),
+            ("shared_gallery_image_id", str, field(default=None)),
+            ("community_gallery_image_id", str, field(default=None)),
+        ],
+    ) = None,
     storage_data_disks: List[
         make_dataclass(
             "StorageDataDisks",
             [
-                ("disk_name", str),
+                ("disk_create_option", str),
                 ("disk_size_in_GB", int),
                 ("disk_logical_unit_number", int),
-                ("disk_caching", str),
-                ("disk_create_option", str),
-                ("disk_delete_option", str),
-                ("disk_id", str),
-                ("storage_account_type", str),
+                ("disk_name", str, field(default=None)),
+                ("disk_caching", str, field(default=None)),
+                ("disk_delete_option", str, field(default=None)),
+                ("disk_id", str, field(default=None)),
+                ("storage_account_type", str, field(default=None)),
             ],
         )
     ] = None,
-    resource_id: str = None,
-    subscription_id: str = None,
     tags: Dict[str, str] = None,
+    plan: make_dataclass(
+        "Plan",
+        [
+            ("name", str),
+            ("publisher", str),
+            ("product", str),
+            ("promotion_code", str, field(default=None)),
+        ],
+    ) = None,
+    availability_set_id: str = None,
+    license_type: str = None,
 ) -> Dict:
     r"""Create or update Virtual Machines.
 
     Args:
         name(str): The identifier for this state.
-        resource_group_name(str): The name of the resource group.
-        resource_id(str, Optional): Virtual Machine resource id on Azure
-        virtual_machine_name(str): The name of the virtual machine.
         location(str): Resource location. Changing this forces a new resource to be created.
-        virtual_machine_size(str): Specifies the size of the Virtual Machine.
-        network_interface_ids(list[str]): A list of Network Interface IDs which should be associated with the Virtual Machine.
-        subscription_id(str, Optional): Subscription Unique id.
-        tags(dict[str, str], Optional): Resource tags.
-        os_profile(dict[str, Any]): Specifies the operating system settings used while creating the virtual machine.
+        network_interface_ids(List[str]): A list of Network Interface IDs which should be associated with the Virtual Machine.
+        os_profile(Dict[str, Any]): Specifies the operating system settings used while creating the virtual machine.
 
             * computer_name(str):
                 Specifies the name of the Virtual Machine.
             * admin_username(str):
                 Specifies the name of the local administrator account.
-            * admin_password(str):
+            * admin_password(str, Optional):
                 (Required for Windows, Optional for Linux) The password associated with the local administrator account.
-        storage_image_reference(dict[str, Any]): Specifies information about the image to use. Eg- platform images, marketplace images.
-
-            * image_sku(str):
-                Specifies the SKU of the image used to create the virtual machine. Changing this forces a new resource to be created.
-            * image_publisher(str):
-                Specifies the publisher of the image used to create the virtual machine. Changing this forces a new resource to be created.
-            * image_version(str):
-                Specifies the version of the image used to create the virtual machine. Changing this forces a new resource to be created.
-            * image_offer(str, Optional):
-                Specifies the offer of the image used to create the virtual machine. Changing this forces a new resource to be created.
-        storage_os_disk(dict[str, Any]): Specifies information about the operating system disk used by the virtual machine.
+        storage_os_disk(Dict[str, Any]): Specifies information about the operating system disk used by the virtual machine.
 
             * disk_name(str):
                 Specifies the name of the OS Disk.
+            * disk_caching(str, Optional):
+                Specifies the caching requirements for the OS Disk. Possible values include None, ReadOnly and ReadWrite.
             * disk_create_option(str):
                 Specifies how the OS Disk should be created. Possible values are Attach (managed disks only) and FromImage.
-            * storage_account_type(str, Optional):
+            * storage_account_type(str):
                 Specifies the type of Managed Disk which should be created. Possible values are Standard_LRS, StandardSSD_LRS or Premium_LRS.
-            * disk_caching(str, Optional):
-                Specifies the caching requirements for the OS Disk. Possible values include None, ReadOnly and ReadWrite.
-            * disk_size_in_GB(str, Optional):
-                Specifies the size of the OS Disk in gigabytes.
             * disk_delete_option(str, Optional):
                 Specifies how the OS Disk should be handled after VM deletion. Possible values are Detach and Delete.
+            * disk_size_in_GB(str, Optional):
+                Specifies the size of the OS Disk in gigabytes.
             * disk_id(str, Optional):
                 Specifies the ID of an existing Managed Disk which should be attached as the OS Disk of this Virtual Machine. If this is set then the create_option must be set to Attach.
-        storage_data_disks(list(dict[str, Any]), Optional): List of Data disks attached/added to a VM.
+            * disk_image_vhd_uri(str, Optional):
+                The source user image virtual hard disk. The virtual hard disk will be copied before being attached to the virtual machine. If SourceImage is provided, the destination virtual hard drive must not exist. Specifies the virtual hard disk's uri.
+            * disk_os_type(str, Optional):
+                This property allows you to specify the type of the OS that is included in the disk if creating a VM from user-image or a specialized VHD. Possible values are: Windows, Linux.
+            * disk_vhd_uri(str, Optional):
+                Specifies the virtual hard disk's uri.
+            * write_accelerator_enabled(bool, Optional):
+                Specifies whether writeAccelerator should be enabled or disabled on the disk.
+        resource_id(str, Optional): Virtual Machine resource id on Azure
+        subscription_id(str, Optional): Subscription Unique id.
+        resource_group_name(str, Optional): The name of the resource group.
+        virtual_machine_name(str, Optional): The name of the virtual machine.
+        virtual_machine_size(str, Optional): Specifies the size of the Virtual Machine.
+        storage_image_reference(Dict[str, Any], Optional): Specifies information about the image to use. Eg- platform images, marketplace images.
+
+            * image_sku(str, Optional):
+                Specifies the SKU of the image used to create the virtual machine. Changing this forces a new resource to be created.
+            * image_publisher(str, Optional):
+                Specifies the publisher of the image used to create the virtual machine. Changing this forces a new resource to be created.
+            * image_version(str, Optional):
+                Specifies the version of the image used to create the virtual machine. Changing this forces a new resource to be created.
+            * image_offer(str, Optional):
+                Specifies the offer of the image used to create the virtual machine. Changing this forces a new resource to be created.
+            * image_id(str, Optional):
+                Resource Id
+            * shared_gallery_image_id(str, Optional):
+                Specified the shared gallery image unique id for vm deployment. This can be fetched from shared gallery image GET call.
+            * community_gallery_image_id(str, Optional):
+                Specified the community gallery image unique id for vm deployment. This can be fetched from community gallery image GET call.
+        storage_data_disks(List[Dict[str, Any]], Optional): List of Data disks attached/added to a VM.
 
-            * disk_name(str):
-                The name of the Data Disk.
             * disk_create_option(str):
                 Specifies how the data disk should be created. Possible values are Attach, FromImage and Empty.
-            * disk_logical_unit_number(str):
+            * disk_size_in_GB(int):
+                Specifies the size of the data disk in gigabytes.
+            * disk_logical_unit_number(int):
                 Specifies the logical unit number of the data disk. This needs to be unique within all the Data Disks on the Virtual Machine.
-            * storage_account_type(str, Optional):
-                Specifies the type of managed disk to create. Possible values are either Standard_LRS, StandardSSD_LRS, Premium_LRS or UltraSSD_LRS.
+            * disk_name(str, Optional):
+                The name of the Data Disk.
             * disk_caching(str, Optional):
                 Specifies the caching requirements for the Data Disk. Possible values include None, ReadOnly and ReadWrite.
-            * disk_size_in_GB(str, Optional):
-                Specifies the size of the data disk in gigabytes.
             * disk_delete_option(str, Optional):
                 Specifies how the OS Disk should be handled after VM deletion. Possible values are Detach and Delete.
             * disk_id(str, Optional):
                 Specifies the ID of an Existing Managed Disk which should be attached to this Virtual Machine. When this field is set create_option must be set to Attach.
+            * storage_account_type(str, Optional):
+                Specifies the type of managed disk to create. Possible values are either Standard_LRS, StandardSSD_LRS, Premium_LRS or UltraSSD_LRS.
+        tags(Dict[str, str], Optional): Resource tags.
+        plan(Dict[str, str], Optional): Specifies information about the marketplace image used to create the virtual machine. This element is only used for marketplace images. Before you can use a marketplace image from an API, you must enable the image for programmatic use.  In the Azure portal, find the marketplace image that you want to use and then click **Want to deploy programmatically, Get Started ->**. Enter any required information and then click **Save**.
+
+            * name(str):
+                The plan ID.
+            * publisher(str):
+                The publisher ID.
+            * product(str):
+                Specifies the product of the image from the marketplace. This is the same value as Offer under the imageReference element.
+            * promotion_code(str, Optional):
+                The promotion code.
+        availability_set_id(str, Optional): Specifies id of the availability set that the virtual machine should be assigned to. Virtual machines specified in the same availability set are allocated to different nodes to maximize availability. Currently, a VM can only be added to availability set at creation time. The availability set to which the VM is being added should be under the same resource group as the availability set resource. An existing VM cannot be added to an availability set. This property cannot exist along with a non-null properties.virtualMachineScaleSet reference.
+        license_type(str, Optional): Specifies that the image or disk that is being used was licensed on-premises. Possible values for Windows Server operating system are: Windows_Client, Windows_Server. Possible values for Linux Server operating system are: RHEL_BYOS (for RHEL), SLES_BYOS (for SUSE). For more information, see Azure Hybrid Use Benefit for Windows Server and Azure Hybrid Use Benefit for Linux Server
 
     Returns:
-        Dict
+        Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
             resource_is_present:
               azure.compute.virtual_machines.present:
                 - name: my-vm
@@ -212,14 +257,17 @@
                     "location": location,
                     "network_interface_ids": network_interface_ids,
                     "storage_image_reference": storage_image_reference,
                     "storage_os_disk": storage_os_disk,
                     "storage_data_disks": storage_data_disks,
                     "os_profile": os_profile,
                     "resource_id": resource_id,
+                    "plan": plan,
+                    "availability_set_id": availability_set_id,
+                    "license_type": license_type,
                 },
             )
             result["comment"].append(
                 f"Would create azure.compute.virtual_machines '{name}'"
             )
             return result
 
@@ -230,14 +278,17 @@
                 virtual_machine_size=virtual_machine_size,
                 network_interface_ids=network_interface_ids,
                 storage_image_reference=storage_image_reference,
                 storage_os_disk=storage_os_disk,
                 storage_data_disks=storage_data_disks,
                 os_profile=os_profile,
                 tags=tags,
+                plan=plan,
+                availability_set_id=availability_set_id,
+                license_type=license_type,
             )
 
             response_put = await hub.exec.request.json.put(
                 ctx,
                 url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2022-03-01",
                 success_codes=[200, 201],
                 json=payload,
@@ -282,14 +333,17 @@
                     "virtual_machine_size": virtual_machine_size,
                     "storage_data_disks": storage_data_disks,
                     "network_interface_ids": network_interface_ids,
                     "storage_os_disk": storage_os_disk,
                     "os_profile": os_profile,
                     "storage_image_reference": storage_image_reference,
                     "tags": tags,
+                    "plan": plan,
+                    "availability_set_id": availability_set_id,
+                    "license_type": license_type,
                 },
             )
         )
         if ctx.get("test", False):
             if new_payload["ret"] is None:
                 result["new_state"] = copy.deepcopy(result["old_state"])
                 result["comment"].append(
@@ -353,25 +407,27 @@
         return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
-    resource_group_name: str,
-    virtual_machine_name: str,
+    resource_group_name: str = None,
+    virtual_machine_name: str = None,
     subscription_id: str = None,
+    resource_id: str = None,
 ) -> Dict:
     r"""Delete a Virtual Machine.
 
     Args:
         name(str): The identifier for this state.
-        resource_group_name(str): The name of the resource group.
-        virtual_machine_name(str): The name of the virtual machine.
+        resource_group_name(str, Optional): The name of the resource group.
+        virtual_machine_name(str, Optional): The name of the virtual machine.
         subscription_id(str, Optional): Subscription Unique id.
+        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
 
     Returns:
         Dict
 
     Examples:
         .. code-block:: sls
 
@@ -385,20 +441,24 @@
     result = {
         "name": name,
         "result": True,
         "old_state": None,
         "new_state": None,
         "comment": [],
     }
-    if subscription_id is None:
-        subscription_id = ctx.acct.subscription_id
-    resource_id = (
-        f"/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}"
-        f"/providers/Microsoft.Compute/virtualMachines/{virtual_machine_name}"
-    )
+
+    if not resource_id:
+        if subscription_id is None:
+            subscription_id = ctx.acct.subscription_id
+
+        resource_id = (
+            f"/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}"
+            f"/providers/Microsoft.Compute/virtualMachines/{virtual_machine_name}"
+        )
+
     response_get = await hub.exec.azure.compute.virtual_machines.get(
         ctx,
         resource_id=resource_id,
     )
     if not response_get["result"]:
         hub.log.debug(
             f"Could not get azure.compute.virtual_machines '{name}' {response_get['comment']} {response_get['ret']}"
```

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/key_vault/vault.py` & `idem-azure-0.4.0/idem_azure/states/azure/key_vault/vault.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/management_groups/management_groups.py` & `idem-azure-0.4.0/idem_azure/states/azure/management_groups/management_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/network/firewall.py` & `idem-azure-0.4.0/idem_azure/states/azure/network/firewall.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/network/firewall_policies.py` & `idem-azure-0.4.0/idem_azure/states/azure/network/firewall_policies.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/network/network_interfaces.py` & `idem-azure-0.4.0/idem_azure/states/azure/network/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/network/network_security_groups.py` & `idem-azure-0.4.0/idem_azure/states/azure/network/network_security_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             payload = hub.tool.azure.network.network_security_groups.convert_present_to_raw_network_security_groups(
                 location=location,
                 security_rules=security_rules,
                 tags=tags,
             )
             response_put = await hub.exec.request.json.put(
                 ctx,
-                url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/networkSecurityGroups/{network_security_group_name}?api-version=2022-07-01",
+                url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/networkSecurityGroups/{network_security_group_name}?api-version=2022-07-01",
                 success_codes=[200, 201],
                 json=payload,
             )
 
             if not response_put["result"]:
                 hub.log.debug(
                     f"Could not create Network Security Groups {response_put['comment']} {response_put['ret']}"
@@ -217,15 +217,15 @@
                     f"Would update azure.network.network_security_groups '{name}'"
                 )
                 return result
             else:
                 # PUT call to update the resource
                 response_put = await hub.exec.request.json.put(
                     ctx,
-                    url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/networkSecurityGroups/{network_security_group_name}?api-version=2022-07-01",
+                    url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/networkSecurityGroups/{network_security_group_name}?api-version=2022-07-01",
                     success_codes=[200, 201],
                     json=new_payload["ret"],
                 )
 
                 if not response_put["result"]:
                     hub.log.debug(
                         f"Could not update azure.network.network_security_groups {response_put['comment']} {response_put['ret']}"
@@ -313,15 +313,15 @@
             result["comment"].append(
                 f"Would delete azure.network.network_security_groups '{name}'"
             )
             return result
 
         response_delete = await hub.exec.request.raw.delete(
             ctx,
-            url=f"{hub.exec.azure.URL}{resource_id}?api-version=2022-07-01",
+            url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2022-07-01",
             success_codes=[200, 202, 204],
         )
 
         if not response_delete["result"]:
             hub.log.debug(
                 f"Could not delete azure.network.network_security_groups {response_delete['comment']} {response_delete['ret']}"
             )
```

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/network/public_ip_addresses.py` & `idem-azure-0.4.0/idem_azure/states/azure/network/public_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/network/route_tables.py` & `idem-azure-0.4.0/idem_azure/states/azure/network/route_tables.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/network/routes.py` & `idem-azure-0.4.0/idem_azure/states/azure/network/routes.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/network/security_rules.py` & `idem-azure-0.4.0/idem_azure/states/azure/network/security_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,15 +167,15 @@
                 destination_port_ranges=destination_port_ranges,
                 destination_address_prefix=destination_address_prefix,
                 destination_address_prefixes=destination_address_prefixes,
                 destination_application_security_groups=destination_application_security_groups,
             )
             response_put = await hub.exec.request.json.put(
                 ctx,
-                url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/networkSecurityGroups/{network_security_group_name}/securityRules/{security_rule_name}?api-version=2022-07-01",
+                url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/networkSecurityGroups/{network_security_group_name}/securityRules/{security_rule_name}?api-version=2022-07-01",
                 success_codes=[200, 201],
                 json=payload,
             )
 
             if not response_put["result"]:
                 hub.log.debug(
                     f"Could not create azure.network.security_rules {response_put['comment']} {response_put['ret']}"
@@ -236,15 +236,15 @@
                     f"Would update azure.network.security_rules '{name}'"
                 )
                 return result
             else:
                 # PUT call to update the resource
                 response_put = await hub.exec.request.json.put(
                     ctx,
-                    url=f"{hub.exec.azure.URL}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/networkSecurityGroups/{network_security_group_name}/securityRules/{security_rule_name}?api-version=2022-07-01",
+                    url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/networkSecurityGroups/{network_security_group_name}/securityRules/{security_rule_name}?api-version=2022-07-01",
                     success_codes=[200, 201],
                     json=new_payload["ret"],
                 )
 
                 if not response_put["result"]:
                     hub.log.debug(
                         f"Could not update azure.network.security_rules {response_put['comment']} {response_put['ret']}"
@@ -322,15 +322,15 @@
             result["comment"].append(
                 f"Would delete azure.network.security_rules '{name}'"
             )
             return result
 
         response_delete = await hub.exec.request.raw.delete(
             ctx,
-            url=f"{hub.exec.azure.URL}{resource_id}?api-version=2022-07-01",
+            url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2022-07-01",
             success_codes=[200, 202, 204],
         )
 
         if not response_delete["result"]:
             hub.log.debug(
                 f"Could not delete azure.network.security_rules {response_delete['comment']} {response_delete['ret']}"
             )
```

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/network/subnets.py` & `idem-azure-0.4.0/idem_azure/states/azure/network/subnets.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/network/virtual_networks.py` & `idem-azure-0.4.0/idem_azure/states/azure/storage_resource_provider/storage_blob.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,376 +1,364 @@
-"""State module for managing Virtual Network."""
+"""State module for managing storage blob."""
 import copy
-from dataclasses import field
-from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
-from typing import List
-
 
 __contracts__ = ["resource"]
 
 
 async def present(
     hub,
     ctx,
     name: str,
+    account_name: str,
+    container_name: str,
     resource_group_name: str,
-    virtual_network_name: str,
-    address_space: List,
-    location: str,
-    resource_id: str = None,
-    bgp_communities: Dict = None,
-    flow_timeout_in_minutes: int = None,
-    subnets: List[
-        make_dataclass(
-            "SubnetSet",
-            [
-                ("name", str, field(default=None)),
-                ("address_prefix", str, field(default=None)),
-                ("security_group_id", str, field(default=None)),
-                ("service_endpoints", List, field(default=None)),
-            ],
-        )
-    ] = None,
     subscription_id: str = None,
-    tags: Dict = None,
-) -> Dict:
-    r"""Create or update Virtual Networks.
-
-    Args:
-        name(str): The identifier for this state.
-        resource_group_name(str): The name of the resource group.
-        virtual_network_name(str): The name of the virtual network.
-        address_space(list): An array of IP address ranges that can be used by subnets of the virtual network.
-        location(str): Resource location. This field can not be updated.
-        resource_id(str, Optional): Virtual Network resource id on Azure
-        bgp_communities(dict, Optional): Bgp Communities sent over ExpressRoute with each route corresponding to a prefix in this VNET.
-        flow_timeout_in_minutes(int, Optional): The FlowTimeout value (in minutes) for the Virtual Network
-        subnets(list, Optional): List of Subnet in a virtual network resource.Each Subnet will have fields
-
-            * name(str):
-                The name of subnet.
-            * address_space(str):
-                Address space of the subnet.
-            * security_group_id(str, Optional):
-                The security group id.
-            * service_endpoints(list, Optional):
-                List of service endpoint.
-        subscription_id(str, Optional): Subscription Unique id.
-        tags(dict, Optional): Resource tags.
-
-    Returns:
-        dict
-
-    Examples:
-        .. code-block:: sls
-
-            my-vnet:
-              azure.network.virtual_networks.present:
-                - name: my-vnet
-                - resource_group_name: my-rg-1
-                - virtual_network_name: my-vnet-1
-                - location: westus
-                - flow_timeout_in_minutes: 15
-                - tags:
-                    my-tag-key: my-tag-value
-                - subnets:
-                    - name: subnet_name
-                      address_prefix: 10.0.0.0/26
-                      security_group_id: /subscriptions/subscription_id/resourceGroups/resource_group_name/providers/Microsoft.Network/networkSecurityGroups/network-security-group-name
-                      service_endpoints:
-                          - Microsoft.Storage
-                - address_space:
-                    - 10.0.0.0/26
-    """
+    resource_id: str = None,
+    default_encryption_scope: str = None,
+    deny_encryption_scope_override: bool = False,
+    has_immutability_policy: bool = False,
+    immutable_storage_with_versioning: bool = False,
+    metadata: Dict = None,
+    public_access: str = "Blob",
+    remaining_retention_days: int = 0,
+):
     result = {
         "name": name,
         "result": True,
         "old_state": None,
         "new_state": None,
         "comment": [],
     }
+
     if subscription_id is None:
         subscription_id = ctx.acct.subscription_id
+
     if resource_id is None:
-        resource_id = f"/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/virtualNetworks/{virtual_network_name}"
-    response_get = await hub.exec.azure.network.virtual_networks.get(
-        ctx,
-        resource_id=resource_id,
-        raw=True,
+        resource_id = (
+            f"/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Storage/"
+            f"storageAccounts/{account_name}/blobServices/default/containers/{container_name}"
+        )
+
+    response_get = await hub.exec.azure.storage_resource_provider.storage_blob.get(
+        ctx, resource_id=resource_id
     )
+
     if response_get["result"]:
-        if response_get["ret"] is None:
+        # 1. Resource is absent,
+        if not response_get["ret"]:
+            # Test mode
             if ctx.get("test", False):
                 # Return a proposed state by Idem state --test
                 result[
                     "new_state"
                 ] = hub.tool.azure.test_state_utils.generate_test_state(
                     enforced_state={},
                     desired_state={
                         "name": name,
                         "resource_group_name": resource_group_name,
-                        "virtual_network_name": virtual_network_name,
-                        "address_space": address_space,
-                        "tags": tags,
-                        "location": location,
-                        "resource_id": resource_id,
-                        "flow_timeout_in_minutes": flow_timeout_in_minutes,
-                        "bgp_communities": bgp_communities,
-                        "subnets": subnets,
+                        "account_name": account_name,
+                        "container_name": container_name,
                         "subscription_id": subscription_id,
+                        "resource_id": resource_id,
                     },
                 )
                 result["comment"].append(
-                    f"Would create azure.network.virtual_networks '{name}'"
+                    f"Would create azure.storage_resource_provider.blob '{name}'"
                 )
                 return result
+            # Create resource
             else:
                 # PUT operation to create a resource
-                payload = hub.tool.azure.network.virtual_networks.convert_present_to_raw_virtual_network(
-                    subscription_id=subscription_id,
-                    address_space=address_space,
-                    location=location,
-                    bgp_communities=bgp_communities,
-                    flow_timeout_in_minutes=flow_timeout_in_minutes,
-                    subnets=subnets,
-                    tags=tags,
-                )
+                payload = {
+                    "id": resource_id,
+                    "name": name,
+                    "container_name": container_name,
+                    "type": "Microsoft.Storage/storageAccounts/blobServices/containers",
+                    "properties": {
+                        "metadata": metadata,
+                        "deleted": False,
+                        "remainingRetentionDays": remaining_retention_days,
+                        "publicAccess": public_access,
+                        "hasImmutabilityPolicy": has_immutability_policy,
+                        "hasLegalHold": False,
+                    },
+                }
+
                 response_put = await hub.exec.request.json.put(
                     ctx,
-                    url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-03-01",
+                    url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-04-01",
                     success_codes=[200, 201],
                     json=payload,
                 )
 
-                if not response_put["result"]:
+                if response_put["status"] == 404:
+                    hub.log.debug(
+                        f"Could not create azure.storage_resource_provider.storage_blob {response_put['comment']} {response_put['ret']}"
+                    )
+                    result["result"] = False
+                    result["comment"] = [response_put["comment"], response_put["ret"]]
+                    return result
+                elif response_put["status"] == 202:
+                    get_response = {"result": False}
+                    while not get_response["result"]:
+                        get_response = await hub.exec.request.json.get(
+                            ctx,
+                            url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-04-01",
+                            success_codes=[200],
+                        )
+                    result[
+                        "new_state"
+                    ] = hub.tool.azure.storage_resource_provider.storage_blob.convert_raw_storage_blob_to_present(
+                        subscription_id=subscription_id,
+                        resource_grp_name=resource_group_name,
+                        account_name=account_name,
+                        result_dict=get_response["ret"],
+                    )
+
+                elif not response_put["result"] and response_put["status"] != 202:
                     hub.log.debug(
-                        f"Could not create azure.network.virtual_networks {response_put['comment']} {response_put['ret']}"
+                        f"Could not create azure.storage_resource_provider.storage_blob {response_put['comment']} {response_put['ret']}"
                     )
                     result["comment"] = [response_put["comment"], response_put["ret"]]
                     result["result"] = False
                     return result
 
-                result[
-                    "new_state"
-                ] = hub.tool.azure.network.virtual_networks.convert_raw_virtual_network_to_present(
-                    resource=response_put["ret"],
-                    idem_resource_name=name,
-                    resource_group_name=resource_group_name,
-                    virtual_network_name=virtual_network_name,
-                    resource_id=resource_id,
-                    subscription_id=subscription_id,
-                )
+                else:
+                    result_payload = get_create_payload(
+                        resource_id,
+                        name,
+                        container_name,
+                        metadata,
+                        resource_group_name,
+                        remaining_retention_days,
+                        public_access,
+                        has_immutability_policy,
+                    )
+                    result[
+                        "new_state"
+                    ] = hub.tool.azure.storage_resource_provider.storage_blob.convert_raw_storage_blob_to_present(
+                        subscription_id=subscription_id,
+                        resource_grp_name=resource_group_name,
+                        account_name=account_name,
+                        result_dict=result_payload,
+                    )
+
                 result["comment"].append(
-                    f"Created azure.network.virtual_networks '{name}'"
+                    f"Created azure.storage_resource_provider.storage_blob '{name}'"
                 )
                 return result
 
+        # 2. Resource is present,
         else:
             existing_resource = response_get["ret"]
+            # Create old and new payloads
             result[
                 "old_state"
-            ] = hub.tool.azure.network.virtual_networks.convert_raw_virtual_network_to_present(
-                resource=existing_resource,
-                idem_resource_name=name,
-                resource_group_name=resource_group_name,
-                virtual_network_name=virtual_network_name,
-                resource_id=resource_id,
+            ] = hub.tool.azure.storage_resource_provider.storage_blob.convert_raw_storage_blob_to_present(
                 subscription_id=subscription_id,
+                resource_grp_name=resource_group_name,
+                account_name=account_name,
+                result_dict=existing_resource,
             )
-            # Generate a new PUT operation payload with new values
-            new_payload = (
-                hub.tool.azure.network.virtual_networks.update_virtual_network_payload(
-                    subscription_id,
-                    existing_resource,
-                    {
-                        "address_space": address_space,
-                        "bgp_communities": bgp_communities,
-                        "flow_timeout_in_minutes": flow_timeout_in_minutes,
-                        "subnets": subnets,
-                        "tags": tags,
-                    },
-                )
+            changed_resources = {
+                "default_encryption_scope": default_encryption_scope,
+                "deny_encryption_scope_override": deny_encryption_scope_override,
+                "has_immutability_policy": has_immutability_policy,
+                "immutable_storage_with_versioning": immutable_storage_with_versioning,
+                "metadata": metadata,
+                "remaining_retention_days": remaining_retention_days,
+                "public_access": public_access,
+            }
+            # Generate PUT operation payload with new values
+            new_payload = hub.tool.azure.storage_resource_provider.storage_blob.update_storage_blob_payload(
+                existing_resource, changed_resources
             )
+
+            # Test mode
             if ctx.get("test", False):
+                # i. If no changed property found which needs to be updated.
                 if new_payload["ret"] is None:
                     result["new_state"] = copy.deepcopy(result["old_state"])
                     result["comment"].append(
-                        f"azure.network.virtual_networks '{name}' has no property need to be updated."
+                        f"azure.storage_resource_provider.storage_blob '{name}' has no property need to be updated."
                     )
+                # ii. Properties will be updated
                 else:
                     result[
                         "new_state"
-                    ] = hub.tool.azure.network.virtual_networks.convert_raw_virtual_network_to_present(
-                        resource=new_payload["ret"],
-                        idem_resource_name=name,
-                        resource_group_name=resource_group_name,
-                        virtual_network_name=virtual_network_name,
-                        resource_id=resource_id,
+                    ] = hub.tool.azure.storage_resource_provider.storage_blob.convert_raw_storage_blob_to_present(
                         subscription_id=subscription_id,
+                        resource_grp_name=resource_group_name,
+                        account_name=account_name,
+                        result_dict=new_payload["ret"],
                     )
                     result["comment"].append(
-                        f"Would update azure.network.virtual_networks '{name}'"
+                        f"Would update azure.storage_resource_provider.storage_blob '{name}'"
                     )
                 return result
-            # PUT operation to update a resource
-            if new_payload["ret"] is None:
+
+            # PUT operation nothing to update the resource
+            if new_payload["ret"] == None:
                 result["new_state"] = copy.deepcopy(result["old_state"])
                 result["comment"].append(
-                    f"azure.network.virtual_networks '{name}' has no property need to be updated."
+                    f"azure.storage_resource_provider.storage_blob '{name}' has no property need to be updated."
                 )
                 return result
-            result["comment"] += new_payload["comment"]
+
+            # Call PUT operation to update the resource
+            result["comment"] = result["comment"] + new_payload["comment"]
             response_put = await hub.exec.request.json.put(
                 ctx,
-                url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-03-01",
+                url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-04-01",
                 success_codes=[200],
                 json=new_payload["ret"],
             )
-
-            if not response_put["result"]:
+            if response_put["result"] == False:
                 hub.log.debug(
-                    f"Could not update azure.network.virtual_networks {response_put['comment']} {response_put['ret']}"
+                    f"Could not update azure.storage_resource_provider.storage_blob {response_put['comment']} {response_put['ret']}"
                 )
                 result["result"] = False
                 result["comment"] = [response_put["comment"], response_put["ret"]]
                 return result
 
             result[
                 "new_state"
-            ] = hub.tool.azure.network.virtual_networks.convert_raw_virtual_network_to_present(
-                resource=response_put["ret"],
-                idem_resource_name=name,
-                resource_group_name=resource_group_name,
-                virtual_network_name=virtual_network_name,
-                resource_id=resource_id,
+            ] = hub.tool.azure.storage_resource_provider.storage_blob.convert_raw_storage_blob_to_present(
                 subscription_id=subscription_id,
+                resource_grp_name=resource_group_name,
+                account_name=account_name,
+                result_dict=response_put["ret"],
             )
-            result["comment"].append(f"Updated azure.network.virtual_networks '{name}'")
-            return result
+            if result["old_state"] == result["new_state"]:
+                result["comment"].append(
+                    f"azure.storage_resource_provider.storage_blob '{name}' has no property need to be updated."
+                )
+                return result
 
+            result["comment"].append(
+                f"Updated azure.storage_resource_provider.storage_blob '{name}'"
+            )
+            return result
+    # 3. If issue occurred while finding resource
     else:
         hub.log.debug(
-            f"Could not get azure.network.virtual_networks {response_get['comment']} {response_get['ret']}"
+            f"Could not get azure.storage_resource_provider.storage_blob {response_get['comment']} {response_get['ret']}"
         )
         result["result"] = False
         result["comment"] = [response_get["comment"], response_get["ret"]]
         return result
 
 
 async def absent(
     hub,
     ctx,
     name: str,
     resource_group_name: str,
-    virtual_network_name: str,
+    account_name: str,
+    container_name: str,
     subscription_id: str = None,
-) -> Dict:
-    r"""Delete Virtual Networks.
+):
+    result = {
+        "name": name,
+        "result": True,
+        "old_state": None,
+        "new_state": None,
+        "comment": [],
+    }
 
-    Args:
-        name(str): The identifier for this state.
-        resource_group_name(str): The name of the resource group.
-        virtual_network_name(str): The name of the virtual network.
-        subscription_id(str, Optional): Subscription Unique id.
-
-    Returns:
-        dict
-
-    Examples:
-        .. code-block:: sls
-
-            resource_is_absent:
-              azure.network.virtual_networks.absent:
-                - name: value
-                - resource_group_name: value
-                - virtual_network_name: value
-    """
-    result = dict(name=name, result=True, comment=[], old_state=None, new_state=None)
     if subscription_id is None:
         subscription_id = ctx.acct.subscription_id
-    resource_id = f"/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Network/virtualNetworks/{virtual_network_name}"
-    response_get = await hub.exec.azure.network.virtual_networks.get(
+    resource_id = (
+        f"/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Storage/"
+        f"storageAccounts/{account_name}/blobServices/default/containers/{container_name}"
+    )
+    response_get = await hub.exec.azure.storage_resource_provider.storage_blob.get(
         ctx,
         resource_id=resource_id,
-        raw=True,
     )
-    if response_get["result"]:
-        if response_get["ret"]:
-            result[
-                "old_state"
-            ] = hub.tool.azure.network.virtual_networks.convert_raw_virtual_network_to_present(
-                resource=response_get["ret"],
-                idem_resource_name=name,
-                resource_group_name=resource_group_name,
-                virtual_network_name=virtual_network_name,
-                resource_id=resource_id,
-                subscription_id=subscription_id,
-            )
-            if ctx.get("test", False):
-                result["comment"].append(
-                    f"Would delete azure.network.virtual_networks '{name}'"
-                )
-                return result
-            response_delete = await hub.exec.request.raw.delete(
-                ctx,
-                url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-03-01",
-                success_codes=[200, 202, 204],
-            )
-
-            if not response_delete["result"]:
-                hub.log.debug(
-                    f"Could not delete azure.network.virtual_networks '{name}' {response_delete['comment']} {response_delete['ret']}"
-                )
-                result["result"] = False
-                result["comment"] = [response_delete["comment"], response_delete["ret"]]
-                return result
-
-            result["comment"].append(f"Deleted azure.network.virtual_networks '{name}'")
-            return result
-        else:
-            # If Azure returns 'Not Found' error, it means the resource has been absent.
-            result["comment"].append(
-                f"azure.network.virtual_networks '{name}' already absent"
-            )
-            return result
-    else:
+    if not response_get["result"]:
         hub.log.debug(
-            f"Could not get azure.network.virtual_networks '{name}' {response_get['comment']} {response_get['ret']}"
+            f"Could not get azure.storage_resource_provider.storage_blob '{name}' {response_get['comment']} {response_get['ret']}"
         )
         result["result"] = False
         result["comment"] = [response_get["comment"], response_get["ret"]]
-    return result
+        return result
 
+    if response_get["ret"]:
+        result["old_state"] = response_get["ret"]
+        result["old_state"]["name"] = name
 
-async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
+        if ctx.get("test", False):
+            result["comment"].append(
+                f"Would delete azure.storage_resource_provider.storage_blob '{name}'"
+            )
+            return result
+        response_delete = await hub.exec.request.raw.delete(
+            ctx,
+            url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-06-01",
+            success_codes=[200, 202],
+        )
 
-    Lists all Virtual Networks under the same subscription
+        if not response_delete["result"]:
+            hub.log.debug(
+                f"Could not delete azure.storage_resource_provider.storage_blob {response_delete['comment']} {response_delete['ret']}"
+            )
+            result["result"] = False
+            result["comment"] = [response_delete["comment"], response_delete["ret"]]
+            return result
 
-    Returns:
-        Dict[str, Any]
+        result["comment"].append(
+            f"Deleted azure.storage_resource_provider.storage_blob '{name}'"
+        )
+        return result
+    else:
+        # If Azure returns 'Not Found' error, it means the resource has been absent.
+        result["comment"].append(
+            f"azure.storage_resource_provider.storage_blob '{name}' already absent"
+        )
+        return result
 
-    Examples:
-        .. code-block:: bash
 
-            $ idem describe azure.network.virtual_networks
-    """
+async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     result = {}
-    ret_list = await hub.exec.azure.network.virtual_networks.list(ctx)
+    ret_list = await hub.exec.azure.storage_resource_provider.storage_blob.list(ctx)
     if not ret_list["ret"]:
-        hub.log.debug(
-            f"Could not describe network virtual_networks {ret_list['comment']}"
-        )
+        hub.log.debug(f"Could not describe storage account {ret_list['comment']}")
         return result
-
     for resource in ret_list["ret"]:
         resource_id = resource["resource_id"]
         result[resource_id] = {
-            "azure.network.virtual_networks.present": [
+            "azure.storage_resource_provider.storage_blob.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
-
     return result
+
+
+def get_create_payload(
+    p_resource_id,
+    p_name,
+    p_container_name,
+    p_metadata,
+    resource_group_name,
+    p_remaining_retention_days,
+    p_public_access,
+    p_has_immutability_policy,
+):
+    return {
+        "id": p_resource_id,
+        "name": p_name,
+        "container_name": p_container_name,
+        "resource_group_name": resource_group_name,
+        "type": "Microsoft.Storage/storageAccounts/blobServices/containers",
+        "properties": {
+            "metadata": p_metadata,
+            "deleted": False,
+            "remainingRetentionDays": p_remaining_retention_days,
+            "publicAccess": p_public_access,
+            "hasImmutabilityPolicy": p_has_immutability_policy,
+            "hasLegalHold": False,
+        },
+    }
```

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/policy/policy_assignments.py` & `idem-azure-0.4.0/idem_azure/states/azure/policy/policy_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/policy/policy_definitions.py` & `idem-azure-0.4.0/idem_azure/states/azure/policy/policy_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/resource_management/resource_groups.py` & `idem-azure-0.4.0/idem_azure/states/azure/resource_management/resource_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/storage_resource_provider/storage_accounts.py` & `idem-azure-0.4.0/idem_azure/states/azure/storage_resource_provider/storage_accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 async def present(
     hub,
     ctx,
     name: str,
     resource_group_name: str,
     account_name: str,
     location: str,
-    sku_tier: str,
     sku_name: str,
+    sku_tier: str = None,
     account_kind: str = None,
     cross_tenant_replication_enabled: bool = None,
     access_tier: str = None,
     edge_zone: str = None,
     enable_https_traffic_only: bool = None,
     min_tls_version: str = None,
     allow_blob_public_access: bool = None,
@@ -36,15 +36,22 @@
         [
             ("name", str),
             ("use_subdomain", bool, field(default=None)),
         ],
     ) = None,
     customer_managed_key: make_dataclass(
         "CustomerManagedKey",
-        [("key_vault_key_id", str), ("user_assigned_identity_id", str)],
+        [
+            ("user_assigned_identity_id", str),
+            ("key_vault_key_id", str, field(default=None)),
+            ("federated_identity_client_id", str, field(default=None)),
+            ("key_name", str, field(default=None)),
+            ("key_vault_uri", str, field(default=None)),
+            ("key_version", str, field(default=None)),
+        ],
     ) = None,
     identity: make_dataclass(
         "Identity",
         [
             ("type", str),
             ("user_assigned_identities", Dict[str, str], field(default=None)),
         ],
@@ -87,14 +94,15 @@
                         ("domain_guid", str),
                         ("forest_name", str),
                         ("netbios_domain_name", str),
                     ],
                 ),
                 field(default=None),
             ),
+            ("default_share_permission", str, field(default=None)),
         ],
     ) = None,
     routing: make_dataclass(
         "Routing",
         [
             ("publish_internet_endpoints", bool, field(default=None)),
             ("publish_microsoft_endpoints", bool, field(default=None)),
@@ -103,14 +111,16 @@
     ) = None,
     encryption_service: make_dataclass(
         "EncryptionService",
         [
             ("encryption_key_source", str, field(default="Microsoft.Storage")),
             ("queue_encryption_key_type", str, field(default=None)),
             ("table_encryption_key_type", str, field(default=None)),
+            ("blob_encryption_key_type", str, field(default=None)),
+            ("file_encryption_key_type", str, field(default=None)),
         ],
     ) = None,
     require_infrastructure_encryption: bool = None,
     immutability_policy: make_dataclass(
         "ImmutabilityPolicy",
         [
             ("allow_protected_append_writes", bool),
@@ -121,93 +131,126 @@
     sas_policy: make_dataclass(
         "SasPolicy",
         [
             ("expiration_period", str),
             ("expiration_action", str, field(default="Log")),
         ],
     ) = None,
+    key_policy: make_dataclass(
+        "KeyPolicy",
+        [
+            ("key_expiration_period_in_days", int),
+        ],
+    ) = None,
     allowed_copy_scope: str = None,
     sftp_enabled: bool = None,
     tags: Dict[str, str] = None,
     subscription_id: str = None,
     resource_id: str = None,
 ) -> Dict:
     r"""Create or update Storage Accounts.
 
     Args:
         name(str): The identifier for this state.
         account_name(str): The name of the storage account within the specified resource group. Storage account names
             must be between 3 and 24 characters in length and use numbers and lower-case letters only.
         resource_group_name(str): The name of the resource group.
         location(str): Specifies the supported Azure location where the resource exists.
-        sku_tier(str): The SKU tier
-        sku_name(str): The SKU name
+        sku_name(str): The SKU name.
+        sku_tier(str, Optional): The SKU tier.
         account_kind(str, Optional): Defines the Kind of account.
         cross_tenant_replication_enabled(bool, Optional): Allow or disallow cross AAD tenant object replication
-        access_tier(str, Optional): Required for storage accounts where account_kind = BlobStorage. The access tier is used for billing
+        access_tier(str, Optional): Required for storage accounts where account_kind = BlobStorage. The access tier is used for billing.
         edge_zone(str, Optional): Specifies the Edge Zone within the Azure Region where this Storage Account should exist.
         enable_https_traffic_only(bool, Optional): Boolean flag which forces HTTPS if enabled.
         min_tls_version(str, Optional): The minimum supported TLS version for the storage account.
         allow_blob_public_access(bool, Optional): Allow or disallow nested items within this Account to opt into being public.
         allow_shared_key_access(bool, Optional): Indicates whether the storage account permits requests to be authorized with the account access key via Shared Key.
         public_network_access(str, Optional): Allow or disallow public network access to Storage Account. Value is optional but if passed in, must be 'Enabled' or 'Disabled'.
         default_to_oauth_authentication(bool, Optional): A boolean flag which indicates whether the default authentication is OAuth or not. The default interpretation is false for this property.
         is_hns_enabled(bool, Optional): Account HierarchicalNamespace enabled if sets to true.
         nfsv3_enabled(bool, Optional): NFS 3.0 protocol support enabled if set to true.
         custom_domain(dict[str, Any], Optional): User domain assigned to the storage account.
 
             * name(str):
-                The Custom Domain Name to use for the Storage Account
+                The Custom Domain Name to use for the Storage Account.
             * use_subdomain(bool, Optional):
-                Indicates whether indirect CName validation is enabled. Default value is false
-        customer_managed_key(dict[str, Any], Optional): Combination of Key vault key id and user assigned id
+                Indicates whether indirect CName validation is enabled. Default value is false.
+        customer_managed_key(dict[str, Any], Optional): Combination of Key vault key id and user assigned id.
 
             * user_assigned_identity_id(str):
-                User Assigned Identity id
-            * key_vault_key_id(str):
+                User Assigned Identity id.
+            * key_vault_key_id(str, Optional):
                 The object identifier of the current versioned Key Vault Key in use.
+            * federated_identity_client_id(str, Optional):
+                ClientId of the multi-tenant application to be used in conjunction with the user-assigned identity for cross-tenant customer-managed-keys server-side encryption on the storage account.
+            * key_name(str, Optional):
+                The name of KeyVault key.
+            * key_vault_uri(str, Optional):
+                The Uri of KeyVault.
+            * key_version(str, Optional):
+               The version of KeyVault key.
         identity(dict[str, Any], Optional): The identity of the resource.
 
             * type(str):
-                The identity type. Possible values are SystemAssigned, UserAssigned, SystemAssigned, UserAssigned
+                The identity type. Possible values are SystemAssigned, UserAssigned, SystemAssigned, UserAssigned.
             * user_assigned_identities(dict[str, Any], Optional):
-                Key value pairs that describe the set of User Assigned identities that will be used with this storage account
-        network_rules(dict[str, Any], Optional): Network rule set
+                Key value pairs that describe the set of User Assigned identities that will be used with this storage account.
+        network_rules(dict[str, Any], Optional): Network rule set.
 
             * default_action(str):
-                Specifies the default action of allow or deny when no other rules match. Valid options are Deny or Allow
+                Specifies the default action of allow or deny when no other rules match. Valid options are Deny or Allow.
             * bypass(str, Optional):
-                Specifies whether traffic is bypassed for Logging/Metrics/AzureServices. Possible values are any combination of Logging|Metrics|AzureServices
+                Specifies whether traffic is bypassed for Logging/Metrics/AzureServices. Possible values are any combination of Logging|Metrics|AzureServices.
             * ip_rule_values(list, Optional):
                 List of IP or IP range in CIDR format. Only IPV4 address is allowed.
             * virtual_network_subnet_ids(list, Optional):
                 A list of resource ids of virtual network subnets.
             * resource_access_rules(dict[str, Any], Optional):
-                The resource access rules
+                The resource access rules.
         large_file_shares_state(str, Optional): Allow large file shares if sets to enable.
         azure_files_authentication(dict[str, Any], Optional): Provides the identity based authentication settings for Azure Files.
 
             * directory_service_options(str):
                 The directory service to be used. Possible values are AADDS, AD and AADKERB.
             * active_directory_properties(dict[str, Any], Optional):
                 Required if directoryServiceOptions are AD, optional if they are AADKERB.
+
+                * azure_storage_sid(str):
+                    Specifies the security identifier (SID) for Azure Storage.
+                * domain_name(str):
+                    Specifies the primary domain that the AD DNS server is authoritative for.
+                * domain_sid(str):
+                    Specifies the security identifier (SID).
+                * domain_guid(str):
+                    Specifies the domain GUID.
+                * forest_name(str):
+                   Specifies the Active Directory forest to get.
+                * netbios_domain_name(str):
+                    Specifies the NetBIOS domain name.
+            * default_share_permission(str):
+                Default share permission for users using Kerberos authentication if RBAC role is not assigned.
         routing(dict[str, Any], Optional): Maintains information about the network routing choice opted by the user for data transfer.
 
             * publish_internet_endpoints(bool, Optional):
                 A boolean flag which indicates whether internet routing storage endpoints are to be published.
             * publish_microsoft_endpoints(bool, Optional):
                 A boolean flag which indicates whether microsoft routing storage endpoints are to be published.
             * routing_choice(str, Optional):
                 Routing Choice defines the kind of network routing opted by the user.
-        encryption_service(dict[str, Any], Optional): Encryption details
+        encryption_service(dict[str, Any], Optional): Encryption details.
 
             * queue_encryption_key_type(str, Optional):
                 The encryption type of the queue service.
             * table_encryption_key_type(str, Optional):
                 The encryption type of the table service.
+            * blob_encryption_key_type(str, Optional):
+                The encryption type of the blob service.
+            * file_encryption_key_type(str, Optional):
+                The encryption type of the file service.
             * encryption_key_source(str, Optional):
                 The encryption keySource (provider)
         require_infrastructure_encryption(bool, Optional): A boolean indicating whether or not the service applies a secondary layer of encryption with platform managed keys for data at rest.
         immutability_policy(dict[str, Any], Optional): This argument specifies the default account-level immutability policy which is inherited and applied to objects.
 
             * allow_protected_append_writes(bool):
                 This property can only be changed for disabled and unlocked time-based retention policies. When enabled, new blocks can be written to an append blob while
@@ -221,33 +264,39 @@
             * period_since_creation_in_days(int): The immutability period for the blobs in the container since the policy creation, in days.
         sas_policy(dict[str, Any], Optional): SasPolicy assigned to the storage account.
 
             * expiration_period(str, Optional):
                 The SAS expiration period, DD.HH:MM:SS.
             * expiration_action(str, Optional):
                 The SAS expiration action. Valid value is Log.
+        key_policy(dict[str, Any], Optional): KeyPolicy assigned to the storage account.
 
+            * key_expiration_period_in_days(int, Optional):
+                The key expiration period in days.
         allowed_copy_scope(str, Optional): Restrict copy to and from Storage Accounts within an AAD tenant or with Private Links to the same VNet.
-        sftp_enabled(bool, Optional): Enables Secure File Transfer Protocol, if set to true
+        sftp_enabled(bool, Optional): Enables Secure File Transfer Protocol, if set to true.
         tags(dict[str, str], Optional): The resource tags.
         subscription_id(str, Optional): Subscription Unique id.
         resource_id(str, Optional): Storage account resource id on Azure.
 
     Returns:
         dict
 
     Examples:
         .. code-block:: sls
 
             resource_is_present:
               azure.storage_resource_provider.storage_accounts.present:
-                - name: value
                 - resource_group_name: value
                 - account_name: value
+                - location: value
+                - sku_name: value
+                - sku_tier: value
     """
+
     result = {
         "name": name,
         "result": True,
         "old_state": None,
         "new_state": None,
         "comment": [],
     }
@@ -296,14 +345,15 @@
                         "large_file_shares_state": large_file_shares_state,
                         "azure_files_authentication": azure_files_authentication,
                         "routing": routing,
                         "encryption_service": encryption_service,
                         "require_infrastructure_encryption": require_infrastructure_encryption,
                         "immutability_policy": immutability_policy,
                         "sas_policy": sas_policy,
+                        "key_policy": key_policy,
                         "allowed_copy_scope": allowed_copy_scope,
                         "sftp_enabled": sftp_enabled,
                         "tags": tags,
                         "resource_id": resource_id,
                         "subscription_id": subscription_id,
                     },
                 )
@@ -336,14 +386,15 @@
                     large_file_shares_state=large_file_shares_state,
                     azure_files_authentication=azure_files_authentication,
                     routing=routing,
                     encryption_service=encryption_service,
                     require_infrastructure_encryption=require_infrastructure_encryption,
                     immutability_policy=immutability_policy,
                     sas_policy=sas_policy,
+                    key_policy=key_policy,
                     allowed_copy_scope=allowed_copy_scope,
                     sftp_enabled=sftp_enabled,
                     tags=tags,
                 )
                 response_put = await hub.exec.request.json.put(
                     ctx,
                     url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-04-01",
@@ -435,14 +486,15 @@
                     "encryption_service": encryption_service,
                     # "queue_encryption_key_type": queue_encryption_key_type,
                     # "table_encryption_key_type": table_encryption_key_type,
                     # "encryption_key_source": encryption_key_source,
                     "require_infrastructure_encryption": require_infrastructure_encryption,
                     "immutability_policy": immutability_policy,
                     "sas_policy": sas_policy,
+                    "key_policy": key_policy,
                     "allowed_copy_scope": allowed_copy_scope,
                     "sftp_enabled": sftp_enabled,
                     "tags": tags,
                 },
             )
 
             if ctx.get("test", False):
```

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/storage_resource_provider/storage_blob.py` & `idem-azure-0.4.0/idem_azure/states/azure/subscription/subscriptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,364 +1,301 @@
-"""State module for managing storage blob."""
+"""State module for managing Subscription."""
 import copy
 from typing import Any
 from typing import Dict
 
 __contracts__ = ["resource"]
+__reconcile_wait__ = {"static": {"wait_in_seconds": 20}}
 
 
 async def present(
     hub,
     ctx,
     name: str,
-    account_name: str,
-    container_name: str,
-    resource_group_name: str,
-    subscription_id: str,
+    alias: str,
+    billing_scope: str,
+    display_name: str,
+    workload: str,
     resource_id: str = None,
-    default_encryption_scope: str = None,
-    deny_encryption_scope_override: bool = False,
-    has_immutability_policy: bool = False,
-    immutable_storage_with_versioning: bool = False,
-    metadata: Dict = None,
-    public_access: str = "Blob",
-    remaining_retention_days: int = 0,
-):
+) -> Dict:
+    r"""Create or update Subscription.
+
+    Args:
+        name(str): The identifier for this state.
+        alias(str): The alias name of the subscription to create or update. Can include alphanumeric,
+          underscore, parentheses, hyphen, period (except at end), and Unicode characters that match
+          the allowed characters.Regex pattern: ^[-\w\._\(\)]+$.
+        billing_scope(str): billing scope associated with billing account id and enrollment account id to create subscription
+        display_name(str): subscription display name
+        workload(str): type of workload where subscription needs to be created. Can be Production/DevTest
+        resource_id(str, Optional): resource unique id
+
+    Returns:
+        Dict
+
+    Examples:
+        .. code-block:: sls
+
+            resource_present:
+              azure.subscription.subscriptions.present:
+                - name: create_subscription_3
+                - alias: dupSubTest
+                - billing_scope: /providers/Microsoft.Billing/billingAccounts/{billingAccountID}/enrollmentAccounts/{enrollmentAccountId}}
+                - display_name: Subscription Display Name
+                - workload: Production
+    """
     result = {
         "name": name,
         "result": True,
         "old_state": None,
         "new_state": None,
         "comment": [],
     }
 
-    if subscription_id is None:
-        subscription_id = ctx.acct.subscription_id
-
     if resource_id is None:
-        resource_id = (
-            f"/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Storage/"
-            f"storageAccounts/{account_name}/blobServices/default/containers/{container_name}"
-        )
-
-    response_get = await hub.exec.azure.storage_resource_provider.storage_blob.get(
-        ctx, resource_id=resource_id
+        resource_id = f"/providers/Microsoft.Subscription/aliases/{alias}"
+    response_get = await hub.exec.azure.subscription.subscriptions.get(
+        ctx, resource_id=resource_id, raw=True
     )
+    hub.log.debug(f"Get Subscription details : {response_get}")
 
-    if response_get["result"]:
-        # 1. Resource is absent,
-        if not response_get["ret"]:
-            # Test mode
-            if ctx.get("test", False):
-                # Return a proposed state by Idem state --test
-                result[
-                    "new_state"
-                ] = hub.tool.azure.test_state_utils.generate_test_state(
-                    enforced_state={},
-                    desired_state={
-                        "name": name,
-                        "resource_group_name": resource_group_name,
-                        "account_name": account_name,
-                        "container_name": container_name,
-                        "subscription_id": subscription_id,
-                        "resource_id": resource_id,
-                    },
-                )
-                result["comment"].append(
-                    f"Would create azure.storage_resource_provider.blob '{name}'"
-                )
-                return result
-            # Create resource
-            else:
-                # PUT operation to create a resource
-                payload = {
-                    "id": resource_id,
-                    "name": name,
-                    "container_name": container_name,
-                    "type": "Microsoft.Storage/storageAccounts/blobServices/containers",
-                    "properties": {
-                        "metadata": metadata,
-                        "deleted": False,
-                        "remainingRetentionDays": remaining_retention_days,
-                        "publicAccess": public_access,
-                        "hasImmutabilityPolicy": has_immutability_policy,
-                        "hasLegalHold": False,
-                    },
-                }
-
-                response_put = await hub.exec.request.json.put(
-                    ctx,
-                    url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-04-01",
-                    success_codes=[200, 201],
-                    json=payload,
-                )
-
-                if response_put["status"] == 404:
-                    hub.log.debug(
-                        f"Could not create azure.storage_resource_provider.storage_blob {response_put['comment']} {response_put['ret']}"
-                    )
-                    result["result"] = False
-                    result["comment"] = [response_put["comment"], response_put["ret"]]
-                    return result
-                elif response_put["status"] == 202:
-                    get_response = {"result": False}
-                    while not get_response["result"]:
-                        get_response = await hub.exec.request.json.get(
-                            ctx,
-                            url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-04-01",
-                            success_codes=[200],
-                        )
-                    result[
-                        "new_state"
-                    ] = hub.tool.azure.storage_resource_provider.storage_blob.convert_raw_storage_blob_to_present(
-                        subscription_id=subscription_id,
-                        resource_grp_name=resource_group_name,
-                        account_name=account_name,
-                        result_dict=get_response["ret"],
-                    )
-
-                elif not response_put["result"] and response_put["status"] != 202:
-                    hub.log.debug(
-                        f"Could not create azure.storage_resource_provider.storage_blob {response_put['comment']} {response_put['ret']}"
-                    )
-                    result["comment"] = [response_put["comment"], response_put["ret"]]
-                    result["result"] = False
-                    return result
-
-                else:
-                    result_payload = get_create_payload(
-                        resource_id,
-                        name,
-                        container_name,
-                        metadata,
-                        resource_group_name,
-                        remaining_retention_days,
-                        public_access,
-                        has_immutability_policy,
-                    )
-                    result[
-                        "new_state"
-                    ] = hub.tool.azure.storage_resource_provider.storage_blob.convert_raw_storage_blob_to_present(
-                        subscription_id=subscription_id,
-                        resource_grp_name=resource_group_name,
-                        account_name=account_name,
-                        result_dict=result_payload,
-                    )
-
-                result["comment"].append(
-                    f"Created azure.storage_resource_provider.storage_blob '{name}'"
-                )
-                return result
+    if not response_get["result"]:
+        hub.log.debug(
+            f"Could not get azure.subscriptions.subscription '{name}' {response_get['comment']} {response_get['ret']}"
+        )
+        result["result"] = False
+        result["comment"] = [response_get["comment"], response_get["ret"]]
+        return result
 
-        # 2. Resource is present,
+    if not response_get["ret"]:
+        if ctx.get("test", False):
+            # Return a proposed state by Idem state --test
+            result["new_state"] = hub.tool.azure.test_state_utils.generate_test_state(
+                enforced_state={},
+                desired_state={
+                    "name": name,
+                    "alias": alias,
+                    "display_name": display_name,
+                    "subscription_id": "subscription_id_known_after_present",
+                    "resource_id": resource_id,
+                },
+            )
+            result["comment"].append(
+                f"Would create azure.subscription.subscriptions '{name}'"
+            )
+            return result
         else:
-            existing_resource = response_get["ret"]
-            # Create old and new payloads
-            result[
-                "old_state"
-            ] = hub.tool.azure.storage_resource_provider.storage_blob.convert_raw_storage_blob_to_present(
-                subscription_id=subscription_id,
-                resource_grp_name=resource_group_name,
-                account_name=account_name,
-                result_dict=existing_resource,
+            # PUT operation to create subscription
+            payload = hub.tool.azure.subscription.subscriptions.convert_present_to_raw_subscription(
+                billing_scope=billing_scope,
+                display_name=display_name,
+                workload=workload,
             )
-            changed_resources = {
-                "default_encryption_scope": default_encryption_scope,
-                "deny_encryption_scope_override": deny_encryption_scope_override,
-                "has_immutability_policy": has_immutability_policy,
-                "immutable_storage_with_versioning": immutable_storage_with_versioning,
-                "metadata": metadata,
-                "remaining_retention_days": remaining_retention_days,
-                "public_access": public_access,
-            }
-            # Generate PUT operation payload with new values
-            new_payload = hub.tool.azure.storage_resource_provider.storage_blob.update_storage_blob_payload(
-                existing_resource, changed_resources
+            response_put = await hub.exec.request.json.put(
+                ctx,
+                url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2020-09-01",
+                success_codes=[200, 201],
+                json=payload,
             )
-
-            # Test mode
-            if ctx.get("test", False):
-                # i. If no changed property found which needs to be updated.
-                if new_payload["ret"] is None:
-                    result["new_state"] = copy.deepcopy(result["old_state"])
-                    result["comment"].append(
-                        f"azure.storage_resource_provider.storage_blob '{name}' has no property need to be updated."
-                    )
-                # ii. Properties will be updated
-                else:
-                    result[
-                        "new_state"
-                    ] = hub.tool.azure.storage_resource_provider.storage_blob.convert_raw_storage_blob_to_present(
-                        subscription_id=subscription_id,
-                        resource_grp_name=resource_group_name,
-                        account_name=account_name,
-                        result_dict=new_payload["ret"],
-                    )
-                    result["comment"].append(
-                        f"Would update azure.storage_resource_provider.storage_blob '{name}'"
-                    )
+            if not response_put["result"]:
+                result["comment"] = [response_put["comment"], response_put["ret"]]
+                result["result"] = False
                 return result
 
-            # PUT operation nothing to update the resource
-            if new_payload["ret"] == None:
+        result[
+            "new_state"
+        ] = hub.tool.azure.subscription.subscriptions.convert_raw_subscription_to_present(
+            resource=response_put["ret"],
+            idem_resource_name=name,
+            alias=alias,
+            display_name=display_name,
+            subscription_id=None,
+            resource_id=resource_id,
+        )
+        result["comment"].append(f"Created azure.subscription.subscriptions '{name}'")
+        return result
+
+    else:
+        # Update/rename subscription display name if given subscription already present
+        # and display name is modified in the input
+        existing_resource = response_get["ret"]
+        result[
+            "old_state"
+        ] = hub.tool.azure.subscription.subscriptions.convert_raw_subscription_to_present(
+            resource=existing_resource,
+            idem_resource_name=name,
+            alias=alias,
+            display_name=None,
+            subscription_id=None,
+            resource_id=resource_id,
+        )
+        subscription_id = result["old_state"]["subscription_id"]
+        # Generate a new PUT operation payload with new values
+        is_display_name_updated = display_name != existing_resource.get("displayName")
+        if ctx.get("test", False):
+            if not is_display_name_updated:
                 result["new_state"] = copy.deepcopy(result["old_state"])
                 result["comment"].append(
-                    f"azure.storage_resource_provider.storage_blob '{name}' has no property need to be updated."
+                    f"azure.subscription.subscriptions '{name}' has no property need to be updated."
                 )
-                return result
-
-            # Call PUT operation to update the resource
-            result["comment"] = result["comment"] + new_payload["comment"]
-            response_put = await hub.exec.request.json.put(
-                ctx,
-                url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-04-01",
-                success_codes=[200],
-                json=new_payload["ret"],
-            )
-            if response_put["result"] == False:
-                hub.log.debug(
-                    f"Could not update azure.storage_resource_provider.storage_blob {response_put['comment']} {response_put['ret']}"
+            else:
+                result[
+                    "new_state"
+                ] = hub.tool.azure.subscription.subscriptions.convert_raw_subscription_to_present(
+                    resource=response_get["ret"],
+                    idem_resource_name=name,
+                    alias=alias,
+                    display_name=display_name,
+                    subscription_id=None,
+                    resource_id=resource_id,
                 )
-                result["result"] = False
-                result["comment"] = [response_put["comment"], response_put["ret"]]
-                return result
-
-            result[
-                "new_state"
-            ] = hub.tool.azure.storage_resource_provider.storage_blob.convert_raw_storage_blob_to_present(
-                subscription_id=subscription_id,
-                resource_grp_name=resource_group_name,
-                account_name=account_name,
-                result_dict=response_put["ret"],
-            )
-            if result["old_state"] == result["new_state"]:
                 result["comment"].append(
-                    f"azure.storage_resource_provider.storage_blob '{name}' has no property need to be updated."
+                    f"Would update azure.subscription.subscriptions '{name}'"
                 )
-                return result
-
+            return result
+        # POST operation to rename subscription display_name
+        if not is_display_name_updated:
+            result["new_state"] = copy.deepcopy(result["old_state"])
             result["comment"].append(
-                f"Updated azure.storage_resource_provider.storage_blob '{name}'"
+                f"azure.subscription.subscriptions '{name}' has no property need to be updated."
             )
             return result
-    # 3. If issue occurred while finding resource
-    else:
-        hub.log.debug(
-            f"Could not get azure.storage_resource_provider.storage_blob {response_get['comment']} {response_get['ret']}"
+        rename_payload = {"subscriptionName": display_name}
+        response_rename = await hub.exec.request.json.post(
+            ctx,
+            url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/providers/Microsoft.Subscription/rename?api-version=2020-09-01",
+            success_codes=[200, 201],
+            json=rename_payload,
         )
-        result["result"] = False
-        result["comment"] = [response_get["comment"], response_get["ret"]]
+        if not response_rename["result"]:
+            hub.log.debug(
+                f"Could not update azure.subscription.subscriptions {response_rename['comment']} {response_rename['ret']}"
+            )
+            result["result"] = False
+            result["comment"] = [response_rename["comment"], response_rename["ret"]]
+            return result
+
+        result["new_state"] = copy.deepcopy(result["old_state"])
+        result["new_state"]["display_name"] = display_name
+        result["comment"].append(f"Updated azure.subscription.subscriptions '{name}'")
         return result
 
 
-async def absent(
-    hub,
-    ctx,
-    name: str,
-    subscription_id: str,
-    resource_group_name: str,
-    account_name: str,
-    container_name: str,
-):
+async def absent(hub, ctx, name: str, alias: str) -> Dict:
+    r"""Delete Subscription. This state disables the subscription and deletes respective alias.
+
+    Once subscription is in disabled state, after 90 days it gets deleted automatically.
+
+    Args:
+        name(str): The identifier for this state.
+        alias(str): The alias name of the subscription to delete.
+
+    Returns:
+        Dict
+
+    Examples:
+        .. code-block:: sls
+
+            subscription_is_absent:
+              azure.subscription.subscriptions.absent:
+                - name: value
+                - alias: value
+    """
     result = {
         "name": name,
         "result": True,
         "old_state": None,
         "new_state": None,
         "comment": [],
     }
 
-    if subscription_id is None:
-        subscription_id = ctx.acct.subscription_id
-    resource_id = (
-        f"/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Storage/"
-        f"storageAccounts/{account_name}/blobServices/default/containers/{container_name}"
-    )
-    response_get = await hub.exec.azure.storage_resource_provider.storage_blob.get(
+    resource_id = f"/providers/Microsoft.Subscription/aliases/{alias}"
+    response_get = await hub.exec.azure.subscription.subscriptions.get(
         ctx,
         resource_id=resource_id,
     )
     if not response_get["result"]:
         hub.log.debug(
-            f"Could not get azure.storage_resource_provider.storage_blob '{name}' {response_get['comment']} {response_get['ret']}"
+            f"Could not get azure.subscriptions.subscription '{name}' {response_get['comment']} {response_get['ret']}"
         )
         result["result"] = False
         result["comment"] = [response_get["comment"], response_get["ret"]]
         return result
 
     if response_get["ret"]:
         result["old_state"] = response_get["ret"]
         result["old_state"]["name"] = name
-
+        subscription_id = response_get["ret"]["subscription_id"]
         if ctx.get("test", False):
             result["comment"].append(
-                f"Would delete azure.storage_resource_provider.storage_blob '{name}'"
+                f"Would delete azure.subscription.subscriptions '{name}'"
             )
             return result
+
+        # Cancel the subscription before deleting
+        # Once subscription is cancelled, it will be in disabled state and after 90 days it gets deleted automatically.
+        response_cancel = await hub.exec.request.json.post(
+            ctx,
+            url=f"{ctx.acct.endpoint_url}/subscriptions/{subscription_id}/providers/Microsoft.Subscription/cancel?api-version=2020-09-01",
+            success_codes=[200, 202],
+        )
+        if not response_cancel["result"]:
+            result["result"] = False
+            result["comment"] = [response_cancel["comment"], response_cancel["ret"]]
+            return result
+
+        # Delete subscription alias.
+        # After deleting the subscription with alias, deleted alias can be used to create new subscription
         response_delete = await hub.exec.request.raw.delete(
             ctx,
-            url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2021-06-01",
+            url=f"{ctx.acct.endpoint_url}{resource_id}?api-version=2020-09-01",
             success_codes=[200, 202],
         )
 
         if not response_delete["result"]:
             hub.log.debug(
-                f"Could not delete azure.storage_resource_provider.storage_blob {response_delete['comment']} {response_delete['ret']}"
+                f"Could not delete azure.subscription.subscriptions {response_delete['comment']} {response_delete['ret']}"
             )
             result["result"] = False
             result["comment"] = [response_delete["comment"], response_delete["ret"]]
             return result
 
-        result["comment"].append(
-            f"Deleted azure.storage_resource_provider.storage_blob '{name}'"
-        )
+        result["comment"].append(f"Deleted azure.subscription.subscriptions '{name}'")
         return result
     else:
-        # If Azure returns 'Not Found' error, it means the resource has been absent.
+        # If Azure returns 'Not Found' error, it means the management group is not associated with given subscription.
         result["comment"].append(
-            f"azure.storage_resource_provider.storage_blob '{name}' already absent"
+            f"azure.subscriptions.subscription '{name}' already absent"
         )
         return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
+    r"""Describe subscriptions in a way that can be recreated/managed with the corresponding "present" function.
+
+    Lists all subscriptions.
+
+    Returns:
+        Dict[str, Any]
+
+    Examples:
+        .. code-block:: sls
+
+            $ idem describe azure.subscription.subscriptions
+    """
     result = {}
-    ret_list = await hub.exec.azure.storage_resource_provider.storage_blob.list(ctx)
+    ret_list = await hub.exec.azure.subscription.subscriptions.list(ctx)
     if not ret_list["ret"]:
-        hub.log.debug(f"Could not describe storage account {ret_list['comment']}")
+        hub.log.debug(
+            f"Could not describe subscription subscriptions {ret_list['comment']}"
+        )
         return result
+
     for resource in ret_list["ret"]:
         resource_id = resource["resource_id"]
         result[resource_id] = {
-            "azure.storage_resource_provider.storage_blob.present": [
+            "azure.subscription.subscriptions.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
     return result
-
-
-def get_create_payload(
-    p_resource_id,
-    p_name,
-    p_container_name,
-    p_metadata,
-    resource_group_name,
-    p_remaining_retention_days,
-    p_public_access,
-    p_has_immutability_policy,
-):
-    return {
-        "id": p_resource_id,
-        "name": p_name,
-        "container_name": p_container_name,
-        "resource_group_name": resource_group_name,
-        "type": "Microsoft.Storage/storageAccounts/blobServices/containers",
-        "properties": {
-            "metadata": p_metadata,
-            "deleted": False,
-            "remainingRetentionDays": p_remaining_retention_days,
-            "publicAccess": p_public_access,
-            "hasImmutabilityPolicy": p_has_immutability_policy,
-            "hasLegalHold": False,
-        },
-    }
```

### Comparing `idem-azure-0.3.4/idem_azure/states/azure/subscription/attach_subscriptions.py` & `idem-azure-0.4.0/idem_azure/states/azure/subscription/attach_subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/authorization/role_assignments.py` & `idem-azure-0.4.0/idem_azure/tool/azure/authorization/role_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/authorization/role_definitions.py` & `idem-azure-0.4.0/idem_azure/tool/azure/authorization/role_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/compute/log_analytics_workspace.py` & `idem-azure-0.4.0/idem_azure/tool/azure/compute/log_analytics_workspace.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/compute/virtual_machines.py` & `idem-azure-0.4.0/idem_azure/tool/azure/compute/virtual_machines.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,36 +3,42 @@
 from typing import Dict
 from typing import List
 
 
 def convert_present_to_raw_virtual_machine(
     hub,
     location: str,
-    virtual_machine_size: str,
     network_interface_ids: List[str],
-    storage_image_reference: Dict[str, Any],
-    storage_os_disk: Dict[str, Any],
-    storage_data_disks: List[Dict[str, Any]],
     os_profile: Dict[str, Any],
+    storage_os_disk: Dict[str, Any],
+    virtual_machine_size: str = None,
+    storage_image_reference: Dict[str, Any] = None,
+    storage_data_disks: List[Dict[str, Any]] = None,
     tags: Dict = None,
+    plan: Dict[str, str] = None,
+    availability_set_id: str = None,
+    license_type: str = None,
 ):
     """
     Giving some present function inputs, generate a payload that can be used during PUT operation to Azure. Any None
     value input will be ignored, unless this parameter is a required input parameter.
 
     Args:
         hub: The redistributed pop central hub.
         location(str): Resource location. Changing this forces a new resource to be created.
-        virtual_machine_size(str): Specifies the size of the Virtual Machine.
         network_interface_ids(List[str]): A list of Network Interface IDs which should be associated with the Virtual Machine.
-        tags(Dict, optional): Resource tags.
-        os_profile(Dict): Specifies the operating system settings used while creating the virtual machine.
-        storage_image_reference(Dict): Specifies information about the image to use. Eg- platform images, marketplace images.
-        storage_os_disk(Dict): Specifies information about the operating system disk used by the virtual machine.
-        storage_data_disks(list(Dict), optional): List of Data disks attached/added to a VM.
+        os_profile(Dict[str, Any]): Specifies the operating system settings used while creating the virtual machine.
+        storage_os_disk(Dict[str, Any]): Specifies information about the operating system disk used by the virtual machine.
+        virtual_machine_size(str, Optional): Specifies the size of the Virtual Machine.
+        storage_image_reference(Dict[str, Any], Optional): Specifies information about the image to use. Eg- platform images, marketplace images.
+        storage_data_disks(List[Dict[str, Any]], Optional): List of Data disks attached/added to a VM.
+        tags(Dict, Optional): Resource tags.
+        plan(Dict[str, str], Optional): Specifies information about the marketplace image used to create the virtual machine.
+        availability_set_id(str, Optional): Specifies id of the availability set that the virtual machine should be assigned to.
+        license_type(str, Optional): Specifies that the image or disk that is being used was licensed on-premises.
 
     Returns:
         A Dict in the format of an Azure PUT operation payload.
     """
     payload = {
         "location": location,
         "properties": {"hardwareProfile": {"vmSize": virtual_machine_size}},
@@ -45,15 +51,17 @@
         }
         payload["properties"]["networkProfile"] = network_interface_ids_payload
 
     storage_profile_payload = {}
     if storage_image_reference is not None:
         storage_profile_payload[
             "imageReference"
-        ] = convert_present_to_raw_image_reference(storage_image_reference)
+        ] = hub.tool.azure.compute.virtual_machines.convert_present_to_raw_image_reference(
+            storage_image_reference
+        )
     if storage_os_disk is not None:
         storage_profile_payload["osDisk"] = convert_present_to_raw_os_disk(
             storage_os_disk
         )
     if storage_data_disks is not None:
         storage_profile_payload["dataDisks"] = convert_present_to_raw_data_disks(
             storage_data_disks
@@ -61,17 +69,26 @@
     payload["properties"]["storageProfile"] = storage_profile_payload
 
     if os_profile is not None:
         payload["properties"]["osProfile"] = convert_present_to_raw_os_profile(
             os_profile
         )
 
+    if availability_set_id is not None:
+        payload["properties"]["availabilitySet"] = {"id": availability_set_id}
+
+    if license_type is not None:
+        payload["properties"]["licenseType"] = license_type
+
     if tags is not None:
         payload["tags"] = tags
 
+    if plan is not None:
+        payload["plan"] = convert_present_to_raw_plan(plan)
+
     return payload
 
 
 def convert_raw_virtual_machine_to_present(
     hub,
     resource: Dict,
     idem_resource_name: str,
@@ -138,16 +155,28 @@
                 )
                 resource_translated["storage_os_disk"] = os_disk_payload
             if storage_profile_properties.get("dataDisks") is not None:
                 data_disk_payload = convert_raw_to_present_data_disks(
                     data_disks=storage_profile_properties.get("dataDisks")
                 )
                 resource_translated["storage_data_disks"] = data_disk_payload
+
+        if properties.get("availabilitySet") is not None:
+            resource_translated["availability_set_id"] = properties.get(
+                "availabilitySet"
+            ).get("id")
+
+        if properties.get("licenseType") is not None:
+            resource_translated["license_type"] = properties.get("licenseType")
+
     if "tags" in resource:
         resource_translated["tags"] = resource.get("tags")
+    if "plan" in resource:
+        resource_translated["plan"] = convert_raw_to_present_plan(resource.get("plan"))
+
     return resource_translated
 
 
 def update_virtual_machine_payload(
     hub, existing_payload: Dict[str, Any], new_values: Dict[str, Any]
 ) -> Dict[str, Any]:
     """
@@ -264,15 +293,15 @@
                     existing_properties.get("storageProfile").get("imageReference"),
                     new_values.get("storage_image_reference"),
                 )
             )
         ):
             updated_properties_payload["storageProfile"][
                 "imageReference"
-            ] = convert_present_to_raw_image_reference(
+            ] = hub.tool.azure.compute.virtual_machines.convert_present_to_raw_image_reference(
                 storage_image_reference=merge_dictionary_payloads(
                     convert_raw_to_present_image_reference(
                         existing_properties.get("storageProfile").get("imageReference")
                     ),
                     new_values.get("storage_image_reference"),
                 )
             )
@@ -289,37 +318,60 @@
                         existing_properties.get("osProfile")
                     ),
                     new_values.get("os_profile"),
                 )
             )
             need_update = True
 
+    if new_values.get("availability_set_id") is not None:
+        if (existing_properties.get("availabilitySet") is None) or (
+            existing_properties.get("availabilitySet").get("id")
+            != new_values.get("availability_set_id")
+        ):
+            updated_properties_payload["availabilitySet"] = {
+                "id": new_values.get("availability_set_id")
+            }
+            need_update = True
+
+    if new_values.get("license_type") is not None:
+        if (existing_properties.get("licenseType") is None) or (
+            existing_properties.get("licenseType") != new_values.get("license_type")
+        ):
+            updated_properties_payload["licenseType"] = new_values.get("license_type")
+            need_update = True
+
     new_payload["properties"] = updated_properties_payload
 
     if (new_values.get("tags") is not None) and (
         existing_payload.get("tags") != new_values.get("tags")
     ):
         new_payload["tags"] = new_values.get("tags")
         need_update = True
 
+    if (new_values.get("plan") is not None) and (
+        existing_payload.get("plan") != new_values.get("plan")
+    ):
+        new_payload["plan"] = new_values.get("plan")
+        need_update = True
+
     if need_update:
         result["ret"] = new_payload
     return result
 
 
 def convert_present_to_raw_network_interfaces(network_interface_ids: List[str]):
     """
     Giving some present function inputs, generate a payload that can be used during PUT operation to Azure. Any None
     value input will be ignored, unless this parameter is a required input parameter.
 
     Args:
-        network_interface_ids(list(str)) : List of Network Interface Ids
+        network_interface_ids(List[str]) : List of Network Interface Ids
 
     Returns:
-        Network Interface Ids List(Dict[str,any]) in the format of an Azure PUT operation payload.
+        Network Interface Ids List[Dict[str, Any]] in the format of an Azure PUT operation payload.
     """
     network_interface_id_counter = 0
     network_interfaces_list: List = []
     for network_interface_id in network_interface_ids:
         network_interfaces_payload = {"id": network_interface_id}
         primary_network_payload = {}
         if network_interface_id_counter == 0:
@@ -328,15 +380,17 @@
             primary_network_payload["primary"] = False
         network_interfaces_payload["properties"] = primary_network_payload
         network_interfaces_list.append(network_interfaces_payload)
         network_interface_id_counter = network_interface_id_counter + 1
     return network_interfaces_list
 
 
-def convert_present_to_raw_image_reference(storage_image_reference: Dict[str, Any]):
+def convert_present_to_raw_image_reference(
+    hub, storage_image_reference: Dict[str, Any]
+):
     """
     Giving some present function inputs, generate a payload that can be used during PUT operation to Azure. Any None
     value input will be ignored, unless this parameter is a required input parameter.
 
     Args:
         storage_image_reference(Dict(str, Any)) : Specifies information about the image to use in VM creation/update
 
@@ -344,16 +398,21 @@
         Storage Image Reference Dict[str,any] in the format of an Azure PUT operation payload.
     """
     storage_image_reference_payload = {
         "publisher": storage_image_reference.get("image_publisher"),
         "offer": storage_image_reference.get("image_offer"),
         "sku": storage_image_reference.get("image_sku"),
         "version": storage_image_reference.get("image_version"),
+        "id": storage_image_reference.get("image_id"),
+        "sharedGalleryImageId": storage_image_reference.get("shared_gallery_image_id"),
+        "communityGalleryImageId": storage_image_reference.get(
+            "community_gallery_image_id"
+        ),
     }
-    return storage_image_reference_payload
+    return hub.tool.azure.utils.cleanup_none_values(storage_image_reference_payload)
 
 
 def convert_present_to_raw_os_disk(os_disk: Dict[str, Any]):
     """
     Giving some present function inputs, generate a payload that can be used during PUT operation to Azure. Any None
     value input will be ignored, unless this parameter is a required input parameter.
 
@@ -370,27 +429,40 @@
         "createOption": os_disk.get("disk_create_option"),
         "deleteOption": os_disk.get("disk_delete_option"),
         "managedDisk": {
             "id": os_disk.get("disk_id"),
             "storageAccountType": os_disk.get("storage_account_type"),
         },
     }
+    if os_disk.get("disk_image_vhd_uri") is not None:
+        os_disk_payload["image"] = {"uri": os_disk.get("disk_image_vhd_uri")}
+    if os_disk.get("disk_os_type") is not None:
+        os_disk_payload["osType"] = os_disk.get("disk_os_type")
+
+    if os_disk.get("disk_vhd_uri") is not None:
+        os_disk_payload["vhd"] = {"uri": os_disk.get("disk_vhd_uri")}
+
+    if os_disk.get("write_accelerator_enabled") is not None:
+        os_disk_payload["writeAcceleratorEnabled"] = os_disk.get(
+            "write_accelerator_enabled"
+        )
+
     return os_disk_payload
 
 
 def convert_present_to_raw_data_disks(data_disks: List[Dict[str, Any]]):
     """
     Giving some present function inputs, generate a payload that can be used during PUT operation to Azure. Any None
     value input will be ignored, unless this parameter is a required input parameter.
 
     Args:
-        data_disks(list(Dict[str, Any]) : List of Data Disk payload for VM
+        data_disks(List[Dict[str, Any]] : List of Data Disk payload for VM
 
     Returns:
-        List of Data Disk payload List(Dict[str,any]) in the format of an Azure PUT operation payload.
+        List of Data Disk payload List[Dict[str, Any]] in the format of an Azure PUT operation payload.
     """
     data_disks_list: List = []
     for data_disk in data_disks:
         data_disks_payload = {
             "name": data_disk.get("disk_name"),
             "diskSizeGB": data_disk.get("disk_size_in_GB"),
             "lun": data_disk.get("disk_logical_unit_number"),
@@ -421,14 +493,22 @@
         "adminUsername": os_profile.get("admin_username"),
         "adminPassword": os_profile.get("admin_password"),
         "computerName": os_profile.get("computer_name"),
     }
     return os_profile_payload
 
 
+def convert_present_to_raw_plan(plan: Dict[str, Any]):
+    plan_payload = {**plan}
+    promotion_code = plan_payload.pop("promotion_code", None)
+    if promotion_code:
+        plan_payload["promotionCode"] = promotion_code
+    return plan_payload
+
+
 def convert_raw_to_present_os_profile(os_profile: Dict[str, Any]):
     """
      Giving an existing resource state and desired state inputs, generate a Dict that match the format of
      present input parameters.
 
     Args:
         os_profile(Dict, optional): OS Profile payload in a virtual machine resource
@@ -445,15 +525,15 @@
 
 def convert_raw_to_present_network_interface(network_interfaces: List[Dict[str, Any]]):
     """
      Giving an existing resource state and desired state inputs, generate a Dict that match the format of
      present input parameters.
 
     Args:
-        network_interfaces(list[Dict], optional): Resource List of Network Interfaces in a virtual machine resource.
+        network_interfaces(List[Dict], optional): Resource List of Network Interfaces in a virtual machine resource.
 
     Returns:
          A Network Interface Id List that contains the parameters that match respective present function's input format.
     """
     present_network_interfaces: List = []
     for network_interface in network_interfaces:
         present_network_interfaces.append(network_interface.get("id"))
@@ -472,14 +552,17 @@
          Image Reference payload contains the parameters that match respective present function's input format.
     """
     image_reference_payload = {
         "image_sku": image_reference.get("sku"),
         "image_publisher": image_reference.get("publisher"),
         "image_version": image_reference.get("version"),
         "image_offer": image_reference.get("offer"),
+        "image_id": image_reference.get("id"),
+        "shared_gallery_image_id": image_reference.get("sharedGalleryImageId"),
+        "community_gallery_image_id": image_reference.get("communityGalleryImageId"),
     }
     return image_reference_payload
 
 
 def convert_raw_to_present_os_disk(os_disk: Dict[str, Any]):
     """
      Giving an existing resource state and desired state inputs, generate a Dict that match the format of
@@ -509,24 +592,34 @@
         and os_disk.get("managedDisk").get("id") is not None
     ):
         os_disk_payload["disk_id"] = os_disk.get("managedDisk").get("id")
     if os_disk.get("createOption") is not None:
         os_disk_payload["disk_create_option"] = os_disk.get("createOption")
     if os_disk.get("deleteOption") is not None:
         os_disk_payload["disk_delete_option"] = os_disk.get("deleteOption")
+    if os_disk.get("image", {}).get("uri") is not None:
+        os_disk_payload["disk_image_vhd_uri"] = os_disk.get("image").get("uri")
+    if os_disk.get("osType") is not None:
+        os_disk_payload["disk_os_type"] = os_disk.get("osType")
+    if os_disk.get("vhd", {}).get("uri") is not None:
+        os_disk_payload["disk_vhd_uri"] = os_disk.get("vhd").get("uri")
+    if os_disk.get("writeAcceleratorEnabled") is not None:
+        os_disk_payload["write_accelerator_enabled"] = os_disk.get(
+            "writeAcceleratorEnabled"
+        )
     return os_disk_payload
 
 
 def convert_raw_to_present_data_disks(data_disks: List[Dict[str, Any]]):
     """
      Giving an existing resource state and desired state inputs, generate a Dict that match the format of
      present input parameters.
 
     Args:
-        data_disks(list[Dict], optional): Resource List of Data Disks in a virtual machine resource.
+        data_disks(List[Dict], optional): Resource List of Data Disks in a virtual machine resource.
 
     Returns:
          A Data Disk List that contains the parameters that match respective present function's input format.
     """
     present_data_disks_payload: List = []
     for data_disk in data_disks:
         data_disk_payload = {
@@ -552,25 +645,33 @@
             data_disk_payload["disk_create_option"] = data_disk.get("createOption")
         if data_disk.get("deleteOption") is not None:
             data_disk_payload["disk_delete_option"] = data_disk.get("deleteOption")
         present_data_disks_payload.append(data_disk_payload)
     return present_data_disks_payload
 
 
+def convert_raw_to_present_plan(plan: Dict[str, Any]):
+    plan_payload = {**plan}
+    promotion_code = plan_payload.pop("promotionCode", None)
+    if promotion_code:
+        plan_payload["promotion_code"] = promotion_code
+    return plan_payload
+
+
 def compare_network_interface_payload(
     existing_network_interface_list: List[Dict[str, Any]],
     network_interface_ids: List[str],
 ):
     """
     Compares network interface payload to check whether any of the state attributes has been added or modified.
     Returns true if there is any updates else false.
 
     Args:
-        existing_network_interface_list(list[Dict]): Existing Network Interface payload
-        network_interface_ids(list[str]): Present value which will be given as input
+        existing_network_interface_list(List[Dict]): Existing Network Interface payload
+        network_interface_ids(List[str]): Present value which will be given as input
 
     Returns:
         A boolean value, True if there is any difference between the arguments else returns False
     """
     if len(network_interface_ids) != len(existing_network_interface_list):
         return True
     existing_network_interface_id_list = []
@@ -607,16 +708,16 @@
     new_storage_data_disks: List[Dict[str, Any]],
 ):
     """
     Compares Data Disks payload to check whether any of the state attributes has been added or modified.
     Returns true if there is any updates else false.
 
     Args:
-        existing_storage_data_disks_payload(list[Dict]): Existing Storage Data Disk payload
-        new_storage_data_disks(list[str]): Present value which will be given as input
+        existing_storage_data_disks_payload(List[Dict]): Existing Storage Data Disk payload
+        new_storage_data_disks(List[str]): Present value which will be given as input
 
     Returns:
         A boolean value, True if there is any difference between the arguments else returns False
     """
     data_disks_present_converted_payload = convert_raw_to_present_data_disks(
         existing_storage_data_disks_payload
     )
@@ -707,15 +808,15 @@
 ):
     """
     Compares the payload to check whether any of the state attributes has been added or modified.
     Returns true if there is any updates else false.
 
     Args:
         existing_payload_map(Dict): Existing payload Map
-        update_payload(List(Dict)): Present value which will be given as input
+        update_payload(List[Dict]): Present value which will be given as input
 
     Returns:
         A boolean value, True if there is any difference between the arguments else returns False
     """
     for update_element in update_payload:
         disk_name = update_element.get("disk_name")
         if disk_name in existing_payload_map:
```

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/container.py` & `idem-azure-0.4.0/idem_azure/tool/azure/container.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/key_vault/vault.py` & `idem-azure-0.4.0/idem_azure/tool/azure/key_vault/vault.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/management_groups/management_groups.py` & `idem-azure-0.4.0/idem_azure/tool/azure/management_groups/management_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/network/firewall.py` & `idem-azure-0.4.0/idem_azure/tool/azure/network/firewall.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/network/firewall_policies.py` & `idem-azure-0.4.0/idem_azure/tool/azure/network/firewall_policies.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/network/network_interfaces.py` & `idem-azure-0.4.0/idem_azure/tool/azure/network/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/network/network_security_groups.py` & `idem-azure-0.4.0/idem_azure/tool/azure/network/network_security_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/network/public_ip_addresses.py` & `idem-azure-0.4.0/idem_azure/tool/azure/network/public_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/network/route_tables.py` & `idem-azure-0.4.0/idem_azure/tool/azure/network/route_tables.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/network/routes.py` & `idem-azure-0.4.0/idem_azure/tool/azure/network/routes.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/network/security_rules.py` & `idem-azure-0.4.0/idem_azure/tool/azure/network/security_rules.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/network/subnets.py` & `idem-azure-0.4.0/idem_azure/tool/azure/network/subnets.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/network/virtual_networks.py` & `idem-azure-0.4.0/idem_azure/tool/azure/network/virtual_networks.py`

 * *Files 23% similar despite different names*

```diff
@@ -35,78 +35,113 @@
         "resource_group_name": resource_group_name,
         "virtual_network_name": virtual_network_name,
         "location": resource["location"],
         "subscription_id": subscription_id,
     }
     if "tags" in resource:
         resource_translated["tags"] = resource["tags"]
+    if "extendedLocation" in resource:
+        resource_translated["extended_location"] = resource["extendedLocation"]
     properties = resource.get("properties")
     if properties:
         properties_parameters = {
             "bgpCommunities": "bgp_communities",
             "flowTimeoutInMinutes": "flow_timeout_in_minutes",
             "provisioningState": "provisioning_state",
+            "ddosProtectionPlan": "ddos_protection_plan",
+            "enableDdosProtection": "enable_ddos_protection",
+            "enableVmProtection": "enable_vm_protection",
         }
         for parameter_raw, parameter_present in properties_parameters.items():
             if parameter_raw in properties:
                 resource_translated[parameter_present] = properties.get(parameter_raw)
         resource_translated["address_space"] = properties["addressSpace"][
             "addressPrefixes"
         ]
         if properties.get("subnets") is not None:
             existing_subnets_required_payload = convert_raw_to_present_vn_subnet(
                 subnets=properties["subnets"]
             )
             resource_translated["subnets"] = existing_subnets_required_payload
+        if (
+            properties.get("dhcpOptions") is not None
+            and properties.get("dhcpOptions", {}).get("dnsServers") is not None
+        ):
+            resource_translated["dhcp_options"] = {
+                "dns_servers": properties["dhcpOptions"]["dnsServers"]
+            }
     return resource_translated
 
 
 def convert_present_to_raw_virtual_network(
     hub,
     subscription_id: str,
     address_space: List,
     location: str,
+    extended_location: Dict = None,
     bgp_communities: str = None,
     flow_timeout_in_minutes: int = None,
     subnets: List = None,
+    ddos_protection_plan: Dict = None,
+    enable_ddos_protection: bool = None,
+    enable_vm_protection: bool = None,
+    dhcp_options: Dict = None,
     tags: Dict = None,
 ):
     """
     Giving some present function inputs, generate a payload that can be used during PUT operation to Azure. Any None
     value input will be ignored, unless this parameter is a required input parameter.
 
     Args:
         hub: The redistributed pop central hub.
         subscription_id: subscription id
         address_space: An array of IP address ranges that can be used by subnets of the virtual network.
         location: Resource location. Update this field will result in resource re-creation.
+        extended_location: The extended location of the virtual network.
         bgp_communities: Bgp Communities sent over ExpressRoute with each route corresponding to a prefix in this VNET.
         flow_timeout_in_minutes: The FlowTimeout value (in minutes) for the Virtual Network
-        subnets(list[dict], optional): List of Subnet in a virtual network resource.Each Subnet will have fields
+        subnets(list[dict], Optional): List of Subnet in a virtual network resource.Each Subnet will have fields
           name(str, required), address_space(str, required) , security_group_id(str, optional) and service_endpoints(list, optional)
+        ddos_protection_plan(Dict, Optional):
+            id(str): The DDoS protection plan associated with the virtual network.
+        enable_ddos_protection(bool, Optional): Indicates if DDoS protection is enabled for all the protected resources in the virtual network. It requires a DDoS protection plan associated with the resource.
+        enable_vm_protection(bool, Optional): Indicates if VM protection is enabled for all the subnets in the virtual network.
+        dhcp_options(Dict, Optional): DhcpOptions contains an array of DNS servers available to VMs deployed in the virtual network. Standard DHCP option for a subnet overrides VNET DHCP options.
         tags: Resource tags.
 
     Returns:
         A dict in the format of an Azure PUT operation payload.
     """
     payload = {
         "location": location,
         "properties": {"addressSpace": {"addressPrefixes": address_space}},
     }
     if tags is not None:
         payload["tags"] = tags
+    if extended_location is not None:
+        payload["extendedLocation"] = extended_location
     if bgp_communities is not None:
         payload["properties"]["bgpCommunities"] = bgp_communities
     if flow_timeout_in_minutes is not None:
         payload["properties"]["flowTimeoutInMinutes"] = flow_timeout_in_minutes
+    if ddos_protection_plan is not None and ddos_protection_plan.get("id") is not None:
+        payload["properties"]["ddosProtectionPlan"] = ddos_protection_plan
+    if enable_ddos_protection is not None:
+        payload["properties"]["enableDdosProtection"] = enable_ddos_protection
+    if enable_vm_protection is not None:
+        payload["properties"]["enableVmProtection"] = enable_vm_protection
     if subnets is not None:
         subnets_payload = convert_present_to_raw_vn_subnet(
             subscription_id=subscription_id, subnets=subnets
         )
         payload["properties"]["subnets"] = subnets_payload
+    if dhcp_options is not None and dhcp_options.get("dns_servers") is not None:
+        payload["properties"]["dhcpOptions"] = {
+            "dnsServers": dhcp_options["dns_servers"]
+        }
     return payload
 
 
 def update_virtual_network_payload(
     hub,
     subscription_id: str,
     existing_payload: Dict[str, Any],
@@ -134,14 +169,19 @@
     is_updated = False
     new_payload = copy.deepcopy(existing_payload)
     if (new_values.get("tags") is not None) and (
         existing_payload.get("tags") != new_values.get("tags")
     ):
         new_payload["tags"] = new_values["tags"]
         is_updated = True
+    if (new_values.get("extended_location") is not None) and (
+        existing_payload.get("extendedLocation") != new_values.get("extended_location")
+    ):
+        new_payload["extendedLocation"] = new_values["extended_location"]
+        is_updated = True
     existing_properties = existing_payload["properties"]
     if (new_values.get("address_space") is not None) and (
         set(new_values["address_space"])
         != set(existing_properties["addressSpace"]["addressPrefixes"])
     ):
         new_payload["properties"]["addressSpace"]["addressPrefixes"] = new_values[
             "address_space"
@@ -156,26 +196,60 @@
         new_values["flow_timeout_in_minutes"]
         != existing_properties.get("flowTimeoutInMinutes")
     ):
         new_payload["properties"]["flowTimeoutInMinutes"] = new_values.get(
             "flow_timeout_in_minutes"
         )
         is_updated = True
+    if (new_values.get("ddos_protection_plan") is not None) and (
+        new_values["ddos_protection_plan"]
+        != existing_properties.get("ddosProtectionPlan")
+    ):
+        new_payload["properties"]["ddosProtectionPlan"] = new_values.get(
+            "ddos_protection_plan"
+        )
+        is_updated = True
+    if (new_values.get("enable_ddos_protection") is not None) and (
+        new_values["enable_ddos_protection"]
+        != existing_properties.get("enableDdosProtection")
+    ):
+        new_payload["properties"]["enableDdosProtection"] = new_values.get(
+            "enable_ddos_protection"
+        )
+        is_updated = True
+    if (new_values.get("enable_vm_protection") is not None) and (
+        new_values["enable_vm_protection"]
+        != existing_properties.get("enableVmProtection")
+    ):
+        new_payload["properties"]["enableVmProtection"] = new_values.get(
+            "enable_vm_protection"
+        )
+        is_updated = True
     if new_values.get("subnets") is not None:
         existing_subnets = existing_properties.get("subnets")
         existing_subnets_required_payload = convert_raw_to_present_vn_subnet(
             subnets=existing_subnets
         )
         if diff_virtual_network_subnets(
             new_values.get("subnets"), existing_subnets_required_payload, "name"
         ):
             new_payload["properties"]["subnets"] = convert_present_to_raw_vn_subnet(
                 subscription_id=subscription_id, subnets=new_values.get("subnets")
             )
             is_updated = True
+    if (
+        new_values.get("dhcp_options") is not None
+        and new_values.get("dhcp_options", {}).get("dns_servers") is not None
+        and new_values.get("dhcp_options", {}).get("dns_servers")
+        != existing_properties.get("dhcpOptions", {}).get("dnsServers")
+    ):
+        new_payload["properties"]["dhcpOptions"] = {
+            "dnsServers": new_values.get("dhcp_options", {}).get("dns_servers")
+        }
+        is_updated = True
     if is_updated:
         result["ret"] = new_payload
     return result
 
 
 def convert_present_to_raw_vn_subnet(
     subscription_id: str, subnets: List[Dict[str, Any]]
```

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/policy/policy_assignment.py` & `idem-azure-0.4.0/idem_azure/tool/azure/policy/policy_assignment.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/policy/policy_definition.py` & `idem-azure-0.4.0/idem_azure/tool/azure/policy/policy_definition.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/request.py` & `idem-azure-0.4.0/idem_azure/tool/azure/request.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/resource_management/resource_groups.py` & `idem-azure-0.4.0/idem_azure/tool/azure/resource_management/resource_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/storage_resource_provider/storage_accounts.py` & `idem-azure-0.4.0/idem_azure/tool/azure/storage_resource_provider/storage_accounts.py`

 * *Files 10% similar despite different names*

```diff
@@ -168,28 +168,34 @@
 
         if properties.get("sasPolicy") is not None:
             sasPolicyPayload = convert_raw_to_present_sas_policy(
                 hub, policy=properties.get("sasPolicy")
             )
             translated_resounrce["sas_policy"] = sasPolicyPayload
 
+        if properties.get("keyPolicy") is not None:
+            key_policy_payload = convert_raw_to_present_key_policy(
+                hub, policy=properties.get("keyPolicy")
+            )
+            translated_resounrce["key_policy"] = key_policy_payload
+
         if "allowedCopyScope" in properties:
             translated_resounrce["allowed_copy_scope"] = properties["allowedCopyScope"]
 
         if "isSftpEnabled" in properties:
             translated_resounrce["sftp_enabled"] = properties["isSftpEnabled"]
 
         return translated_resounrce
 
 
 def convert_present_to_raw_storage_accounts(
     hub,
     location: str,
-    sku_tier: str,
     sku_name: str,
+    sku_tier: str = None,
     account_kind: str = None,
     cross_tenant_replication_enabled: bool = None,
     access_tier: str = None,
     edge_zone: str = None,
     enable_https_traffic_only: bool = None,
     min_tls_version: str = None,
     allow_blob_public_access: bool = None,
@@ -205,14 +211,15 @@
     large_file_shares_state: str = None,
     azure_files_authentication: Dict[str, Any] = None,
     routing: Dict[str, Any] = None,
     encryption_service: Dict[str, Any] = None,
     require_infrastructure_encryption: bool = None,
     immutability_policy: Dict[str, Any] = None,
     sas_policy: Dict[str, Any] = None,
+    key_policy: Dict[str, Any] = None,
     allowed_copy_scope: str = None,
     sftp_enabled: bool = None,
     tags: Dict[str, str] = None,
 ):
     """
     Giving some present function inputs, generate a payload that can be used during PUT operation to Azure. Any None
     value input will be ignored, unless this parameter is a required input parameter.
@@ -241,14 +248,15 @@
          large_file_shares_state: Allow large file shares if sets to enabled.
          azure_files_authentication: Provides the identity based authentication settings for Azure Files.
          routing: Maintains information about the network routing choice opted by the user for data transfer
          encryption_service: set of encryption services
          require_infrastructure_encryption: A boolean indicating whether or not the service applies a secondary layer of encryption with platform managed keys for data at rest.
          immutability_policy: This argument specifies the default account-level immutability policy which is inherited and applied to objects
          sas_policy: SasPolicy assigned to the storage account.
+         key_policy: KeyPolicy assigned to the storage account.
          allowed_copy_scope: Restrict copy to and from Storage Accounts within an AAD tenant or with Private Links to the same VNet.
          sftp_enabled: Enables Secure File Transfer Protocol, if set to true
          tags: Gets or sets a list of key value pairs that describe the resource.
 
     Returns:
         A dict in the format of an Azure PUT operation payload.
     """
@@ -291,14 +299,15 @@
         or (large_file_shares_state is not None)
         or (azure_files_authentication is not None)
         or (routing is not None)
         or (encryption_service is not None)
         or (require_infrastructure_encryption is not None)
         or (immutability_policy is not None)
         or (sas_policy is not None)
+        or (key_policy is not None)
         or (allowed_copy_scope is not None)
         or (sftp_enabled is not None)
     ):
         payload["properties"] = {}
     if cross_tenant_replication_enabled is not None:
         payload["properties"][
             "allowCrossTenantReplication"
@@ -343,23 +352,45 @@
         or (encryption_service is not None)
         or (require_infrastructure_encryption is not None)
     ):
         payload["properties"]["encryption"] = {}
 
     if customer_managed_key is not None:
         payload["properties"]["encryption"]["keyvaultproperties"] = {}
-        payload["properties"]["encryption"]["keyvaultproperties"][
-            "currentVersionedKeyIdentifier"
-        ] = customer_managed_key["key_vault_key_id"]
+
+        if customer_managed_key.get("key_vault_key_id") is not None:
+            payload["properties"]["encryption"]["keyvaultproperties"][
+                "currentVersionedKeyIdentifier"
+            ] = customer_managed_key["key_vault_key_id"]
+
+        if customer_managed_key.get("key_name") is not None:
+            payload["properties"]["encryption"]["keyvaultproperties"][
+                "keyname"
+            ] = customer_managed_key.get("key_name")
+
+        if customer_managed_key.get("key_version") is not None:
+            payload["properties"]["encryption"]["keyvaultproperties"][
+                "keyversion"
+            ] = customer_managed_key.get("key_version")
+
+        if customer_managed_key.get("key_vault_uri") is not None:
+            payload["properties"]["encryption"]["keyvaultproperties"][
+                "keyvaulturi"
+            ] = customer_managed_key.get("key_vault_uri")
 
         payload["properties"]["encryption"]["identity"] = {}
         payload["properties"]["encryption"]["identity"][
             "userAssignedIdentity"
         ] = customer_managed_key["user_assigned_identity_id"]
 
+        if customer_managed_key.get("federated_identity_client_id") is not None:
+            payload["properties"]["encryption"]["identity"][
+                "federatedIdentityClientId"
+            ] = customer_managed_key.get("federated_identity_client_id")
+
     if network_rules is not None:
         payload["properties"]["networkAcls"] = convert_present_to_raw_network_rules(
             hub, rules=network_rules
         )
 
     if large_file_shares_state is not None:
         payload["properties"]["largeFileSharesState"] = large_file_shares_state
@@ -376,16 +407,19 @@
             hub, routing_pref=routing
         )
 
     if encryption_service is not None:
         payload["properties"]["encryption"]["keySource"] = encryption_service[
             "encryption_key_source"
         ]
-        if (encryption_service.get("queue_encryption_key_type") is not None) or (
-            encryption_service.get("table_encryption_key_type") is not None
+        if (
+            (encryption_service.get("queue_encryption_key_type") is not None)
+            or (encryption_service.get("table_encryption_key_type") is not None)
+            or (encryption_service.get("blob_encryption_key_type") is not None)
+            or (encryption_service.get("file_encryption_key_type") is not None)
         ):
             payload["properties"]["encryption"]["services"] = {}
 
         if encryption_service.get("queue_encryption_key_type") is not None:
             payload["properties"]["encryption"]["services"]["queue"] = {}
             payload["properties"]["encryption"]["services"]["queue"][
                 "keyType"
@@ -393,14 +427,26 @@
 
         if encryption_service.get("table_encryption_key_type") is not None:
             payload["properties"]["encryption"]["services"]["table"] = {}
             payload["properties"]["encryption"]["services"]["table"][
                 "keyType"
             ] = encryption_service.get("table_encryption_key_type")
 
+        if encryption_service.get("blob_encryption_key_type") is not None:
+            payload["properties"]["encryption"]["services"]["blob"] = {}
+            payload["properties"]["encryption"]["services"]["blob"][
+                "keyType"
+            ] = encryption_service.get("blob_encryption_key_type")
+
+        if encryption_service.get("file_encryption_key_type") is not None:
+            payload["properties"]["encryption"]["services"]["file"] = {}
+            payload["properties"]["encryption"]["services"]["file"][
+                "keyType"
+            ] = encryption_service.get("file_encryption_key_type")
+
     if require_infrastructure_encryption is not None:
         payload["properties"]["encryption"][
             "requireInfrastructureEncryption"
         ] = require_infrastructure_encryption
 
     if immutability_policy is not None:
         payload["properties"]["immutableStorageWithVersioning"] = {}
@@ -411,14 +457,19 @@
         )
 
     if sas_policy is not None:
         payload["properties"]["sasPolicy"] = convert_present_to_raw_sas_policy(
             hub, policy=sas_policy
         )
 
+    if key_policy is not None:
+        payload["properties"]["keyPolicy"] = convert_present_to_raw_key_policy(
+            hub, policy=key_policy
+        )
+
     if allowed_copy_scope is not None:
         payload["properties"]["allowedCopyScope"] = allowed_copy_scope
 
     if sftp_enabled is not None:
         payload["properties"]["isSftpEnabled"] = sftp_enabled
 
     return payload
@@ -604,15 +655,17 @@
     ):
         new_payload["properties"]["isNfsV3Enabled"] = new_values.get("nfsv3_enabled")
         need_update = True
 
     if (new_values.get("custom_domain") is not None) and (
         existing_payload.get("properties") is not None
     ):
-        existing_custom_domain = existing_payload.get("properties").get("customDomain")
+        existing_custom_domain = existing_payload.get("properties").get(
+            "customDomain", {}
+        )
         existing_custom_domain_required_payload = convert_raw_to_present_custom_domain(
             hub, c_domain=existing_custom_domain
         )
         if compare_update_dict_payload(
             existing_custom_domain_required_payload, new_values.get("custom_domain")
         ):
             new_payload["properties"][
@@ -621,50 +674,92 @@
                 hub, c_domain=new_values.get("custom_domain")
             )
             need_update = True
     if (new_values.get("customer_managed_key") is not None) and (
         existing_payload.get("properties") is not None
     ):
         existing_customer_managed_key = existing_payload.get("properties").get(
-            "encryption"
+            "encryption", {}
         )
         existing_customer_managed_key_required_payload = (
             convert_raw_to_present_customer_managed_key(
                 hub, customer_key=existing_customer_managed_key
             )
         )
         if compare_update_dict_payload(
             existing_customer_managed_key_required_payload,
             new_values.get("customer_managed_key"),
         ):
-            new_payload["properties"]["encryption"]["identity"][
-                "userAssignedIdentity"
-            ] = new_values.get("customer_managed_key").get("user_assigned_identity_id")
-            new_payload["properties"]["encryption"]["keyvaultproperties"][
-                "currentVersionedKeyIdentifier"
-            ] = new_values.get("customer_managed_key").get("key_vault_key_id")
+            if (
+                new_values.get("customer_managed_key", {}).get(
+                    "user_assigned_identity_id"
+                )
+                is not None
+            ):
+                new_payload["properties"]["encryption"]["identity"][
+                    "userAssignedIdentity"
+                ] = new_values.get("customer_managed_key").get(
+                    "user_assigned_identity_id"
+                )
+
+            if (
+                new_values.get("customer_managed_key", {}).get("key_vault_key_id")
+                is not None
+            ):
+                new_payload["properties"]["encryption"]["keyvaultproperties"] = {
+                    "currentVersionedKeyIdentifier": new_values.get(
+                        "customer_managed_key"
+                    ).get("key_vault_key_id"),
+                }
+
+            if new_values.get("customer_managed_key", {}).get("key_name") is not None:
+                new_payload["properties"]["encryption"]["keyvaultproperties"] = {
+                    "keyname": new_values.get("customer_managed_key").get("key_name"),
+                }
+
+            if (
+                new_values.get("customer_managed_key", {}).get("key_version")
+                is not None
+            ):
+                new_payload["properties"]["encryption"]["keyvaultproperties"] = {
+                    "keyversion": new_values.get("customer_managed_key").get(
+                        "key_version"
+                    ),
+                }
+
+            if (
+                new_values.get("customer_managed_key", {}).get("key_vault_uri")
+                is not None
+            ):
+                new_payload["properties"]["encryption"]["keyvaultproperties"] = {
+                    "keyvaulturi": new_values.get("customer_managed_key").get(
+                        "key_vault_uri"
+                    ),
+                }
             need_update = True
 
     if new_values.get("identity") is not None:
-        existing_identity = existing_payload.get("identity")
+        existing_identity = existing_payload.get("identity", {})
         existing_identity_required_payload = convert_raw_to_present_identity(
             hub, identity=existing_identity
         )
         if compare_update_dict_payload(
             existing_identity_required_payload, new_values.get("identity")
         ):
             new_payload["identity"] = convert_present_to_raw_identity(
                 hub, identity=new_values.get("identity")
             )
             need_update = True
 
     if (new_values.get("network_rules") is not None) and (
         existing_payload.get("properties") is not None
     ):
-        existing_network_rules = existing_payload.get("properties").get("networkAcls")
+        existing_network_rules = existing_payload.get("properties").get(
+            "networkAcls", {}
+        )
         existing_network_rules_required_payload = convert_raw_to_present_network_rules(
             hub, rules=existing_network_rules
         )
         if compare_update_dict_payload(
             existing_network_rules_required_payload, new_values.get("network_rules")
         ):
             new_payload["properties"][
@@ -687,15 +782,15 @@
         )
         need_update = True
 
     if (new_values.get("azure_files_authentication") is not None) and (
         existing_payload.get("properties") is not None
     ):
         existing_files_authentication = existing_payload.get("properties").get(
-            "azureFilesIdentityBasedAuthentication"
+            "azureFilesIdentityBasedAuthentication", {}
         )
         existing_files_authentication_required_payload = (
             convert_raw_to_present_files_authentication(
                 hub, file_auth=existing_files_authentication
             )
         )
         if compare_update_dict_payload(
@@ -708,15 +803,17 @@
                 hub, file_auth=new_values.get("azure_files_authentication")
             )
             need_update = True
 
     if (new_values.get("routing") is not None) and (
         existing_payload.get("properties") is not None
     ):
-        existing_routing = existing_payload.get("properties").get("routingPreference")
+        existing_routing = existing_payload.get("properties").get(
+            "routingPreference", {}
+        )
         existing_routing_required_payload = convert_raw_to_present_routing(
             hub, routing_pref=existing_routing
         )
         if compare_update_dict_payload(
             existing_routing_required_payload, new_values.get("routing")
         ):
             new_payload["properties"][
@@ -726,15 +823,15 @@
             )
             need_update = True
 
     if (new_values.get("encryption_service") is not None) and (
         existing_payload.get("properties") is not None
     ):
         existing_encryption_service = existing_payload.get("properties").get(
-            "encryption"
+            "encryption", {}
         )
         existing_encryption_service_required_payload = (
             convert_raw_to_present_encryption_service(
                 hub, encryption_service=existing_encryption_service
             )
         )
         if compare_update_dict_payload(
@@ -744,38 +841,57 @@
             new_payload["properties"]["encryption"]["keySource"] = new_values.get(
                 "encryption_service"
             ).get("encryption_key_source")
             if (
                 existing_payload.get("properties").get("encryption").get("services")
                 is not None
             ):
+                new_services = {}
                 if (
-                    existing_payload.get("properties")
-                    .get("encryption")
-                    .get("services")
-                    .get("queue")
-                    is not None
-                ):
-                    new_payload["properties"]["encryption"]["services"]["queue"][
-                        "keyType"
-                    ] = new_values.get("encryption_service").get(
+                    new_values.get("encryption_service").get(
                         "queue_encryption_key_type"
                     )
-                if (
-                    existing_payload.get("properties")
-                    .get("encryption")
-                    .get("services")
-                    .get("table")
                     is not None
                 ):
-                    new_payload["properties"]["encryption"]["services"]["table"][
-                        "keyType"
-                    ] = new_values.get("encryption_service").get(
+                    new_services["queue"] = {
+                        "keyType": new_values.get("encryption_service").get(
+                            "queue_encryption_key_type"
+                        )
+                    }
+                if (
+                    new_values.get("encryption_service").get(
                         "table_encryption_key_type"
                     )
+                    is not None
+                ):
+                    new_services["table"] = {
+                        "keyType": new_values.get("encryption_service").get(
+                            "table_encryption_key_type"
+                        ),
+                    }
+                if (
+                    new_values.get("encryption_service").get("blob_encryption_key_type")
+                    is not None
+                ):
+                    new_services["blob"] = {
+                        "keyType": new_values.get("encryption_service").get(
+                            "blob_encryption_key_type"
+                        ),
+                    }
+                if (
+                    new_values.get("encryption_service").get("file_encryption_key_type")
+                    is not None
+                ):
+                    new_services["file"] = {
+                        "keyType": new_values.get("encryption_service").get(
+                            "file_encryption_key_type"
+                        ),
+                    }
+                if new_services:
+                    new_payload["properties"]["encryption"]["services"] = new_services
             need_update = True
 
     if (
         (new_values.get("require_infrastructure_encryption") is not None)
         and (existing_payload.get("properties") is not None)
         and (existing_payload.get("properties").get("encryption") is not None)
         and (
@@ -794,15 +910,15 @@
         (new_values.get("immutability_policy") is not None)
         and (existing_payload.get("properties") is not None)
         and (existing_payload.get("immutableStorageWithVersioning") is not None)
     ):
         existing_immutability_policy = (
             existing_payload.get("properties")
             .get("immutableStorageWithVersioning")
-            .get("immutabilityPolicy")
+            .get("immutabilityPolicy", {})
         )
         existing_immutability_policy_required_payload = (
             convert_raw_to_present_immutability_policy(
                 hub, immute_policy=existing_immutability_policy
             )
         )
         if compare_update_dict_payload(
@@ -815,26 +931,41 @@
                 hub, immute_policy=new_values.get("immutability_policy")
             )
             need_update = True
 
     if (new_values.get("sas_policy") is not None) and (
         existing_payload.get("properties") is not None
     ):
-        existing_sas_policy = existing_payload.get("properties").get(".sasPolicy")
+        existing_sas_policy = existing_payload.get("properties").get("sasPolicy", {})
         existing_sas_policy_required_payload = convert_raw_to_present_sas_policy(
             hub, policy=existing_sas_policy
         )
         if compare_update_dict_payload(
             existing_sas_policy_required_payload, new_values.get("sas_policy")
         ):
             new_payload["properties"]["sasPolicy"] = convert_present_to_raw_sas_policy(
                 hub, policy=new_values.get("sas_policy")
             )
             need_update = True
 
+    if (new_values.get("key_policy") is not None) and (
+        existing_payload.get("properties") is not None
+    ):
+        existing_key_policy = existing_payload.get("properties").get("keyPolicy", {})
+        existing_key_policy_required_payload = convert_raw_to_present_key_policy(
+            hub, policy=existing_key_policy
+        )
+        if compare_update_dict_payload(
+            existing_key_policy_required_payload, new_values.get("key_policy")
+        ):
+            new_payload["properties"]["keyPolicy"] = convert_present_to_raw_key_policy(
+                hub, policy=new_values.get("key_policy")
+            )
+            need_update = True
+
     if (
         (new_values.get("allowed_copy_scope") is not None)
         and (existing_payload.get("properties") is not None)
         and (
             new_values["allowed_copy_scope"]
             != existing_payload.get("properties").get("allowedCopyScope")
         )
@@ -896,17 +1027,19 @@
 
     Args:
         c_domain(Dict, optional): Custom Disk payload in a storage account resource.
 
     Returns:
          Custom Domain payload that contains the parameters that match respective present function's input format.
     """
-    custom_domain_payload = {
-        "name": c_domain.get("name"),
-    }
+    custom_domain_payload = {}
+
+    if c_domain.get("name") is not None:
+        custom_domain_payload["name"] = c_domain.get("name")
+
     if c_domain.get("useSubDomainName") is not None:
         custom_domain_payload["use_subdomain"] = c_domain.get("useSubDomainName")
 
     return custom_domain_payload
 
 
 def convert_raw_to_present_customer_managed_key(hub, customer_key: Dict[str, Any]):
@@ -916,46 +1049,61 @@
 
     Args:
         customer_key(Dict, optional): customer key payload in a storage account resource.
 
     Returns:
          customer key payload that contains the parameters that match respective present function's input format.
     """
-    customer_key_payload = {}
-    if customer_key.get("keyvaultproperties") and customer_key.get(
-        "keyvaultproperties"
-    ).get("currentVersionedKeyIdentifier"):
-        customer_key_payload["key_vault_key_id"] = customer_key.get(
+    customer_key_present = {}
+
+    if customer_key.get("keyvaultproperties") is not None:
+        customer_key_present["key_vault_key_id"] = customer_key.get(
             "keyvaultproperties"
         ).get("currentVersionedKeyIdentifier")
+        customer_key_present["key_name"] = customer_key.get("keyvaultproperties").get(
+            "keyname"
+        )
+        customer_key_present["key_version"] = customer_key.get(
+            "keyvaultproperties"
+        ).get("keyversion")
+        customer_key_present["key_vault_uri"] = customer_key.get(
+            "keyvaultproperties"
+        ).get("keyvaulturi")
 
-    if customer_key.get("identity") and customer_key.get("identity").get(
-        "userAssignedIdentity"
-    ):
-        customer_key_payload["user_assigned_identity_id"] = customer_key.get(
+    if customer_key.get("identity") is not None:
+        customer_key_present["user_assigned_identity_id"] = customer_key.get(
             "identity"
         ).get("userAssignedIdentity")
+        customer_key_present["federated_identity_client_id"] = customer_key.get(
+            "identity"
+        ).get("federatedIdentityClientId")
+
+    customer_key_present = {
+        k: v for k, v in customer_key_present.items() if v is not None
+    }
 
-    return customer_key_payload
+    return customer_key_present
 
 
 def convert_raw_to_present_identity(hub, identity: Dict[str, Any]):
     """
      Giving an existing resource state and desired state inputs, generate a Dict that match the format of
      present input parameters.
 
     Args:
         identity(Dict, optional): Identity payload in a storage account resource.
 
     Returns:
          Identity payload that contains the parameters that match respective present function's input format.
     """
-    identity_payload = {
-        "type": identity.get("type"),
-    }
+    identity_payload = {}
+
+    if identity.get("type") is not None:
+        identity_payload["type"] = identity.get("type")
+
     if identity.get("userAssignedIdentities") is not None:
         identity_payload["user_assigned_identities"] = identity.get(
             "userAssignedIdentities"
         ).copy()
 
     return identity_payload
 
@@ -967,41 +1115,72 @@
 
     Args:
         policy(Dict, optional): sas policy payload in a storage account resource.
 
     Returns:
          sas policy payload that contains the parameters that match respective present function's input format.
     """
-    sas_policy_payload = {
-        "expiration_period": policy.get["sasExpirationPeriod"],
-    }
+    sas_policy_payload = {}
+
+    if policy.get("sasExpirationPeriod") is not None:
+        sas_policy_payload["expiration_period"] = policy["sasExpirationPeriod"]
+
     if policy.get("expirationAction") is not None:
         sas_policy_payload["expiration_action"] = policy["expirationAction"]
 
     return sas_policy_payload
 
 
+def convert_raw_to_present_key_policy(hub, policy: Dict[str, Any]):
+    """
+     Giving an existing resource state and desired state inputs, generate a Dict that match the format of
+     present input parameters.
+
+    Args:
+        policy(Dict, optional): key policy payload in a storage account resource.
+
+    Returns:
+         key policy payload that contains the parameters that match respective present function's input format.
+    """
+    key_policy_payload = {}
+
+    if policy.get("keyExpirationPeriodInDays") is not None:
+        key_policy_payload["key_expiration_period_in_days"] = policy.get(
+            "keyExpirationPeriodInDays"
+        )
+
+    return key_policy_payload
+
+
 def convert_raw_to_present_immutability_policy(hub, immutePolicy: Dict[str, Any]):
     """
      Giving an existing resource state and desired state inputs, generate a Dict that match the format of
      present input parameters.
 
      Args:
          immutePolicy(Dict, optional): immutability policy payload in a storage account resource.
 
     Returns:
         immutability policy payload that contains the parameters that match respective present function's input format.
     """
-    immutability_policy_payload = {
-        "allow_protected_append_writes": immutePolicy["allowProtectedAppendWrites"],
-        "state": immutePolicy["state"],
-        "period_since_creation_in_days": immutePolicy[
+    immutability_policy_payload = {}
+
+    if immutePolicy.get("allowProtectedAppendWrites") is not None:
+        immutability_policy_payload["allow_protected_append_writes"] = immutePolicy.get(
+            "allowProtectedAppendWrites"
+        )
+
+    if immutePolicy.get("state") is not None:
+        immutability_policy_payload["state"] = immutePolicy.get("state")
+
+    if immutePolicy.get("immutabilityPeriodSinceCreationInDays") is not None:
+        immutability_policy_payload["period_since_creation_in_days"] = immutePolicy.get(
             "immutabilityPeriodSinceCreationInDays"
-        ],
-    }
+        )
+
     return immutability_policy_payload
 
 
 def convert_raw_to_present_routing(hub, routing_pref: Dict[str, Any]):
     """
      Giving an existing resource state and desired state inputs, generate a Dict that match the format of
      present input parameters.
@@ -1037,91 +1216,135 @@
     Args:
         encryption_service(Dict, optional): encryption service payload in a storage account resource.
 
     Returns:
          encryption service payload that contains the parameters that match respective present function's input format.
     """
     encryption_service_payload = {}
-    if encryption_service.get("keySource"):
+    if encryption_service.get("keySource") is not None:
         encryption_service_payload["encryption_key_source"] = encryption_service.get(
             "keySource"
         )
 
     if (
-        (encryption_service.get("services"))
-        and (encryption_service.get("services").get("queue"))
-        and (encryption_service.get("services").get("queue").get("keyType"))
+        (encryption_service.get("services") is not None)
+        and (encryption_service.get("services").get("queue") is not None)
+        and (encryption_service.get("services").get("queue").get("keyType") is not None)
     ):
-        encryption_service["queue_encryption_key_type"] = (
+        encryption_service_payload["queue_encryption_key_type"] = (
             encryption_service.get("services").get("queue").get("keyType")
         )
 
     if (
-        (encryption_service.get("services"))
-        and (encryption_service.get("services").get("table"))
-        and (encryption_service.get("services").get("table").get("keyType"))
+        (encryption_service.get("services") is not None)
+        and (encryption_service.get("services").get("table") is not None)
+        and (encryption_service.get("services").get("table").get("keyType") is not None)
     ):
-        encryption_service["table_encryption_key_type"] = (
+        encryption_service_payload["table_encryption_key_type"] = (
             encryption_service.get("services").get("table").get("keyType")
         )
 
+    if (
+        (encryption_service.get("services") is not None)
+        and (encryption_service.get("services").get("blob") is not None)
+        and (encryption_service.get("services").get("blob").get("keyType") is not None)
+    ):
+        encryption_service_payload["blob_encryption_key_type"] = (
+            encryption_service.get("services").get("blob").get("keyType")
+        )
+
+    if (
+        (encryption_service.get("services") is not None)
+        and (encryption_service.get("services").get("file") is not None)
+        and (encryption_service.get("services").get("file").get("keyType") is not None)
+    ):
+        encryption_service_payload["file_encryption_key_type"] = (
+            encryption_service.get("services").get("file").get("keyType")
+        )
+
     return encryption_service_payload
 
 
 def convert_raw_to_present_files_authentication(hub, file_auth: Dict[str, Any]):
     """
     Giving an existing resource state and desired state inputs, generate a Dict that match the format of
     present input parameters.
 
     Args:
         file_auth(Dict, optional): file authentication payload in a storage account resource.
 
     Returns:
         file authentication payload that contains the parameters that match respective present function's input format.
     """
-    files_authentication_payload = {
-        "directory_service_options": file_auth["directoryServiceOptions"],
-    }
+    files_authentication_payload = {}
+
+    if file_auth.get("directoryServiceOptions") is not None:
+        files_authentication_payload["directory_service_options"] = file_auth.get(
+            "directoryServiceOptions"
+        )
+
+    if file_auth.get("defaultSharePermission") is not None:
+        files_authentication_payload["default_share_permission"] = file_auth.get(
+            "defaultSharePermission"
+        )
 
     if file_auth.get("activeDirectoryProperties") is not None:
         active_directory_payload = covert_raw_to_present_active_directory(
             hub, directory_properties=file_auth.get("activeDirectoryProperties")
         )
         files_authentication_payload[
             "active_directory_properties"
         ] = active_directory_payload
     return files_authentication_payload
 
 
 def covert_raw_to_present_active_directory(hub, directory_properties: Dict[str, Any]):
-    current_directory_payload = {
-        "azure_storage_sid": directory_properties["azureStorageSid"],
-        "domain_name": directory_properties["domainName"],
-        "domain_sid": directory_properties["domainSid"],
-        "domain_guid": directory_properties["domainGuid"],
-        "forest_name": directory_properties["forestName"],
-        "netbios_domain_name": directory_properties["netBiosDomainName"],
-    }
+    current_directory_payload = {}
+
+    if directory_properties.get("domainName") is not None:
+        current_directory_payload["domain_name"] = directory_properties["domainName"]
+
+    if directory_properties.get("domainGuid") is not None:
+        current_directory_payload["domain_guid"] = directory_properties["domainGuid"]
+
+    if directory_properties.get("azureStorageSid") is not None:
+        current_directory_payload["azure_storage_sid"] = directory_properties[
+            "azureStorageSid"
+        ]
+
+    if directory_properties.get("domainSid") is not None:
+        current_directory_payload["domain_sid"] = directory_properties["domainSid"]
+
+    if directory_properties.get("forestName") is not None:
+        current_directory_payload["forest_name"] = directory_properties["forestName"]
+
+    if directory_properties.get("netBiosDomainName") is not None:
+        current_directory_payload["netbios_domain_name"] = directory_properties[
+            "netBiosDomainName"
+        ]
+
     return current_directory_payload
 
 
 def convert_raw_to_present_network_rules(hub, rules: Dict[str, Any]):
     """
     Giving an existing resource state and desired state inputs, generate a Dict that match the format of
     present input parameters.
 
     Args:
         rules(Dict, optional): network rules payload in a storage account resource.
 
     Returns:
        network rules payload that contains the parameters that match respective present function's input format.
     """
-    network_rule_payload = {
-        "default_action": rules["defaultAction"],
-    }
+    network_rule_payload = {}
+
+    if rules.get("defaultAction") is not None:
+        network_rule_payload["default_action"] = rules.get("defaultAction")
+
     if rules.get("bypass") is not None:
         network_rule_payload["bypass"] = rules["bypass"]
 
     if rules.get("ipRules") is not None:
         ip = []
         for ip_rule in rules["ipRules"]:
             ip.append(ip_rule.get("value"))
@@ -1168,15 +1391,15 @@
     Returns:
         Custom Domain Payload Dict[str,any] in the format of an Azure PUT operation payload.
     """
     custom_domain_payload = {
         "name": c_domain.get("name"),
     }
 
-    if c_domain.get("use_subdomain"):
+    if c_domain.get("use_subdomain") is not None:
         custom_domain_payload["useSubDomainName"] = c_domain["use_subdomain"]
 
     return custom_domain_payload
 
 
 def convert_present_to_raw_identity(hub, identity: Dict[str, Any]):
     """
@@ -1189,15 +1412,15 @@
     Returns:
         identity Payload Dict[str,any] in the format of an Azure PUT operation payload.
     """
     identity_payload = {
         "type": identity.get("type"),
     }
 
-    if identity.get("user_assigned_identities"):
+    if identity.get("user_assigned_identities") is not None:
         identity_payload["userAssignedIdentities"] = identity.get(
             "user_assigned_identities"
         ).copy()
 
         return identity_payload
 
 
@@ -1212,20 +1435,38 @@
     Returns:
         Sas Policy Payload Dict[str,any] in the format of an Azure PUT operation payload.
     """
     sas_policy_payload = {
         "sasExpirationPeriod": policy.get("expiration_period"),
     }
 
-    if policy.get("expiration_action"):
+    if policy.get("expiration_action") is not None:
         sas_policy_payload["expirationAction"] = policy["expiration_action"]
 
     return sas_policy_payload
 
 
+def convert_present_to_raw_key_policy(hub, policy: Dict[str, Any]):
+    """
+    Giving some present function inputs, generate a payload that can be used during PUT operation to Azure. Any None
+    value input will be ignored, unless this parameter is a required input parameter.
+
+    Args:
+        policy(Dict(str, Any)) :
+
+    Returns:
+        Key Policy Payload Dict[str,any] in the format of an Azure PUT operation payload.
+    """
+    key_policy_payload = {
+        "keyExpirationPeriodInDays": policy.get("key_expiration_period_in_days"),
+    }
+
+    return key_policy_payload
+
+
 def convert_present_to_raw_immutability_policy(hub, immute_policy: Dict[str, Any]):
     """
     Giving some present function inputs, generate a payload that can be used during PUT operation to Azure. Any None
     value input will be ignored, unless this parameter is a required input parameter.
 
     Args:
         immute_policy(Dict(str, Any)) :
@@ -1252,25 +1493,25 @@
         routing_pref(Dict(str, Any)) :
 
     Returns:
         Routing Payload Dict[str,any] in the format of an Azure PUT operation payload.
     """
     routing_payload = {}
 
-    if routing_pref.get("publish_internet_endpoints"):
+    if routing_pref.get("publish_internet_endpoints") is not None:
         routing_payload["publishInternetEndpoints"] = routing_pref[
             "publish_internet_endpoints"
         ]
 
-    if routing_pref.get("publish_microsoft_endpoints"):
+    if routing_pref.get("publish_microsoft_endpoints") is not None:
         routing_payload["publishMicrosoftEndpoints"] = routing_pref[
             "publish_microsoft_endpoints"
         ]
 
-    if routing_pref.get("routing_choice"):
+    if routing_pref.get("routing_choice") is not None:
         routing_payload["routingChoice"] = routing_pref["routing_choice"]
     return routing_payload
 
 
 def convert_present_to_raw_files_authentication(hub, file_auth: Dict[str, Any]):
     """
     Giving some present function inputs, generate a payload that can be used during PUT operation to Azure. Any None
@@ -1279,35 +1520,53 @@
     Args:
        file_auth(Dict(str, Any)) :
 
     Returns:
         file authentication Payload Dict[str,any] in the format of an Azure PUT operation payload.
     """
     files_authentication_payload = {
-        "directoryServiceOptions": file_auth["directory_service_options"],
+        "directoryServiceOptions": file_auth["directory_service_options"]
     }
 
+    if file_auth.get("default_share_permission"):
+        files_authentication_payload["defaultSharePermission"] = file_auth.get(
+            "default_share_permission"
+        )
+
     if file_auth.get("active_directory_properties"):
         files_authentication_payload[
             "activeDirectoryProperties"
         ] = convert_present_to_raw_active_directory(
             hub, directory_properties=file_auth.get("active_directory_properties")
         )
     return files_authentication_payload
 
 
 def convert_present_to_raw_active_directory(hub, directory_properties: Dict[str, Any]):
     current_directory_payload = {
-        "azureStorageSid": directory_properties["azure_storage_sid"],
         "domainName": directory_properties["domain_name"],
-        "domainSid": directory_properties["domain_sid"],
         "domainGuid": directory_properties["domain_guid"],
-        "forestName": directory_properties["forest_name"],
-        "netBiosDomainName": directory_properties["netbios_domain_name"],
     }
+
+    if directory_properties.get("azure_storage_sid") is not None:
+        current_directory_payload["azureStorageSid"] = directory_properties[
+            "azure_storage_sid"
+        ]
+
+    if directory_properties.get("domain_sid") is not None:
+        current_directory_payload["domainSid"] = directory_properties["domain_sid"]
+
+    if directory_properties.get("forest_name") is not None:
+        current_directory_payload["forestName"] = directory_properties["forest_name"]
+
+    if directory_properties.get("netbios_domain_name") is not None:
+        current_directory_payload["netBiosDomainName"] = directory_properties[
+            "netbios_domain_name"
+        ]
+
     return current_directory_payload
 
 
 def convert_present_to_raw_network_rules(hub, rules: Dict[str, Any]):
     """
     Giving some present function inputs, generate a payload that can be used during PUT operation to Azure. Any None
     value input will be ignored, unless this parameter is a required input parameter.
@@ -1318,32 +1577,32 @@
     Returns:
        Network rules Payload Dict[str,any] in the format of an Azure PUT operation payload.
     """
     network_rule_payload = {
         "defaultAction": rules["default_action"],
     }
 
-    if rules.get("bypass"):
+    if rules.get("bypass") is not None:
         network_rule_payload["bypass"] = rules["bypass"]
 
-    if rules.get("ip_rule_values"):
+    if rules.get("ip_rule_values") is not None:
         ipRuleList = []
         for value in rules["ip_rule_values"]:
             ipRuleList.append({"action": "Allow", "value": value})
         network_rule_payload["ipRules"] = ipRuleList
 
-    if rules.get("virtual_network_subnet_ids"):
+    if rules.get("virtual_network_subnet_ids") is not None:
         virtualNetworkRuleList = []
         for id in rules["virtual_network_subnet_ids"]:
             virtualNetworkRuleList.append(
                 {"action": "Allow", "id": id, "state": "Succeeded"}
             )
         network_rule_payload["virtualNetworkRules"] = virtualNetworkRuleList
 
-    if rules.get("resource_access_rules"):
+    if rules.get("resource_access_rules") is not None:
         network_rule_payload[
             "resourceAccessRules"
         ] = convert_present_to_raw_resource_access_rules(
             hub, resource_access=rules.get("resource_access_rules")
         )
 
     return network_rule_payload
@@ -1354,12 +1613,12 @@
 ):
     raw_access_rules = []
 
     for access_rule in resource_access:
         payload = {
             "resourceId": access_rule["endpoint_resource_id"],
         }
-        if access_rule.get("endpoint_tenant_id"):
+        if access_rule.get("endpoint_tenant_id") is not None:
             payload["tenantId"] = access_rule["endpoint_tenant_id"]
         raw_access_rules.append(payload)
 
     return raw_access_rules
```

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/storage_resource_provider/storage_blob.py` & `idem-azure-0.4.0/idem_azure/tool/azure/storage_resource_provider/storage_blob.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/subscription/subscriptions.py` & `idem-azure-0.4.0/idem_azure/tool/azure/subscription/subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/test_state_utils.py` & `idem-azure-0.4.0/idem_azure/tool/azure/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/azure/uri.py` & `idem-azure-0.4.0/idem_azure/tool/azure/uri.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure/tool/validators/http.py` & `idem-azure-0.4.0/idem_azure/tool/validators/http.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.4/idem_azure.egg-info/PKG-INFO` & `idem-azure-0.4.0/idem_azure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-azure
-Version: 0.3.4
+Version: 0.4.0
 Summary: UNKNOWN
 Home-page: https://gitlab.com/vmware/idem/idem-azure
 Author: Yingzhi Hao
 Author-email: hyingzhi@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-azure-0.3.4/idem_azure.egg-info/SOURCES.txt` & `idem-azure-0.4.0/idem_azure.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 idem_azure/exec/azure/network/network_interfaces.py
 idem_azure/exec/azure/network/network_security_groups.py
 idem_azure/exec/azure/network/public_ip_addresses.py
 idem_azure/exec/azure/network/route_tables.py
 idem_azure/exec/azure/network/routes.py
 idem_azure/exec/azure/network/security_rules.py
 idem_azure/exec/azure/network/subnets.py
+idem_azure/exec/azure/network/virtual_network_peerings.py
 idem_azure/exec/azure/network/virtual_networks.py
 idem_azure/exec/azure/policy/policy_assignments.py
 idem_azure/exec/azure/policy/policy_definitions.py
 idem_azure/exec/azure/resource_management/resource_groups.py
+idem_azure/exec/azure/sql_database/databases.py
 idem_azure/exec/azure/storage_resource_provider/storage_accounts.py
 idem_azure/exec/azure/storage_resource_provider/storage_blob.py
 idem_azure/exec/azure/subscription/attach_subscriptions.py
 idem_azure/exec/azure/subscription/subscriptions.py
 idem_azure/pop_create/azure/api_reference.py
 idem_azure/pop_create/azure/api_spec.py
 idem_azure/pop_create/azure/init.py
@@ -60,26 +62,34 @@
 idem_azure/states/azure/network/network_interfaces.py
 idem_azure/states/azure/network/network_security_groups.py
 idem_azure/states/azure/network/public_ip_addresses.py
 idem_azure/states/azure/network/route_tables.py
 idem_azure/states/azure/network/routes.py
 idem_azure/states/azure/network/security_rules.py
 idem_azure/states/azure/network/subnets.py
+idem_azure/states/azure/network/virtual_network_peerings.py
 idem_azure/states/azure/network/virtual_networks.py
 idem_azure/states/azure/policy/policy_assignments.py
 idem_azure/states/azure/policy/policy_definitions.py
+idem_azure/states/azure/recursive_contracts/init.py
 idem_azure/states/azure/resource_management/resource_groups.py
+idem_azure/states/azure/sql_database/databases.py
 idem_azure/states/azure/storage_resource_provider/storage_accounts.py
 idem_azure/states/azure/storage_resource_provider/storage_blob.py
 idem_azure/states/azure/subscription/attach_subscriptions.py
 idem_azure/states/azure/subscription/subscriptions.py
+idem_azure/tool/azure/comment_utils.py
 idem_azure/tool/azure/container.py
+idem_azure/tool/azure/generic.py
+idem_azure/tool/azure/polling.py
 idem_azure/tool/azure/request.py
+idem_azure/tool/azure/resource_utils.py
 idem_azure/tool/azure/test_state_utils.py
 idem_azure/tool/azure/uri.py
+idem_azure/tool/azure/utils.py
 idem_azure/tool/azure/authorization/role_assignments.py
 idem_azure/tool/azure/authorization/role_definitions.py
 idem_azure/tool/azure/compute/log_analytics_workspace.py
 idem_azure/tool/azure/compute/virtual_machines.py
 idem_azure/tool/azure/key_vault/vault.py
 idem_azure/tool/azure/management_groups/management_groups.py
 idem_azure/tool/azure/network/firewall.py
@@ -87,15 +97,17 @@
 idem_azure/tool/azure/network/network_interfaces.py
 idem_azure/tool/azure/network/network_security_groups.py
 idem_azure/tool/azure/network/public_ip_addresses.py
 idem_azure/tool/azure/network/route_tables.py
 idem_azure/tool/azure/network/routes.py
 idem_azure/tool/azure/network/security_rules.py
 idem_azure/tool/azure/network/subnets.py
+idem_azure/tool/azure/network/virtual_network_peerings.py
 idem_azure/tool/azure/network/virtual_networks.py
 idem_azure/tool/azure/policy/policy_assignment.py
 idem_azure/tool/azure/policy/policy_definition.py
 idem_azure/tool/azure/resource_management/resource_groups.py
+idem_azure/tool/azure/sql_database/databases.py
 idem_azure/tool/azure/storage_resource_provider/storage_accounts.py
 idem_azure/tool/azure/storage_resource_provider/storage_blob.py
 idem_azure/tool/azure/subscription/subscriptions.py
 idem_azure/tool/validators/http.py
```

### Comparing `idem-azure-0.3.4/setup.py` & `idem-azure-0.4.0/setup.py`

 * *Files identical despite different names*

