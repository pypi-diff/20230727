# Comparing `tmp/pulumi_rancher2-5.1.0a1689400040.tar.gz` & `tmp/pulumi_rancher2-5.1.0a1690482743.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rancher2-5.1.0a1689400040.tar", last modified: Sat Jul 15 05:52:30 2023, max compression
+gzip compressed data, was "pulumi_rancher2-5.1.0a1690482743.tar", last modified: Thu Jul 27 18:37:56 2023, max compression
```

## Comparing `pulumi_rancher2-5.1.0a1689400040.tar` & `pulumi_rancher2-5.1.0a1690482743.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:52:30.533661 pulumi_rancher2-5.1.0a1689400040/
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-15 05:52:30.533661 pulumi_rancher2-5.1.0a1689400040/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:52:30.533661 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1287716 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/active_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    39478 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/app_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    81893 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_active_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_adfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_azure_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    74864 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_free_ipa.py
--rw-r--r--   0 runner    (1001) docker     (123)    26284 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    37428 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_keycloak.py
--rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_okta.py
--rw-r--r--   0 runner    (1001) docker     (123)    74951 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_open_ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_ping.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    32734 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    34681 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    45103 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)   141124 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    39686 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25349 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_alter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_alter_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    31455 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    25028 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    41552 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:52:30.533661 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_catalog_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cloud_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    23570 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster_alter_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_config_map_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_etcd_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_global_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_node_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_node_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    29150 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_principal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_role_tempalte.py
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_role_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/global_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/global_dns_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/global_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/global_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    47168 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/machine_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41496 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/multi_cluster_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/node_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    31694 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/node_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    82407 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/node_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)  1602525 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    77219 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/pod_security_policy_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/project_alert_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    37710 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/project_alert_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/project_role_template_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/role_tempalte.py
--rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/role_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/secret_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    28125 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/storage_class_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:52:30.533661 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 05:52:30.533661 pulumi_rancher2-5.1.0a1689400040/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-15 05:52:30.000000 pulumi_rancher2-5.1.0a1689400040/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:37:56.699710 pulumi_rancher2-5.1.0a1690482743/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-27 18:37:56.699710 pulumi_rancher2-5.1.0a1690482743/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:37:56.695709 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1331725 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39478 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/app_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81893 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_active_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_adfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_azure_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74864 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_free_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26284 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37428 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35228 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74951 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_open_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36725 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32734 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34681 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45103 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154396 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25128 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39686 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25349 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_alter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35202 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_alter_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25480 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31455 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25028 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53172 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:37:56.699710 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32293 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/custom_user_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_catalog_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cloud_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24961 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster_alter_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_config_map_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_etcd_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_global_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_node_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29150 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_principal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_role_tempalte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_role_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23732 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/global_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/global_dns_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/global_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/global_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47168 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/machine_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41496 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/multi_cluster_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/node_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31694 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82407 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/node_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1650650 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77219 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/pod_security_policy_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37627 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/project_alert_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37710 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/project_alert_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25172 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/project_role_template_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21144 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/role_tempalte.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31809 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/role_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/secret_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28125 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/storage_class_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:37:56.699710 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 18:37:56.699710 pulumi_rancher2-5.1.0a1690482743/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-27 18:37:56.000000 pulumi_rancher2-5.1.0a1690482743/setup.py
```

### Comparing `pulumi_rancher2-5.1.0a1689400040/PKG-INFO` & `pulumi_rancher2-5.1.0a1690482743/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rancher2
-Version: 5.1.0a1689400040
+Version: 5.1.0a1690482743
 Summary: A Pulumi package for creating and managing rancher2 resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi rancher2
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rancher2-5.1.0a1689400040/README.md` & `pulumi_rancher2-5.1.0a1690482743/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/__init__.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from .cluster_alter_rule import *
 from .cluster_driver import *
 from .cluster_role_template_binding import *
 from .cluster_sync import *
 from .cluster_template import *
 from .cluster_v2 import *
 from .config_map_v2 import *
+from .custom_user_token import *
 from .etcd_backup import *
 from .feature import *
 from .get_app import *
 from .get_catalog import *
 from .get_catalog_v2 import *
 from .get_certificate import *
 from .get_cloud_credential import *
@@ -333,14 +334,22 @@
   "fqn": "pulumi_rancher2",
   "classes": {
    "rancher2:index/configMapV2:ConfigMapV2": "ConfigMapV2"
   }
  },
  {
   "pkg": "rancher2",
+  "mod": "index/customUserToken",
+  "fqn": "pulumi_rancher2",
+  "classes": {
+   "rancher2:index/customUserToken:CustomUserToken": "CustomUserToken"
+  }
+ },
+ {
+  "pkg": "rancher2",
   "mod": "index/etcdBackup",
   "fqn": "pulumi_rancher2",
   "classes": {
    "rancher2:index/etcdBackup:EtcdBackup": "EtcdBackup"
   }
  },
  {
```

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/_inputs.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,23 +29,29 @@
     'ClusterAlertRuleNodeRuleArgs',
     'ClusterAlertRuleSystemServiceRuleArgs',
     'ClusterAlterGroupRecipientArgs',
     'ClusterAlterRuleEventRuleArgs',
     'ClusterAlterRuleMetricRuleArgs',
     'ClusterAlterRuleNodeRuleArgs',
     'ClusterAlterRuleSystemServiceRuleArgs',
+    'ClusterClusterAgentDeploymentCustomizationArgs',
+    'ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs',
+    'ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs',
     'ClusterClusterAuthEndpointArgs',
     'ClusterClusterMonitoringInputArgs',
     'ClusterClusterRegistrationTokenArgs',
     'ClusterClusterTemplateAnswersArgs',
     'ClusterClusterTemplateQuestionArgs',
     'ClusterEksConfigArgs',
     'ClusterEksConfigV2Args',
     'ClusterEksConfigV2NodeGroupArgs',
     'ClusterEksConfigV2NodeGroupLaunchTemplateArgs',
+    'ClusterFleetAgentDeploymentCustomizationArgs',
+    'ClusterFleetAgentDeploymentCustomizationAppendTolerationArgs',
+    'ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirementArgs',
     'ClusterGkeConfigArgs',
     'ClusterGkeConfigV2Args',
     'ClusterGkeConfigV2ClusterAddonsArgs',
     'ClusterGkeConfigV2IpAllocationPolicyArgs',
     'ClusterGkeConfigV2MasterAuthorizedNetworksConfigArgs',
     'ClusterGkeConfigV2MasterAuthorizedNetworksConfigCidrBlockArgs',
     'ClusterGkeConfigV2NodePoolArgs',
@@ -105,14 +111,16 @@
     'ClusterRkeConfigPrivateRegistryArgs',
     'ClusterRkeConfigPrivateRegistryEcrCredentialPluginArgs',
     'ClusterRkeConfigServicesArgs',
     'ClusterRkeConfigServicesEtcdArgs',
     'ClusterRkeConfigServicesEtcdBackupConfigArgs',
     'ClusterRkeConfigServicesEtcdBackupConfigS3BackupConfigArgs',
     'ClusterRkeConfigServicesKubeApiArgs',
+    'ClusterRkeConfigServicesKubeApiAdmissionConfigurationArgs',
+    'ClusterRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs',
     'ClusterRkeConfigServicesKubeApiAuditLogArgs',
     'ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs',
     'ClusterRkeConfigServicesKubeApiEventRateLimitArgs',
     'ClusterRkeConfigServicesKubeApiSecretsEncryptionConfigArgs',
     'ClusterRkeConfigServicesKubeControllerArgs',
     'ClusterRkeConfigServicesKubeletArgs',
     'ClusterRkeConfigServicesKubeproxyArgs',
@@ -170,35 +178,44 @@
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigPrivateRegistryArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigPrivateRegistryEcrCredentialPluginArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcdArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcdBackupConfigArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcdBackupConfigS3BackupConfigArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiArgs',
+    'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationArgs',
+    'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLogArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLogConfigurationArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiEventRateLimitArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiSecretsEncryptionConfigArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeControllerArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeletArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeproxyArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesSchedulerArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigUpgradeStrategyArgs',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigUpgradeStrategyDrainInputArgs',
     'ClusterTemplateTemplateRevisionQuestionArgs',
     'ClusterV2AgentEnvVarArgs',
+    'ClusterV2ClusterAgentDeploymentCustomizationArgs',
+    'ClusterV2ClusterAgentDeploymentCustomizationAppendTolerationArgs',
+    'ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs',
     'ClusterV2ClusterRegistrationTokenArgs',
+    'ClusterV2FleetAgentDeploymentCustomizationArgs',
+    'ClusterV2FleetAgentDeploymentCustomizationAppendTolerationArgs',
+    'ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirementArgs',
     'ClusterV2LocalAuthEndpointArgs',
     'ClusterV2RkeConfigArgs',
     'ClusterV2RkeConfigEtcdArgs',
     'ClusterV2RkeConfigEtcdS3ConfigArgs',
     'ClusterV2RkeConfigEtcdSnapshotCreateArgs',
     'ClusterV2RkeConfigEtcdSnapshotRestoreArgs',
     'ClusterV2RkeConfigLocalAuthEndpointArgs',
     'ClusterV2RkeConfigMachinePoolArgs',
+    'ClusterV2RkeConfigMachinePoolDefaultArgs',
     'ClusterV2RkeConfigMachinePoolMachineConfigArgs',
     'ClusterV2RkeConfigMachinePoolRollingUpdateArgs',
     'ClusterV2RkeConfigMachinePoolTaintArgs',
     'ClusterV2RkeConfigMachineSelectorConfigArgs',
     'ClusterV2RkeConfigMachineSelectorConfigMachineLabelSelectorArgs',
     'ClusterV2RkeConfigMachineSelectorConfigMachineLabelSelectorMatchExpressionArgs',
     'ClusterV2RkeConfigRegistriesArgs',
@@ -1907,61 +1924,73 @@
 @pulumi.input_type
 class ClusterAksConfigV2NodePoolArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  availability_zones: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  count: Optional[pulumi.Input[int]] = None,
                  enable_auto_scaling: Optional[pulumi.Input[bool]] = None,
+                 labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  max_count: Optional[pulumi.Input[int]] = None,
                  max_pods: Optional[pulumi.Input[int]] = None,
+                 max_surge: Optional[pulumi.Input[str]] = None,
                  min_count: Optional[pulumi.Input[int]] = None,
                  mode: Optional[pulumi.Input[str]] = None,
                  orchestrator_version: Optional[pulumi.Input[str]] = None,
                  os_disk_size_gb: Optional[pulumi.Input[int]] = None,
                  os_disk_type: Optional[pulumi.Input[str]] = None,
                  os_type: Optional[pulumi.Input[str]] = None,
+                 taints: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  vm_size: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: The name of the Cluster (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] availability_zones: The AKS node pool availability zones (list)
         :param pulumi.Input[int] count: Number of machines (VMs) in the agent pool. Allowed values must be in the range of 1 to 100 (inclusive). Default `1` (int)
         :param pulumi.Input[bool] enable_auto_scaling: Is AKS node pool auto scaling enabled? Default: `false` (bool)
+        :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster (map)
         :param pulumi.Input[int] max_count: The AKS node pool max count. Required if `enable_auto_scaling=true` (int)
         :param pulumi.Input[int] max_pods: Maximum number of pods that can run on a node. Default `110` (int)
+        :param pulumi.Input[str] max_surge: Monitoring deployment rolling update max surge. Default: `1` (int)
         :param pulumi.Input[int] min_count: The AKS node pool min count. Required if `enable_auto_scaling=true` (int)
         :param pulumi.Input[str] mode: RKE mode for authorization. `rbac` and `none` modes are available. Default `rbac` (string)
         :param pulumi.Input[str] orchestrator_version: The AKS node pool orchestrator version (string)
         :param pulumi.Input[int] os_disk_size_gb: The AKS node pool os disk size gb. Default: `128` (int)
         :param pulumi.Input[str] os_disk_type: The AKS node pool os disk type. Default: `Managed` (string)
         :param pulumi.Input[str] os_type: The AKS node pool os type. Default: `Linux` (string)
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] taints: The AKS node pool taints (list)
         :param pulumi.Input[str] vm_size: The AKS node pool orchestrator version (string)
         """
         pulumi.set(__self__, "name", name)
         if availability_zones is not None:
             pulumi.set(__self__, "availability_zones", availability_zones)
         if count is not None:
             pulumi.set(__self__, "count", count)
         if enable_auto_scaling is not None:
             pulumi.set(__self__, "enable_auto_scaling", enable_auto_scaling)
+        if labels is not None:
+            pulumi.set(__self__, "labels", labels)
         if max_count is not None:
             pulumi.set(__self__, "max_count", max_count)
         if max_pods is not None:
             pulumi.set(__self__, "max_pods", max_pods)
+        if max_surge is not None:
+            pulumi.set(__self__, "max_surge", max_surge)
         if min_count is not None:
             pulumi.set(__self__, "min_count", min_count)
         if mode is not None:
             pulumi.set(__self__, "mode", mode)
         if orchestrator_version is not None:
             pulumi.set(__self__, "orchestrator_version", orchestrator_version)
         if os_disk_size_gb is not None:
             pulumi.set(__self__, "os_disk_size_gb", os_disk_size_gb)
         if os_disk_type is not None:
             pulumi.set(__self__, "os_disk_type", os_disk_type)
         if os_type is not None:
             pulumi.set(__self__, "os_type", os_type)
+        if taints is not None:
+            pulumi.set(__self__, "taints", taints)
         if vm_size is not None:
             pulumi.set(__self__, "vm_size", vm_size)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
@@ -2006,14 +2035,26 @@
         return pulumi.get(self, "enable_auto_scaling")
 
     @enable_auto_scaling.setter
     def enable_auto_scaling(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_auto_scaling", value)
 
     @property
+    @pulumi.getter
+    def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+        """
+        Labels for the Cluster (map)
+        """
+        return pulumi.get(self, "labels")
+
+    @labels.setter
+    def labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+        pulumi.set(self, "labels", value)
+
+    @property
     @pulumi.getter(name="maxCount")
     def max_count(self) -> Optional[pulumi.Input[int]]:
         """
         The AKS node pool max count. Required if `enable_auto_scaling=true` (int)
         """
         return pulumi.get(self, "max_count")
 
@@ -2030,14 +2071,26 @@
         return pulumi.get(self, "max_pods")
 
     @max_pods.setter
     def max_pods(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_pods", value)
 
     @property
+    @pulumi.getter(name="maxSurge")
+    def max_surge(self) -> Optional[pulumi.Input[str]]:
+        """
+        Monitoring deployment rolling update max surge. Default: `1` (int)
+        """
+        return pulumi.get(self, "max_surge")
+
+    @max_surge.setter
+    def max_surge(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "max_surge", value)
+
+    @property
     @pulumi.getter(name="minCount")
     def min_count(self) -> Optional[pulumi.Input[int]]:
         """
         The AKS node pool min count. Required if `enable_auto_scaling=true` (int)
         """
         return pulumi.get(self, "min_count")
 
@@ -2102,14 +2155,26 @@
         return pulumi.get(self, "os_type")
 
     @os_type.setter
     def os_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "os_type", value)
 
     @property
+    @pulumi.getter
+    def taints(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The AKS node pool taints (list)
+        """
+        return pulumi.get(self, "taints")
+
+    @taints.setter
+    def taints(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "taints", value)
+
+    @property
     @pulumi.getter(name="vmSize")
     def vm_size(self) -> Optional[pulumi.Input[str]]:
         """
         The AKS node pool orchestrator version (string)
         """
         return pulumi.get(self, "vm_size")
 
@@ -2665,14 +2730,194 @@
 
     @condition.setter
     def condition(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "condition", value)
 
 
 @pulumi.input_type
+class ClusterClusterAgentDeploymentCustomizationArgs:
+    def __init__(__self__, *,
+                 append_tolerations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs']]]] = None,
+                 override_affinity: Optional[pulumi.Input[str]] = None,
+                 override_resource_requirements: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]] = None):
+        if append_tolerations is not None:
+            pulumi.set(__self__, "append_tolerations", append_tolerations)
+        if override_affinity is not None:
+            pulumi.set(__self__, "override_affinity", override_affinity)
+        if override_resource_requirements is not None:
+            pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
+
+    @property
+    @pulumi.getter(name="appendTolerations")
+    def append_tolerations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs']]]]:
+        return pulumi.get(self, "append_tolerations")
+
+    @append_tolerations.setter
+    def append_tolerations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs']]]]):
+        pulumi.set(self, "append_tolerations", value)
+
+    @property
+    @pulumi.getter(name="overrideAffinity")
+    def override_affinity(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "override_affinity")
+
+    @override_affinity.setter
+    def override_affinity(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "override_affinity", value)
+
+    @property
+    @pulumi.getter(name="overrideResourceRequirements")
+    def override_resource_requirements(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]:
+        return pulumi.get(self, "override_resource_requirements")
+
+    @override_resource_requirements.setter
+    def override_resource_requirements(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]):
+        pulumi.set(self, "override_resource_requirements", value)
+
+
+@pulumi.input_type
+class ClusterClusterAgentDeploymentCustomizationAppendTolerationArgs:
+    def __init__(__self__, *,
+                 key: pulumi.Input[str],
+                 effect: Optional[pulumi.Input[str]] = None,
+                 operator: Optional[pulumi.Input[str]] = None,
+                 seconds: Optional[pulumi.Input[int]] = None,
+                 value: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] key: The toleration key (string)
+        :param pulumi.Input[str] effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        :param pulumi.Input[str] operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        :param pulumi.Input[int] seconds: The toleration seconds (int)
+        :param pulumi.Input[str] value: Rancher agent env var value (string)
+        """
+        pulumi.set(__self__, "key", key)
+        if effect is not None:
+            pulumi.set(__self__, "effect", effect)
+        if operator is not None:
+            pulumi.set(__self__, "operator", operator)
+        if seconds is not None:
+            pulumi.set(__self__, "seconds", seconds)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> pulumi.Input[str]:
+        """
+        The toleration key (string)
+        """
+        return pulumi.get(self, "key")
+
+    @key.setter
+    def key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "key", value)
+
+    @property
+    @pulumi.getter
+    def effect(self) -> Optional[pulumi.Input[str]]:
+        """
+        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        """
+        return pulumi.get(self, "effect")
+
+    @effect.setter
+    def effect(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "effect", value)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> Optional[pulumi.Input[str]]:
+        """
+        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        """
+        return pulumi.get(self, "operator")
+
+    @operator.setter
+    def operator(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "operator", value)
+
+    @property
+    @pulumi.getter
+    def seconds(self) -> Optional[pulumi.Input[int]]:
+        """
+        The toleration seconds (int)
+        """
+        return pulumi.get(self, "seconds")
+
+    @seconds.setter
+    def seconds(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "seconds", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> Optional[pulumi.Input[str]]:
+        """
+        Rancher agent env var value (string)
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
+class ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs:
+    def __init__(__self__, *,
+                 cpu_limit: Optional[pulumi.Input[str]] = None,
+                 cpu_request: Optional[pulumi.Input[str]] = None,
+                 memory_limit: Optional[pulumi.Input[str]] = None,
+                 memory_request: Optional[pulumi.Input[str]] = None):
+        if cpu_limit is not None:
+            pulumi.set(__self__, "cpu_limit", cpu_limit)
+        if cpu_request is not None:
+            pulumi.set(__self__, "cpu_request", cpu_request)
+        if memory_limit is not None:
+            pulumi.set(__self__, "memory_limit", memory_limit)
+        if memory_request is not None:
+            pulumi.set(__self__, "memory_request", memory_request)
+
+    @property
+    @pulumi.getter(name="cpuLimit")
+    def cpu_limit(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cpu_limit")
+
+    @cpu_limit.setter
+    def cpu_limit(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cpu_limit", value)
+
+    @property
+    @pulumi.getter(name="cpuRequest")
+    def cpu_request(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cpu_request")
+
+    @cpu_request.setter
+    def cpu_request(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cpu_request", value)
+
+    @property
+    @pulumi.getter(name="memoryLimit")
+    def memory_limit(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "memory_limit")
+
+    @memory_limit.setter
+    def memory_limit(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "memory_limit", value)
+
+    @property
+    @pulumi.getter(name="memoryRequest")
+    def memory_request(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "memory_request")
+
+    @memory_request.setter
+    def memory_request(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "memory_request", value)
+
+
+@pulumi.input_type
 class ClusterClusterAuthEndpointArgs:
     def __init__(__self__, *,
                  ca_certs: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  fqdn: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] ca_certs: CA certs for the authorized cluster endpoint (string)
@@ -4032,14 +4277,194 @@
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "version", value)
 
 
 @pulumi.input_type
+class ClusterFleetAgentDeploymentCustomizationArgs:
+    def __init__(__self__, *,
+                 append_tolerations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationAppendTolerationArgs']]]] = None,
+                 override_affinity: Optional[pulumi.Input[str]] = None,
+                 override_resource_requirements: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]] = None):
+        if append_tolerations is not None:
+            pulumi.set(__self__, "append_tolerations", append_tolerations)
+        if override_affinity is not None:
+            pulumi.set(__self__, "override_affinity", override_affinity)
+        if override_resource_requirements is not None:
+            pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
+
+    @property
+    @pulumi.getter(name="appendTolerations")
+    def append_tolerations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationAppendTolerationArgs']]]]:
+        return pulumi.get(self, "append_tolerations")
+
+    @append_tolerations.setter
+    def append_tolerations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationAppendTolerationArgs']]]]):
+        pulumi.set(self, "append_tolerations", value)
+
+    @property
+    @pulumi.getter(name="overrideAffinity")
+    def override_affinity(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "override_affinity")
+
+    @override_affinity.setter
+    def override_affinity(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "override_affinity", value)
+
+    @property
+    @pulumi.getter(name="overrideResourceRequirements")
+    def override_resource_requirements(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]:
+        return pulumi.get(self, "override_resource_requirements")
+
+    @override_resource_requirements.setter
+    def override_resource_requirements(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]):
+        pulumi.set(self, "override_resource_requirements", value)
+
+
+@pulumi.input_type
+class ClusterFleetAgentDeploymentCustomizationAppendTolerationArgs:
+    def __init__(__self__, *,
+                 key: pulumi.Input[str],
+                 effect: Optional[pulumi.Input[str]] = None,
+                 operator: Optional[pulumi.Input[str]] = None,
+                 seconds: Optional[pulumi.Input[int]] = None,
+                 value: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] key: The toleration key (string)
+        :param pulumi.Input[str] effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        :param pulumi.Input[str] operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        :param pulumi.Input[int] seconds: The toleration seconds (int)
+        :param pulumi.Input[str] value: Rancher agent env var value (string)
+        """
+        pulumi.set(__self__, "key", key)
+        if effect is not None:
+            pulumi.set(__self__, "effect", effect)
+        if operator is not None:
+            pulumi.set(__self__, "operator", operator)
+        if seconds is not None:
+            pulumi.set(__self__, "seconds", seconds)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> pulumi.Input[str]:
+        """
+        The toleration key (string)
+        """
+        return pulumi.get(self, "key")
+
+    @key.setter
+    def key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "key", value)
+
+    @property
+    @pulumi.getter
+    def effect(self) -> Optional[pulumi.Input[str]]:
+        """
+        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        """
+        return pulumi.get(self, "effect")
+
+    @effect.setter
+    def effect(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "effect", value)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> Optional[pulumi.Input[str]]:
+        """
+        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        """
+        return pulumi.get(self, "operator")
+
+    @operator.setter
+    def operator(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "operator", value)
+
+    @property
+    @pulumi.getter
+    def seconds(self) -> Optional[pulumi.Input[int]]:
+        """
+        The toleration seconds (int)
+        """
+        return pulumi.get(self, "seconds")
+
+    @seconds.setter
+    def seconds(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "seconds", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> Optional[pulumi.Input[str]]:
+        """
+        Rancher agent env var value (string)
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
+class ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirementArgs:
+    def __init__(__self__, *,
+                 cpu_limit: Optional[pulumi.Input[str]] = None,
+                 cpu_request: Optional[pulumi.Input[str]] = None,
+                 memory_limit: Optional[pulumi.Input[str]] = None,
+                 memory_request: Optional[pulumi.Input[str]] = None):
+        if cpu_limit is not None:
+            pulumi.set(__self__, "cpu_limit", cpu_limit)
+        if cpu_request is not None:
+            pulumi.set(__self__, "cpu_request", cpu_request)
+        if memory_limit is not None:
+            pulumi.set(__self__, "memory_limit", memory_limit)
+        if memory_request is not None:
+            pulumi.set(__self__, "memory_request", memory_request)
+
+    @property
+    @pulumi.getter(name="cpuLimit")
+    def cpu_limit(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cpu_limit")
+
+    @cpu_limit.setter
+    def cpu_limit(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cpu_limit", value)
+
+    @property
+    @pulumi.getter(name="cpuRequest")
+    def cpu_request(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cpu_request")
+
+    @cpu_request.setter
+    def cpu_request(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cpu_request", value)
+
+    @property
+    @pulumi.getter(name="memoryLimit")
+    def memory_limit(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "memory_limit")
+
+    @memory_limit.setter
+    def memory_limit(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "memory_limit", value)
+
+    @property
+    @pulumi.getter(name="memoryRequest")
+    def memory_request(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "memory_request")
+
+    @memory_request.setter
+    def memory_request(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "memory_request", value)
+
+
+@pulumi.input_type
 class ClusterGkeConfigArgs:
     def __init__(__self__, *,
                  cluster_ipv4_cidr: pulumi.Input[str],
                  credential: pulumi.Input[str],
                  disk_type: pulumi.Input[str],
                  image_type: pulumi.Input[str],
                  ip_policy_cluster_ipv4_cidr_block: pulumi.Input[str],
@@ -4138,15 +4563,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] master_authorized_network_cidr_blocks: Define up to 10 external networks that could access Kubernetes master through HTTPS (list)
         :param pulumi.Input[int] max_node_count: Maximum number of nodes in the NodePool. Must be >= minNodeCount. There has to enough quota to scale up the cluster. Default `0` (int)
         :param pulumi.Input[int] min_node_count: Minimmum number of nodes in the NodePool. Must be >= 1 and <= maxNodeCount. Default `0` (int)
         :param pulumi.Input[int] node_count: Node count for GKE cluster. Default `3` (int)
         :param pulumi.Input[bool] preemptible: Whether the nodes are created as preemptible VM instances. Default `false` (bool)
         :param pulumi.Input[str] region: (string)
         :param pulumi.Input[Mapping[str, Any]] resource_labels: The map of Kubernetes labels to be applied to each cluster (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] taints: List of Kubernetes taints to be applied to each node (list)
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] taints: The AKS node pool taints (list)
         :param pulumi.Input[bool] use_ip_aliases: Whether alias IPs will be used for pod IPs in the cluster. Default `false` (bool)
         :param pulumi.Input[str] zone: (string)
         """
         pulumi.set(__self__, "cluster_ipv4_cidr", cluster_ipv4_cidr)
         pulumi.set(__self__, "credential", credential)
         pulumi.set(__self__, "disk_type", disk_type)
         pulumi.set(__self__, "image_type", image_type)
@@ -4831,15 +5256,15 @@
     def resource_labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "resource_labels", value)
 
     @property
     @pulumi.getter
     def taints(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of Kubernetes taints to be applied to each node (list)
+        The AKS node pool taints (list)
         """
         return pulumi.get(self, "taints")
 
     @taints.setter
     def taints(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "taints", value)
 
@@ -5700,15 +6125,15 @@
         :param pulumi.Input[str] image_type: The image to use for the worker nodes (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster (map)
         :param pulumi.Input[int] local_ssd_count: The number of local SSD disks to be attached to the node. Default `0` (int)
         :param pulumi.Input[str] machine_type: Machine type for GKE cluster (string)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] oauth_scopes: The set of Google API scopes to be made available on all of the node VMs under the default service account (list)
         :param pulumi.Input[bool] preemptible: Whether the nodes are created as preemptible VM instances. Default `false` (bool)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags for Kubernetes cluster. For example, `["foo=bar","bar=foo"]` (list)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterGkeConfigV2NodePoolConfigTaintArgs']]] taints: List of Kubernetes taints to be applied to each node (list)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterGkeConfigV2NodePoolConfigTaintArgs']]] taints: The AKS node pool taints (list)
         """
         if disk_size_gb is not None:
             pulumi.set(__self__, "disk_size_gb", disk_size_gb)
         if disk_type is not None:
             pulumi.set(__self__, "disk_type", disk_type)
         if image_type is not None:
             pulumi.set(__self__, "image_type", image_type)
@@ -5835,15 +6260,15 @@
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def taints(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterGkeConfigV2NodePoolConfigTaintArgs']]]]:
         """
-        List of Kubernetes taints to be applied to each node (list)
+        The AKS node pool taints (list)
         """
         return pulumi.get(self, "taints")
 
     @taints.setter
     def taints(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterGkeConfigV2NodePoolConfigTaintArgs']]]]):
         pulumi.set(self, "taints", value)
 
@@ -12566,28 +12991,28 @@
     def secret_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_key", value)
 
 
 @pulumi.input_type
 class ClusterRkeConfigServicesKubeApiArgs:
     def __init__(__self__, *,
-                 admission_configuration: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 admission_configuration: Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAdmissionConfigurationArgs']] = None,
                  always_pull_images: Optional[pulumi.Input[bool]] = None,
                  audit_log: Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogArgs']] = None,
                  event_rate_limit: Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiEventRateLimitArgs']] = None,
                  extra_args: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  extra_binds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  extra_envs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  image: Optional[pulumi.Input[str]] = None,
                  pod_security_policy: Optional[pulumi.Input[bool]] = None,
                  secrets_encryption_config: Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiSecretsEncryptionConfigArgs']] = None,
                  service_cluster_ip_range: Optional[pulumi.Input[str]] = None,
                  service_node_port_range: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Mapping[str, Any]] admission_configuration: Admission configuration (map)
+        :param pulumi.Input['ClusterRkeConfigServicesKubeApiAdmissionConfigurationArgs'] admission_configuration: Admission configuration (map)
         :param pulumi.Input[bool] always_pull_images: Enable [AlwaysPullImages](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/#alwayspullimages) Admission controller plugin. [Rancher docs](https://rancher.com/docs/rke/latest/en/config-options/services/#kubernetes-api-server-options) Default: `false` (bool)
         :param pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogArgs'] audit_log: K8s audit log configuration. (list maxitems: 1)
         :param pulumi.Input['ClusterRkeConfigServicesKubeApiEventRateLimitArgs'] event_rate_limit: K8s event rate limit configuration. (list maxitems: 1)
         :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for RKE Ingress (map)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for etcd service (list)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for etcd service (list)
         :param pulumi.Input[str] image: Docker image for etcd service (string)
@@ -12619,22 +13044,22 @@
         if service_cluster_ip_range is not None:
             pulumi.set(__self__, "service_cluster_ip_range", service_cluster_ip_range)
         if service_node_port_range is not None:
             pulumi.set(__self__, "service_node_port_range", service_node_port_range)
 
     @property
     @pulumi.getter(name="admissionConfiguration")
-    def admission_configuration(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def admission_configuration(self) -> Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAdmissionConfigurationArgs']]:
         """
         Admission configuration (map)
         """
         return pulumi.get(self, "admission_configuration")
 
     @admission_configuration.setter
-    def admission_configuration(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def admission_configuration(self, value: Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAdmissionConfigurationArgs']]):
         pulumi.set(self, "admission_configuration", value)
 
     @property
     @pulumi.getter(name="alwaysPullImages")
     def always_pull_images(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable [AlwaysPullImages](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/#alwayspullimages) Admission controller plugin. [Rancher docs](https://rancher.com/docs/rke/latest/en/config-options/services/#kubernetes-api-server-options) Default: `false` (bool)
@@ -12763,32 +13188,190 @@
 
     @service_node_port_range.setter
     def service_node_port_range(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_node_port_range", value)
 
 
 @pulumi.input_type
+class ClusterRkeConfigServicesKubeApiAdmissionConfigurationArgs:
+    def __init__(__self__, *,
+                 api_version: Optional[pulumi.Input[str]] = None,
+                 kind: Optional[pulumi.Input[str]] = None,
+                 plugins: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs']]]] = None):
+        """
+        :param pulumi.Input[str] api_version: Admission configuration ApiVersion. Default: `apiserver.config.k8s.io/v1` (string)
+        :param pulumi.Input[str] kind: Admission configuration Kind. Default: `AdmissionConfiguration` (string)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs']]] plugins: Admission configuration plugins. (list `plugin`)
+        """
+        if api_version is not None:
+            pulumi.set(__self__, "api_version", api_version)
+        if kind is not None:
+            pulumi.set(__self__, "kind", kind)
+        if plugins is not None:
+            pulumi.set(__self__, "plugins", plugins)
+
+    @property
+    @pulumi.getter(name="apiVersion")
+    def api_version(self) -> Optional[pulumi.Input[str]]:
+        """
+        Admission configuration ApiVersion. Default: `apiserver.config.k8s.io/v1` (string)
+        """
+        return pulumi.get(self, "api_version")
+
+    @api_version.setter
+    def api_version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "api_version", value)
+
+    @property
+    @pulumi.getter
+    def kind(self) -> Optional[pulumi.Input[str]]:
+        """
+        Admission configuration Kind. Default: `AdmissionConfiguration` (string)
+        """
+        return pulumi.get(self, "kind")
+
+    @kind.setter
+    def kind(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "kind", value)
+
+    @property
+    @pulumi.getter
+    def plugins(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs']]]]:
+        """
+        Admission configuration plugins. (list `plugin`)
+        """
+        return pulumi.get(self, "plugins")
+
+    @plugins.setter
+    def plugins(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs']]]]):
+        pulumi.set(self, "plugins", value)
+
+
+@pulumi.input_type
+class ClusterRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs:
+    def __init__(__self__, *,
+                 configuration: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 path: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] configuration: Plugin configuration. (string) Ex:
+               
+               ```python
+               import pulumi
+               ```
+               configuration = <<EOF
+               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+               kind: Configuration
+               limits:
+               - type: Server
+               burst: 35000
+               qps: 6000
+               EOF
+        :param pulumi.Input[str] name: The name of the Cluster (string)
+        :param pulumi.Input[str] path: Path for etcd service (string)
+        """
+        if configuration is not None:
+            pulumi.set(__self__, "configuration", configuration)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if path is not None:
+            pulumi.set(__self__, "path", path)
+
+    @property
+    @pulumi.getter
+    def configuration(self) -> Optional[pulumi.Input[str]]:
+        """
+        Plugin configuration. (string) Ex:
+
+        ```python
+        import pulumi
+        ```
+        configuration = <<EOF
+        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+        kind: Configuration
+        limits:
+        - type: Server
+        burst: 35000
+        qps: 6000
+        EOF
+        """
+        return pulumi.get(self, "configuration")
+
+    @configuration.setter
+    def configuration(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "configuration", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The name of the Cluster (string)
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def path(self) -> Optional[pulumi.Input[str]]:
+        """
+        Path for etcd service (string)
+        """
+        return pulumi.get(self, "path")
+
+    @path.setter
+    def path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "path", value)
+
+
+@pulumi.input_type
 class ClusterRkeConfigServicesKubeApiAuditLogArgs:
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs']] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs'] configuration: Audit log configuration. (list maxitems: 1)
+        :param pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs'] configuration: Plugin configuration. (string) Ex:
+               
+               ```python
+               import pulumi
+               ```
+               configuration = <<EOF
+               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+               kind: Configuration
+               limits:
+               - type: Server
+               burst: 35000
+               qps: 6000
+               EOF
         :param pulumi.Input[bool] enabled: Enable etcd backup (bool)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs']]:
         """
-        Audit log configuration. (list maxitems: 1)
+        Plugin configuration. (string) Ex:
+
+        ```python
+        import pulumi
+        ```
+        configuration = <<EOF
+        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+        kind: Configuration
+        limits:
+        - type: Server
+        burst: 35000
+        qps: 6000
+        EOF
         """
         return pulumi.get(self, "configuration")
 
     @configuration.setter
     def configuration(self, value: Optional[pulumi.Input['ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs']]):
         pulumi.set(self, "configuration", value)
 
@@ -12910,27 +13493,51 @@
 
 @pulumi.input_type
 class ClusterRkeConfigServicesKubeApiEventRateLimitArgs:
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] configuration: Audit log configuration. (list maxitems: 1)
+        :param pulumi.Input[str] configuration: Plugin configuration. (string) Ex:
+               
+               ```python
+               import pulumi
+               ```
+               configuration = <<EOF
+               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+               kind: Configuration
+               limits:
+               - type: Server
+               burst: 35000
+               qps: 6000
+               EOF
         :param pulumi.Input[bool] enabled: Enable etcd backup (bool)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[pulumi.Input[str]]:
         """
-        Audit log configuration. (list maxitems: 1)
+        Plugin configuration. (string) Ex:
+
+        ```python
+        import pulumi
+        ```
+        configuration = <<EOF
+        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+        kind: Configuration
+        limits:
+        - type: Server
+        burst: 35000
+        qps: 6000
+        EOF
         """
         return pulumi.get(self, "configuration")
 
     @configuration.setter
     def configuration(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "configuration", value)
 
@@ -14017,14 +14624,15 @@
 
 @pulumi.input_type
 class ClusterTemplateTemplateRevisionClusterConfigArgs:
     def __init__(__self__, *,
                  rke_config: pulumi.Input['ClusterTemplateTemplateRevisionClusterConfigRkeConfigArgs'],
                  cluster_auth_endpoint: Optional[pulumi.Input['ClusterTemplateTemplateRevisionClusterConfigClusterAuthEndpointArgs']] = None,
                  default_cluster_role_for_project_members: Optional[pulumi.Input[str]] = None,
+                 default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[str]] = None,
                  default_pod_security_policy_template_id: Optional[pulumi.Input[str]] = None,
                  desired_agent_image: Optional[pulumi.Input[str]] = None,
                  desired_auth_image: Optional[pulumi.Input[str]] = None,
                  docker_root_dir: Optional[pulumi.Input[str]] = None,
                  enable_cluster_alerting: Optional[pulumi.Input[bool]] = None,
                  enable_cluster_monitoring: Optional[pulumi.Input[bool]] = None,
                  enable_network_policy: Optional[pulumi.Input[bool]] = None,
@@ -14043,14 +14651,16 @@
         :param pulumi.Input[bool] windows_prefered_cluster: Windows prefered cluster. Default: `false` (bool)
         """
         pulumi.set(__self__, "rke_config", rke_config)
         if cluster_auth_endpoint is not None:
             pulumi.set(__self__, "cluster_auth_endpoint", cluster_auth_endpoint)
         if default_cluster_role_for_project_members is not None:
             pulumi.set(__self__, "default_cluster_role_for_project_members", default_cluster_role_for_project_members)
+        if default_pod_security_admission_configuration_template_name is not None:
+            pulumi.set(__self__, "default_pod_security_admission_configuration_template_name", default_pod_security_admission_configuration_template_name)
         if default_pod_security_policy_template_id is not None:
             pulumi.set(__self__, "default_pod_security_policy_template_id", default_pod_security_policy_template_id)
         if desired_agent_image is not None:
             pulumi.set(__self__, "desired_agent_image", desired_agent_image)
         if desired_auth_image is not None:
             pulumi.set(__self__, "desired_auth_image", desired_auth_image)
         if docker_root_dir is not None:
@@ -14097,14 +14707,23 @@
         return pulumi.get(self, "default_cluster_role_for_project_members")
 
     @default_cluster_role_for_project_members.setter
     def default_cluster_role_for_project_members(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_cluster_role_for_project_members", value)
 
     @property
+    @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
+    def default_pod_security_admission_configuration_template_name(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
+
+    @default_pod_security_admission_configuration_template_name.setter
+    def default_pod_security_admission_configuration_template_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_pod_security_admission_configuration_template_name", value)
+
+    @property
     @pulumi.getter(name="defaultPodSecurityPolicyTemplateId")
     def default_pod_security_policy_template_id(self) -> Optional[pulumi.Input[str]]:
         """
         Default pod security policy template ID (string)
         """
         return pulumi.get(self, "default_pod_security_policy_template_id")
 
@@ -18625,15 +19244,15 @@
     def secret_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_key", value)
 
 
 @pulumi.input_type
 class ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiArgs:
     def __init__(__self__, *,
-                 admission_configuration: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 admission_configuration: Optional[pulumi.Input['ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationArgs']] = None,
                  always_pull_images: Optional[pulumi.Input[bool]] = None,
                  audit_log: Optional[pulumi.Input['ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLogArgs']] = None,
                  event_rate_limit: Optional[pulumi.Input['ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiEventRateLimitArgs']] = None,
                  extra_args: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  extra_binds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  extra_envs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  image: Optional[pulumi.Input[str]] = None,
@@ -18664,19 +19283,19 @@
         if service_cluster_ip_range is not None:
             pulumi.set(__self__, "service_cluster_ip_range", service_cluster_ip_range)
         if service_node_port_range is not None:
             pulumi.set(__self__, "service_node_port_range", service_node_port_range)
 
     @property
     @pulumi.getter(name="admissionConfiguration")
-    def admission_configuration(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def admission_configuration(self) -> Optional[pulumi.Input['ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationArgs']]:
         return pulumi.get(self, "admission_configuration")
 
     @admission_configuration.setter
-    def admission_configuration(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def admission_configuration(self, value: Optional[pulumi.Input['ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationArgs']]):
         pulumi.set(self, "admission_configuration", value)
 
     @property
     @pulumi.getter(name="alwaysPullImages")
     def always_pull_images(self) -> Optional[pulumi.Input[bool]]:
         return pulumi.get(self, "always_pull_images")
 
@@ -18772,14 +19391,102 @@
 
     @service_node_port_range.setter
     def service_node_port_range(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_node_port_range", value)
 
 
 @pulumi.input_type
+class ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationArgs:
+    def __init__(__self__, *,
+                 api_version: Optional[pulumi.Input[str]] = None,
+                 kind: Optional[pulumi.Input[str]] = None,
+                 plugins: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs']]]] = None):
+        if api_version is not None:
+            pulumi.set(__self__, "api_version", api_version)
+        if kind is not None:
+            pulumi.set(__self__, "kind", kind)
+        if plugins is not None:
+            pulumi.set(__self__, "plugins", plugins)
+
+    @property
+    @pulumi.getter(name="apiVersion")
+    def api_version(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "api_version")
+
+    @api_version.setter
+    def api_version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "api_version", value)
+
+    @property
+    @pulumi.getter
+    def kind(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "kind")
+
+    @kind.setter
+    def kind(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "kind", value)
+
+    @property
+    @pulumi.getter
+    def plugins(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs']]]]:
+        return pulumi.get(self, "plugins")
+
+    @plugins.setter
+    def plugins(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs']]]]):
+        pulumi.set(self, "plugins", value)
+
+
+@pulumi.input_type
+class ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs:
+    def __init__(__self__, *,
+                 configuration: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 path: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] name: The cluster template name (string)
+        """
+        if configuration is not None:
+            pulumi.set(__self__, "configuration", configuration)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if path is not None:
+            pulumi.set(__self__, "path", path)
+
+    @property
+    @pulumi.getter
+    def configuration(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "configuration")
+
+    @configuration.setter
+    def configuration(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "configuration", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The cluster template name (string)
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "path")
+
+    @path.setter
+    def path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "path", value)
+
+
+@pulumi.input_type
 class ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLogArgs:
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input['ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLogConfigurationArgs']] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[bool] enabled: Enable cluster template revision. Default `true` (bool)
         """
@@ -19474,14 +20181,190 @@
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
 
 
 @pulumi.input_type
+class ClusterV2ClusterAgentDeploymentCustomizationArgs:
+    def __init__(__self__, *,
+                 append_tolerations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationAppendTolerationArgs']]]] = None,
+                 override_affinity: Optional[pulumi.Input[str]] = None,
+                 override_resource_requirements: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]] = None):
+        if append_tolerations is not None:
+            pulumi.set(__self__, "append_tolerations", append_tolerations)
+        if override_affinity is not None:
+            pulumi.set(__self__, "override_affinity", override_affinity)
+        if override_resource_requirements is not None:
+            pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
+
+    @property
+    @pulumi.getter(name="appendTolerations")
+    def append_tolerations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationAppendTolerationArgs']]]]:
+        return pulumi.get(self, "append_tolerations")
+
+    @append_tolerations.setter
+    def append_tolerations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationAppendTolerationArgs']]]]):
+        pulumi.set(self, "append_tolerations", value)
+
+    @property
+    @pulumi.getter(name="overrideAffinity")
+    def override_affinity(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "override_affinity")
+
+    @override_affinity.setter
+    def override_affinity(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "override_affinity", value)
+
+    @property
+    @pulumi.getter(name="overrideResourceRequirements")
+    def override_resource_requirements(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]:
+        return pulumi.get(self, "override_resource_requirements")
+
+    @override_resource_requirements.setter
+    def override_resource_requirements(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]):
+        pulumi.set(self, "override_resource_requirements", value)
+
+
+@pulumi.input_type
+class ClusterV2ClusterAgentDeploymentCustomizationAppendTolerationArgs:
+    def __init__(__self__, *,
+                 key: pulumi.Input[str],
+                 effect: Optional[pulumi.Input[str]] = None,
+                 operator: Optional[pulumi.Input[str]] = None,
+                 seconds: Optional[pulumi.Input[int]] = None,
+                 value: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] key: The taint key (string)
+        :param pulumi.Input[str] effect: The taint effect. Default: `\\"NoExecute\\"` (string)
+        :param pulumi.Input[str] operator: Machine selector label match expressions operator (string)
+        :param pulumi.Input[str] value: Rancher agent env var value (string)
+        """
+        pulumi.set(__self__, "key", key)
+        if effect is not None:
+            pulumi.set(__self__, "effect", effect)
+        if operator is not None:
+            pulumi.set(__self__, "operator", operator)
+        if seconds is not None:
+            pulumi.set(__self__, "seconds", seconds)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> pulumi.Input[str]:
+        """
+        The taint key (string)
+        """
+        return pulumi.get(self, "key")
+
+    @key.setter
+    def key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "key", value)
+
+    @property
+    @pulumi.getter
+    def effect(self) -> Optional[pulumi.Input[str]]:
+        """
+        The taint effect. Default: `\\"NoExecute\\"` (string)
+        """
+        return pulumi.get(self, "effect")
+
+    @effect.setter
+    def effect(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "effect", value)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> Optional[pulumi.Input[str]]:
+        """
+        Machine selector label match expressions operator (string)
+        """
+        return pulumi.get(self, "operator")
+
+    @operator.setter
+    def operator(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "operator", value)
+
+    @property
+    @pulumi.getter
+    def seconds(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "seconds")
+
+    @seconds.setter
+    def seconds(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "seconds", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> Optional[pulumi.Input[str]]:
+        """
+        Rancher agent env var value (string)
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
+class ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirementArgs:
+    def __init__(__self__, *,
+                 cpu_limit: Optional[pulumi.Input[str]] = None,
+                 cpu_request: Optional[pulumi.Input[str]] = None,
+                 memory_limit: Optional[pulumi.Input[str]] = None,
+                 memory_request: Optional[pulumi.Input[str]] = None):
+        if cpu_limit is not None:
+            pulumi.set(__self__, "cpu_limit", cpu_limit)
+        if cpu_request is not None:
+            pulumi.set(__self__, "cpu_request", cpu_request)
+        if memory_limit is not None:
+            pulumi.set(__self__, "memory_limit", memory_limit)
+        if memory_request is not None:
+            pulumi.set(__self__, "memory_request", memory_request)
+
+    @property
+    @pulumi.getter(name="cpuLimit")
+    def cpu_limit(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cpu_limit")
+
+    @cpu_limit.setter
+    def cpu_limit(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cpu_limit", value)
+
+    @property
+    @pulumi.getter(name="cpuRequest")
+    def cpu_request(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cpu_request")
+
+    @cpu_request.setter
+    def cpu_request(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cpu_request", value)
+
+    @property
+    @pulumi.getter(name="memoryLimit")
+    def memory_limit(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "memory_limit")
+
+    @memory_limit.setter
+    def memory_limit(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "memory_limit", value)
+
+    @property
+    @pulumi.getter(name="memoryRequest")
+    def memory_request(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "memory_request")
+
+    @memory_request.setter
+    def memory_request(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "memory_request", value)
+
+
+@pulumi.input_type
 class ClusterV2ClusterRegistrationTokenArgs:
     def __init__(__self__, *,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  command: Optional[pulumi.Input[str]] = None,
                  id: Optional[pulumi.Input[str]] = None,
                  insecure_command: Optional[pulumi.Input[str]] = None,
@@ -19689,14 +20572,190 @@
 
     @windows_node_command.setter
     def windows_node_command(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "windows_node_command", value)
 
 
 @pulumi.input_type
+class ClusterV2FleetAgentDeploymentCustomizationArgs:
+    def __init__(__self__, *,
+                 append_tolerations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationAppendTolerationArgs']]]] = None,
+                 override_affinity: Optional[pulumi.Input[str]] = None,
+                 override_resource_requirements: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]] = None):
+        if append_tolerations is not None:
+            pulumi.set(__self__, "append_tolerations", append_tolerations)
+        if override_affinity is not None:
+            pulumi.set(__self__, "override_affinity", override_affinity)
+        if override_resource_requirements is not None:
+            pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
+
+    @property
+    @pulumi.getter(name="appendTolerations")
+    def append_tolerations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationAppendTolerationArgs']]]]:
+        return pulumi.get(self, "append_tolerations")
+
+    @append_tolerations.setter
+    def append_tolerations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationAppendTolerationArgs']]]]):
+        pulumi.set(self, "append_tolerations", value)
+
+    @property
+    @pulumi.getter(name="overrideAffinity")
+    def override_affinity(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "override_affinity")
+
+    @override_affinity.setter
+    def override_affinity(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "override_affinity", value)
+
+    @property
+    @pulumi.getter(name="overrideResourceRequirements")
+    def override_resource_requirements(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]:
+        return pulumi.get(self, "override_resource_requirements")
+
+    @override_resource_requirements.setter
+    def override_resource_requirements(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirementArgs']]]]):
+        pulumi.set(self, "override_resource_requirements", value)
+
+
+@pulumi.input_type
+class ClusterV2FleetAgentDeploymentCustomizationAppendTolerationArgs:
+    def __init__(__self__, *,
+                 key: pulumi.Input[str],
+                 effect: Optional[pulumi.Input[str]] = None,
+                 operator: Optional[pulumi.Input[str]] = None,
+                 seconds: Optional[pulumi.Input[int]] = None,
+                 value: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] key: The taint key (string)
+        :param pulumi.Input[str] effect: The taint effect. Default: `\\"NoExecute\\"` (string)
+        :param pulumi.Input[str] operator: Machine selector label match expressions operator (string)
+        :param pulumi.Input[str] value: Rancher agent env var value (string)
+        """
+        pulumi.set(__self__, "key", key)
+        if effect is not None:
+            pulumi.set(__self__, "effect", effect)
+        if operator is not None:
+            pulumi.set(__self__, "operator", operator)
+        if seconds is not None:
+            pulumi.set(__self__, "seconds", seconds)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> pulumi.Input[str]:
+        """
+        The taint key (string)
+        """
+        return pulumi.get(self, "key")
+
+    @key.setter
+    def key(self, value: pulumi.Input[str]):
+        pulumi.set(self, "key", value)
+
+    @property
+    @pulumi.getter
+    def effect(self) -> Optional[pulumi.Input[str]]:
+        """
+        The taint effect. Default: `\\"NoExecute\\"` (string)
+        """
+        return pulumi.get(self, "effect")
+
+    @effect.setter
+    def effect(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "effect", value)
+
+    @property
+    @pulumi.getter
+    def operator(self) -> Optional[pulumi.Input[str]]:
+        """
+        Machine selector label match expressions operator (string)
+        """
+        return pulumi.get(self, "operator")
+
+    @operator.setter
+    def operator(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "operator", value)
+
+    @property
+    @pulumi.getter
+    def seconds(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "seconds")
+
+    @seconds.setter
+    def seconds(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "seconds", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> Optional[pulumi.Input[str]]:
+        """
+        Rancher agent env var value (string)
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
+class ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirementArgs:
+    def __init__(__self__, *,
+                 cpu_limit: Optional[pulumi.Input[str]] = None,
+                 cpu_request: Optional[pulumi.Input[str]] = None,
+                 memory_limit: Optional[pulumi.Input[str]] = None,
+                 memory_request: Optional[pulumi.Input[str]] = None):
+        if cpu_limit is not None:
+            pulumi.set(__self__, "cpu_limit", cpu_limit)
+        if cpu_request is not None:
+            pulumi.set(__self__, "cpu_request", cpu_request)
+        if memory_limit is not None:
+            pulumi.set(__self__, "memory_limit", memory_limit)
+        if memory_request is not None:
+            pulumi.set(__self__, "memory_request", memory_request)
+
+    @property
+    @pulumi.getter(name="cpuLimit")
+    def cpu_limit(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cpu_limit")
+
+    @cpu_limit.setter
+    def cpu_limit(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cpu_limit", value)
+
+    @property
+    @pulumi.getter(name="cpuRequest")
+    def cpu_request(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cpu_request")
+
+    @cpu_request.setter
+    def cpu_request(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cpu_request", value)
+
+    @property
+    @pulumi.getter(name="memoryLimit")
+    def memory_limit(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "memory_limit")
+
+    @memory_limit.setter
+    def memory_limit(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "memory_limit", value)
+
+    @property
+    @pulumi.getter(name="memoryRequest")
+    def memory_request(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "memory_request")
+
+    @memory_request.setter
+    def memory_request(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "memory_request", value)
+
+
+@pulumi.input_type
 class ClusterV2LocalAuthEndpointArgs:
     def __init__(__self__, *,
                  ca_certs: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  fqdn: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] ca_certs: CA certs for the authorized cluster endpoint (string)
@@ -19753,14 +20812,15 @@
                  additional_manifest: Optional[pulumi.Input[str]] = None,
                  chart_values: Optional[pulumi.Input[str]] = None,
                  etcd: Optional[pulumi.Input['ClusterV2RkeConfigEtcdArgs']] = None,
                  etcd_snapshot_create: Optional[pulumi.Input['ClusterV2RkeConfigEtcdSnapshotCreateArgs']] = None,
                  etcd_snapshot_restore: Optional[pulumi.Input['ClusterV2RkeConfigEtcdSnapshotRestoreArgs']] = None,
                  local_auth_endpoint: Optional[pulumi.Input['ClusterV2RkeConfigLocalAuthEndpointArgs']] = None,
                  machine_global_config: Optional[pulumi.Input[str]] = None,
+                 machine_pool_defaults: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2RkeConfigMachinePoolDefaultArgs']]]] = None,
                  machine_pools: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2RkeConfigMachinePoolArgs']]]] = None,
                  machine_selector_configs: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2RkeConfigMachineSelectorConfigArgs']]]] = None,
                  registries: Optional[pulumi.Input['ClusterV2RkeConfigRegistriesArgs']] = None,
                  rotate_certificates: Optional[pulumi.Input['ClusterV2RkeConfigRotateCertificatesArgs']] = None,
                  upgrade_strategy: Optional[pulumi.Input['ClusterV2RkeConfigUpgradeStrategyArgs']] = None):
         """
         :param pulumi.Input[str] additional_manifest: Cluster V2 additional manifest (string)
@@ -19789,14 +20849,16 @@
         if local_auth_endpoint is not None:
             warnings.warn("""Use rancher2_cluster_v2.local_auth_endpoint instead""", DeprecationWarning)
             pulumi.log.warn("""local_auth_endpoint is deprecated: Use rancher2_cluster_v2.local_auth_endpoint instead""")
         if local_auth_endpoint is not None:
             pulumi.set(__self__, "local_auth_endpoint", local_auth_endpoint)
         if machine_global_config is not None:
             pulumi.set(__self__, "machine_global_config", machine_global_config)
+        if machine_pool_defaults is not None:
+            pulumi.set(__self__, "machine_pool_defaults", machine_pool_defaults)
         if machine_pools is not None:
             pulumi.set(__self__, "machine_pools", machine_pools)
         if machine_selector_configs is not None:
             pulumi.set(__self__, "machine_selector_configs", machine_selector_configs)
         if registries is not None:
             pulumi.set(__self__, "registries", registries)
         if rotate_certificates is not None:
@@ -19885,14 +20947,23 @@
         return pulumi.get(self, "machine_global_config")
 
     @machine_global_config.setter
     def machine_global_config(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "machine_global_config", value)
 
     @property
+    @pulumi.getter(name="machinePoolDefaults")
+    def machine_pool_defaults(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2RkeConfigMachinePoolDefaultArgs']]]]:
+        return pulumi.get(self, "machine_pool_defaults")
+
+    @machine_pool_defaults.setter
+    def machine_pool_defaults(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2RkeConfigMachinePoolDefaultArgs']]]]):
+        pulumi.set(self, "machine_pool_defaults", value)
+
+    @property
     @pulumi.getter(name="machinePools")
     def machine_pools(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2RkeConfigMachinePoolArgs']]]]:
         """
         Cluster V2 machine pools (list)
         """
         return pulumi.get(self, "machine_pools")
 
@@ -20273,14 +21344,15 @@
                  machine_config: pulumi.Input['ClusterV2RkeConfigMachinePoolMachineConfigArgs'],
                  name: pulumi.Input[str],
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  cloud_credential_secret_name: Optional[pulumi.Input[str]] = None,
                  control_plane_role: Optional[pulumi.Input[bool]] = None,
                  drain_before_delete: Optional[pulumi.Input[bool]] = None,
                  etcd_role: Optional[pulumi.Input[bool]] = None,
+                 hostname_length_limit: Optional[pulumi.Input[int]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  machine_labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  max_unhealthy: Optional[pulumi.Input[str]] = None,
                  node_drain_timeout: Optional[pulumi.Input[int]] = None,
                  node_startup_timeout_seconds: Optional[pulumi.Input[int]] = None,
                  paused: Optional[pulumi.Input[bool]] = None,
                  quantity: Optional[pulumi.Input[int]] = None,
@@ -20318,14 +21390,16 @@
             pulumi.set(__self__, "cloud_credential_secret_name", cloud_credential_secret_name)
         if control_plane_role is not None:
             pulumi.set(__self__, "control_plane_role", control_plane_role)
         if drain_before_delete is not None:
             pulumi.set(__self__, "drain_before_delete", drain_before_delete)
         if etcd_role is not None:
             pulumi.set(__self__, "etcd_role", etcd_role)
+        if hostname_length_limit is not None:
+            pulumi.set(__self__, "hostname_length_limit", hostname_length_limit)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if machine_labels is not None:
             pulumi.set(__self__, "machine_labels", machine_labels)
         if max_unhealthy is not None:
             pulumi.set(__self__, "max_unhealthy", max_unhealthy)
         if node_drain_timeout is not None:
@@ -20428,14 +21502,23 @@
         return pulumi.get(self, "etcd_role")
 
     @etcd_role.setter
     def etcd_role(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "etcd_role", value)
 
     @property
+    @pulumi.getter(name="hostnameLengthLimit")
+    def hostname_length_limit(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "hostname_length_limit")
+
+    @hostname_length_limit.setter
+    def hostname_length_limit(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "hostname_length_limit", value)
+
+    @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Labels for the Cluster V2 (map)
         """
         return pulumi.get(self, "labels")
 
@@ -20573,14 +21656,31 @@
 
     @worker_role.setter
     def worker_role(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "worker_role", value)
 
 
 @pulumi.input_type
+class ClusterV2RkeConfigMachinePoolDefaultArgs:
+    def __init__(__self__, *,
+                 hostname_length_limit: Optional[pulumi.Input[int]] = None):
+        if hostname_length_limit is not None:
+            pulumi.set(__self__, "hostname_length_limit", hostname_length_limit)
+
+    @property
+    @pulumi.getter(name="hostnameLengthLimit")
+    def hostname_length_limit(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "hostname_length_limit")
+
+    @hostname_length_limit.setter
+    def hostname_length_limit(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "hostname_length_limit", value)
+
+
+@pulumi.input_type
 class ClusterV2RkeConfigMachinePoolMachineConfigArgs:
     def __init__(__self__, *,
                  kind: pulumi.Input[str],
                  name: pulumi.Input[str]):
         """
         :param pulumi.Input[str] kind: Machine config kind (string)
         :param pulumi.Input[str] name: The name of the Cluster v2 (string)
```

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/_utilities.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/active_directory.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/app.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/app_v2.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/app_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_active_directory.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_adfs.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_adfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_azure_ad.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_azure_ad.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_free_ipa.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_free_ipa.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_github.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_keycloak.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_keycloak.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_okta.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_okta.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_open_ldap.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_open_ldap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/auth_config_ping.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/auth_config_ping.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
                  sp_key: pulumi.Input[str],
                  uid_field: pulumi.Input[str],
                  user_name_field: pulumi.Input[str],
                  access_mode: Optional[pulumi.Input[str]] = None,
                  allowed_principal_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
+                 entity_id_field: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None):
         """
         The set of arguments for constructing a AuthConfigPing resource.
         :param pulumi.Input[str] display_name_field: Ping display name field (string)
         :param pulumi.Input[str] groups_field: Ping group field (string)
         :param pulumi.Input[str] idp_metadata_content: Ping IDP metadata content (string)
         :param pulumi.Input[str] rancher_api_host: Rancher URL. URL scheme needs to be specified, `https://<RANCHER_API_HOST>` (string)
@@ -55,14 +56,16 @@
             pulumi.set(__self__, "access_mode", access_mode)
         if allowed_principal_ids is not None:
             pulumi.set(__self__, "allowed_principal_ids", allowed_principal_ids)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
+        if entity_id_field is not None:
+            pulumi.set(__self__, "entity_id_field", entity_id_field)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
 
     @property
     @pulumi.getter(name="displayNameField")
     def display_name_field(self) -> pulumi.Input[str]:
         """
@@ -203,14 +206,23 @@
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
+    @pulumi.getter(name="entityIdField")
+    def entity_id_field(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "entity_id_field")
+
+    @entity_id_field.setter
+    def entity_id_field(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "entity_id_field", value)
+
+    @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
         Labels of the resource (map)
         """
         return pulumi.get(self, "labels")
 
@@ -223,14 +235,15 @@
 class _AuthConfigPingState:
     def __init__(__self__, *,
                  access_mode: Optional[pulumi.Input[str]] = None,
                  allowed_principal_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  display_name_field: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
+                 entity_id_field: Optional[pulumi.Input[str]] = None,
                  groups_field: Optional[pulumi.Input[str]] = None,
                  idp_metadata_content: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  rancher_api_host: Optional[pulumi.Input[str]] = None,
                  sp_cert: Optional[pulumi.Input[str]] = None,
                  sp_key: Optional[pulumi.Input[str]] = None,
@@ -261,14 +274,16 @@
             pulumi.set(__self__, "allowed_principal_ids", allowed_principal_ids)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if display_name_field is not None:
             pulumi.set(__self__, "display_name_field", display_name_field)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
+        if entity_id_field is not None:
+            pulumi.set(__self__, "entity_id_field", entity_id_field)
         if groups_field is not None:
             pulumi.set(__self__, "groups_field", groups_field)
         if idp_metadata_content is not None:
             pulumi.set(__self__, "idp_metadata_content", idp_metadata_content)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
@@ -343,14 +358,23 @@
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
+    @pulumi.getter(name="entityIdField")
+    def entity_id_field(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "entity_id_field")
+
+    @entity_id_field.setter
+    def entity_id_field(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "entity_id_field", value)
+
+    @property
     @pulumi.getter(name="groupsField")
     def groups_field(self) -> Optional[pulumi.Input[str]]:
         """
         Ping group field (string)
         """
         return pulumi.get(self, "groups_field")
 
@@ -473,14 +497,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_mode: Optional[pulumi.Input[str]] = None,
                  allowed_principal_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  display_name_field: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
+                 entity_id_field: Optional[pulumi.Input[str]] = None,
                  groups_field: Optional[pulumi.Input[str]] = None,
                  idp_metadata_content: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  rancher_api_host: Optional[pulumi.Input[str]] = None,
                  sp_cert: Optional[pulumi.Input[str]] = None,
                  sp_key: Optional[pulumi.Input[str]] = None,
                  uid_field: Optional[pulumi.Input[str]] = None,
@@ -570,14 +595,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_mode: Optional[pulumi.Input[str]] = None,
                  allowed_principal_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  display_name_field: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
+                 entity_id_field: Optional[pulumi.Input[str]] = None,
                  groups_field: Optional[pulumi.Input[str]] = None,
                  idp_metadata_content: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  rancher_api_host: Optional[pulumi.Input[str]] = None,
                  sp_cert: Optional[pulumi.Input[str]] = None,
                  sp_key: Optional[pulumi.Input[str]] = None,
                  uid_field: Optional[pulumi.Input[str]] = None,
@@ -594,14 +620,15 @@
             __props__.__dict__["access_mode"] = access_mode
             __props__.__dict__["allowed_principal_ids"] = allowed_principal_ids
             __props__.__dict__["annotations"] = annotations
             if display_name_field is None and not opts.urn:
                 raise TypeError("Missing required property 'display_name_field'")
             __props__.__dict__["display_name_field"] = display_name_field
             __props__.__dict__["enabled"] = enabled
+            __props__.__dict__["entity_id_field"] = entity_id_field
             if groups_field is None and not opts.urn:
                 raise TypeError("Missing required property 'groups_field'")
             __props__.__dict__["groups_field"] = groups_field
             if idp_metadata_content is None and not opts.urn:
                 raise TypeError("Missing required property 'idp_metadata_content'")
             __props__.__dict__["idp_metadata_content"] = None if idp_metadata_content is None else pulumi.Output.secret(idp_metadata_content)
             __props__.__dict__["labels"] = labels
@@ -635,14 +662,15 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             access_mode: Optional[pulumi.Input[str]] = None,
             allowed_principal_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
             display_name_field: Optional[pulumi.Input[str]] = None,
             enabled: Optional[pulumi.Input[bool]] = None,
+            entity_id_field: Optional[pulumi.Input[str]] = None,
             groups_field: Optional[pulumi.Input[str]] = None,
             idp_metadata_content: Optional[pulumi.Input[str]] = None,
             labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             rancher_api_host: Optional[pulumi.Input[str]] = None,
             sp_cert: Optional[pulumi.Input[str]] = None,
             sp_key: Optional[pulumi.Input[str]] = None,
@@ -677,14 +705,15 @@
         __props__ = _AuthConfigPingState.__new__(_AuthConfigPingState)
 
         __props__.__dict__["access_mode"] = access_mode
         __props__.__dict__["allowed_principal_ids"] = allowed_principal_ids
         __props__.__dict__["annotations"] = annotations
         __props__.__dict__["display_name_field"] = display_name_field
         __props__.__dict__["enabled"] = enabled
+        __props__.__dict__["entity_id_field"] = entity_id_field
         __props__.__dict__["groups_field"] = groups_field
         __props__.__dict__["idp_metadata_content"] = idp_metadata_content
         __props__.__dict__["labels"] = labels
         __props__.__dict__["name"] = name
         __props__.__dict__["rancher_api_host"] = rancher_api_host
         __props__.__dict__["sp_cert"] = sp_cert
         __props__.__dict__["sp_key"] = sp_key
@@ -730,14 +759,19 @@
     def enabled(self) -> pulumi.Output[Optional[bool]]:
         """
         Enable auth config provider. Default `true` (bool)
         """
         return pulumi.get(self, "enabled")
 
     @property
+    @pulumi.getter(name="entityIdField")
+    def entity_id_field(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "entity_id_field")
+
+    @property
     @pulumi.getter(name="groupsField")
     def groups_field(self) -> pulumi.Output[str]:
         """
         Ping group field (string)
         """
         return pulumi.get(self, "groups_field")
```

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/bootstrap.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/catalog.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/catalog_v2.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/certificate.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cloud_credential.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,31 +16,34 @@
 @pulumi.input_type
 class ClusterArgs:
     def __init__(__self__, *,
                  agent_env_vars: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterAgentEnvVarArgs']]]] = None,
                  aks_config: Optional[pulumi.Input['ClusterAksConfigArgs']] = None,
                  aks_config_v2: Optional[pulumi.Input['ClusterAksConfigV2Args']] = None,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 cluster_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]]] = None,
                  cluster_auth_endpoint: Optional[pulumi.Input['ClusterClusterAuthEndpointArgs']] = None,
                  cluster_monitoring_input: Optional[pulumi.Input['ClusterClusterMonitoringInputArgs']] = None,
                  cluster_template_answers: Optional[pulumi.Input['ClusterClusterTemplateAnswersArgs']] = None,
                  cluster_template_id: Optional[pulumi.Input[str]] = None,
                  cluster_template_questions: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterTemplateQuestionArgs']]]] = None,
                  cluster_template_revision_id: Optional[pulumi.Input[str]] = None,
+                 default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[str]] = None,
                  default_pod_security_policy_template_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  desired_agent_image: Optional[pulumi.Input[str]] = None,
                  desired_auth_image: Optional[pulumi.Input[str]] = None,
                  docker_root_dir: Optional[pulumi.Input[str]] = None,
                  driver: Optional[pulumi.Input[str]] = None,
                  eks_config: Optional[pulumi.Input['ClusterEksConfigArgs']] = None,
                  eks_config_v2: Optional[pulumi.Input['ClusterEksConfigV2Args']] = None,
                  enable_cluster_alerting: Optional[pulumi.Input[bool]] = None,
                  enable_cluster_monitoring: Optional[pulumi.Input[bool]] = None,
                  enable_network_policy: Optional[pulumi.Input[bool]] = None,
+                 fleet_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]]] = None,
                  fleet_workspace_name: Optional[pulumi.Input[str]] = None,
                  gke_config: Optional[pulumi.Input['ClusterGkeConfigArgs']] = None,
                  gke_config_v2: Optional[pulumi.Input['ClusterGkeConfigV2Args']] = None,
                  k3s_config: Optional[pulumi.Input['ClusterK3sConfigArgs']] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  oke_config: Optional[pulumi.Input['ClusterOkeConfigArgs']] = None,
@@ -49,31 +52,34 @@
                  windows_prefered_cluster: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Cluster resource.
         :param pulumi.Input[Sequence[pulumi.Input['ClusterAgentEnvVarArgs']]] agent_env_vars: Optional Agent Env Vars for Rancher agent. Just for Rancher v2.5.6 and above (list)
         :param pulumi.Input['ClusterAksConfigArgs'] aks_config: The Azure AKS configuration for `aks` Clusters. Conflicts with `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input['ClusterAksConfigV2Args'] aks_config_v2: The Azure AKS v2 configuration for creating/import `aks` Clusters. Conflicts with `aks_config`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster (map)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]] cluster_agent_deployment_customizations: Optional customization for cluster agent
         :param pulumi.Input['ClusterClusterAuthEndpointArgs'] cluster_auth_endpoint: Enabling the [local cluster authorized endpoint](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#local-cluster-auth-endpoint) allows direct communication with the cluster, bypassing the Rancher API proxy. (list maxitems:1)
         :param pulumi.Input['ClusterClusterMonitoringInputArgs'] cluster_monitoring_input: Cluster monitoring config. Any parameter defined in [rancher-monitoring charts](https://github.com/rancher/system-charts/tree/dev/charts/rancher-monitoring) could be configured  (list maxitems:1)
         :param pulumi.Input['ClusterClusterTemplateAnswersArgs'] cluster_template_answers: Cluster template answers. Just for Rancher v2.3.x and above (list maxitems:1)
         :param pulumi.Input[str] cluster_template_id: Cluster template ID. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterTemplateQuestionArgs']]] cluster_template_questions: Cluster template questions. Just for Rancher v2.3.x and above (list)
         :param pulumi.Input[str] cluster_template_revision_id: Cluster template revision ID. Just for Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster default pod security admission configuration template name
         :param pulumi.Input[str] default_pod_security_policy_template_id: [Default pod security policy template id](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#pod-security-policy-support) (string)
         :param pulumi.Input[str] description: The description for Cluster (string)
         :param pulumi.Input[str] desired_agent_image: Desired agent image. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[str] desired_auth_image: Desired auth image. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[str] docker_root_dir: Desired auth image. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[str] driver: (Computed) The driver used for the Cluster. `imported`, `azurekubernetesservice`, `amazonelasticcontainerservice`, `googlekubernetesengine` and `rancherKubernetesEngine` are supported (string)
         :param pulumi.Input['ClusterEksConfigArgs'] eks_config: The Amazon EKS configuration for `eks` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input['ClusterEksConfigV2Args'] eks_config_v2: The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x or above (list maxitems:1)
         :param pulumi.Input[bool] enable_cluster_alerting: Enable built-in cluster alerting (bool)
         :param pulumi.Input[bool] enable_cluster_monitoring: Enable built-in cluster monitoring (bool)
         :param pulumi.Input[bool] enable_network_policy: Enable project network isolation (bool)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]] fleet_agent_deployment_customizations: Optional customization for fleet agent
         :param pulumi.Input[str] fleet_workspace_name: Fleet workspace name (string)
         :param pulumi.Input['ClusterGkeConfigArgs'] gke_config: The Google GKE configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config_v2`, `oke_config`, `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input['ClusterGkeConfigV2Args'] gke_config_v2: The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 or above (list maxitems:1)
         :param pulumi.Input['ClusterK3sConfigArgs'] k3s_config: The K3S configuration for `k3s` imported Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster (map)
         :param pulumi.Input[str] name: The name of the Cluster (string)
         :param pulumi.Input['ClusterOkeConfigArgs'] oke_config: The Oracle OKE configuration for `oke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `k3s_config` and `rke_config` (list maxitems:1)
@@ -85,26 +91,30 @@
             pulumi.set(__self__, "agent_env_vars", agent_env_vars)
         if aks_config is not None:
             pulumi.set(__self__, "aks_config", aks_config)
         if aks_config_v2 is not None:
             pulumi.set(__self__, "aks_config_v2", aks_config_v2)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
+        if cluster_agent_deployment_customizations is not None:
+            pulumi.set(__self__, "cluster_agent_deployment_customizations", cluster_agent_deployment_customizations)
         if cluster_auth_endpoint is not None:
             pulumi.set(__self__, "cluster_auth_endpoint", cluster_auth_endpoint)
         if cluster_monitoring_input is not None:
             pulumi.set(__self__, "cluster_monitoring_input", cluster_monitoring_input)
         if cluster_template_answers is not None:
             pulumi.set(__self__, "cluster_template_answers", cluster_template_answers)
         if cluster_template_id is not None:
             pulumi.set(__self__, "cluster_template_id", cluster_template_id)
         if cluster_template_questions is not None:
             pulumi.set(__self__, "cluster_template_questions", cluster_template_questions)
         if cluster_template_revision_id is not None:
             pulumi.set(__self__, "cluster_template_revision_id", cluster_template_revision_id)
+        if default_pod_security_admission_configuration_template_name is not None:
+            pulumi.set(__self__, "default_pod_security_admission_configuration_template_name", default_pod_security_admission_configuration_template_name)
         if default_pod_security_policy_template_id is not None:
             pulumi.set(__self__, "default_pod_security_policy_template_id", default_pod_security_policy_template_id)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if desired_agent_image is not None:
             pulumi.set(__self__, "desired_agent_image", desired_agent_image)
         if desired_auth_image is not None:
@@ -119,14 +129,16 @@
             pulumi.set(__self__, "eks_config_v2", eks_config_v2)
         if enable_cluster_alerting is not None:
             pulumi.set(__self__, "enable_cluster_alerting", enable_cluster_alerting)
         if enable_cluster_monitoring is not None:
             pulumi.set(__self__, "enable_cluster_monitoring", enable_cluster_monitoring)
         if enable_network_policy is not None:
             pulumi.set(__self__, "enable_network_policy", enable_network_policy)
+        if fleet_agent_deployment_customizations is not None:
+            pulumi.set(__self__, "fleet_agent_deployment_customizations", fleet_agent_deployment_customizations)
         if fleet_workspace_name is not None:
             pulumi.set(__self__, "fleet_workspace_name", fleet_workspace_name)
         if gke_config is not None:
             pulumi.set(__self__, "gke_config", gke_config)
         if gke_config_v2 is not None:
             pulumi.set(__self__, "gke_config_v2", gke_config_v2)
         if k3s_config is not None:
@@ -189,14 +201,26 @@
         return pulumi.get(self, "annotations")
 
     @annotations.setter
     def annotations(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "annotations", value)
 
     @property
+    @pulumi.getter(name="clusterAgentDeploymentCustomizations")
+    def cluster_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]]]:
+        """
+        Optional customization for cluster agent
+        """
+        return pulumi.get(self, "cluster_agent_deployment_customizations")
+
+    @cluster_agent_deployment_customizations.setter
+    def cluster_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]]]):
+        pulumi.set(self, "cluster_agent_deployment_customizations", value)
+
+    @property
     @pulumi.getter(name="clusterAuthEndpoint")
     def cluster_auth_endpoint(self) -> Optional[pulumi.Input['ClusterClusterAuthEndpointArgs']]:
         """
         Enabling the [local cluster authorized endpoint](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#local-cluster-auth-endpoint) allows direct communication with the cluster, bypassing the Rancher API proxy. (list maxitems:1)
         """
         return pulumi.get(self, "cluster_auth_endpoint")
 
@@ -261,14 +285,26 @@
         return pulumi.get(self, "cluster_template_revision_id")
 
     @cluster_template_revision_id.setter
     def cluster_template_revision_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_template_revision_id", value)
 
     @property
+    @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
+    def default_pod_security_admission_configuration_template_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Cluster default pod security admission configuration template name
+        """
+        return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
+
+    @default_pod_security_admission_configuration_template_name.setter
+    def default_pod_security_admission_configuration_template_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_pod_security_admission_configuration_template_name", value)
+
+    @property
     @pulumi.getter(name="defaultPodSecurityPolicyTemplateId")
     def default_pod_security_policy_template_id(self) -> Optional[pulumi.Input[str]]:
         """
         [Default pod security policy template id](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#pod-security-policy-support) (string)
         """
         return pulumi.get(self, "default_pod_security_policy_template_id")
 
@@ -393,14 +429,26 @@
         return pulumi.get(self, "enable_network_policy")
 
     @enable_network_policy.setter
     def enable_network_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_network_policy", value)
 
     @property
+    @pulumi.getter(name="fleetAgentDeploymentCustomizations")
+    def fleet_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]]]:
+        """
+        Optional customization for fleet agent
+        """
+        return pulumi.get(self, "fleet_agent_deployment_customizations")
+
+    @fleet_agent_deployment_customizations.setter
+    def fleet_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]]]):
+        pulumi.set(self, "fleet_agent_deployment_customizations", value)
+
+    @property
     @pulumi.getter(name="fleetWorkspaceName")
     def fleet_workspace_name(self) -> Optional[pulumi.Input[str]]:
         """
         Fleet workspace name (string)
         """
         return pulumi.get(self, "fleet_workspace_name")
 
@@ -521,34 +569,37 @@
 class _ClusterState:
     def __init__(__self__, *,
                  agent_env_vars: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterAgentEnvVarArgs']]]] = None,
                  aks_config: Optional[pulumi.Input['ClusterAksConfigArgs']] = None,
                  aks_config_v2: Optional[pulumi.Input['ClusterAksConfigV2Args']] = None,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  ca_cert: Optional[pulumi.Input[str]] = None,
+                 cluster_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]]] = None,
                  cluster_auth_endpoint: Optional[pulumi.Input['ClusterClusterAuthEndpointArgs']] = None,
                  cluster_monitoring_input: Optional[pulumi.Input['ClusterClusterMonitoringInputArgs']] = None,
                  cluster_registration_token: Optional[pulumi.Input['ClusterClusterRegistrationTokenArgs']] = None,
                  cluster_template_answers: Optional[pulumi.Input['ClusterClusterTemplateAnswersArgs']] = None,
                  cluster_template_id: Optional[pulumi.Input[str]] = None,
                  cluster_template_questions: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterTemplateQuestionArgs']]]] = None,
                  cluster_template_revision_id: Optional[pulumi.Input[str]] = None,
+                 default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[str]] = None,
                  default_pod_security_policy_template_id: Optional[pulumi.Input[str]] = None,
                  default_project_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  desired_agent_image: Optional[pulumi.Input[str]] = None,
                  desired_auth_image: Optional[pulumi.Input[str]] = None,
                  docker_root_dir: Optional[pulumi.Input[str]] = None,
                  driver: Optional[pulumi.Input[str]] = None,
                  eks_config: Optional[pulumi.Input['ClusterEksConfigArgs']] = None,
                  eks_config_v2: Optional[pulumi.Input['ClusterEksConfigV2Args']] = None,
                  enable_cluster_alerting: Optional[pulumi.Input[bool]] = None,
                  enable_cluster_istio: Optional[pulumi.Input[bool]] = None,
                  enable_cluster_monitoring: Optional[pulumi.Input[bool]] = None,
                  enable_network_policy: Optional[pulumi.Input[bool]] = None,
+                 fleet_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]]] = None,
                  fleet_workspace_name: Optional[pulumi.Input[str]] = None,
                  gke_config: Optional[pulumi.Input['ClusterGkeConfigArgs']] = None,
                  gke_config_v2: Optional[pulumi.Input['ClusterGkeConfigV2Args']] = None,
                  istio_enabled: Optional[pulumi.Input[bool]] = None,
                  k3s_config: Optional[pulumi.Input['ClusterK3sConfigArgs']] = None,
                  kube_config: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
@@ -561,34 +612,37 @@
         """
         Input properties used for looking up and filtering Cluster resources.
         :param pulumi.Input[Sequence[pulumi.Input['ClusterAgentEnvVarArgs']]] agent_env_vars: Optional Agent Env Vars for Rancher agent. Just for Rancher v2.5.6 and above (list)
         :param pulumi.Input['ClusterAksConfigArgs'] aks_config: The Azure AKS configuration for `aks` Clusters. Conflicts with `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input['ClusterAksConfigV2Args'] aks_config_v2: The Azure AKS v2 configuration for creating/import `aks` Clusters. Conflicts with `aks_config`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster (map)
         :param pulumi.Input[str] ca_cert: TLS CA certificate for etcd service (string)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]] cluster_agent_deployment_customizations: Optional customization for cluster agent
         :param pulumi.Input['ClusterClusterAuthEndpointArgs'] cluster_auth_endpoint: Enabling the [local cluster authorized endpoint](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#local-cluster-auth-endpoint) allows direct communication with the cluster, bypassing the Rancher API proxy. (list maxitems:1)
         :param pulumi.Input['ClusterClusterMonitoringInputArgs'] cluster_monitoring_input: Cluster monitoring config. Any parameter defined in [rancher-monitoring charts](https://github.com/rancher/system-charts/tree/dev/charts/rancher-monitoring) could be configured  (list maxitems:1)
         :param pulumi.Input['ClusterClusterRegistrationTokenArgs'] cluster_registration_token: (Computed) Cluster Registration Token generated for the cluster (list maxitems:1)
         :param pulumi.Input['ClusterClusterTemplateAnswersArgs'] cluster_template_answers: Cluster template answers. Just for Rancher v2.3.x and above (list maxitems:1)
         :param pulumi.Input[str] cluster_template_id: Cluster template ID. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[Sequence[pulumi.Input['ClusterClusterTemplateQuestionArgs']]] cluster_template_questions: Cluster template questions. Just for Rancher v2.3.x and above (list)
         :param pulumi.Input[str] cluster_template_revision_id: Cluster template revision ID. Just for Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster default pod security admission configuration template name
         :param pulumi.Input[str] default_pod_security_policy_template_id: [Default pod security policy template id](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#pod-security-policy-support) (string)
         :param pulumi.Input[str] default_project_id: (Computed) Default project ID for the cluster (string)
         :param pulumi.Input[str] description: The description for Cluster (string)
         :param pulumi.Input[str] desired_agent_image: Desired agent image. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[str] desired_auth_image: Desired auth image. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[str] docker_root_dir: Desired auth image. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[str] driver: (Computed) The driver used for the Cluster. `imported`, `azurekubernetesservice`, `amazonelasticcontainerservice`, `googlekubernetesengine` and `rancherKubernetesEngine` are supported (string)
         :param pulumi.Input['ClusterEksConfigArgs'] eks_config: The Amazon EKS configuration for `eks` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input['ClusterEksConfigV2Args'] eks_config_v2: The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x or above (list maxitems:1)
         :param pulumi.Input[bool] enable_cluster_alerting: Enable built-in cluster alerting (bool)
         :param pulumi.Input[bool] enable_cluster_istio: Deploy istio on `system` project and `istio-system` namespace, using App resource instead. See above example.
         :param pulumi.Input[bool] enable_cluster_monitoring: Enable built-in cluster monitoring (bool)
         :param pulumi.Input[bool] enable_network_policy: Enable project network isolation (bool)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]] fleet_agent_deployment_customizations: Optional customization for fleet agent
         :param pulumi.Input[str] fleet_workspace_name: Fleet workspace name (string)
         :param pulumi.Input['ClusterGkeConfigArgs'] gke_config: The Google GKE configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config_v2`, `oke_config`, `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input['ClusterGkeConfigV2Args'] gke_config_v2: The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 or above (list maxitems:1)
         :param pulumi.Input[bool] istio_enabled: (Computed) Is istio enabled at cluster? Just for Rancher v2.3.x and above (bool)
         :param pulumi.Input['ClusterK3sConfigArgs'] k3s_config: The K3S configuration for `k3s` imported Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[str] kube_config: (Computed/Sensitive) Kube Config generated for the cluster. Note: For Rancher 2.6.0 and above, when the cluster has `cluster_auth_endpoint` enabled, the kube_config will not be available until the cluster is `connected` (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster (map)
@@ -605,28 +659,32 @@
             pulumi.set(__self__, "aks_config", aks_config)
         if aks_config_v2 is not None:
             pulumi.set(__self__, "aks_config_v2", aks_config_v2)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if ca_cert is not None:
             pulumi.set(__self__, "ca_cert", ca_cert)
+        if cluster_agent_deployment_customizations is not None:
+            pulumi.set(__self__, "cluster_agent_deployment_customizations", cluster_agent_deployment_customizations)
         if cluster_auth_endpoint is not None:
             pulumi.set(__self__, "cluster_auth_endpoint", cluster_auth_endpoint)
         if cluster_monitoring_input is not None:
             pulumi.set(__self__, "cluster_monitoring_input", cluster_monitoring_input)
         if cluster_registration_token is not None:
             pulumi.set(__self__, "cluster_registration_token", cluster_registration_token)
         if cluster_template_answers is not None:
             pulumi.set(__self__, "cluster_template_answers", cluster_template_answers)
         if cluster_template_id is not None:
             pulumi.set(__self__, "cluster_template_id", cluster_template_id)
         if cluster_template_questions is not None:
             pulumi.set(__self__, "cluster_template_questions", cluster_template_questions)
         if cluster_template_revision_id is not None:
             pulumi.set(__self__, "cluster_template_revision_id", cluster_template_revision_id)
+        if default_pod_security_admission_configuration_template_name is not None:
+            pulumi.set(__self__, "default_pod_security_admission_configuration_template_name", default_pod_security_admission_configuration_template_name)
         if default_pod_security_policy_template_id is not None:
             pulumi.set(__self__, "default_pod_security_policy_template_id", default_pod_security_policy_template_id)
         if default_project_id is not None:
             pulumi.set(__self__, "default_project_id", default_project_id)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if desired_agent_image is not None:
@@ -648,14 +706,16 @@
             pulumi.log.warn("""enable_cluster_istio is deprecated: Deploy istio using rancher2_app resource instead""")
         if enable_cluster_istio is not None:
             pulumi.set(__self__, "enable_cluster_istio", enable_cluster_istio)
         if enable_cluster_monitoring is not None:
             pulumi.set(__self__, "enable_cluster_monitoring", enable_cluster_monitoring)
         if enable_network_policy is not None:
             pulumi.set(__self__, "enable_network_policy", enable_network_policy)
+        if fleet_agent_deployment_customizations is not None:
+            pulumi.set(__self__, "fleet_agent_deployment_customizations", fleet_agent_deployment_customizations)
         if fleet_workspace_name is not None:
             pulumi.set(__self__, "fleet_workspace_name", fleet_workspace_name)
         if gke_config is not None:
             pulumi.set(__self__, "gke_config", gke_config)
         if gke_config_v2 is not None:
             pulumi.set(__self__, "gke_config_v2", gke_config_v2)
         if istio_enabled is not None:
@@ -736,14 +796,26 @@
         return pulumi.get(self, "ca_cert")
 
     @ca_cert.setter
     def ca_cert(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ca_cert", value)
 
     @property
+    @pulumi.getter(name="clusterAgentDeploymentCustomizations")
+    def cluster_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]]]:
+        """
+        Optional customization for cluster agent
+        """
+        return pulumi.get(self, "cluster_agent_deployment_customizations")
+
+    @cluster_agent_deployment_customizations.setter
+    def cluster_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterClusterAgentDeploymentCustomizationArgs']]]]):
+        pulumi.set(self, "cluster_agent_deployment_customizations", value)
+
+    @property
     @pulumi.getter(name="clusterAuthEndpoint")
     def cluster_auth_endpoint(self) -> Optional[pulumi.Input['ClusterClusterAuthEndpointArgs']]:
         """
         Enabling the [local cluster authorized endpoint](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#local-cluster-auth-endpoint) allows direct communication with the cluster, bypassing the Rancher API proxy. (list maxitems:1)
         """
         return pulumi.get(self, "cluster_auth_endpoint")
 
@@ -820,14 +892,26 @@
         return pulumi.get(self, "cluster_template_revision_id")
 
     @cluster_template_revision_id.setter
     def cluster_template_revision_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_template_revision_id", value)
 
     @property
+    @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
+    def default_pod_security_admission_configuration_template_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Cluster default pod security admission configuration template name
+        """
+        return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
+
+    @default_pod_security_admission_configuration_template_name.setter
+    def default_pod_security_admission_configuration_template_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_pod_security_admission_configuration_template_name", value)
+
+    @property
     @pulumi.getter(name="defaultPodSecurityPolicyTemplateId")
     def default_pod_security_policy_template_id(self) -> Optional[pulumi.Input[str]]:
         """
         [Default pod security policy template id](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#pod-security-policy-support) (string)
         """
         return pulumi.get(self, "default_pod_security_policy_template_id")
 
@@ -976,14 +1060,26 @@
         return pulumi.get(self, "enable_network_policy")
 
     @enable_network_policy.setter
     def enable_network_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_network_policy", value)
 
     @property
+    @pulumi.getter(name="fleetAgentDeploymentCustomizations")
+    def fleet_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]]]:
+        """
+        Optional customization for fleet agent
+        """
+        return pulumi.get(self, "fleet_agent_deployment_customizations")
+
+    @fleet_agent_deployment_customizations.setter
+    def fleet_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterFleetAgentDeploymentCustomizationArgs']]]]):
+        pulumi.set(self, "fleet_agent_deployment_customizations", value)
+
+    @property
     @pulumi.getter(name="fleetWorkspaceName")
     def fleet_workspace_name(self) -> Optional[pulumi.Input[str]]:
         """
         Fleet workspace name (string)
         """
         return pulumi.get(self, "fleet_workspace_name")
 
@@ -1141,31 +1237,34 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  agent_env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterAgentEnvVarArgs']]]]] = None,
                  aks_config: Optional[pulumi.Input[pulumi.InputType['ClusterAksConfigArgs']]] = None,
                  aks_config_v2: Optional[pulumi.Input[pulumi.InputType['ClusterAksConfigV2Args']]] = None,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 cluster_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterAgentDeploymentCustomizationArgs']]]]] = None,
                  cluster_auth_endpoint: Optional[pulumi.Input[pulumi.InputType['ClusterClusterAuthEndpointArgs']]] = None,
                  cluster_monitoring_input: Optional[pulumi.Input[pulumi.InputType['ClusterClusterMonitoringInputArgs']]] = None,
                  cluster_template_answers: Optional[pulumi.Input[pulumi.InputType['ClusterClusterTemplateAnswersArgs']]] = None,
                  cluster_template_id: Optional[pulumi.Input[str]] = None,
                  cluster_template_questions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterTemplateQuestionArgs']]]]] = None,
                  cluster_template_revision_id: Optional[pulumi.Input[str]] = None,
+                 default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[str]] = None,
                  default_pod_security_policy_template_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  desired_agent_image: Optional[pulumi.Input[str]] = None,
                  desired_auth_image: Optional[pulumi.Input[str]] = None,
                  docker_root_dir: Optional[pulumi.Input[str]] = None,
                  driver: Optional[pulumi.Input[str]] = None,
                  eks_config: Optional[pulumi.Input[pulumi.InputType['ClusterEksConfigArgs']]] = None,
                  eks_config_v2: Optional[pulumi.Input[pulumi.InputType['ClusterEksConfigV2Args']]] = None,
                  enable_cluster_alerting: Optional[pulumi.Input[bool]] = None,
                  enable_cluster_monitoring: Optional[pulumi.Input[bool]] = None,
                  enable_network_policy: Optional[pulumi.Input[bool]] = None,
+                 fleet_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterFleetAgentDeploymentCustomizationArgs']]]]] = None,
                  fleet_workspace_name: Optional[pulumi.Input[str]] = None,
                  gke_config: Optional[pulumi.Input[pulumi.InputType['ClusterGkeConfigArgs']]] = None,
                  gke_config_v2: Optional[pulumi.Input[pulumi.InputType['ClusterGkeConfigV2Args']]] = None,
                  k3s_config: Optional[pulumi.Input[pulumi.InputType['ClusterK3sConfigArgs']]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  oke_config: Optional[pulumi.Input[pulumi.InputType['ClusterOkeConfigArgs']]] = None,
@@ -1550,26 +1649,48 @@
             aks_config_v2=rancher2.ClusterAksConfigV2Args(
                 cloud_credential_id=foo_aks.id,
                 resource_group="<RESOURCE_GROUP>",
                 resource_location="<RESOURCE_LOCATION>",
                 dns_prefix="<DNS_PREFIX>",
                 kubernetes_version="1.24.6",
                 network_plugin="<NETWORK_PLUGIN>",
-                node_pools=[rancher2.ClusterAksConfigV2NodePoolArgs(
-                    availability_zones=[
-                        "1",
-                        "2",
-                        "3",
-                    ],
-                    name="<NODEPOOL_NAME>",
-                    count=1,
-                    orchestrator_version="1.21.2",
-                    os_disk_size_gb=128,
-                    vm_size="Standard_DS2_v2",
-                )],
+                node_pools=[
+                    rancher2.ClusterAksConfigV2NodePoolArgs(
+                        availability_zones=[
+                            "1",
+                            "2",
+                            "3",
+                        ],
+                        name="<NODEPOOL_NAME_1>",
+                        mode="System",
+                        count=1,
+                        orchestrator_version="1.21.2",
+                        os_disk_size_gb=128,
+                        vm_size="Standard_DS2_v2",
+                    ),
+                    rancher2.ClusterAksConfigV2NodePoolArgs(
+                        availability_zones=[
+                            "1",
+                            "2",
+                            "3",
+                        ],
+                        name="<NODEPOOL_NAME_2>",
+                        count=1,
+                        mode="User",
+                        orchestrator_version="1.21.2",
+                        os_disk_size_gb=128,
+                        vm_size="Standard_DS2_v2",
+                        max_surge="25%",
+                        labels={
+                            "test1": "data1",
+                            "test2": "data2",
+                        },
+                        taints=["none:PreferNoSchedule"],
+                    ),
+                ],
             ))
         ```
 
         ## Import
 
         Clusters can be imported using the Rancher Cluster ID
 
@@ -1579,31 +1700,34 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterAgentEnvVarArgs']]]] agent_env_vars: Optional Agent Env Vars for Rancher agent. Just for Rancher v2.5.6 and above (list)
         :param pulumi.Input[pulumi.InputType['ClusterAksConfigArgs']] aks_config: The Azure AKS configuration for `aks` Clusters. Conflicts with `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterAksConfigV2Args']] aks_config_v2: The Azure AKS v2 configuration for creating/import `aks` Clusters. Conflicts with `aks_config`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster (map)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterAgentDeploymentCustomizationArgs']]]] cluster_agent_deployment_customizations: Optional customization for cluster agent
         :param pulumi.Input[pulumi.InputType['ClusterClusterAuthEndpointArgs']] cluster_auth_endpoint: Enabling the [local cluster authorized endpoint](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#local-cluster-auth-endpoint) allows direct communication with the cluster, bypassing the Rancher API proxy. (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterClusterMonitoringInputArgs']] cluster_monitoring_input: Cluster monitoring config. Any parameter defined in [rancher-monitoring charts](https://github.com/rancher/system-charts/tree/dev/charts/rancher-monitoring) could be configured  (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterClusterTemplateAnswersArgs']] cluster_template_answers: Cluster template answers. Just for Rancher v2.3.x and above (list maxitems:1)
         :param pulumi.Input[str] cluster_template_id: Cluster template ID. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterTemplateQuestionArgs']]]] cluster_template_questions: Cluster template questions. Just for Rancher v2.3.x and above (list)
         :param pulumi.Input[str] cluster_template_revision_id: Cluster template revision ID. Just for Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster default pod security admission configuration template name
         :param pulumi.Input[str] default_pod_security_policy_template_id: [Default pod security policy template id](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#pod-security-policy-support) (string)
         :param pulumi.Input[str] description: The description for Cluster (string)
         :param pulumi.Input[str] desired_agent_image: Desired agent image. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[str] desired_auth_image: Desired auth image. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[str] docker_root_dir: Desired auth image. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[str] driver: (Computed) The driver used for the Cluster. `imported`, `azurekubernetesservice`, `amazonelasticcontainerservice`, `googlekubernetesengine` and `rancherKubernetesEngine` are supported (string)
         :param pulumi.Input[pulumi.InputType['ClusterEksConfigArgs']] eks_config: The Amazon EKS configuration for `eks` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterEksConfigV2Args']] eks_config_v2: The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x or above (list maxitems:1)
         :param pulumi.Input[bool] enable_cluster_alerting: Enable built-in cluster alerting (bool)
         :param pulumi.Input[bool] enable_cluster_monitoring: Enable built-in cluster monitoring (bool)
         :param pulumi.Input[bool] enable_network_policy: Enable project network isolation (bool)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterFleetAgentDeploymentCustomizationArgs']]]] fleet_agent_deployment_customizations: Optional customization for fleet agent
         :param pulumi.Input[str] fleet_workspace_name: Fleet workspace name (string)
         :param pulumi.Input[pulumi.InputType['ClusterGkeConfigArgs']] gke_config: The Google GKE configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config_v2`, `oke_config`, `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterGkeConfigV2Args']] gke_config_v2: The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 or above (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterK3sConfigArgs']] k3s_config: The K3S configuration for `k3s` imported Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster (map)
         :param pulumi.Input[str] name: The name of the Cluster (string)
         :param pulumi.Input[pulumi.InputType['ClusterOkeConfigArgs']] oke_config: The Oracle OKE configuration for `oke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `k3s_config` and `rke_config` (list maxitems:1)
@@ -1994,26 +2118,48 @@
             aks_config_v2=rancher2.ClusterAksConfigV2Args(
                 cloud_credential_id=foo_aks.id,
                 resource_group="<RESOURCE_GROUP>",
                 resource_location="<RESOURCE_LOCATION>",
                 dns_prefix="<DNS_PREFIX>",
                 kubernetes_version="1.24.6",
                 network_plugin="<NETWORK_PLUGIN>",
-                node_pools=[rancher2.ClusterAksConfigV2NodePoolArgs(
-                    availability_zones=[
-                        "1",
-                        "2",
-                        "3",
-                    ],
-                    name="<NODEPOOL_NAME>",
-                    count=1,
-                    orchestrator_version="1.21.2",
-                    os_disk_size_gb=128,
-                    vm_size="Standard_DS2_v2",
-                )],
+                node_pools=[
+                    rancher2.ClusterAksConfigV2NodePoolArgs(
+                        availability_zones=[
+                            "1",
+                            "2",
+                            "3",
+                        ],
+                        name="<NODEPOOL_NAME_1>",
+                        mode="System",
+                        count=1,
+                        orchestrator_version="1.21.2",
+                        os_disk_size_gb=128,
+                        vm_size="Standard_DS2_v2",
+                    ),
+                    rancher2.ClusterAksConfigV2NodePoolArgs(
+                        availability_zones=[
+                            "1",
+                            "2",
+                            "3",
+                        ],
+                        name="<NODEPOOL_NAME_2>",
+                        count=1,
+                        mode="User",
+                        orchestrator_version="1.21.2",
+                        os_disk_size_gb=128,
+                        vm_size="Standard_DS2_v2",
+                        max_surge="25%",
+                        labels={
+                            "test1": "data1",
+                            "test2": "data2",
+                        },
+                        taints=["none:PreferNoSchedule"],
+                    ),
+                ],
             ))
         ```
 
         ## Import
 
         Clusters can be imported using the Rancher Cluster ID
 
@@ -2036,31 +2182,34 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  agent_env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterAgentEnvVarArgs']]]]] = None,
                  aks_config: Optional[pulumi.Input[pulumi.InputType['ClusterAksConfigArgs']]] = None,
                  aks_config_v2: Optional[pulumi.Input[pulumi.InputType['ClusterAksConfigV2Args']]] = None,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 cluster_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterAgentDeploymentCustomizationArgs']]]]] = None,
                  cluster_auth_endpoint: Optional[pulumi.Input[pulumi.InputType['ClusterClusterAuthEndpointArgs']]] = None,
                  cluster_monitoring_input: Optional[pulumi.Input[pulumi.InputType['ClusterClusterMonitoringInputArgs']]] = None,
                  cluster_template_answers: Optional[pulumi.Input[pulumi.InputType['ClusterClusterTemplateAnswersArgs']]] = None,
                  cluster_template_id: Optional[pulumi.Input[str]] = None,
                  cluster_template_questions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterTemplateQuestionArgs']]]]] = None,
                  cluster_template_revision_id: Optional[pulumi.Input[str]] = None,
+                 default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[str]] = None,
                  default_pod_security_policy_template_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  desired_agent_image: Optional[pulumi.Input[str]] = None,
                  desired_auth_image: Optional[pulumi.Input[str]] = None,
                  docker_root_dir: Optional[pulumi.Input[str]] = None,
                  driver: Optional[pulumi.Input[str]] = None,
                  eks_config: Optional[pulumi.Input[pulumi.InputType['ClusterEksConfigArgs']]] = None,
                  eks_config_v2: Optional[pulumi.Input[pulumi.InputType['ClusterEksConfigV2Args']]] = None,
                  enable_cluster_alerting: Optional[pulumi.Input[bool]] = None,
                  enable_cluster_monitoring: Optional[pulumi.Input[bool]] = None,
                  enable_network_policy: Optional[pulumi.Input[bool]] = None,
+                 fleet_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterFleetAgentDeploymentCustomizationArgs']]]]] = None,
                  fleet_workspace_name: Optional[pulumi.Input[str]] = None,
                  gke_config: Optional[pulumi.Input[pulumi.InputType['ClusterGkeConfigArgs']]] = None,
                  gke_config_v2: Optional[pulumi.Input[pulumi.InputType['ClusterGkeConfigV2Args']]] = None,
                  k3s_config: Optional[pulumi.Input[pulumi.InputType['ClusterK3sConfigArgs']]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  oke_config: Optional[pulumi.Input[pulumi.InputType['ClusterOkeConfigArgs']]] = None,
@@ -2076,31 +2225,34 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ClusterArgs.__new__(ClusterArgs)
 
             __props__.__dict__["agent_env_vars"] = agent_env_vars
             __props__.__dict__["aks_config"] = aks_config
             __props__.__dict__["aks_config_v2"] = aks_config_v2
             __props__.__dict__["annotations"] = annotations
+            __props__.__dict__["cluster_agent_deployment_customizations"] = cluster_agent_deployment_customizations
             __props__.__dict__["cluster_auth_endpoint"] = cluster_auth_endpoint
             __props__.__dict__["cluster_monitoring_input"] = cluster_monitoring_input
             __props__.__dict__["cluster_template_answers"] = cluster_template_answers
             __props__.__dict__["cluster_template_id"] = cluster_template_id
             __props__.__dict__["cluster_template_questions"] = cluster_template_questions
             __props__.__dict__["cluster_template_revision_id"] = cluster_template_revision_id
+            __props__.__dict__["default_pod_security_admission_configuration_template_name"] = default_pod_security_admission_configuration_template_name
             __props__.__dict__["default_pod_security_policy_template_id"] = default_pod_security_policy_template_id
             __props__.__dict__["description"] = description
             __props__.__dict__["desired_agent_image"] = desired_agent_image
             __props__.__dict__["desired_auth_image"] = desired_auth_image
             __props__.__dict__["docker_root_dir"] = docker_root_dir
             __props__.__dict__["driver"] = driver
             __props__.__dict__["eks_config"] = eks_config
             __props__.__dict__["eks_config_v2"] = eks_config_v2
             __props__.__dict__["enable_cluster_alerting"] = enable_cluster_alerting
             __props__.__dict__["enable_cluster_monitoring"] = enable_cluster_monitoring
             __props__.__dict__["enable_network_policy"] = enable_network_policy
+            __props__.__dict__["fleet_agent_deployment_customizations"] = fleet_agent_deployment_customizations
             __props__.__dict__["fleet_workspace_name"] = fleet_workspace_name
             __props__.__dict__["gke_config"] = gke_config
             __props__.__dict__["gke_config_v2"] = gke_config_v2
             __props__.__dict__["k3s_config"] = k3s_config
             __props__.__dict__["labels"] = labels
             __props__.__dict__["name"] = name
             __props__.__dict__["oke_config"] = oke_config
@@ -2127,34 +2279,37 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             agent_env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterAgentEnvVarArgs']]]]] = None,
             aks_config: Optional[pulumi.Input[pulumi.InputType['ClusterAksConfigArgs']]] = None,
             aks_config_v2: Optional[pulumi.Input[pulumi.InputType['ClusterAksConfigV2Args']]] = None,
             annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
             ca_cert: Optional[pulumi.Input[str]] = None,
+            cluster_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterAgentDeploymentCustomizationArgs']]]]] = None,
             cluster_auth_endpoint: Optional[pulumi.Input[pulumi.InputType['ClusterClusterAuthEndpointArgs']]] = None,
             cluster_monitoring_input: Optional[pulumi.Input[pulumi.InputType['ClusterClusterMonitoringInputArgs']]] = None,
             cluster_registration_token: Optional[pulumi.Input[pulumi.InputType['ClusterClusterRegistrationTokenArgs']]] = None,
             cluster_template_answers: Optional[pulumi.Input[pulumi.InputType['ClusterClusterTemplateAnswersArgs']]] = None,
             cluster_template_id: Optional[pulumi.Input[str]] = None,
             cluster_template_questions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterTemplateQuestionArgs']]]]] = None,
             cluster_template_revision_id: Optional[pulumi.Input[str]] = None,
+            default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[str]] = None,
             default_pod_security_policy_template_id: Optional[pulumi.Input[str]] = None,
             default_project_id: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             desired_agent_image: Optional[pulumi.Input[str]] = None,
             desired_auth_image: Optional[pulumi.Input[str]] = None,
             docker_root_dir: Optional[pulumi.Input[str]] = None,
             driver: Optional[pulumi.Input[str]] = None,
             eks_config: Optional[pulumi.Input[pulumi.InputType['ClusterEksConfigArgs']]] = None,
             eks_config_v2: Optional[pulumi.Input[pulumi.InputType['ClusterEksConfigV2Args']]] = None,
             enable_cluster_alerting: Optional[pulumi.Input[bool]] = None,
             enable_cluster_istio: Optional[pulumi.Input[bool]] = None,
             enable_cluster_monitoring: Optional[pulumi.Input[bool]] = None,
             enable_network_policy: Optional[pulumi.Input[bool]] = None,
+            fleet_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterFleetAgentDeploymentCustomizationArgs']]]]] = None,
             fleet_workspace_name: Optional[pulumi.Input[str]] = None,
             gke_config: Optional[pulumi.Input[pulumi.InputType['ClusterGkeConfigArgs']]] = None,
             gke_config_v2: Optional[pulumi.Input[pulumi.InputType['ClusterGkeConfigV2Args']]] = None,
             istio_enabled: Optional[pulumi.Input[bool]] = None,
             k3s_config: Optional[pulumi.Input[pulumi.InputType['ClusterK3sConfigArgs']]] = None,
             kube_config: Optional[pulumi.Input[str]] = None,
             labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
@@ -2172,34 +2327,37 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterAgentEnvVarArgs']]]] agent_env_vars: Optional Agent Env Vars for Rancher agent. Just for Rancher v2.5.6 and above (list)
         :param pulumi.Input[pulumi.InputType['ClusterAksConfigArgs']] aks_config: The Azure AKS configuration for `aks` Clusters. Conflicts with `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterAksConfigV2Args']] aks_config_v2: The Azure AKS v2 configuration for creating/import `aks` Clusters. Conflicts with `aks_config`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster (map)
         :param pulumi.Input[str] ca_cert: TLS CA certificate for etcd service (string)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterAgentDeploymentCustomizationArgs']]]] cluster_agent_deployment_customizations: Optional customization for cluster agent
         :param pulumi.Input[pulumi.InputType['ClusterClusterAuthEndpointArgs']] cluster_auth_endpoint: Enabling the [local cluster authorized endpoint](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#local-cluster-auth-endpoint) allows direct communication with the cluster, bypassing the Rancher API proxy. (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterClusterMonitoringInputArgs']] cluster_monitoring_input: Cluster monitoring config. Any parameter defined in [rancher-monitoring charts](https://github.com/rancher/system-charts/tree/dev/charts/rancher-monitoring) could be configured  (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterClusterRegistrationTokenArgs']] cluster_registration_token: (Computed) Cluster Registration Token generated for the cluster (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterClusterTemplateAnswersArgs']] cluster_template_answers: Cluster template answers. Just for Rancher v2.3.x and above (list maxitems:1)
         :param pulumi.Input[str] cluster_template_id: Cluster template ID. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterClusterTemplateQuestionArgs']]]] cluster_template_questions: Cluster template questions. Just for Rancher v2.3.x and above (list)
         :param pulumi.Input[str] cluster_template_revision_id: Cluster template revision ID. Just for Rancher v2.3.x and above (string)
+        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster default pod security admission configuration template name
         :param pulumi.Input[str] default_pod_security_policy_template_id: [Default pod security policy template id](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#pod-security-policy-support) (string)
         :param pulumi.Input[str] default_project_id: (Computed) Default project ID for the cluster (string)
         :param pulumi.Input[str] description: The description for Cluster (string)
         :param pulumi.Input[str] desired_agent_image: Desired agent image. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[str] desired_auth_image: Desired auth image. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[str] docker_root_dir: Desired auth image. Just for Rancher v2.3.x and above (string)
         :param pulumi.Input[str] driver: (Computed) The driver used for the Cluster. `imported`, `azurekubernetesservice`, `amazonelasticcontainerservice`, `googlekubernetesengine` and `rancherKubernetesEngine` are supported (string)
         :param pulumi.Input[pulumi.InputType['ClusterEksConfigArgs']] eks_config: The Amazon EKS configuration for `eks` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterEksConfigV2Args']] eks_config_v2: The Amazon EKS V2 configuration to create or import `eks` Clusters. Conflicts with `aks_config`, `eks_config`, `gke_config`, `gke_config_v2`, `oke_config` `k3s_config` and `rke_config`. For Rancher v2.5.x or above (list maxitems:1)
         :param pulumi.Input[bool] enable_cluster_alerting: Enable built-in cluster alerting (bool)
         :param pulumi.Input[bool] enable_cluster_istio: Deploy istio on `system` project and `istio-system` namespace, using App resource instead. See above example.
         :param pulumi.Input[bool] enable_cluster_monitoring: Enable built-in cluster monitoring (bool)
         :param pulumi.Input[bool] enable_network_policy: Enable project network isolation (bool)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterFleetAgentDeploymentCustomizationArgs']]]] fleet_agent_deployment_customizations: Optional customization for fleet agent
         :param pulumi.Input[str] fleet_workspace_name: Fleet workspace name (string)
         :param pulumi.Input[pulumi.InputType['ClusterGkeConfigArgs']] gke_config: The Google GKE configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config_v2`, `oke_config`, `k3s_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[pulumi.InputType['ClusterGkeConfigV2Args']] gke_config_v2: The Google GKE V2 configuration for `gke` Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `oke_config`, `k3s_config` and `rke_config`. For Rancher v2.5.8 or above (list maxitems:1)
         :param pulumi.Input[bool] istio_enabled: (Computed) Is istio enabled at cluster? Just for Rancher v2.3.x and above (bool)
         :param pulumi.Input[pulumi.InputType['ClusterK3sConfigArgs']] k3s_config: The K3S configuration for `k3s` imported Clusters. Conflicts with `aks_config`, `aks_config_v2`, `eks_config`, `eks_config_v2`, `gke_config`, `gke_config_v2`, `oke_config` and `rke_config` (list maxitems:1)
         :param pulumi.Input[str] kube_config: (Computed/Sensitive) Kube Config generated for the cluster. Note: For Rancher 2.6.0 and above, when the cluster has `cluster_auth_endpoint` enabled, the kube_config will not be available until the cluster is `connected` (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster (map)
@@ -2215,34 +2373,37 @@
         __props__ = _ClusterState.__new__(_ClusterState)
 
         __props__.__dict__["agent_env_vars"] = agent_env_vars
         __props__.__dict__["aks_config"] = aks_config
         __props__.__dict__["aks_config_v2"] = aks_config_v2
         __props__.__dict__["annotations"] = annotations
         __props__.__dict__["ca_cert"] = ca_cert
+        __props__.__dict__["cluster_agent_deployment_customizations"] = cluster_agent_deployment_customizations
         __props__.__dict__["cluster_auth_endpoint"] = cluster_auth_endpoint
         __props__.__dict__["cluster_monitoring_input"] = cluster_monitoring_input
         __props__.__dict__["cluster_registration_token"] = cluster_registration_token
         __props__.__dict__["cluster_template_answers"] = cluster_template_answers
         __props__.__dict__["cluster_template_id"] = cluster_template_id
         __props__.__dict__["cluster_template_questions"] = cluster_template_questions
         __props__.__dict__["cluster_template_revision_id"] = cluster_template_revision_id
+        __props__.__dict__["default_pod_security_admission_configuration_template_name"] = default_pod_security_admission_configuration_template_name
         __props__.__dict__["default_pod_security_policy_template_id"] = default_pod_security_policy_template_id
         __props__.__dict__["default_project_id"] = default_project_id
         __props__.__dict__["description"] = description
         __props__.__dict__["desired_agent_image"] = desired_agent_image
         __props__.__dict__["desired_auth_image"] = desired_auth_image
         __props__.__dict__["docker_root_dir"] = docker_root_dir
         __props__.__dict__["driver"] = driver
         __props__.__dict__["eks_config"] = eks_config
         __props__.__dict__["eks_config_v2"] = eks_config_v2
         __props__.__dict__["enable_cluster_alerting"] = enable_cluster_alerting
         __props__.__dict__["enable_cluster_istio"] = enable_cluster_istio
         __props__.__dict__["enable_cluster_monitoring"] = enable_cluster_monitoring
         __props__.__dict__["enable_network_policy"] = enable_network_policy
+        __props__.__dict__["fleet_agent_deployment_customizations"] = fleet_agent_deployment_customizations
         __props__.__dict__["fleet_workspace_name"] = fleet_workspace_name
         __props__.__dict__["gke_config"] = gke_config
         __props__.__dict__["gke_config_v2"] = gke_config_v2
         __props__.__dict__["istio_enabled"] = istio_enabled
         __props__.__dict__["k3s_config"] = k3s_config
         __props__.__dict__["kube_config"] = kube_config
         __props__.__dict__["labels"] = labels
@@ -2291,14 +2452,22 @@
     def ca_cert(self) -> pulumi.Output[str]:
         """
         TLS CA certificate for etcd service (string)
         """
         return pulumi.get(self, "ca_cert")
 
     @property
+    @pulumi.getter(name="clusterAgentDeploymentCustomizations")
+    def cluster_agent_deployment_customizations(self) -> pulumi.Output[Optional[Sequence['outputs.ClusterClusterAgentDeploymentCustomization']]]:
+        """
+        Optional customization for cluster agent
+        """
+        return pulumi.get(self, "cluster_agent_deployment_customizations")
+
+    @property
     @pulumi.getter(name="clusterAuthEndpoint")
     def cluster_auth_endpoint(self) -> pulumi.Output['outputs.ClusterClusterAuthEndpoint']:
         """
         Enabling the [local cluster authorized endpoint](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#local-cluster-auth-endpoint) allows direct communication with the cluster, bypassing the Rancher API proxy. (list maxitems:1)
         """
         return pulumi.get(self, "cluster_auth_endpoint")
 
@@ -2347,14 +2516,22 @@
     def cluster_template_revision_id(self) -> pulumi.Output[Optional[str]]:
         """
         Cluster template revision ID. Just for Rancher v2.3.x and above (string)
         """
         return pulumi.get(self, "cluster_template_revision_id")
 
     @property
+    @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
+    def default_pod_security_admission_configuration_template_name(self) -> pulumi.Output[str]:
+        """
+        Cluster default pod security admission configuration template name
+        """
+        return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
+
+    @property
     @pulumi.getter(name="defaultPodSecurityPolicyTemplateId")
     def default_pod_security_policy_template_id(self) -> pulumi.Output[str]:
         """
         [Default pod security policy template id](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#pod-security-policy-support) (string)
         """
         return pulumi.get(self, "default_pod_security_policy_template_id")
 
@@ -2451,14 +2628,22 @@
     def enable_network_policy(self) -> pulumi.Output[bool]:
         """
         Enable project network isolation (bool)
         """
         return pulumi.get(self, "enable_network_policy")
 
     @property
+    @pulumi.getter(name="fleetAgentDeploymentCustomizations")
+    def fleet_agent_deployment_customizations(self) -> pulumi.Output[Optional[Sequence['outputs.ClusterFleetAgentDeploymentCustomization']]]:
+        """
+        Optional customization for fleet agent
+        """
+        return pulumi.get(self, "fleet_agent_deployment_customizations")
+
+    @property
     @pulumi.getter(name="fleetWorkspaceName")
     def fleet_workspace_name(self) -> pulumi.Output[str]:
         """
         Fleet workspace name (string)
         """
         return pulumi.get(self, "fleet_workspace_name")
```

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_alert_group.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_alert_rule.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_alter_group.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_alter_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_alter_rule.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_alter_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_driver.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_role_template_binding.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_sync.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_sync.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_template.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/cluster_v2.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/cluster_v2.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,50 +16,62 @@
 @pulumi.input_type
 class ClusterV2Args:
     def __init__(__self__, *,
                  kubernetes_version: pulumi.Input[str],
                  agent_env_vars: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2AgentEnvVarArgs']]]] = None,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  cloud_credential_secret_name: Optional[pulumi.Input[str]] = None,
+                 cluster_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]] = None,
                  default_cluster_role_for_project_members: Optional[pulumi.Input[str]] = None,
+                 default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[str]] = None,
                  default_pod_security_policy_template_name: Optional[pulumi.Input[str]] = None,
                  enable_network_policy: Optional[pulumi.Input[bool]] = None,
+                 fleet_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]]] = None,
                  fleet_namespace: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  local_auth_endpoint: Optional[pulumi.Input['ClusterV2LocalAuthEndpointArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  rke_config: Optional[pulumi.Input['ClusterV2RkeConfigArgs']] = None):
         """
         The set of arguments for constructing a ClusterV2 resource.
         :param pulumi.Input[str] kubernetes_version: The kubernetes version of the Cluster v2 (list maxitems:1)
         :param pulumi.Input[Sequence[pulumi.Input['ClusterV2AgentEnvVarArgs']]] agent_env_vars: Optional Agent Env Vars for Rancher agent (list)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster V2 (map)
         :param pulumi.Input[str] cloud_credential_secret_name: Cluster V2 cloud credential secret name (string)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]] cluster_agent_deployment_customizations: Optional customization for cluster agent
         :param pulumi.Input[str] default_cluster_role_for_project_members: Cluster V2 default cluster role for project members (string)
+        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster V2 default pod security admission configuration template name (string)
         :param pulumi.Input[str] default_pod_security_policy_template_name: Cluster V2 default pod security policy template name (string)
         :param pulumi.Input[bool] enable_network_policy: Enable k8s network policy at Cluster V2 (bool)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]] fleet_agent_deployment_customizations: Optional customization for fleet agent
         :param pulumi.Input[str] fleet_namespace: The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster V2 (map)
         :param pulumi.Input['ClusterV2LocalAuthEndpointArgs'] local_auth_endpoint: Cluster V2 local auth endpoint (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Cluster v2 (string)
         :param pulumi.Input['ClusterV2RkeConfigArgs'] rke_config: The RKE configuration for `k3s` and `rke2` Clusters v2. (list maxitems:1)
         """
         pulumi.set(__self__, "kubernetes_version", kubernetes_version)
         if agent_env_vars is not None:
             pulumi.set(__self__, "agent_env_vars", agent_env_vars)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if cloud_credential_secret_name is not None:
             pulumi.set(__self__, "cloud_credential_secret_name", cloud_credential_secret_name)
+        if cluster_agent_deployment_customizations is not None:
+            pulumi.set(__self__, "cluster_agent_deployment_customizations", cluster_agent_deployment_customizations)
         if default_cluster_role_for_project_members is not None:
             pulumi.set(__self__, "default_cluster_role_for_project_members", default_cluster_role_for_project_members)
+        if default_pod_security_admission_configuration_template_name is not None:
+            pulumi.set(__self__, "default_pod_security_admission_configuration_template_name", default_pod_security_admission_configuration_template_name)
         if default_pod_security_policy_template_name is not None:
             pulumi.set(__self__, "default_pod_security_policy_template_name", default_pod_security_policy_template_name)
         if enable_network_policy is not None:
             pulumi.set(__self__, "enable_network_policy", enable_network_policy)
+        if fleet_agent_deployment_customizations is not None:
+            pulumi.set(__self__, "fleet_agent_deployment_customizations", fleet_agent_deployment_customizations)
         if fleet_namespace is not None:
             pulumi.set(__self__, "fleet_namespace", fleet_namespace)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if local_auth_endpoint is not None:
             pulumi.set(__self__, "local_auth_endpoint", local_auth_endpoint)
         if name is not None:
@@ -112,26 +124,50 @@
         return pulumi.get(self, "cloud_credential_secret_name")
 
     @cloud_credential_secret_name.setter
     def cloud_credential_secret_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cloud_credential_secret_name", value)
 
     @property
+    @pulumi.getter(name="clusterAgentDeploymentCustomizations")
+    def cluster_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]]:
+        """
+        Optional customization for cluster agent
+        """
+        return pulumi.get(self, "cluster_agent_deployment_customizations")
+
+    @cluster_agent_deployment_customizations.setter
+    def cluster_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]]):
+        pulumi.set(self, "cluster_agent_deployment_customizations", value)
+
+    @property
     @pulumi.getter(name="defaultClusterRoleForProjectMembers")
     def default_cluster_role_for_project_members(self) -> Optional[pulumi.Input[str]]:
         """
         Cluster V2 default cluster role for project members (string)
         """
         return pulumi.get(self, "default_cluster_role_for_project_members")
 
     @default_cluster_role_for_project_members.setter
     def default_cluster_role_for_project_members(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_cluster_role_for_project_members", value)
 
     @property
+    @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
+    def default_pod_security_admission_configuration_template_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Cluster V2 default pod security admission configuration template name (string)
+        """
+        return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
+
+    @default_pod_security_admission_configuration_template_name.setter
+    def default_pod_security_admission_configuration_template_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_pod_security_admission_configuration_template_name", value)
+
+    @property
     @pulumi.getter(name="defaultPodSecurityPolicyTemplateName")
     def default_pod_security_policy_template_name(self) -> Optional[pulumi.Input[str]]:
         """
         Cluster V2 default pod security policy template name (string)
         """
         return pulumi.get(self, "default_pod_security_policy_template_name")
 
@@ -148,14 +184,26 @@
         return pulumi.get(self, "enable_network_policy")
 
     @enable_network_policy.setter
     def enable_network_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_network_policy", value)
 
     @property
+    @pulumi.getter(name="fleetAgentDeploymentCustomizations")
+    def fleet_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]]]:
+        """
+        Optional customization for fleet agent
+        """
+        return pulumi.get(self, "fleet_agent_deployment_customizations")
+
+    @fleet_agent_deployment_customizations.setter
+    def fleet_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]]]):
+        pulumi.set(self, "fleet_agent_deployment_customizations", value)
+
+    @property
     @pulumi.getter(name="fleetNamespace")
     def fleet_namespace(self) -> Optional[pulumi.Input[str]]:
         """
         The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
         """
         return pulumi.get(self, "fleet_namespace")
 
@@ -214,37 +262,43 @@
 
 @pulumi.input_type
 class _ClusterV2State:
     def __init__(__self__, *,
                  agent_env_vars: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2AgentEnvVarArgs']]]] = None,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  cloud_credential_secret_name: Optional[pulumi.Input[str]] = None,
+                 cluster_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]] = None,
                  cluster_registration_token: Optional[pulumi.Input['ClusterV2ClusterRegistrationTokenArgs']] = None,
                  cluster_v1_id: Optional[pulumi.Input[str]] = None,
                  default_cluster_role_for_project_members: Optional[pulumi.Input[str]] = None,
+                 default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[str]] = None,
                  default_pod_security_policy_template_name: Optional[pulumi.Input[str]] = None,
                  enable_network_policy: Optional[pulumi.Input[bool]] = None,
+                 fleet_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]]] = None,
                  fleet_namespace: Optional[pulumi.Input[str]] = None,
                  kube_config: Optional[pulumi.Input[str]] = None,
                  kubernetes_version: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  local_auth_endpoint: Optional[pulumi.Input['ClusterV2LocalAuthEndpointArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  resource_version: Optional[pulumi.Input[str]] = None,
                  rke_config: Optional[pulumi.Input['ClusterV2RkeConfigArgs']] = None):
         """
         Input properties used for looking up and filtering ClusterV2 resources.
         :param pulumi.Input[Sequence[pulumi.Input['ClusterV2AgentEnvVarArgs']]] agent_env_vars: Optional Agent Env Vars for Rancher agent (list)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster V2 (map)
         :param pulumi.Input[str] cloud_credential_secret_name: Cluster V2 cloud credential secret name (string)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]] cluster_agent_deployment_customizations: Optional customization for cluster agent
         :param pulumi.Input['ClusterV2ClusterRegistrationTokenArgs'] cluster_registration_token: (Computed/Sensitive) Cluster Registration Token generated for the cluster v2 (list maxitems:1)
         :param pulumi.Input[str] cluster_v1_id: (Computed) Cluster v1 id for cluster v2. (e.g to be used with `rancher2_sync`) (string)
         :param pulumi.Input[str] default_cluster_role_for_project_members: Cluster V2 default cluster role for project members (string)
+        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster V2 default pod security admission configuration template name (string)
         :param pulumi.Input[str] default_pod_security_policy_template_name: Cluster V2 default pod security policy template name (string)
         :param pulumi.Input[bool] enable_network_policy: Enable k8s network policy at Cluster V2 (bool)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]] fleet_agent_deployment_customizations: Optional customization for fleet agent
         :param pulumi.Input[str] fleet_namespace: The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
         :param pulumi.Input[str] kube_config: (Computed/Sensitive) Kube Config generated for the cluster v2. Note: When the cluster has `local_auth_endpoint` enabled, the kube_config will not be available until the cluster is `connected` (string)
         :param pulumi.Input[str] kubernetes_version: The kubernetes version of the Cluster v2 (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster V2 (map)
         :param pulumi.Input['ClusterV2LocalAuthEndpointArgs'] local_auth_endpoint: Cluster V2 local auth endpoint (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Cluster v2 (string)
         :param pulumi.Input[str] resource_version: (Computed) Cluster v2 k8s resource version (string)
@@ -252,24 +306,30 @@
         """
         if agent_env_vars is not None:
             pulumi.set(__self__, "agent_env_vars", agent_env_vars)
         if annotations is not None:
             pulumi.set(__self__, "annotations", annotations)
         if cloud_credential_secret_name is not None:
             pulumi.set(__self__, "cloud_credential_secret_name", cloud_credential_secret_name)
+        if cluster_agent_deployment_customizations is not None:
+            pulumi.set(__self__, "cluster_agent_deployment_customizations", cluster_agent_deployment_customizations)
         if cluster_registration_token is not None:
             pulumi.set(__self__, "cluster_registration_token", cluster_registration_token)
         if cluster_v1_id is not None:
             pulumi.set(__self__, "cluster_v1_id", cluster_v1_id)
         if default_cluster_role_for_project_members is not None:
             pulumi.set(__self__, "default_cluster_role_for_project_members", default_cluster_role_for_project_members)
+        if default_pod_security_admission_configuration_template_name is not None:
+            pulumi.set(__self__, "default_pod_security_admission_configuration_template_name", default_pod_security_admission_configuration_template_name)
         if default_pod_security_policy_template_name is not None:
             pulumi.set(__self__, "default_pod_security_policy_template_name", default_pod_security_policy_template_name)
         if enable_network_policy is not None:
             pulumi.set(__self__, "enable_network_policy", enable_network_policy)
+        if fleet_agent_deployment_customizations is not None:
+            pulumi.set(__self__, "fleet_agent_deployment_customizations", fleet_agent_deployment_customizations)
         if fleet_namespace is not None:
             pulumi.set(__self__, "fleet_namespace", fleet_namespace)
         if kube_config is not None:
             pulumi.set(__self__, "kube_config", kube_config)
         if kubernetes_version is not None:
             pulumi.set(__self__, "kubernetes_version", kubernetes_version)
         if labels is not None:
@@ -316,14 +376,26 @@
         return pulumi.get(self, "cloud_credential_secret_name")
 
     @cloud_credential_secret_name.setter
     def cloud_credential_secret_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cloud_credential_secret_name", value)
 
     @property
+    @pulumi.getter(name="clusterAgentDeploymentCustomizations")
+    def cluster_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]]:
+        """
+        Optional customization for cluster agent
+        """
+        return pulumi.get(self, "cluster_agent_deployment_customizations")
+
+    @cluster_agent_deployment_customizations.setter
+    def cluster_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]]):
+        pulumi.set(self, "cluster_agent_deployment_customizations", value)
+
+    @property
     @pulumi.getter(name="clusterRegistrationToken")
     def cluster_registration_token(self) -> Optional[pulumi.Input['ClusterV2ClusterRegistrationTokenArgs']]:
         """
         (Computed/Sensitive) Cluster Registration Token generated for the cluster v2 (list maxitems:1)
         """
         return pulumi.get(self, "cluster_registration_token")
 
@@ -352,14 +424,26 @@
         return pulumi.get(self, "default_cluster_role_for_project_members")
 
     @default_cluster_role_for_project_members.setter
     def default_cluster_role_for_project_members(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_cluster_role_for_project_members", value)
 
     @property
+    @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
+    def default_pod_security_admission_configuration_template_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Cluster V2 default pod security admission configuration template name (string)
+        """
+        return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
+
+    @default_pod_security_admission_configuration_template_name.setter
+    def default_pod_security_admission_configuration_template_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_pod_security_admission_configuration_template_name", value)
+
+    @property
     @pulumi.getter(name="defaultPodSecurityPolicyTemplateName")
     def default_pod_security_policy_template_name(self) -> Optional[pulumi.Input[str]]:
         """
         Cluster V2 default pod security policy template name (string)
         """
         return pulumi.get(self, "default_pod_security_policy_template_name")
 
@@ -376,14 +460,26 @@
         return pulumi.get(self, "enable_network_policy")
 
     @enable_network_policy.setter
     def enable_network_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_network_policy", value)
 
     @property
+    @pulumi.getter(name="fleetAgentDeploymentCustomizations")
+    def fleet_agent_deployment_customizations(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]]]:
+        """
+        Optional customization for fleet agent
+        """
+        return pulumi.get(self, "fleet_agent_deployment_customizations")
+
+    @fleet_agent_deployment_customizations.setter
+    def fleet_agent_deployment_customizations(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterV2FleetAgentDeploymentCustomizationArgs']]]]):
+        pulumi.set(self, "fleet_agent_deployment_customizations", value)
+
+    @property
     @pulumi.getter(name="fleetNamespace")
     def fleet_namespace(self) -> Optional[pulumi.Input[str]]:
         """
         The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
         """
         return pulumi.get(self, "fleet_namespace")
 
@@ -480,17 +576,20 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  agent_env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2AgentEnvVarArgs']]]]] = None,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  cloud_credential_secret_name: Optional[pulumi.Input[str]] = None,
+                 cluster_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]]] = None,
                  default_cluster_role_for_project_members: Optional[pulumi.Input[str]] = None,
+                 default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[str]] = None,
                  default_pod_security_policy_template_name: Optional[pulumi.Input[str]] = None,
                  enable_network_policy: Optional[pulumi.Input[bool]] = None,
+                 fleet_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2FleetAgentDeploymentCustomizationArgs']]]]] = None,
                  fleet_namespace: Optional[pulumi.Input[str]] = None,
                  kubernetes_version: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  local_auth_endpoint: Optional[pulumi.Input[pulumi.InputType['ClusterV2LocalAuthEndpointArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  rke_config: Optional[pulumi.Input[pulumi.InputType['ClusterV2RkeConfigArgs']]] = None,
                  __props__=None):
@@ -523,17 +622,20 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2AgentEnvVarArgs']]]] agent_env_vars: Optional Agent Env Vars for Rancher agent (list)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster V2 (map)
         :param pulumi.Input[str] cloud_credential_secret_name: Cluster V2 cloud credential secret name (string)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]] cluster_agent_deployment_customizations: Optional customization for cluster agent
         :param pulumi.Input[str] default_cluster_role_for_project_members: Cluster V2 default cluster role for project members (string)
+        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster V2 default pod security admission configuration template name (string)
         :param pulumi.Input[str] default_pod_security_policy_template_name: Cluster V2 default pod security policy template name (string)
         :param pulumi.Input[bool] enable_network_policy: Enable k8s network policy at Cluster V2 (bool)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2FleetAgentDeploymentCustomizationArgs']]]] fleet_agent_deployment_customizations: Optional customization for fleet agent
         :param pulumi.Input[str] fleet_namespace: The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
         :param pulumi.Input[str] kubernetes_version: The kubernetes version of the Cluster v2 (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster V2 (map)
         :param pulumi.Input[pulumi.InputType['ClusterV2LocalAuthEndpointArgs']] local_auth_endpoint: Cluster V2 local auth endpoint (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Cluster v2 (string)
         :param pulumi.Input[pulumi.InputType['ClusterV2RkeConfigArgs']] rke_config: The RKE configuration for `k3s` and `rke2` Clusters v2. (list maxitems:1)
         """
@@ -585,17 +687,20 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  agent_env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2AgentEnvVarArgs']]]]] = None,
                  annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  cloud_credential_secret_name: Optional[pulumi.Input[str]] = None,
+                 cluster_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]]] = None,
                  default_cluster_role_for_project_members: Optional[pulumi.Input[str]] = None,
+                 default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[str]] = None,
                  default_pod_security_policy_template_name: Optional[pulumi.Input[str]] = None,
                  enable_network_policy: Optional[pulumi.Input[bool]] = None,
+                 fleet_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2FleetAgentDeploymentCustomizationArgs']]]]] = None,
                  fleet_namespace: Optional[pulumi.Input[str]] = None,
                  kubernetes_version: Optional[pulumi.Input[str]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  local_auth_endpoint: Optional[pulumi.Input[pulumi.InputType['ClusterV2LocalAuthEndpointArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  rke_config: Optional[pulumi.Input[pulumi.InputType['ClusterV2RkeConfigArgs']]] = None,
                  __props__=None):
@@ -606,17 +711,20 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ClusterV2Args.__new__(ClusterV2Args)
 
             __props__.__dict__["agent_env_vars"] = agent_env_vars
             __props__.__dict__["annotations"] = annotations
             __props__.__dict__["cloud_credential_secret_name"] = cloud_credential_secret_name
+            __props__.__dict__["cluster_agent_deployment_customizations"] = cluster_agent_deployment_customizations
             __props__.__dict__["default_cluster_role_for_project_members"] = default_cluster_role_for_project_members
+            __props__.__dict__["default_pod_security_admission_configuration_template_name"] = default_pod_security_admission_configuration_template_name
             __props__.__dict__["default_pod_security_policy_template_name"] = default_pod_security_policy_template_name
             __props__.__dict__["enable_network_policy"] = enable_network_policy
+            __props__.__dict__["fleet_agent_deployment_customizations"] = fleet_agent_deployment_customizations
             __props__.__dict__["fleet_namespace"] = fleet_namespace
             if kubernetes_version is None and not opts.urn:
                 raise TypeError("Missing required property 'kubernetes_version'")
             __props__.__dict__["kubernetes_version"] = kubernetes_version
             __props__.__dict__["labels"] = labels
             __props__.__dict__["local_auth_endpoint"] = local_auth_endpoint
             __props__.__dict__["name"] = name
@@ -636,19 +744,22 @@
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             agent_env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2AgentEnvVarArgs']]]]] = None,
             annotations: Optional[pulumi.Input[Mapping[str, Any]]] = None,
             cloud_credential_secret_name: Optional[pulumi.Input[str]] = None,
+            cluster_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]]] = None,
             cluster_registration_token: Optional[pulumi.Input[pulumi.InputType['ClusterV2ClusterRegistrationTokenArgs']]] = None,
             cluster_v1_id: Optional[pulumi.Input[str]] = None,
             default_cluster_role_for_project_members: Optional[pulumi.Input[str]] = None,
+            default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[str]] = None,
             default_pod_security_policy_template_name: Optional[pulumi.Input[str]] = None,
             enable_network_policy: Optional[pulumi.Input[bool]] = None,
+            fleet_agent_deployment_customizations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2FleetAgentDeploymentCustomizationArgs']]]]] = None,
             fleet_namespace: Optional[pulumi.Input[str]] = None,
             kube_config: Optional[pulumi.Input[str]] = None,
             kubernetes_version: Optional[pulumi.Input[str]] = None,
             labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
             local_auth_endpoint: Optional[pulumi.Input[pulumi.InputType['ClusterV2LocalAuthEndpointArgs']]] = None,
             name: Optional[pulumi.Input[str]] = None,
             resource_version: Optional[pulumi.Input[str]] = None,
@@ -659,19 +770,22 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2AgentEnvVarArgs']]]] agent_env_vars: Optional Agent Env Vars for Rancher agent (list)
         :param pulumi.Input[Mapping[str, Any]] annotations: Annotations for the Cluster V2 (map)
         :param pulumi.Input[str] cloud_credential_secret_name: Cluster V2 cloud credential secret name (string)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2ClusterAgentDeploymentCustomizationArgs']]]] cluster_agent_deployment_customizations: Optional customization for cluster agent
         :param pulumi.Input[pulumi.InputType['ClusterV2ClusterRegistrationTokenArgs']] cluster_registration_token: (Computed/Sensitive) Cluster Registration Token generated for the cluster v2 (list maxitems:1)
         :param pulumi.Input[str] cluster_v1_id: (Computed) Cluster v1 id for cluster v2. (e.g to be used with `rancher2_sync`) (string)
         :param pulumi.Input[str] default_cluster_role_for_project_members: Cluster V2 default cluster role for project members (string)
+        :param pulumi.Input[str] default_pod_security_admission_configuration_template_name: Cluster V2 default pod security admission configuration template name (string)
         :param pulumi.Input[str] default_pod_security_policy_template_name: Cluster V2 default pod security policy template name (string)
         :param pulumi.Input[bool] enable_network_policy: Enable k8s network policy at Cluster V2 (bool)
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterV2FleetAgentDeploymentCustomizationArgs']]]] fleet_agent_deployment_customizations: Optional customization for fleet agent
         :param pulumi.Input[str] fleet_namespace: The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
         :param pulumi.Input[str] kube_config: (Computed/Sensitive) Kube Config generated for the cluster v2. Note: When the cluster has `local_auth_endpoint` enabled, the kube_config will not be available until the cluster is `connected` (string)
         :param pulumi.Input[str] kubernetes_version: The kubernetes version of the Cluster v2 (list maxitems:1)
         :param pulumi.Input[Mapping[str, Any]] labels: Labels for the Cluster V2 (map)
         :param pulumi.Input[pulumi.InputType['ClusterV2LocalAuthEndpointArgs']] local_auth_endpoint: Cluster V2 local auth endpoint (list maxitems:1)
         :param pulumi.Input[str] name: The name of the Cluster v2 (string)
         :param pulumi.Input[str] resource_version: (Computed) Cluster v2 k8s resource version (string)
@@ -680,19 +794,22 @@
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ClusterV2State.__new__(_ClusterV2State)
 
         __props__.__dict__["agent_env_vars"] = agent_env_vars
         __props__.__dict__["annotations"] = annotations
         __props__.__dict__["cloud_credential_secret_name"] = cloud_credential_secret_name
+        __props__.__dict__["cluster_agent_deployment_customizations"] = cluster_agent_deployment_customizations
         __props__.__dict__["cluster_registration_token"] = cluster_registration_token
         __props__.__dict__["cluster_v1_id"] = cluster_v1_id
         __props__.__dict__["default_cluster_role_for_project_members"] = default_cluster_role_for_project_members
+        __props__.__dict__["default_pod_security_admission_configuration_template_name"] = default_pod_security_admission_configuration_template_name
         __props__.__dict__["default_pod_security_policy_template_name"] = default_pod_security_policy_template_name
         __props__.__dict__["enable_network_policy"] = enable_network_policy
+        __props__.__dict__["fleet_agent_deployment_customizations"] = fleet_agent_deployment_customizations
         __props__.__dict__["fleet_namespace"] = fleet_namespace
         __props__.__dict__["kube_config"] = kube_config
         __props__.__dict__["kubernetes_version"] = kubernetes_version
         __props__.__dict__["labels"] = labels
         __props__.__dict__["local_auth_endpoint"] = local_auth_endpoint
         __props__.__dict__["name"] = name
         __props__.__dict__["resource_version"] = resource_version
@@ -720,14 +837,22 @@
     def cloud_credential_secret_name(self) -> pulumi.Output[Optional[str]]:
         """
         Cluster V2 cloud credential secret name (string)
         """
         return pulumi.get(self, "cloud_credential_secret_name")
 
     @property
+    @pulumi.getter(name="clusterAgentDeploymentCustomizations")
+    def cluster_agent_deployment_customizations(self) -> pulumi.Output[Optional[Sequence['outputs.ClusterV2ClusterAgentDeploymentCustomization']]]:
+        """
+        Optional customization for cluster agent
+        """
+        return pulumi.get(self, "cluster_agent_deployment_customizations")
+
+    @property
     @pulumi.getter(name="clusterRegistrationToken")
     def cluster_registration_token(self) -> pulumi.Output['outputs.ClusterV2ClusterRegistrationToken']:
         """
         (Computed/Sensitive) Cluster Registration Token generated for the cluster v2 (list maxitems:1)
         """
         return pulumi.get(self, "cluster_registration_token")
 
@@ -744,14 +869,22 @@
     def default_cluster_role_for_project_members(self) -> pulumi.Output[Optional[str]]:
         """
         Cluster V2 default cluster role for project members (string)
         """
         return pulumi.get(self, "default_cluster_role_for_project_members")
 
     @property
+    @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
+    def default_pod_security_admission_configuration_template_name(self) -> pulumi.Output[Optional[str]]:
+        """
+        Cluster V2 default pod security admission configuration template name (string)
+        """
+        return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
+
+    @property
     @pulumi.getter(name="defaultPodSecurityPolicyTemplateName")
     def default_pod_security_policy_template_name(self) -> pulumi.Output[Optional[str]]:
         """
         Cluster V2 default pod security policy template name (string)
         """
         return pulumi.get(self, "default_pod_security_policy_template_name")
 
@@ -760,14 +893,22 @@
     def enable_network_policy(self) -> pulumi.Output[bool]:
         """
         Enable k8s network policy at Cluster V2 (bool)
         """
         return pulumi.get(self, "enable_network_policy")
 
     @property
+    @pulumi.getter(name="fleetAgentDeploymentCustomizations")
+    def fleet_agent_deployment_customizations(self) -> pulumi.Output[Optional[Sequence['outputs.ClusterV2FleetAgentDeploymentCustomization']]]:
+        """
+        Optional customization for fleet agent
+        """
+        return pulumi.get(self, "fleet_agent_deployment_customizations")
+
+    @property
     @pulumi.getter(name="fleetNamespace")
     def fleet_namespace(self) -> pulumi.Output[Optional[str]]:
         """
         The fleet namespace of the Cluster v2. Default: `\\"fleet-default\\"` (string)
         """
         return pulumi.get(self, "fleet_namespace")
```

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/config/vars.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/config_map_v2.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/etcd_backup.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/feature.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/feature.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_app.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_catalog.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_catalog_v2.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_catalog_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_certificate.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cloud_credential.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cloud_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetClusterResult:
     """
     A collection of values returned by getCluster.
     """
-    def __init__(__self__, agent_env_vars=None, aks_config=None, aks_config_v2=None, annotations=None, ca_cert=None, cluster_auth_endpoint=None, cluster_monitoring_input=None, cluster_registration_token=None, cluster_template_answers=None, cluster_template_id=None, cluster_template_questions=None, cluster_template_revision_id=None, default_pod_security_policy_template_id=None, default_project_id=None, description=None, driver=None, eks_config=None, eks_config_v2=None, enable_cluster_alerting=None, enable_cluster_monitoring=None, enable_network_policy=None, fleet_workspace_name=None, gke_config=None, gke_config_v2=None, id=None, k3s_config=None, kube_config=None, labels=None, name=None, oke_config=None, rke2_config=None, rke_config=None, system_project_id=None):
+    def __init__(__self__, agent_env_vars=None, aks_config=None, aks_config_v2=None, annotations=None, ca_cert=None, cluster_auth_endpoint=None, cluster_monitoring_input=None, cluster_registration_token=None, cluster_template_answers=None, cluster_template_id=None, cluster_template_questions=None, cluster_template_revision_id=None, default_pod_security_admission_configuration_template_name=None, default_pod_security_policy_template_id=None, default_project_id=None, description=None, driver=None, eks_config=None, eks_config_v2=None, enable_cluster_alerting=None, enable_cluster_monitoring=None, enable_network_policy=None, fleet_workspace_name=None, gke_config=None, gke_config_v2=None, id=None, k3s_config=None, kube_config=None, labels=None, name=None, oke_config=None, rke2_config=None, rke_config=None, system_project_id=None):
         if agent_env_vars and not isinstance(agent_env_vars, list):
             raise TypeError("Expected argument 'agent_env_vars' to be a list")
         pulumi.set(__self__, "agent_env_vars", agent_env_vars)
         if aks_config and not isinstance(aks_config, dict):
             raise TypeError("Expected argument 'aks_config' to be a dict")
         pulumi.set(__self__, "aks_config", aks_config)
         if aks_config_v2 and not isinstance(aks_config_v2, dict):
@@ -55,14 +55,17 @@
         pulumi.set(__self__, "cluster_template_id", cluster_template_id)
         if cluster_template_questions and not isinstance(cluster_template_questions, list):
             raise TypeError("Expected argument 'cluster_template_questions' to be a list")
         pulumi.set(__self__, "cluster_template_questions", cluster_template_questions)
         if cluster_template_revision_id and not isinstance(cluster_template_revision_id, str):
             raise TypeError("Expected argument 'cluster_template_revision_id' to be a str")
         pulumi.set(__self__, "cluster_template_revision_id", cluster_template_revision_id)
+        if default_pod_security_admission_configuration_template_name and not isinstance(default_pod_security_admission_configuration_template_name, str):
+            raise TypeError("Expected argument 'default_pod_security_admission_configuration_template_name' to be a str")
+        pulumi.set(__self__, "default_pod_security_admission_configuration_template_name", default_pod_security_admission_configuration_template_name)
         if default_pod_security_policy_template_id and not isinstance(default_pod_security_policy_template_id, str):
             raise TypeError("Expected argument 'default_pod_security_policy_template_id' to be a str")
         pulumi.set(__self__, "default_pod_security_policy_template_id", default_pod_security_policy_template_id)
         if default_project_id and not isinstance(default_project_id, str):
             raise TypeError("Expected argument 'default_project_id' to be a str")
         pulumi.set(__self__, "default_project_id", default_project_id)
         if description and not isinstance(description, str):
@@ -216,14 +219,19 @@
     def cluster_template_revision_id(self) -> str:
         """
         (Computed) Cluster template revision ID (string)
         """
         return pulumi.get(self, "cluster_template_revision_id")
 
     @property
+    @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
+    def default_pod_security_admission_configuration_template_name(self) -> str:
+        return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
+
+    @property
     @pulumi.getter(name="defaultPodSecurityPolicyTemplateId")
     def default_pod_security_policy_template_id(self) -> str:
         """
         (Optional/Computed) [Default pod security policy template id](https://rancher.com/docs/rancher/v2.x/en/cluster-provisioning/rke-clusters/options/#pod-security-policy-support) (string)
         """
         return pulumi.get(self, "default_pod_security_policy_template_id")
 
@@ -396,14 +404,15 @@
             cluster_auth_endpoint=self.cluster_auth_endpoint,
             cluster_monitoring_input=self.cluster_monitoring_input,
             cluster_registration_token=self.cluster_registration_token,
             cluster_template_answers=self.cluster_template_answers,
             cluster_template_id=self.cluster_template_id,
             cluster_template_questions=self.cluster_template_questions,
             cluster_template_revision_id=self.cluster_template_revision_id,
+            default_pod_security_admission_configuration_template_name=self.default_pod_security_admission_configuration_template_name,
             default_pod_security_policy_template_id=self.default_pod_security_policy_template_id,
             default_project_id=self.default_project_id,
             description=self.description,
             driver=self.driver,
             eks_config=self.eks_config,
             eks_config_v2=self.eks_config_v2,
             enable_cluster_alerting=self.enable_cluster_alerting,
@@ -419,15 +428,16 @@
             name=self.name,
             oke_config=self.oke_config,
             rke2_config=self.rke2_config,
             rke_config=self.rke_config,
             system_project_id=self.system_project_id)
 
 
-def get_cluster(name: Optional[str] = None,
+def get_cluster(default_pod_security_admission_configuration_template_name: Optional[str] = None,
+                name: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetClusterResult:
     """
     Use this data source to retrieve information about a Rancher v2 cluster.
 
     ## Example Usage
 
     ```python
@@ -437,14 +447,15 @@
     foo_custom = rancher2.get_cluster(name="foo-custom")
     ```
 
 
     :param str name: The name of the Cluster (string)
     """
     __args__ = dict()
+    __args__['defaultPodSecurityAdmissionConfigurationTemplateName'] = default_pod_security_admission_configuration_template_name
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('rancher2:index/getCluster:getCluster', __args__, opts=opts, typ=GetClusterResult).value
 
     return AwaitableGetClusterResult(
         agent_env_vars=__ret__.agent_env_vars,
         aks_config=__ret__.aks_config,
@@ -454,14 +465,15 @@
         cluster_auth_endpoint=__ret__.cluster_auth_endpoint,
         cluster_monitoring_input=__ret__.cluster_monitoring_input,
         cluster_registration_token=__ret__.cluster_registration_token,
         cluster_template_answers=__ret__.cluster_template_answers,
         cluster_template_id=__ret__.cluster_template_id,
         cluster_template_questions=__ret__.cluster_template_questions,
         cluster_template_revision_id=__ret__.cluster_template_revision_id,
+        default_pod_security_admission_configuration_template_name=__ret__.default_pod_security_admission_configuration_template_name,
         default_pod_security_policy_template_id=__ret__.default_pod_security_policy_template_id,
         default_project_id=__ret__.default_project_id,
         description=__ret__.description,
         driver=__ret__.driver,
         eks_config=__ret__.eks_config,
         eks_config_v2=__ret__.eks_config_v2,
         enable_cluster_alerting=__ret__.enable_cluster_alerting,
@@ -478,15 +490,16 @@
         oke_config=__ret__.oke_config,
         rke2_config=__ret__.rke2_config,
         rke_config=__ret__.rke_config,
         system_project_id=__ret__.system_project_id)
 
 
 @_utilities.lift_output_func(get_cluster)
-def get_cluster_output(name: Optional[pulumi.Input[str]] = None,
+def get_cluster_output(default_pod_security_admission_configuration_template_name: Optional[pulumi.Input[Optional[str]]] = None,
+                       name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClusterResult]:
     """
     Use this data source to retrieve information about a Rancher v2 cluster.
 
     ## Example Usage
 
     ```python
```

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster_alert_group.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster_alter_rule.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster_alter_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster_driver.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster_role_template_binding.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster_template.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_cluster_v2.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_cluster_v2.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetClusterV2Result:
     """
     A collection of values returned by getClusterV2.
     """
-    def __init__(__self__, agent_env_vars=None, annotations=None, cloud_credential_secret_name=None, cluster_registration_token=None, cluster_v1_id=None, default_cluster_role_for_project_members=None, default_pod_security_policy_template_name=None, enable_network_policy=None, fleet_namespace=None, id=None, kube_config=None, kubernetes_version=None, labels=None, name=None, resource_version=None, rke_config=None):
+    def __init__(__self__, agent_env_vars=None, annotations=None, cloud_credential_secret_name=None, cluster_registration_token=None, cluster_v1_id=None, default_cluster_role_for_project_members=None, default_pod_security_admission_configuration_template_name=None, default_pod_security_policy_template_name=None, enable_network_policy=None, fleet_namespace=None, id=None, kube_config=None, kubernetes_version=None, labels=None, name=None, resource_version=None, rke_config=None):
         if agent_env_vars and not isinstance(agent_env_vars, list):
             raise TypeError("Expected argument 'agent_env_vars' to be a list")
         pulumi.set(__self__, "agent_env_vars", agent_env_vars)
         if annotations and not isinstance(annotations, dict):
             raise TypeError("Expected argument 'annotations' to be a dict")
         pulumi.set(__self__, "annotations", annotations)
         if cloud_credential_secret_name and not isinstance(cloud_credential_secret_name, str):
@@ -37,14 +37,17 @@
         pulumi.set(__self__, "cluster_registration_token", cluster_registration_token)
         if cluster_v1_id and not isinstance(cluster_v1_id, str):
             raise TypeError("Expected argument 'cluster_v1_id' to be a str")
         pulumi.set(__self__, "cluster_v1_id", cluster_v1_id)
         if default_cluster_role_for_project_members and not isinstance(default_cluster_role_for_project_members, str):
             raise TypeError("Expected argument 'default_cluster_role_for_project_members' to be a str")
         pulumi.set(__self__, "default_cluster_role_for_project_members", default_cluster_role_for_project_members)
+        if default_pod_security_admission_configuration_template_name and not isinstance(default_pod_security_admission_configuration_template_name, str):
+            raise TypeError("Expected argument 'default_pod_security_admission_configuration_template_name' to be a str")
+        pulumi.set(__self__, "default_pod_security_admission_configuration_template_name", default_pod_security_admission_configuration_template_name)
         if default_pod_security_policy_template_name and not isinstance(default_pod_security_policy_template_name, str):
             raise TypeError("Expected argument 'default_pod_security_policy_template_name' to be a str")
         pulumi.set(__self__, "default_pod_security_policy_template_name", default_pod_security_policy_template_name)
         if enable_network_policy and not isinstance(enable_network_policy, bool):
             raise TypeError("Expected argument 'enable_network_policy' to be a bool")
         pulumi.set(__self__, "enable_network_policy", enable_network_policy)
         if fleet_namespace and not isinstance(fleet_namespace, str):
@@ -114,14 +117,22 @@
     def default_cluster_role_for_project_members(self) -> str:
         """
         (Computed) Cluster V2 default cluster role for project members (string)
         """
         return pulumi.get(self, "default_cluster_role_for_project_members")
 
     @property
+    @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
+    def default_pod_security_admission_configuration_template_name(self) -> str:
+        """
+        (Computed) Cluster V2 default pod security admission configuration template name (string)
+        """
+        return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
+
+    @property
     @pulumi.getter(name="defaultPodSecurityPolicyTemplateName")
     def default_pod_security_policy_template_name(self) -> str:
         """
         (Computed) Cluster V2 default pod security policy template name (string)
         """
         return pulumi.get(self, "default_pod_security_policy_template_name")
 
@@ -197,14 +208,15 @@
         return GetClusterV2Result(
             agent_env_vars=self.agent_env_vars,
             annotations=self.annotations,
             cloud_credential_secret_name=self.cloud_credential_secret_name,
             cluster_registration_token=self.cluster_registration_token,
             cluster_v1_id=self.cluster_v1_id,
             default_cluster_role_for_project_members=self.default_cluster_role_for_project_members,
+            default_pod_security_admission_configuration_template_name=self.default_pod_security_admission_configuration_template_name,
             default_pod_security_policy_template_name=self.default_pod_security_policy_template_name,
             enable_network_policy=self.enable_network_policy,
             fleet_namespace=self.fleet_namespace,
             id=self.id,
             kube_config=self.kube_config,
             kubernetes_version=self.kubernetes_version,
             labels=self.labels,
@@ -242,14 +254,15 @@
     return AwaitableGetClusterV2Result(
         agent_env_vars=__ret__.agent_env_vars,
         annotations=__ret__.annotations,
         cloud_credential_secret_name=__ret__.cloud_credential_secret_name,
         cluster_registration_token=__ret__.cluster_registration_token,
         cluster_v1_id=__ret__.cluster_v1_id,
         default_cluster_role_for_project_members=__ret__.default_cluster_role_for_project_members,
+        default_pod_security_admission_configuration_template_name=__ret__.default_pod_security_admission_configuration_template_name,
         default_pod_security_policy_template_name=__ret__.default_pod_security_policy_template_name,
         enable_network_policy=__ret__.enable_network_policy,
         fleet_namespace=__ret__.fleet_namespace,
         id=__ret__.id,
         kube_config=__ret__.kube_config,
         kubernetes_version=__ret__.kubernetes_version,
         labels=__ret__.labels,
```

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_config_map_v2.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_config_map_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_etcd_backup.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_etcd_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_global_dns_provider.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_global_role.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_global_role_binding.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_global_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_multi_cluster_app.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_namespace.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_node_driver.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_node_pool.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_node_template.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_notifier.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_pod_security_policy_template.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_principal.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_principal.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_project.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_project_alert_group.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_project_alert_rule.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_project_role_template_binding.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_registry.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_role_tempalte.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_role_tempalte.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_role_template.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_secret.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_secret_v2.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_setting.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_storage_class_v2.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/get_user.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/global_dns.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/global_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/global_dns_provider.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/global_dns_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/global_role.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/global_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/global_role_binding.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/global_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/machine_config_v2.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/machine_config_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/multi_cluster_app.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/multi_cluster_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/namespace.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/node_driver.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/node_driver.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/node_pool.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/node_template.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/notifier.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/notifier.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/outputs.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,23 +30,29 @@
     'ClusterAlertRuleNodeRule',
     'ClusterAlertRuleSystemServiceRule',
     'ClusterAlterGroupRecipient',
     'ClusterAlterRuleEventRule',
     'ClusterAlterRuleMetricRule',
     'ClusterAlterRuleNodeRule',
     'ClusterAlterRuleSystemServiceRule',
+    'ClusterClusterAgentDeploymentCustomization',
+    'ClusterClusterAgentDeploymentCustomizationAppendToleration',
+    'ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirement',
     'ClusterClusterAuthEndpoint',
     'ClusterClusterMonitoringInput',
     'ClusterClusterRegistrationToken',
     'ClusterClusterTemplateAnswers',
     'ClusterClusterTemplateQuestion',
     'ClusterEksConfig',
     'ClusterEksConfigV2',
     'ClusterEksConfigV2NodeGroup',
     'ClusterEksConfigV2NodeGroupLaunchTemplate',
+    'ClusterFleetAgentDeploymentCustomization',
+    'ClusterFleetAgentDeploymentCustomizationAppendToleration',
+    'ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirement',
     'ClusterGkeConfig',
     'ClusterGkeConfigV2',
     'ClusterGkeConfigV2ClusterAddons',
     'ClusterGkeConfigV2IpAllocationPolicy',
     'ClusterGkeConfigV2MasterAuthorizedNetworksConfig',
     'ClusterGkeConfigV2MasterAuthorizedNetworksConfigCidrBlock',
     'ClusterGkeConfigV2NodePool',
@@ -106,14 +112,16 @@
     'ClusterRkeConfigPrivateRegistry',
     'ClusterRkeConfigPrivateRegistryEcrCredentialPlugin',
     'ClusterRkeConfigServices',
     'ClusterRkeConfigServicesEtcd',
     'ClusterRkeConfigServicesEtcdBackupConfig',
     'ClusterRkeConfigServicesEtcdBackupConfigS3BackupConfig',
     'ClusterRkeConfigServicesKubeApi',
+    'ClusterRkeConfigServicesKubeApiAdmissionConfiguration',
+    'ClusterRkeConfigServicesKubeApiAdmissionConfigurationPlugin',
     'ClusterRkeConfigServicesKubeApiAuditLog',
     'ClusterRkeConfigServicesKubeApiAuditLogConfiguration',
     'ClusterRkeConfigServicesKubeApiEventRateLimit',
     'ClusterRkeConfigServicesKubeApiSecretsEncryptionConfig',
     'ClusterRkeConfigServicesKubeController',
     'ClusterRkeConfigServicesKubelet',
     'ClusterRkeConfigServicesKubeproxy',
@@ -171,35 +179,44 @@
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigPrivateRegistry',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigPrivateRegistryEcrCredentialPlugin',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServices',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcd',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcdBackupConfig',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcdBackupConfigS3BackupConfig',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApi',
+    'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfiguration',
+    'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPlugin',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLog',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLogConfiguration',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiEventRateLimit',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiSecretsEncryptionConfig',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeController',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubelet',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeproxy',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesScheduler',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigUpgradeStrategy',
     'ClusterTemplateTemplateRevisionClusterConfigRkeConfigUpgradeStrategyDrainInput',
     'ClusterTemplateTemplateRevisionQuestion',
     'ClusterV2AgentEnvVar',
+    'ClusterV2ClusterAgentDeploymentCustomization',
+    'ClusterV2ClusterAgentDeploymentCustomizationAppendToleration',
+    'ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirement',
     'ClusterV2ClusterRegistrationToken',
+    'ClusterV2FleetAgentDeploymentCustomization',
+    'ClusterV2FleetAgentDeploymentCustomizationAppendToleration',
+    'ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirement',
     'ClusterV2LocalAuthEndpoint',
     'ClusterV2RkeConfig',
     'ClusterV2RkeConfigEtcd',
     'ClusterV2RkeConfigEtcdS3Config',
     'ClusterV2RkeConfigEtcdSnapshotCreate',
     'ClusterV2RkeConfigEtcdSnapshotRestore',
     'ClusterV2RkeConfigLocalAuthEndpoint',
     'ClusterV2RkeConfigMachinePool',
+    'ClusterV2RkeConfigMachinePoolDefault',
     'ClusterV2RkeConfigMachinePoolMachineConfig',
     'ClusterV2RkeConfigMachinePoolRollingUpdate',
     'ClusterV2RkeConfigMachinePoolTaint',
     'ClusterV2RkeConfigMachineSelectorConfig',
     'ClusterV2RkeConfigMachineSelectorConfigMachineLabelSelector',
     'ClusterV2RkeConfigMachineSelectorConfigMachineLabelSelectorMatchExpression',
     'ClusterV2RkeConfigRegistries',
@@ -356,14 +373,16 @@
     'GetClusterRkeConfigPrivateRegistryResult',
     'GetClusterRkeConfigPrivateRegistryEcrCredentialPluginResult',
     'GetClusterRkeConfigServicesResult',
     'GetClusterRkeConfigServicesEtcdResult',
     'GetClusterRkeConfigServicesEtcdBackupConfigResult',
     'GetClusterRkeConfigServicesEtcdBackupConfigS3BackupConfigResult',
     'GetClusterRkeConfigServicesKubeApiResult',
+    'GetClusterRkeConfigServicesKubeApiAdmissionConfigurationResult',
+    'GetClusterRkeConfigServicesKubeApiAdmissionConfigurationPluginResult',
     'GetClusterRkeConfigServicesKubeApiAuditLogResult',
     'GetClusterRkeConfigServicesKubeApiAuditLogConfigurationResult',
     'GetClusterRkeConfigServicesKubeApiEventRateLimitResult',
     'GetClusterRkeConfigServicesKubeApiSecretsEncryptionConfigResult',
     'GetClusterRkeConfigServicesKubeControllerResult',
     'GetClusterRkeConfigServicesKubeletResult',
     'GetClusterRkeConfigServicesKubeproxyResult',
@@ -420,14 +439,16 @@
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigPrivateRegistryResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigPrivateRegistryEcrCredentialPluginResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcdResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcdBackupConfigResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesEtcdBackupConfigS3BackupConfigResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiResult',
+    'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationResult',
+    'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPluginResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLogResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLogConfigurationResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiEventRateLimitResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiSecretsEncryptionConfigResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeControllerResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeletResult',
     'GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeproxyResult',
@@ -440,14 +461,15 @@
     'GetClusterV2RkeConfigResult',
     'GetClusterV2RkeConfigEtcdResult',
     'GetClusterV2RkeConfigEtcdS3ConfigResult',
     'GetClusterV2RkeConfigEtcdSnapshotCreateResult',
     'GetClusterV2RkeConfigEtcdSnapshotRestoreResult',
     'GetClusterV2RkeConfigLocalAuthEndpointResult',
     'GetClusterV2RkeConfigMachinePoolResult',
+    'GetClusterV2RkeConfigMachinePoolDefaultResult',
     'GetClusterV2RkeConfigMachinePoolMachineConfigResult',
     'GetClusterV2RkeConfigMachinePoolRollingUpdateResult',
     'GetClusterV2RkeConfigMachinePoolTaintResult',
     'GetClusterV2RkeConfigMachineSelectorConfigResult',
     'GetClusterV2RkeConfigMachineSelectorConfigMachineLabelSelectorResult',
     'GetClusterV2RkeConfigMachineSelectorConfigMachineLabelSelectorMatchExpressionResult',
     'GetClusterV2RkeConfigRegistriesResult',
@@ -2029,14 +2051,16 @@
             suggest = "availability_zones"
         elif key == "enableAutoScaling":
             suggest = "enable_auto_scaling"
         elif key == "maxCount":
             suggest = "max_count"
         elif key == "maxPods":
             suggest = "max_pods"
+        elif key == "maxSurge":
+            suggest = "max_surge"
         elif key == "minCount":
             suggest = "min_count"
         elif key == "orchestratorVersion":
             suggest = "orchestrator_version"
         elif key == "osDiskSizeGb":
             suggest = "os_disk_size_gb"
         elif key == "osDiskType":
@@ -2058,61 +2082,73 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  name: str,
                  availability_zones: Optional[Sequence[str]] = None,
                  count: Optional[int] = None,
                  enable_auto_scaling: Optional[bool] = None,
+                 labels: Optional[Mapping[str, Any]] = None,
                  max_count: Optional[int] = None,
                  max_pods: Optional[int] = None,
+                 max_surge: Optional[str] = None,
                  min_count: Optional[int] = None,
                  mode: Optional[str] = None,
                  orchestrator_version: Optional[str] = None,
                  os_disk_size_gb: Optional[int] = None,
                  os_disk_type: Optional[str] = None,
                  os_type: Optional[str] = None,
+                 taints: Optional[Sequence[str]] = None,
                  vm_size: Optional[str] = None):
         """
         :param str name: The name of the Cluster (string)
         :param Sequence[str] availability_zones: The AKS node pool availability zones (list)
         :param int count: Number of machines (VMs) in the agent pool. Allowed values must be in the range of 1 to 100 (inclusive). Default `1` (int)
         :param bool enable_auto_scaling: Is AKS node pool auto scaling enabled? Default: `false` (bool)
+        :param Mapping[str, Any] labels: Labels for the Cluster (map)
         :param int max_count: The AKS node pool max count. Required if `enable_auto_scaling=true` (int)
         :param int max_pods: Maximum number of pods that can run on a node. Default `110` (int)
+        :param str max_surge: Monitoring deployment rolling update max surge. Default: `1` (int)
         :param int min_count: The AKS node pool min count. Required if `enable_auto_scaling=true` (int)
         :param str mode: RKE mode for authorization. `rbac` and `none` modes are available. Default `rbac` (string)
         :param str orchestrator_version: The AKS node pool orchestrator version (string)
         :param int os_disk_size_gb: The AKS node pool os disk size gb. Default: `128` (int)
         :param str os_disk_type: The AKS node pool os disk type. Default: `Managed` (string)
         :param str os_type: The AKS node pool os type. Default: `Linux` (string)
+        :param Sequence[str] taints: The AKS node pool taints (list)
         :param str vm_size: The AKS node pool orchestrator version (string)
         """
         pulumi.set(__self__, "name", name)
         if availability_zones is not None:
             pulumi.set(__self__, "availability_zones", availability_zones)
         if count is not None:
             pulumi.set(__self__, "count", count)
         if enable_auto_scaling is not None:
             pulumi.set(__self__, "enable_auto_scaling", enable_auto_scaling)
+        if labels is not None:
+            pulumi.set(__self__, "labels", labels)
         if max_count is not None:
             pulumi.set(__self__, "max_count", max_count)
         if max_pods is not None:
             pulumi.set(__self__, "max_pods", max_pods)
+        if max_surge is not None:
+            pulumi.set(__self__, "max_surge", max_surge)
         if min_count is not None:
             pulumi.set(__self__, "min_count", min_count)
         if mode is not None:
             pulumi.set(__self__, "mode", mode)
         if orchestrator_version is not None:
             pulumi.set(__self__, "orchestrator_version", orchestrator_version)
         if os_disk_size_gb is not None:
             pulumi.set(__self__, "os_disk_size_gb", os_disk_size_gb)
         if os_disk_type is not None:
             pulumi.set(__self__, "os_disk_type", os_disk_type)
         if os_type is not None:
             pulumi.set(__self__, "os_type", os_type)
+        if taints is not None:
+            pulumi.set(__self__, "taints", taints)
         if vm_size is not None:
             pulumi.set(__self__, "vm_size", vm_size)
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
@@ -2141,14 +2177,22 @@
     def enable_auto_scaling(self) -> Optional[bool]:
         """
         Is AKS node pool auto scaling enabled? Default: `false` (bool)
         """
         return pulumi.get(self, "enable_auto_scaling")
 
     @property
+    @pulumi.getter
+    def labels(self) -> Optional[Mapping[str, Any]]:
+        """
+        Labels for the Cluster (map)
+        """
+        return pulumi.get(self, "labels")
+
+    @property
     @pulumi.getter(name="maxCount")
     def max_count(self) -> Optional[int]:
         """
         The AKS node pool max count. Required if `enable_auto_scaling=true` (int)
         """
         return pulumi.get(self, "max_count")
 
@@ -2157,14 +2201,22 @@
     def max_pods(self) -> Optional[int]:
         """
         Maximum number of pods that can run on a node. Default `110` (int)
         """
         return pulumi.get(self, "max_pods")
 
     @property
+    @pulumi.getter(name="maxSurge")
+    def max_surge(self) -> Optional[str]:
+        """
+        Monitoring deployment rolling update max surge. Default: `1` (int)
+        """
+        return pulumi.get(self, "max_surge")
+
+    @property
     @pulumi.getter(name="minCount")
     def min_count(self) -> Optional[int]:
         """
         The AKS node pool min count. Required if `enable_auto_scaling=true` (int)
         """
         return pulumi.get(self, "min_count")
 
@@ -2205,14 +2257,22 @@
     def os_type(self) -> Optional[str]:
         """
         The AKS node pool os type. Default: `Linux` (string)
         """
         return pulumi.get(self, "os_type")
 
     @property
+    @pulumi.getter
+    def taints(self) -> Optional[Sequence[str]]:
+        """
+        The AKS node pool taints (list)
+        """
+        return pulumi.get(self, "taints")
+
+    @property
     @pulumi.getter(name="vmSize")
     def vm_size(self) -> Optional[str]:
         """
         The AKS node pool orchestrator version (string)
         """
         return pulumi.get(self, "vm_size")
 
@@ -2784,14 +2844,190 @@
     @property
     @pulumi.getter
     def condition(self) -> Optional[str]:
         return pulumi.get(self, "condition")
 
 
 @pulumi.output_type
+class ClusterClusterAgentDeploymentCustomization(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "appendTolerations":
+            suggest = "append_tolerations"
+        elif key == "overrideAffinity":
+            suggest = "override_affinity"
+        elif key == "overrideResourceRequirements":
+            suggest = "override_resource_requirements"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterClusterAgentDeploymentCustomization. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterClusterAgentDeploymentCustomization.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterClusterAgentDeploymentCustomization.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 append_tolerations: Optional[Sequence['outputs.ClusterClusterAgentDeploymentCustomizationAppendToleration']] = None,
+                 override_affinity: Optional[str] = None,
+                 override_resource_requirements: Optional[Sequence['outputs.ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirement']] = None):
+        if append_tolerations is not None:
+            pulumi.set(__self__, "append_tolerations", append_tolerations)
+        if override_affinity is not None:
+            pulumi.set(__self__, "override_affinity", override_affinity)
+        if override_resource_requirements is not None:
+            pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
+
+    @property
+    @pulumi.getter(name="appendTolerations")
+    def append_tolerations(self) -> Optional[Sequence['outputs.ClusterClusterAgentDeploymentCustomizationAppendToleration']]:
+        return pulumi.get(self, "append_tolerations")
+
+    @property
+    @pulumi.getter(name="overrideAffinity")
+    def override_affinity(self) -> Optional[str]:
+        return pulumi.get(self, "override_affinity")
+
+    @property
+    @pulumi.getter(name="overrideResourceRequirements")
+    def override_resource_requirements(self) -> Optional[Sequence['outputs.ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirement']]:
+        return pulumi.get(self, "override_resource_requirements")
+
+
+@pulumi.output_type
+class ClusterClusterAgentDeploymentCustomizationAppendToleration(dict):
+    def __init__(__self__, *,
+                 key: str,
+                 effect: Optional[str] = None,
+                 operator: Optional[str] = None,
+                 seconds: Optional[int] = None,
+                 value: Optional[str] = None):
+        """
+        :param str key: The toleration key (string)
+        :param str effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        :param str operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        :param int seconds: The toleration seconds (int)
+        :param str value: Rancher agent env var value (string)
+        """
+        pulumi.set(__self__, "key", key)
+        if effect is not None:
+            pulumi.set(__self__, "effect", effect)
+        if operator is not None:
+            pulumi.set(__self__, "operator", operator)
+        if seconds is not None:
+            pulumi.set(__self__, "seconds", seconds)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> str:
+        """
+        The toleration key (string)
+        """
+        return pulumi.get(self, "key")
+
+    @property
+    @pulumi.getter
+    def effect(self) -> Optional[str]:
+        """
+        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        """
+        return pulumi.get(self, "effect")
+
+    @property
+    @pulumi.getter
+    def operator(self) -> Optional[str]:
+        """
+        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        """
+        return pulumi.get(self, "operator")
+
+    @property
+    @pulumi.getter
+    def seconds(self) -> Optional[int]:
+        """
+        The toleration seconds (int)
+        """
+        return pulumi.get(self, "seconds")
+
+    @property
+    @pulumi.getter
+    def value(self) -> Optional[str]:
+        """
+        Rancher agent env var value (string)
+        """
+        return pulumi.get(self, "value")
+
+
+@pulumi.output_type
+class ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirement(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "cpuLimit":
+            suggest = "cpu_limit"
+        elif key == "cpuRequest":
+            suggest = "cpu_request"
+        elif key == "memoryLimit":
+            suggest = "memory_limit"
+        elif key == "memoryRequest":
+            suggest = "memory_request"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirement. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirement.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterClusterAgentDeploymentCustomizationOverrideResourceRequirement.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 cpu_limit: Optional[str] = None,
+                 cpu_request: Optional[str] = None,
+                 memory_limit: Optional[str] = None,
+                 memory_request: Optional[str] = None):
+        if cpu_limit is not None:
+            pulumi.set(__self__, "cpu_limit", cpu_limit)
+        if cpu_request is not None:
+            pulumi.set(__self__, "cpu_request", cpu_request)
+        if memory_limit is not None:
+            pulumi.set(__self__, "memory_limit", memory_limit)
+        if memory_request is not None:
+            pulumi.set(__self__, "memory_request", memory_request)
+
+    @property
+    @pulumi.getter(name="cpuLimit")
+    def cpu_limit(self) -> Optional[str]:
+        return pulumi.get(self, "cpu_limit")
+
+    @property
+    @pulumi.getter(name="cpuRequest")
+    def cpu_request(self) -> Optional[str]:
+        return pulumi.get(self, "cpu_request")
+
+    @property
+    @pulumi.getter(name="memoryLimit")
+    def memory_limit(self) -> Optional[str]:
+        return pulumi.get(self, "memory_limit")
+
+    @property
+    @pulumi.getter(name="memoryRequest")
+    def memory_request(self) -> Optional[str]:
+        return pulumi.get(self, "memory_request")
+
+
+@pulumi.output_type
 class ClusterClusterAuthEndpoint(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "caCerts":
             suggest = "ca_certs"
 
@@ -4013,14 +4249,190 @@
         """
         RKE2 kubernetes version (string)
         """
         return pulumi.get(self, "version")
 
 
 @pulumi.output_type
+class ClusterFleetAgentDeploymentCustomization(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "appendTolerations":
+            suggest = "append_tolerations"
+        elif key == "overrideAffinity":
+            suggest = "override_affinity"
+        elif key == "overrideResourceRequirements":
+            suggest = "override_resource_requirements"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterFleetAgentDeploymentCustomization. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterFleetAgentDeploymentCustomization.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterFleetAgentDeploymentCustomization.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 append_tolerations: Optional[Sequence['outputs.ClusterFleetAgentDeploymentCustomizationAppendToleration']] = None,
+                 override_affinity: Optional[str] = None,
+                 override_resource_requirements: Optional[Sequence['outputs.ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirement']] = None):
+        if append_tolerations is not None:
+            pulumi.set(__self__, "append_tolerations", append_tolerations)
+        if override_affinity is not None:
+            pulumi.set(__self__, "override_affinity", override_affinity)
+        if override_resource_requirements is not None:
+            pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
+
+    @property
+    @pulumi.getter(name="appendTolerations")
+    def append_tolerations(self) -> Optional[Sequence['outputs.ClusterFleetAgentDeploymentCustomizationAppendToleration']]:
+        return pulumi.get(self, "append_tolerations")
+
+    @property
+    @pulumi.getter(name="overrideAffinity")
+    def override_affinity(self) -> Optional[str]:
+        return pulumi.get(self, "override_affinity")
+
+    @property
+    @pulumi.getter(name="overrideResourceRequirements")
+    def override_resource_requirements(self) -> Optional[Sequence['outputs.ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirement']]:
+        return pulumi.get(self, "override_resource_requirements")
+
+
+@pulumi.output_type
+class ClusterFleetAgentDeploymentCustomizationAppendToleration(dict):
+    def __init__(__self__, *,
+                 key: str,
+                 effect: Optional[str] = None,
+                 operator: Optional[str] = None,
+                 seconds: Optional[int] = None,
+                 value: Optional[str] = None):
+        """
+        :param str key: The toleration key (string)
+        :param str effect: The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        :param str operator: The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        :param int seconds: The toleration seconds (int)
+        :param str value: Rancher agent env var value (string)
+        """
+        pulumi.set(__self__, "key", key)
+        if effect is not None:
+            pulumi.set(__self__, "effect", effect)
+        if operator is not None:
+            pulumi.set(__self__, "operator", operator)
+        if seconds is not None:
+            pulumi.set(__self__, "seconds", seconds)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> str:
+        """
+        The toleration key (string)
+        """
+        return pulumi.get(self, "key")
+
+    @property
+    @pulumi.getter
+    def effect(self) -> Optional[str]:
+        """
+        The toleration effect. `NoExecute`, `NoSchedule`, and `PreferNoSchedule` are supported. Default: `NoExecute` (string)
+        """
+        return pulumi.get(self, "effect")
+
+    @property
+    @pulumi.getter
+    def operator(self) -> Optional[str]:
+        """
+        The toleration operator. `Equal`, and `Exists` are supported. Default: `Equal` (string)
+        """
+        return pulumi.get(self, "operator")
+
+    @property
+    @pulumi.getter
+    def seconds(self) -> Optional[int]:
+        """
+        The toleration seconds (int)
+        """
+        return pulumi.get(self, "seconds")
+
+    @property
+    @pulumi.getter
+    def value(self) -> Optional[str]:
+        """
+        Rancher agent env var value (string)
+        """
+        return pulumi.get(self, "value")
+
+
+@pulumi.output_type
+class ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirement(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "cpuLimit":
+            suggest = "cpu_limit"
+        elif key == "cpuRequest":
+            suggest = "cpu_request"
+        elif key == "memoryLimit":
+            suggest = "memory_limit"
+        elif key == "memoryRequest":
+            suggest = "memory_request"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirement. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirement.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterFleetAgentDeploymentCustomizationOverrideResourceRequirement.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 cpu_limit: Optional[str] = None,
+                 cpu_request: Optional[str] = None,
+                 memory_limit: Optional[str] = None,
+                 memory_request: Optional[str] = None):
+        if cpu_limit is not None:
+            pulumi.set(__self__, "cpu_limit", cpu_limit)
+        if cpu_request is not None:
+            pulumi.set(__self__, "cpu_request", cpu_request)
+        if memory_limit is not None:
+            pulumi.set(__self__, "memory_limit", memory_limit)
+        if memory_request is not None:
+            pulumi.set(__self__, "memory_request", memory_request)
+
+    @property
+    @pulumi.getter(name="cpuLimit")
+    def cpu_limit(self) -> Optional[str]:
+        return pulumi.get(self, "cpu_limit")
+
+    @property
+    @pulumi.getter(name="cpuRequest")
+    def cpu_request(self) -> Optional[str]:
+        return pulumi.get(self, "cpu_request")
+
+    @property
+    @pulumi.getter(name="memoryLimit")
+    def memory_limit(self) -> Optional[str]:
+        return pulumi.get(self, "memory_limit")
+
+    @property
+    @pulumi.getter(name="memoryRequest")
+    def memory_request(self) -> Optional[str]:
+        return pulumi.get(self, "memory_request")
+
+
+@pulumi.output_type
 class ClusterGkeConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "clusterIpv4Cidr":
             suggest = "cluster_ipv4_cidr"
         elif key == "diskType":
@@ -4222,15 +4634,15 @@
         :param Sequence[str] master_authorized_network_cidr_blocks: Define up to 10 external networks that could access Kubernetes master through HTTPS (list)
         :param int max_node_count: Maximum number of nodes in the NodePool. Must be >= minNodeCount. There has to enough quota to scale up the cluster. Default `0` (int)
         :param int min_node_count: Minimmum number of nodes in the NodePool. Must be >= 1 and <= maxNodeCount. Default `0` (int)
         :param int node_count: Node count for GKE cluster. Default `3` (int)
         :param bool preemptible: Whether the nodes are created as preemptible VM instances. Default `false` (bool)
         :param str region: (string)
         :param Mapping[str, Any] resource_labels: The map of Kubernetes labels to be applied to each cluster (map)
-        :param Sequence[str] taints: List of Kubernetes taints to be applied to each node (list)
+        :param Sequence[str] taints: The AKS node pool taints (list)
         :param bool use_ip_aliases: Whether alias IPs will be used for pod IPs in the cluster. Default `false` (bool)
         :param str zone: (string)
         """
         pulumi.set(__self__, "cluster_ipv4_cidr", cluster_ipv4_cidr)
         pulumi.set(__self__, "credential", credential)
         pulumi.set(__self__, "disk_type", disk_type)
         pulumi.set(__self__, "image_type", image_type)
@@ -4715,15 +5127,15 @@
         """
         return pulumi.get(self, "resource_labels")
 
     @property
     @pulumi.getter
     def taints(self) -> Optional[Sequence[str]]:
         """
-        List of Kubernetes taints to be applied to each node (list)
+        The AKS node pool taints (list)
         """
         return pulumi.get(self, "taints")
 
     @property
     @pulumi.getter(name="useIpAliases")
     def use_ip_aliases(self) -> Optional[bool]:
         """
@@ -5576,15 +5988,15 @@
         :param str image_type: The image to use for the worker nodes (string)
         :param Mapping[str, Any] labels: Labels for the Cluster (map)
         :param int local_ssd_count: The number of local SSD disks to be attached to the node. Default `0` (int)
         :param str machine_type: Machine type for GKE cluster (string)
         :param Sequence[str] oauth_scopes: The set of Google API scopes to be made available on all of the node VMs under the default service account (list)
         :param bool preemptible: Whether the nodes are created as preemptible VM instances. Default `false` (bool)
         :param Sequence[str] tags: Tags for Kubernetes cluster. For example, `["foo=bar","bar=foo"]` (list)
-        :param Sequence['ClusterGkeConfigV2NodePoolConfigTaintArgs'] taints: List of Kubernetes taints to be applied to each node (list)
+        :param Sequence['ClusterGkeConfigV2NodePoolConfigTaintArgs'] taints: The AKS node pool taints (list)
         """
         if disk_size_gb is not None:
             pulumi.set(__self__, "disk_size_gb", disk_size_gb)
         if disk_type is not None:
             pulumi.set(__self__, "disk_type", disk_type)
         if image_type is not None:
             pulumi.set(__self__, "image_type", image_type)
@@ -5675,15 +6087,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def taints(self) -> Optional[Sequence['outputs.ClusterGkeConfigV2NodePoolConfigTaint']]:
         """
-        List of Kubernetes taints to be applied to each node (list)
+        The AKS node pool taints (list)
         """
         return pulumi.get(self, "taints")
 
 
 @pulumi.output_type
 class ClusterGkeConfigV2NodePoolConfigTaint(dict):
     def __init__(__self__, *,
@@ -12092,28 +12504,28 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ClusterRkeConfigServicesKubeApi.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 admission_configuration: Optional[Mapping[str, Any]] = None,
+                 admission_configuration: Optional['outputs.ClusterRkeConfigServicesKubeApiAdmissionConfiguration'] = None,
                  always_pull_images: Optional[bool] = None,
                  audit_log: Optional['outputs.ClusterRkeConfigServicesKubeApiAuditLog'] = None,
                  event_rate_limit: Optional['outputs.ClusterRkeConfigServicesKubeApiEventRateLimit'] = None,
                  extra_args: Optional[Mapping[str, Any]] = None,
                  extra_binds: Optional[Sequence[str]] = None,
                  extra_envs: Optional[Sequence[str]] = None,
                  image: Optional[str] = None,
                  pod_security_policy: Optional[bool] = None,
                  secrets_encryption_config: Optional['outputs.ClusterRkeConfigServicesKubeApiSecretsEncryptionConfig'] = None,
                  service_cluster_ip_range: Optional[str] = None,
                  service_node_port_range: Optional[str] = None):
         """
-        :param Mapping[str, Any] admission_configuration: Admission configuration (map)
+        :param 'ClusterRkeConfigServicesKubeApiAdmissionConfigurationArgs' admission_configuration: Admission configuration (map)
         :param bool always_pull_images: Enable [AlwaysPullImages](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/#alwayspullimages) Admission controller plugin. [Rancher docs](https://rancher.com/docs/rke/latest/en/config-options/services/#kubernetes-api-server-options) Default: `false` (bool)
         :param 'ClusterRkeConfigServicesKubeApiAuditLogArgs' audit_log: K8s audit log configuration. (list maxitems: 1)
         :param 'ClusterRkeConfigServicesKubeApiEventRateLimitArgs' event_rate_limit: K8s event rate limit configuration. (list maxitems: 1)
         :param Mapping[str, Any] extra_args: Extra arguments for RKE Ingress (map)
         :param Sequence[str] extra_binds: Extra binds for etcd service (list)
         :param Sequence[str] extra_envs: Extra environment for etcd service (list)
         :param str image: Docker image for etcd service (string)
@@ -12145,15 +12557,15 @@
         if service_cluster_ip_range is not None:
             pulumi.set(__self__, "service_cluster_ip_range", service_cluster_ip_range)
         if service_node_port_range is not None:
             pulumi.set(__self__, "service_node_port_range", service_node_port_range)
 
     @property
     @pulumi.getter(name="admissionConfiguration")
-    def admission_configuration(self) -> Optional[Mapping[str, Any]]:
+    def admission_configuration(self) -> Optional['outputs.ClusterRkeConfigServicesKubeApiAdmissionConfiguration']:
         """
         Admission configuration (map)
         """
         return pulumi.get(self, "admission_configuration")
 
     @property
     @pulumi.getter(name="alwaysPullImages")
@@ -12241,32 +12653,183 @@
         """
         Service Node Port Range option for kube API service (string)
         """
         return pulumi.get(self, "service_node_port_range")
 
 
 @pulumi.output_type
+class ClusterRkeConfigServicesKubeApiAdmissionConfiguration(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "apiVersion":
+            suggest = "api_version"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterRkeConfigServicesKubeApiAdmissionConfiguration. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterRkeConfigServicesKubeApiAdmissionConfiguration.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterRkeConfigServicesKubeApiAdmissionConfiguration.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 api_version: Optional[str] = None,
+                 kind: Optional[str] = None,
+                 plugins: Optional[Sequence['outputs.ClusterRkeConfigServicesKubeApiAdmissionConfigurationPlugin']] = None):
+        """
+        :param str api_version: Admission configuration ApiVersion. Default: `apiserver.config.k8s.io/v1` (string)
+        :param str kind: Admission configuration Kind. Default: `AdmissionConfiguration` (string)
+        :param Sequence['ClusterRkeConfigServicesKubeApiAdmissionConfigurationPluginArgs'] plugins: Admission configuration plugins. (list `plugin`)
+        """
+        if api_version is not None:
+            pulumi.set(__self__, "api_version", api_version)
+        if kind is not None:
+            pulumi.set(__self__, "kind", kind)
+        if plugins is not None:
+            pulumi.set(__self__, "plugins", plugins)
+
+    @property
+    @pulumi.getter(name="apiVersion")
+    def api_version(self) -> Optional[str]:
+        """
+        Admission configuration ApiVersion. Default: `apiserver.config.k8s.io/v1` (string)
+        """
+        return pulumi.get(self, "api_version")
+
+    @property
+    @pulumi.getter
+    def kind(self) -> Optional[str]:
+        """
+        Admission configuration Kind. Default: `AdmissionConfiguration` (string)
+        """
+        return pulumi.get(self, "kind")
+
+    @property
+    @pulumi.getter
+    def plugins(self) -> Optional[Sequence['outputs.ClusterRkeConfigServicesKubeApiAdmissionConfigurationPlugin']]:
+        """
+        Admission configuration plugins. (list `plugin`)
+        """
+        return pulumi.get(self, "plugins")
+
+
+@pulumi.output_type
+class ClusterRkeConfigServicesKubeApiAdmissionConfigurationPlugin(dict):
+    def __init__(__self__, *,
+                 configuration: Optional[str] = None,
+                 name: Optional[str] = None,
+                 path: Optional[str] = None):
+        """
+        :param str configuration: Plugin configuration. (string) Ex:
+               
+               ```python
+               import pulumi
+               ```
+               configuration = <<EOF
+               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+               kind: Configuration
+               limits:
+               - type: Server
+               burst: 35000
+               qps: 6000
+               EOF
+        :param str name: The name of the Cluster (string)
+        :param str path: Path for etcd service (string)
+        """
+        if configuration is not None:
+            pulumi.set(__self__, "configuration", configuration)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if path is not None:
+            pulumi.set(__self__, "path", path)
+
+    @property
+    @pulumi.getter
+    def configuration(self) -> Optional[str]:
+        """
+        Plugin configuration. (string) Ex:
+
+        ```python
+        import pulumi
+        ```
+        configuration = <<EOF
+        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+        kind: Configuration
+        limits:
+        - type: Server
+        burst: 35000
+        qps: 6000
+        EOF
+        """
+        return pulumi.get(self, "configuration")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        The name of the Cluster (string)
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def path(self) -> Optional[str]:
+        """
+        Path for etcd service (string)
+        """
+        return pulumi.get(self, "path")
+
+
+@pulumi.output_type
 class ClusterRkeConfigServicesKubeApiAuditLog(dict):
     def __init__(__self__, *,
                  configuration: Optional['outputs.ClusterRkeConfigServicesKubeApiAuditLogConfiguration'] = None,
                  enabled: Optional[bool] = None):
         """
-        :param 'ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs' configuration: Audit log configuration. (list maxitems: 1)
+        :param 'ClusterRkeConfigServicesKubeApiAuditLogConfigurationArgs' configuration: Plugin configuration. (string) Ex:
+               
+               ```python
+               import pulumi
+               ```
+               configuration = <<EOF
+               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+               kind: Configuration
+               limits:
+               - type: Server
+               burst: 35000
+               qps: 6000
+               EOF
         :param bool enabled: Enable etcd backup (bool)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional['outputs.ClusterRkeConfigServicesKubeApiAuditLogConfiguration']:
         """
-        Audit log configuration. (list maxitems: 1)
+        Plugin configuration. (string) Ex:
+
+        ```python
+        import pulumi
+        ```
+        configuration = <<EOF
+        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+        kind: Configuration
+        limits:
+        - type: Server
+        burst: 35000
+        qps: 6000
+        EOF
         """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
@@ -12377,27 +12940,51 @@
 
 @pulumi.output_type
 class ClusterRkeConfigServicesKubeApiEventRateLimit(dict):
     def __init__(__self__, *,
                  configuration: Optional[str] = None,
                  enabled: Optional[bool] = None):
         """
-        :param str configuration: Audit log configuration. (list maxitems: 1)
+        :param str configuration: Plugin configuration. (string) Ex:
+               
+               ```python
+               import pulumi
+               ```
+               configuration = <<EOF
+               apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+               kind: Configuration
+               limits:
+               - type: Server
+               burst: 35000
+               qps: 6000
+               EOF
         :param bool enabled: Enable etcd backup (bool)
         """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[str]:
         """
-        Audit log configuration. (list maxitems: 1)
+        Plugin configuration. (string) Ex:
+
+        ```python
+        import pulumi
+        ```
+        configuration = <<EOF
+        apiVersion: eventratelimit.admission.k8s.io/v1alpha1
+        kind: Configuration
+        limits:
+        - type: Server
+        burst: 35000
+        qps: 6000
+        EOF
         """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
         """
@@ -13463,14 +14050,16 @@
         suggest = None
         if key == "rkeConfig":
             suggest = "rke_config"
         elif key == "clusterAuthEndpoint":
             suggest = "cluster_auth_endpoint"
         elif key == "defaultClusterRoleForProjectMembers":
             suggest = "default_cluster_role_for_project_members"
+        elif key == "defaultPodSecurityAdmissionConfigurationTemplateName":
+            suggest = "default_pod_security_admission_configuration_template_name"
         elif key == "defaultPodSecurityPolicyTemplateId":
             suggest = "default_pod_security_policy_template_id"
         elif key == "desiredAgentImage":
             suggest = "desired_agent_image"
         elif key == "desiredAuthImage":
             suggest = "desired_auth_image"
         elif key == "dockerRootDir":
@@ -13495,14 +14084,15 @@
         ClusterTemplateTemplateRevisionClusterConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  rke_config: 'outputs.ClusterTemplateTemplateRevisionClusterConfigRkeConfig',
                  cluster_auth_endpoint: Optional['outputs.ClusterTemplateTemplateRevisionClusterConfigClusterAuthEndpoint'] = None,
                  default_cluster_role_for_project_members: Optional[str] = None,
+                 default_pod_security_admission_configuration_template_name: Optional[str] = None,
                  default_pod_security_policy_template_id: Optional[str] = None,
                  desired_agent_image: Optional[str] = None,
                  desired_auth_image: Optional[str] = None,
                  docker_root_dir: Optional[str] = None,
                  enable_cluster_alerting: Optional[bool] = None,
                  enable_cluster_monitoring: Optional[bool] = None,
                  enable_network_policy: Optional[bool] = None,
@@ -13521,14 +14111,16 @@
         :param bool windows_prefered_cluster: Windows prefered cluster. Default: `false` (bool)
         """
         pulumi.set(__self__, "rke_config", rke_config)
         if cluster_auth_endpoint is not None:
             pulumi.set(__self__, "cluster_auth_endpoint", cluster_auth_endpoint)
         if default_cluster_role_for_project_members is not None:
             pulumi.set(__self__, "default_cluster_role_for_project_members", default_cluster_role_for_project_members)
+        if default_pod_security_admission_configuration_template_name is not None:
+            pulumi.set(__self__, "default_pod_security_admission_configuration_template_name", default_pod_security_admission_configuration_template_name)
         if default_pod_security_policy_template_id is not None:
             pulumi.set(__self__, "default_pod_security_policy_template_id", default_pod_security_policy_template_id)
         if desired_agent_image is not None:
             pulumi.set(__self__, "desired_agent_image", desired_agent_image)
         if desired_auth_image is not None:
             pulumi.set(__self__, "desired_auth_image", desired_auth_image)
         if docker_root_dir is not None:
@@ -13563,14 +14155,19 @@
     def default_cluster_role_for_project_members(self) -> Optional[str]:
         """
         Default cluster role for project members (string)
         """
         return pulumi.get(self, "default_cluster_role_for_project_members")
 
     @property
+    @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
+    def default_pod_security_admission_configuration_template_name(self) -> Optional[str]:
+        return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
+
+    @property
     @pulumi.getter(name="defaultPodSecurityPolicyTemplateId")
     def default_pod_security_policy_template_id(self) -> Optional[str]:
         """
         Default pod security policy template ID (string)
         """
         return pulumi.get(self, "default_pod_security_policy_template_id")
 
@@ -17769,15 +18366,15 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApi.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 admission_configuration: Optional[Mapping[str, Any]] = None,
+                 admission_configuration: Optional['outputs.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfiguration'] = None,
                  always_pull_images: Optional[bool] = None,
                  audit_log: Optional['outputs.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLog'] = None,
                  event_rate_limit: Optional['outputs.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiEventRateLimit'] = None,
                  extra_args: Optional[Mapping[str, Any]] = None,
                  extra_binds: Optional[Sequence[str]] = None,
                  extra_envs: Optional[Sequence[str]] = None,
                  image: Optional[str] = None,
@@ -17808,15 +18405,15 @@
         if service_cluster_ip_range is not None:
             pulumi.set(__self__, "service_cluster_ip_range", service_cluster_ip_range)
         if service_node_port_range is not None:
             pulumi.set(__self__, "service_node_port_range", service_node_port_range)
 
     @property
     @pulumi.getter(name="admissionConfiguration")
-    def admission_configuration(self) -> Optional[Mapping[str, Any]]:
+    def admission_configuration(self) -> Optional['outputs.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfiguration']:
         return pulumi.get(self, "admission_configuration")
 
     @property
     @pulumi.getter(name="alwaysPullImages")
     def always_pull_images(self) -> Optional[bool]:
         return pulumi.get(self, "always_pull_images")
 
@@ -17868,14 +18465,95 @@
     @property
     @pulumi.getter(name="serviceNodePortRange")
     def service_node_port_range(self) -> Optional[str]:
         return pulumi.get(self, "service_node_port_range")
 
 
 @pulumi.output_type
+class ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfiguration(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "apiVersion":
+            suggest = "api_version"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfiguration. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfiguration.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfiguration.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 api_version: Optional[str] = None,
+                 kind: Optional[str] = None,
+                 plugins: Optional[Sequence['outputs.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPlugin']] = None):
+        if api_version is not None:
+            pulumi.set(__self__, "api_version", api_version)
+        if kind is not None:
+            pulumi.set(__self__, "kind", kind)
+        if plugins is not None:
+            pulumi.set(__self__, "plugins", plugins)
+
+    @property
+    @pulumi.getter(name="apiVersion")
+    def api_version(self) -> Optional[str]:
+        return pulumi.get(self, "api_version")
+
+    @property
+    @pulumi.getter
+    def kind(self) -> Optional[str]:
+        return pulumi.get(self, "kind")
+
+    @property
+    @pulumi.getter
+    def plugins(self) -> Optional[Sequence['outputs.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPlugin']]:
+        return pulumi.get(self, "plugins")
+
+
+@pulumi.output_type
+class ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPlugin(dict):
+    def __init__(__self__, *,
+                 configuration: Optional[str] = None,
+                 name: Optional[str] = None,
+                 path: Optional[str] = None):
+        """
+        :param str name: The cluster template name (string)
+        """
+        if configuration is not None:
+            pulumi.set(__self__, "configuration", configuration)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if path is not None:
+            pulumi.set(__self__, "path", path)
+
+    @property
+    @pulumi.getter
+    def configuration(self) -> Optional[str]:
+        return pulumi.get(self, "configuration")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        The cluster template name (string)
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def path(self) -> Optional[str]:
+        return pulumi.get(self, "path")
+
+
+@pulumi.output_type
 class ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLog(dict):
     def __init__(__self__, *,
                  configuration: Optional['outputs.ClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLogConfiguration'] = None,
                  enabled: Optional[bool] = None):
         """
         :param bool enabled: Enable cluster template revision. Default `true` (bool)
         """
@@ -18548,14 +19226,186 @@
         """
         Rancher agent env var value (string)
         """
         return pulumi.get(self, "value")
 
 
 @pulumi.output_type
+class ClusterV2ClusterAgentDeploymentCustomization(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "appendTolerations":
+            suggest = "append_tolerations"
+        elif key == "overrideAffinity":
+            suggest = "override_affinity"
+        elif key == "overrideResourceRequirements":
+            suggest = "override_resource_requirements"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterV2ClusterAgentDeploymentCustomization. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterV2ClusterAgentDeploymentCustomization.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterV2ClusterAgentDeploymentCustomization.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 append_tolerations: Optional[Sequence['outputs.ClusterV2ClusterAgentDeploymentCustomizationAppendToleration']] = None,
+                 override_affinity: Optional[str] = None,
+                 override_resource_requirements: Optional[Sequence['outputs.ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirement']] = None):
+        if append_tolerations is not None:
+            pulumi.set(__self__, "append_tolerations", append_tolerations)
+        if override_affinity is not None:
+            pulumi.set(__self__, "override_affinity", override_affinity)
+        if override_resource_requirements is not None:
+            pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
+
+    @property
+    @pulumi.getter(name="appendTolerations")
+    def append_tolerations(self) -> Optional[Sequence['outputs.ClusterV2ClusterAgentDeploymentCustomizationAppendToleration']]:
+        return pulumi.get(self, "append_tolerations")
+
+    @property
+    @pulumi.getter(name="overrideAffinity")
+    def override_affinity(self) -> Optional[str]:
+        return pulumi.get(self, "override_affinity")
+
+    @property
+    @pulumi.getter(name="overrideResourceRequirements")
+    def override_resource_requirements(self) -> Optional[Sequence['outputs.ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirement']]:
+        return pulumi.get(self, "override_resource_requirements")
+
+
+@pulumi.output_type
+class ClusterV2ClusterAgentDeploymentCustomizationAppendToleration(dict):
+    def __init__(__self__, *,
+                 key: str,
+                 effect: Optional[str] = None,
+                 operator: Optional[str] = None,
+                 seconds: Optional[int] = None,
+                 value: Optional[str] = None):
+        """
+        :param str key: The taint key (string)
+        :param str effect: The taint effect. Default: `\\"NoExecute\\"` (string)
+        :param str operator: Machine selector label match expressions operator (string)
+        :param str value: Rancher agent env var value (string)
+        """
+        pulumi.set(__self__, "key", key)
+        if effect is not None:
+            pulumi.set(__self__, "effect", effect)
+        if operator is not None:
+            pulumi.set(__self__, "operator", operator)
+        if seconds is not None:
+            pulumi.set(__self__, "seconds", seconds)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> str:
+        """
+        The taint key (string)
+        """
+        return pulumi.get(self, "key")
+
+    @property
+    @pulumi.getter
+    def effect(self) -> Optional[str]:
+        """
+        The taint effect. Default: `\\"NoExecute\\"` (string)
+        """
+        return pulumi.get(self, "effect")
+
+    @property
+    @pulumi.getter
+    def operator(self) -> Optional[str]:
+        """
+        Machine selector label match expressions operator (string)
+        """
+        return pulumi.get(self, "operator")
+
+    @property
+    @pulumi.getter
+    def seconds(self) -> Optional[int]:
+        return pulumi.get(self, "seconds")
+
+    @property
+    @pulumi.getter
+    def value(self) -> Optional[str]:
+        """
+        Rancher agent env var value (string)
+        """
+        return pulumi.get(self, "value")
+
+
+@pulumi.output_type
+class ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirement(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "cpuLimit":
+            suggest = "cpu_limit"
+        elif key == "cpuRequest":
+            suggest = "cpu_request"
+        elif key == "memoryLimit":
+            suggest = "memory_limit"
+        elif key == "memoryRequest":
+            suggest = "memory_request"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirement. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirement.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterV2ClusterAgentDeploymentCustomizationOverrideResourceRequirement.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 cpu_limit: Optional[str] = None,
+                 cpu_request: Optional[str] = None,
+                 memory_limit: Optional[str] = None,
+                 memory_request: Optional[str] = None):
+        if cpu_limit is not None:
+            pulumi.set(__self__, "cpu_limit", cpu_limit)
+        if cpu_request is not None:
+            pulumi.set(__self__, "cpu_request", cpu_request)
+        if memory_limit is not None:
+            pulumi.set(__self__, "memory_limit", memory_limit)
+        if memory_request is not None:
+            pulumi.set(__self__, "memory_request", memory_request)
+
+    @property
+    @pulumi.getter(name="cpuLimit")
+    def cpu_limit(self) -> Optional[str]:
+        return pulumi.get(self, "cpu_limit")
+
+    @property
+    @pulumi.getter(name="cpuRequest")
+    def cpu_request(self) -> Optional[str]:
+        return pulumi.get(self, "cpu_request")
+
+    @property
+    @pulumi.getter(name="memoryLimit")
+    def memory_limit(self) -> Optional[str]:
+        return pulumi.get(self, "memory_limit")
+
+    @property
+    @pulumi.getter(name="memoryRequest")
+    def memory_request(self) -> Optional[str]:
+        return pulumi.get(self, "memory_request")
+
+
+@pulumi.output_type
 class ClusterV2ClusterRegistrationToken(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "clusterId":
             suggest = "cluster_id"
         elif key == "insecureCommand":
@@ -18740,14 +19590,186 @@
         """
         Node command to execute in windows nodes for custom k8s cluster (string)
         """
         return pulumi.get(self, "windows_node_command")
 
 
 @pulumi.output_type
+class ClusterV2FleetAgentDeploymentCustomization(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "appendTolerations":
+            suggest = "append_tolerations"
+        elif key == "overrideAffinity":
+            suggest = "override_affinity"
+        elif key == "overrideResourceRequirements":
+            suggest = "override_resource_requirements"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterV2FleetAgentDeploymentCustomization. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterV2FleetAgentDeploymentCustomization.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterV2FleetAgentDeploymentCustomization.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 append_tolerations: Optional[Sequence['outputs.ClusterV2FleetAgentDeploymentCustomizationAppendToleration']] = None,
+                 override_affinity: Optional[str] = None,
+                 override_resource_requirements: Optional[Sequence['outputs.ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirement']] = None):
+        if append_tolerations is not None:
+            pulumi.set(__self__, "append_tolerations", append_tolerations)
+        if override_affinity is not None:
+            pulumi.set(__self__, "override_affinity", override_affinity)
+        if override_resource_requirements is not None:
+            pulumi.set(__self__, "override_resource_requirements", override_resource_requirements)
+
+    @property
+    @pulumi.getter(name="appendTolerations")
+    def append_tolerations(self) -> Optional[Sequence['outputs.ClusterV2FleetAgentDeploymentCustomizationAppendToleration']]:
+        return pulumi.get(self, "append_tolerations")
+
+    @property
+    @pulumi.getter(name="overrideAffinity")
+    def override_affinity(self) -> Optional[str]:
+        return pulumi.get(self, "override_affinity")
+
+    @property
+    @pulumi.getter(name="overrideResourceRequirements")
+    def override_resource_requirements(self) -> Optional[Sequence['outputs.ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirement']]:
+        return pulumi.get(self, "override_resource_requirements")
+
+
+@pulumi.output_type
+class ClusterV2FleetAgentDeploymentCustomizationAppendToleration(dict):
+    def __init__(__self__, *,
+                 key: str,
+                 effect: Optional[str] = None,
+                 operator: Optional[str] = None,
+                 seconds: Optional[int] = None,
+                 value: Optional[str] = None):
+        """
+        :param str key: The taint key (string)
+        :param str effect: The taint effect. Default: `\\"NoExecute\\"` (string)
+        :param str operator: Machine selector label match expressions operator (string)
+        :param str value: Rancher agent env var value (string)
+        """
+        pulumi.set(__self__, "key", key)
+        if effect is not None:
+            pulumi.set(__self__, "effect", effect)
+        if operator is not None:
+            pulumi.set(__self__, "operator", operator)
+        if seconds is not None:
+            pulumi.set(__self__, "seconds", seconds)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def key(self) -> str:
+        """
+        The taint key (string)
+        """
+        return pulumi.get(self, "key")
+
+    @property
+    @pulumi.getter
+    def effect(self) -> Optional[str]:
+        """
+        The taint effect. Default: `\\"NoExecute\\"` (string)
+        """
+        return pulumi.get(self, "effect")
+
+    @property
+    @pulumi.getter
+    def operator(self) -> Optional[str]:
+        """
+        Machine selector label match expressions operator (string)
+        """
+        return pulumi.get(self, "operator")
+
+    @property
+    @pulumi.getter
+    def seconds(self) -> Optional[int]:
+        return pulumi.get(self, "seconds")
+
+    @property
+    @pulumi.getter
+    def value(self) -> Optional[str]:
+        """
+        Rancher agent env var value (string)
+        """
+        return pulumi.get(self, "value")
+
+
+@pulumi.output_type
+class ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirement(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "cpuLimit":
+            suggest = "cpu_limit"
+        elif key == "cpuRequest":
+            suggest = "cpu_request"
+        elif key == "memoryLimit":
+            suggest = "memory_limit"
+        elif key == "memoryRequest":
+            suggest = "memory_request"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirement. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirement.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterV2FleetAgentDeploymentCustomizationOverrideResourceRequirement.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 cpu_limit: Optional[str] = None,
+                 cpu_request: Optional[str] = None,
+                 memory_limit: Optional[str] = None,
+                 memory_request: Optional[str] = None):
+        if cpu_limit is not None:
+            pulumi.set(__self__, "cpu_limit", cpu_limit)
+        if cpu_request is not None:
+            pulumi.set(__self__, "cpu_request", cpu_request)
+        if memory_limit is not None:
+            pulumi.set(__self__, "memory_limit", memory_limit)
+        if memory_request is not None:
+            pulumi.set(__self__, "memory_request", memory_request)
+
+    @property
+    @pulumi.getter(name="cpuLimit")
+    def cpu_limit(self) -> Optional[str]:
+        return pulumi.get(self, "cpu_limit")
+
+    @property
+    @pulumi.getter(name="cpuRequest")
+    def cpu_request(self) -> Optional[str]:
+        return pulumi.get(self, "cpu_request")
+
+    @property
+    @pulumi.getter(name="memoryLimit")
+    def memory_limit(self) -> Optional[str]:
+        return pulumi.get(self, "memory_limit")
+
+    @property
+    @pulumi.getter(name="memoryRequest")
+    def memory_request(self) -> Optional[str]:
+        return pulumi.get(self, "memory_request")
+
+
+@pulumi.output_type
 class ClusterV2LocalAuthEndpoint(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "caCerts":
             suggest = "ca_certs"
 
@@ -18816,14 +19838,16 @@
             suggest = "etcd_snapshot_create"
         elif key == "etcdSnapshotRestore":
             suggest = "etcd_snapshot_restore"
         elif key == "localAuthEndpoint":
             suggest = "local_auth_endpoint"
         elif key == "machineGlobalConfig":
             suggest = "machine_global_config"
+        elif key == "machinePoolDefaults":
+            suggest = "machine_pool_defaults"
         elif key == "machinePools":
             suggest = "machine_pools"
         elif key == "machineSelectorConfigs":
             suggest = "machine_selector_configs"
         elif key == "rotateCertificates":
             suggest = "rotate_certificates"
         elif key == "upgradeStrategy":
@@ -18844,14 +19868,15 @@
                  additional_manifest: Optional[str] = None,
                  chart_values: Optional[str] = None,
                  etcd: Optional['outputs.ClusterV2RkeConfigEtcd'] = None,
                  etcd_snapshot_create: Optional['outputs.ClusterV2RkeConfigEtcdSnapshotCreate'] = None,
                  etcd_snapshot_restore: Optional['outputs.ClusterV2RkeConfigEtcdSnapshotRestore'] = None,
                  local_auth_endpoint: Optional['outputs.ClusterV2RkeConfigLocalAuthEndpoint'] = None,
                  machine_global_config: Optional[str] = None,
+                 machine_pool_defaults: Optional[Sequence['outputs.ClusterV2RkeConfigMachinePoolDefault']] = None,
                  machine_pools: Optional[Sequence['outputs.ClusterV2RkeConfigMachinePool']] = None,
                  machine_selector_configs: Optional[Sequence['outputs.ClusterV2RkeConfigMachineSelectorConfig']] = None,
                  registries: Optional['outputs.ClusterV2RkeConfigRegistries'] = None,
                  rotate_certificates: Optional['outputs.ClusterV2RkeConfigRotateCertificates'] = None,
                  upgrade_strategy: Optional['outputs.ClusterV2RkeConfigUpgradeStrategy'] = None):
         """
         :param str additional_manifest: Cluster V2 additional manifest (string)
@@ -18877,14 +19902,16 @@
             pulumi.set(__self__, "etcd_snapshot_create", etcd_snapshot_create)
         if etcd_snapshot_restore is not None:
             pulumi.set(__self__, "etcd_snapshot_restore", etcd_snapshot_restore)
         if local_auth_endpoint is not None:
             pulumi.set(__self__, "local_auth_endpoint", local_auth_endpoint)
         if machine_global_config is not None:
             pulumi.set(__self__, "machine_global_config", machine_global_config)
+        if machine_pool_defaults is not None:
+            pulumi.set(__self__, "machine_pool_defaults", machine_pool_defaults)
         if machine_pools is not None:
             pulumi.set(__self__, "machine_pools", machine_pools)
         if machine_selector_configs is not None:
             pulumi.set(__self__, "machine_selector_configs", machine_selector_configs)
         if registries is not None:
             pulumi.set(__self__, "registries", registries)
         if rotate_certificates is not None:
@@ -18945,14 +19972,19 @@
     def machine_global_config(self) -> Optional[str]:
         """
         Cluster V2 machine global config. Must be in YAML format (string)
         """
         return pulumi.get(self, "machine_global_config")
 
     @property
+    @pulumi.getter(name="machinePoolDefaults")
+    def machine_pool_defaults(self) -> Optional[Sequence['outputs.ClusterV2RkeConfigMachinePoolDefault']]:
+        return pulumi.get(self, "machine_pool_defaults")
+
+    @property
     @pulumi.getter(name="machinePools")
     def machine_pools(self) -> Optional[Sequence['outputs.ClusterV2RkeConfigMachinePool']]:
         """
         Cluster V2 machine pools (list)
         """
         return pulumi.get(self, "machine_pools")
 
@@ -19324,14 +20356,16 @@
             suggest = "cloud_credential_secret_name"
         elif key == "controlPlaneRole":
             suggest = "control_plane_role"
         elif key == "drainBeforeDelete":
             suggest = "drain_before_delete"
         elif key == "etcdRole":
             suggest = "etcd_role"
+        elif key == "hostnameLengthLimit":
+            suggest = "hostname_length_limit"
         elif key == "machineLabels":
             suggest = "machine_labels"
         elif key == "maxUnhealthy":
             suggest = "max_unhealthy"
         elif key == "nodeDrainTimeout":
             suggest = "node_drain_timeout"
         elif key == "nodeStartupTimeoutSeconds":
@@ -19360,14 +20394,15 @@
                  machine_config: 'outputs.ClusterV2RkeConfigMachinePoolMachineConfig',
                  name: str,
                  annotations: Optional[Mapping[str, Any]] = None,
                  cloud_credential_secret_name: Optional[str] = None,
                  control_plane_role: Optional[bool] = None,
                  drain_before_delete: Optional[bool] = None,
                  etcd_role: Optional[bool] = None,
+                 hostname_length_limit: Optional[int] = None,
                  labels: Optional[Mapping[str, Any]] = None,
                  machine_labels: Optional[Mapping[str, Any]] = None,
                  max_unhealthy: Optional[str] = None,
                  node_drain_timeout: Optional[int] = None,
                  node_startup_timeout_seconds: Optional[int] = None,
                  paused: Optional[bool] = None,
                  quantity: Optional[int] = None,
@@ -19405,14 +20440,16 @@
             pulumi.set(__self__, "cloud_credential_secret_name", cloud_credential_secret_name)
         if control_plane_role is not None:
             pulumi.set(__self__, "control_plane_role", control_plane_role)
         if drain_before_delete is not None:
             pulumi.set(__self__, "drain_before_delete", drain_before_delete)
         if etcd_role is not None:
             pulumi.set(__self__, "etcd_role", etcd_role)
+        if hostname_length_limit is not None:
+            pulumi.set(__self__, "hostname_length_limit", hostname_length_limit)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if machine_labels is not None:
             pulumi.set(__self__, "machine_labels", machine_labels)
         if max_unhealthy is not None:
             pulumi.set(__self__, "max_unhealthy", max_unhealthy)
         if node_drain_timeout is not None:
@@ -19487,14 +20524,19 @@
     def etcd_role(self) -> Optional[bool]:
         """
         Machine pool etcd role? (bool)
         """
         return pulumi.get(self, "etcd_role")
 
     @property
+    @pulumi.getter(name="hostnameLengthLimit")
+    def hostname_length_limit(self) -> Optional[int]:
+        return pulumi.get(self, "hostname_length_limit")
+
+    @property
     @pulumi.getter
     def labels(self) -> Optional[Mapping[str, Any]]:
         """
         Labels for the Cluster V2 (map)
         """
         return pulumi.get(self, "labels")
 
@@ -19584,14 +20626,44 @@
         """
         Machine pool worker role? (bool)
         """
         return pulumi.get(self, "worker_role")
 
 
 @pulumi.output_type
+class ClusterV2RkeConfigMachinePoolDefault(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "hostnameLengthLimit":
+            suggest = "hostname_length_limit"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ClusterV2RkeConfigMachinePoolDefault. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ClusterV2RkeConfigMachinePoolDefault.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ClusterV2RkeConfigMachinePoolDefault.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 hostname_length_limit: Optional[int] = None):
+        if hostname_length_limit is not None:
+            pulumi.set(__self__, "hostname_length_limit", hostname_length_limit)
+
+    @property
+    @pulumi.getter(name="hostnameLengthLimit")
+    def hostname_length_limit(self) -> Optional[int]:
+        return pulumi.get(self, "hostname_length_limit")
+
+
+@pulumi.output_type
 class ClusterV2RkeConfigMachinePoolMachineConfig(dict):
     def __init__(__self__, *,
                  kind: str,
                  name: str):
         """
         :param str kind: Machine config kind (string)
         :param str name: The name of the Cluster v2 (string)
@@ -29981,42 +31053,50 @@
     def node_pools(self) -> Optional[Sequence['outputs.GetClusterAksConfigV2NodePoolResult']]:
         return pulumi.get(self, "node_pools")
 
 
 @pulumi.output_type
 class GetClusterAksConfigV2NodePoolResult(dict):
     def __init__(__self__, *,
+                 labels: Mapping[str, Any],
                  name: str,
+                 taints: Sequence[str],
                  vm_size: str,
                  availability_zones: Optional[Sequence[str]] = None,
                  count: Optional[int] = None,
                  enable_auto_scaling: Optional[bool] = None,
                  max_count: Optional[int] = None,
                  max_pods: Optional[int] = None,
+                 max_surge: Optional[str] = None,
                  min_count: Optional[int] = None,
                  mode: Optional[str] = None,
                  orchestrator_version: Optional[str] = None,
                  os_disk_size_gb: Optional[int] = None,
                  os_disk_type: Optional[str] = None,
                  os_type: Optional[str] = None):
         """
+        :param Mapping[str, Any] labels: (Computed) Labels for Node Pool object (map)
         :param str name: The name of the Cluster (string)
         """
+        pulumi.set(__self__, "labels", labels)
         pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "taints", taints)
         pulumi.set(__self__, "vm_size", vm_size)
         if availability_zones is not None:
             pulumi.set(__self__, "availability_zones", availability_zones)
         if count is not None:
             pulumi.set(__self__, "count", count)
         if enable_auto_scaling is not None:
             pulumi.set(__self__, "enable_auto_scaling", enable_auto_scaling)
         if max_count is not None:
             pulumi.set(__self__, "max_count", max_count)
         if max_pods is not None:
             pulumi.set(__self__, "max_pods", max_pods)
+        if max_surge is not None:
+            pulumi.set(__self__, "max_surge", max_surge)
         if min_count is not None:
             pulumi.set(__self__, "min_count", min_count)
         if mode is not None:
             pulumi.set(__self__, "mode", mode)
         if orchestrator_version is not None:
             pulumi.set(__self__, "orchestrator_version", orchestrator_version)
         if os_disk_size_gb is not None:
@@ -30024,21 +31104,34 @@
         if os_disk_type is not None:
             pulumi.set(__self__, "os_disk_type", os_disk_type)
         if os_type is not None:
             pulumi.set(__self__, "os_type", os_type)
 
     @property
     @pulumi.getter
+    def labels(self) -> Mapping[str, Any]:
+        """
+        (Computed) Labels for Node Pool object (map)
+        """
+        return pulumi.get(self, "labels")
+
+    @property
+    @pulumi.getter
     def name(self) -> str:
         """
         The name of the Cluster (string)
         """
         return pulumi.get(self, "name")
 
     @property
+    @pulumi.getter
+    def taints(self) -> Sequence[str]:
+        return pulumi.get(self, "taints")
+
+    @property
     @pulumi.getter(name="vmSize")
     def vm_size(self) -> str:
         return pulumi.get(self, "vm_size")
 
     @property
     @pulumi.getter(name="availabilityZones")
     def availability_zones(self) -> Optional[Sequence[str]]:
@@ -30061,14 +31154,19 @@
 
     @property
     @pulumi.getter(name="maxPods")
     def max_pods(self) -> Optional[int]:
         return pulumi.get(self, "max_pods")
 
     @property
+    @pulumi.getter(name="maxSurge")
+    def max_surge(self) -> Optional[str]:
+        return pulumi.get(self, "max_surge")
+
+    @property
     @pulumi.getter(name="minCount")
     def min_count(self) -> Optional[int]:
         return pulumi.get(self, "min_count")
 
     @property
     @pulumi.getter
     def mode(self) -> Optional[str]:
@@ -35152,15 +36250,15 @@
 @pulumi.output_type
 class GetClusterRkeConfigServicesKubeApiResult(dict):
     def __init__(__self__, *,
                  extra_args: Mapping[str, Any],
                  image: str,
                  service_cluster_ip_range: str,
                  service_node_port_range: str,
-                 admission_configuration: Optional[Mapping[str, Any]] = None,
+                 admission_configuration: Optional['outputs.GetClusterRkeConfigServicesKubeApiAdmissionConfigurationResult'] = None,
                  always_pull_images: Optional[bool] = None,
                  audit_log: Optional['outputs.GetClusterRkeConfigServicesKubeApiAuditLogResult'] = None,
                  event_rate_limit: Optional['outputs.GetClusterRkeConfigServicesKubeApiEventRateLimitResult'] = None,
                  extra_binds: Optional[Sequence[str]] = None,
                  extra_envs: Optional[Sequence[str]] = None,
                  pod_security_policy: Optional[bool] = None,
                  secrets_encryption_config: Optional['outputs.GetClusterRkeConfigServicesKubeApiSecretsEncryptionConfigResult'] = None):
@@ -35203,15 +36301,15 @@
     @property
     @pulumi.getter(name="serviceNodePortRange")
     def service_node_port_range(self) -> str:
         return pulumi.get(self, "service_node_port_range")
 
     @property
     @pulumi.getter(name="admissionConfiguration")
-    def admission_configuration(self) -> Optional[Mapping[str, Any]]:
+    def admission_configuration(self) -> Optional['outputs.GetClusterRkeConfigServicesKubeApiAdmissionConfigurationResult']:
         return pulumi.get(self, "admission_configuration")
 
     @property
     @pulumi.getter(name="alwaysPullImages")
     def always_pull_images(self) -> Optional[bool]:
         return pulumi.get(self, "always_pull_images")
 
@@ -35243,14 +36341,75 @@
     @property
     @pulumi.getter(name="secretsEncryptionConfig")
     def secrets_encryption_config(self) -> Optional['outputs.GetClusterRkeConfigServicesKubeApiSecretsEncryptionConfigResult']:
         return pulumi.get(self, "secrets_encryption_config")
 
 
 @pulumi.output_type
+class GetClusterRkeConfigServicesKubeApiAdmissionConfigurationResult(dict):
+    def __init__(__self__, *,
+                 plugins: Sequence['outputs.GetClusterRkeConfigServicesKubeApiAdmissionConfigurationPluginResult'],
+                 api_version: Optional[str] = None,
+                 kind: Optional[str] = None):
+        pulumi.set(__self__, "plugins", plugins)
+        if api_version is not None:
+            pulumi.set(__self__, "api_version", api_version)
+        if kind is not None:
+            pulumi.set(__self__, "kind", kind)
+
+    @property
+    @pulumi.getter
+    def plugins(self) -> Sequence['outputs.GetClusterRkeConfigServicesKubeApiAdmissionConfigurationPluginResult']:
+        return pulumi.get(self, "plugins")
+
+    @property
+    @pulumi.getter(name="apiVersion")
+    def api_version(self) -> Optional[str]:
+        return pulumi.get(self, "api_version")
+
+    @property
+    @pulumi.getter
+    def kind(self) -> Optional[str]:
+        return pulumi.get(self, "kind")
+
+
+@pulumi.output_type
+class GetClusterRkeConfigServicesKubeApiAdmissionConfigurationPluginResult(dict):
+    def __init__(__self__, *,
+                 configuration: str,
+                 name: str,
+                 path: Optional[str] = None):
+        """
+        :param str name: The name of the Cluster (string)
+        """
+        pulumi.set(__self__, "configuration", configuration)
+        pulumi.set(__self__, "name", name)
+        if path is not None:
+            pulumi.set(__self__, "path", path)
+
+    @property
+    @pulumi.getter
+    def configuration(self) -> str:
+        return pulumi.get(self, "configuration")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        The name of the Cluster (string)
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def path(self) -> Optional[str]:
+        return pulumi.get(self, "path")
+
+
+@pulumi.output_type
 class GetClusterRkeConfigServicesKubeApiAuditLogResult(dict):
     def __init__(__self__, *,
                  configuration: 'outputs.GetClusterRkeConfigServicesKubeApiAuditLogConfigurationResult',
                  enabled: Optional[bool] = None):
         pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
@@ -35748,25 +36907,27 @@
 
 
 @pulumi.output_type
 class GetClusterTemplateTemplateRevisionClusterConfigResult(dict):
     def __init__(__self__, *,
                  cluster_auth_endpoint: 'outputs.GetClusterTemplateTemplateRevisionClusterConfigClusterAuthEndpointResult',
                  default_cluster_role_for_project_members: str,
+                 default_pod_security_admission_configuration_template_name: str,
                  default_pod_security_policy_template_id: str,
                  desired_agent_image: str,
                  desired_auth_image: str,
                  docker_root_dir: str,
                  rke_config: 'outputs.GetClusterTemplateTemplateRevisionClusterConfigRkeConfigResult',
                  enable_cluster_alerting: Optional[bool] = None,
                  enable_cluster_monitoring: Optional[bool] = None,
                  enable_network_policy: Optional[bool] = None,
                  windows_prefered_cluster: Optional[bool] = None):
         pulumi.set(__self__, "cluster_auth_endpoint", cluster_auth_endpoint)
         pulumi.set(__self__, "default_cluster_role_for_project_members", default_cluster_role_for_project_members)
+        pulumi.set(__self__, "default_pod_security_admission_configuration_template_name", default_pod_security_admission_configuration_template_name)
         pulumi.set(__self__, "default_pod_security_policy_template_id", default_pod_security_policy_template_id)
         pulumi.set(__self__, "desired_agent_image", desired_agent_image)
         pulumi.set(__self__, "desired_auth_image", desired_auth_image)
         pulumi.set(__self__, "docker_root_dir", docker_root_dir)
         pulumi.set(__self__, "rke_config", rke_config)
         if enable_cluster_alerting is not None:
             pulumi.set(__self__, "enable_cluster_alerting", enable_cluster_alerting)
@@ -35784,14 +36945,19 @@
 
     @property
     @pulumi.getter(name="defaultClusterRoleForProjectMembers")
     def default_cluster_role_for_project_members(self) -> str:
         return pulumi.get(self, "default_cluster_role_for_project_members")
 
     @property
+    @pulumi.getter(name="defaultPodSecurityAdmissionConfigurationTemplateName")
+    def default_pod_security_admission_configuration_template_name(self) -> str:
+        return pulumi.get(self, "default_pod_security_admission_configuration_template_name")
+
+    @property
     @pulumi.getter(name="defaultPodSecurityPolicyTemplateId")
     def default_pod_security_policy_template_id(self) -> str:
         return pulumi.get(self, "default_pod_security_policy_template_id")
 
     @property
     @pulumi.getter(name="desiredAgentImage")
     def desired_agent_image(self) -> str:
@@ -38709,15 +39875,15 @@
 @pulumi.output_type
 class GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiResult(dict):
     def __init__(__self__, *,
                  extra_args: Mapping[str, Any],
                  image: str,
                  service_cluster_ip_range: str,
                  service_node_port_range: str,
-                 admission_configuration: Optional[Mapping[str, Any]] = None,
+                 admission_configuration: Optional['outputs.GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationResult'] = None,
                  always_pull_images: Optional[bool] = None,
                  audit_log: Optional['outputs.GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLogResult'] = None,
                  event_rate_limit: Optional['outputs.GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiEventRateLimitResult'] = None,
                  extra_binds: Optional[Sequence[str]] = None,
                  extra_envs: Optional[Sequence[str]] = None,
                  pod_security_policy: Optional[bool] = None,
                  secrets_encryption_config: Optional['outputs.GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiSecretsEncryptionConfigResult'] = None):
@@ -38760,15 +39926,15 @@
     @property
     @pulumi.getter(name="serviceNodePortRange")
     def service_node_port_range(self) -> str:
         return pulumi.get(self, "service_node_port_range")
 
     @property
     @pulumi.getter(name="admissionConfiguration")
-    def admission_configuration(self) -> Optional[Mapping[str, Any]]:
+    def admission_configuration(self) -> Optional['outputs.GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationResult']:
         return pulumi.get(self, "admission_configuration")
 
     @property
     @pulumi.getter(name="alwaysPullImages")
     def always_pull_images(self) -> Optional[bool]:
         return pulumi.get(self, "always_pull_images")
 
@@ -38800,14 +39966,75 @@
     @property
     @pulumi.getter(name="secretsEncryptionConfig")
     def secrets_encryption_config(self) -> Optional['outputs.GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiSecretsEncryptionConfigResult']:
         return pulumi.get(self, "secrets_encryption_config")
 
 
 @pulumi.output_type
+class GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationResult(dict):
+    def __init__(__self__, *,
+                 plugins: Sequence['outputs.GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPluginResult'],
+                 api_version: Optional[str] = None,
+                 kind: Optional[str] = None):
+        pulumi.set(__self__, "plugins", plugins)
+        if api_version is not None:
+            pulumi.set(__self__, "api_version", api_version)
+        if kind is not None:
+            pulumi.set(__self__, "kind", kind)
+
+    @property
+    @pulumi.getter
+    def plugins(self) -> Sequence['outputs.GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPluginResult']:
+        return pulumi.get(self, "plugins")
+
+    @property
+    @pulumi.getter(name="apiVersion")
+    def api_version(self) -> Optional[str]:
+        return pulumi.get(self, "api_version")
+
+    @property
+    @pulumi.getter
+    def kind(self) -> Optional[str]:
+        return pulumi.get(self, "kind")
+
+
+@pulumi.output_type
+class GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAdmissionConfigurationPluginResult(dict):
+    def __init__(__self__, *,
+                 configuration: str,
+                 name: str,
+                 path: Optional[str] = None):
+        """
+        :param str name: The cluster template name (string)
+        """
+        pulumi.set(__self__, "configuration", configuration)
+        pulumi.set(__self__, "name", name)
+        if path is not None:
+            pulumi.set(__self__, "path", path)
+
+    @property
+    @pulumi.getter
+    def configuration(self) -> str:
+        return pulumi.get(self, "configuration")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        The cluster template name (string)
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def path(self) -> Optional[str]:
+        return pulumi.get(self, "path")
+
+
+@pulumi.output_type
 class GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLogResult(dict):
     def __init__(__self__, *,
                  configuration: 'outputs.GetClusterTemplateTemplateRevisionClusterConfigRkeConfigServicesKubeApiAuditLogConfigurationResult',
                  enabled: Optional[bool] = None):
         pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
@@ -39352,26 +40579,28 @@
         return pulumi.get(self, "windows_node_command")
 
 
 @pulumi.output_type
 class GetClusterV2RkeConfigResult(dict):
     def __init__(__self__, *,
                  etcd: 'outputs.GetClusterV2RkeConfigEtcdResult',
+                 machine_pool_defaults: Sequence['outputs.GetClusterV2RkeConfigMachinePoolDefaultResult'],
                  machine_pools: Sequence['outputs.GetClusterV2RkeConfigMachinePoolResult'],
                  machine_selector_configs: Sequence['outputs.GetClusterV2RkeConfigMachineSelectorConfigResult'],
                  additional_manifest: Optional[str] = None,
                  chart_values: Optional[str] = None,
                  etcd_snapshot_create: Optional['outputs.GetClusterV2RkeConfigEtcdSnapshotCreateResult'] = None,
                  etcd_snapshot_restore: Optional['outputs.GetClusterV2RkeConfigEtcdSnapshotRestoreResult'] = None,
                  local_auth_endpoint: Optional['outputs.GetClusterV2RkeConfigLocalAuthEndpointResult'] = None,
                  machine_global_config: Optional[str] = None,
                  registries: Optional['outputs.GetClusterV2RkeConfigRegistriesResult'] = None,
                  rotate_certificates: Optional['outputs.GetClusterV2RkeConfigRotateCertificatesResult'] = None,
                  upgrade_strategy: Optional['outputs.GetClusterV2RkeConfigUpgradeStrategyResult'] = None):
         pulumi.set(__self__, "etcd", etcd)
+        pulumi.set(__self__, "machine_pool_defaults", machine_pool_defaults)
         pulumi.set(__self__, "machine_pools", machine_pools)
         pulumi.set(__self__, "machine_selector_configs", machine_selector_configs)
         if additional_manifest is not None:
             pulumi.set(__self__, "additional_manifest", additional_manifest)
         if chart_values is not None:
             pulumi.set(__self__, "chart_values", chart_values)
         if etcd_snapshot_create is not None:
@@ -39391,14 +40620,19 @@
 
     @property
     @pulumi.getter
     def etcd(self) -> 'outputs.GetClusterV2RkeConfigEtcdResult':
         return pulumi.get(self, "etcd")
 
     @property
+    @pulumi.getter(name="machinePoolDefaults")
+    def machine_pool_defaults(self) -> Sequence['outputs.GetClusterV2RkeConfigMachinePoolDefaultResult']:
+        return pulumi.get(self, "machine_pool_defaults")
+
+    @property
     @pulumi.getter(name="machinePools")
     def machine_pools(self) -> Sequence['outputs.GetClusterV2RkeConfigMachinePoolResult']:
         return pulumi.get(self, "machine_pools")
 
     @property
     @pulumi.getter(name="machineSelectorConfigs")
     def machine_selector_configs(self) -> Sequence['outputs.GetClusterV2RkeConfigMachineSelectorConfigResult']:
@@ -39628,14 +40862,15 @@
                  machine_config: 'outputs.GetClusterV2RkeConfigMachinePoolMachineConfigResult',
                  machine_labels: Mapping[str, Any],
                  name: str,
                  cloud_credential_secret_name: Optional[str] = None,
                  control_plane_role: Optional[bool] = None,
                  drain_before_delete: Optional[bool] = None,
                  etcd_role: Optional[bool] = None,
+                 hostname_length_limit: Optional[int] = None,
                  max_unhealthy: Optional[str] = None,
                  node_drain_timeout: Optional[int] = None,
                  node_startup_timeout_seconds: Optional[int] = None,
                  paused: Optional[bool] = None,
                  quantity: Optional[int] = None,
                  rolling_update: Optional['outputs.GetClusterV2RkeConfigMachinePoolRollingUpdateResult'] = None,
                  taints: Optional[Sequence['outputs.GetClusterV2RkeConfigMachinePoolTaintResult']] = None,
@@ -39655,14 +40890,16 @@
             pulumi.set(__self__, "cloud_credential_secret_name", cloud_credential_secret_name)
         if control_plane_role is not None:
             pulumi.set(__self__, "control_plane_role", control_plane_role)
         if drain_before_delete is not None:
             pulumi.set(__self__, "drain_before_delete", drain_before_delete)
         if etcd_role is not None:
             pulumi.set(__self__, "etcd_role", etcd_role)
+        if hostname_length_limit is not None:
+            pulumi.set(__self__, "hostname_length_limit", hostname_length_limit)
         if max_unhealthy is not None:
             pulumi.set(__self__, "max_unhealthy", max_unhealthy)
         if node_drain_timeout is not None:
             pulumi.set(__self__, "node_drain_timeout", node_drain_timeout)
         if node_startup_timeout_seconds is not None:
             pulumi.set(__self__, "node_startup_timeout_seconds", node_startup_timeout_seconds)
         if paused is not None:
@@ -39728,14 +40965,19 @@
 
     @property
     @pulumi.getter(name="etcdRole")
     def etcd_role(self) -> Optional[bool]:
         return pulumi.get(self, "etcd_role")
 
     @property
+    @pulumi.getter(name="hostnameLengthLimit")
+    def hostname_length_limit(self) -> Optional[int]:
+        return pulumi.get(self, "hostname_length_limit")
+
+    @property
     @pulumi.getter(name="maxUnhealthy")
     def max_unhealthy(self) -> Optional[str]:
         return pulumi.get(self, "max_unhealthy")
 
     @property
     @pulumi.getter(name="nodeDrainTimeout")
     def node_drain_timeout(self) -> Optional[int]:
@@ -39779,14 +41021,27 @@
     @property
     @pulumi.getter(name="workerRole")
     def worker_role(self) -> Optional[bool]:
         return pulumi.get(self, "worker_role")
 
 
 @pulumi.output_type
+class GetClusterV2RkeConfigMachinePoolDefaultResult(dict):
+    def __init__(__self__, *,
+                 hostname_length_limit: Optional[int] = None):
+        if hostname_length_limit is not None:
+            pulumi.set(__self__, "hostname_length_limit", hostname_length_limit)
+
+    @property
+    @pulumi.getter(name="hostnameLengthLimit")
+    def hostname_length_limit(self) -> Optional[int]:
+        return pulumi.get(self, "hostname_length_limit")
+
+
+@pulumi.output_type
 class GetClusterV2RkeConfigMachinePoolMachineConfigResult(dict):
     def __init__(__self__, *,
                  kind: str,
                  name: str):
         """
         :param str name: The name of the Cluster v2 (string)
         """
```

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/pod_security_policy_template.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/pod_security_policy_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/project.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/project_alert_group.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/project_alert_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/project_alert_rule.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/project_alert_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/project_role_template_binding.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/project_role_template_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/provider.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/registry.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/role_tempalte.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/role_tempalte.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/role_template.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/role_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/secret.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/secret_v2.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/secret_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/setting.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/setting.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/storage_class_v2.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/storage_class_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/token.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2/user.py` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2.egg-info/PKG-INFO` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-rancher2
-Version: 5.1.0a1689400040
+Version: 5.1.0a1690482743
 Summary: A Pulumi package for creating and managing rancher2 resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rancher2
 Keywords: pulumi rancher2
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rancher2-5.1.0a1689400040/pulumi_rancher2.egg-info/SOURCES.txt` & `pulumi_rancher2-5.1.0a1690482743/pulumi_rancher2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 pulumi_rancher2/cluster_alter_rule.py
 pulumi_rancher2/cluster_driver.py
 pulumi_rancher2/cluster_role_template_binding.py
 pulumi_rancher2/cluster_sync.py
 pulumi_rancher2/cluster_template.py
 pulumi_rancher2/cluster_v2.py
 pulumi_rancher2/config_map_v2.py
+pulumi_rancher2/custom_user_token.py
 pulumi_rancher2/etcd_backup.py
 pulumi_rancher2/feature.py
 pulumi_rancher2/get_app.py
 pulumi_rancher2/get_catalog.py
 pulumi_rancher2/get_catalog_v2.py
 pulumi_rancher2/get_certificate.py
 pulumi_rancher2/get_cloud_credential.py
```

### Comparing `pulumi_rancher2-5.1.0a1689400040/setup.py` & `pulumi_rancher2-5.1.0a1690482743/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.1.0a1689400040"
-PLUGIN_VERSION = "5.1.0-alpha.1689400040+c8af607d"
+VERSION = "5.1.0a1690482743"
+PLUGIN_VERSION = "5.1.0-alpha.1690482743+2606b537"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'rancher2', PLUGIN_VERSION])
         except OSError as error:
```

