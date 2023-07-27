# Comparing `tmp/ionoscloud-dbaas-postgres-1.1.1.tar.gz` & `tmp/ionoscloud-dbaas-postgres-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ionoscloud-dbaas-postgres-1.1.1.tar", last modified: Mon Mar  6 18:14:39 2023, max compression
+gzip compressed data, was "ionoscloud-dbaas-postgres-1.2.0.tar", last modified: Thu Jul 27 12:29:00 2023, max compression
```

## Comparing `ionoscloud-dbaas-postgres-1.1.1.tar` & `ionoscloud-dbaas-postgres-1.2.0.tar`

### file list

```diff
@@ -1,63 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:14:39.530907 ionoscloud-dbaas-postgres-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-06 18:13:54.000000 ionoscloud-dbaas-postgres-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-03-06 18:14:39.530907 ionoscloud-dbaas-postgres-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:14:39.526907 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:14:39.526907 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21653 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api/backups_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46723 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api/clusters_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api/logs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api/metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api/restores_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17846 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:14:39.530907 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-03-06 18:13:54.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/backup_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/backup_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/backup_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_backup_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_backup_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_list_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_logs_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_logs_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/create_cluster_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/create_cluster_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/create_restore_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/day_of_the_week.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-06 18:13:54.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/pagination_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/patch_cluster_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/patch_cluster_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/postgres_version_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/postgres_version_list_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/resource_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/storage_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/synchronization_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/rest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3245 2023-03-06 18:13:54.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/test-driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:14:39.526907 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-03-06 18:14:39.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-03-06 18:14:39.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 18:14:39.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-06 18:14:39.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-06 18:14:39.000000 ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-06 18:14:39.530907 ionoscloud-dbaas-postgres-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-03-06 18:14:15.000000 ionoscloud-dbaas-postgres-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:29:00.756672 ionoscloud-dbaas-postgres-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 12:28:25.000000 ionoscloud-dbaas-postgres-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-07-27 12:29:00.756672 ionoscloud-dbaas-postgres-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12151 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:29:00.748672 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:29:00.752672 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21653 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/backups_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46723 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/clusters_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30708 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/databases_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/restores_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39711 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33068 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17846 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:29:00.756672 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-27 12:28:25.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/backup_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/backup_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/backup_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_backup_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_backup_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_list_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_logs_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_logs_instances_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-27 12:28:25.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_logs_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/create_cluster_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/create_cluster_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/create_restore_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/database_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/database_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/database_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/database_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/day_of_the_week.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/deprecated_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-07-27 12:28:25.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/pagination_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/patch_cluster_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/patch_cluster_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/patch_user_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/postgres_version_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/postgres_version_list_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/resource_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/storage_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/synchronization_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-27 12:28:46.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/user_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/user_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/user_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/user_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/users_patch_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/rest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3245 2023-07-27 12:28:25.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/test-driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:29:00.748672 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-07-27 12:29:00.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-27 12:29:00.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:29:00.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-27 12:29:00.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 12:29:00.000000 ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 12:29:00.756672 ionoscloud-dbaas-postgres-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-27 12:28:47.000000 ionoscloud-dbaas-postgres-1.2.0/setup.py
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/LICENSE` & `ionoscloud-dbaas-postgres-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/PKG-INFO` & `ionoscloud-dbaas-postgres-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionoscloud-dbaas-postgres
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python SDK for the Ionos DBaaS Postgres API
 Home-page: https://github.com/ionos-cloud/sdk-python-dbaas-postgres
 Author: Ionos Cloud
 Author-email: sdk@cloud.ionos.com
 Keywords: OpenAPI,OpenAPI-Generator,IONOS DBaaS PostgreSQL REST API
 Classifier: Natural Language :: English
 Classifier: Environment :: Web Environment
@@ -171,18 +171,27 @@
 | ClustersApi | [**cluster_postgres_versions_get**](docs/api/ClustersApi.md#cluster_postgres_versions_get) | **GET** /clusters/{clusterId}/postgresversions | List PostgreSQL versions |
 | ClustersApi | [**clusters_delete**](docs/api/ClustersApi.md#clusters_delete) | **DELETE** /clusters/{clusterId} | Delete a cluster |
 | ClustersApi | [**clusters_find_by_id**](docs/api/ClustersApi.md#clusters_find_by_id) | **GET** /clusters/{clusterId} | Fetch a cluster |
 | ClustersApi | [**clusters_get**](docs/api/ClustersApi.md#clusters_get) | **GET** /clusters | List clusters |
 | ClustersApi | [**clusters_patch**](docs/api/ClustersApi.md#clusters_patch) | **PATCH** /clusters/{clusterId} | Patch a cluster |
 | ClustersApi | [**clusters_post**](docs/api/ClustersApi.md#clusters_post) | **POST** /clusters | Create a cluster |
 | ClustersApi | [**postgres_versions_get**](docs/api/ClustersApi.md#postgres_versions_get) | **GET** /clusters/postgresversions | List PostgreSQL versions |
+| DatabasesApi | [**databases_delete**](docs/api/DatabasesApi.md#databases_delete) | **DELETE** /clusters/{clusterId}/databases/{databasename} | Delete database |
+| DatabasesApi | [**databases_get**](docs/api/DatabasesApi.md#databases_get) | **GET** /clusters/{clusterId}/databases/{databasename} | Get database |
+| DatabasesApi | [**databases_list**](docs/api/DatabasesApi.md#databases_list) | **GET** /clusters/{clusterId}/databases | List databases |
+| DatabasesApi | [**databases_post**](docs/api/DatabasesApi.md#databases_post) | **POST** /clusters/{clusterId}/databases | Create a database |
 | LogsApi | [**cluster_logs_get**](docs/api/LogsApi.md#cluster_logs_get) | **GET** /clusters/{clusterId}/logs | Get logs of your cluster |
 | MetadataApi | [**infos_version_get**](docs/api/MetadataApi.md#infos_version_get) | **GET** /infos/version | Get the current API version |
 | MetadataApi | [**infos_versions_get**](docs/api/MetadataApi.md#infos_versions_get) | **GET** /infos/versions | Fetch all API versions |
 | RestoresApi | [**cluster_restore_post**](docs/api/RestoresApi.md#cluster_restore_post) | **POST** /clusters/{clusterId}/restore | In-place restore of a cluster |
+| UsersApi | [**users_delete**](docs/api/UsersApi.md#users_delete) | **DELETE** /clusters/{clusterId}/users/{username} | Delete user |
+| UsersApi | [**users_get**](docs/api/UsersApi.md#users_get) | **GET** /clusters/{clusterId}/users/{username} | Get user |
+| UsersApi | [**users_list**](docs/api/UsersApi.md#users_list) | **GET** /clusters/{clusterId}/users | List users |
+| UsersApi | [**users_patch**](docs/api/UsersApi.md#users_patch) | **PATCH** /clusters/{clusterId}/users/{username} | Patch user |
+| UsersApi | [**users_post**](docs/api/UsersApi.md#users_post) | **POST** /clusters/{clusterId}/users | Create a user |
 
 </details>
 
 ## Documentation For Models
 
 All URIs are relative to *https://api.ionos.com/databases/postgresql*
 <details >
@@ -194,35 +203,51 @@
  - [ClusterBackup](docs/models/ClusterBackup)
  - [ClusterBackupList](docs/models/ClusterBackupList)
  - [ClusterBackupListAllOf](docs/models/ClusterBackupListAllOf)
  - [ClusterList](docs/models/ClusterList)
  - [ClusterListAllOf](docs/models/ClusterListAllOf)
  - [ClusterLogs](docs/models/ClusterLogs)
  - [ClusterLogsInstances](docs/models/ClusterLogsInstances)
- - [ClusterLogsMessages](docs/models/ClusterLogsMessages)
+ - [ClusterLogsInstancesMessages](docs/models/ClusterLogsInstancesMessages)
+ - [ClusterMetadata](docs/models/ClusterMetadata)
  - [ClusterProperties](docs/models/ClusterProperties)
  - [ClusterResponse](docs/models/ClusterResponse)
  - [Connection](docs/models/Connection)
  - [CreateClusterProperties](docs/models/CreateClusterProperties)
  - [CreateClusterRequest](docs/models/CreateClusterRequest)
  - [CreateRestoreRequest](docs/models/CreateRestoreRequest)
  - [DBUser](docs/models/DBUser)
+ - [Database](docs/models/Database)
+ - [DatabaseItems](docs/models/DatabaseItems)
+ - [DatabaseList](docs/models/DatabaseList)
+ - [DatabaseProperties](docs/models/DatabaseProperties)
+ - [DatabaseResource](docs/models/DatabaseResource)
  - [DayOfTheWeek](docs/models/DayOfTheWeek)
+ - [DeprecatedPagination](docs/models/DeprecatedPagination)
  - [ErrorMessage](docs/models/ErrorMessage)
  - [ErrorResponse](docs/models/ErrorResponse)
  - [MaintenanceWindow](docs/models/MaintenanceWindow)
  - [Metadata](docs/models/Metadata)
  - [Pagination](docs/models/Pagination)
  - [PaginationLinks](docs/models/PaginationLinks)
  - [PatchClusterProperties](docs/models/PatchClusterProperties)
  - [PatchClusterRequest](docs/models/PatchClusterRequest)
+ - [PatchUserProperties](docs/models/PatchUserProperties)
  - [PostgresVersionList](docs/models/PostgresVersionList)
  - [PostgresVersionListData](docs/models/PostgresVersionListData)
+ - [Resource](docs/models/Resource)
+ - [ResourceMetadata](docs/models/ResourceMetadata)
  - [ResourceType](docs/models/ResourceType)
  - [State](docs/models/State)
  - [StorageType](docs/models/StorageType)
  - [SynchronizationMode](docs/models/SynchronizationMode)
+ - [User](docs/models/User)
+ - [UserItems](docs/models/UserItems)
+ - [UserList](docs/models/UserList)
+ - [UserProperties](docs/models/UserProperties)
+ - [UserResource](docs/models/UserResource)
+ - [UsersPatchRequest](docs/models/UsersPatchRequest)
 
 
 [[Back to API list]](#documentation-for-api-endpoints) [[Back to Model list]](#documentation-for-models)
 
 </details>
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/README.md` & `ionoscloud-dbaas-postgres-1.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -150,18 +150,27 @@
 | ClustersApi | [**cluster_postgres_versions_get**](docs/api/ClustersApi.md#cluster_postgres_versions_get) | **GET** /clusters/{clusterId}/postgresversions | List PostgreSQL versions |
 | ClustersApi | [**clusters_delete**](docs/api/ClustersApi.md#clusters_delete) | **DELETE** /clusters/{clusterId} | Delete a cluster |
 | ClustersApi | [**clusters_find_by_id**](docs/api/ClustersApi.md#clusters_find_by_id) | **GET** /clusters/{clusterId} | Fetch a cluster |
 | ClustersApi | [**clusters_get**](docs/api/ClustersApi.md#clusters_get) | **GET** /clusters | List clusters |
 | ClustersApi | [**clusters_patch**](docs/api/ClustersApi.md#clusters_patch) | **PATCH** /clusters/{clusterId} | Patch a cluster |
 | ClustersApi | [**clusters_post**](docs/api/ClustersApi.md#clusters_post) | **POST** /clusters | Create a cluster |
 | ClustersApi | [**postgres_versions_get**](docs/api/ClustersApi.md#postgres_versions_get) | **GET** /clusters/postgresversions | List PostgreSQL versions |
+| DatabasesApi | [**databases_delete**](docs/api/DatabasesApi.md#databases_delete) | **DELETE** /clusters/{clusterId}/databases/{databasename} | Delete database |
+| DatabasesApi | [**databases_get**](docs/api/DatabasesApi.md#databases_get) | **GET** /clusters/{clusterId}/databases/{databasename} | Get database |
+| DatabasesApi | [**databases_list**](docs/api/DatabasesApi.md#databases_list) | **GET** /clusters/{clusterId}/databases | List databases |
+| DatabasesApi | [**databases_post**](docs/api/DatabasesApi.md#databases_post) | **POST** /clusters/{clusterId}/databases | Create a database |
 | LogsApi | [**cluster_logs_get**](docs/api/LogsApi.md#cluster_logs_get) | **GET** /clusters/{clusterId}/logs | Get logs of your cluster |
 | MetadataApi | [**infos_version_get**](docs/api/MetadataApi.md#infos_version_get) | **GET** /infos/version | Get the current API version |
 | MetadataApi | [**infos_versions_get**](docs/api/MetadataApi.md#infos_versions_get) | **GET** /infos/versions | Fetch all API versions |
 | RestoresApi | [**cluster_restore_post**](docs/api/RestoresApi.md#cluster_restore_post) | **POST** /clusters/{clusterId}/restore | In-place restore of a cluster |
+| UsersApi | [**users_delete**](docs/api/UsersApi.md#users_delete) | **DELETE** /clusters/{clusterId}/users/{username} | Delete user |
+| UsersApi | [**users_get**](docs/api/UsersApi.md#users_get) | **GET** /clusters/{clusterId}/users/{username} | Get user |
+| UsersApi | [**users_list**](docs/api/UsersApi.md#users_list) | **GET** /clusters/{clusterId}/users | List users |
+| UsersApi | [**users_patch**](docs/api/UsersApi.md#users_patch) | **PATCH** /clusters/{clusterId}/users/{username} | Patch user |
+| UsersApi | [**users_post**](docs/api/UsersApi.md#users_post) | **POST** /clusters/{clusterId}/users | Create a user |
 
 </details>
 
 ## Documentation For Models
 
 All URIs are relative to *https://api.ionos.com/databases/postgresql*
 <details >
@@ -173,35 +182,51 @@
  - [ClusterBackup](docs/models/ClusterBackup)
  - [ClusterBackupList](docs/models/ClusterBackupList)
  - [ClusterBackupListAllOf](docs/models/ClusterBackupListAllOf)
  - [ClusterList](docs/models/ClusterList)
  - [ClusterListAllOf](docs/models/ClusterListAllOf)
  - [ClusterLogs](docs/models/ClusterLogs)
  - [ClusterLogsInstances](docs/models/ClusterLogsInstances)
- - [ClusterLogsMessages](docs/models/ClusterLogsMessages)
+ - [ClusterLogsInstancesMessages](docs/models/ClusterLogsInstancesMessages)
+ - [ClusterMetadata](docs/models/ClusterMetadata)
  - [ClusterProperties](docs/models/ClusterProperties)
  - [ClusterResponse](docs/models/ClusterResponse)
  - [Connection](docs/models/Connection)
  - [CreateClusterProperties](docs/models/CreateClusterProperties)
  - [CreateClusterRequest](docs/models/CreateClusterRequest)
  - [CreateRestoreRequest](docs/models/CreateRestoreRequest)
  - [DBUser](docs/models/DBUser)
+ - [Database](docs/models/Database)
+ - [DatabaseItems](docs/models/DatabaseItems)
+ - [DatabaseList](docs/models/DatabaseList)
+ - [DatabaseProperties](docs/models/DatabaseProperties)
+ - [DatabaseResource](docs/models/DatabaseResource)
  - [DayOfTheWeek](docs/models/DayOfTheWeek)
+ - [DeprecatedPagination](docs/models/DeprecatedPagination)
  - [ErrorMessage](docs/models/ErrorMessage)
  - [ErrorResponse](docs/models/ErrorResponse)
  - [MaintenanceWindow](docs/models/MaintenanceWindow)
  - [Metadata](docs/models/Metadata)
  - [Pagination](docs/models/Pagination)
  - [PaginationLinks](docs/models/PaginationLinks)
  - [PatchClusterProperties](docs/models/PatchClusterProperties)
  - [PatchClusterRequest](docs/models/PatchClusterRequest)
+ - [PatchUserProperties](docs/models/PatchUserProperties)
  - [PostgresVersionList](docs/models/PostgresVersionList)
  - [PostgresVersionListData](docs/models/PostgresVersionListData)
+ - [Resource](docs/models/Resource)
+ - [ResourceMetadata](docs/models/ResourceMetadata)
  - [ResourceType](docs/models/ResourceType)
  - [State](docs/models/State)
  - [StorageType](docs/models/StorageType)
  - [SynchronizationMode](docs/models/SynchronizationMode)
+ - [User](docs/models/User)
+ - [UserItems](docs/models/UserItems)
+ - [UserList](docs/models/UserList)
+ - [UserProperties](docs/models/UserProperties)
+ - [UserResource](docs/models/UserResource)
+ - [UsersPatchRequest](docs/models/UsersPatchRequest)
 
 
 [[Back to API list]](#documentation-for-api-endpoints) [[Back to Model list]](#documentation-for-models)
 
 </details>
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/__init__.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,62 +8,79 @@
     An enterprise-grade Database is provided as a Service (DBaaS) solution that can be managed through a browser-based \"Data Center Designer\" (DCD) tool or via an easy to use API.  The API allows you to create additional PostgreSQL database clusters or modify existing ones. It is designed to allow users to leverage the same power and flexibility found within the DCD visual tool. Both tools are consistent with their concepts and lend well to making the experience smooth and intuitive.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
-__version__ = "1.1.1"
+__version__ = "1.2.0"
 
 # import apis into sdk package
 from ionoscloud_dbaas_postgres.api.backups_api import BackupsApi
 from ionoscloud_dbaas_postgres.api.clusters_api import ClustersApi
+from ionoscloud_dbaas_postgres.api.databases_api import DatabasesApi
 from ionoscloud_dbaas_postgres.api.logs_api import LogsApi
 from ionoscloud_dbaas_postgres.api.metadata_api import MetadataApi
 from ionoscloud_dbaas_postgres.api.restores_api import RestoresApi
+from ionoscloud_dbaas_postgres.api.users_api import UsersApi
 
 # import ApiClient
+from ionoscloud_dbaas_postgres.api_response import ApiResponse
 from ionoscloud_dbaas_postgres.api_client import ApiClient
 from ionoscloud_dbaas_postgres.configuration import Configuration
 from ionoscloud_dbaas_postgres.exceptions import OpenApiException
 from ionoscloud_dbaas_postgres.exceptions import ApiTypeError
 from ionoscloud_dbaas_postgres.exceptions import ApiValueError
 from ionoscloud_dbaas_postgres.exceptions import ApiKeyError
 from ionoscloud_dbaas_postgres.exceptions import ApiAttributeError
 from ionoscloud_dbaas_postgres.exceptions import ApiException
+
 # import models into sdk package
 from ionoscloud_dbaas_postgres.models.api_version import APIVersion
 from ionoscloud_dbaas_postgres.models.backup_metadata import BackupMetadata
 from ionoscloud_dbaas_postgres.models.backup_response import BackupResponse
 from ionoscloud_dbaas_postgres.models.cluster_backup import ClusterBackup
 from ionoscloud_dbaas_postgres.models.cluster_backup_list import ClusterBackupList
 from ionoscloud_dbaas_postgres.models.cluster_backup_list_all_of import ClusterBackupListAllOf
 from ionoscloud_dbaas_postgres.models.cluster_list import ClusterList
 from ionoscloud_dbaas_postgres.models.cluster_list_all_of import ClusterListAllOf
 from ionoscloud_dbaas_postgres.models.cluster_logs import ClusterLogs
 from ionoscloud_dbaas_postgres.models.cluster_logs_instances import ClusterLogsInstances
-from ionoscloud_dbaas_postgres.models.cluster_logs_messages import ClusterLogsMessages
+from ionoscloud_dbaas_postgres.models.cluster_logs_instances_messages import ClusterLogsInstancesMessages
+from ionoscloud_dbaas_postgres.models.cluster_metadata import ClusterMetadata
 from ionoscloud_dbaas_postgres.models.cluster_properties import ClusterProperties
 from ionoscloud_dbaas_postgres.models.cluster_response import ClusterResponse
 from ionoscloud_dbaas_postgres.models.connection import Connection
 from ionoscloud_dbaas_postgres.models.create_cluster_properties import CreateClusterProperties
 from ionoscloud_dbaas_postgres.models.create_cluster_request import CreateClusterRequest
 from ionoscloud_dbaas_postgres.models.create_restore_request import CreateRestoreRequest
 from ionoscloud_dbaas_postgres.models.db_user import DBUser
+from ionoscloud_dbaas_postgres.models.database import Database
+from ionoscloud_dbaas_postgres.models.database_items import DatabaseItems
+from ionoscloud_dbaas_postgres.models.database_list import DatabaseList
+from ionoscloud_dbaas_postgres.models.database_properties import DatabaseProperties
+from ionoscloud_dbaas_postgres.models.database_resource import DatabaseResource
 from ionoscloud_dbaas_postgres.models.day_of_the_week import DayOfTheWeek
+from ionoscloud_dbaas_postgres.models.deprecated_pagination import DeprecatedPagination
 from ionoscloud_dbaas_postgres.models.error_message import ErrorMessage
 from ionoscloud_dbaas_postgres.models.error_response import ErrorResponse
 from ionoscloud_dbaas_postgres.models.maintenance_window import MaintenanceWindow
 from ionoscloud_dbaas_postgres.models.metadata import Metadata
 from ionoscloud_dbaas_postgres.models.pagination import Pagination
 from ionoscloud_dbaas_postgres.models.pagination_links import PaginationLinks
 from ionoscloud_dbaas_postgres.models.patch_cluster_properties import PatchClusterProperties
 from ionoscloud_dbaas_postgres.models.patch_cluster_request import PatchClusterRequest
+from ionoscloud_dbaas_postgres.models.patch_user_properties import PatchUserProperties
 from ionoscloud_dbaas_postgres.models.postgres_version_list import PostgresVersionList
 from ionoscloud_dbaas_postgres.models.postgres_version_list_data import PostgresVersionListData
+from ionoscloud_dbaas_postgres.models.resource import Resource
+from ionoscloud_dbaas_postgres.models.resource_metadata import ResourceMetadata
 from ionoscloud_dbaas_postgres.models.resource_type import ResourceType
 from ionoscloud_dbaas_postgres.models.state import State
 from ionoscloud_dbaas_postgres.models.storage_type import StorageType
 from ionoscloud_dbaas_postgres.models.synchronization_mode import SynchronizationMode
-
+from ionoscloud_dbaas_postgres.models.user import User
+from ionoscloud_dbaas_postgres.models.user_items import UserItems
+from ionoscloud_dbaas_postgres.models.user_list import UserList
+from ionoscloud_dbaas_postgres.models.user_properties import UserProperties
+from ionoscloud_dbaas_postgres.models.user_resource import UserResource
+from ionoscloud_dbaas_postgres.models.users_patch_request import UsersPatchRequest
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api/backups_api.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/backups_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api/clusters_api.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/clusters_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api/logs_api.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api/metadata_api.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api/restores_api.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api/restores_api.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/api_client.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'ionos-cloud-sdk-python/1.1.1'
+        self.user_agent = 'ionos-cloud-sdk-python/1.2.0'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -805,18 +805,21 @@
             check_response = fn_check(resp)
 
             if check_response:
                 break
 
             current_time = time.time()
             if timeout and current_time > timeout:
-                raise ApiTimeout(
-                    message='Timed out waiting for request {0}.'.format(resp['requestId']),
-                    request_id=resp['requestId']
-                )
+                if type(resp) == dict and resp.get('requestId'):
+                    raise ApiTimeout(
+                        message='Timed out waiting for request {0}.'.format(resp['requestId']),
+                        request_id=resp['requestId'],
+                    )
+                else:
+                    raise ApiTimeout(message='Timeout reached')
 
             if current_time > next_increase:
                 wait_period *= 2
                 next_increase = time.time() + wait_period * scaleup
                 scaleup *= 2
 
             logger.info("Sleeping for %i seconds...", wait_period)
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/configuration.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.1.1".\
+               "SDK Package Version: 1.2.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/exceptions.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/exceptions.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/__init__.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,43 +7,57 @@
     An enterprise-grade Database is provided as a Service (DBaaS) solution that can be managed through a browser-based \"Data Center Designer\" (DCD) tool or via an easy to use API.  The API allows you to create additional PostgreSQL database clusters or modify existing ones. It is designed to allow users to leverage the same power and flexibility found within the DCD visual tool. Both tools are consistent with their concepts and lend well to making the experience smooth and intuitive.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
-from __future__ import absolute_import
-
 # import models into model package
 from ionoscloud_dbaas_postgres.models.api_version import APIVersion
 from ionoscloud_dbaas_postgres.models.backup_metadata import BackupMetadata
 from ionoscloud_dbaas_postgres.models.backup_response import BackupResponse
 from ionoscloud_dbaas_postgres.models.cluster_backup import ClusterBackup
 from ionoscloud_dbaas_postgres.models.cluster_backup_list import ClusterBackupList
 from ionoscloud_dbaas_postgres.models.cluster_backup_list_all_of import ClusterBackupListAllOf
 from ionoscloud_dbaas_postgres.models.cluster_list import ClusterList
 from ionoscloud_dbaas_postgres.models.cluster_list_all_of import ClusterListAllOf
 from ionoscloud_dbaas_postgres.models.cluster_logs import ClusterLogs
 from ionoscloud_dbaas_postgres.models.cluster_logs_instances import ClusterLogsInstances
-from ionoscloud_dbaas_postgres.models.cluster_logs_messages import ClusterLogsMessages
+from ionoscloud_dbaas_postgres.models.cluster_logs_instances_messages import ClusterLogsInstancesMessages
+from ionoscloud_dbaas_postgres.models.cluster_metadata import ClusterMetadata
 from ionoscloud_dbaas_postgres.models.cluster_properties import ClusterProperties
 from ionoscloud_dbaas_postgres.models.cluster_response import ClusterResponse
 from ionoscloud_dbaas_postgres.models.connection import Connection
 from ionoscloud_dbaas_postgres.models.create_cluster_properties import CreateClusterProperties
 from ionoscloud_dbaas_postgres.models.create_cluster_request import CreateClusterRequest
 from ionoscloud_dbaas_postgres.models.create_restore_request import CreateRestoreRequest
 from ionoscloud_dbaas_postgres.models.db_user import DBUser
+from ionoscloud_dbaas_postgres.models.database import Database
+from ionoscloud_dbaas_postgres.models.database_items import DatabaseItems
+from ionoscloud_dbaas_postgres.models.database_list import DatabaseList
+from ionoscloud_dbaas_postgres.models.database_properties import DatabaseProperties
+from ionoscloud_dbaas_postgres.models.database_resource import DatabaseResource
 from ionoscloud_dbaas_postgres.models.day_of_the_week import DayOfTheWeek
+from ionoscloud_dbaas_postgres.models.deprecated_pagination import DeprecatedPagination
 from ionoscloud_dbaas_postgres.models.error_message import ErrorMessage
 from ionoscloud_dbaas_postgres.models.error_response import ErrorResponse
 from ionoscloud_dbaas_postgres.models.maintenance_window import MaintenanceWindow
 from ionoscloud_dbaas_postgres.models.metadata import Metadata
 from ionoscloud_dbaas_postgres.models.pagination import Pagination
 from ionoscloud_dbaas_postgres.models.pagination_links import PaginationLinks
 from ionoscloud_dbaas_postgres.models.patch_cluster_properties import PatchClusterProperties
 from ionoscloud_dbaas_postgres.models.patch_cluster_request import PatchClusterRequest
+from ionoscloud_dbaas_postgres.models.patch_user_properties import PatchUserProperties
 from ionoscloud_dbaas_postgres.models.postgres_version_list import PostgresVersionList
 from ionoscloud_dbaas_postgres.models.postgres_version_list_data import PostgresVersionListData
+from ionoscloud_dbaas_postgres.models.resource import Resource
+from ionoscloud_dbaas_postgres.models.resource_metadata import ResourceMetadata
 from ionoscloud_dbaas_postgres.models.resource_type import ResourceType
 from ionoscloud_dbaas_postgres.models.state import State
 from ionoscloud_dbaas_postgres.models.storage_type import StorageType
 from ionoscloud_dbaas_postgres.models.synchronization_mode import SynchronizationMode
+from ionoscloud_dbaas_postgres.models.user import User
+from ionoscloud_dbaas_postgres.models.user_items import UserItems
+from ionoscloud_dbaas_postgres.models.user_list import UserList
+from ionoscloud_dbaas_postgres.models.user_properties import UserProperties
+from ionoscloud_dbaas_postgres.models.user_resource import UserResource
+from ionoscloud_dbaas_postgres.models.users_patch_request import UsersPatchRequest
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/api_version.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/api_version.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/backup_location.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/backup_location.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/backup_metadata.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/backup_metadata.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/backup_response.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/backup_response.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_backup.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_backup.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_backup_list.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_backup_list.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_backup_list_all_of.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_backup_list_all_of.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_list.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_list.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_list_all_of.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_list_all_of.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_logs.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_logs.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_logs_instances.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_logs_instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
         'name': 'str',
 
-        'messages': 'list[ClusterLogsMessages]',
+        'messages': 'list[ClusterLogsInstancesMessages]',
     }
 
     attribute_map = {
 
         'name': 'name',
 
         'messages': 'messages',
@@ -87,25 +87,25 @@
 
     @property
     def messages(self):
         """Gets the messages of this ClusterLogsInstances.  # noqa: E501
 
 
         :return: The messages of this ClusterLogsInstances.  # noqa: E501
-        :rtype: list[ClusterLogsMessages]
+        :rtype: list[ClusterLogsInstancesMessages]
         """
         return self._messages
 
     @messages.setter
     def messages(self, messages):
         """Sets the messages of this ClusterLogsInstances.
 
 
         :param messages: The messages of this ClusterLogsInstances.  # noqa: E501
-        :type messages: list[ClusterLogsMessages]
+        :type messages: list[ClusterLogsInstancesMessages]
         """
 
         self._messages = messages
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_logs_messages.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_logs_messages.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_properties.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/cluster_response.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     """
     openapi_types = {
 
         'type': 'ResourceType',
 
         'id': 'str',
 
-        'metadata': 'Metadata',
+        'metadata': 'ClusterMetadata',
 
         'properties': 'ClusterProperties',
     }
 
     attribute_map = {
 
         'type': 'type',
@@ -122,25 +122,25 @@
 
     @property
     def metadata(self):
         """Gets the metadata of this ClusterResponse.  # noqa: E501
 
 
         :return: The metadata of this ClusterResponse.  # noqa: E501
-        :rtype: Metadata
+        :rtype: ClusterMetadata
         """
         return self._metadata
 
     @metadata.setter
     def metadata(self, metadata):
         """Sets the metadata of this ClusterResponse.
 
 
         :param metadata: The metadata of this ClusterResponse.  # noqa: E501
-        :type metadata: Metadata
+        :type metadata: ClusterMetadata
         """
 
         self._metadata = metadata
 
     @property
     def properties(self):
         """Gets the properties of this ClusterResponse.  # noqa: E501
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/connection.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/connection.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/create_cluster_properties.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/create_cluster_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/create_cluster_request.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/create_cluster_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'metadata': 'Metadata',
+        'metadata': 'ClusterMetadata',
 
         'properties': 'CreateClusterProperties',
     }
 
     attribute_map = {
 
         'metadata': 'metadata',
@@ -64,25 +64,25 @@
 
     @property
     def metadata(self):
         """Gets the metadata of this CreateClusterRequest.  # noqa: E501
 
 
         :return: The metadata of this CreateClusterRequest.  # noqa: E501
-        :rtype: Metadata
+        :rtype: ClusterMetadata
         """
         return self._metadata
 
     @metadata.setter
     def metadata(self, metadata):
         """Sets the metadata of this CreateClusterRequest.
 
 
         :param metadata: The metadata of this CreateClusterRequest.  # noqa: E501
-        :type metadata: Metadata
+        :type metadata: ClusterMetadata
         """
 
         self._metadata = metadata
 
     @property
     def properties(self):
         """Gets the properties of this CreateClusterRequest.  # noqa: E501
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/create_restore_request.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/create_restore_request.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/day_of_the_week.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/day_of_the_week.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    SUNDAY = "Sunday"
-    MONDAY = "Monday"
-    TUESDAY = "Tuesday"
-    WEDNESDAY = "Wednesday"
-    THURSDAY = "Thursday"
-    FRIDAY = "Friday"
-    SATURDAY = "Saturday"
+    SUNDAY = 'Sunday'
+    MONDAY = 'Monday'
+    TUESDAY = 'Tuesday'
+    WEDNESDAY = 'Wednesday'
+    THURSDAY = 'Thursday'
+    FRIDAY = 'Friday'
+    SATURDAY = 'Saturday'
 
     allowable_values = [SUNDAY, MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/db_user.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/db_user.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/error_message.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/error_message.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/error_response.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/error_response.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/location.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/location.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/maintenance_window.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/metadata.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/cluster_metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ionoscloud_dbaas_postgres.configuration import Configuration
 
 
-class Metadata(object):
+class ClusterMetadata(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -63,15 +63,15 @@
 
         'last_modified_by_user_id': 'lastModifiedByUserId',
 
         'state': 'state',
     }
 
     def __init__(self, created_date=None, created_by=None, created_by_user_id=None, last_modified_date=None, last_modified_by=None, last_modified_by_user_id=None, state=None, local_vars_configuration=None):  # noqa: E501
-        """Metadata - a model defined in OpenAPI"""  # noqa: E501
+        """ClusterMetadata - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._created_date = None
         self._created_by = None
         self._created_by_user_id = None
@@ -95,158 +95,158 @@
             self.last_modified_by_user_id = last_modified_by_user_id
         if state is not None:
             self.state = state
 
 
     @property
     def created_date(self):
-        """Gets the created_date of this Metadata.  # noqa: E501
+        """Gets the created_date of this ClusterMetadata.  # noqa: E501
 
         The ISO 8601 creation timestamp.  # noqa: E501
 
-        :return: The created_date of this Metadata.  # noqa: E501
+        :return: The created_date of this ClusterMetadata.  # noqa: E501
         :rtype: datetime
         """
         return self._created_date
 
     @created_date.setter
     def created_date(self, created_date):
-        """Sets the created_date of this Metadata.
+        """Sets the created_date of this ClusterMetadata.
 
         The ISO 8601 creation timestamp.  # noqa: E501
 
-        :param created_date: The created_date of this Metadata.  # noqa: E501
+        :param created_date: The created_date of this ClusterMetadata.  # noqa: E501
         :type created_date: datetime
         """
 
         self._created_date = created_date
 
     @property
     def created_by(self):
-        """Gets the created_by of this Metadata.  # noqa: E501
+        """Gets the created_by of this ClusterMetadata.  # noqa: E501
 
 
-        :return: The created_by of this Metadata.  # noqa: E501
+        :return: The created_by of this ClusterMetadata.  # noqa: E501
         :rtype: str
         """
         return self._created_by
 
     @created_by.setter
     def created_by(self, created_by):
-        """Sets the created_by of this Metadata.
+        """Sets the created_by of this ClusterMetadata.
 
 
-        :param created_by: The created_by of this Metadata.  # noqa: E501
+        :param created_by: The created_by of this ClusterMetadata.  # noqa: E501
         :type created_by: str
         """
 
         self._created_by = created_by
 
     @property
     def created_by_user_id(self):
-        """Gets the created_by_user_id of this Metadata.  # noqa: E501
+        """Gets the created_by_user_id of this ClusterMetadata.  # noqa: E501
 
 
-        :return: The created_by_user_id of this Metadata.  # noqa: E501
+        :return: The created_by_user_id of this ClusterMetadata.  # noqa: E501
         :rtype: str
         """
         return self._created_by_user_id
 
     @created_by_user_id.setter
     def created_by_user_id(self, created_by_user_id):
-        """Sets the created_by_user_id of this Metadata.
+        """Sets the created_by_user_id of this ClusterMetadata.
 
 
-        :param created_by_user_id: The created_by_user_id of this Metadata.  # noqa: E501
+        :param created_by_user_id: The created_by_user_id of this ClusterMetadata.  # noqa: E501
         :type created_by_user_id: str
         """
 
         self._created_by_user_id = created_by_user_id
 
     @property
     def last_modified_date(self):
-        """Gets the last_modified_date of this Metadata.  # noqa: E501
+        """Gets the last_modified_date of this ClusterMetadata.  # noqa: E501
 
         The ISO 8601 modified timestamp.  # noqa: E501
 
-        :return: The last_modified_date of this Metadata.  # noqa: E501
+        :return: The last_modified_date of this ClusterMetadata.  # noqa: E501
         :rtype: datetime
         """
         return self._last_modified_date
 
     @last_modified_date.setter
     def last_modified_date(self, last_modified_date):
-        """Sets the last_modified_date of this Metadata.
+        """Sets the last_modified_date of this ClusterMetadata.
 
         The ISO 8601 modified timestamp.  # noqa: E501
 
-        :param last_modified_date: The last_modified_date of this Metadata.  # noqa: E501
+        :param last_modified_date: The last_modified_date of this ClusterMetadata.  # noqa: E501
         :type last_modified_date: datetime
         """
 
         self._last_modified_date = last_modified_date
 
     @property
     def last_modified_by(self):
-        """Gets the last_modified_by of this Metadata.  # noqa: E501
+        """Gets the last_modified_by of this ClusterMetadata.  # noqa: E501
 
 
-        :return: The last_modified_by of this Metadata.  # noqa: E501
+        :return: The last_modified_by of this ClusterMetadata.  # noqa: E501
         :rtype: str
         """
         return self._last_modified_by
 
     @last_modified_by.setter
     def last_modified_by(self, last_modified_by):
-        """Sets the last_modified_by of this Metadata.
+        """Sets the last_modified_by of this ClusterMetadata.
 
 
-        :param last_modified_by: The last_modified_by of this Metadata.  # noqa: E501
+        :param last_modified_by: The last_modified_by of this ClusterMetadata.  # noqa: E501
         :type last_modified_by: str
         """
 
         self._last_modified_by = last_modified_by
 
     @property
     def last_modified_by_user_id(self):
-        """Gets the last_modified_by_user_id of this Metadata.  # noqa: E501
+        """Gets the last_modified_by_user_id of this ClusterMetadata.  # noqa: E501
 
 
-        :return: The last_modified_by_user_id of this Metadata.  # noqa: E501
+        :return: The last_modified_by_user_id of this ClusterMetadata.  # noqa: E501
         :rtype: str
         """
         return self._last_modified_by_user_id
 
     @last_modified_by_user_id.setter
     def last_modified_by_user_id(self, last_modified_by_user_id):
-        """Sets the last_modified_by_user_id of this Metadata.
+        """Sets the last_modified_by_user_id of this ClusterMetadata.
 
 
-        :param last_modified_by_user_id: The last_modified_by_user_id of this Metadata.  # noqa: E501
+        :param last_modified_by_user_id: The last_modified_by_user_id of this ClusterMetadata.  # noqa: E501
         :type last_modified_by_user_id: str
         """
 
         self._last_modified_by_user_id = last_modified_by_user_id
 
     @property
     def state(self):
-        """Gets the state of this Metadata.  # noqa: E501
+        """Gets the state of this ClusterMetadata.  # noqa: E501
 
 
-        :return: The state of this Metadata.  # noqa: E501
+        :return: The state of this ClusterMetadata.  # noqa: E501
         :rtype: State
         """
         return self._state
 
     @state.setter
     def state(self, state):
-        """Sets the state of this Metadata.
+        """Sets the state of this ClusterMetadata.
 
 
-        :param state: The state of this Metadata.  # noqa: E501
+        :param state: The state of this ClusterMetadata.  # noqa: E501
         :type state: State
         """
 
         self._state = state
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -277,18 +277,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Metadata):
+        if not isinstance(other, ClusterMetadata):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Metadata):
+        if not isinstance(other, ClusterMetadata):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/pagination.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     attribute_map = {
 
         'offset': 'offset',
 
         'limit': 'limit',
 
-        'links': 'links',
+        'links': '_links',
     }
 
     def __init__(self, offset=0, limit=100, links=None, local_vars_configuration=None):  # noqa: E501
         """Pagination - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/pagination_links.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/deprecated_pagination.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from ionoscloud_dbaas_postgres.configuration import Configuration
 
 
-class PaginationLinks(object):
+class DeprecatedPagination(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -30,117 +30,124 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'prev': 'str',
+        'offset': 'int',
 
-        '_self': 'str',
+        'limit': 'int',
 
-        'next': 'str',
+        'links': 'PaginationLinks',
     }
 
     attribute_map = {
 
-        'prev': 'prev',
+        'offset': 'offset',
 
-        '_self': 'self',
+        'limit': 'limit',
 
-        'next': 'next',
+        'links': 'links',
     }
 
-    def __init__(self, prev=None, _self=None, next=None, local_vars_configuration=None):  # noqa: E501
-        """PaginationLinks - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, offset=0, limit=100, links=None, local_vars_configuration=None):  # noqa: E501
+        """DeprecatedPagination - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._prev = None
-        self.__self = None
-        self._next = None
+        self._offset = None
+        self._limit = None
+        self._links = None
         self.discriminator = None
 
-        if prev is not None:
-            self.prev = prev
-        if _self is not None:
-            self._self = _self
-        if next is not None:
-            self.next = next
+        if offset is not None:
+            self.offset = offset
+        if limit is not None:
+            self.limit = limit
+        if links is not None:
+            self.links = links
 
 
     @property
-    def prev(self):
-        """Gets the prev of this PaginationLinks.  # noqa: E501
+    def offset(self):
+        """Gets the offset of this DeprecatedPagination.  # noqa: E501
 
-        URL (with offset and limit parameters) of the previous page; only present if offset is greater than 0.   # noqa: E501
+        The offset specified in the request (if none was specified, the default offset is 0).   # noqa: E501
 
-        :return: The prev of this PaginationLinks.  # noqa: E501
-        :rtype: str
+        :return: The offset of this DeprecatedPagination.  # noqa: E501
+        :rtype: int
         """
-        return self._prev
+        return self._offset
 
-    @prev.setter
-    def prev(self, prev):
-        """Sets the prev of this PaginationLinks.
+    @offset.setter
+    def offset(self, offset):
+        """Sets the offset of this DeprecatedPagination.
 
-        URL (with offset and limit parameters) of the previous page; only present if offset is greater than 0.   # noqa: E501
+        The offset specified in the request (if none was specified, the default offset is 0).   # noqa: E501
 
-        :param prev: The prev of this PaginationLinks.  # noqa: E501
-        :type prev: str
+        :param offset: The offset of this DeprecatedPagination.  # noqa: E501
+        :type offset: int
         """
+        if (self.local_vars_configuration.client_side_validation and
+                offset is not None and offset < 0):  # noqa: E501
+            raise ValueError("Invalid value for `offset`, must be a value greater than or equal to `0`")  # noqa: E501
 
-        self._prev = prev
+        self._offset = offset
 
     @property
-    def _self(self):
-        """Gets the _self of this PaginationLinks.  # noqa: E501
+    def limit(self):
+        """Gets the limit of this DeprecatedPagination.  # noqa: E501
 
-        URL (with offset and limit parameters) of the current page.   # noqa: E501
+        The limit specified in the request (if none was specified, the default limit is 100).   # noqa: E501
 
-        :return: The _self of this PaginationLinks.  # noqa: E501
-        :rtype: str
+        :return: The limit of this DeprecatedPagination.  # noqa: E501
+        :rtype: int
         """
-        return self.__self
+        return self._limit
 
-    @_self.setter
-    def _self(self, _self):
-        """Sets the _self of this PaginationLinks.
+    @limit.setter
+    def limit(self, limit):
+        """Sets the limit of this DeprecatedPagination.
 
-        URL (with offset and limit parameters) of the current page.   # noqa: E501
+        The limit specified in the request (if none was specified, the default limit is 100).   # noqa: E501
 
-        :param _self: The _self of this PaginationLinks.  # noqa: E501
-        :type _self: str
+        :param limit: The limit of this DeprecatedPagination.  # noqa: E501
+        :type limit: int
         """
+        if (self.local_vars_configuration.client_side_validation and
+                limit is not None and limit > 1000):  # noqa: E501
+            raise ValueError("Invalid value for `limit`, must be a value less than or equal to `1000`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                limit is not None and limit < 0):  # noqa: E501
+            raise ValueError("Invalid value for `limit`, must be a value greater than or equal to `0`")  # noqa: E501
 
-        self.__self = _self
+        self._limit = limit
 
     @property
-    def next(self):
-        """Gets the next of this PaginationLinks.  # noqa: E501
+    def links(self):
+        """Gets the links of this DeprecatedPagination.  # noqa: E501
 
-        URL (with offset and limit parameters) of the next page; only present if offset + limit is less than the total number of elements.   # noqa: E501
 
-        :return: The next of this PaginationLinks.  # noqa: E501
-        :rtype: str
+        :return: The links of this DeprecatedPagination.  # noqa: E501
+        :rtype: PaginationLinks
         """
-        return self._next
+        return self._links
 
-    @next.setter
-    def next(self, next):
-        """Sets the next of this PaginationLinks.
+    @links.setter
+    def links(self, links):
+        """Sets the links of this DeprecatedPagination.
 
-        URL (with offset and limit parameters) of the next page; only present if offset + limit is less than the total number of elements.   # noqa: E501
 
-        :param next: The next of this PaginationLinks.  # noqa: E501
-        :type next: str
+        :param links: The links of this DeprecatedPagination.  # noqa: E501
+        :type links: PaginationLinks
         """
 
-        self._next = next
+        self._links = links
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -167,18 +174,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PaginationLinks):
+        if not isinstance(other, DeprecatedPagination):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, PaginationLinks):
+        if not isinstance(other, DeprecatedPagination):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/patch_cluster_properties.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/patch_cluster_properties.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/patch_cluster_request.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/patch_cluster_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
 
-        'metadata': 'Metadata',
+        'metadata': 'ClusterMetadata',
 
         'properties': 'PatchClusterProperties',
     }
 
     attribute_map = {
 
         'metadata': 'metadata',
@@ -64,25 +64,25 @@
 
     @property
     def metadata(self):
         """Gets the metadata of this PatchClusterRequest.  # noqa: E501
 
 
         :return: The metadata of this PatchClusterRequest.  # noqa: E501
-        :rtype: Metadata
+        :rtype: ClusterMetadata
         """
         return self._metadata
 
     @metadata.setter
     def metadata(self, metadata):
         """Sets the metadata of this PatchClusterRequest.
 
 
         :param metadata: The metadata of this PatchClusterRequest.  # noqa: E501
-        :type metadata: Metadata
+        :type metadata: ClusterMetadata
         """
 
         self._metadata = metadata
 
     @property
     def properties(self):
         """Gets the properties of this PatchClusterRequest.  # noqa: E501
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/postgres_version_list.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/postgres_version_list.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/postgres_version_list_data.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/postgres_version_list_data.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/resource_type.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/resource_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,21 @@
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    COLLECTION = "collection"
-    CLUSTER = "cluster"
-    BACKUP = "backup"
+    COLLECTION = 'collection'
+    CLUSTER = 'cluster'
+    BACKUP = 'backup'
+    USER = 'user'
+    DATABASE = 'database'
 
-    allowable_values = [COLLECTION, CLUSTER, BACKUP]  # noqa: E501
+    allowable_values = [COLLECTION, CLUSTER, BACKUP, USER, DATABASE]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/state.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    AVAILABLE = "AVAILABLE"
-    BUSY = "BUSY"
-    DESTROYING = "DESTROYING"
-    DEGRADED = "DEGRADED"
-    FAILED = "FAILED"
-    UNKNOWN = "UNKNOWN"
+    AVAILABLE = 'AVAILABLE'
+    BUSY = 'BUSY'
+    DESTROYING = 'DESTROYING'
+    DEGRADED = 'DEGRADED'
+    FAILED = 'FAILED'
+    UNKNOWN = 'UNKNOWN'
 
     allowable_values = [AVAILABLE, BUSY, DESTROYING, DEGRADED, FAILED, UNKNOWN]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/storage_type.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/storage_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    HDD = "HDD"
-    SSD = "SSD"
-    SSD_STANDARD = "SSD Standard"
-    SSD_PREMIUM = "SSD Premium"
+    HDD = 'HDD'
+    SSD = 'SSD'
+    SSD_STANDARD = 'SSD Standard'
+    SSD_PREMIUM = 'SSD Premium'
 
     allowable_values = [HDD, SSD, SSD_STANDARD, SSD_PREMIUM]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/models/synchronization_mode.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/models/synchronization_mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    ASYNCHRONOUS = "ASYNCHRONOUS"
-    SYNCHRONOUS = "SYNCHRONOUS"
-    STRICTLY_SYNCHRONOUS = "STRICTLY_SYNCHRONOUS"
+    ASYNCHRONOUS = 'ASYNCHRONOUS'
+    SYNCHRONOUS = 'SYNCHRONOUS'
+    STRICTLY_SYNCHRONOUS = 'STRICTLY_SYNCHRONOUS'
 
     allowable_values = [ASYNCHRONOUS, SYNCHRONOUS, STRICTLY_SYNCHRONOUS]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/rest.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/rest.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres/test-driver.py` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres/test-driver.py`

 * *Files identical despite different names*

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres.egg-info/PKG-INFO` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionoscloud-dbaas-postgres
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python SDK for the Ionos DBaaS Postgres API
 Home-page: https://github.com/ionos-cloud/sdk-python-dbaas-postgres
 Author: Ionos Cloud
 Author-email: sdk@cloud.ionos.com
 Keywords: OpenAPI,OpenAPI-Generator,IONOS DBaaS PostgreSQL REST API
 Classifier: Natural Language :: English
 Classifier: Environment :: Web Environment
@@ -171,18 +171,27 @@
 | ClustersApi | [**cluster_postgres_versions_get**](docs/api/ClustersApi.md#cluster_postgres_versions_get) | **GET** /clusters/{clusterId}/postgresversions | List PostgreSQL versions |
 | ClustersApi | [**clusters_delete**](docs/api/ClustersApi.md#clusters_delete) | **DELETE** /clusters/{clusterId} | Delete a cluster |
 | ClustersApi | [**clusters_find_by_id**](docs/api/ClustersApi.md#clusters_find_by_id) | **GET** /clusters/{clusterId} | Fetch a cluster |
 | ClustersApi | [**clusters_get**](docs/api/ClustersApi.md#clusters_get) | **GET** /clusters | List clusters |
 | ClustersApi | [**clusters_patch**](docs/api/ClustersApi.md#clusters_patch) | **PATCH** /clusters/{clusterId} | Patch a cluster |
 | ClustersApi | [**clusters_post**](docs/api/ClustersApi.md#clusters_post) | **POST** /clusters | Create a cluster |
 | ClustersApi | [**postgres_versions_get**](docs/api/ClustersApi.md#postgres_versions_get) | **GET** /clusters/postgresversions | List PostgreSQL versions |
+| DatabasesApi | [**databases_delete**](docs/api/DatabasesApi.md#databases_delete) | **DELETE** /clusters/{clusterId}/databases/{databasename} | Delete database |
+| DatabasesApi | [**databases_get**](docs/api/DatabasesApi.md#databases_get) | **GET** /clusters/{clusterId}/databases/{databasename} | Get database |
+| DatabasesApi | [**databases_list**](docs/api/DatabasesApi.md#databases_list) | **GET** /clusters/{clusterId}/databases | List databases |
+| DatabasesApi | [**databases_post**](docs/api/DatabasesApi.md#databases_post) | **POST** /clusters/{clusterId}/databases | Create a database |
 | LogsApi | [**cluster_logs_get**](docs/api/LogsApi.md#cluster_logs_get) | **GET** /clusters/{clusterId}/logs | Get logs of your cluster |
 | MetadataApi | [**infos_version_get**](docs/api/MetadataApi.md#infos_version_get) | **GET** /infos/version | Get the current API version |
 | MetadataApi | [**infos_versions_get**](docs/api/MetadataApi.md#infos_versions_get) | **GET** /infos/versions | Fetch all API versions |
 | RestoresApi | [**cluster_restore_post**](docs/api/RestoresApi.md#cluster_restore_post) | **POST** /clusters/{clusterId}/restore | In-place restore of a cluster |
+| UsersApi | [**users_delete**](docs/api/UsersApi.md#users_delete) | **DELETE** /clusters/{clusterId}/users/{username} | Delete user |
+| UsersApi | [**users_get**](docs/api/UsersApi.md#users_get) | **GET** /clusters/{clusterId}/users/{username} | Get user |
+| UsersApi | [**users_list**](docs/api/UsersApi.md#users_list) | **GET** /clusters/{clusterId}/users | List users |
+| UsersApi | [**users_patch**](docs/api/UsersApi.md#users_patch) | **PATCH** /clusters/{clusterId}/users/{username} | Patch user |
+| UsersApi | [**users_post**](docs/api/UsersApi.md#users_post) | **POST** /clusters/{clusterId}/users | Create a user |
 
 </details>
 
 ## Documentation For Models
 
 All URIs are relative to *https://api.ionos.com/databases/postgresql*
 <details >
@@ -194,35 +203,51 @@
  - [ClusterBackup](docs/models/ClusterBackup)
  - [ClusterBackupList](docs/models/ClusterBackupList)
  - [ClusterBackupListAllOf](docs/models/ClusterBackupListAllOf)
  - [ClusterList](docs/models/ClusterList)
  - [ClusterListAllOf](docs/models/ClusterListAllOf)
  - [ClusterLogs](docs/models/ClusterLogs)
  - [ClusterLogsInstances](docs/models/ClusterLogsInstances)
- - [ClusterLogsMessages](docs/models/ClusterLogsMessages)
+ - [ClusterLogsInstancesMessages](docs/models/ClusterLogsInstancesMessages)
+ - [ClusterMetadata](docs/models/ClusterMetadata)
  - [ClusterProperties](docs/models/ClusterProperties)
  - [ClusterResponse](docs/models/ClusterResponse)
  - [Connection](docs/models/Connection)
  - [CreateClusterProperties](docs/models/CreateClusterProperties)
  - [CreateClusterRequest](docs/models/CreateClusterRequest)
  - [CreateRestoreRequest](docs/models/CreateRestoreRequest)
  - [DBUser](docs/models/DBUser)
+ - [Database](docs/models/Database)
+ - [DatabaseItems](docs/models/DatabaseItems)
+ - [DatabaseList](docs/models/DatabaseList)
+ - [DatabaseProperties](docs/models/DatabaseProperties)
+ - [DatabaseResource](docs/models/DatabaseResource)
  - [DayOfTheWeek](docs/models/DayOfTheWeek)
+ - [DeprecatedPagination](docs/models/DeprecatedPagination)
  - [ErrorMessage](docs/models/ErrorMessage)
  - [ErrorResponse](docs/models/ErrorResponse)
  - [MaintenanceWindow](docs/models/MaintenanceWindow)
  - [Metadata](docs/models/Metadata)
  - [Pagination](docs/models/Pagination)
  - [PaginationLinks](docs/models/PaginationLinks)
  - [PatchClusterProperties](docs/models/PatchClusterProperties)
  - [PatchClusterRequest](docs/models/PatchClusterRequest)
+ - [PatchUserProperties](docs/models/PatchUserProperties)
  - [PostgresVersionList](docs/models/PostgresVersionList)
  - [PostgresVersionListData](docs/models/PostgresVersionListData)
+ - [Resource](docs/models/Resource)
+ - [ResourceMetadata](docs/models/ResourceMetadata)
  - [ResourceType](docs/models/ResourceType)
  - [State](docs/models/State)
  - [StorageType](docs/models/StorageType)
  - [SynchronizationMode](docs/models/SynchronizationMode)
+ - [User](docs/models/User)
+ - [UserItems](docs/models/UserItems)
+ - [UserList](docs/models/UserList)
+ - [UserProperties](docs/models/UserProperties)
+ - [UserResource](docs/models/UserResource)
+ - [UsersPatchRequest](docs/models/UsersPatchRequest)
 
 
 [[Back to API list]](#documentation-for-api-endpoints) [[Back to Model list]](#documentation-for-models)
 
 </details>
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/ionoscloud_dbaas_postgres.egg-info/SOURCES.txt` & `ionoscloud-dbaas-postgres-1.2.0/ionoscloud_dbaas_postgres.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,78 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 ionoscloud_dbaas_postgres/__init__.py
 ionoscloud_dbaas_postgres/api_client.py
+ionoscloud_dbaas_postgres/api_response.py
 ionoscloud_dbaas_postgres/configuration.py
 ionoscloud_dbaas_postgres/exceptions.py
 ionoscloud_dbaas_postgres/rest.py
 ionoscloud_dbaas_postgres/test-driver.py
 ionoscloud_dbaas_postgres.egg-info/PKG-INFO
 ionoscloud_dbaas_postgres.egg-info/SOURCES.txt
 ionoscloud_dbaas_postgres.egg-info/dependency_links.txt
 ionoscloud_dbaas_postgres.egg-info/requires.txt
 ionoscloud_dbaas_postgres.egg-info/top_level.txt
 ionoscloud_dbaas_postgres/api/__init__.py
 ionoscloud_dbaas_postgres/api/backups_api.py
 ionoscloud_dbaas_postgres/api/clusters_api.py
+ionoscloud_dbaas_postgres/api/databases_api.py
 ionoscloud_dbaas_postgres/api/logs_api.py
 ionoscloud_dbaas_postgres/api/metadata_api.py
 ionoscloud_dbaas_postgres/api/restores_api.py
+ionoscloud_dbaas_postgres/api/users_api.py
 ionoscloud_dbaas_postgres/models/__init__.py
 ionoscloud_dbaas_postgres/models/api_version.py
 ionoscloud_dbaas_postgres/models/backup_location.py
 ionoscloud_dbaas_postgres/models/backup_metadata.py
 ionoscloud_dbaas_postgres/models/backup_response.py
 ionoscloud_dbaas_postgres/models/cluster_backup.py
 ionoscloud_dbaas_postgres/models/cluster_backup_list.py
 ionoscloud_dbaas_postgres/models/cluster_backup_list_all_of.py
 ionoscloud_dbaas_postgres/models/cluster_list.py
 ionoscloud_dbaas_postgres/models/cluster_list_all_of.py
 ionoscloud_dbaas_postgres/models/cluster_logs.py
 ionoscloud_dbaas_postgres/models/cluster_logs_instances.py
+ionoscloud_dbaas_postgres/models/cluster_logs_instances_messages.py
 ionoscloud_dbaas_postgres/models/cluster_logs_messages.py
+ionoscloud_dbaas_postgres/models/cluster_metadata.py
 ionoscloud_dbaas_postgres/models/cluster_properties.py
 ionoscloud_dbaas_postgres/models/cluster_response.py
 ionoscloud_dbaas_postgres/models/connection.py
 ionoscloud_dbaas_postgres/models/create_cluster_properties.py
 ionoscloud_dbaas_postgres/models/create_cluster_request.py
 ionoscloud_dbaas_postgres/models/create_restore_request.py
+ionoscloud_dbaas_postgres/models/database.py
+ionoscloud_dbaas_postgres/models/database_items.py
+ionoscloud_dbaas_postgres/models/database_list.py
+ionoscloud_dbaas_postgres/models/database_properties.py
+ionoscloud_dbaas_postgres/models/database_resource.py
 ionoscloud_dbaas_postgres/models/day_of_the_week.py
 ionoscloud_dbaas_postgres/models/db_user.py
+ionoscloud_dbaas_postgres/models/deprecated_pagination.py
 ionoscloud_dbaas_postgres/models/error_message.py
 ionoscloud_dbaas_postgres/models/error_response.py
 ionoscloud_dbaas_postgres/models/location.py
 ionoscloud_dbaas_postgres/models/maintenance_window.py
 ionoscloud_dbaas_postgres/models/metadata.py
 ionoscloud_dbaas_postgres/models/pagination.py
 ionoscloud_dbaas_postgres/models/pagination_links.py
 ionoscloud_dbaas_postgres/models/patch_cluster_properties.py
 ionoscloud_dbaas_postgres/models/patch_cluster_request.py
+ionoscloud_dbaas_postgres/models/patch_user_properties.py
 ionoscloud_dbaas_postgres/models/postgres_version_list.py
 ionoscloud_dbaas_postgres/models/postgres_version_list_data.py
+ionoscloud_dbaas_postgres/models/resource.py
+ionoscloud_dbaas_postgres/models/resource_metadata.py
 ionoscloud_dbaas_postgres/models/resource_type.py
 ionoscloud_dbaas_postgres/models/state.py
 ionoscloud_dbaas_postgres/models/storage_type.py
-ionoscloud_dbaas_postgres/models/synchronization_mode.py
+ionoscloud_dbaas_postgres/models/synchronization_mode.py
+ionoscloud_dbaas_postgres/models/user.py
+ionoscloud_dbaas_postgres/models/user_items.py
+ionoscloud_dbaas_postgres/models/user_list.py
+ionoscloud_dbaas_postgres/models/user_properties.py
+ionoscloud_dbaas_postgres/models/user_resource.py
+ionoscloud_dbaas_postgres/models/users_patch_request.py
```

### Comparing `ionoscloud-dbaas-postgres-1.1.1/setup.py` & `ionoscloud-dbaas-postgres-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 from setuptools import setup  # noqa: H301
 import os
 import codecs
 
 NAME = "ionoscloud-dbaas-postgres"
-VERSION = "1.1.1"
+VERSION = "1.2.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

