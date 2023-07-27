# Comparing `tmp/cartup-dag-1.0.2.tar.gz` & `tmp/cartup_dag-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartup-dag-1.0.2.tar", last modified: Wed Jul 26 05:54:45 2023, max compression
+gzip compressed data, was "cartup_dag-1.0.3.tar", last modified: Thu Jul 27 03:00:23 2023, max compression
```

## Comparing `cartup-dag-1.0.2.tar` & `cartup_dag-1.0.3.tar`

### file list

```diff
@@ -1,84 +1,47 @@
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.953878 cartup-dag-1.0.2/
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.941282 cartup-dag-1.0.2/.idea/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      338 2023-07-10 06:45:55.000000 cartup-dag-1.0.2/.idea/dag-jobs.iml
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.941592 cartup-dag-1.0.2/.idea/dictionaries/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      191 2022-06-02 06:21:57.000000 cartup-dag-1.0.2/.idea/dictionaries/arvind_rapaka.xml
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.942095 cartup-dag-1.0.2/.idea/inspectionProfiles/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1117 2022-05-26 02:23:08.000000 cartup-dag-1.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      174 2022-05-26 02:23:08.000000 cartup-dag-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      313 2023-07-05 20:29:11.000000 cartup-dag-1.0.2/.idea/misc.xml
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      268 2022-05-26 02:23:08.000000 cartup-dag-1.0.2/.idea/modules.xml
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      183 2022-05-26 02:23:08.000000 cartup-dag-1.0.2/.idea/vcs.xml
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)    10642 2023-07-06 09:07:55.000000 cartup-dag-1.0.2/.idea/workspace.xml
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)       21 2023-07-26 05:37:06.000000 cartup-dag-1.0.2/MANIFEST.in
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      566 2023-07-26 05:54:45.953715 cartup-dag-1.0.2/PKG-INFO
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.942338 cartup-dag-1.0.2/airflow/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup-dag-1.0.2/airflow/__init__.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.942879 cartup-dag-1.0.2/airflow/__pycache__/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      159 2022-05-27 09:18:05.000000 cartup-dag-1.0.2/airflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1849 2022-05-27 09:18:05.000000 cartup-dag-1.0.2/airflow/__pycache__/airflow_service.cpython-39.pyc
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     3746 2022-05-31 05:47:36.000000 cartup-dag-1.0.2/airflow/airflow_service.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.943371 cartup-dag-1.0.2/build/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      594 2022-06-07 04:36:22.000000 cartup-dag-1.0.2/build/Dockerfile
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.938536 cartup-dag-1.0.2/build/lib/
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.943691 cartup-dag-1.0.2/build/lib/airflow/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup-dag-1.0.2/build/lib/airflow/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     3746 2022-05-31 05:47:36.000000 cartup-dag-1.0.2/build/lib/airflow/airflow_service.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.944606 cartup-dag-1.0.2/build/lib/config/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:26:35.000000 cartup-dag-1.0.2/build/lib/config/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1522 2023-07-26 03:40:43.000000 cartup-dag-1.0.2/build/lib/config/config.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1318 2023-07-25 06:10:16.000000 cartup-dag-1.0.2/build/lib/config/config_local.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1074 2023-07-24 23:40:32.000000 cartup-dag-1.0.2/build/lib/config/config_prod.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.945098 cartup-dag-1.0.2/build/lib/server/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup-dag-1.0.2/build/lib/server/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      998 2022-05-26 02:35:43.000000 cartup-dag-1.0.2/build/lib/server/response_ws.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     6033 2023-07-26 02:11:13.000000 cartup-dag-1.0.2/build/lib/server/server.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.945335 cartup-dag-1.0.2/build/lib/ssh/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup-dag-1.0.2/build/lib/ssh/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      943 2022-05-26 09:36:53.000000 cartup-dag-1.0.2/build/lib/ssh/ssh_client.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.945659 cartup-dag-1.0.2/build/lib/utils/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup-dag-1.0.2/build/lib/utils/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     2221 2023-07-26 05:05:31.000000 cartup-dag-1.0.2/build/lib/utils/utils.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      362 2022-06-07 04:36:22.000000 cartup-dag-1.0.2/build/requirements.txt
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.946371 cartup-dag-1.0.2/cartup_dag.egg-info/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      566 2023-07-26 05:54:45.000000 cartup-dag-1.0.2/cartup_dag.egg-info/PKG-INFO
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     2056 2023-07-26 05:54:45.000000 cartup-dag-1.0.2/cartup_dag.egg-info/SOURCES.txt
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        1 2023-07-26 05:54:45.000000 cartup-dag-1.0.2/cartup_dag.egg-info/dependency_links.txt
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      335 2023-07-26 05:54:45.000000 cartup-dag-1.0.2/cartup_dag.egg-info/requires.txt
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)       32 2023-07-26 05:54:45.000000 cartup-dag-1.0.2/cartup_dag.egg-info/top_level.txt
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.947051 cartup-dag-1.0.2/config/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:26:35.000000 cartup-dag-1.0.2/config/__init__.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.947415 cartup-dag-1.0.2/config/__pycache__/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      158 2022-05-27 09:18:05.000000 cartup-dag-1.0.2/config/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      674 2022-05-27 09:18:05.000000 cartup-dag-1.0.2/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1522 2023-07-26 03:40:43.000000 cartup-dag-1.0.2/config/config.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1318 2023-07-25 06:10:16.000000 cartup-dag-1.0.2/config/config_local.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1074 2023-07-24 23:40:32.000000 cartup-dag-1.0.2/config/config_prod.py
--rwxr-xr-x   0 arvind.rapaka   (501) staff       (20)       85 2023-07-26 05:54:27.000000 cartup-dag-1.0.2/create_package.sh
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.947556 cartup-dag-1.0.2/docs/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)       19 2023-07-26 04:35:31.000000 cartup-dag-1.0.2/docs/README.md
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.939131 cartup-dag-1.0.2/jobs/
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.939058 cartup-dag-1.0.2/jobs/dashboard/
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.947686 cartup-dag-1.0.2/jobs/dashboard/config/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      730 2022-06-02 06:54:22.000000 cartup-dag-1.0.2/jobs/dashboard/config/config-dashboard.prop
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.947918 cartup-dag-1.0.2/jobs/dashboard/dags/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1088 2022-07-29 03:12:57.000000 cartup-dag-1.0.2/jobs/dashboard/dags/dag_dashboard.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.939178 cartup-dag-1.0.2/jobs/search/
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.948151 cartup-dag-1.0.2/jobs/search/dags/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1094 2022-06-02 06:54:22.000000 cartup-dag-1.0.2/jobs/search/dags/dag_search.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      335 2023-07-26 05:51:52.000000 cartup-dag-1.0.2/requirements.txt
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.950369 cartup-dag-1.0.2/server/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup-dag-1.0.2/server/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      998 2022-05-26 02:35:43.000000 cartup-dag-1.0.2/server/response_ws.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     6033 2023-07-26 02:11:13.000000 cartup-dag-1.0.2/server/server.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)       38 2023-07-26 05:54:45.953926 cartup-dag-1.0.2/setup.cfg
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      936 2023-07-26 05:54:41.000000 cartup-dag-1.0.2/setup.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.952489 cartup-dag-1.0.2/ssh/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup-dag-1.0.2/ssh/__init__.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.953055 cartup-dag-1.0.2/ssh/__pycache__/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      155 2022-05-27 09:18:05.000000 cartup-dag-1.0.2/ssh/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1537 2022-05-27 09:18:05.000000 cartup-dag-1.0.2/ssh/__pycache__/ssh_client.cpython-39.pyc
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)      943 2022-05-26 09:36:53.000000 cartup-dag-1.0.2/ssh/ssh_client.py
-drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 05:54:45.953285 cartup-dag-1.0.2/utils/
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup-dag-1.0.2/utils/__init__.py
--rw-r--r--   0 arvind.rapaka   (501) staff       (20)     2221 2023-07-26 05:05:31.000000 cartup-dag-1.0.2/utils/utils.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.433517 cartup_dag-1.0.3/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)       55 2023-07-26 06:42:37.000000 cartup_dag-1.0.3/MANIFEST.in
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      566 2023-07-27 03:00:23.433323 cartup_dag-1.0.3/PKG-INFO
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.426824 cartup_dag-1.0.3/cartup_dag/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)       33 2023-07-26 06:24:53.000000 cartup_dag-1.0.3/cartup_dag/__init__.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.428077 cartup_dag-1.0.3/cartup_dag/airflow/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup_dag-1.0.3/cartup_dag/airflow/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     3757 2023-07-27 02:07:48.000000 cartup_dag-1.0.3/cartup_dag/airflow/airflow_service.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.428695 cartup_dag-1.0.3/cartup_dag/build/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:05:58.000000 cartup_dag-1.0.3/cartup_dag/build/__init__.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.429839 cartup_dag-1.0.3/cartup_dag/config/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:26:35.000000 cartup_dag-1.0.3/cartup_dag/config/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1474 2023-07-26 06:06:49.000000 cartup_dag-1.0.3/cartup_dag/config/config.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1270 2023-07-26 06:06:49.000000 cartup_dag-1.0.3/cartup_dag/config/config_local.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1289 2023-07-26 08:17:00.000000 cartup_dag-1.0.3/cartup_dag/config/config_notification.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1026 2023-07-26 06:06:49.000000 cartup_dag-1.0.3/cartup_dag/config/config_prod.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.430033 cartup_dag-1.0.3/cartup_dag/jobs/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.3/cartup_dag/jobs/__init__.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.430138 cartup_dag-1.0.3/cartup_dag/jobs/dashboard/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.3/cartup_dag/jobs/dashboard/__init__.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.430365 cartup_dag-1.0.3/cartup_dag/jobs/dashboard/dags/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.3/cartup_dag/jobs/dashboard/dags/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1088 2022-07-29 03:12:57.000000 cartup_dag-1.0.3/cartup_dag/jobs/dashboard/dags/dag_dashboard.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.430928 cartup_dag-1.0.3/cartup_dag/jobs/search/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.3/cartup_dag/jobs/search/__init__.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.431180 cartup_dag-1.0.3/cartup_dag/jobs/search/dags/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2023-07-26 06:06:18.000000 cartup_dag-1.0.3/cartup_dag/jobs/search/dags/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     1094 2022-06-02 06:54:22.000000 cartup_dag-1.0.3/cartup_dag/jobs/search/dags/dag_search.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.432075 cartup_dag-1.0.3/cartup_dag/server/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup_dag-1.0.3/cartup_dag/server/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      998 2022-05-26 02:35:43.000000 cartup_dag-1.0.3/cartup_dag/server/response_ws.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     6068 2023-07-27 02:09:30.000000 cartup_dag-1.0.3/cartup_dag/server/server.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.432514 cartup_dag-1.0.3/cartup_dag/ssh/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup_dag-1.0.3/cartup_dag/ssh/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      954 2023-07-26 06:43:24.000000 cartup_dag-1.0.3/cartup_dag/ssh/ssh_client.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.433038 cartup_dag-1.0.3/cartup_dag/utils/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        0 2022-05-26 02:28:16.000000 cartup_dag-1.0.3/cartup_dag/utils/__init__.py
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)     2689 2023-07-27 01:36:36.000000 cartup_dag-1.0.3/cartup_dag/utils/utils.py
+drwxr-xr-x   0 arvind.rapaka   (501) staff       (20)        0 2023-07-27 03:00:23.427798 cartup_dag-1.0.3/cartup_dag.egg-info/
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      566 2023-07-27 03:00:23.000000 cartup_dag-1.0.3/cartup_dag.egg-info/PKG-INFO
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      969 2023-07-27 03:00:23.000000 cartup_dag-1.0.3/cartup_dag.egg-info/SOURCES.txt
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)        1 2023-07-27 03:00:23.000000 cartup_dag-1.0.3/cartup_dag.egg-info/dependency_links.txt
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      335 2023-07-27 03:00:23.000000 cartup_dag-1.0.3/cartup_dag.egg-info/requires.txt
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)       11 2023-07-27 03:00:23.000000 cartup_dag-1.0.3/cartup_dag.egg-info/top_level.txt
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      334 2023-07-26 06:15:15.000000 cartup_dag-1.0.3/requirements.txt
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)       38 2023-07-27 03:00:23.433567 cartup_dag-1.0.3/setup.cfg
+-rw-r--r--   0 arvind.rapaka   (501) staff       (20)      936 2023-07-26 06:42:37.000000 cartup_dag-1.0.3/setup.py
```

### Comparing `cartup-dag-1.0.2/PKG-INFO` & `cartup_dag-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cartup-dag
-Version: 1.0.2
+Name: cartup_dag
+Version: 1.0.3
 Summary: DAG Job Library.
 Author: Arvind Rapaka
 Author-email: arvind@cartup.ai
 License: Apache
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cartup-dag-1.0.2/airflow/airflow_service.py` & `cartup_dag-1.0.3/cartup_dag/airflow/airflow_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from config.config import *
+from cartup_dag.config.config import *
 import json
 import re
 import copy
 import traceback
 import logging
 import uuid
```

### Comparing `cartup-dag-1.0.2/build/lib/config/config.py` & `cartup_dag-1.0.3/cartup_dag/config/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Deploy Directory Configs
 SSH_CERTIFICATE = "/Users/arvind.rapaka/.ssh/id_rsa"
 SSH_SERVER = "127.0.0.1"
 SSH_USER = "arvind.rapaka"
 DEPLOY_DIR = "/Users/arvind.rapaka/venvs/airflow-2.6.2/airflow/dagfiles/accounts"
 
 # Jobs directory. This directory is where template dag files are found.
-JOB_DIR = "/Users/arvind.rapaka/git/cartup-ml-apis/dag-jobs/jobs/"
+JOB_DIR = "/jobs/"
 TEMP_DIR = "/tmp/dag"
 
 # config = JOBS[data["jobname"]] + "/dag_template/" + data["jobname"] + "_template"
 JOB_DAG_CONFIG_PATH = {
     "social_videos": "/Users/arvind.rapaka/git/cartup-ml-apis/social_videos/dag_template/social_videos_template",
     "widget_stats_report": ""
 }
```

### Comparing `cartup-dag-1.0.2/build/lib/config/config_local.py` & `cartup_dag-1.0.3/cartup_dag/config/config_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Deploy Directory Configs
 SSH_CERTIFICATE = "/Users/arvind.rapaka/.ssh/id_rsa"
 SSH_SERVER = "127.0.0.1"
 SSH_USER = "arvind.rapaka"
 DEPLOY_DIR = "/Users/arvind.rapaka/venvs/airflow-2.6.2/airflow/dagfiles/accounts"
 
 # Jobs directory. This directory is where template dag files are found.
-JOB_DIR = "/Users/arvind.rapaka/git/cartup-ml-apis/dag-jobs/jobs/"
+JOB_DIR = "/jobs/"
 TEMP_DIR = "/tmp/dag"
 
 # Replace Parameters
 
 SEARCH_LIBS = ""
 ML_LIBS = ""
 DASHBOARD_LIB = "/opt/airflow/dagfiles/dashboard-libs"
```

### Comparing `cartup-dag-1.0.2/build/lib/config/config_prod.py` & `cartup_dag-1.0.3/cartup_dag/config/config_prod.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Deploy Directory Configs
 SSH_CERTIFICATE = "/Users/arvind.rapaka/.ssh/id_rsa"
 SSH_SERVER = "178.62.214.94"
 SSH_USER = "arvind.rapaka"
 DEPLOY_DIR = "/home/ubuntu/airflow-docker/dagfiles/accounts"
 
 # Jobs directory. This directory is where template dag files are found.
-JOB_DIR = "/Users/arvind.rapaka/git/cartup-ml-apis/dag-jobs/jobs/"
+JOB_DIR = "/jobs/"
 TEMP_DIR = "/tmp/dag"
 
 # Replace Parameters
 SEARCH_LIBS = ""
 ML_LIBS = ""
 DASHBOARD_LIB = "/opt/airflow/dagfiles/dashboard-libs"
```

### Comparing `cartup-dag-1.0.2/build/lib/server/response_ws.py` & `cartup_dag-1.0.3/cartup_dag/server/response_ws.py`

 * *Files identical despite different names*

### Comparing `cartup-dag-1.0.2/build/lib/server/server.py` & `cartup_dag-1.0.3/cartup_dag/server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from flask import Flask, request, Response
 from flask_cors import CORS
-from config.config import *
+from cartup_dag.config.config import *
 import logging
 import traceback
 import json
 import os
-from ssh.ssh_client import SSHClient
+from cartup_dag.ssh.ssh_client import SSHClient
 import shutil
 from pathlib import Path
-from airflow.airflow_service import AirflowService
+from cartup_dag.airflow.airflow_service import AirflowService
 import re
 import copy
 import uuid
 
 
 app = Flask(__name__)
 CORS(app)
@@ -139,16 +139,16 @@
             replace_dag_id = {'DAG_NAME':  dag_id}
             write_close_file(dag_file, replace_dag_id)
             n_dag_file = head + "/" + data['org_s'] + "_" + tail
             os.rename(dag_file, n_dag_file)
             ssh_client.export_file_directory(AIRFLOW_DAG_DIR, n_dag_file, recursive=False)
             uu_id = str(uuid.uuid4())
             resp, flag = ("success", True)
-            resp, flag = airflow_client.run_airflow_cmd(cmd='trigger_dag_run', replace_params={'dag_id': dag_id},
-                                            data=json.dumps({"conf": {}, "dag_run_id": uu_id}))
+            #resp, flag = airflow_client.run_airflow_cmd(cmd='trigger_dag_run', replace_params={'dag_id': dag_id},
+            #                                data=json.dumps({"conf": {}, "dag_run_id": uu_id}))
             if not flag:
                 logging.error("Not able to trigger the job {} {}".format(n_dag_file, uu_id))
             else:
                 logging.info(resp.text)
 
     except Exception as e:
         logging.error(traceback.print_exc())
```

### Comparing `cartup-dag-1.0.2/build/lib/ssh/ssh_client.py` & `cartup_dag-1.0.3/cartup_dag/ssh/ssh_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import paramiko
-from config.config import *
+from cartup_dag.config.config import *
 from scp import SCPClient
 
 
 class SSHClient:
     def __init__(self):
         self.sshcon = paramiko.SSHClient()  # will create the object
         self.sshcon.set_missing_host_key_policy(paramiko.AutoAddPolicy())
```

### Comparing `cartup-dag-1.0.2/build/lib/utils/utils.py` & `cartup_dag-1.0.3/cartup_dag/utils/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import boto3
 from botocore.exceptions import ClientError
+from cartup_dag.config.config_notification import s3_config
 
 
 def replace_line_with_regex(file_path, regex_pattern, new_value):
     try:
         with open(file_path, 'r') as file:
             content = file.read()
             file.close()
@@ -19,47 +20,55 @@
         print("Line replaced successfully.")
     except FileNotFoundError:
         print("File not found.")
     except Exception as e:
         print(f"An error occurred: {str(e)}")
 
 
-def create_s3_bucket(bucket_name):
-    s3 = boto3.client('s3')
+def create_s3_bucket(bucket_name, client):
     try:
-        s3.create_bucket(Bucket=bucket_name)
+        client.create_bucket(Bucket=bucket_name)
         print(f"Bucket '{bucket_name}' created successfully.")
     except ClientError as e:
         if e.response['Error']['Code'] == 'BucketAlreadyOwnedByYou':
             print(f"Bucket '{bucket_name}' already exists.")
         else:
             print(f"Error creating bucket '{bucket_name}': {e}")
 
 
 def push_file_to_s3(bucket_name, file_path, s3_key):
     try:
-        s3 = boto3.client('s3')
+        session = boto3.session.Session()
+        client = session.client('s3',
+                                region_name=s3_config["region"],
+                                endpoint_url=s3_config["endpoint_url"],
+                                aws_access_key_id=s3_config["ACCESS_ID"],
+                                aws_secret_access_key=s3_config["SECRET_KEY"])
 
         # Check if the bucket exists, if not, create it
-        response = s3.list_buckets()
+        response = client.list_buckets()
         buckets = [bucket['Name'] for bucket in response['Buckets']]
         if bucket_name not in buckets:
-            create_s3_bucket(bucket_name)
+            create_s3_bucket(bucket_name, client)
 
         # Upload the file to S3
         with open(file_path, 'rb') as file:
-            s3.upload_fileobj(file, bucket_name, s3_key)
+            client.upload_fileobj(file, bucket_name, s3_key)
 
         print("File successfully uploaded to S3.")
-    except FileNotFoundError:
-        print("File not found.")
     except Exception as e:
         print(f"An error occurred: {str(e)}")
 
 
+def job_status_update():
+
+    pass
+
+
 if __name__ == '__main__':
     # Example usage
-    bucket_name = 'your-bucket-name'  # Replace this with the name of your S3 bucket
-    file_path = 'path/to/your/file.txt'  # Replace this with the path to your file
-    s3_key = 'destination/file.txt'  # Replace this with the destination key (S3 object key)
-    replace_line_with_regex("/tmp/dag/demo/social_videos/config/config.py", "last_update_time *?=.*",
-                            "last_update_time=\"1 TO 2\"")
+    bucket_name = 'cartup-demo-test'  # Replace this with the name of your S3 bucket
+    file_path = '/tmp/dag/demo/social_videos/config/config.py'  # Replace this with the path to your file
+    s3_key = 'dag/demo/social_videos/config/config.py'  # Replace this with the destination key (S3 object key)
+    push_file_to_s3(bucket_name, file_path, s3_key)
+    #replace_line_with_regex("/tmp/dag/demo/social_videos/config/config.py", "last_update_time *?=.*",
+    #                        "last_update_time=\"1 TO 2\"")
```

### Comparing `cartup-dag-1.0.2/cartup_dag.egg-info/PKG-INFO` & `cartup_dag-1.0.3/cartup_dag.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartup-dag
-Version: 1.0.2
+Version: 1.0.3
 Summary: DAG Job Library.
 Author: Arvind Rapaka
 Author-email: arvind@cartup.ai
 License: Apache
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `cartup-dag-1.0.2/jobs/dashboard/dags/dag_dashboard.py` & `cartup_dag-1.0.3/cartup_dag/jobs/dashboard/dags/dag_dashboard.py`

 * *Files identical despite different names*

### Comparing `cartup-dag-1.0.2/jobs/search/dags/dag_search.py` & `cartup_dag-1.0.3/cartup_dag/jobs/search/dags/dag_search.py`

 * *Files identical despite different names*

### Comparing `cartup-dag-1.0.2/setup.py` & `cartup_dag-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 with open('docs/README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
-    name='cartup-dag',
-    version='1.0.2',
+    name='cartup_dag',
+    version='1.0.3',
     license='Apache',
     description='DAG Job Library.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='arvind@cartup.ai',
     author='Arvind Rapaka',
     packages=find_packages(),
```

