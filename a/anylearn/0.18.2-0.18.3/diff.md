# Comparing `tmp/anylearn-0.18.2.tar.gz` & `tmp/anylearn-0.18.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylearn-0.18.2.tar", last modified: Tue Jul 11 13:03:39 2023, max compression
+gzip compressed data, was "anylearn-0.18.3.tar", last modified: Thu Jul 27 10:15:34 2023, max compression
```

## Comparing `anylearn-0.18.2.tar` & `anylearn-0.18.3.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.138455 anylearn-0.18.2/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-11 13:03:30.000000 anylearn-0.18.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-11 13:03:39.138455 anylearn-0.18.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-11 13:03:30.000000 anylearn-0.18.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.126455 anylearn-0.18.2/anylearn/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.126455 anylearn-0.18.2/anylearn/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/analyzers/artifact_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/anylearnctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.126455 anylearn-0.18.2/anylearn/applications/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/applications/algorithm_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/applications/dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/applications/git_progress_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/applications/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    22943 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/applications/hpo_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    38251 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/applications/quickstart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/applications/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/applications/train_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/applications/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.130455 anylearn-0.18.2/anylearn/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/add_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/add_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/anylearn_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/quota.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/cli/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.130455 anylearn-0.18.2/anylearn/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.130455 anylearn-0.18.2/anylearn/interfaces/quota/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/quota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/quota/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.130455 anylearn-0.18.2/anylearn/interfaces/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/resource/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/resource/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/resource/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/resource/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/resource/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/resource/resource_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/resource/resource_uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.130455 anylearn-0.18.2/anylearn/interfaces/service/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/service/record.py
--rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/service/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    25688 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/train_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/interfaces/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.130455 anylearn-0.18.2/anylearn/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.134455 anylearn-0.18.2/anylearn/sdk/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/sdk/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/sdk/artifacts/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/sdk/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/sdk/artifacts/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/sdk/artifacts/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/sdk/artifacts/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/sdk/artifacts/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/sdk/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.134455 anylearn-0.18.2/anylearn/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.134455 anylearn-0.18.2/anylearn/storage/db/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/db/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.134455 anylearn-0.18.2/anylearn/storage/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/db/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/db/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.134455 anylearn-0.18.2/anylearn/storage/db/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/db/migrations/versions/6dfd859f129e_add_train_hpo_id_hpo_final_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/db/migrations/versions/848203d98d73_recreate_resource_tables_for_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/db/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/db/migrations/versions/c1ee06d84c12_create_local_train_profile_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/db/migrations/versions/c22620b97e39_create_local_hpo_experiment_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/db/migrations/versions/ed56a42729b7_alter_train_profile_datasetid_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.134455 anylearn-0.18.2/anylearn/storage/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/storage/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.134455 anylearn-0.18.2/anylearn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/utils/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/utils/func.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-11 13:03:30.000000 anylearn-0.18.2/anylearn/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.126455 anylearn-0.18.2/anylearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-11 13:03:39.000000 anylearn-0.18.2/anylearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-11 13:03:39.000000 anylearn-0.18.2/anylearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:03:39.000000 anylearn-0.18.2/anylearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 13:03:39.000000 anylearn-0.18.2/anylearn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-11 13:03:39.000000 anylearn-0.18.2/anylearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 13:03:39.000000 anylearn-0.18.2/anylearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 13:03:30.000000 anylearn-0.18.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 13:03:39.138455 anylearn-0.18.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-11 13:03:30.000000 anylearn-0.18.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.134455 anylearn-0.18.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.134455 anylearn-0.18.2/tests/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/analyzers/test_artifact_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.134455 anylearn-0.18.2/tests/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22758 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/applications/test_quick_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.138455 anylearn-0.18.2/tests/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.138455 anylearn-0.18.2/tests/interfaces/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/resource/test_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/resource/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/resource/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/resource/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/resource/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/resource/test_resource_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/resource/test_resource_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/test_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/test_train_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/interfaces/test_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:39.138455 anylearn-0.18.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 13:03:30.000000 anylearn-0.18.2/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.714265 anylearn-0.18.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 10:15:24.000000 anylearn-0.18.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-27 10:15:34.714265 anylearn-0.18.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-27 10:15:24.000000 anylearn-0.18.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.698264 anylearn-0.18.3/anylearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.698264 anylearn-0.18.3/anylearn/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/analyzers/artifact_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/anylearnctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.702264 anylearn-0.18.3/anylearn/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/applications/algorithm_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/applications/dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/applications/git_progress_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/applications/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22943 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/applications/hpo_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37920 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/applications/quickstart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/applications/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/applications/train_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/applications/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.702264 anylearn-0.18.3/anylearn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/add_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/add_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/anylearn_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/cli/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.702264 anylearn-0.18.3/anylearn/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.706264 anylearn-0.18.3/anylearn/interfaces/quota/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/quota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/quota/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.706264 anylearn-0.18.3/anylearn/interfaces/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/resource/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/resource/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/resource/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/resource/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/resource/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/resource/resource_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/resource/resource_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.706264 anylearn-0.18.3/anylearn/interfaces/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/service/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25688 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/train_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/interfaces/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.706264 anylearn-0.18.3/anylearn/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.706264 anylearn-0.18.3/anylearn/sdk/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/sdk/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/sdk/artifacts/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/sdk/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/sdk/artifacts/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/sdk/artifacts/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/sdk/artifacts/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/sdk/artifacts/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/sdk/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.706264 anylearn-0.18.3/anylearn/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.710265 anylearn-0.18.3/anylearn/storage/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/db/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.710265 anylearn-0.18.3/anylearn/storage/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/db/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/db/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.710265 anylearn-0.18.3/anylearn/storage/db/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/db/migrations/versions/6dfd859f129e_add_train_hpo_id_hpo_final_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/db/migrations/versions/848203d98d73_recreate_resource_tables_for_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/db/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/db/migrations/versions/c1ee06d84c12_create_local_train_profile_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/db/migrations/versions/c22620b97e39_create_local_hpo_experiment_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/db/migrations/versions/ed56a42729b7_alter_train_profile_datasetid_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.710265 anylearn-0.18.3/anylearn/storage/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/storage/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.710265 anylearn-0.18.3/anylearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/utils/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/utils/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-27 10:15:24.000000 anylearn-0.18.3/anylearn/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.698264 anylearn-0.18.3/anylearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-27 10:15:34.000000 anylearn-0.18.3/anylearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-27 10:15:34.000000 anylearn-0.18.3/anylearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:15:34.000000 anylearn-0.18.3/anylearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-27 10:15:34.000000 anylearn-0.18.3/anylearn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-27 10:15:34.000000 anylearn-0.18.3/anylearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 10:15:34.000000 anylearn-0.18.3/anylearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-27 10:15:24.000000 anylearn-0.18.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 10:15:34.714265 anylearn-0.18.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-27 10:15:24.000000 anylearn-0.18.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.710265 anylearn-0.18.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.714265 anylearn-0.18.3/tests/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/analyzers/test_artifact_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.714265 anylearn-0.18.3/tests/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23099 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/applications/test_quick_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.714265 anylearn-0.18.3/tests/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.714265 anylearn-0.18.3/tests/interfaces/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/resource/test_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/resource/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/resource/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/resource/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/resource/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/resource/test_resource_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/resource/test_resource_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/test_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/test_train_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/interfaces/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:34.714265 anylearn-0.18.3/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:15:24.000000 anylearn-0.18.3/tests/utils/__init__.py
```

### Comparing `anylearn-0.18.2/PKG-INFO` & `anylearn-0.18.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylearn
-Version: 0.18.2
+Version: 0.18.3
 Summary: Anylearn Python SDK
 Author: Dmagine
 Author-email: anylearn@nelbds.org.cn
 License: Proprietary
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

### Comparing `anylearn-0.18.2/README.md` & `anylearn-0.18.3/README.md`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/__init__.py` & `anylearn-0.18.3/anylearn/__init__.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/analyzers/artifact_collector.py` & `anylearn-0.18.3/anylearn/analyzers/artifact_collector.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/anylearnctl.py` & `anylearn-0.18.3/anylearn/anylearnctl.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/applications/algorithm_manager.py` & `anylearn-0.18.3/anylearn/applications/algorithm_manager.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/applications/dataset_manager.py` & `anylearn-0.18.3/anylearn/applications/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/applications/git_progress_printer.py` & `anylearn-0.18.3/anylearn/applications/git_progress_printer.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/applications/hpo.py` & `anylearn-0.18.3/anylearn/applications/hpo.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/applications/hpo_experiment.py` & `anylearn-0.18.3/anylearn/applications/hpo_experiment.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/applications/quickstart.py` & `anylearn-0.18.3/anylearn/applications/quickstart.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,26 +191,14 @@
 def _get_or_create_default_project():
     try:
         return Project.get_my_default_project()
     except:
         return Project.create_my_default_project()
 
 
-def _get_or_create_project(project_id: Optional[str]=None,
-                           project_name: Optional[str]=None):
-    try:
-        return Project(id=project_id, load_detail=True)
-    except:
-        name = project_name or f"PROJ_{generate_random_name()}"
-        description = project_name or "SDK_QUICKSTART"
-        project = Project(name=name, description=description)
-        project.save()
-        return project
-
-
 def _format_resource_request(resource_request: List[Dict[str, Dict[str, int]]]):
     if not resource_request:
         return None
     # Resource group by ID or name
     for i, req in enumerate(copy.deepcopy(resource_request)):
         for key, val in req.items():
             if key in ['default', 'besteffort'] or key.startswith('QGRP'):
@@ -874,23 +862,28 @@
         mounts[dataset_hyperparam_name] = datasets
     if models and model_hyperparam_name:
         mounts[model_hyperparam_name] = models
     if pretrain_tasks and pretrain_hyperparam_name:
         mounts[pretrain_hyperparam_name] = [t.get_results_file() for t in pretrain_tasks]
 
     # Project
-    if project_id or project_name:
-        project = _get_or_create_project(project_id=project_id,
-                                         project_name=project_name)
-    else:
+    if project_id:
+        project = Project(id=project_id, load_detail=True)
+    elif project_name:
         try:
-            project = _get_or_create_default_project()
-        except:
-            # Backward compatibility when default projects not supported
-            project = _get_or_create_project()
+            project = SDKProject.from_full_name(project_name)
+        except HTTPError as e:
+            status_code = e.response.status_code
+            cmd_error(
+                f"Error fetching project {project_name}, "
+                f"status code {status_code}."
+            )
+            raise
+    else:
+        project = _get_or_create_default_project()
 
     # Train task
     train_task_name = task_name or generate_random_name()
     _hyperparams = hyperparams or algorithm_hyperparams
     _hyperparams_prefix = hyperparams_prefix or algorithm_hyperparams_prefix
     _hyperparams_delimeter = hyperparams_delimeter or algorithm_hyperparams_delimeter
     _entrypoint = entrypoint or algorithm_entrypoint
```

### Comparing `anylearn-0.18.2/anylearn/applications/tracking.py` & `anylearn-0.18.3/anylearn/applications/tracking.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/applications/train_profile.py` & `anylearn-0.18.3/anylearn/applications/train_profile.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/applications/utils.py` & `anylearn-0.18.3/anylearn/applications/utils.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/add_algorithm.py` & `anylearn-0.18.3/anylearn/cli/add_algorithm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/add_dataset.py` & `anylearn-0.18.3/anylearn/cli/add_dataset.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/anylearn_cli_config.py` & `anylearn-0.18.3/anylearn/cli/anylearn_cli_config.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/cli.py` & `anylearn-0.18.3/anylearn/cli/cli.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/config.py` & `anylearn-0.18.3/anylearn/cli/config.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/download.py` & `anylearn-0.18.3/anylearn/cli/download.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/push.py` & `anylearn-0.18.3/anylearn/cli/push.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/quota.py` & `anylearn-0.18.3/anylearn/cli/quota.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/rm.py` & `anylearn-0.18.3/anylearn/cli/rm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/run.py` & `anylearn-0.18.3/anylearn/cli/run.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/task.py` & `anylearn-0.18.3/anylearn/cli/task.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/utils.py` & `anylearn-0.18.3/anylearn/cli/utils.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/cli/view.py` & `anylearn-0.18.3/anylearn/cli/view.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/config.py` & `anylearn-0.18.3/anylearn/config.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/env.py` & `anylearn-0.18.3/anylearn/env.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/__init__.py` & `anylearn-0.18.3/anylearn/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/base.py` & `anylearn-0.18.3/anylearn/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/mirror.py` & `anylearn-0.18.3/anylearn/interfaces/mirror.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/project.py` & `anylearn-0.18.3/anylearn/interfaces/project.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/quota/group.py` & `anylearn-0.18.3/anylearn/interfaces/quota/group.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/resource/algorithm.py` & `anylearn-0.18.3/anylearn/interfaces/resource/algorithm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/resource/dataset.py` & `anylearn-0.18.3/anylearn/interfaces/resource/dataset.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/resource/file.py` & `anylearn-0.18.3/anylearn/interfaces/resource/file.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/resource/model.py` & `anylearn-0.18.3/anylearn/interfaces/resource/model.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/resource/resource.py` & `anylearn-0.18.3/anylearn/interfaces/resource/resource.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/resource/resource_downloader.py` & `anylearn-0.18.3/anylearn/interfaces/resource/resource_downloader.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/resource/resource_uploader.py` & `anylearn-0.18.3/anylearn/interfaces/resource/resource_uploader.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/service/record.py` & `anylearn-0.18.3/anylearn/interfaces/service/record.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/service/service.py` & `anylearn-0.18.3/anylearn/interfaces/service/service.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/train_task.py` & `anylearn-0.18.3/anylearn/interfaces/train_task.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/interfaces/user.py` & `anylearn-0.18.3/anylearn/interfaces/user.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/sdk/__init__.py` & `anylearn-0.18.3/anylearn/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/sdk/artifacts/algorithm.py` & `anylearn-0.18.3/anylearn/sdk/artifacts/algorithm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/sdk/artifacts/artifact.py` & `anylearn-0.18.3/anylearn/sdk/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/sdk/artifacts/compression.py` & `anylearn-0.18.3/anylearn/sdk/artifacts/compression.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/sdk/artifacts/dataset.py` & `anylearn-0.18.3/anylearn/sdk/artifacts/dataset.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/sdk/artifacts/file.py` & `anylearn-0.18.3/anylearn/sdk/artifacts/file.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/sdk/artifacts/model.py` & `anylearn-0.18.3/anylearn/sdk/artifacts/model.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/sdk/project.py` & `anylearn-0.18.3/anylearn/sdk/project.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/sdk/task.py` & `anylearn-0.18.3/anylearn/sdk/task.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/storage/db/db.py` & `anylearn-0.18.3/anylearn/storage/db/db.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/storage/db/migrations/alembic.ini` & `anylearn-0.18.3/anylearn/storage/db/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/storage/db/migrations/env.py` & `anylearn-0.18.3/anylearn/storage/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/storage/db/migrations/versions/6dfd859f129e_add_train_hpo_id_hpo_final_metric.py` & `anylearn-0.18.3/anylearn/storage/db/migrations/versions/6dfd859f129e_add_train_hpo_id_hpo_final_metric.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/storage/db/migrations/versions/848203d98d73_recreate_resource_tables_for_checksum.py` & `anylearn-0.18.3/anylearn/storage/db/migrations/versions/848203d98d73_recreate_resource_tables_for_checksum.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/storage/db/migrations/versions/c1ee06d84c12_create_local_train_profile_table.py` & `anylearn-0.18.3/anylearn/storage/db/migrations/versions/c1ee06d84c12_create_local_train_profile_table.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/storage/db/migrations/versions/c22620b97e39_create_local_hpo_experiment_table.py` & `anylearn-0.18.3/anylearn/storage/db/migrations/versions/c22620b97e39_create_local_hpo_experiment_table.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/storage/db/migrations/versions/ed56a42729b7_alter_train_profile_datasetid_nullable.py` & `anylearn-0.18.3/anylearn/storage/db/migrations/versions/ed56a42729b7_alter_train_profile_datasetid_nullable.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/storage/db/models.py` & `anylearn-0.18.3/anylearn/storage/db/models.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/utils/api.py` & `anylearn-0.18.3/anylearn/utils/api.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/utils/errors.py` & `anylearn-0.18.3/anylearn/utils/errors.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn/utils/func.py` & `anylearn-0.18.3/anylearn/utils/func.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/anylearn.egg-info/PKG-INFO` & `anylearn-0.18.3/anylearn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylearn
-Version: 0.18.2
+Version: 0.18.3
 Summary: Anylearn Python SDK
 Author: Dmagine
 Author-email: anylearn@nelbds.org.cn
 License: Proprietary
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

### Comparing `anylearn-0.18.2/anylearn.egg-info/SOURCES.txt` & `anylearn-0.18.3/anylearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/setup.py` & `anylearn-0.18.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 
 import setuptools
 
 
-CLIENT_VERSION = "0.18.2"
+CLIENT_VERSION = "0.18.3"
 PACKAGE_NAME = "anylearn"
 
 try:
     with io.open("README.md", encoding="utf-8") as f:
         LONG_DESCRIPTION = f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = ""
```

### Comparing `anylearn-0.18.2/tests/analyzers/test_artifact_collector.py` & `anylearn-0.18.3/tests/analyzers/test_artifact_collector.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/applications/test_quick_train.py` & `anylearn-0.18.3/tests/applications/test_quick_train.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,14 @@
         responses.add(responses.POST, url=self._url("algorithm/add"),
                       json={'data': "ALGO001", 'message': "算法添加成功"},
                       status=200)
         # Stub dset creation
         responses.add(responses.POST, url=self._url("dataset/add"),
                       json={'data': "DSET001", 'message': "数据集添加成功"},
                       status=200)
-        # Stub project creation
-        responses.add(responses.POST, url=self._url("project/add"),
-                      json={'data': "PROJ001", 'message': "项目添加成功"},
-                      status=200)
         # Stub algo upload finish
         responses.add(responses.POST, url=self._url("resource/upload_finish"),
                       json={
                           'msg': "上传已完成，稍后可查看上传结果"
                       },
                       status=200)
         # Stub dset upload finish
@@ -109,14 +105,26 @@
                           'is_zipfile': 1,
                           'file': "USER001/datasets/DSET001/buzhongyao",
                           'size': 250.41,
                           'creator_id': "USER001",
                           'node_id': "NODE001",
                       }],
                       status=200)
+        # Stub default project query
+        responses.add(responses.GET,
+                      url=self._url("project/default"),
+                      json=[{
+                          'id': "PROJ001",
+                          'name': "TestProject1",
+                          'description': "test",
+                          'create_time': "2020-01-01 00:00:00",
+                          'update_time': "2020-01-01 00:00:00",
+                          'creator_id': "USER001",
+                          'datasets': "DSET001",
+                      }])
         # Stub train task creation
         responses.add(responses.POST, url=self._url("train_task/add"),
                       json={'data': "TRAI001", 'message': "服务添加成功"},
                       status=200)
         # Stub train task query
         responses.add(responses.GET, url=self._url("train_task/query?id=TRAI001"),
                       match_querystring=True, json=[{
```

### Comparing `anylearn-0.18.2/tests/base_test_case.py` & `anylearn-0.18.3/tests/base_test_case.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/interfaces/resource/test_algorithm.py` & `anylearn-0.18.3/tests/interfaces/resource/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/interfaces/resource/test_dataset.py` & `anylearn-0.18.3/tests/interfaces/resource/test_dataset.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/interfaces/resource/test_file.py` & `anylearn-0.18.3/tests/interfaces/resource/test_file.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/interfaces/resource/test_model.py` & `anylearn-0.18.3/tests/interfaces/resource/test_model.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/interfaces/resource/test_resource.py` & `anylearn-0.18.3/tests/interfaces/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/interfaces/resource/test_resource_downloader.py` & `anylearn-0.18.3/tests/interfaces/resource/test_resource_downloader.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/interfaces/resource/test_resource_uploader.py` & `anylearn-0.18.3/tests/interfaces/resource/test_resource_uploader.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/interfaces/test_db.py` & `anylearn-0.18.3/tests/interfaces/test_db.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/interfaces/test_mirror.py` & `anylearn-0.18.3/tests/interfaces/test_mirror.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/interfaces/test_project.py` & `anylearn-0.18.3/tests/interfaces/test_project.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/interfaces/test_train_task.py` & `anylearn-0.18.3/tests/interfaces/test_train_task.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.18.2/tests/interfaces/test_user.py` & `anylearn-0.18.3/tests/interfaces/test_user.py`

 * *Files identical despite different names*

