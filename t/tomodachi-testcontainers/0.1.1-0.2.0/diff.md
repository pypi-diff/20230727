# Comparing `tmp/tomodachi_testcontainers-0.1.1.tar.gz` & `tmp/tomodachi_testcontainers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomodachi_testcontainers-0.1.1.tar", max compression
+gzip compressed data, was "tomodachi_testcontainers-0.2.0.tar", max compression
```

## Comparing `tomodachi_testcontainers-0.1.1.tar` & `tomodachi_testcontainers-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.1.1/LICENSE
--rw-r--r--   0        0        0    24828 2023-07-23 10:30:40.079394 tomodachi_testcontainers-0.1.1/README.md
--rw-r--r--   0        0        0     3490 2023-07-24 15:08:57.356890 tomodachi_testcontainers-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/clients/__init__.py
--rw-r--r--   0        0        0     2300 2023-07-23 10:30:40.087069 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/clients/snssqs_client.py
--rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/__init__.py
--rw-r--r--   0        0        0     1602 2023-07-23 10:30:40.087572 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/common.py
--rw-r--r--   0        0        0     1854 2023-07-23 10:30:40.087734 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/localstack.py
--rw-r--r--   0        0        0     2121 2023-07-23 10:30:40.087931 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/moto.py
--rw-r--r--   0        0        0     3150 2023-07-23 10:30:40.088136 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/sftp.py
--rw-r--r--   0        0        0      965 2023-07-23 10:30:40.088352 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/tomodachi.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/py.typed
--rw-r--r--   0        0        0     1346 2023-07-23 10:30:40.088641 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/__init__.py
--rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/assertions.py
--rw-r--r--   0        0        0     2290 2023-07-23 10:30:40.088974 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
--rw-r--r--   0        0        0     2109 2023-07-23 10:30:40.089100 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/moto_fixtures.py
--rw-r--r--   0        0        0     1594 2023-07-23 10:30:40.089262 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
--rw-r--r--   0        0        0      605 2023-07-23 10:30:40.089418 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
--rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/utils.py
--rw-r--r--   0        0        0    26017 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.2.0/LICENSE
+-rw-r--r--   0        0        0    26475 2023-07-27 14:17:21.581583 tomodachi_testcontainers-0.2.0/README.md
+-rw-r--r--   0        0        0     3649 2023-07-27 14:17:30.478183 tomodachi_testcontainers-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/clients/__init__.py
+-rw-r--r--   0        0        0     2300 2023-07-23 10:30:40.087069 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/clients/snssqs_client.py
+-rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/__init__.py
+-rw-r--r--   0        0        0     2185 2023-07-27 14:17:21.582366 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/common.py
+-rw-r--r--   0        0        0     1818 2023-07-27 14:17:21.582876 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/localstack.py
+-rw-r--r--   0        0        0     2085 2023-07-27 14:17:21.583252 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/moto.py
+-rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/sftp.py
+-rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/tomodachi.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/py.typed
+-rw-r--r--   0        0        0     1346 2023-07-23 10:30:40.088641 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/__init__.py
+-rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/assertions.py
+-rw-r--r--   0        0        0     2290 2023-07-27 13:30:06.032389 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
+-rw-r--r--   0        0        0     2109 2023-07-27 13:30:09.023818 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/moto_fixtures.py
+-rw-r--r--   0        0        0     1594 2023-07-27 13:30:16.939169 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
+-rw-r--r--   0        0        0      605 2023-07-23 10:30:40.089418 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
+-rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/utils.py
+-rw-r--r--   0        0        0    27664 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.2.0/PKG-INFO
```

### Comparing `tomodachi_testcontainers-0.1.1/LICENSE` & `tomodachi_testcontainers-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.1/README.md` & `tomodachi_testcontainers-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: tomodachi-testcontainers
+Version: 0.2.0
+Summary: Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing.
+Home-page: https://github.com/filipsnastins/tomodachi-testcontainers
+License: MIT
+Author: Filips Nastins
+Author-email: nastinsfilips@gmail.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: sftp
+Requires-Dist: aiobotocore (>=2.5.2,<3.0.0)
+Requires-Dist: asyncssh (>=2.13.2,<3.0.0) ; extra == "sftp"
+Requires-Dist: pytest (>=7.1.2,<8.0.0)
+Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0)
+Requires-Dist: testcontainers (>=3.7.1,<4.0.0)
+Requires-Dist: types-aiobotocore[dynamodb,s3,sns,sqs,ssm] (>=2.5.2,<3.0.0)
+Project-URL: Repository, https://github.com/filipsnastins/tomodachi-testcontainers
+Description-Content-Type: text/markdown
+
 # tomodachi-testcontainers
 
 The library provides [Testcontainers](src/tomodachi_testcontainers/containers/),
 [Pytest fixtures](src/tomodachi_testcontainers/pytest/),
 and [test clients](src/tomodachi_testcontainers/clients/) for working with Testcontainers,
 and testing applications built with [Python Tomodachi framework](https://github.com/kalaspuff/tomodachi).
 
@@ -15,42 +39,44 @@
 [Testcontainers](https://testcontainers.com/) is an open-source framework for providing throwaway,
 lightweight instances of databases, message brokers, web browsers,
 or just about anything that can run in a Docker container.
 It facilitates the use of Docker containers for functional, integration, and end-to-end testing.
 
 - [tomodachi-testcontainers](#tomodachi-testcontainers)
   - [Installation](#installation)
-  - [Quickstart and Examples](#quickstart-and-examples)
+  - [Quickstart and examples](#quickstart-and-examples)
   - [Getting started](#getting-started)
     - [Testing standalone Tomodachi service](#testing-standalone-tomodachi-service)
     - [Changing Dockerfile location](#changing-dockerfile-location)
     - [Running Tomodachi container from pre-built image](#running-tomodachi-container-from-pre-built-image)
     - [Testing Tomodachi service with external dependencies](#testing-tomodachi-service-with-external-dependencies)
   - [Benefits and dangers of end-to-end tests](#benefits-and-dangers-of-end-to-end-tests)
     - [Building confidence of releasability](#building-confidence-of-releasability)
-    - [⚠️ Mind the Test Pyramid - not overdue end-to-end tests](#️-mind-the-test-pyramid---not-overdue-end-to-end-tests)
+    - [⚠️ Mind the Test Pyramid - don't overdo end-to-end tests](#️-mind-the-test-pyramid---dont-overdo-end-to-end-tests)
   - [Running Testcontainers in CI pipeline](#running-testcontainers-in-ci-pipeline)
   - [Supported Testcontainers](#supported-testcontainers)
     - [Tomodachi](#tomodachi)
     - [Moto](#moto)
     - [LocalStack](#localstack)
     - [SFTP](#sftp)
+  - [Configuration with environment variables](#configuration-with-environment-variables)
+  - [Changing default Docker network](#changing-default-docker-network)
   - [Resources and acknowledgements](#resources-and-acknowledgements)
   - [Development](#development)
 
 ## Installation
 
 ```bash
 pip install tomodachi-testcontainers
 
 # Extra dependency - SFTP container and asyncssh
 pip install tomodachi-testcontainers[sftp]
 ```
 
-## Quickstart and Examples
+## Quickstart and examples
 
 Tomodachi service examples are in [examples/](examples/) folder. Their end-to-end tests are in [tests/test_services](tests/test_services).
 
 For full list of available testcontainers, check out [Supported Testcontainers](#supported-testcontainers) section,
 [tomodachi_testcontainers.containers](src/tomodachi_testcontainers/containers/) module,
 and the official [testcontainers-python](https://github.com/testcontainers/testcontainers-python) library -
 it makes it easy to create your own Testcontainers.
@@ -151,18 +177,14 @@
 with the `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` environment variable.
 
 Examples:
 
 - `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/` - specify just a directory, Dockerfile is inferred automatically
 - `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/Dockerfile.testing` - explicitly specify the Dockerfile name
 
-⚠️ Make sure that the environment variable is set before running `pytest` -
-e.g. with [pytest-env](https://pypi.org/project/pytest-env/) plugin or
-by setting it in the shell before running `pytest`.
-
 ### Running Tomodachi container from pre-built image
 
 If the Tomodachi service Docker image is already built, you can run the container
 by specifying the image ID in the `TOMODACHI_TESTCONTAINER_IMAGE_ID` environment variable.
 
 It is useful when running tests in the CI pipeline when the image has been already built
 on the build step.
@@ -359,15 +381,15 @@
 that the system will work in production without more manual testing._
 
 _To get a high confidence of releasability, it's necessary to test the system with real dependencies and infrastructure.
 Testcontainers make it easy to spin up real dependencies in Docker containers, and throw them away
 when the tests are finished. They work in thw same way locally and in the CI pipeline, so you need to
 setup test suite only once._
 
-### ⚠️ Mind the Test Pyramid - not overdue end-to-end tests
+### ⚠️ Mind the Test Pyramid - don't overdo end-to-end tests
 
 Despite many benefits of end-to-end tests, they are the most expensive kind 💸 -
 they're slow, sometimes [flaky](https://martinfowler.com/articles/nonDeterminism.html),
 it's hard to understand what's broken when they fail.
 
 End-to-end tests are expensive, but necessary to build confidence of releasability,
 so it's important to use them intentionally and know about other kinds of tests.
@@ -474,14 +496,37 @@
 
 Repository: <https://github.com/atmoz/sftp>
 DockerHub: <https://hub.docker.com/r/atmoz/sftp>
 
 - Available as an extra dependency `sftp` - install with
   `pip install tomodachi-testcontainers[sftp]` or `poetry install -E sftp`
 
+## Configuration with environment variables
+
+⚠️ Make sure that environment variables are set before running `pytest` -
+e.g. with [pytest-env](https://pypi.org/project/pytest-env/) plugin or
+by setting it in the shell before running `pytest`.
+
+| Environment Variable                      | Description                                                                                                                   |
+| :---------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
+| `TESTCONTAINER_DOCKER_NETWORK`            | Launch testcontainers in specified Docker network. Defaults to 'bridge'. Network must be created beforehand                   |
+| `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` | Override path to Dockerfile for building Tomodachi service image. Defaults to '.'                                             |
+| `<CONTAINER-NAME>_TESTCONTAINER_IMAGE_ID` | Override any supported Testcontainer Image ID. Defaults to `None`, `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` takes precedence |
+
+## Changing default Docker network
+
+By default, testcontainers are started in the default `bridge` Docker network.
+Sometimes it's useful to start containers in a different network, e.g. a network
+specifically dedicated for running automated tests.
+
+Specify a new network name with the `TOMODACHI_TESTCONTAINER_NETWORK` environment variable.
+The Docker network is not created automatically, so make sure that it exists before running tests.
+
+⚠️ Make sure that the environment variable is set before running `pytest`.
+
 ## Resources and acknowledgements
 
 - [testcontainers.com](https://testcontainers.com/) - home of Testcontainers.
 
 - [testcontainers-python](https://testcontainers-python.readthedocs.io/) - Python SDK for Testcontainers.
 
 - Talk ["Integration tests are needed and simple"](https://softwaregarden.dev/en/talks/integration-tests-are-needed-and-simple/)
@@ -513,14 +558,16 @@
 poetry shell
 pre-commit install
 ```
 
 - Run tests
 
 ```bash
+docker network create tomodachi-testcontainers
+
 pytest
 poetry run test-ci
 ```
 
 - Format and lint code
 
 ```bash
@@ -535,7 +582,8 @@
 ```
 
 - Build package release
 
 ```bash
 poetry build
 ```
+
```

### Comparing `tomodachi_testcontainers-0.1.1/pyproject.toml` & `tomodachi_testcontainers-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomodachi-testcontainers"
-version = "0.1.1"
+version = "0.2.0"
 description = "Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing."
 authors = ["Filips Nastins <nastinsfilips@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/filipsnastins/tomodachi-testcontainers"
 repository = "https://github.com/filipsnastins/tomodachi-testcontainers"
@@ -12,15 +12,21 @@
 [tool.poetry.dependencies]
 python = "^3.8.1"
 aiobotocore = "^2.5.2"
 asyncssh = { version = "^2.13.2", optional = true }
 pytest = "^7.1.2"
 pytest-asyncio = "^0.21.1"
 testcontainers = "^3.7.1"
-types-aiobotocore = { extras = ["dynamodb", "s3", "sns", "sqs", "ssm"], version = "^2.5.2" }
+types-aiobotocore = { extras = [
+    "dynamodb",
+    "s3",
+    "sns",
+    "sqs",
+    "ssm",
+], version = "^2.5.2" }
 
 [tool.poetry.group.dev.dependencies]
 autoflake = "^2.2.0"
 bandit = "^1.7.5"
 black = "^23.7.0"
 busypie = "^0.5.1"
 colorama = "^0.4.6"
@@ -74,35 +80,59 @@
 target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '\.git/|\.mypy_cache/|\.venv/|\.pytest_cache/|\.vscode/|__pycache__/|build/|dist/'
 
 [tool.isort]
 profile = "black"
 line_length = 120
-skip = [".git", ".ruff_cache", ".mypy_cache", ".venv", ".pytest_cache", ".vscode", "__pycache__", "build", "dist"]
+skip = [
+    ".git",
+    ".ruff_cache",
+    ".mypy_cache",
+    ".venv",
+    ".pytest_cache",
+    ".vscode",
+    "__pycache__",
+    "build",
+    "dist",
+]
 
 [tool.bandit]
-exclude_dirs = ["tests", ".git", ".ruff_cache", ".mypy_cache", ".venv", ".pytest_cache", ".vscode", "__pycache__", "build", "dist"]
+exclude_dirs = [
+    "tests",
+    ".git",
+    ".ruff_cache",
+    ".mypy_cache",
+    ".venv",
+    ".pytest_cache",
+    ".vscode",
+    "__pycache__",
+    "build",
+    "dist",
+]
 
 [tool.mypy]
 python_version = "3.8"
 ignore_missing_imports = true
 
 [tool.flake8]
-ignore = [
-    "ANN101",
-    "ANN401",
-    "BLK100",
-    "E501",
-    "LIT101",
-    "PL123",
-]
+ignore = ["ANN101", "ANN401", "BLK100", "E501", "LIT101", "PL123"]
 literal-inline-quotes = "double"
 literal-multiline-quotes = "double"
-exclude = [".git", ".ruff_cache", ".mypy_cache", ".venv", ".pytest_cache", ".vscode", "__pycache__", "build", "dist"]
+exclude = [
+    ".git",
+    ".ruff_cache",
+    ".mypy_cache",
+    ".venv",
+    ".pytest_cache",
+    ".vscode",
+    "__pycache__",
+    "build",
+    "dist",
+]
 
 [tool.ruff]
 target-version = "py38"
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
@@ -126,19 +156,14 @@
     "venv",
 ]
 line-length = 120
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 junit_family = "xunit2"
-testpaths = [
-    "tests"
-]
-norecursedirs = [
-    ".venv",
-    "__pycache__",
-    ".git"
-]
+testpaths = ["tests"]
+norecursedirs = [".venv", "__pycache__", ".git"]
 log_cli_level = "INFO"
 env = [
-    "TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/Dockerfile"
+    "TESTCONTAINER_DOCKER_NETWORK=tomodachi-testcontainers",
+    "TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/Dockerfile",
 ]
```

### Comparing `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/clients/snssqs_client.py` & `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/clients/snssqs_client.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/__init__.py` & `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/localstack.py` & `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/localstack.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from typing import Any, Optional
 
-from testcontainers.core.container import DockerContainer
 from testcontainers.core.waiting_utils import wait_for_logs
 
+from tomodachi_testcontainers.containers.common import DockerContainer
 from tomodachi_testcontainers.utils import AWSClientConfig
 
 
 class LocalStackContainer(DockerContainer):
     def __init__(
         self,
         image: str = "localstack/localstack:2.1",
@@ -23,16 +23,16 @@
         self.region_name = region_name or os.environ.get("AWS_DEFAULT_REGION") or "eu-west-1"
         self.aws_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID") or "testing"  # nosec: B105
         self.aws_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY") or "testing"  # nosec: B105
 
         self.with_bind_ports(self.internal_port, self.edge_port)
 
     def get_internal_url(self) -> str:
-        bridge_ip = self.get_docker_client().bridge_ip(self.get_wrapped_container().id)
-        return f"http://{bridge_ip}:{self.internal_port}"
+        ip = self.get_container_internal_ip()
+        return f"http://{ip}:{self.internal_port}"
 
     def get_external_url(self) -> str:
         host = self.get_container_host_ip()
         return f"http://{host}:{self.edge_port}"
 
     def get_aws_client_config(self) -> AWSClientConfig:
         return AWSClientConfig(
```

### Comparing `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/moto.py` & `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/moto.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from typing import Any, Optional
 
-from testcontainers.core.container import DockerContainer
 from testcontainers.core.waiting_utils import wait_for_logs
 
+from tomodachi_testcontainers.containers.common import DockerContainer
 from tomodachi_testcontainers.utils import AWSClientConfig
 
 
 class MotoContainer(DockerContainer):
     def __init__(
         self,
         image: str = "motoserver/moto:latest",
@@ -26,16 +26,16 @@
 
         self.with_bind_ports(self.internal_port, self.edge_port)
         self.with_env("AWS_DEFAULT_REGION", self.region_name)
         self.with_env("AWS_ACCESS_KEY_ID", self.aws_access_key_id)
         self.with_env("AWS_SECRET_ACCESS_KEY", self.aws_secret_access_key)
 
     def get_internal_url(self) -> str:
-        bridge_ip = self.get_docker_client().bridge_ip(self.get_wrapped_container().id)
-        return f"http://{bridge_ip}:{self.internal_port}"
+        ip = self.get_container_internal_ip()
+        return f"http://{ip}:{self.internal_port}"
 
     def get_external_url(self) -> str:
         host = self.get_container_host_ip()
         return f"http://{host}:{self.edge_port}"
 
     def get_aws_client_config(self) -> AWSClientConfig:
         return AWSClientConfig(
```

### Comparing `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/sftp.py` & `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/sftp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, NamedTuple
 
 import asyncssh
-from testcontainers.core.container import DockerContainer
 from testcontainers.core.waiting_utils import wait_for_logs
 
+from tomodachi_testcontainers.containers.common import DockerContainer
+
 ConnectionDetails = NamedTuple("ConnectionDetails", [("host", str), ("port", int)])
 
 
 class SFTPContainer(DockerContainer):
     def __init__(
         self,
         image: str = "atmoz/sftp:latest",
@@ -22,15 +23,15 @@
 
         self.with_command("userpass:pass:1001 userssh::1002")
 
         self.authorized_private_key = asyncssh.generate_private_key("ssh-ed25519")
         self.authorized_public_key = self.authorized_private_key.export_public_key().decode()
 
     def get_internal_conn_details(self) -> ConnectionDetails:
-        host = self.get_docker_client().bridge_ip(self.get_wrapped_container().id)
+        host = self.get_container_internal_ip()
         return ConnectionDetails(host=host, port=self.internal_port)
 
     def get_external_conn_details(self) -> ConnectionDetails:
         host = self.get_container_host_ip()
         return ConnectionDetails(host=host, port=self.edge_port)
 
     def get_host_public_key(self) -> str:
```

### Comparing `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/containers/tomodachi.py` & `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/containers/tomodachi.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Any
 
-from testcontainers.core.container import DockerContainer
 from testcontainers.core.waiting_utils import wait_for_logs
 
+from tomodachi_testcontainers.containers.common import DockerContainer
+
 
 class TomodachiContainer(DockerContainer):
     def __init__(self, image: str, internal_port: int = 9700, edge_port: int = 9700, **kwargs: Any) -> None:
         super().__init__(image, **kwargs)
         self.internal_port = internal_port
         self.edge_port = edge_port
         self.with_bind_ports(internal_port, edge_port)
 
     def get_internal_url(self) -> str:
-        bridge_ip = self.get_docker_client().bridge_ip(self.get_wrapped_container().id)
-        return f"http://{bridge_ip}:{self.internal_port}"
+        ip = self.get_container_internal_ip()
+        return f"http://{ip}:{self.internal_port}"
 
     def get_external_url(self) -> str:
         host = self.get_container_host_ip()
         return f"http://{host}:{self.edge_port}"
 
     def start(self, timeout: float = 10) -> "TomodachiContainer":
         super().start()
```

### Comparing `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/__init__.py` & `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/localstack_fixtures.py` & `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/localstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/moto_fixtures.py` & `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/moto_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/sftp_fixtures.py` & `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/sftp_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.1/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py` & `tomodachi_testcontainers-0.2.0/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.1.1/PKG-INFO` & `tomodachi_testcontainers-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: tomodachi-testcontainers
-Version: 0.1.1
-Summary: Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing.
-Home-page: https://github.com/filipsnastins/tomodachi-testcontainers
-License: MIT
-Author: Filips Nastins
-Author-email: nastinsfilips@gmail.com
-Requires-Python: >=3.8.1,<4.0.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: sftp
-Requires-Dist: aiobotocore (>=2.5.2,<3.0.0)
-Requires-Dist: asyncssh (>=2.13.2,<3.0.0) ; extra == "sftp"
-Requires-Dist: pytest (>=7.1.2,<8.0.0)
-Requires-Dist: pytest-asyncio (>=0.21.1,<0.22.0)
-Requires-Dist: testcontainers (>=3.7.1,<4.0.0)
-Requires-Dist: types-aiobotocore[dynamodb,s3,sns,sqs,ssm] (>=2.5.2,<3.0.0)
-Project-URL: Repository, https://github.com/filipsnastins/tomodachi-testcontainers
-Description-Content-Type: text/markdown
-
 # tomodachi-testcontainers
 
 The library provides [Testcontainers](src/tomodachi_testcontainers/containers/),
 [Pytest fixtures](src/tomodachi_testcontainers/pytest/),
 and [test clients](src/tomodachi_testcontainers/clients/) for working with Testcontainers,
 and testing applications built with [Python Tomodachi framework](https://github.com/kalaspuff/tomodachi).
 
@@ -39,42 +15,44 @@
 [Testcontainers](https://testcontainers.com/) is an open-source framework for providing throwaway,
 lightweight instances of databases, message brokers, web browsers,
 or just about anything that can run in a Docker container.
 It facilitates the use of Docker containers for functional, integration, and end-to-end testing.
 
 - [tomodachi-testcontainers](#tomodachi-testcontainers)
   - [Installation](#installation)
-  - [Quickstart and Examples](#quickstart-and-examples)
+  - [Quickstart and examples](#quickstart-and-examples)
   - [Getting started](#getting-started)
     - [Testing standalone Tomodachi service](#testing-standalone-tomodachi-service)
     - [Changing Dockerfile location](#changing-dockerfile-location)
     - [Running Tomodachi container from pre-built image](#running-tomodachi-container-from-pre-built-image)
     - [Testing Tomodachi service with external dependencies](#testing-tomodachi-service-with-external-dependencies)
   - [Benefits and dangers of end-to-end tests](#benefits-and-dangers-of-end-to-end-tests)
     - [Building confidence of releasability](#building-confidence-of-releasability)
-    - [⚠️ Mind the Test Pyramid - not overdue end-to-end tests](#️-mind-the-test-pyramid---not-overdue-end-to-end-tests)
+    - [⚠️ Mind the Test Pyramid - don't overdo end-to-end tests](#️-mind-the-test-pyramid---dont-overdo-end-to-end-tests)
   - [Running Testcontainers in CI pipeline](#running-testcontainers-in-ci-pipeline)
   - [Supported Testcontainers](#supported-testcontainers)
     - [Tomodachi](#tomodachi)
     - [Moto](#moto)
     - [LocalStack](#localstack)
     - [SFTP](#sftp)
+  - [Configuration with environment variables](#configuration-with-environment-variables)
+  - [Changing default Docker network](#changing-default-docker-network)
   - [Resources and acknowledgements](#resources-and-acknowledgements)
   - [Development](#development)
 
 ## Installation
 
 ```bash
 pip install tomodachi-testcontainers
 
 # Extra dependency - SFTP container and asyncssh
 pip install tomodachi-testcontainers[sftp]
 ```
 
-## Quickstart and Examples
+## Quickstart and examples
 
 Tomodachi service examples are in [examples/](examples/) folder. Their end-to-end tests are in [tests/test_services](tests/test_services).
 
 For full list of available testcontainers, check out [Supported Testcontainers](#supported-testcontainers) section,
 [tomodachi_testcontainers.containers](src/tomodachi_testcontainers/containers/) module,
 and the official [testcontainers-python](https://github.com/testcontainers/testcontainers-python) library -
 it makes it easy to create your own Testcontainers.
@@ -175,18 +153,14 @@
 with the `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` environment variable.
 
 Examples:
 
 - `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/` - specify just a directory, Dockerfile is inferred automatically
 - `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH=examples/Dockerfile.testing` - explicitly specify the Dockerfile name
 
-⚠️ Make sure that the environment variable is set before running `pytest` -
-e.g. with [pytest-env](https://pypi.org/project/pytest-env/) plugin or
-by setting it in the shell before running `pytest`.
-
 ### Running Tomodachi container from pre-built image
 
 If the Tomodachi service Docker image is already built, you can run the container
 by specifying the image ID in the `TOMODACHI_TESTCONTAINER_IMAGE_ID` environment variable.
 
 It is useful when running tests in the CI pipeline when the image has been already built
 on the build step.
@@ -383,15 +357,15 @@
 that the system will work in production without more manual testing._
 
 _To get a high confidence of releasability, it's necessary to test the system with real dependencies and infrastructure.
 Testcontainers make it easy to spin up real dependencies in Docker containers, and throw them away
 when the tests are finished. They work in thw same way locally and in the CI pipeline, so you need to
 setup test suite only once._
 
-### ⚠️ Mind the Test Pyramid - not overdue end-to-end tests
+### ⚠️ Mind the Test Pyramid - don't overdo end-to-end tests
 
 Despite many benefits of end-to-end tests, they are the most expensive kind 💸 -
 they're slow, sometimes [flaky](https://martinfowler.com/articles/nonDeterminism.html),
 it's hard to understand what's broken when they fail.
 
 End-to-end tests are expensive, but necessary to build confidence of releasability,
 so it's important to use them intentionally and know about other kinds of tests.
@@ -498,14 +472,37 @@
 
 Repository: <https://github.com/atmoz/sftp>
 DockerHub: <https://hub.docker.com/r/atmoz/sftp>
 
 - Available as an extra dependency `sftp` - install with
   `pip install tomodachi-testcontainers[sftp]` or `poetry install -E sftp`
 
+## Configuration with environment variables
+
+⚠️ Make sure that environment variables are set before running `pytest` -
+e.g. with [pytest-env](https://pypi.org/project/pytest-env/) plugin or
+by setting it in the shell before running `pytest`.
+
+| Environment Variable                      | Description                                                                                                                   |
+| :---------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------- |
+| `TESTCONTAINER_DOCKER_NETWORK`            | Launch testcontainers in specified Docker network. Defaults to 'bridge'. Network must be created beforehand                   |
+| `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` | Override path to Dockerfile for building Tomodachi service image. Defaults to '.'                                             |
+| `<CONTAINER-NAME>_TESTCONTAINER_IMAGE_ID` | Override any supported Testcontainer Image ID. Defaults to `None`, `TOMODACHI_TESTCONTAINER_DOCKERFILE_PATH` takes precedence |
+
+## Changing default Docker network
+
+By default, testcontainers are started in the default `bridge` Docker network.
+Sometimes it's useful to start containers in a different network, e.g. a network
+specifically dedicated for running automated tests.
+
+Specify a new network name with the `TOMODACHI_TESTCONTAINER_NETWORK` environment variable.
+The Docker network is not created automatically, so make sure that it exists before running tests.
+
+⚠️ Make sure that the environment variable is set before running `pytest`.
+
 ## Resources and acknowledgements
 
 - [testcontainers.com](https://testcontainers.com/) - home of Testcontainers.
 
 - [testcontainers-python](https://testcontainers-python.readthedocs.io/) - Python SDK for Testcontainers.
 
 - Talk ["Integration tests are needed and simple"](https://softwaregarden.dev/en/talks/integration-tests-are-needed-and-simple/)
@@ -537,14 +534,16 @@
 poetry shell
 pre-commit install
 ```
 
 - Run tests
 
 ```bash
+docker network create tomodachi-testcontainers
+
 pytest
 poetry run test-ci
 ```
 
 - Format and lint code
 
 ```bash
@@ -559,8 +558,7 @@
 ```
 
 - Build package release
 
 ```bash
 poetry build
 ```
-
```

