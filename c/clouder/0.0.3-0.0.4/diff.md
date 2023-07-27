# Comparing `tmp/clouder-0.0.3.tar.gz` & `tmp/clouder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clouder-0.0.3.tar", last modified: Sat May  8 14:23:16 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `clouder-0.0.3.tar` & `clouder-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,196 @@
-drwxr-xr-x   0 echarles   (501) staff       (20)        0 2021-05-08 14:23:16.329803 clouder-0.0.3/
--rw-r--r--   0 echarles   (501) staff       (20)      420 2021-05-08 14:23:16.329536 clouder-0.0.3/PKG-INFO
--rwxr-xr-x   0 echarles   (501) staff       (20)      223 2021-05-08 14:21:52.000000 clouder-0.0.3/README.md
-drwxr-xr-x   0 echarles   (501) staff       (20)        0 2021-05-08 14:23:16.327279 clouder-0.0.3/clouder/
--rw-r--r--   0 echarles   (501) staff       (20)       16 2021-05-08 14:20:52.000000 clouder-0.0.3/clouder/__init__.py
-drwxr-xr-x   0 echarles   (501) staff       (20)        0 2021-05-08 14:23:16.329136 clouder-0.0.3/clouder.egg-info/
--rw-r--r--   0 echarles   (501) staff       (20)      420 2021-05-08 14:23:16.000000 clouder-0.0.3/clouder.egg-info/PKG-INFO
--rw-r--r--   0 echarles   (501) staff       (20)      226 2021-05-08 14:23:16.000000 clouder-0.0.3/clouder.egg-info/SOURCES.txt
--rw-r--r--   0 echarles   (501) staff       (20)        1 2021-05-08 14:23:16.000000 clouder-0.0.3/clouder.egg-info/dependency_links.txt
--rw-r--r--   0 echarles   (501) staff       (20)       51 2021-05-08 14:23:16.000000 clouder-0.0.3/clouder.egg-info/entry_points.txt
--rw-r--r--   0 echarles   (501) staff       (20)      102 2021-05-08 14:23:16.000000 clouder-0.0.3/clouder.egg-info/requires.txt
--rw-r--r--   0 echarles   (501) staff       (20)        8 2021-05-08 14:23:16.000000 clouder-0.0.3/clouder.egg-info/top_level.txt
--rw-r--r--   0 echarles   (501) staff       (20)       38 2021-05-08 14:23:16.329901 clouder-0.0.3/setup.cfg
--rwxr-xr-x   0 echarles   (501) staff       (20)      767 2021-05-08 14:22:14.000000 clouder-0.0.3/setup.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 clouder-0.0.4/.dockerignore
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 clouder-0.0.4/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 clouder-0.0.4/.eslintrc.js
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 clouder-0.0.4/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 clouder-0.0.4/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 clouder-0.0.4/.stylelintrc
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 clouder-0.0.4/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 clouder-0.0.4/CHANGELOG.md
+-rwxr-xr-x   0        0        0      388 2020-02-02 00:00:00.000000 clouder-0.0.4/Dockerfile
+-rwxr-xr-x   0        0        0     1743 2020-02-02 00:00:00.000000 clouder-0.0.4/Makefile
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 clouder-0.0.4/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 clouder-0.0.4/babel.config.js
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 clouder-0.0.4/conftest.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 clouder-0.0.4/environment.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 clouder-0.0.4/install.json
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 clouder-0.0.4/jest-playwright.config.js
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 clouder-0.0.4/jest.config.js
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 clouder-0.0.4/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 clouder-0.0.4/setup.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 clouder-0.0.4/tsconfig.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 clouder-0.0.4/webpack.config.js
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 clouder-0.0.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 clouder-0.0.4/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 clouder-0.0.4/.github/workflows/update-integration-tests.yml
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 clouder-0.0.4/.yarn/cache/.gitignore
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/README.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/tf_k8s_1/README.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/tf_k8s_1/outputs.tf
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/tf_k8s_1/provider.tf
+-rw-r--r--   0        0        0    11253 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/tf_k8s_1/resources.tf
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/tf_k8s_2/README.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/tf_k8s_2/outputs.tf
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/tf_k8s_2/provider.tf
+-rw-r--r--   0        0        0    11269 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/tf_k8s_2/resources.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/tf_k8s_3/README.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/tf_k8s_3/outputs.tf
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/tf_k8s_3/provider.tf
+-rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/k8s/tf_k8s_3/resources.tf
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/Makefile
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/README.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/outputs.tf
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/provider.tf
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/resources.tf
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/variables.tf
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/_resources/cloud.conf
+-rwxr-xr-x   0        0        0     5552 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/_resources/gpu-centos-base.sh
+-rwxr-xr-x   0        0        0     1807 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/_resources/gpu-centos-docker.sh
+-rwxr-xr-x   0        0        0     5187 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/_resources/gpu-centos-kubernetes.sh
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/_resources/gpu-ubuntu-base.sh
+-rwxr-xr-x   0        0        0    11938 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/_resources/kubeadm-common_centos_7.sh
+-rwxr-xr-x   0        0        0     2643 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/_resources/kubeadm-common_ubuntu_20.04.sh
+-rwxr-xr-x   0        0        0     5849 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/_resources/kubeadm-master.sh
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/_resources/kubeadm-master.yaml
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/_resources/kubeadm-worker.sh
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/_resources/kubeadm-worker.yaml
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 clouder-0.0.4/_templates/kubeadm/_resources/openstack-api-ca.pem
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/__main__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/_version.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/application.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/handlers.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/serverapplication.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/shell.py
+-rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/package.json
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/schemas/@datalayer/clouder/package.json.orig
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/schemas/@datalayer/clouder/plugin.json
+-rw-r--r--   0        0        0   218571 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/static/123.06972f7884f1ede837c2.js
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/static/123.06972f7884f1ede837c2.js.LICENSE.txt
+-rw-r--r--   0        0        0    35296 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/static/430.2af15ae087ac6ca2d912.js
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/static/570.f089e49c340468520511.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/static/570.f089e49c340468520511.js.LICENSE.txt
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/static/643.7040e4348cafa45c143c.js
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/static/887.b67da9b0eb64d459103e.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/static/887.b67da9b0eb64d459103e.js.LICENSE.txt
+-rw-r--r--   0        0        0     8032 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/static/955.d7bffe85834763adb37c.js
+-rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/static/remoteEntry.384be67575a032bdaaff.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/static/style.js
+-rw-r--r--   0        0        0    58608 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/ovh/create_database_mysql.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/ovh/create_kubernetes.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/ovh/get_apps.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/ovh/get_authorized_apps.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/ovh/get_bills.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/ovh/get_consumer_key.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/ovh/get_databases_mysql.py
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/ovh/get_services.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/ovh/get_services_expiring.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/ovh/me.py
+-rw-r--r--   0        0        0  1899852 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/ovh/specs/cloud.json
+-rwxr-xr-x   0        0        0     3668 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/sbin/cli.sh
+-rwxr-xr-x   0        0        0      391 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/sbin/clouder.sh
+-rwxr-xr-x   0        0        0      386 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/sbin/header.sh
+-rwxr-xr-x   0        0        0     3824 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/sbin/kind-create-cluster.sh
+-rwxr-xr-x   0        0        0     1286 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/sbin/kind-install.sh
+-rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/sbin/os.sh
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/sbin/ping.sh
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/static/README.md
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/templates/index.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/tests/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 clouder-0.0.4/clouder/tests/test_handlers.py
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/README.md
+-rwxr-xr-x   0        0        0      299 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/config/README.md
+-rwxr-xr-x   0        0        0     2362 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/config/jupyter_server_config.py
+-rwxr-xr-x   0        0        0      301 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/notebooks/README.md
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/notebooks/ping.ipynb
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/notebooks/test.ipynb
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/notebooks/tmp.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/notebooks/untitled.txt
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/notebooks/subfolder-1/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/notebooks/subfolder-1/test-1.ipynb
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/notebooks/subfolder-1/subfolder-1-1/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/notebooks/subfolder-1/subfolder-1-1/test-1-1.ipynb
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/notebooks/subfolder-2/README.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/notebooks/subfolder-2/test-2.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/notebooks/subfolder-2/untitled.txt
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/sh/README.md
+-rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/sh/kill.sh
+-rwxr-xr-x   0        0        0      746 2020-02-02 00:00:00.000000 clouder-0.0.4/dev/sh/start-jupyter-server.sh
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/LICENSE
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/Makefile
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/README.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/babel.config.js
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/docusaurus.config.js
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/environment.yml
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/package.json
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/sidebars.js
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/docs/index.mdx
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/docs/setup/_category_.yml
+-rw-r--r--   0        0        0    80754 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/docs/setup/aws.md
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/docs/setup/azure.md
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/docs/setup/docker.md
+-rw-r--r--   0        0        0    22747 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/docs/setup/gcloud.md
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/docs/setup/index.mdx
+-rw-r--r--   0        0        0    21206 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/docs/setup/minikube.md
+-rw-r--r--   0        0        0    10733 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/docs/setup/ovhcloud.md
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/src/components/HomepageFeatures.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/src/components/HomepageFeatures.module.css
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/src/components/HomepageProducts.js
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/src/components/HomepageProducts.module.css
+-rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/src/css/custom.css
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/src/pages/index.js
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/src/pages/markdown-page.md
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/src/pages/testimonials.tsx
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/static/img/feature_1.svg
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/static/img/feature_2.svg
+-rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/static/img/feature_3.svg
+-rw-r--r--   0        0        0    15652 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/static/img/product_1.svg
+-rw-r--r--   0        0        0    38790 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/static/img/product_2.svg
+-rw-r--r--   0        0        0   103421 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/static/img/product_3.svg
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/static/img/datalayer/logo.png
+-rwxr-xr-x   0        0        0     4924 2020-02-02 00:00:00.000000 clouder-0.0.4/docs/static/img/datalayer/logo.svg
+-rw-r--r--   0        0        0    27996 2020-02-02 00:00:00.000000 clouder-0.0.4/examples/index.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 clouder-0.0.4/examples/manifests/deployment-nginx.yml
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 clouder-0.0.4/examples/manifests/jupyterhub-nginx-proxy.yaml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 clouder-0.0.4/examples/manifests/jupyterhub-psql.yaml
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 clouder-0.0.4/examples/manifests/jupyterhub-simple.yaml
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 clouder-0.0.4/examples/manifests/pvc-cinder.yml
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 clouder-0.0.4/examples/manifests/pvc.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 clouder-0.0.4/examples/manifests/svc-lb.yml
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 clouder-0.0.4/examples/manifests/svc-nginx.yml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 clouder-0.0.4/jupyter-config/nb-config/clouder.json
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 clouder-0.0.4/jupyter-config/server-config/clouder.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 clouder-0.0.4/node_modules/@eslint/eslintrc/node_modules/ajv/scripts/.eslintrc.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 clouder-0.0.4/node_modules/eslint/node_modules/ajv/scripts/.eslintrc.yml
+-rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 clouder-0.0.4/public/index.html
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 clouder-0.0.4/schema/plugin.json
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 clouder-0.0.4/src/App.tsx
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 clouder-0.0.4/src/emptyshim.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 clouder-0.0.4/src/handler.ts
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 clouder-0.0.4/src/index.ts
+-rwxr-xr-x   0        0        0      334 2020-02-02 00:00:00.000000 clouder-0.0.4/src/typings.d.ts
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 clouder-0.0.4/src/widget.tsx
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 clouder-0.0.4/src/__tests__/browser.spec.ts
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 clouder-0.0.4/src/__tests__/datalayer.spec.ts
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 clouder-0.0.4/src/components/Clouder.tsx
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 clouder-0.0.4/src/components/ClouderTab.tsx
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 clouder-0.0.4/src/components/KeysTab.tsx
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 clouder-0.0.4/src/components/VirtualMachineTab.tsx
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 clouder-0.0.4/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 clouder-0.0.4/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 clouder-0.0.4/style/index.js
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 clouder-0.0.4/style/svg/icon.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 clouder-0.0.4/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 clouder-0.0.4/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 clouder-0.0.4/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 clouder-0.0.4/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 clouder-0.0.4/ui-tests/tests/datalayer.spec.ts
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 clouder-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 clouder-0.0.4/LICENSE
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 clouder-0.0.4/README.md
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 clouder-0.0.4/hatch_build.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 clouder-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 clouder-0.0.4/PKG-INFO
```

