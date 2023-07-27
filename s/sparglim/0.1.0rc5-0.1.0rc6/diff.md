# Comparing `tmp/sparglim-0.1.0rc5.tar.gz` & `tmp/sparglim-0.1.0rc6.tar.gz`

## Comparing `sparglim-0.1.0rc5.tar` & `sparglim-0.1.0rc6.tar`

### file list

```diff
@@ -1,60 +1,70 @@
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/.editorconfig
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/RELEASE.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/.github/workflows/lint.yml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/dev/pyspark-app/Dockerfile.jupyterlab-sparglim
--rwxr-xr-x   0        0        0      127 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/dev/pyspark-app/reload.sh
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/dev/pyspark-app/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/dev/pyspark-app/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/dev/pyspark-app/k8s/lab-service.yaml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/dev/sparglim-server/Dockerfile.sparglim-server
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/dev/sparglim-server/reload.sh
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/dev/sparglim-server/k8s/connect-server-service.yaml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/dev/sparglim-server/k8s/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/dev/sparglim-server/k8s/headless-service.yaml
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/docker/Dockerfile.jupyterlab-sparglim
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/docker/Dockerfile.sparglim-server
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/docs/Makefile
--rwxr-xr-x   0        0        0     4786 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/docs/conf.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/docs/index.rst
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/docs/make.bat
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/docs/usage.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/example/pyspark-app/README.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/example/pyspark-app/k8s/deployment.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/example/pyspark-app/k8s/headless-service.yaml
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/example/pyspark-app/k8s/lab-service.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/example/sparglim-server/README.md
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/example/sparglim-server/k8s/connect-server-service.yaml
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/example/sparglim-server/k8s/deployment.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/example/sparglim-server/k8s/headless-service.yaml
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/exceptions.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/py.typed
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/utils.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/config/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/config/builder.py
--rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/config/configer.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/config/k8s.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/server/__init__.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/server/cli.py
--rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/server/daemon.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/server/tailer.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/sql/__init__.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/sparglim/sql/magic.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/tests/conftest.py
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/tests/test_builder.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/tests/test_daemon.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/tests/test_magic.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/tests/example/people.json
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/tests/mock/sbin/entrypoint.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/tests/mock/sbin/mock_spark_server.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/tests/mock/sbin/start-connect-server.sh
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/LICENSE
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/README.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/pyproject.toml
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 sparglim-0.1.0rc5/PKG-INFO
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.dockerignore
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.editorconfig
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/RELEASE.md
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/config.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/docker/Dockerfile.jupyterlab-sparglim
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/docker/Dockerfile.sparglim-server
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-on-k8s/README.md
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
+-rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/scripts/reload.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/sparglim-server/README.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/sparglim-server/k8s/connect-server-service.yaml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/sparglim-server/k8s/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/dev/sparglim-server/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/docker/Dockerfile.jupyterlab-sparglim
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/docker/Dockerfile.sparglim-server
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-on-k8s/README.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-on-k8s/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-on-k8s/k8s/lab-service.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/README.md
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/deployment.yaml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/jupyter-sparglim/lab-service.yaml
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/sparglim-server/connect-server-service.yaml
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/sparglim-server/headless-service.yaml
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/sparglim-server/README.md
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/sparglim-server/k8s/connect-server-service.yaml
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/sparglim-server/k8s/deployment.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/examples/sparglim-server/k8s/headless-service.yaml
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/exceptions.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/py.typed
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/utils.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/config/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/config/builder.py
+-rw-r--r--   0        0        0    11568 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/config/configer.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/config/k8s.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/server/__init__.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/server/cli.py
+-rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/server/daemon.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/server/tailer.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/sql/__init__.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/sparglim/sql/magic.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/conftest.py
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/test_builder.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/test_daemon.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/test_magic.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/example/people.json
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/mock/sbin/entrypoint.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/mock/sbin/mock_spark_server.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/tests/mock/sbin/start-connect-server.sh
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/LICENSE
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/README.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/pyproject.toml
+-rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 sparglim-0.1.0rc6/PKG-INFO
```

### Comparing `sparglim-0.1.0rc5/.pre-commit-config.yaml` & `sparglim-0.1.0rc6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/RELEASE.md` & `sparglim-0.1.0rc6/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/.github/workflows/python-package.yml` & `sparglim-0.1.0rc6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/.github/workflows/python-publish.yml` & `sparglim-0.1.0rc6/.github/workflows/publish.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Upload Python Package
+name: Upload Python Package and Docker Image
 
 on:
   release:
     types: [published]
 
 permissions:
   contents: read
@@ -40,24 +40,46 @@
     -
       name: Login to DockerHub
       uses: docker/login-action@v2
       with:
         username: ${{ secrets.DOCKERHUB_USERNAME }}
         password: ${{ secrets.DOCKERHUB_TOKEN }}
     -
-      name: Build and push
+      name: Build and push jupyterlab-sparglim
       id: docker_build_jupyterlab_sparglim
       uses: docker/build-push-action@v4
       with:
         context: .
         file: ./docker/Dockerfile.jupyterlab-sparglim
         push: true
         tags: ${{ secrets.DOCKERHUB_USERNAME }}/jupyterlab-sparglim:${{  github.ref_name }}
     -
-      name: Build and push
+      name: Build and push sparglim-server
       id: docker_build_sparglim_server
       uses: docker/build-push-action@v4
       with:
         context: .
         file: ./docker/Dockerfile.sparglim-server
         push: true
         tags: ${{ secrets.DOCKERHUB_USERNAME }}/sparglim-server:${{  github.ref_name }}
+
+    # Build latest if release
+    -
+      name: Build and push jupyterlab-sparglim_latest
+      id: docker_build_jupyterlab_sparglim_latest
+      if: '!github.event.prerelease'
+      uses: docker/build-push-action@v4
+      with:
+        context: .
+        file: ./docker/Dockerfile.jupyterlab-sparglim
+        push: true
+        tags: ${{ secrets.DOCKERHUB_USERNAME }}/jupyterlab-sparglim:latest
+    -
+      name: Build and push sparglim-server_latest
+      if: '!github.event.prerelease'
+      id: docker_build_sparglim_server_latest
+      uses: docker/build-push-action@v4
+      with:
+        context: .
+        file: ./docker/Dockerfile.sparglim-server
+        push: true
+        tags: ${{ secrets.DOCKERHUB_USERNAME }}/sparglim-server:latest
```

### Comparing `sparglim-0.1.0rc5/dev/pyspark-app/Dockerfile.jupyterlab-sparglim` & `sparglim-0.1.0rc6/dev/docker/Dockerfile.jupyterlab-sparglim`

 * *Files 24% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 
 COPY --chown=application:application ./ ./sparglim
 RUN pip install --no-cache-dir ./sparglim[all]
 
 ENTRYPOINT ["tini","--","jupyter-lab", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--IdentityProvider.token=''"]
 EXPOSE 8888
 
-# docker build -t wh1isper/jupyterlab-sparglim:dev -f dev/pyspark-app/Dockerfile.jupyterlab-sparglim . && ./dev/pyspark-app/reload.sh
+# docker build -t wh1isper/jupyterlab-sparglim:dev -f dev/docker/Dockerfile.jupyterlab-sparglim . && ./scripts/reload.sh
```

### Comparing `sparglim-0.1.0rc5/dev/pyspark-app/k8s/deployment.yaml` & `sparglim-0.1.0rc6/dev/jupyter-sparglim-on-k8s/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/dev/sparglim-server/k8s/deployment.yaml` & `sparglim-0.1.0rc6/dev/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/example/pyspark-app/k8s/deployment.yaml` & `sparglim-0.1.0rc6/examples/jupyter-sparglim-on-k8s/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/example/sparglim-server/k8s/deployment.yaml` & `sparglim-0.1.0rc6/examples/jupyter-sparglim-sc/k8s/sparglim-server/deployment.yaml`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/sparglim/utils.py` & `sparglim-0.1.0rc6/sparglim/utils.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/sparglim/config/builder.py` & `sparglim-0.1.0rc6/sparglim/config/builder.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/sparglim/config/configer.py` & `sparglim-0.1.0rc6/sparglim/config/configer.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/sparglim/config/k8s.py` & `sparglim-0.1.0rc6/sparglim/config/k8s.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/sparglim/server/cli.py` & `sparglim-0.1.0rc6/sparglim/server/cli.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/sparglim/server/daemon.py` & `sparglim-0.1.0rc6/sparglim/server/daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,35 +51,48 @@
         if not self.start_cmd_path.exists():
             raise UnconfigurableError(
                 f"{self.start_cmd_path.name} not found in $SPARK_HOME/sbin, check your SPARK_HOME"
             )
 
         SPARK_VERSION = os.getenv("SPARK_VERSION", get_spark_version())
         SCALA_VERSION = os.getenv("SCALA_VERSION", get_scala_version())
+        add_connect_package = os.getenv("SPARGLIM_SERVER_CONNECT_PACKAGES", "false") in [
+            "true",
+            "True",
+        ]
         self.daemon_package = []
-        if SPARK_VERSION and SCALA_VERSION:
+        if add_connect_package and (SPARK_VERSION and SCALA_VERSION):
             # Specify the spark-connect package or use the default one
             self.daemon_package.append(
                 f"org.apache.spark:spark-connect_{SCALA_VERSION}:{SPARK_VERSION}"
             )
         self.builder = SparkEnvConfiger().config_connect_server(
             self.mode, k8s_config_path=k8s_config_path
         )
 
         self._tailer: Optional[Tailer] = None
         self._daemon: Optional[threading.Thread] = None
         self.is_stopping: bool = False
 
     @property
     def config(self) -> List[str]:
-        return [f"--conf {k}={v}" for k, v in self.builder.get_all().items()]
+        config = []
+        for k, v in self.builder.get_all().items():
+            config.append("--conf")
+            config.append(f"{k}={v}")
+        return config
 
     @property
     def packages(self) -> List[str]:
-        return [f"--packages {p}" for p in self.daemon_package]
+        packages = []
+        for p in self.daemon_package:
+            packages.append("--packages")
+            packages.append(p)
+
+        return packages
 
     @property
     def pid_file(self) -> Optional[Path]:
         for pid_file in self.pid_dir.glob(self.pid_glob_format):
             return pid_file
         return None
 
@@ -136,15 +149,16 @@
         )
         p.wait()
 
         assert self.pid
         assert self.log_file
 
         logger.info(
-            f"Connect server started, pid: {self.pid}, logs {self.log_file.absolute().as_posix()}"  # type: ignore
+            # type: ignore
+            f"Connect server started, pid: {self.pid}, logs {self.log_file.absolute().as_posix()}"
         )
 
     def _wait_exit(self):
         signal.signal(signal.SIGINT, self.stop)
         signal.signal(signal.SIGTERM, self.stop)
         signal.pause()
         self.daemon_pid_file.unlink()
```

### Comparing `sparglim-0.1.0rc5/sparglim/server/tailer.py` & `sparglim-0.1.0rc6/sparglim/server/tailer.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/sparglim/sql/magic.py` & `sparglim-0.1.0rc6/sparglim/sql/magic.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,24 @@
 
         Init a table
 
         ```python
         from datetime import datetime, date
         from pyspark.sql import Row
 
+        from sparglim.config.builder import ConfigBuilder
+        spark = ConfigBuilder().get_or_create()
+
+
         df = spark.createDataFrame([
             Row(a=1, b=2., c='string1', d=date(2000, 1, 1), e=datetime(2000, 1, 1, 12, 0)),
             Row(a=2, b=3., c='string2', d=date(2000, 2, 1), e=datetime(2000, 1, 2, 12, 0)),
             Row(a=4, b=5., c='string3', d=date(2000, 3, 1), e=datetime(2000, 1, 3, 12, 0))
         ])
+        df.show()
         df.createOrReplaceTempView("tb")
         ```
 
         Query it
 
         ```ipython
         %sql SELECT * FROM tb
@@ -102,15 +107,16 @@
             return
         logger.debug(f"Execute Spark SQL: {sql}")
         return self.spark.sql(sql)
 
     def _execute(self, sql=str):
         r = None
         for s in sql.split(";"):
-            r = self._execute_one(s.strip())
+            if s.strip():  # ignore empty sql
+                r = self._execute_one(s.strip())
         return r
 
     @line_magic
     @cell_magic
     def sql(self, line: Optional[str] = None, cell: Optional[str] = None):
         return self._execute(self.format_sql([line, cell]))
```

### Comparing `sparglim-0.1.0rc5/tests/conftest.py` & `sparglim-0.1.0rc6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/tests/test_builder.py` & `sparglim-0.1.0rc6/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/tests/test_daemon.py` & `sparglim-0.1.0rc6/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/tests/test_magic.py` & `sparglim-0.1.0rc6/tests/test_magic.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/tests/mock/sbin/entrypoint.py` & `sparglim-0.1.0rc6/tests/mock/sbin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/tests/mock/sbin/mock_spark_server.py` & `sparglim-0.1.0rc6/tests/mock/sbin/mock_spark_server.py`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/.gitignore` & `sparglim-0.1.0rc6/.gitignore`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/LICENSE` & `sparglim-0.1.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `sparglim-0.1.0rc5/pyproject.toml` & `sparglim-0.1.0rc6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,30 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "sparglim"
 description = "sparglim"
 keywords = ["sparglim"]
 requires-python = ">=3.8"
-dependencies = ["loguru", "click", "findspark", "psutil"]
+dependencies = ["loguru", "click", "findspark", "psutil", "kubernetes"]
 dynamic = ["version"]
 classifiers = [
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 [project.optional-dependencies]
 pyspark = ["pyspark[pandas_on_spark,sql,connect]"]
 magic = ["sparglim[pyspark]", "ipython"]
-k8s = ["sparglim[pyspark]", "kubernetes"]
 
-all = ["sparglim[pyspark]", "sparglim[magic]", "sparglim[k8s]"]
+all = ["sparglim[pyspark]", "sparglim[magic]"]
 test = ["sparglim[all]", "pytest", "pytest-cov", "pytype", "pytest-timeout"]
-# TODO: Docs and its dependencies
+
 dev = ["sparglim[test]"]
 
 [project.scripts]
 sparglim-server = "sparglim.server.cli:cli"
 
 [[project.authors]]
 name = "wh1isper"
```

