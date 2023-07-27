# Comparing `tmp/dpdispatcher-0.5.8.tar.gz` & `tmp/dpdispatcher-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpdispatcher-0.5.8.tar", last modified: Mon Jul 17 08:13:01 2023, max compression
+gzip compressed data, was "dpdispatcher-0.5.9.tar", last modified: Wed Jul 19 04:23:04 2023, max compression
```

## Comparing `dpdispatcher-0.5.8.tar` & `dpdispatcher-0.5.9.tar`

### file list

```diff
@@ -1,301 +1,304 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.070121 dpdispatcher-0.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.074121 dpdispatcher-0.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/ci-docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/machines.yml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/mirror_gitee.yml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/publish_conda.yml
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/pyright.yml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/ci/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/ci/pbs/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/pbs/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/pbs/start-pbs.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/pbs.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/ci/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/slurm/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/slurm/register_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/slurm/start-slurm.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/slurm.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/ci/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/ssh/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/ssh/start-ssh.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      411 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/ssh.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/ci/ssh_rsync.sh
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/conda/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/conda/conda_build_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/batch.md
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/context.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/credits.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/dpdispatcher_on_yarn.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.078121 dpdispatcher-0.5.8/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/examples/expanse.md
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/examples/g16.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/examples/shell.md
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/install.md
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/machine.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/doc/task.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.082121 dpdispatcher-0.5.8/dpdispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/JobStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 08:13:00.000000 dpdispatcher-0.5.8/dpdispatcher/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/arginfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/base_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/distributed_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dp_cloud_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dp_cloud_server_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.082121 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/retcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/temp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/zip_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/dpdisp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/fugaku.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/hdfs_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/hdfs_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/lazy_local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    14648 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/ssh_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    46643 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/dpdispatcher/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.082121 dpdispatcher-0.5.8/dpdispatcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-17 08:13:01.000000 dpdispatcher-0.5.8/dpdispatcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-07-17 08:13:01.000000 dpdispatcher-0.5.8/dpdispatcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:13:01.000000 dpdispatcher-0.5.8/dpdispatcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 08:13:01.000000 dpdispatcher-0.5.8/dpdispatcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 08:13:01.000000 dpdispatcher-0.5.8/dpdispatcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 08:13:01.000000 dpdispatcher-0.5.8/dpdispatcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.070121 dpdispatcher-0.5.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.082121 dpdispatcher-0.5.8/examples/machine/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/machine/expanse.json
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/machine/lazy_local.json
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/machine/mandu.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.082121 dpdispatcher-0.5.8/examples/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/resources/expanse_cpu.json
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/resources/mandu.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.082121 dpdispatcher-0.5.8/examples/task/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/task/deepmd-kit.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/examples/task/g16.json
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.086121 dpdispatcher-0.5.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/scripts/script_gen_dargs_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/scripts/script_gen_dargs_json.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.090122 dpdispatcher-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/batch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/context.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1843 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/debug_test_class_submission_init.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3228 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_ali_ehpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2669 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_dp_cloud_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1752 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_lazy_ali_ehpc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_lsf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_shell.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_slurm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2629 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/devel_test_ssh_ali_ehpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.094122 dpdispatcher-0.5.8/tests/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/job.json
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine.json
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_ali_ehpc.json
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_center.json
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_diffenert.json
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_dp_cloud_server.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_fugaku.json
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_if_cuda_multi_devices.json
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_lazy_local_lsf.json
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_lazy_local_slurm.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_lazylocal_shell.json
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_local_fugaku.json
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_local_shell.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_lsf.json
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_slurm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/machine_yarn.json
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/resources.json
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/submission.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/jsons/task.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.094122 dpdispatcher-0.5.8/tests/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/lsf/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/lsf/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/lsf/test_lsf_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.094122 dpdispatcher-0.5.8/tests/old/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/old/test_dispatcher_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/old/test_lazy_local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/old/test_local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/old/test_local_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/old/test_ssh_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.094122 dpdispatcher-0.5.8/tests/pbs/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/pbs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/pbs/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/pbs/test_pbs_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/sample_class.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1074 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/script_gen_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/shell/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/shell/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/shell/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/shell/test_shell_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/shell/test_shell_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm/test_dispatcher_lazy_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm/test_slurm_lazy_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm/test_slurm_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm/test_slurm_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/slurm_test.env
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_argcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_job.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_machine_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_submission_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_class_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.070121 dpdispatcher-0.5.8/tests/test_context_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-1/some_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-1/some_dir/some_file
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.098122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-4/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/dir with space/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/dir with space/file with space
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_context_dir/0_md/some_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_context_dir/0_md/some_dir/some_file
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_group_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.070121 dpdispatcher-0.5.8/tests/test_hdfs_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.070121 dpdispatcher-0.5.8/tests/test_if_cuda_multi_devices/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_if_cuda_multi_devices/test_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_if_cuda_multi_devices/test_dir/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_import_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lazy_local_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_local_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.074121 dpdispatcher-0.5.8/tests/test_lsf_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.102122 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/graph.pb
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/submission.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     4068 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_lsf_script_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.074121 dpdispatcher-0.5.8/tests/test_pbs_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/graph.pb
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_run_submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_run_submission_ratio_unfinished.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1913 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_cuda_multi_devices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4895 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.074121 dpdispatcher-0.5.8/tests/test_shell_trival_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/fail_dir/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/fail_dir/mock_fail_task.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir with space/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir with space/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir1/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir2/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir2/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir3/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir3/example.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir4/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/dir4/example.txt
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/parent_dir/graph.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.106122 dpdispatcher-0.5.8/tests/test_shell_trival_dir/recover_dir/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_shell_trival_dir/recover_dir/mock_recover_task.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.074121 dpdispatcher-0.5.8/tests/test_slurm_dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-1/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-1/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-1/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-2/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-2/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-3/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-3/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-3/input.lammps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-4/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-4/conf.lmp
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-4/input.lammps
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/graph.pb
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/submission.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     2349 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_slurm_script_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_ssh_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:01.110122 dpdispatcher-0.5.8/tests/test_work_path/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:12:50.000000 dpdispatcher-0.5.8/tests/test_work_path/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.784278 dpdispatcher-0.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.748278 dpdispatcher-0.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.756278 dpdispatcher-0.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/.github/workflows/ci-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/.github/workflows/machines.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/.github/workflows/publish_conda.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/.github/workflows/pyright.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-19 04:23:04.784278 dpdispatcher-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.760278 dpdispatcher-0.5.9/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.760278 dpdispatcher-0.5.9/ci/pbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/pbs/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/pbs/start-pbs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/pbs.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.760278 dpdispatcher-0.5.9/ci/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/slurm/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/slurm/register_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/slurm/start-slurm.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      423 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/slurm.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.760278 dpdispatcher-0.5.9/ci/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/ssh/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/ssh/start-ssh.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      411 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/ssh.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/ci/ssh_rsync.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.760278 dpdispatcher-0.5.9/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/conda/conda_build_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.760278 dpdispatcher-0.5.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/batch.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/context.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/dpdispatcher_on_yarn.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.760278 dpdispatcher-0.5.9/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/examples/expanse.md
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/examples/g16.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/examples/shell.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/doc/task.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.764278 dpdispatcher-0.5.9/dpdispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/JobStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-19 04:23:04.000000 dpdispatcher-0.5.9/dpdispatcher/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/arginfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/base_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/distributed_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/dp_cloud_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/dp_cloud_server_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.764278 dpdispatcher-0.5.9/dpdispatcher/dpcloudserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/dpcloudserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/dpcloudserver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/dpcloudserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/dpcloudserver/retcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/dpcloudserver/temp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/dpcloudserver/zip_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/dpdisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/fugaku.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/hdfs_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/hdfs_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/lazy_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/openapi_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/ssh_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46295 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/dpdispatcher/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.764278 dpdispatcher-0.5.9/dpdispatcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-19 04:23:04.000000 dpdispatcher-0.5.9/dpdispatcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-07-19 04:23:04.000000 dpdispatcher-0.5.9/dpdispatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 04:23:04.000000 dpdispatcher-0.5.9/dpdispatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 04:23:04.000000 dpdispatcher-0.5.9/dpdispatcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-19 04:23:04.000000 dpdispatcher-0.5.9/dpdispatcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-19 04:23:04.000000 dpdispatcher-0.5.9/dpdispatcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.752277 dpdispatcher-0.5.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.764278 dpdispatcher-0.5.9/examples/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/examples/machine/expanse.json
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/examples/machine/lazy_local.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/examples/machine/mandu.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.764278 dpdispatcher-0.5.9/examples/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/examples/resources/expanse_cpu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/examples/resources/mandu.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.764278 dpdispatcher-0.5.9/examples/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/examples/task/deepmd-kit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/examples/task/g16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.768278 dpdispatcher-0.5.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/scripts/script_gen_dargs_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/scripts/script_gen_dargs_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 04:23:04.784278 dpdispatcher-0.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.772278 dpdispatcher-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/context.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1843 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/debug_test_class_submission_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3228 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/devel_test_ali_ehpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2669 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/devel_test_dp_cloud_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1752 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/devel_test_lazy_ali_ehpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/devel_test_lsf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/devel_test_shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/devel_test_slurm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2629 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/devel_test_ssh_ali_ehpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.772278 dpdispatcher-0.5.9/tests/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/job.json
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine.json
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_ali_ehpc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_center.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_diffenert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_dp_cloud_server.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_fugaku.json
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_if_cuda_multi_devices.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_lazy_local_lsf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_lazy_local_slurm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_lazylocal_shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_local_fugaku.json
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_local_shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_lsf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_openapi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_slurm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/machine_yarn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/resources.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/submission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/jsons/task.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.772278 dpdispatcher-0.5.9/tests/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/lsf/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/lsf/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/lsf/test_lsf_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.772278 dpdispatcher-0.5.9/tests/old/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/old/test_dispatcher_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/old/test_lazy_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/old/test_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/old/test_local_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/old/test_ssh_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.772278 dpdispatcher-0.5.9/tests/pbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/pbs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/pbs/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/pbs/test_pbs_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/sample_class.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1074 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/script_gen_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/shell/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/shell/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/shell/test_shell_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/shell/test_shell_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/slurm/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/slurm/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/slurm/test_dispatcher_lazy_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/slurm/test_slurm_lazy_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/slurm/test_slurm_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/slurm/test_slurm_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/slurm_test.env
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_argcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_class_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_class_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_class_machine_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_class_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_class_submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_class_submission_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_class_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.752277 dpdispatcher-0.5.9/tests/test_context_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_context_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-1/some_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-1/some_dir/some_file
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-4/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_context_dir/0_md/dir with space/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_context_dir/0_md/dir with space/file with space
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_context_dir/0_md/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_context_dir/0_md/some_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_context_dir/0_md/some_dir/some_file
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_hdfs_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.752277 dpdispatcher-0.5.9/tests/test_hdfs_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.752277 dpdispatcher-0.5.9/tests/test_if_cuda_multi_devices/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.776278 dpdispatcher-0.5.9/tests/test_if_cuda_multi_devices/test_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_if_cuda_multi_devices/test_dir/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_import_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_lazy_local_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_local_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.752277 dpdispatcher-0.5.9/tests/test_lsf_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/submission.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4068 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_lsf_script_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.752277 dpdispatcher-0.5.9/tests/test_pbs_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_run_submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_run_submission_ratio_unfinished.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1913 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_shell_cuda_multi_devices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4895 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_shell_trival.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.756278 dpdispatcher-0.5.9/tests/test_shell_trival_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_shell_trival_dir/fail_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_shell_trival_dir/fail_dir/mock_fail_task.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_shell_trival_dir/parent_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_shell_trival_dir/parent_dir/dir with space/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_shell_trival_dir/parent_dir/dir with space/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_shell_trival_dir/parent_dir/dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_shell_trival_dir/parent_dir/dir1/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_shell_trival_dir/parent_dir/dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_shell_trival_dir/parent_dir/dir2/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_shell_trival_dir/parent_dir/dir3/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_shell_trival_dir/parent_dir/dir3/example.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_shell_trival_dir/parent_dir/dir4/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_shell_trival_dir/parent_dir/dir4/example.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_shell_trival_dir/parent_dir/graph.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_shell_trival_dir/recover_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_shell_trival_dir/recover_dir/mock_recover_task.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.756278 dpdispatcher-0.5.9/tests/test_slurm_dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-1/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-1/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-1/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.780278 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-2/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-2/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.784278 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-3/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-3/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-3/input.lammps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.784278 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-4/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-4/conf.lmp
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-4/input.lammps
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/graph.pb
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/submission.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2349 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_slurm_script_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_ssh_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 04:23:04.784278 dpdispatcher-0.5.9/tests/test_work_path/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 04:22:46.000000 dpdispatcher-0.5.9/tests/test_work_path/.gitkeep
```

### Comparing `dpdispatcher-0.5.8/.github/workflows/ci-docker.yml` & `dpdispatcher-0.5.9/.github/workflows/ci-docker.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/.github/workflows/test.yml` & `dpdispatcher-0.5.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/.pre-commit-config.yaml` & `dpdispatcher-0.5.9/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,27 @@
     -   id: check-json
     -   id: check-added-large-files
     -   id: check-merge-conflict
     -   id: check-symlinks
     -   id: check-toml
 # Python
 -   repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
     -   id: black-jupyter
--   repo: https://github.com/charliermarsh/ruff-pre-commit
+-   repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.0.275
+    rev: v0.0.278
     hooks:
     - id: ruff
       args: ["--fix"]
 # numpydoc
 -   repo: https://github.com/Carreau/velin
     rev: 0.0.12
     hooks:
     - id: velin
       args: ["--write"]
 # Python inside docs
 -   repo: https://github.com/asottile/blacken-docs
-    rev: 1.14.0
+    rev: 1.15.0
     hooks:
     -   id: blacken-docs
```

### Comparing `dpdispatcher-0.5.8/CONTRIBUTING.md` & `dpdispatcher-0.5.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/LICENSE` & `dpdispatcher-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/PKG-INFO` & `dpdispatcher-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpdispatcher
-Version: 0.5.8
+Version: 0.5.9
 Summary: Generate HPC scheduler systems jobs input scripts, submit these scripts to HPC systems, and poke until they finish
 Author: DeepModeling
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -182,14 +182,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: cloudserver
+Provides-Extra: bohrium
 Provides-Extra: test
 License-File: LICENSE
 
 # DPDispatcher
 
 [![conda-forge](https://img.shields.io/conda/dn/conda-forge/dpdispatcher?color=red&label=conda-forge&logo=conda-forge)](https://anaconda.org/conda-forge/dpdispatcher)
 [![pip install](https://img.shields.io/pypi/dm/dpdispatcher?label=pip%20install&logo=pypi)](https://pypi.org/project/dpdispatcher)
@@ -206,14 +207,20 @@
 
 DPDispatcher can be installed by `pip`:
 
 ```bash
 pip install dpdispatcher
 ```
 
+To add [Bohrium](https://bohrium.dp.tech/) support, execute
+
+```bash
+pip install dpdispatcher[bohrium]
+```
+
 ## Usage
 
 See [Getting Started](https://dpdispatcher.readthedocs.io/en/latest/getting-started.html) for usage.
 
 ## Contributing
 
 DPDispatcher is maintained by Deep Modeling's developers and welcomes other people.
```

### Comparing `dpdispatcher-0.5.8/README.md` & `dpdispatcher-0.5.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 
 DPDispatcher can be installed by `pip`:
 
 ```bash
 pip install dpdispatcher
 ```
 
+To add [Bohrium](https://bohrium.dp.tech/) support, execute
+
+```bash
+pip install dpdispatcher[bohrium]
+```
+
 ## Usage
 
 See [Getting Started](https://dpdispatcher.readthedocs.io/en/latest/getting-started.html) for usage.
 
 ## Contributing
 
 DPDispatcher is maintained by Deep Modeling's developers and welcomes other people.
```

### Comparing `dpdispatcher-0.5.8/ci/LICENSE` & `dpdispatcher-0.5.9/ci/LICENSE`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/ci/pbs/docker-compose.yml` & `dpdispatcher-0.5.9/ci/pbs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/ci/pbs.sh` & `dpdispatcher-0.5.9/ci/pbs.sh`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/ci/slurm/docker-compose.yml` & `dpdispatcher-0.5.9/ci/slurm/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/ci/slurm/start-slurm.sh` & `dpdispatcher-0.5.9/ci/slurm/start-slurm.sh`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/ci/ssh/docker-compose.yml` & `dpdispatcher-0.5.9/ci/ssh/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/ci/ssh_rsync.sh` & `dpdispatcher-0.5.9/ci/ssh_rsync.sh`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/conda/meta.yaml` & `dpdispatcher-0.5.9/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/doc/.gitignore` & `dpdispatcher-0.5.9/doc/.gitignore`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/doc/Makefile` & `dpdispatcher-0.5.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/doc/batch.md` & `dpdispatcher-0.5.9/doc/batch.md`

 * *Files 6% similar despite different names*

```diff
@@ -66,7 +66,13 @@
 ## Fugaku
 
 {dargs:argument}`batch_type <resources/batch_type>`: `Fugaku`
 
 [Fujitsu cloud service](https://doc.cloud.global.fujitsu.com/lib/common/jp/hpc-user-manual/) is a job scheduling system used by Fujitsu's HPCs such as Fugaku, ITO and K computer. It should be noted that although the same job scheduling system is used, there are some differences in the details, Fagaku class cannot be directly used for other HPCs.
 
 Read Fujitsu cloud service documentation for details.
+
+
+## OpenAPI
+
+{dargs:argument}`batcy_type <resources/batch_type>`: `OpenAPI`
+OpenAPI is a new way to submit jobs to Bohrium. It using [AccessKey](https://bohrium.dp.tech/personal/setting) instead of username and password. Read Bohrium documentation for details.
```

### Comparing `dpdispatcher-0.5.8/doc/conf.py` & `dpdispatcher-0.5.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/doc/context.md` & `dpdispatcher-0.5.9/doc/context.md`

 * *Files 10% similar despite different names*

```diff
@@ -38,7 +38,15 @@
 
 ## HDFS
 
 {dargs:argument}`context_type <machine/context_type>`: `HDFS`
 
 The Hadoop Distributed File System (HDFS) is a distributed file system.
 Read [Support DPDispatcher on Yarn](dpdispatcher_on_yarn.md) for details.
+
+
+## OpenAPI
+
+{dargs:argument}`context_type <machine/context_type>`: `OpenAPI`
+
+OpenAPI is a new way to submit jobs to Bohrium. It using [AccessKey](https://bohrium.dp.tech/personal/setting) instead of username and password. Read Bohrium documentation for details.
+To use OpenAPI, one needs to provide necessary parameters in {dargs:argument}`remote_profile <machine[OpenAPIContext]/remote_profile>`.
```

### Comparing `dpdispatcher-0.5.8/doc/dpdispatcher_on_yarn.md` & `dpdispatcher-0.5.9/doc/dpdispatcher_on_yarn.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/doc/examples/expanse.md` & `dpdispatcher-0.5.9/doc/examples/expanse.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/doc/examples/shell.md` & `dpdispatcher-0.5.9/doc/examples/shell.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/doc/getting-started.md` & `dpdispatcher-0.5.9/doc/getting-started.md`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/doc/index.rst` & `dpdispatcher-0.5.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/doc/make.bat` & `dpdispatcher-0.5.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/dpdispatcher/__init__.py` & `dpdispatcher-0.5.9/dpdispatcher/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 from .dp_cloud_server_context import DpCloudServerContext, LebesgueContext
 from .fugaku import Fugaku
 from .hdfs_context import HDFSContext
 from .lazy_local_context import LazyLocalContext
 from .local_context import LocalContext
 from .lsf import LSF
 from .machine import Machine
+from .openapi import OpenAPI
+from .openapi_context import OpenAPIContext
 from .pbs import PBS, Torque
 from .shell import Shell
 from .slurm import Slurm
 from .ssh_context import SSHContext
 from .submission import Job, Resources, Submission, Task
 
 
@@ -73,14 +75,16 @@
     print()
 
 
 __all__ = [
     "__version__",
     "DistributedShell",
     "DpCloudServer",
+    "OpenAPI",
+    "OpenAPIContext",
     "DpCloudServerContext",
     "HDFSContext",
     "LazyLocalContext",
     "LocalContext",
     "LSF",
     "Machine",
     "PBS",
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher/base_context.py` & `dpdispatcher-0.5.9/dpdispatcher/base_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/dpdispatcher/distributed_shell.py` & `dpdispatcher-0.5.9/dpdispatcher/distributed_shell.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/dpdispatcher/dp_cloud_server.py` & `dpdispatcher-0.5.9/dpdispatcher/dp_cloud_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,21 @@
         if "lebesgue_version" in self.input_data:
             self.api_version = self.input_data.get("lebesgue_version", 2)
         self.grouped = self.input_data.get("grouped", False)
         email = context.remote_profile.get("email", None)
         phone = context.remote_profile.get("phone", None)
         username = context.remote_profile.get("username", None)
         password = context.remote_profile.get("password", None)
+
+        ticket = os.environ.get("BOHR_TICKET", None)
+        if ticket:
+            self.api = Client(ticket=ticket)
+            self.group_id = None
+            return
+
         if email is None and username is not None:
             raise DeprecationWarning(
                 "username is no longer support in current version, "
                 "please consider use email instead of username."
             )
         if email is None and phone is None:
             raise ValueError(
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher/dp_cloud_server_context.py` & `dpdispatcher-0.5.9/dpdispatcher/dp_cloud_server_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # from zip_file import zip_files
 
 DP_CLOUD_SERVER_HOME_DIR = os.path.join(
     os.path.expanduser("~"), ".dpdispatcher/", "dp_cloud_server/"
 )
 ENDPOINT = "http://oss-cn-shenzhen.aliyuncs.com"
-BUCKET_NAME = "dpcloudserver"
+BUCKET_NAME = os.environ.get("BUCKET_NAME", "dpcloudserver")
 
 
 class BohriumContext(BaseContext):
     alias = ("DpCloudServerContext", "LebesgueContext")
 
     def __init__(
         self,
@@ -35,17 +35,24 @@
         *args,
         **kwargs,
     ):
         self.init_local_root = local_root
         self.init_remote_root = remote_root
         self.temp_local_root = os.path.abspath(local_root)
         self.remote_profile = remote_profile
+        ticket = os.environ.get("BOHR_TICKET", None)
         email = remote_profile.get("email", None)
         phone = remote_profile.get("phone", None)
         password = remote_profile.get("password")
+        os.makedirs(DP_CLOUD_SERVER_HOME_DIR, exist_ok=True)
+
+        if ticket is not None:
+            self.api = Client(ticket=ticket)
+            return
+
         if email is None and phone is None:
             raise ValueError(
                 "can not find email/phone number in remote_profile, please check your machine file."
             )
         if password is None:
             raise ValueError(
                 "can not find password in remote_profile, please check your machine file."
@@ -53,16 +60,14 @@
         # account 作为登录账号
         account = email
         if email is None:
             account = phone
 
         self.api = Client(account, password)
 
-        os.makedirs(DP_CLOUD_SERVER_HOME_DIR, exist_ok=True)
-
     @classmethod
     def load_from_dict(cls, context_dict):
         local_root = context_dict["local_root"]
         remote_root = context_dict.get("remote_root", None)
         remote_profile = context_dict.get("remote_profile", {})
 
         dp_cloud_server_context = cls(
@@ -252,17 +257,15 @@
         result = self.check_home_file_exits(fname)
         return result
 
     def check_home_file_exits(self, fname):
         return os.path.isfile(os.path.join(DP_CLOUD_SERVER_HOME_DIR, fname))
 
     def clean(self):
-        submission_file_name = "{submission_hash}.json".format(
-            submission_hash=self.submission.submission_hash
-        )
+        submission_file_name = f"{self.submission.submission_hash}.json"
         submission_json = os.path.join(DP_CLOUD_SERVER_HOME_DIR, submission_file_name)
         os.remove(submission_json)
         return True
 
     # def get_return(self, cmd_pipes):
     #     if not self.check_finish(cmd_pipes):
     #         return None, None, None
@@ -284,15 +287,15 @@
         )
         return [
             Argument(
                 "remote_profile",
                 dict,
                 [
                     Argument("email", str, optional=True, doc="Email"),
-                    Argument("password", str, optional=False, doc="Password"),
+                    Argument("password", str, optional=True, doc="Password"),
                     Argument(
                         "program_id",
                         int,
                         optional=False,
                         alias=["project_id"],
                         doc="Program ID",
                     ),
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/client.py` & `dpdispatcher-0.5.9/dpdispatcher/dpcloudserver/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,24 +21,27 @@
 
 
 class RequestInfoException(Exception):
     pass
 
 
 class Client:
-    def __init__(self, email=None, password=None, debug=False, base_url=API_HOST):
+    def __init__(
+        self, email=None, password=None, debug=False, ticket=None, base_url=API_HOST
+    ):
         self.debug = debug
         self.debug = os.getenv("LBG_CLI_DEBUG_PRINT", debug)
         self.config = {}
         self.token = ""
         self.user_id = None
         self.config["email"] = email
         self.config["password"] = password
         self.base_url = base_url
         self.last_log_offset = 0
+        self.ticket = ticket
 
     def post(self, url, data=None, header=None, params=None, retry=5):
         return self._req(
             "POST", url, data=data, header=header, params=params, retry=retry
         )
 
     def get(self, url, header=None, params=None, retry=5):
@@ -47,15 +50,17 @@
     def _req(self, method, url, data=None, header=None, params=None, retry=5):
         short_url = url
         url = urllib.parse.urljoin(self.base_url, url)
         if header is None:
             header = {}
         if not self.token:
             self.refresh_token()
+        self.ticket = os.environ.get("BOHR_TICKET", "")
         header["Authorization"] = f"jwt {self.token}"
+        header["Brm-Ticket"] = self.ticket
         resp_code = None
         err = None
         for i in range(retry):
             resp = None
             if method == "GET":
                 resp = requests.get(url, params=params, headers=header)
             else:
@@ -92,14 +97,17 @@
         post_data = {"email": self.config["email"], "password": self.config["password"]}
         resp = self.post("/account/login", post_data)
         self.token = resp["token"]
         # print(self.token)
         self.user_id = resp["user_id"]
 
     def refresh_token(self, retry=3):
+        self.ticket = os.environ.get("BOHR_TICKET", "")
+        if self.ticket:
+            return
         url = "/account/login"
         post_data = {"email": self.config["email"], "password": self.config["password"]}
         resp_code = None
         err = None
         for i in range(retry):
             resp = requests.post(
                 urljoin(API_HOST, url),
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/config.py` & `dpdispatcher-0.5.9/dpdispatcher/dpcloudserver/config.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/retcode.py` & `dpdispatcher-0.5.9/dpdispatcher/dpcloudserver/retcode.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/temp_test.py` & `dpdispatcher-0.5.9/dpdispatcher/dpcloudserver/temp_test.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/dpdispatcher/dpcloudserver/zip_file.py` & `dpdispatcher-0.5.9/dpdispatcher/dpcloudserver/zip_file.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/dpdispatcher/fugaku.py` & `dpdispatcher-0.5.9/dpdispatcher/fugaku.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,15 @@
         resources = job.resources
         fugaku_script_header_dict = {}
         fugaku_script_header_dict[
             "fugaku_node_number_line"
         ] = f'#PJM -L "node={resources.number_node}" '
         fugaku_script_header_dict[
             "fugaku_ntasks_per_node_line"
-        ] = '#PJM --mpi "max-proc-per-node={cpu_per_node}"'.format(
-            cpu_per_node=resources.cpu_per_node
-        )
+        ] = f'#PJM --mpi "max-proc-per-node={resources.cpu_per_node}"'
         fugaku_script_header_dict[
             "queue_name_line"
         ] = f'#PJM -L "rscgrp={resources.queue_name}"'
         fugaku_script_header = fugaku_script_header_template.format(
             **fugaku_script_header_dict
         )
         return fugaku_script_header
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher/hdfs_cli.py` & `dpdispatcher-0.5.9/dpdispatcher/hdfs_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,62 +86,54 @@
         Raises: on unexpected error.
         """
         # Make sure local_path is accessible
         if not os.path.exists(local_path) or not os.access(local_path, os.R_OK):
             raise RuntimeError(
                 "try to access local_path[{}] " "but failed".format(local_path)
             )
-        cmd = "hadoop fs -copyFromLocal -f {local} {remote}".format(
-            local=local_path, remote=to_uri
-        )
+        cmd = f"hadoop fs -copyFromLocal -f {local_path} {to_uri}"
         try:
             ret, out, err = run_cmd_with_all_output(cmd)
             if ret == 0:
                 return True, out
             else:
                 raise RuntimeError(
                     "Cannot copy local[{}] to remote[{}] with cmd[{}]; "
                     "ret[{}] output[{}] stderr[{}]".format(
                         local_path, to_uri, cmd, ret, out, err
                     )
                 )
         except Exception as e:
             raise RuntimeError(
-                "Cannot copy local[{}] to remote[{}] with cmd[{}]".format(
-                    local_path, to_uri, cmd
-                )
+                f"Cannot copy local[{local_path}] to remote[{to_uri}] with cmd[{cmd}]"
             ) from e
 
     @staticmethod
     def copy_to_local(from_uri, local_path):
         remote = ""
         if isinstance(from_uri, str):
             remote = from_uri
         elif isinstance(from_uri, list) or isinstance(from_uri, tuple):
             remote = " ".join(from_uri)
-        cmd = "hadoop fs -copyToLocal {remote} {local}".format(
-            remote=remote, local=local_path
-        )
+        cmd = f"hadoop fs -copyToLocal {remote} {local_path}"
 
         try:
             ret, out, err = run_cmd_with_all_output(cmd)
             if ret == 0:
                 return True
             else:
                 raise RuntimeError(
                     "Cannot copy remote[{}] to local[{}] with cmd[{}]; "
                     "ret[{}] output[{}] stderr[{}]".format(
                         from_uri, local_path, cmd, ret, out, err
                     )
                 )
         except Exception as e:
             raise RuntimeError(
-                "Cannot copy remote[{}] to local[{}] with cmd[{}]".format(
-                    from_uri, local_path, cmd
-                )
+                f"Cannot copy remote[{from_uri}] to local[{local_path}] with cmd[{cmd}]"
             ) from e
 
     @staticmethod
     def read_hdfs_file(uri):
         cmd = f"hadoop fs -text {uri}"
         try:
             ret, out, err = run_cmd_with_all_output(cmd)
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher/hdfs_context.py` & `dpdispatcher-0.5.9/dpdispatcher/hdfs_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,18 +133,15 @@
         cwd = os.getcwd()
 
         # download all hdfs files to tmp dir
         gz_dir = os.path.join(self.local_root, "tmp")
         if os.path.exists(gz_dir):
             shutil.rmtree(gz_dir, ignore_errors=True)
         os.mkdir(os.path.join(self.local_root, "tmp"))
-        rfile_tgz = "{}/{}_*_download.tar.gz".format(
-            self.remote_root,
-            submission.submission_hash,
-        )
+        rfile_tgz = f"{self.remote_root}/{submission.submission_hash}_*_download.tar.gz"
         lfile_tgz = "%s/tmp/" % (self.local_root)
         HDFS.copy_to_local(rfile_tgz, lfile_tgz)
 
         tgz_file_list = glob(os.path.join(self.local_root, "tmp/*_download.tar.gz"))
         for tgz in tgz_file_list:
             with tarfile.open(tgz, "r:gz") as tar:
                 tar.extractall(path=gz_dir)
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher/lazy_local_context.py` & `dpdispatcher-0.5.9/dpdispatcher/lazy_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/dpdispatcher/local_context.py` & `dpdispatcher-0.5.9/dpdispatcher/local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/dpdispatcher/lsf.py` & `dpdispatcher-0.5.9/dpdispatcher/lsf.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,16 @@
 
     def gen_script_header(self, job):
         resources = job.resources
         script_header_dict = {
             "lsf_nodes_line": "#BSUB -n {number_cores}".format(
                 number_cores=resources.number_node * resources.cpu_per_node
             ),
-            "lsf_ptile_line": "#BSUB -R 'span[ptile={cpu_per_node}]'".format(
-                cpu_per_node=resources.cpu_per_node
-            ),
-            "lsf_partition_line": "#BSUB -q {queue_name}".format(
-                queue_name=resources.queue_name
-            ),
+            "lsf_ptile_line": f"#BSUB -R 'span[ptile={resources.cpu_per_node}]'",
+            "lsf_partition_line": f"#BSUB -q {resources.queue_name}",
         }
         gpu_usage_flag = resources.kwargs.get("gpu_usage", False)
         gpu_new_syntax_flag = resources.kwargs.get("gpu_new_syntax", False)
         gpu_exclusive_flag = resources.kwargs.get("gpu_exclusive", True)
         custom_gpu_line = resources.kwargs.get("custom_gpu_line", None)
         if not custom_gpu_line:
             if gpu_usage_flag is True:
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher/machine.py` & `dpdispatcher-0.5.9/dpdispatcher/machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,17 +204,15 @@
             script_command=script_command,
             script_end=script_end,
         )
         return script
 
     def check_if_recover(self, submission):
         submission_hash = submission.submission_hash
-        submission_file_name = "{submission_hash}.json".format(
-            submission_hash=submission_hash
-        )
+        submission_file_name = f"{submission_hash}.json"
         if_recover = self.context.check_file_exists(submission_file_name)
         return if_recover
 
     @abstractmethod
     def check_finish_tag(self, **kwargs):
         raise NotImplementedError(
             "abstract method check_finish_tag should be implemented by derived class"
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher/pbs.py` & `dpdispatcher-0.5.9/dpdispatcher/pbs.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,24 +18,20 @@
         return pbs_script
 
     def gen_script_header(self, job):
         resources = job.resources
         pbs_script_header_dict = {}
         pbs_script_header_dict[
             "select_node_line"
-        ] = "#PBS -l select={number_node}:ncpus={cpu_per_node}".format(
-            number_node=resources.number_node, cpu_per_node=resources.cpu_per_node
-        )
+        ] = f"#PBS -l select={resources.number_node}:ncpus={resources.cpu_per_node}"
         if resources.gpu_per_node != 0:
             pbs_script_header_dict[
                 "select_node_line"
             ] += f":ngpus={resources.gpu_per_node}"
-        pbs_script_header_dict["queue_name_line"] = "#PBS -q {queue_name}".format(
-            queue_name=resources.queue_name
-        )
+        pbs_script_header_dict["queue_name_line"] = f"#PBS -q {resources.queue_name}"
         pbs_script_header = pbs_script_header_template.format(**pbs_script_header_dict)
         return pbs_script_header
 
     def do_submit(self, job):
         script_file_name = job.script_file_name
         script_str = self.gen_script(job)
         job_id_name = job.job_hash + "_job_id"
@@ -143,19 +139,15 @@
 
     def gen_script_header(self, job):
         # ref: https://support.adaptivecomputing.com/wp-content/uploads/2021/02/torque/torque.htm#topics/torque/2-jobs/requestingRes.htm
         resources = job.resources
         pbs_script_header_dict = {}
         pbs_script_header_dict[
             "select_node_line"
-        ] = "#PBS -l nodes={number_node}:ppn={cpu_per_node}".format(
-            number_node=resources.number_node, cpu_per_node=resources.cpu_per_node
-        )
+        ] = f"#PBS -l nodes={resources.number_node}:ppn={resources.cpu_per_node}"
         if resources.gpu_per_node != 0:
             pbs_script_header_dict["select_node_line"] += ":gpus={gpu_per_node}".format(
                 gpu_per_node=resources.gpu_per_node
             )
-        pbs_script_header_dict["queue_name_line"] = "#PBS -q {queue_name}".format(
-            queue_name=resources.queue_name
-        )
+        pbs_script_header_dict["queue_name_line"] = f"#PBS -q {resources.queue_name}"
         pbs_script_header = pbs_script_header_template.format(**pbs_script_header_dict)
         return pbs_script_header
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher/shell.py` & `dpdispatcher-0.5.9/dpdispatcher/shell.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/dpdispatcher/slurm.py` & `dpdispatcher-0.5.9/dpdispatcher/slurm.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,24 +30,20 @@
         resources = job.resources
         script_header_dict = {}
         script_header_dict["slurm_nodes_line"] = "#SBATCH --nodes {number_node}".format(
             number_node=resources.number_node
         )
         script_header_dict[
             "slurm_ntasks_per_node_line"
-        ] = "#SBATCH --ntasks-per-node {cpu_per_node}".format(
-            cpu_per_node=resources.cpu_per_node
-        )
+        ] = f"#SBATCH --ntasks-per-node {resources.cpu_per_node}"
         custom_gpu_line = resources.kwargs.get("custom_gpu_line", None)
         if not custom_gpu_line:
             script_header_dict[
                 "slurm_number_gpu_line"
-            ] = "#SBATCH --gres=gpu:{gpu_per_node}".format(
-                gpu_per_node=resources.gpu_per_node
-            )
+            ] = f"#SBATCH --gres=gpu:{resources.gpu_per_node}"
         else:
             script_header_dict["slurm_number_gpu_line"] = custom_gpu_line
         if resources.queue_name != "":
             script_header_dict[
                 "slurm_partition_line"
             ] = f"#SBATCH --partition {resources.queue_name}"
         else:
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher/ssh_context.py` & `dpdispatcher-0.5.9/dpdispatcher/ssh_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/dpdispatcher/submission.py` & `dpdispatcher-0.5.9/dpdispatcher/submission.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,31 +262,31 @@
         self.submission_to_json()
         if clean:
             self.clean_jobs()
         return self.serialize()
 
     def try_download_result(self):
         start_time = time.time()
-        retry_interval = 60  # 每1分钟重试一次
+        retry_interval = 60  # retry every 1 minute
         success = False
         while not success:
             try:
                 self.download_jobs()
                 success = True
             except (EOFError, Exception) as e:
                 dlog.exception(e)
                 elapsed_time = time.time() - start_time
-                if elapsed_time < 3600:  # 1小时内
+                if elapsed_time < 3600:  # in 1 h
                     dlog.info("Retrying in 1 minute...")
                     time.sleep(retry_interval)
-                elif elapsed_time < 86400:  # 1小时后，但在24小时内
-                    retry_interval = 600  # 每10分钟重试一次
+                elif elapsed_time < 86400:  # 1 h ~ 24 h
+                    retry_interval = 600  # retry every 10 min
                     dlog.info("Retrying in 10 minutes...")
                     time.sleep(retry_interval)
-                else:  # 超过24小时
+                else:  # > 24 h
                     dlog.info("Maximum retries time reached. Exiting.")
                     break
 
     async def async_run_submission(self, **kwargs):
         """Async interface of run_submission.
 
         Examples
@@ -505,33 +505,29 @@
 
     def clean_jobs(self):
         self.machine.context.clean()
 
     def submission_to_json(self):
         # self.update_submission_state()
         write_str = json.dumps(self.serialize(), indent=4, default=str)
-        submission_file_name = "{submission_hash}.json".format(
-            submission_hash=self.submission_hash
-        )
+        submission_file_name = f"{self.submission_hash}.json"
         self.machine.context.write_file(submission_file_name, write_str=write_str)
 
     @classmethod
     def submission_from_json(cls, json_file_name="submission.json"):
         with open(json_file_name) as f:
             submission_dict = json.load(f)
         # submission_dict = machine.context.read_file(json_file_name)
         submission = cls.deserialize(submission_dict=submission_dict, machine=None)
         return submission
 
     # def check_if_recover()
 
     def try_recover_from_json(self):
-        submission_file_name = "{submission_hash}.json".format(
-            submission_hash=self.submission_hash
-        )
+        submission_file_name = f"{self.submission_hash}.json"
         if_recover = self.machine.context.check_file_exists(submission_file_name)
         submission = None
         submission_dict = {}
         if if_recover:
             submission_dict_str = self.machine.context.read_file(
                 fname=submission_file_name
             )
@@ -783,17 +779,15 @@
         Returns
         -------
         submission : Job
             the Job class instance converted from the job_dict
         """
         if len(job_dict.keys()) != 1:
             raise RuntimeError(
-                "json file may be broken, len(job_dict.keys()) must be 1. {job_dict}".format(
-                    job_dict=job_dict
-                )
+                f"json file may be broken, len(job_dict.keys()) must be 1. {job_dict}"
             )
         job_hash = list(job_dict.keys())[0]
 
         job_task_list = [
             Task.deserialize(task_dict)
             for task_dict in job_dict[job_hash]["job_task_list"]
         ]
@@ -867,19 +861,15 @@
 
         if job_state == JobStatus.unsubmitted:
             dlog.debug(f"job: {self.job_hash} unsubmitted; submit it")
             # if self.fail_count > 3:
             #     raise RuntimeError("job:job {job} failed 3 times".format(job=self))
             self.submit_job()
             if self.job_state != JobStatus.unsubmitted:
-                dlog.info(
-                    "job: {job_hash} submit; job_id is {job_id}".format(
-                        job_hash=self.job_hash, job_id=self.job_id
-                    )
-                )
+                dlog.info(f"job: {self.job_hash} submit; job_id is {self.job_id}")
             if self.resources.wait_time != 0:
                 time.sleep(self.resources.wait_time)
             # self.get_job_state()
 
     def get_hash(self):
         return str(list(self.serialize(if_static=True).keys())[0])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher/utils.py` & `dpdispatcher-0.5.9/dpdispatcher/utils.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/dpdispatcher.egg-info/PKG-INFO` & `dpdispatcher-0.5.9/dpdispatcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpdispatcher
-Version: 0.5.8
+Version: 0.5.9
 Summary: Generate HPC scheduler systems jobs input scripts, submit these scripts to HPC systems, and poke until they finish
 Author: DeepModeling
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -182,14 +182,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: cloudserver
+Provides-Extra: bohrium
 Provides-Extra: test
 License-File: LICENSE
 
 # DPDispatcher
 
 [![conda-forge](https://img.shields.io/conda/dn/conda-forge/dpdispatcher?color=red&label=conda-forge&logo=conda-forge)](https://anaconda.org/conda-forge/dpdispatcher)
 [![pip install](https://img.shields.io/pypi/dm/dpdispatcher?label=pip%20install&logo=pypi)](https://pypi.org/project/dpdispatcher)
@@ -206,14 +207,20 @@
 
 DPDispatcher can be installed by `pip`:
 
 ```bash
 pip install dpdispatcher
 ```
 
+To add [Bohrium](https://bohrium.dp.tech/) support, execute
+
+```bash
+pip install dpdispatcher[bohrium]
+```
+
 ## Usage
 
 See [Getting Started](https://dpdispatcher.readthedocs.io/en/latest/getting-started.html) for usage.
 
 ## Contributing
 
 DPDispatcher is maintained by Deep Modeling's developers and welcomes other people.
```

### Comparing `dpdispatcher-0.5.8/dpdispatcher.egg-info/SOURCES.txt` & `dpdispatcher-0.5.9/dpdispatcher.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,16 @@
 dpdispatcher/fugaku.py
 dpdispatcher/hdfs_cli.py
 dpdispatcher/hdfs_context.py
 dpdispatcher/lazy_local_context.py
 dpdispatcher/local_context.py
 dpdispatcher/lsf.py
 dpdispatcher/machine.py
+dpdispatcher/openapi.py
+dpdispatcher/openapi_context.py
 dpdispatcher/pbs.py
 dpdispatcher/shell.py
 dpdispatcher/slurm.py
 dpdispatcher/ssh_context.py
 dpdispatcher/submission.py
 dpdispatcher/utils.py
 dpdispatcher.egg-info/PKG-INFO
@@ -136,14 +138,15 @@
 tests/jsons/machine_if_cuda_multi_devices.json
 tests/jsons/machine_lazy_local_lsf.json
 tests/jsons/machine_lazy_local_slurm.json
 tests/jsons/machine_lazylocal_shell.json
 tests/jsons/machine_local_fugaku.json
 tests/jsons/machine_local_shell.json
 tests/jsons/machine_lsf.json
+tests/jsons/machine_openapi.json
 tests/jsons/machine_slurm.json
 tests/jsons/machine_yarn.json
 tests/jsons/resources.json
 tests/jsons/submission.json
 tests/jsons/task.json
 tests/lsf/context.py
 tests/lsf/test_dispatcher.py
```

### Comparing `dpdispatcher-0.5.8/examples/resources/expanse_cpu.json` & `dpdispatcher-0.5.9/examples/resources/expanse_cpu.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/pyproject.toml` & `dpdispatcher-0.5.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     'sphinx',
     'myst-parser',
     'sphinx_rtd_theme>=1.0.0rc1',
     'numpydoc',
     'deepmodeling_sphinx>=0.1.1',
     'dargs>=0.3.1',
 ]
-cloudserver = ["oss2", "tqdm"]
+cloudserver = ["oss2", "tqdm", "bohrium-sdk"]
+bohrium = ["oss2", "tqdm", "bohrium-sdk"]
 test = []
 
 [tool.setuptools.packages.find]
 include = ["dpdispatcher*"]
 
 [tool.setuptools_scm]
 write_to = "dpdispatcher/_version.py"
```

### Comparing `dpdispatcher-0.5.8/scripts/script_gen_dargs_docs.py` & `dpdispatcher-0.5.9/scripts/script_gen_dargs_docs.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/context.py` & `dpdispatcher-0.5.9/tests/context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/debug_test_class_submission_init.py` & `dpdispatcher-0.5.9/tests/debug_test_class_submission_init.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/devel_test_ali_ehpc.py` & `dpdispatcher-0.5.9/tests/devel_test_ali_ehpc.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/devel_test_dp_cloud_server.py` & `dpdispatcher-0.5.9/tests/devel_test_dp_cloud_server.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/devel_test_lazy_ali_ehpc.py` & `dpdispatcher-0.5.9/tests/devel_test_lazy_ali_ehpc.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/devel_test_lsf.py` & `dpdispatcher-0.5.9/tests/devel_test_lsf.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/devel_test_shell.py` & `dpdispatcher-0.5.9/tests/devel_test_shell.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/devel_test_slurm.py` & `dpdispatcher-0.5.9/tests/devel_test_slurm.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/devel_test_ssh_ali_ehpc.py` & `dpdispatcher-0.5.9/tests/devel_test_ssh_ali_ehpc.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/jsons/job.json` & `dpdispatcher-0.5.9/tests/jsons/job.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/jsons/machine_center.json` & `dpdispatcher-0.5.9/tests/jsons/machine_center.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/jsons/machine_diffenert.json` & `dpdispatcher-0.5.9/tests/jsons/machine_diffenert.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/jsons/machine_dp_cloud_server.json` & `dpdispatcher-0.5.9/tests/jsons/machine_dp_cloud_server.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/jsons/machine_fugaku.json` & `dpdispatcher-0.5.9/tests/jsons/machine_fugaku.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/jsons/machine_lazy_local_lsf.json` & `dpdispatcher-0.5.9/tests/jsons/machine_lazy_local_lsf.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/jsons/machine_lazy_local_slurm.json` & `dpdispatcher-0.5.9/tests/jsons/machine_lazy_local_slurm.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/jsons/machine_lsf.json` & `dpdispatcher-0.5.9/tests/jsons/machine_lsf.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/jsons/machine_slurm.json` & `dpdispatcher-0.5.9/tests/jsons/machine_slurm.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/jsons/machine_yarn.json` & `dpdispatcher-0.5.9/tests/jsons/machine_yarn.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/jsons/submission.json` & `dpdispatcher-0.5.9/tests/jsons/submission.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/lsf/context.py` & `dpdispatcher-0.5.9/tests/lsf/context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/lsf/test_dispatcher.py` & `dpdispatcher-0.5.9/tests/lsf/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/lsf/test_lsf_local.py` & `dpdispatcher-0.5.9/tests/lsf/test_lsf_local.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/old/test_dispatcher_utils.py` & `dpdispatcher-0.5.9/tests/old/test_dispatcher_utils.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/old/test_lazy_local_context.py` & `dpdispatcher-0.5.9/tests/old/test_lazy_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/old/test_local_context.py` & `dpdispatcher-0.5.9/tests/old/test_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/old/test_ssh_context.py` & `dpdispatcher-0.5.9/tests/old/test_ssh_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/pbs/context.py` & `dpdispatcher-0.5.9/tests/pbs/context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/pbs/test_dispatcher.py` & `dpdispatcher-0.5.9/tests/pbs/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/pbs/test_pbs_local.py` & `dpdispatcher-0.5.9/tests/pbs/test_pbs_local.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/sample_class.py` & `dpdispatcher-0.5.9/tests/sample_class.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/script_gen_json.py` & `dpdispatcher-0.5.9/tests/script_gen_json.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/shell/context.py` & `dpdispatcher-0.5.9/tests/shell/context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/shell/test_dispatcher.py` & `dpdispatcher-0.5.9/tests/shell/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/shell/test_shell_local.py` & `dpdispatcher-0.5.9/tests/shell/test_shell_local.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/shell/test_shell_ssh.py` & `dpdispatcher-0.5.9/tests/shell/test_shell_ssh.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/slurm/context.py` & `dpdispatcher-0.5.9/tests/slurm/context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/slurm/test_dispatcher.py` & `dpdispatcher-0.5.9/tests/slurm/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/slurm/test_dispatcher_lazy_local.py` & `dpdispatcher-0.5.9/tests/slurm/test_dispatcher_lazy_local.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/slurm/test_slurm_lazy_local.py` & `dpdispatcher-0.5.9/tests/slurm/test_slurm_lazy_local.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/slurm/test_slurm_local.py` & `dpdispatcher-0.5.9/tests/slurm/test_slurm_local.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/slurm/test_slurm_ssh.py` & `dpdispatcher-0.5.9/tests/slurm/test_slurm_ssh.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_argcheck.py` & `dpdispatcher-0.5.9/tests/test_argcheck.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_class_job.py` & `dpdispatcher-0.5.9/tests/test_class_job.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_class_machine.py` & `dpdispatcher-0.5.9/tests/test_class_machine.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_class_machine_dispatch.py` & `dpdispatcher-0.5.9/tests/test_class_machine_dispatch.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_class_resources.py` & `dpdispatcher-0.5.9/tests/test_class_resources.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_class_submission.py` & `dpdispatcher-0.5.9/tests/test_class_submission.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_class_submission_init.py` & `dpdispatcher-0.5.9/tests/test_class_submission_init.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_class_task.py` & `dpdispatcher-0.5.9/tests/test_class_task.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_context_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.9/tests/test_context_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_group_size.py` & `dpdispatcher-0.5.9/tests/test_group_size.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_hdfs_context.py` & `dpdispatcher-0.5.9/tests/test_hdfs_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_hdfs_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.9/tests/test_hdfs_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_import_classes.py` & `dpdispatcher-0.5.9/tests/test_import_classes.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_lazy_local_context.py` & `dpdispatcher-0.5.9/tests/test_lazy_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_local_context.py` & `dpdispatcher-0.5.9/tests/test_local_context.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_lsf_dir/0_md/submission.json` & `dpdispatcher-0.5.9/tests/test_lsf_dir/0_md/submission.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_lsf_script_generation.py` & `dpdispatcher-0.5.9/tests/test_lsf_script_generation.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_pbs_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.9/tests/test_pbs_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_retry.py` & `dpdispatcher-0.5.9/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_run_submission.py` & `dpdispatcher-0.5.9/tests/test_run_submission.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_run_submission_ratio_unfinished.py` & `dpdispatcher-0.5.9/tests/test_run_submission_ratio_unfinished.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_shell_cuda_multi_devices.py` & `dpdispatcher-0.5.9/tests/test_shell_cuda_multi_devices.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_shell_trival.py` & `dpdispatcher-0.5.9/tests/test_shell_trival.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-1/input.lammps` & `dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-1/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-2/input.lammps` & `dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-2/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-3/input.lammps` & `dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-3/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/bct-4/input.lammps` & `dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/bct-4/input.lammps`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json` & `dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/d3c842c5b9476e48f7145b370cd330372b9293e1.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_slurm_dir/0_md/submission.json` & `dpdispatcher-0.5.9/tests/test_slurm_dir/0_md/submission.json`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_slurm_script_generation.py` & `dpdispatcher-0.5.9/tests/test_slurm_script_generation.py`

 * *Files identical despite different names*

### Comparing `dpdispatcher-0.5.8/tests/test_ssh_context.py` & `dpdispatcher-0.5.9/tests/test_ssh_context.py`

 * *Files identical despite different names*

