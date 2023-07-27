# Comparing `tmp/dolbyio-rest-apis-3.7.1.tar.gz` & `tmp/dolbyio-rest-apis-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolbyio-rest-apis-3.7.1.tar", last modified: Mon Jun 19 22:00:50 2023, max compression
+gzip compressed data, was "dolbyio-rest-apis-4.0.0.tar", last modified: Thu Jul 27 00:37:01 2023, max compression
```

## Comparing `dolbyio-rest-apis-3.7.1.tar` & `dolbyio-rest-apis-4.0.0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.951564 dolbyio-rest-apis-3.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.939564 dolbyio-rest-apis-3.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.943564 dolbyio-rest-apis-3.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/ISSUE_TEMPLATE/report-an-issue.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.939564 dolbyio-rest-apis-3.7.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.943564 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/oidc-exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/print-hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.943564 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime-prerequisites.in
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime-prerequisites.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.in
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     4067 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/twine-upload.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.943564 dolbyio-rest-apis-3.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/workflows/build-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.github/workflows/publish-package-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-06-19 22:00:50.951564 dolbyio-rest-apis-3.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.939564 dolbyio-rest-apis-3.7.1/client/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/conference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/internal/http_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/conferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/recordings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/remix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/http_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/http_request_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/analyze_music.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/analyze_speech.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/enhance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/internal/http_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/mastering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.947564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/analyze_music_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/analyze_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/analyze_speech_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/diagnose_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/enhance_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/mastering_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/result_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/transcode_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/transcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.951564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.951564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/internal/http_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:50.951564 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/publish_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/subscribe_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/publish_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/subscribe_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-19 22:00:34.000000 dolbyio-rest-apis-3.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 22:00:50.951564 dolbyio-rest-apis-3.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.441175 dolbyio-rest-apis-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.433175 dolbyio-rest-apis-4.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.433175 dolbyio-rest-apis-4.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/ISSUE_TEMPLATE/report-an-issue.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.433175 dolbyio-rest-apis-4.0.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.433175 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/oidc-exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/print-hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.433175 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime-prerequisites.in
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime-prerequisites.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4067 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/twine-upload.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.437175 dolbyio-rest-apis-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/workflows/build-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.github/workflows/publish-package-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-07-27 00:37:01.441175 dolbyio-rest-apis-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.437175 dolbyio-rest-apis-4.0.0/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.433175 dolbyio-rest-apis-4.0.0/client/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.437175 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.437175 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/conference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.437175 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/internal/http_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.437175 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/monitor/conferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/monitor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/monitor/recordings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/monitor/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/remix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.437175 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/core/http_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/core/http_request_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/core/rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/core/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.441175 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/analyze_music.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/analyze_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/diagnose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/enhance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.441175 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/internal/http_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/mastering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.441175 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/analyze_music_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/analyze_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/analyze_speech_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/diagnose_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/enhance_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/mastering_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/result_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/transcode_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/transcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.441175 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.441175 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/internal/http_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:01.441175 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/models/publish_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/models/subscribe_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/publish_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/subscribe_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-27 00:36:44.000000 dolbyio-rest-apis-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:37:01.441175 dolbyio-rest-apis-4.0.0/setup.cfg
```

### Comparing `dolbyio-rest-apis-3.7.1/.github/ISSUE_TEMPLATE/report-an-issue.md` & `dolbyio-rest-apis-4.0.0/.github/ISSUE_TEMPLATE/report-an-issue.md`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/.gitignore` & `dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/.pre-commit-config.yaml` & `dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/Dockerfile` & `dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/LICENSE.md` & `dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/README.md` & `dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/action.yml` & `dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/action.yml`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/oidc-exchange.py` & `dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/oidc-exchange.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/print-hash.py` & `dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/print-hash.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.in` & `dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.in`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.txt` & `dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/requirements/runtime.txt`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/actions/gh-action-pypi-publish-1.8.6/twine-upload.sh` & `dolbyio-rest-apis-4.0.0/.github/actions/gh-action-pypi-publish-1.8.6/twine-upload.sh`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/workflows/build-package.yml` & `dolbyio-rest-apis-4.0.0/.github/workflows/build-package.yml`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/workflows/codeql-analysis.yml` & `dolbyio-rest-apis-4.0.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.github/workflows/publish-package-to-pypi.yml` & `dolbyio-rest-apis-4.0.0/.github/workflows/publish-package-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.gitignore` & `dolbyio-rest-apis-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/.pylintrc` & `dolbyio-rest-apis-4.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/LICENSE` & `dolbyio-rest-apis-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/PKG-INFO` & `dolbyio-rest-apis-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dolbyio-rest-apis
-Version: 3.7.1
+Version: 4.0.0
 Summary: A Python wrapper for the Dolby.io REST APIs.
 Home-page: https://github.com/dolbyio/dolbyio-rest-apis-client-python
 Author: Dolby.io
 Author-email: fabien.lavocat@dolby.com
 License: MIT
 Project-URL: Documentation, https://docs.dolby.io/communications-apis/reference
 Project-URL: Source, https://github.com/dolbyio/dolbyio-rest-apis-client-python
```

### Comparing `dolbyio-rest-apis-3.7.1/README.md` & `dolbyio-rest-apis-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/README.md` & `dolbyio-rest-apis-4.0.0/client/README.md`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/setup.py` & `dolbyio-rest-apis-4.0.0/client/setup.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/authentication.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/authentication.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/authentication.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/authentication.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,20 @@
 """
 dolbyio_rest_apis.communications.authentication
 ~~~~~~~~~~~~~~~
 
 This module contains the functions to work with the authentication API.
 """
 
-from deprecated import deprecated
 from dolbyio_rest_apis.communications.internal.http_context import CommunicationsHttpContext
 from dolbyio_rest_apis.core.helpers import add_if_not_none
-from dolbyio_rest_apis.core.urls import get_comms_session_url, get_comms_url_v2
+from dolbyio_rest_apis.core.urls import get_comms_url_v2
 from dolbyio_rest_apis.models import AccessToken
 from typing import List
 
-@deprecated(reason='''
-    This function is now deprecated and will be removed in the next release of this SDK.
-    Please start using :meth:`get_client_access_token_v2` instead.
-    ''')
-async def get_client_access_token(
-        app_key: str,
-        app_secret: str,
-        expires_in: int=None,
-    ) -> AccessToken:
-    r"""
-    This API returns an access token that your backend can request on behalf of a client to initialize
-    the Dolby.io SDK in a secure way.
-
-    See: https://docs.dolby.io/communications-apis/reference/get-client-access-token-v1
-
-    Args:
-        app_key: Your Dolby.io App Key.
-        app_secret: Your Dolby.io App Secret.
-        expires_in: (Optional) Access token expiration time in seconds.
-            The maximum value is 86,400, indicating 24 hours.
-            If no value is specified, the default is 3,600, indicating one hour.
-
-    Returns:
-        An :class:`AccessToken` object.
-
-    Raises:
-        HttpRequestError: If a client error one occurred.
-        HTTPError: If one occurred.
-    """
-    data = {
-        'grant_type': 'client_credentials',
-    }
-    add_if_not_none(data, 'expires_in', expires_in)
-
-    async with CommunicationsHttpContext() as http_context:
-        json_response = await http_context.requests_post_basic_auth(
-            app_key=app_key,
-            app_secret=app_secret,
-            url=f'{get_comms_session_url()}/oauth2/token',
-            data=data
-        )
-
-    return AccessToken(json_response)
-
 async def get_client_access_token_v2(
         access_token: str,
         session_scope: List[str],
         external_id: str=None,
         expires_in: int=None,
     ) -> AccessToken:
     r"""
@@ -67,15 +22,16 @@
     the Dolby.io SDK in a secure way.
 
     See: https://docs.dolby.io/communications-apis/reference/get-client-access-token
 
     Args:
         access_token: Access token to use for authentication.
         session_scope: A list of case-sensitive strings allowing you to control
-            what scope of access the client access token should have.
+            what scope of access the client access token should have. If not specified,
+            the token will possess unrestricted access to all resources and actions.
             The API supports the following scopes:
                 - conf:create: Allows creating a new conference.
                 - notifications:set: Allows the client to subscribe to events.
                 - file:convert: Allows converting files.
                 - session:update: Allows updating the participant's name and avatar URL.
             Incorrect values are omitted. If you want to give the token access to all scopes, you can use a wildcard, such as *.
         external_id: (Optional) The unique identifier of the participant who requests the token.
```

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/conference.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/conference.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/internal/http_context.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/internal/http_context.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/models.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,14 +131,25 @@
     def __init__(self, dictionary: dict):
         dict.__init__(self, dictionary)
 
         self.status = get_value_or_default(self, 'status', None)
         self.region = get_value_or_default(self, 'region', None)
         self.alias = get_value_or_default(self, 'alias', None)
 
+class RtsStream(dict):
+    """Representation of an RTS Stream start response."""
+
+    def __init__(self, dictionary: dict):
+        dict.__init__(self, dictionary)
+
+        self.stream_name = get_value_or_default(self, 'streamName', None)
+        self.subscribe_token = get_value_or_default(self, 'subscribeToken', None)
+        self.stream_account_id = get_value_or_default(self, 'streamAccountID', None)
+        self.viewer_url = get_value_or_default(self, 'viewerURL', None)
+
 @dataclass
 class Coordinates:
     """Representation of a Coordinate object."""
     x: int
     y: int
     z: int
```

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/conferences.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/monitor/conferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ~~~~~~~~~~~~~~~
 
 This module contains the functions to work with the monitor API related to conferences.
 """
 
 from dolbyio_rest_apis.communications.internal.http_context import CommunicationsHttpContext
 from dolbyio_rest_apis.communications.monitor.models import GetConferencesResponse, ConferenceSummary, ConferenceStatistics, ConferenceParticipants, ConferenceParticipant
-from dolbyio_rest_apis.core.urls import get_comms_monitor_url
+from dolbyio_rest_apis.core.urls import get_comms_monitor_url_v1
 from typing import Any, Dict, List
 
 async def get_conferences(
         access_token: str,
         tr_from: int=0,
         tr_to: int=9999999999999,
         maximum: int=100,
@@ -55,15 +55,15 @@
     Returns:
         A :class:`GetConferencesResponse` object.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-    url = f'{get_comms_monitor_url()}/conferences'
+    url = f'{get_comms_monitor_url_v1()}/conferences'
 
     params = {
         'from': tr_from,
         'to': tr_to,
         'max': maximum,
         'active': str(active),
         'livestats': str(live_stats),
@@ -125,15 +125,15 @@
     Returns:
         A list of :class:`Conference` objects.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-    url = f'{get_comms_monitor_url()}/conferences'
+    url = f'{get_comms_monitor_url_v1()}/conferences'
 
     params = {
         'from': tr_from,
         'to': tr_to,
         'max': page_size,
         'active': str(active),
         'livestats': str(live_stats),
@@ -183,15 +183,15 @@
         A :class:`ConferenceSummary` object.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
 
-    url = f'{get_comms_monitor_url()}/conferences/{conference_id}'
+    url = f'{get_comms_monitor_url_v1()}/conferences/{conference_id}'
 
     params = {
         'livestats': str(live_stats),
     }
 
     async with CommunicationsHttpContext() as http_context:
         json_response = await http_context.requests_get(
@@ -226,15 +226,15 @@
         A :class:`ConferenceStatistics` object.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
 
-    url = f'{get_comms_monitor_url()}/conferences/{conference_id}/statistics'
+    url = f'{get_comms_monitor_url_v1()}/conferences/{conference_id}/statistics'
 
     async with CommunicationsHttpContext() as http_context:
         json_response = await http_context.requests_get(
             access_token=access_token,
             url=url,
         )
 
@@ -276,15 +276,15 @@
     Returns:
         A :class:`ConferenceParticipants` object.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-    url = f'{get_comms_monitor_url()}/conferences/{conference_id}/participants'
+    url = f'{get_comms_monitor_url_v1()}/conferences/{conference_id}/participants'
 
     params = {
         'from': tr_from,
         'to': tr_to,
         'max': maximum,
     }
     if not participant_type is None:
@@ -332,15 +332,15 @@
     Returns:
         A list of :class:`ConferenceParticipant` objects.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-    url = f'{get_comms_monitor_url()}/conferences/{conference_id}/participants'
+    url = f'{get_comms_monitor_url_v1()}/conferences/{conference_id}/participants'
 
     params = {
         'from': tr_from,
         'to': tr_to,
         'max': page_size,
     }
     if not participant_type is None:
@@ -411,15 +411,15 @@
     Returns:
         A :class:`ConferenceParticipant` object.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-    url = f'{get_comms_monitor_url()}/conferences/{conference_id}/participants/{participant_id}'
+    url = f'{get_comms_monitor_url_v1()}/conferences/{conference_id}/participants/{participant_id}'
 
     params = {
         'from': tr_from,
         'to': tr_to,
         'max': maximum,
     }
     if not participant_type is None:
```

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/models.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/monitor/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class ConferenceOwner(dict):
     """Representation of a Conference Owner."""
 
     def __init__(self, dictionary: dict):
         dict.__init__(self, dictionary)
 
-        self.user_id = get_value_or_default(self, 'userID', None)
+        self.user_id = get_value_or_default(self, 'userId', None)
 
         if in_and_not_none(self, 'metadata'):
             self.metadata = UserMetadata(self['metadata'])
 
 class ConferenceStatisticsMaxParticipants(dict):
     """Representation of a Conference Statistics Max Participants."""
 
@@ -190,108 +190,83 @@
 
         self.user_id = get_value_or_default(self, 'userID', None)
         self.external_name = get_value_or_default(self, 'externalName', None)
         self.external_id = get_value_or_default(self, 'externalId', None)
         self.external_photo_url = get_value_or_default(self, 'externalPhotoUrl', None)
         self.ip_address = get_value_or_default(self, 'ipAddress', None)
 
-class RecordingSplit(dict):
-    """Representation of a Recording Split."""
+class ConferenceRecordingMix(dict):
+    """Representation of a Conference Recording Mix."""
 
     def __init__(self, dictionary: dict):
         dict.__init__(self, dictionary)
 
-        self.start_time = get_value_or_default(self, 'startTime', 0)
-        self.duration = get_value_or_default(self, 'duration', 0)
-        self.size = get_value_or_default(self, 'size', 0)
-        self.file_name = get_value_or_default(self, 'fileName', None)
-        self.url = get_value_or_default(self, 'url', None)
+        self.mix_id = get_value_or_default(self, 'mixId', None)
+        self.width = get_value_or_default(self, 'width', -1)
+        self.height = get_value_or_default(self, 'height', -1)
+        self.layout_url = get_value_or_default(self, 'layoutUrl', None)
 
-        if in_and_not_none(self, 'metadata'):
-            self.metadata = UserMetadata(self['metadata'])
-
-class RecordingRecord(dict):
-    """Representation of a Recording Record."""
+class Conference(dict):
+    """Representation of a Conference."""
 
     def __init__(self, dictionary: dict):
         dict.__init__(self, dictionary)
 
-        self.start_time = get_value_or_default(self, 'startTime', 0)
-        self.duration = get_value_or_default(self, 'duration', 0)
-        self.size = get_value_or_default(self, 'size', 0)
-        self.file_name = get_value_or_default(self, 'fileName', None)
-        self.url = get_value_or_default(self, 'url', None)
-
-        self.splits = []
-        if in_and_not_none(self, 'splits'):
-            for split in self['splits']:
-                self.splits.append(RecordingSplit(split))
+        self.conf_id = get_value_or_default(self, 'confId', None)
+        self.conf_alias = get_value_or_default(self, 'confAlias', None)
 
-class RecordingAudio(dict):
-    """Representation of a Recording Audio."""
+class ConferenceRecording(dict):
+    """Representation of a Conference Recording."""
 
     def __init__(self, dictionary: dict):
         dict.__init__(self, dictionary)
 
-        self.region = get_value_or_default(self, 'region', None)
-
-        if in_and_not_none(self, 'mix'):
-            self.mix = RecordingMix(self['mix'])
-
-        self.records = []
-        if in_and_not_none(self, 'records'):
-            for record in self['records']:
-                self.records.append(RecordingRecord(record))
-
-class Recording(dict):
-    """Representation of a Recording."""
-
-    def __init__(self, dictionary: dict):
-        dict.__init__(self, dictionary)
+        if in_and_not_none(self, 'conference'):
+            self.conference = Conference(self['conference'])
 
-        self.conf_id = get_value_or_default(self, 'confId', None)
-        self.alias = get_value_or_default(self, 'alias', None)
-        self.duration = get_value_or_default(self, 'duration', 0)
-        self.ts = get_value_or_default(self, 'ts', 0)
+        self.region = get_value_or_default(self, 'region', None)
+        self.url = get_value_or_default(self, 'url', None)
+        self.created_at = get_value_or_default(self, 'createdAt', None)
+        self.recording_type = get_value_or_default(self, 'recordingType', None)
+        self.duration = get_value_or_default(self, 'duration', -1)
+        self.filename = get_value_or_default(self, 'filename', None)
+        self.size = get_value_or_default(self, 'size', -1)
+        self.start_time = get_value_or_default(self, 'startTime', 0)
+        self.media_type = get_value_or_default(self, 'mediaType', None)
         self.region = get_value_or_default(self, 'region', None)
 
         if in_and_not_none(self, 'mix'):
-            self.mix = RecordingMix(self['mix'])
-
-        if in_and_not_none(self, 'audio'):
-            self.audio = RecordingAudio(self['audio'])
+            self.mix = ConferenceRecordingMix(self['mix'])
 
 class GetRecordingsResponse(PagedResponse):
     """Representation of a Recordings response."""
 
     def __init__(self, dictionary: dict):
         PagedResponse.__init__(self, dictionary)
 
         self.recordings = []
         if in_and_not_none(self, 'recordings'):
             for recording in self['recordings']:
-                self.recordings.append(Recording(recording))
+                self.recordings.append(ConferenceRecording(recording))
 
-class DolbyVoiceRecording(dict):
-    """Representation of a Dolby Voice Recording."""
+class GetConferenceRecordingsResponse(GetRecordingsResponse):
+    """Representation of a Conference Recordings response."""
 
     def __init__(self, dictionary: dict):
-        dict.__init__(self, dictionary)
+        GetRecordingsResponse.__init__(self, dictionary)
 
-        self.region = get_value_or_default(self, 'region', None)
-        self.conf_id = None
-        self.conf_alias = None
         if in_and_not_none(self, 'conference'):
-            self.conf_id = get_value_or_default(self, 'confId', None)
-            self.conf_alias = get_value_or_default(self, 'confAlias', None)
+            self.conference = Conference(self['conference'])
 
-        self.records = []
-        if in_and_not_none(self, 'records'):
-            for record in self['records']:
-                self.records.append(RecordingRecord(record))
+        self.live_conference = get_value_or_default(self, 'liveConference', False)
+
+        self.recordings = []
+        if in_and_not_none(self, 'recordings'):
+            for recording in self['recordings']:
+                self.recordings.append(ConferenceRecording(recording))
 
 class WebHookResponse(dict):
     """Representation of a WebHook event response."""
 
     def __init__(self, dictionary: dict):
         dict.__init__(self, dictionary)
```

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/recordings.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/monitor/recordings.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,246 +2,300 @@
 dolbyio_rest_apis.communications.monitor.recordings
 ~~~~~~~~~~~~~~~
 
 This module contains the functions to work with the monitor API related to recordings.
 """
 
 from dolbyio_rest_apis.communications.internal.http_context import CommunicationsHttpContext
-from dolbyio_rest_apis.communications.monitor.models import GetRecordingsResponse, Recording, DolbyVoiceRecording
-from dolbyio_rest_apis.core.urls import get_comms_monitor_url
+from dolbyio_rest_apis.communications.monitor.models import GetConferenceRecordingsResponse
+from dolbyio_rest_apis.communications.monitor.models import GetRecordingsResponse, ConferenceRecording
+from dolbyio_rest_apis.core.urls import get_comms_monitor_url_v2
 from typing import Any, List
 
 async def get_recordings(
         access_token: str,
+        region: str=None,
+        media_type: str=None,
+        recording_type: str=None,
         tr_from: int=0,
         tr_to: int=9999999999999,
-        maximum: int=100,
+        page_size: int=100,
         start: str=None,
-        perm: bool=False,
     ) -> GetRecordingsResponse:
     r"""
-    Get recording details
-
-    Get a list of the recorded conference metadata, such as duration or size of the recording.
+    Gets a list of the recorded conference metadata, such as duration or size of the recording.
     This API checks only the recordings that have ended during a specific time range.
     Recordings are indexed based on the ending time.
 
+    This API returns presigned URLs for secure download of the recording files.
+    The URL returned in the response is an AWS S3 presigned URL with a validity of ten minutes.
+
     See: https://docs.dolby.io/communications-apis/reference/get-recordings
 
     Args:
         access_token: Access token to use for authentication.
-        tr_from: The beginning of the time range (in milliseconds that have elapsed since epoch).
-        tr_to: The end of the time range (in milliseconds that have elapsed since epoch).
-        maximum: The maximum number of displayed results.
-            We recommend setting the proper value of this parameter to shorten the response time.
-        start: When the results span multiple pages, use this option to navigate through pages.
+        region: (Optional) The region code in which the mix recording took place.
+        media_type: (Optional) The media type of the recordings to return, 'audio/mpeg' or 'video/mp4'.
+        recording_type: (Optional) The type of the recordings to return, 'mix' or 'participant'.
+        tr_from: (Optional) The beginning of the time range (in milliseconds that have elapsed since epoch).
+        tr_to: (Optional) The end of the time range (in milliseconds that have elapsed since epoch).
+        page_size: (Optional) Number of elements to return per page.
+        start: (Optional) When the results span multiple pages, use this option to navigate through pages.
             By default, only the max number of results is displayed. To see the next results,
             set the start parameter to the value of the next key returned in the previous response.
-        perm: When set to true, the URL is replaced with a monitor API signed URL with unlimited validity.
 
     Returns:
-        A :class:`GetRecordingsResponse` object.
+        A :class:`GetRecordingsV2Response` object.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-    url = f'{get_comms_monitor_url()}/recordings'
+    url = f'{get_comms_monitor_url_v2()}/recordings'
 
     params = {
         'from': tr_from,
         'to': tr_to,
-        'max': maximum,
-        'perm': str(perm).lower(),
+        'max': page_size,
     }
 
+    if not region is None:
+        params['region'] = region
+    if not media_type is None:
+        params['mediaType'] = media_type
+    if not recording_type is None:
+        params['type'] = recording_type
     if not start is None:
         params['start'] = start
 
     async with CommunicationsHttpContext() as http_context:
         json_response = await http_context.requests_get(
             access_token=access_token,
             url=url,
             params=params,
         )
 
     return GetRecordingsResponse(json_response)
 
 async def get_all_recordings(
         access_token: str,
+        region: str=None,
+        media_type: str=None,
+        recording_type: str=None,
         tr_from: int=0,
         tr_to: int=9999999999999,
         page_size: int=100,
-        perm: bool=False,
-    ) -> List[Recording]:
+    ) -> List[ConferenceRecording]:
     r"""
-    Get all recording details
-
-    Get a list of all the recorded conference metadata, such as duration or size of the recording.
+    Gets a list of all the recorded conference metadata, such as duration or size of the recording.
     This API checks only the recordings that have ended during a specific time range.
     Recordings are indexed based on the ending time.
 
+    This API returns presigned URLs for secure download of the recording files.
+    The URL returned in the response is an AWS S3 presigned URL with a validity of ten minutes.
+
     See: https://docs.dolby.io/communications-apis/reference/get-recordings
 
     Args:
         access_token: Access token to use for authentication.
-        tr_from: The beginning of the time range (in milliseconds that have elapsed since epoch).
-        tr_to: The end of the time range (in milliseconds that have elapsed since epoch).
+        region: (Optional) The region code in which the mix recording took place.
+        media_type: (Optional) The media type of the recordings to return, 'audio/mpeg' or 'video/mp4'.
+        recording_type: (Optional) The type of the recordings to return, 'mix' or 'participant'.
+        tr_from: (Optional) The beginning of the time range (in milliseconds that have elapsed since epoch).
+        tr_to: (Optional) The end of the time range (in milliseconds that have elapsed since epoch).
         page_size: (Optional) Number of elements to return per page.
-        perm: When set to true, the URL is replaced with a monitor API signed URL with unlimited validity.
 
     Returns:
-        A list of :class:`Recording` objects.
+        A list of :class:`ConferenceRecording` objects.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-    url = f'{get_comms_monitor_url()}/recordings'
+    url = f'{get_comms_monitor_url_v2()}/recordings'
 
     params = {
         'from': tr_from,
         'to': tr_to,
         'max': page_size,
-        'perm': str(perm).lower(),
     }
 
+    if not region is None:
+        params['region'] = region
+    if not media_type is None:
+        params['mediaType'] = media_type
+    if not recording_type is None:
+        params['type'] = recording_type
+
     recordings = []
 
     async with CommunicationsHttpContext() as http_context:
         elements: List[Any] = await http_context.requests_get_all(
             access_token=access_token,
             url=url,
             params=params,
             property_name='recordings',
             page_size=page_size
         )
 
-    recordings: List[Recording] = []
+    recordings: List[ConferenceRecording] = []
     for element in elements:
-        recording = Recording(element)
+        recording = ConferenceRecording(element)
         recordings.append(recording)
 
     return recordings
 
-async def get_recording(
+async def get_conference_recordings(
         access_token: str,
         conference_id: str,
+        media_type: str=None,
+        recording_type: str=None,
         tr_from: int=0,
         tr_to: int=9999999999999,
         page_size: int=100,
-        perm: bool=False,
-    ) -> GetRecordingsResponse:
+        start: str=None,
+    ) -> GetConferenceRecordingsResponse:
     r"""
-    Get the recording of a specific conference
+    Gets a list of the recorded conference metadata, such as duration or size of the recording.
 
-    Get a list of the recorded conference metadata, such as duration or size of the recording.
-    This API checks the recordings that have ended during a specific time range.
+    This API checks only the recordings that have ended during a specific time range.
     Recordings are indexed based on the ending time.
 
+    This API returns presigned URLs for secure download of the recording files.
+    The URL returned in the response is an AWS S3 presigned URL with a validity of ten minutes.
+
     See: https://docs.dolby.io/communications-apis/reference/get-conference-recordings
 
     Args:
         access_token: Access token to use for authentication.
         conference_id: Identifier of the conference.
-        tr_from: The beginning of the time range (in milliseconds that have elapsed since epoch).
-        tr_to: The end of the time range (in milliseconds that have elapsed since epoch).
+        media_type: (Optional) The media type of the recordings to return, 'audio/mpeg' or 'video/mp4'.
+        recording_type: (Optional) The type of the recordings to return, 'mix' or 'participant'.
+        tr_from:(Optional)  The beginning of the time range (in milliseconds that have elapsed since epoch).
+        tr_to: (Optional) The end of the time range (in milliseconds that have elapsed since epoch).
         page_size: (Optional) Number of elements to return per page.
-        perm: When set to true, the URL is replaced with a monitor API signed URL with unlimited validity.
 
     Returns:
-        A :class:`GetRecordingsResponse` object.
+        A :class:`GetConferenceRecordingsResponse` object.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-    url = f'{get_comms_monitor_url()}/conferences/{conference_id}/recordings'
+    url = f'{get_comms_monitor_url_v2()}/conferences/{conference_id}/recordings'
 
     params = {
         'from': tr_from,
         'to': tr_to,
         'max': page_size,
-        'perm': str(perm).lower(),
     }
 
-    recordings = []
+    if not media_type is None:
+        params['mediaType'] = media_type
+    if not recording_type is None:
+        params['type'] = recording_type
+    if not start is None:
+        params['start'] = start
 
     async with CommunicationsHttpContext() as http_context:
-        elements: List[Any] = await http_context.requests_get_all(
+        json_response = await http_context.requests_get(
             access_token=access_token,
             url=url,
             params=params,
-            property_name='recordings',
-            page_size=page_size
         )
 
-    recordings: List[Recording] = []
-    for element in elements:
-        recording = Recording(element)
-        recordings.append(recording)
+    return GetConferenceRecordingsResponse(json_response)
 
-    return recordings
-
-async def delete_recording(
+async def get_all_conference_recordings(
         access_token: str,
         conference_id: str,
-    ) -> None:
+        media_type: str=None,
+        recording_type: str=None,
+        tr_from: int=0,
+        tr_to: int=9999999999999,
+        page_size: int=100,
+    ) -> List[ConferenceRecording]:
     r"""
-    Delete recordings
+    Gets a list of all the recorded conference metadata, such as duration or size of the recording.
 
-    Delete all recording data related to a specific conference.
+    This API checks only the recordings that have ended during a specific time range.
+    Recordings are indexed based on the ending time.
 
-    Warning: After deleting the recording, it is not possible to restore the recording data.
+    This API returns presigned URLs for secure download of the recording files.
+    The URL returned in the response is an AWS S3 presigned URL with a validity of ten minutes.
 
-    See: https://docs.dolby.io/communications-apis/reference/delete-conference-recordings
+    See: https://docs.dolby.io/communications-apis/reference/get-conference-recordings
 
     Args:
         access_token: Access token to use for authentication.
         conference_id: Identifier of the conference.
+        media_type: (Optional) The media type of the recordings to return, 'audio/mpeg' or 'video/mp4'.
+        recording_type: (Optional) The type of the recordings to return, 'mix' or 'participant'.
+        tr_from:(Optional)  The beginning of the time range (in milliseconds that have elapsed since epoch).
+        tr_to: (Optional) The end of the time range (in milliseconds that have elapsed since epoch).
+        page_size: (Optional) Number of elements to return per page.
+
+    Returns:
+        A list of :class:`ConferenceRecording` objects.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
+    url = f'{get_comms_monitor_url_v2()}/conferences/{conference_id}/recordings'
+
+    params = {
+        'from': tr_from,
+        'to': tr_to,
+    }
 
-    url = f'{get_comms_monitor_url()}/conferences/{conference_id}/recordings'
+    if not media_type is None:
+        params['mediaType'] = media_type
+    if not recording_type is None:
+        params['type'] = recording_type
+
+    recordings = []
 
     async with CommunicationsHttpContext() as http_context:
-        await http_context.requests_delete(
+        elements: List[Any] = await http_context.requests_get_all(
             access_token=access_token,
             url=url,
+            params=params,
+            property_name='recordings',
+            page_size=page_size
         )
 
-async def get_dolby_voice_recordings(
+    recordings: List[ConferenceRecording] = []
+    for element in elements:
+        recording = ConferenceRecording(element)
+        recordings.append(recording)
+
+    return recordings
+
+async def delete_recording(
         access_token: str,
         conference_id: str,
-    ) -> DolbyVoiceRecording:
+    ) -> None:
     r"""
-    Get Dolby Voice audio recordings of a conference
+    Delete recordings
 
-    Get details of all Dolby Voice-based audio recordings, and associated split recordings,
-    for a given conference and download the conference recording in the MP3 audio format.
+    Delete all recording data related to a specific conference.
 
-    See: https://docs.dolby.io/communications-apis/reference/get-dolby-voice-audio-recordings
+    Warning: After deleting the recording, it is not possible to restore the recording data.
+
+    See: https://docs.dolby.io/communications-apis/reference/delete-conference-recordings
 
     Args:
         access_token: Access token to use for authentication.
         conference_id: Identifier of the conference.
 
-    Returns:
-        A :class:`DolbyVoiceRecording` object.
-
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-
-    url = f'{get_comms_monitor_url()}/conferences/{conference_id}/recordings/audio'
+    url = f'{get_comms_monitor_url_v2()}/conferences/{conference_id}/recordings'
 
     async with CommunicationsHttpContext() as http_context:
-        json_response = await http_context.requests_get(
+        await http_context.requests_delete(
             access_token=access_token,
             url=url,
         )
-
-    return DolbyVoiceRecording(json_response)
```

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/monitor/webhooks.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/communications/monitor/webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ~~~~~~~~~~~~~~~
 
 This module contains the functions to work with the monitor API related to webhooks.
 """
 
 from dolbyio_rest_apis.communications.internal.http_context import CommunicationsHttpContext
 from dolbyio_rest_apis.communications.monitor.models import GetWebHookResponse, WebHook
-from dolbyio_rest_apis.core.urls import get_comms_monitor_url
+from dolbyio_rest_apis.core.urls import get_comms_monitor_url_v1
 from typing import Any, List
 
 async def get_events(
         access_token: str,
         conference_id: str=None,
         tr_from: int=0,
         tr_to: int=9999999999999,
@@ -41,15 +41,15 @@
     Returns:
         A :class:`GetWebHookResponse` object.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-    url = f'{get_comms_monitor_url()}/'
+    url = f'{get_comms_monitor_url_v1()}/'
     if not conference_id is None:
         url += f'conferences/{conference_id}/'
     url += 'webhooks'
 
     params = {
         'from': tr_from,
         'to': tr_to,
@@ -96,15 +96,15 @@
     Returns:
         A list of :class:`WebHook` objects.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-    url = f'{get_comms_monitor_url()}/'
+    url = f'{get_comms_monitor_url_v1()}/'
     if not conference_id is None:
         url += f'conferences/{conference_id}/'
     url += 'webhooks'
 
     params = {
         'from': tr_from,
         'to': tr_to,
```

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/communications/recording.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/io.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,105 @@
 """
-dolbyio_rest_apis.communications.recording
+dolbyio_rest_apis.media.io
 ~~~~~~~~~~~~~~~
 
-This module contains the functions to work with the recording API.
+This module contains the functions to work with the IO APIs.
 """
 
-from dolbyio_rest_apis.communications.internal.http_context import CommunicationsHttpContext
-from dolbyio_rest_apis.core.helpers import add_if_not_none
-from dolbyio_rest_apis.core.urls import get_comms_url_v2
+from dolbyio_rest_apis.core.urls import get_mapi_url
+from dolbyio_rest_apis.media.internal.http_context import MediaHttpContext
 
-async def start(
+async def get_upload_url(
         access_token: str,
-        conference_id: str,
-        layout_url: str=None,
-    ) -> None:
+        dlb_url: str,
+    ) -> str or None:
     r"""
-    Starts recording for the specified conference.
-    You can specify a custom layout URL per recording request.
-    The `layoutURL` parameter overrides the layout URL configured in the dashboard.
+    Start Media Input
+
+    To use the Dolby provided temporary storage is a two step process.
+
+    You start by declaring a dlb:// url that you can reference in any other Media API calls.
+    The response will provide a url where you can put your media.
+    This allows you to use the dlb:// url as a short-cut for a temporary storage location.
 
-    See: https://docs.dolby.io/communications-apis/reference/api-recording-start
+    You'll be returned a pre-signed url you can use to PUT and upload your media file.
+    The temporary storage should allow you to read and write to the dlb:// locations for a period of at least 24 hours before it is removed.
+
+    See: https://docs.dolby.io/media-apis/reference/media-input-post
 
     Args:
         access_token: Access token to use for authentication.
-        conference_id: Identifier of the conference.
-        layout_url: Overwrites the layout URL configuration.
-            This field is ignored if it is not relevant regarding recording configuration,
-            for example if live_recording set to false or if the recording is MP3 only.
-            - `null`: uses the layout URL configured in the dashboard (if no URL is set in the dashboard, then uses the Dolby.io default);
-            - `default`: uses the Dolby.io default layout;
-            - URL string: uses this layout URL
+        dlb_url: The `url` should be in the form `dlb://object-key` where the object-key can be any alpha-numeric string.
+            The object-key is unique to your account API Key so there is no risk of collision with other users.
 
     Raises:
         HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-    url = f'{get_comms_url_v2()}/conferences/mix/{conference_id}/recording/start'
-
-    payload = {}
-    add_if_not_none(payload, 'layoutUrl', layout_url)
+    payload = {
+        'url': dlb_url
+    }
 
-    async with CommunicationsHttpContext() as http_context:
-        await http_context.requests_post(
+    async with MediaHttpContext() as http_context:
+        json_response = await http_context.requests_post(
             access_token=access_token,
-            url=url,
-            payload=payload,
+            url=f'{get_mapi_url()}/media/input',
+            payload=payload
         )
 
-async def stop(
+    if 'url' in json_response:
+        return json_response['url']
+
+async def upload_file(
+        upload_url: str,
+        file_path: str,
+    ) -> None:
+    r"""
+    Upload a file.
+
+    Args:
+        upload_url: URL where to upload the file to.
+        file_path: Local file path to upload.
+
+    Raises:
+        HTTPError: If one occurred.
+    """
+    async with MediaHttpContext() as http_context:
+        await http_context.upload(
+            upload_url=upload_url,
+            file_path=file_path,
+        )
+
+async def download_file(
         access_token: str,
-        conference_id: str,
+        dlb_url: str,
+        file_path: str,
     ) -> None:
     r"""
-    Stops the recording of the specified conference.
+    Start Media Download
+
+    You can download media you previously uploaded with /media/input or media that was generated through another Dolby Media API.
 
-    See: https://docs.dolby.io/communications-apis/reference/api-recording-stop
+    The temporary storage should allow you to read and write to the dlb:// locations for a period of at least 24 hours before it is removed.
+
+    See: https://docs.dolby.io/media-apis/reference/media-output-get
 
     Args:
         access_token: Access token to use for authentication.
-        conference_id: Identifier of the conference.
+        dlb_url: The `url` should be in the form `dlb://object-key` where the object-key can be any alpha-numeric string.
+            The object-key is unique to your account API Key so there is no risk of collision with other users.
+        file_path: Local file path where to download the file to.
 
     Raises:
-        HttpRequestError: If a client error one occurred.
         HTTPError: If one occurred.
     """
-    url = f'{get_comms_url_v2()}/conferences/mix/{conference_id}/recording/stop'
+    params = {
+        'url': dlb_url,
+    }
 
-    async with CommunicationsHttpContext() as http_context:
-        await http_context.requests_post(
+    async with MediaHttpContext() as http_context:
+        await http_context.download(
             access_token=access_token,
-            url=url,
+            url=f'{get_mapi_url()}/media/output',
+            file_path=file_path,
+            params=params,
         )
```

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/helpers.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/core/helpers.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/http_context.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/core/http_context.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/http_request_error.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/core/http_request_error.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/rate_limiter.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/core/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/core/urls.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/core/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,37 +2,33 @@
 dolbyio_rest_apis.core.urls
 ~~~~~~~~~~~~~~~
 
 This module contains the URLs to use to call the REST APIs.
 """
 
 API_URL = 'api.dolby.io'
-
 COMMS_URL = 'comms.api.dolby.io'
-COMMS_SESSION_URL = 'session.voxeet.com'
-
 SAPI_URL = 'api.millicast.com'
-
 MAPI_URL = 'api.dolby.com'
 
 def get_api_url() -> str:
     return f'https://{API_URL}/v1'
 
 def get_comms_url_v1() -> str:
     return f'https://{COMMS_URL}/v1'
 
-def get_comms_monitor_url() -> str:
-    return f'{get_comms_url_v1()}/monitor'
-
 def get_comms_url_v2(region: str = None) -> str:
     if region is None:
         return f'https://{COMMS_URL}/v2'
     return f'https://{region}.{COMMS_URL}/v2'
 
-def get_comms_session_url() -> str:
-    return f'https://{COMMS_SESSION_URL}/v1'
+def get_comms_monitor_url_v1() -> str:
+    return f'{get_comms_url_v1()}/monitor'
+
+def get_comms_monitor_url_v2() -> str:
+    return f'{get_comms_url_v2()}/monitor'
 
 def get_rts_url() -> str:
     return f'https://{SAPI_URL}'
 
 def get_mapi_url() -> str:
     return f'https://{MAPI_URL}'
```

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/analyze.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/analyze.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/analyze_music.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/analyze_music.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/analyze_speech.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/analyze_speech.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/diagnose.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/diagnose.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/enhance.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/enhance.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/internal/http_context.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/internal/http_context.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/jobs.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/jobs.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/mastering.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/mastering.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/analyze_music_response.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/analyze_music_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/analyze_response.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/analyze_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/analyze_speech_response.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/analyze_speech_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/diagnose_response.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/diagnose_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/enhance_response.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/enhance_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/job_response.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/job_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/jobs_response.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/jobs_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/mastering_response.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/mastering_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/result_error.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/result_error.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/transcode_response.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/transcode_response.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/models/webhook.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/models/webhook.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/transcode.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/transcode.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/media/webhooks.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/media/webhooks.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/models.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/models.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/cluster.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/cluster.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/internal/http_context.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/internal/http_context.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/cluster.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/models/cluster.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/core.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/models/core.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/publish_token.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/models/publish_token.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/models/subscribe_token.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/models/subscribe_token.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/publish_token.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/publish_token.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/stream.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/stream.py`

 * *Files identical despite different names*

### Comparing `dolbyio-rest-apis-3.7.1/client/src/dolbyio_rest_apis/streaming/subscribe_token.py` & `dolbyio-rest-apis-4.0.0/client/src/dolbyio_rest_apis/streaming/subscribe_token.py`

 * *Files identical despite different names*

