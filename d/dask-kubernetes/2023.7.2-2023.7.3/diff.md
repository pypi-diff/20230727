# Comparing `tmp/dask-kubernetes-2023.7.2.tar.gz` & `tmp/dask-kubernetes-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-kubernetes-2023.7.2.tar", last modified: Fri Jul 14 15:52:45 2023, max compression
+gzip compressed data, was "dask-kubernetes-2023.7.3.tar", last modified: Thu Jul 27 09:41:43 2023, max compression
```

## Comparing `dask-kubernetes-2023.7.2.tar` & `dask-kubernetes-2023.7.3.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/dask_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/dask_kubernetes/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/tests/test_pykube_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/tests/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/classic/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28558 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/classic/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/config-demo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/fake_gcp_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/common/
--rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/common/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/common/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/common/tests/test_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/common/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/helm/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/helm/helmcluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/helm/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/helm/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/helm/tests/resources/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/helm/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/kubernetes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32989 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/plugins/noop/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/plugins/noop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/plugins/noop/noop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/test_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.145387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskjob.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/templates.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.137386 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.145387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/chartpress.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.145387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.145387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   283847 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   471240 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   140704 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.145387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    42764 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.137386 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68747 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.351725 dask-kubernetes-2023.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-27 09:41:43.351725 dask-kubernetes-2023.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.355725 dask-kubernetes-2023.7.3/dask_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-27 09:41:43.355725 dask-kubernetes-2023.7.3/dask_kubernetes/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.343724 dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.343724 dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/tests/test_pykube_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.343724 dask-kubernetes-2023.7.3/dask_kubernetes/classic/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28558 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/classic/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.343724 dask-kubernetes-2023.7.3/dask_kubernetes/classic/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/classic/tests/config-demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/classic/tests/fake_gcp_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28722 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/classic/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/classic/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.343724 dask-kubernetes-2023.7.3/dask_kubernetes/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.343724 dask-kubernetes-2023.7.3/dask_kubernetes/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/common/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/common/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.343724 dask-kubernetes-2023.7.3/dask_kubernetes/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/common/tests/test_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/common/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/helm/helmcluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/helm/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/helm/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/helm/tests/resources/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/helm/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/kubernetes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29340 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/plugins/noop/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/plugins/noop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/plugins/noop/noop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    26294 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/tests/test_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskjob.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/templates.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.339724 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/chartpress.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.347725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.351725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   283847 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   471240 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   140704 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.351725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.351725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42764 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.351725 dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:41:43.343724 dask-kubernetes-2023.7.3/dask_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-27 09:41:43.000000 dask-kubernetes-2023.7.3/dask_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-27 09:41:43.000000 dask-kubernetes-2023.7.3/dask_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:41:43.000000 dask-kubernetes-2023.7.3/dask_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-27 09:41:43.000000 dask-kubernetes-2023.7.3/dask_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:41:43.000000 dask-kubernetes-2023.7.3/dask_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-27 09:41:43.000000 dask-kubernetes-2023.7.3/dask_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 09:41:43.000000 dask-kubernetes-2023.7.3/dask_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-27 09:41:43.351725 dask-kubernetes-2023.7.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68747 2023-07-27 09:41:34.000000 dask-kubernetes-2023.7.3/versioneer.py
```

### Comparing `dask-kubernetes-2023.7.2/LICENSE` & `dask-kubernetes-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/PKG-INFO` & `dask-kubernetes-2023.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2023.7.2
+Version: 2023.7.3
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `dask-kubernetes-2023.7.2/README.rst` & `dask-kubernetes-2023.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/__init__.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/dask.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/dask.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/mixins.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/mixins.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/objects.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/query.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/query.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/tests/test_pykube_objects.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/tests/test_pykube_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import uuid
 
 from dask_kubernetes.aiopykube import HTTPClient, KubeConfig
 from dask_kubernetes.aiopykube.objects import Pod
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_pod_create_and_delete(docker_image, k8s_cluster):
     api = HTTPClient(KubeConfig.from_env())
     name = "test-" + uuid.uuid4().hex[:10]
     pod = Pod(
         api,
         {
             "apiVersion": "v1",
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/tests/test_query.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/aiopykube/tests/test_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pytest
 
 from dask_kubernetes.aiopykube import HTTPClient, KubeConfig
 from dask_kubernetes.aiopykube.query import Query
 from dask_kubernetes.aiopykube.objects import Pod
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_pod_query(k8s_cluster):
     api = HTTPClient(KubeConfig.from_env())
     async for pod in Query(api, Pod, namespace="kube-system"):
         assert isinstance(pod, Pod)
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_pod_objects(k8s_cluster):
     api = HTTPClient(KubeConfig.from_env())
     async for pod in Pod.objects(api).filter(namespace="kube-system"):
         assert isinstance(pod, Pod)
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/classic/kubecluster.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/classic/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/config-demo.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/classic/tests/config-demo.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/test_async.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/classic/tests/test_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pytest_asyncio
 import asyncio
 import base64
 import getpass
 import os
 import random
 from time import time
 import yaml
@@ -64,53 +63,53 @@
     else:
         yield
 
 
 cluster_kwargs = {"asynchronous": True}
 
 
-@pytest_asyncio.fixture
+@pytest.fixture
 async def cluster(k8s_cluster, pod_spec):
     async with KubeCluster(pod_spec, **cluster_kwargs) as cluster:
         yield cluster
 
 
-@pytest_asyncio.fixture
+@pytest.fixture
 async def remote_cluster(k8s_cluster, pod_spec):
     async with KubeCluster(pod_spec, deploy_mode="remote", **cluster_kwargs) as cluster:
         yield cluster
 
 
-@pytest_asyncio.fixture
+@pytest.fixture
 async def client(cluster):
     async with Client(cluster, asynchronous=True) as client:
         yield client
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_fixtures(client):
     """An initial test to get all the fixtures to run and check the cluster is usable."""
     assert client
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_versions(client):
     await client.get_versions(check=True)
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_cluster_create(cluster):
     cluster.scale(1)
     await cluster
     async with Client(cluster, asynchronous=True) as client:
         result = await client.submit(lambda x: x + 1, 10)
         assert result == 11
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_basic(cluster, client):
     cluster.scale(2)
     future = client.submit(lambda x: x + 1, 10)
     result = await future
     assert result == 11
 
     await client.wait_for_workers(2)
@@ -118,15 +117,15 @@
     # Ensure that inter-worker communication works well
     futures = client.map(lambda x: x + 1, range(10))
     total = client.submit(sum, futures)
     assert (await total) == sum(map(lambda x: x + 1, range(10)))
     assert all((await client.has_what()).values())
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_logs(remote_cluster):
     cluster = remote_cluster
     cluster.scale(2)
     await cluster
 
     async with Client(cluster, asynchronous=True) as client:
         await client.wait_for_workers(2)
@@ -137,58 +136,58 @@
         assert (
             "distributed.scheduler" in log
             or "distributed.worker" in log
             or "Creating scheduler pod" in log
         )
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_dask_worker_name_env_variable(k8s_cluster, pod_spec, user_env):
     with dask.config.set({"kubernetes.name": "foo-{USER}-{uuid}"}):
         async with KubeCluster(pod_spec, **cluster_kwargs) as cluster:
             assert "foo-" + getpass.getuser() in cluster.name
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_diagnostics_link_env_variable(k8s_cluster, pod_spec, user_env):
     pytest.importorskip("bokeh")
     with dask.config.set({"distributed.dashboard.link": "foo-{USER}-{port}"}):
         async with KubeCluster(pod_spec, asynchronous=True) as cluster:
             port = cluster.forwarded_dashboard_port
 
             assert (
                 "foo-" + getpass.getuser() + "-" + str(port) in cluster.dashboard_link
             )
 
 
 @pytest.mark.skip(reason="Cannot run two closers locally as loadbalancer ports collide")
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_namespace(k8s_cluster, pod_spec):
     async with KubeCluster(pod_spec, **cluster_kwargs) as cluster:
         assert "dask" in cluster.name
         assert getpass.getuser() in cluster.name
         async with KubeCluster(pod_spec, **cluster_kwargs) as cluster2:
             assert cluster.name != cluster2.name
 
             cluster2.scale(1)
             while len(await cluster2.pods()) != 1:
                 await asyncio.sleep(0.1)
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_adapt(cluster):
     cluster.adapt()
     async with Client(cluster, asynchronous=True) as client:
         future = client.submit(lambda x: x + 1, 10)
         result = await future
         assert result == 11
 
 
 @pytest.mark.xfail(reason="The widget has changed upstream")
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_ipython_display(cluster):
     ipywidgets = pytest.importorskip("ipywidgets")
     cluster.scale(1)
     await cluster
     cluster._ipython_display_()
     box = cluster._cached_widget
     assert isinstance(box, ipywidgets.Widget)
@@ -197,26 +196,26 @@
 
     start = time()
     while "<td>1</td>" not in str(box):  # one worker in a table
         assert time() < start + 20
         await asyncio.sleep(0.5)
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_env(k8s_cluster, pod_spec):
     async with KubeCluster(pod_spec, env={"ABC": "DEF"}, **cluster_kwargs) as cluster:
         cluster.scale(1)
         await cluster
         async with Client(cluster, asynchronous=True) as client:
             await client.wait_for_workers(1)
             env = await client.run(lambda: dict(os.environ))
             assert all(v["ABC"] == "DEF" for v in env.values())
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_pod_from_yaml(k8s_cluster, docker_image):
     test_yaml = {
         "kind": "Pod",
         "metadata": {"labels": {"app": "dask", "component": "dask-worker"}},
         "spec": {
             "containers": [
                 {
@@ -250,15 +249,15 @@
                 # Ensure that inter-worker communication works well
                 futures = client.map(lambda x: x + 1, range(10))
                 total = client.submit(sum, futures)
                 assert (await total) == sum(map(lambda x: x + 1, range(10)))
                 assert all((await client.has_what()).values())
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_pod_expand_env_vars(k8s_cluster, docker_image):
     try:
         os.environ["FOO_IMAGE"] = docker_image
 
         test_yaml = {
             "kind": "Pod",
             "metadata": {"labels": {"app": "dask", "component": "dask-worker"}},
@@ -284,15 +283,15 @@
                 yaml.dump(test_yaml, f)
             async with KubeCluster(f.name, **cluster_kwargs) as cluster:
                 assert cluster.pod_template.spec.containers[0].image == docker_image
     finally:
         del os.environ["FOO_IMAGE"]
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_pod_template_dict(docker_image):
     spec = {
         "metadata": {},
         "restartPolicy": "Never",
         "spec": {
             "containers": [
                 {
@@ -326,15 +325,15 @@
             # Ensure that inter-worker communication works well
             futures = client.map(lambda x: x + 1, range(10))
             total = client.submit(sum, futures)
             assert (await total) == sum(map(lambda x: x + 1, range(10)))
             assert all((await client.has_what()).values())
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_pod_template_minimal_dict(k8s_cluster, docker_image):
     spec = {
         "spec": {
             "containers": [
                 {
                     "args": [
                         "dask-worker",
@@ -357,15 +356,15 @@
         cluster.adapt()
         async with Client(cluster, asynchronous=True) as client:
             future = client.submit(lambda x: x + 1, 10)
             result = await future
             assert result == 11
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_pod_template_from_conf(docker_image):
     spec = {
         "spec": {
             "containers": [{"name": KUBECLUSTER_CONTAINER_NAME, "image": docker_image}]
         }
     }
 
@@ -373,25 +372,25 @@
         async with KubeCluster(**cluster_kwargs) as cluster:
             assert (
                 cluster.pod_template.spec.containers[0].name
                 == KUBECLUSTER_CONTAINER_NAME
             )
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_pod_template_with_custom_container_name(docker_image):
     container_name = "my-custom-container"
     spec = {"spec": {"containers": [{"name": container_name, "image": docker_image}]}}
 
     with dask.config.set({"kubernetes.worker-template": spec}):
         async with KubeCluster(**cluster_kwargs) as cluster:
             assert cluster.pod_template.spec.containers[0].name == container_name
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_constructor_parameters(k8s_cluster, pod_spec):
     env = {"FOO": "BAR", "A": 1}
     async with KubeCluster(
         pod_spec, name="myname", env=env, **cluster_kwargs
     ) as cluster:
         pod = cluster.pod_template
         assert pod.metadata.namespace == get_current_namespace()
@@ -401,15 +400,15 @@
 
         var = [v for v in pod.spec.containers[0].env if v.name == "A"]
         assert var and var[0].value == "1"
 
         assert pod.metadata.generate_name == "myname"
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_reject_evicted_workers(cluster):
     cluster.scale(1)
     await cluster
 
     start = time()
     while len(cluster.scheduler_info["workers"]) != 1:
         await asyncio.sleep(0.1)
@@ -436,15 +435,15 @@
     # Wait until worker removal has been handled by cluster
     while len(cluster.workers) != 0:
         delta = time() - start
         assert delta < 60, f"Cluster failed to remove worker in {delta:.0f}s"
         await asyncio.sleep(0.1)
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_scale_up_down(cluster, client):
     np = pytest.importorskip("numpy")
     cluster.scale(2)
     await cluster
 
     start = time()
     while len(cluster.scheduler_info["workers"]) != 2:
@@ -467,15 +466,15 @@
 
     # assert set(cluster.scheduler_info["workers"]) == {b}
 
 
 @pytest.mark.xfail(
     reason="The delay between scaling up, starting a worker, and then scale down causes issues"
 )
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_scale_up_down_fast(cluster, client):
     cluster.scale(1)
     await cluster
 
     start = time()
     await client.wait_for_workers(1)
 
@@ -504,15 +503,15 @@
     # has never been deleted when rescaling the cluster and the result can
     # still be fetched back.
     assert worker in cluster.scheduler.tasks[future.key].who_has
     assert len(await future) == int(1e6)
 
 
 @pytest.mark.xfail(reason="scaling has some unfortunate state")
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_scale_down_pending(cluster, client, cleanup_namespaces):
     # Try to scale the cluster to use more pods than available
     nodes = (await cluster.core_api.list_node()).items
     max_pods = sum(int(node.status.allocatable["pods"]) for node in nodes)
     if max_pods > 50:
         # It's probably not reasonable to run this test against a large
         # kubernetes cluster.
@@ -567,15 +566,15 @@
 
     start = time()
     while len(cluster.scheduler_info["workers"]) > 0:
         await asyncio.sleep(0.1)
         assert time() < start + 60
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_automatic_startup(k8s_cluster, docker_image):
     test_yaml = {
         "kind": "Pod",
         "metadata": {"labels": {"foo": "bar"}},
         "spec": {
             "containers": [
                 {
@@ -596,43 +595,43 @@
         with open(fn, mode="w") as f:
             yaml.dump(test_yaml, f)
         with dask.config.set({"kubernetes.worker-template-path": fn}):
             async with KubeCluster(**cluster_kwargs) as cluster:
                 assert cluster.pod_template.metadata.labels["foo"] == "bar"
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_repr(cluster):
     for text in [repr(cluster), str(cluster)]:
         assert "Box" not in text
         assert (
             cluster.scheduler.address in text
             or cluster.scheduler.external_address in text
         )
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_escape_username(k8s_cluster, pod_spec, monkeypatch):
     monkeypatch.setenv("LOGNAME", "Foo!._")
 
     async with KubeCluster(pod_spec, **cluster_kwargs) as cluster:
         assert "foo" in cluster.name
         assert "!" not in cluster.name
         assert "." not in cluster.name
         assert "_" not in cluster.name
         assert "foo" in cluster.pod_template.metadata.labels["user"]
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_escape_name(k8s_cluster, pod_spec):
     async with KubeCluster(pod_spec, name="foo@bar", **cluster_kwargs) as cluster:
         assert "@" not in str(cluster.pod_template)
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_maximum(cluster):
     with dask.config.set({"kubernetes.count.max": 1}):
         with captured_logger("dask_kubernetes") as logger:
             cluster.scale(10)
             await cluster
 
             start = time()
@@ -699,23 +698,23 @@
     assert {
         "key": "example.org/toleration",
         "operator": "Exists",
         "effect": "NoSchedule",
     } in tolerations
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_auth_missing(k8s_cluster, pod_spec):
     with pytest.raises(kubernetes.config.ConfigException) as info:
         await KubeCluster(pod_spec, auth=[], **cluster_kwargs)
 
     assert "No authorization methods were provided" in str(info.value)
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_auth_tries_all_methods(k8s_cluster, pod_spec):
     fails = {"count": 0}
 
     class FailAuth(ClusterAuth):
         def load(self):
             fails["count"] += 1
             raise kubernetes.config.ConfigException("Fail #{count}".format(**fails))
@@ -726,67 +725,67 @@
     assert "Fail #3" in str(info.value)
     assert fails["count"] == 3
 
 
 @pytest.mark.xfail(
     reason="Updating the default client configuration is broken in kubernetes"
 )
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_auth_kubeconfig_with_filename():
     await KubeConfig(config_file=CONFIG_DEMO).load()
 
     # we've set the default configuration, so check that it is default
     config = kubernetes.client.Configuration()
     assert config.host == "https://1.2.3.4"
     assert config.cert_file == FAKE_CERT
     assert config.key_file == FAKE_KEY
     assert config.ssl_ca_cert == FAKE_CA
 
 
 @pytest.mark.xfail(
     reason="Updating the default client configuration is broken in kubernetes"
 )
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_auth_kubeconfig_with_context():
     await KubeConfig(config_file=CONFIG_DEMO, context="exp-scratch").load()
 
     # we've set the default configuration, so check that it is default
     config = kubernetes.client.Configuration()
     assert config.host == "https://5.6.7.8"
     assert config.api_key["authorization"] == "Basic {}".format(
         base64.b64encode(b"exp:some-password").decode("ascii")
     )
 
 
 @pytest.mark.xfail(
     reason="Updating the default client configuration is broken in async kubernetes"
 )
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_auth_explicit():
     await KubeAuth(
         host="https://9.8.7.6", username="abc", password="some-password"
     ).load()
 
     config = kubernetes.client.Configuration()
     assert config.host == "https://9.8.7.6"
     assert config.username == "abc"
     assert config.password == "some-password"
     assert config.get_basic_auth_token() == "Basic {}".format(
         base64.b64encode(b"abc:some-password").decode("ascii")
     )
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_start_with_workers(k8s_cluster, pod_spec):
     async with KubeCluster(pod_spec, n_workers=2, **cluster_kwargs) as cluster:
         async with Client(cluster, asynchronous=True) as client:
             await client.wait_for_workers(2)
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 @pytest.mark.xfail(reason="Flaky in CI and classic is deprecated anyway")
 async def test_adapt_delete(cluster, ns):
     """
     testing whether KubeCluster.adapt will bring
     back deleted worker pod (issue #244)
     """
     core_api = cluster.core_api
@@ -821,15 +820,15 @@
     start = time()
     while len(cluster.scheduler_info["workers"]) != 2:
         await asyncio.sleep(0.1)
         assert time() < start + 60
     assert len(cluster.scheduler_info["workers"]) == 2
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 @pytest.mark.xfail(reason="Failing in CI with FileNotFoundError")
 async def test_auto_refresh(cluster):
     config = {
         "apiVersion": "v1",
         "clusters": [
             {
                 "cluster": {"certificate-authority-data": "", "server": ""},
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/test_sync.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/classic/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/cli/cli.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/common/auth.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/common/auth.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/common/networking.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/common/networking.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/common/objects.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/common/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/common/tests/test_kind.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/common/tests/test_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dask_kubernetes.common.utils import get_current_namespace
 
 
 def test_config_detection(k8s_cluster):
     assert b"pytest-kind" in check_output(["kubectl", "config", "current-context"])
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 @pytest.mark.xfail(reason="Has asyncio issues on CI")
 async def test_auth(k8s_cluster):
     await ClusterAuth.load_first(ClusterAuth.DEFAULT)
     core_v1_api = kubernetes.client.CoreV1Api()
     request = await core_v1_api.list_namespace()
     assert get_current_namespace() in [
         namespace.metadata.name for namespace in request.items
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/common/tests/test_objects.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/common/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/common/utils.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/common/utils.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/conftest.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,14 @@
         )
     else:
         yield
 
 
 @pytest.fixture(scope="session", autouse=True)
 def customresources(k8s_cluster):
-
     temp_dir = tempfile.TemporaryDirectory()
     crd_path = os.path.join(DIR, "operator", "customresources")
 
     def run_generate(crd_path, patch_path, temp_path):
         subprocess.run(
             ["k8s-crd-resolver", "-r", "-j", patch_path, crd_path, temp_path],
             check=True,
@@ -123,9 +122,14 @@
             os.path.join(crd_path, f"{crd}.yaml"),
             os.path.join(crd_path, f"{crd}.patch.yaml"),
             os.path.join(temp_dir.name, f"{crd}.yaml"),
         )
 
     k8s_cluster.kubectl("apply", "-f", temp_dir.name)
     yield
-    k8s_cluster.kubectl("delete", "-f", temp_dir.name)
+    k8s_cluster.kubectl("delete", "--wait=false", "-f", temp_dir.name)
     temp_dir.cleanup()
+
+
+@pytest.fixture
+def anyio_backend():
+    return "asyncio"
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/experimental/__init__.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/helm/helmcluster.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/helm/helmcluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/helm/tests/test_helm.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/helm/tests/test_helm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-import pytest_asyncio
 
 import subprocess
 import os.path
 
 import dask.config
 from distributed import Client
 from distributed.core import Status
@@ -91,15 +90,15 @@
         ],
         check=True,
     )
     yield release_name
     subprocess.run(["helm", "delete", "-n", test_namespace, release_name], check=True)
 
 
-@pytest_asyncio.fixture
+@pytest.fixture
 async def cluster(k8s_cluster, release, test_namespace):
     from dask_kubernetes import HelmCluster
 
     tries = 5
     while True:
         try:
             cluster = await HelmCluster(
@@ -150,29 +149,29 @@
 def test_raises_on_non_existant_release(k8s_cluster):
     from dask_kubernetes import HelmCluster
 
     with pytest.raises(RuntimeError):
         HelmCluster(release_name="nosuchrelease", namespace="default")
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_create_helm_cluster(cluster, release_name):
     assert cluster.status == Status.running
     assert cluster.release_name == release_name
     assert "id" in cluster.scheduler_info
 
 
 def test_create_sync_helm_cluster(sync_cluster, release_name):
     cluster = sync_cluster
     assert cluster.status == Status.running
     assert cluster.release_name == release_name
     assert "id" in cluster.scheduler_info
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_scale_cluster(cluster):
     # Scale up
     await cluster.scale(4)
     await cluster  # Wait for workers
     assert len(cluster.scheduler_info["workers"]) == 4
 
     # Scale down
@@ -193,35 +192,35 @@
     # Scaling a non-existent eorker group 'bar' raises a ValueError
     import kubernetes_asyncio as kubernetes
 
     with pytest.raises((ValueError, kubernetes.client.exceptions.ApiException)):
         await cluster.scale(2, worker_group="bar")
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_logs(cluster):
     from distributed.utils import Logs
 
     logs = await cluster.get_logs()
 
     assert isinstance(logs, Logs)
     assert any(["scheduler" in log for log in logs])
     assert any(["worker" in log for log in logs])
 
     [scheduler_logs] = [logs[log] for log in logs if "scheduler" in log]
     assert "Scheduler at:" in scheduler_logs
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_adaptivity_warning(cluster):
     with pytest.raises(NotImplementedError):
         await cluster.adapt(minimum=3, maximum=3)
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 @pytest.mark.xfail(reason="Has asyncio issues on CI")
 async def test_discovery(release, release_name):
     discovery = "helmcluster"
     methods = list_discovery_methods()
 
     assert discovery in methods
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/kubernetes.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/kubernetes.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/_objects.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/controller.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 from contextlib import suppress
 from datetime import datetime
 from uuid import uuid4
 
 import aiohttp
 import kopf
 import kr8s
-from kr8s.asyncio.objects import Pod
-import kubernetes_asyncio as kubernetes
+from kr8s.asyncio.objects import Pod, Deployment, Service
 from importlib_metadata import entry_points
-from kubernetes_asyncio.client import ApiException
 
 from dask_kubernetes.operator._objects import (
     DaskCluster,
     DaskAutoscaler,
     DaskWorkerGroup,
     DaskJob,
 )
@@ -284,87 +282,60 @@
 
 @kopf.on.field("daskcluster.kubernetes.dask.org", field="status.phase", new="Created")
 async def daskcluster_create_components(
     spec, name, namespace, logger, patch, meta, **kwargs
 ):
     """When the DaskCluster status.phase goes into Created create the cluster components."""
     logger.info("Creating Dask cluster components.")
-    async with kubernetes.client.api_client.ApiClient() as api_client:
-        api = kubernetes.client.CoreV1Api(api_client)
-        custom_api = kubernetes.client.CustomObjectsApi(api_client)
 
-        annotations = _get_annotations(meta)
-        labels = _get_labels(meta)
-        scheduler_spec = spec.get("scheduler", {})
-        if "metadata" in scheduler_spec:
-            if "annotations" in scheduler_spec["metadata"]:
-                annotations.update(**scheduler_spec["metadata"]["annotations"])
-            if "labels" in scheduler_spec["metadata"]:
-                labels.update(**scheduler_spec["metadata"]["labels"])
-        data = build_scheduler_deployment_spec(
-            name, namespace, scheduler_spec.get("spec"), annotations, labels
-        )
-        kopf.adopt(data)
-        pod = await api.list_namespaced_pod(
-            namespace=namespace,
-            label_selector=f"dask.org/component=scheduler,dask.org/cluster-name={name}",
-        )
-        if not pod.items:
-            await kubernetes.client.AppsV1Api(api_client).create_namespaced_deployment(
-                namespace=namespace,
-                body=data,
-            )
-            logger.info(
-                f"Scheduler deployment {data['metadata']['name']} created in {namespace}."
-            )
+    # Create scheduler deployment
+    annotations = _get_annotations(meta)
+    labels = _get_labels(meta)
+    scheduler_spec = spec.get("scheduler", {})
+    if "metadata" in scheduler_spec:
+        if "annotations" in scheduler_spec["metadata"]:
+            annotations.update(**scheduler_spec["metadata"]["annotations"])
+        if "labels" in scheduler_spec["metadata"]:
+            labels.update(**scheduler_spec["metadata"]["labels"])
+    data = build_scheduler_deployment_spec(
+        name, namespace, scheduler_spec.get("spec"), annotations, labels
+    )
+    kopf.adopt(data)
+    scheduler_deployment = await Deployment(data, namespace=namespace)
+    if not await scheduler_deployment.exists():
+        await scheduler_deployment.create()
+    logger.info(
+        f"Scheduler deployment {scheduler_deployment.name} created in {namespace}."
+    )
+
+    # Create scheduler service
+    data = build_scheduler_service_spec(
+        name, scheduler_spec.get("service"), annotations, labels
+    )
+    kopf.adopt(data)
+    scheduler_service = await Service(data, namespace=namespace)
+    if not await scheduler_service.exists():
+        await scheduler_service.create()
+    logger.info(f"Scheduler service {data['metadata']['name']} created in {namespace}.")
+
+    # Create default worker group
+    worker_spec = spec.get("worker", {})
+    annotations = _get_annotations(meta)
+    labels = _get_labels(meta)
+    if "metadata" in worker_spec:
+        if "annotations" in worker_spec["metadata"]:
+            annotations.update(**worker_spec["metadata"]["annotations"])
+        if "labels" in worker_spec["metadata"]:
+            labels.update(**worker_spec["metadata"]["labels"])
+    data = build_default_worker_group_spec(name, worker_spec, annotations, labels)
+    worker_group = await DaskWorkerGroup(data, namespace=namespace)
+    if not await worker_group.exists():
+        await worker_group.create()
+    logger.info(f"Worker group {data['metadata']['name']} created in {namespace}.")
 
-        data = build_scheduler_service_spec(
-            name, scheduler_spec.get("service"), annotations, labels
-        )
-        kopf.adopt(data)
-        service = await api.list_namespaced_service(
-            namespace=namespace,
-            label_selector=f"dask.org/component=scheduler,dask.org/cluster-name={name}",
-        )
-        if not service.items:
-            await api.create_namespaced_service(
-                namespace=namespace,
-                body=data,
-            )
-        logger.info(
-            f"Scheduler service {data['metadata']['name']} created in {namespace}."
-        )
-
-        worker_spec = spec.get("worker", {})
-        annotations = _get_annotations(meta)
-        labels = _get_labels(meta)
-        if "metadata" in worker_spec:
-            if "annotations" in worker_spec["metadata"]:
-                annotations.update(**worker_spec["metadata"]["annotations"])
-            if "labels" in worker_spec["metadata"]:
-                labels.update(**worker_spec["metadata"]["labels"])
-        data = build_default_worker_group_spec(name, worker_spec, annotations, labels)
-        worker_group = await custom_api.list_namespaced_custom_object(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskworkergroups",
-            namespace=namespace,
-            label_selector=f"dask.org/component=workergroup,dask.org/cluster-name={name}",
-        )
-        if not worker_group["items"]:
-            await custom_api.create_namespaced_custom_object(
-                group="kubernetes.dask.org",
-                version="v1",
-                plural="daskworkergroups",
-                namespace=namespace,
-                body=data,
-            )
-            logger.info(
-                f"Worker group {data['metadata']['name']} created in {namespace}."
-            )
     patch.status["phase"] = "Pending"
 
 
 @kopf.on.field("service", field="status", labels={"dask.org/component": "scheduler"})
 async def handle_scheduler_service_status(
     spec, labels, status, namespace, logger, **kwargs
 ):
@@ -379,46 +350,26 @@
     cluster = await DaskCluster.get(
         labels["dask.org/cluster-name"], namespace=namespace
     )
     await cluster.patch({"status": {"phase": phase}})
 
 
 @kopf.on.create("daskworkergroup.kubernetes.dask.org")
-async def daskworkergroup_create(spec, name, namespace, logger, **kwargs):
-    async with kubernetes.client.api_client.ApiClient() as api_client:
-        api = kubernetes.client.CustomObjectsApi(api_client)
-        cluster = await api.get_namespaced_custom_object(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskclusters",
-            namespace=namespace,
-            name=spec["cluster"],
-        )
-        new_spec = dict(spec)
-        kopf.adopt(new_spec, owner=cluster)
-        api.api_client.set_default_header(
-            "content-type", "application/merge-patch+json"
-        )
-        await api.patch_namespaced_custom_object(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskworkergroups",
-            namespace=namespace,
-            name=name,
-            body=new_spec,
-        )
-        logger.info(f"Successfully adopted by {spec['cluster']}")
+async def daskworkergroup_create(body, namespace, logger, **kwargs):
+    wg = await DaskWorkerGroup(body, namespace=namespace)
+    cluster = await wg.cluster()
+    await cluster.adopt(wg)
+    logger.info(f"Successfully adopted by {cluster.name}")
 
     del kwargs["new"]
     await daskworkergroup_replica_update(
-        spec=spec,
-        name=name,
-        namespace=namespace,
+        body=body,
         logger=logger,
-        new=spec["worker"]["replicas"],
+        new=wg.replicas,
+        namespace=namespace,
         **kwargs,
     )
 
 
 async def retire_workers(
     n_workers, scheduler_service_name, worker_group_name, namespace, logger
 ):
@@ -587,111 +538,86 @@
 
 
 @kopf.on.field("daskworkergroup.kubernetes.dask.org", field="spec.worker.replicas")
 async def daskworkergroup_replica_update(
     name, namespace, meta, spec, new, body, logger, **kwargs
 ):
     cluster_name = spec["cluster"]
+    wg = await DaskWorkerGroup(body, namespace=namespace)
+    try:
+        cluster = await wg.cluster()
+    except kr8s.NotFoundError:
+        # No need to scale if cluster is deleted, pods will be cleaned up
+        return
 
     # Replica updates can come in quick succession and the changes must be applied atomically to ensure
     # the number of workers ends in the correct state
     async with worker_group_scale_locks[f"{namespace}/{name}"]:
-        async with kubernetes.client.api_client.ApiClient() as api_client:
-            customobjectsapi = kubernetes.client.CustomObjectsApi(api_client)
-            corev1api = kubernetes.client.CoreV1Api(api_client)
-
-            try:
-                cluster = await customobjectsapi.get_namespaced_custom_object(
-                    group="kubernetes.dask.org",
-                    version="v1",
-                    plural="daskclusters",
-                    namespace=namespace,
-                    name=cluster_name,
-                )
-            except ApiException as e:
-                if e.status == 404:
-                    # No need to scale if worker group is deleted, pods will be cleaned up
-                    return
-                else:
-                    raise e
-
-            cluster_labels = cluster.get("metadata", {}).get("labels", {})
-
-            workers = await corev1api.list_namespaced_pod(
+        current_workers = len(
+            await kr8s.asyncio.get(
+                "deployments",
                 namespace=namespace,
-                label_selector=f"dask.org/workergroup-name={name}",
-            )
-            current_workers = len(
-                [w for w in workers.items if w.status.phase != "Terminating"]
-            )
-            desired_workers = new
-            workers_needed = desired_workers - current_workers
-            labels = _get_labels(meta)
-            annotations = _get_annotations(meta)
-            worker_spec = spec["worker"]
-            if "metadata" in worker_spec:
-                if "annotations" in worker_spec["metadata"]:
-                    annotations.update(**worker_spec["metadata"]["annotations"])
-                if "labels" in worker_spec["metadata"]:
-                    labels.update(**worker_spec["metadata"]["labels"])
-
-            SIZE = int(
-                dask.config.get("kubernetes.controller.worker-allocation.batch-size")
-                or 0
+                label_selector={"dask.org/workergroup-name": name},
             )
-            DELAY = int(
-                dask.config.get("kubernetes.controller.worker-allocation.delay") or 0
-            )
-            batch_size = min(workers_needed, SIZE) if SIZE else workers_needed
-            if workers_needed > 0:
-                for _ in range(batch_size):
-                    data = build_worker_deployment_spec(
-                        worker_group_name=name,
-                        namespace=namespace,
-                        cluster_name=cluster_name,
-                        uuid=uuid4().hex[:10],
-                        pod_spec=worker_spec["spec"],
-                        annotations=annotations,
-                        labels=labels,
-                    )
-                    kopf.adopt(data, owner=body)
-                    kopf.label(data, labels=cluster_labels)
-                    await kubernetes.client.AppsV1Api(
-                        api_client
-                    ).create_namespaced_deployment(
-                        namespace=namespace,
-                        body=data,
-                    )
-            if SIZE:
-                if workers_needed > SIZE:
-                    raise kopf.TemporaryError(
-                        "Added maximum number of workers for this batch but still need to create more workers, "
-                        f"waiting for {DELAY} seconds before continuing.",
-                        delay=DELAY,
-                    )
-            logger.info(f"Scaled worker group {name} up to {desired_workers} workers.")
-            if workers_needed < 0:
-                worker_ids = await retire_workers(
-                    n_workers=-workers_needed,
-                    scheduler_service_name=f"{cluster_name}-scheduler",
+        )
+        desired_workers = new
+        workers_needed = desired_workers - current_workers
+        labels = _get_labels(meta)
+        annotations = _get_annotations(meta)
+        worker_spec = spec["worker"]
+        if "metadata" in worker_spec:
+            if "annotations" in worker_spec["metadata"]:
+                annotations.update(**worker_spec["metadata"]["annotations"])
+            if "labels" in worker_spec["metadata"]:
+                labels.update(**worker_spec["metadata"]["labels"])
+
+        batch_size = int(
+            dask.config.get("kubernetes.controller.worker-allocation.batch-size") or 0
+        )
+        batch_size = min(workers_needed, batch_size) if batch_size else workers_needed
+        batch_delay = int(
+            dask.config.get("kubernetes.controller.worker-allocation.delay") or 0
+        )
+        if workers_needed > 0:
+            for _ in range(batch_size):
+                data = build_worker_deployment_spec(
                     worker_group_name=name,
                     namespace=namespace,
-                    logger=logger,
-                )
-                logger.info(f"Workers to close: {worker_ids}")
-                for wid in worker_ids:
-                    await kubernetes.client.AppsV1Api(
-                        api_client
-                    ).delete_namespaced_deployment(
-                        name=wid,
-                        namespace=namespace,
-                    )
-                logger.info(
-                    f"Scaled worker group {name} down to {desired_workers} workers."
+                    cluster_name=cluster_name,
+                    uuid=uuid4().hex[:10],
+                    pod_spec=worker_spec["spec"],
+                    annotations=annotations,
+                    labels=labels,
                 )
+                kopf.adopt(data, owner=body)
+                kopf.label(data, labels=cluster.labels)
+                worker_deployment = await Deployment(data, namespace=namespace)
+                await worker_deployment.create()
+        if workers_needed > batch_size:
+            raise kopf.TemporaryError(
+                "Added maximum number of workers for this batch but still need to create more workers, "
+                f"waiting for {batch_delay} seconds before continuing.",
+                delay=batch_delay,
+            )
+        logger.info(f"Scaled worker group {name} up to {desired_workers} workers.")
+        if workers_needed < 0:
+            worker_ids = await retire_workers(
+                n_workers=-workers_needed,
+                scheduler_service_name=f"{cluster_name}-scheduler",
+                worker_group_name=name,
+                namespace=namespace,
+                logger=logger,
+            )
+            logger.info(f"Workers to close: {worker_ids}")
+            for wid in worker_ids:
+                worker_deployment = await Deployment(wid, namespace=namespace)
+                await worker_deployment.delete()
+            logger.info(
+                f"Scaled worker group {name} down to {desired_workers} workers."
+            )
 
 
 @kopf.on.delete("daskworkergroup.kubernetes.dask.org", optional=True)
 async def daskworkergroup_remove(name, namespace, **kwargs):
     lock_key = f"{name}/{namespace}"
     if lock_key in worker_group_scale_locks:
         del worker_group_scale_locks[lock_key]
@@ -706,70 +632,59 @@
 @kopf.on.field(
     "daskjob.kubernetes.dask.org", field="status.jobStatus", new="JobCreated"
 )
 async def daskjob_create_components(
     spec, name, namespace, logger, patch, meta, **kwargs
 ):
     logger.info("Creating Dask job components.")
-    async with kubernetes.client.api_client.ApiClient() as api_client:
-        customobjectsapi = kubernetes.client.CustomObjectsApi(api_client)
-        corev1api = kubernetes.client.CoreV1Api(api_client)
-
-        cluster_name = f"{name}"
-        labels = _get_labels(meta)
-        annotations = _get_annotations(meta)
-        cluster_spec = spec["cluster"]
-        if "metadata" in cluster_spec:
-            if "annotations" in cluster_spec["metadata"]:
-                annotations.update(**cluster_spec["metadata"]["annotations"])
-            if "labels" in cluster_spec["metadata"]:
-                labels.update(**cluster_spec["metadata"]["labels"])
-        cluster_spec = build_cluster_spec(
-            cluster_name,
-            cluster_spec["spec"]["worker"],
-            cluster_spec["spec"]["scheduler"],
-            annotations,
-            labels,
-        )
-        kopf.adopt(cluster_spec)
-        await customobjectsapi.create_namespaced_custom_object(
-            group="kubernetes.dask.org",
-            version="v1",
-            plural="daskclusters",
-            namespace=namespace,
-            body=cluster_spec,
-        )
-        logger.info(
-            f"Cluster {cluster_spec['metadata']['name']} for job {name} created in {namespace}."
-        )
-
-        labels = _get_labels(meta)
-        annotations = _get_annotations(meta)
-        job_spec = spec["job"]
-        if "metadata" in job_spec:
-            if "annotations" in job_spec["metadata"]:
-                annotations.update(**job_spec["metadata"]["annotations"])
-            if "labels" in job_spec["metadata"]:
-                labels.update(**job_spec["metadata"]["labels"])
-        job_pod_spec = build_job_pod_spec(
-            job_name=name,
-            cluster_name=cluster_name,
-            namespace=namespace,
-            spec=job_spec["spec"],
-            annotations=annotations,
-            labels=labels,
-        )
-        kopf.adopt(job_pod_spec)
-        await corev1api.create_namespaced_pod(
-            namespace=namespace,
-            body=job_pod_spec,
-        )
-        patch.status["clusterName"] = cluster_name
-        patch.status["jobStatus"] = "ClusterCreated"
-        patch.status["jobRunnerPodName"] = get_job_runner_pod_name(name)
+    cluster_name = f"{name}"
+    labels = _get_labels(meta)
+    annotations = _get_annotations(meta)
+    cluster_spec = spec["cluster"]
+    if "metadata" in cluster_spec:
+        if "annotations" in cluster_spec["metadata"]:
+            annotations.update(**cluster_spec["metadata"]["annotations"])
+        if "labels" in cluster_spec["metadata"]:
+            labels.update(**cluster_spec["metadata"]["labels"])
+    cluster_spec = build_cluster_spec(
+        cluster_name,
+        cluster_spec["spec"]["worker"],
+        cluster_spec["spec"]["scheduler"],
+        annotations,
+        labels,
+    )
+    kopf.adopt(cluster_spec)
+    cluster = await DaskCluster(cluster_spec, namespace=namespace)
+    await cluster.create()
+    logger.info(
+        f"Cluster {cluster_spec['metadata']['name']} for job {name} created in {namespace}."
+    )
+
+    labels = _get_labels(meta)
+    annotations = _get_annotations(meta)
+    job_spec = spec["job"]
+    if "metadata" in job_spec:
+        if "annotations" in job_spec["metadata"]:
+            annotations.update(**job_spec["metadata"]["annotations"])
+        if "labels" in job_spec["metadata"]:
+            labels.update(**job_spec["metadata"]["labels"])
+    job_pod_spec = build_job_pod_spec(
+        job_name=name,
+        cluster_name=cluster_name,
+        namespace=namespace,
+        spec=job_spec["spec"],
+        annotations=annotations,
+        labels=labels,
+    )
+    kopf.adopt(job_pod_spec)
+    job_pod = await Pod(job_pod_spec, namespace=namespace)
+    await job_pod.create()
+    patch.status["clusterName"] = cluster_name
+    patch.status["jobStatus"] = "ClusterCreated"
+    patch.status["jobRunnerPodName"] = get_job_runner_pod_name(name)
 
 
 @kopf.on.field(
     "pod",
     field="status.phase",
     labels={"dask.org/component": "job-runner"},
     new="Running",
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/test_controller.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/controller/tests/test_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
     assert runner.exit_code == 0
     assert runner.exception is None
     assert "Plugin 'noop' running." in runner.stdout
 
 
 @pytest.mark.timeout(180)
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_simplecluster(k8s_cluster, kopf_runner, gen_cluster):
     with kopf_runner as runner:
         async with gen_cluster() as (cluster_name, ns):
             scheduler_deployment_name = "simple-scheduler"
             worker_pod_name = "simple-default-worker"
             service_name = "simple-scheduler"
 
@@ -243,15 +243,15 @@
                     "jsonpath='{.items[0].metadata.labels}'",
                 )[1:-1]
             )
             assert _EXPECTED_LABELS.items() <= worker_labels.items()
             assert "worker-sublabel" in workergroup_labels
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_scalesimplecluster(k8s_cluster, kopf_runner, gen_cluster):
     with kopf_runner as runner:
         async with gen_cluster() as (cluster_name, ns):
             scheduler_deployment_name = "simple-scheduler"
             worker_pod_name = "simple-default-worker"
             service_name = "simple-scheduler"
             while scheduler_deployment_name not in k8s_cluster.kubectl(
@@ -288,15 +288,15 @@
                     )
                     # TODO: Currently, doesn't test anything. Need to add optional
                     #       argument to wait when removing workers once distributed
                     #       PR github.com/dask/distributed/pull/6377 is merged.
                     await client.wait_for_workers(3)
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_scalesimplecluster_from_cluster_spec(
     k8s_cluster, kopf_runner, gen_cluster
 ):
     with kopf_runner as runner:
         async with gen_cluster() as (cluster_name, ns):
             scheduler_deployment_name = "simple-scheduler"
             worker_pod_name = "simple-default-worker"
@@ -335,15 +335,15 @@
                     )
                     # TODO: Currently, doesn't test anything. Need to add optional
                     #       argument to wait when removing workers once distributed
                     #       PR github.com/dask/distributed/pull/6377 is merged.
                     await client.wait_for_workers(3)
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_recreate_scheduler_pod(k8s_cluster, kopf_runner, gen_cluster):
     with kopf_runner as runner:
         async with gen_cluster() as (cluster_name, ns):
             scheduler_deployment_name = "simple-scheduler"
             worker_pod_name = "simple-default-worker"
             service_name = "simple-scheduler"
             while scheduler_deployment_name not in k8s_cluster.kubectl(
@@ -373,15 +373,15 @@
                 "--timeout=60s",
             )
             assert scheduler_deployment_name in k8s_cluster.kubectl(
                 "get", "pods", "-n", ns
             )
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_recreate_worker_pods(k8s_cluster, kopf_runner, gen_cluster):
     with kopf_runner as runner:
         async with gen_cluster() as (cluster_name, ns):
             cluster = await DaskCluster.get(cluster_name, namespace=ns)
             # Get the default worker group
             while not (wgs := await cluster.worker_groups()):
                 await asyncio.sleep(0.1)
@@ -402,15 +402,15 @@
                 await asyncio.sleep(0.1)
             # Wait for worker Pods to be ready
             await asyncio.gather(
                 *[pod.wait(conditions="condition=Ready", timeout=60) for pod in pods]
             )
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_simplecluster_batched_worker_deployments(
     k8s_cluster, kopf_runner, gen_cluster
 ):
     with kopf_runner as runner:
         with dask.config.set(
             {
                 "kubernetes.controller.worker-allocation.batch-size": 1,
@@ -488,15 +488,15 @@
         "jobRunnerPodName",
         "jobStatus",
         "startTime",
         "endTime",
     }
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_job(k8s_cluster, kopf_runner, gen_job):
     with kopf_runner as runner:
         async with gen_job("simplejob.yaml") as (job, ns):
             assert job
 
             runner_name = f"{job}-runner"
 
@@ -559,15 +559,15 @@
             job_status = _get_job_status(k8s_cluster, ns)
             _assert_final_job_status(job, job_status, "Successful")
 
     assert "A DaskJob has been created" in runner.stdout
     assert "Job succeeded, deleting Dask cluster." in runner.stdout
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_failed_job(k8s_cluster, kopf_runner, gen_job):
     with kopf_runner as runner:
         async with gen_job("failedjob.yaml") as (job, ns):
             assert job
 
             runner_name = f"{job}-runner"
 
@@ -617,15 +617,15 @@
             job_status = _get_job_status(k8s_cluster, ns)
             _assert_final_job_status(job, job_status, "Failed")
 
     assert "A DaskJob has been created" in runner.stdout
     assert "Job failed, deleting Dask cluster." in runner.stdout
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_object_dask_cluster(k8s_cluster, kopf_runner, gen_cluster):
     with kopf_runner as runner:
         async with gen_cluster() as (cluster_name, ns):
             cluster = await DaskCluster.get(cluster_name, namespace=ns)
 
             worker_groups = []
             while not worker_groups:
@@ -641,15 +641,15 @@
             scheduler_deployment = await cluster.scheduler_deployment()
             assert isinstance(scheduler_deployment, Deployment)
 
             scheduler_service = await cluster.scheduler_service()
             assert isinstance(scheduler_service, Service)
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_object_dask_worker_group(k8s_cluster, kopf_runner, gen_cluster):
     with kopf_runner as runner:
         async with gen_cluster() as (cluster_name, ns):
             cluster = await DaskCluster.get(cluster_name, namespace=ns)
 
             worker_groups = []
             while not worker_groups:
@@ -670,15 +670,15 @@
                 deployments = await wg.deployments()
                 await asyncio.sleep(0.1)
             assert all([isinstance(d, Deployment) for d in deployments])
 
             assert (await wg.cluster()).name == cluster.name
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 @pytest.mark.skip(reason="Flaky in CI")
 async def test_object_dask_job(k8s_cluster, kopf_runner, gen_job):
     with kopf_runner as runner:
         async with gen_job("simplejob.yaml") as (job_name, ns):
             job = await DaskJob.get(job_name, namespace=ns)
 
             job_pod = await job.pod()
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskautoscaler.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskcluster.patch.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskcluster.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskcluster.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskjob.patch.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskjob.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskjob.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskworkergroup.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/templates.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/customresources/templates.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/chartpress.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/chartpress.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -17,21 +17,22 @@
   cluster: true # Creates a ClusterRole if true, else create a namespaced Role
 
 podAnnotations: {}  # Extra annotations for the operator pod
 
 podSecurityContext: {}  # Security context for the operator pod
   # fsGroup: 2000
 
-securityContext: {}  # Security context for the operator container
-  # capabilities:
-  #   drop:
-  #   - ALL
+securityContext:  # Security context for the operator container
+  capabilities:
+    drop:
+    - ALL
+  runAsNonRoot: true
+  runAsUser: 1000
+  allowPrivilegeEscalation: false
   # readOnlyRootFilesystem: true
-  # runAsNonRoot: true
-  # runAsUser: 1000
 
 resources: {}  # Resources for the operator pod
   # We usually recommend not to specify default resources and to leave this as a conscious
   # choice for the user. This also increases chances charts run on environments with little
   # resources, such as Minikube. If you do want to specify resources, uncomment the following
   # lines, adjust them as necessary, and remove the curly braces after 'resources:'.
   # limits:
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/discovery.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/kubecluster.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/conftest.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/tests/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import pytest
-import pytest_asyncio
 
 import dask.config
 
 from dask_kubernetes.operator import KubeCluster
 
 
 @pytest.fixture
 def cluster(kopf_runner, docker_image):
     with dask.config.set({"kubernetes.name": "foo-{uuid}"}):
         with kopf_runner:
             with KubeCluster(image=docker_image, n_workers=1) as cluster:
                 yield cluster
 
 
-@pytest_asyncio.fixture
+@pytest.fixture
 async def async_cluster(kopf_runner, docker_image):
     with dask.config.set({"kubernetes.name": "foo-{uuid}"}):
         with kopf_runner:
             async with KubeCluster(
                 image=docker_image, n_workers=1, asynchronous=True
             ) as cluster:
                 yield cluster
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/test_discovery.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/tests/test_discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 from dask.distributed import Client
 from dask_kubernetes.operator import KubeCluster
 from dask_kubernetes.operator import discover
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_discovery(async_cluster):
     clusters = [name async for name, _ in discover()]
     assert async_cluster.name in clusters
     async with KubeCluster.from_name(async_cluster.name, asynchronous=True) as cluster2:
         assert async_cluster == cluster2
         assert "id" in cluster2.scheduler_info
         async with Client(cluster2, asynchronous=True) as client:
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py` & `dask-kubernetes-2023.7.3/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     with Client(cluster) as client:
         client.scheduler_info()
         cluster.scale(1)
         assert client.submit(lambda x: x + 1, 10).result() == 11
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_kubecluster_async(kopf_runner, docker_image):
     with kopf_runner:
         async with KubeCluster(
             name="async",
             image=docker_image,
             n_workers=1,
             asynchronous=True,
@@ -92,15 +92,15 @@
         ) as cluster2:
             with Client(cluster1) as client1, Client(cluster2) as client2:
                 assert cluster1.loop is cluster2.loop is client1.loop is client2.loop
                 assert client1.submit(lambda x: x + 1, 10).result() == 11
                 assert client2.submit(lambda x: x + 1, 10).result() == 11
 
 
-@pytest.mark.asyncio
+@pytest.mark.anyio
 async def test_cluster_from_name(kopf_runner, docker_image, ns):
     with kopf_runner:
         async with KubeCluster(
             name="abc",
             namespace=ns,
             image=docker_image,
             n_workers=1,
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/PKG-INFO` & `dask-kubernetes-2023.7.3/dask_kubernetes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2023.7.2
+Version: 2023.7.3
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/SOURCES.txt` & `dask-kubernetes-2023.7.3/dask_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/setup.cfg` & `dask-kubernetes-2023.7.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -73,16 +73,15 @@
 00000480: 696c 6420 3d20 6461 736b 5f6b 7562 6572  ild = dask_kuber
 00000490: 6e65 7465 732f 5f76 6572 7369 6f6e 2e70  netes/_version.p
 000004a0: 790a 7461 675f 7072 6566 6978 203d 200a  y.tag_prefix = .
 000004b0: 7061 7265 6e74 6469 725f 7072 6566 6978  parentdir_prefix
 000004c0: 203d 2064 6173 6b2d 6b75 6265 726e 6574   = dask-kubernet
 000004d0: 6573 2d0a 0a5b 746f 6f6c 3a70 7974 6573  es-..[tool:pytes
 000004e0: 745d 0a61 6464 6f70 7473 203d 202d 7620  t].addopts = -v 
-000004f0: 2d2d 6b65 6570 2d63 6c75 7374 6572 202d  --keep-cluster -
-00000500: 2d64 7572 6174 696f 6e73 3d31 300a 7469  -durations=10.ti
-00000510: 6d65 6f75 7420 3d20 3630 0a74 696d 656f  meout = 60.timeo
-00000520: 7574 5f66 756e 635f 6f6e 6c79 203d 2074  ut_func_only = t
-00000530: 7275 650a 7265 7275 6e73 203d 2033 0a61  rue.reruns = 3.a
-00000540: 7379 6e63 696f 5f6d 6f64 6520 3d20 7374  syncio_mode = st
-00000550: 7269 6374 0a0a 5b65 6767 5f69 6e66 6f5d  rict..[egg_info]
-00000560: 0a74 6167 5f62 7569 6c64 203d 200a 7461  .tag_build = .ta
-00000570: 675f 6461 7465 203d 2030 0a0a            g_date = 0..
+000004f0: 2d78 202d 2d6b 6565 702d 636c 7573 7465  -x --keep-cluste
+00000500: 7220 2d2d 6475 7261 7469 6f6e 733d 3130  r --durations=10
+00000510: 0a74 696d 656f 7574 203d 2036 300a 7469  .timeout = 60.ti
+00000520: 6d65 6f75 745f 6675 6e63 5f6f 6e6c 7920  meout_func_only 
+00000530: 3d20 7472 7565 0a72 6572 756e 7320 3d20  = true.reruns = 
+00000540: 330a 0a5b 6567 675f 696e 666f 5d0a 7461  3..[egg_info].ta
+00000550: 675f 6275 696c 6420 3d20 0a74 6167 5f64  g_build = .tag_d
+00000560: 6174 6520 3d20 300a 0a                   ate = 0..
```

### Comparing `dask-kubernetes-2023.7.2/setup.py` & `dask-kubernetes-2023.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.2/versioneer.py` & `dask-kubernetes-2023.7.3/versioneer.py`

 * *Files identical despite different names*

