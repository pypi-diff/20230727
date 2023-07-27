# Comparing `tmp/newrelic-8.8.1.tar.gz` & `tmp/newrelic-8.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic-8.8.1.tar", last modified: Mon Jun 26 21:30:53 2023, max compression
+gzip compressed data, was "newrelic-8.9.0.tar", last modified: Thu Jul 27 21:42:28 2023, max compression
```

## Comparing `newrelic-8.8.1.tar` & `newrelic-8.9.0.tar`

### file list

```diff
@@ -1,1217 +1,1225 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.301334 newrelic-8.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 21:30:38.000000 newrelic-8.8.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-26 21:30:38.000000 newrelic-8.8.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/ISSUE_TEMPLATE/troubleshooting.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.153334 newrelic-8.8.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.github/actions/setup-python-matrix/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/actions/setup-python-matrix/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.github/containers/
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/containers/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/containers/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     1704 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/containers/install-python.sh
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/containers/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/mergify.yml
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1263 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/scripts/retry.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/workflows/build-ci-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/workflows/deploy-python.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      964 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/workflows/get-envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/workflows/mega-linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)    22953 2023-06-26 21:30:38.000000 newrelic-8.8.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-26 21:30:38.000000 newrelic-8.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-26 21:30:38.000000 newrelic-8.8.1/.mega-linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-06-26 21:30:38.000000 newrelic-8.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-26 21:30:38.000000 newrelic-8.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-26 21:30:38.000000 newrelic-8.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-06-26 21:30:53.301334 newrelic-8.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-26 21:30:38.000000 newrelic-8.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-26 21:30:38.000000 newrelic-8.8.1/ROADMAP.md
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-26 21:30:38.000000 newrelic-8.8.1/THIRD_PARTY_NOTICES.md
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-26 21:30:38.000000 newrelic-8.8.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.165334 newrelic-8.8.1/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.165334 newrelic-8.8.1/newrelic/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/debug_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/generate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/license_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/network_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/record_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/run_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/run_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/server_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/admin/validate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.169334 newrelic-8.8.1/newrelic/api/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/asgi_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/background_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/cat_header_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/database_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/datastore_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/error_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/external_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/function_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/function_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/generator_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/graphql_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/html_insertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/in_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/memcache_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/message_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/message_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/object_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/out_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/post_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/pre_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/profile_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/solr_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/supportability.py
--rw-r--r--   0 runner    (1001) docker     (123)    26330 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/time_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    69566 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/transaction_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    35165 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/web_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    25411 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/api/wsgi_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.169334 newrelic-8.8.1/newrelic/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/bootstrap/sitecustomize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.173334 newrelic-8.8.1/newrelic/common/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/_monotonic.c
--rw-r--r--   0 runner    (1001) docker     (123)    21225 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/agent_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/async_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/async_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    64813 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/coroutine.py
--rw-r--r--   0 runner    (1001) docker     (123)    18641 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/encoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/log_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/object_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/object_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/package_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/streaming_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/common/utilization.py
--rw-r--r--   0 runner    (1001) docker     (123)   114637 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18465 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.177334 newrelic-8.8.1/newrelic/core/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/_thread_utilization.c
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/adaptive_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31544 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/agent_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/agent_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)    70315 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    40694 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/custom_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/database_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/datastore_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/error_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/error_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/external_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/function_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/graphql_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/graphql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/infinite_tracing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/infinite_tracing_v3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/infinite_tracing_v4_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/internal_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/log_event_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/loop_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/memcache_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/message_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/node_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16490 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/profile_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/root_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/rules_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/solr_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/stack_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    64178 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/stats_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/string_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/thread_utilization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/trace_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    22650 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/core/transaction_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.181334 newrelic-8.8.1/newrelic/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.181334 newrelic-8.8.1/newrelic/extras/framework_django/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/extras/framework_django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.181334 newrelic-8.8.1/newrelic/extras/framework_django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/extras/framework_django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/extras/framework_django/templatetags/newrelic_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.193334 newrelic-8.8.1/newrelic/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_asgiref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_cheroot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_cherrypy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_daphne.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_flup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_gevent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_gunicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_hypercorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_meinheld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_paste.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_uvicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_waitress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/adapter_wsgiref.py
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/application_celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/application_gearman.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_cornice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_djangorestframework.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_flask_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_graphqlserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_piston.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/component_tastypie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/coroutines_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/coroutines_gevent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_cx_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_dbapi2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_ibm_db_dbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_mysqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_oursql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_psycopg2cffi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_psycopg2ct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_pymssql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_pymysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_pyodbc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/database_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_aioredis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_aredis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_bmemcached.py
--rw-r--r--   0 runner    (1001) docker     (123)    21862 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_memcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_motor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_pyelasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_pylibmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_pymemcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_pymongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_pysolr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_solrpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/datastore_umemcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_botocore.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_dropbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_facepy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_feedparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_httplib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_httplib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_pywapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_thrift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_urllib2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/external_xmlrpclib.py
--rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_ariadne.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_cherrypy.py
--rw-r--r--   0 runner    (1001) docker     (123)    42753 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_django.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_django_py3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_falcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_graphene.py
--rw-r--r--   0 runner    (1001) docker     (123)    17278 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_pylons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_sanic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_starlette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_strawberry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_tornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_web2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/framework_webpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/logger_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/logger_loguru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/memcache_memcache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/messagebroker_confluentkafka.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/messagebroker_kafkapython.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/messagebroker_pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/middleware_flask_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/middleware_weberror.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/template_genshi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/template_jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/hooks/template_mako.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.193334 newrelic-8.8.1/newrelic/network/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/network/addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/network/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11460 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/newrelic.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.193334 newrelic-8.8.1/newrelic/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/asgiref_compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.193334 newrelic-8.8.1/newrelic/packages/isort/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.193334 newrelic-8.8.1/newrelic/packages/isort/stdlibs/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/all.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py27.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py310.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py311.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py36.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py37.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py38.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/isort/stdlibs/py39.py
--rw-r--r--   0 runner    (1001) docker     (123)    34549 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/six.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/urllib3/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    39128 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/connectionpool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/urllib3/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/urllib3/contrib/_securetransport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/appengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/securetransport.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/contrib/socks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/filepost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/urllib3/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/urllib3/packages/backports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/packages/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/packages/backports/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/packages/six.py
--rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/poolmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/urllib3/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    22003 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/ssltransport.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/urllib3/util/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/packages/wrapt/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95815 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/_wrappers.c
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    35521 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/packages/wrapt/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/newrelic/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/samplers/cpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/samplers/data_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/samplers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/samplers/gc_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-26 21:30:38.000000 newrelic-8.8.1/newrelic/samplers/memory_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.165334 newrelic-8.8.1/newrelic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    54801 2023-06-26 21:30:53.000000 newrelic-8.8.1/newrelic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-26 21:30:52.000000 newrelic-8.8.1/newrelic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-26 21:30:38.000000 newrelic-8.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/scripts/newrelic-admin
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-26 21:30:53.301334 newrelic-8.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-06-26 21:30:38.000000 newrelic-8.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.161334 newrelic-8.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/tests/adapter_cheroot/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_cheroot/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_cheroot/test_wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/tests/adapter_daphne/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_daphne/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_daphne/test_daphne.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/tests/adapter_gevent/
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gevent/_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gevent/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gevent/test_patching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gevent/test_pywsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/tests/adapter_gunicorn/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/asgi_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/async_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/test_aiohttp_app_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/test_asgi_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/test_gaiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_gunicorn/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/tests/adapter_hypercorn/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_hypercorn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_hypercorn/test_hypercorn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.201334 newrelic-8.8.1/tests/adapter_uvicorn/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_uvicorn/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_uvicorn/test_uvicorn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.205334 newrelic-8.8.1/tests/adapter_waitress/
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_waitress/_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_waitress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/adapter_waitress/test_wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.209334 newrelic-8.8.1/tests/agent_features/
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/_test_async_coroutine_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/_test_async_coroutine_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/_test_code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_apdex_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    32524 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_asgi_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_asgi_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_asgi_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_asgi_w3c_trace_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_async_context_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_async_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    35695 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_attributes_in_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_background_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    33137 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_browser_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_collector_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    20320 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_coroutine_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_coroutine_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_custom_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_dead_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_error_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_error_group_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_event_loop_wait_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    12523 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_exception_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_function_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    24665 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_high_security_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_ignore_expected_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_log_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_logs_in_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_notice_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_priority_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_serverless_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    24778 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_span_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_stack_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_supportability_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_synthetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_time_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15892 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_transaction_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_transaction_trace_segments.py
--rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_w3c_trace_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_web_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_features/test_wsgi_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.209334 newrelic-8.8.1/tests/agent_streaming/
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_streaming/_test_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_streaming/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17309 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_streaming/test_infinite_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_streaming/test_span_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_streaming/test_stream_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_streaming/test_streaming_rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/agent_unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/_test_import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_agent_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    20228 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_agent_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_check_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_connect_response_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_distributed_tracing_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_full_uri_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    31635 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_harvest_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    20941 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_infinite_trace_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_package_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_region_aware_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_sampler_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_serverless_mode_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_trace_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/agent_unittests/test_utilization_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/application_celery/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/application_celery/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/application_celery/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/application_celery/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/application_celery/test_celery_max_tasks_per_child.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/application_gearman/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/application_gearman/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/application_gearman/test_gearman.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/component_djangorestframework/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_djangorestframework/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_djangorestframework/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_djangorestframework/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_djangorestframework/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_djangorestframework/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_djangorestframework/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/component_flask_rest/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_flask_rest/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_flask_rest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_flask_rest/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/component_graphqlserver/
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_graphqlserver/_test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_graphqlserver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_graphqlserver/test_graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/component_tastypie/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/component_tastypie/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.213334 newrelic-8.8.1/tests/coroutines_asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/coroutines_asyncio/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/coroutines_asyncio/test_context_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.217334 newrelic-8.8.1/tests/cross_agent/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.217334 newrelic-8.8.1/tests/cross_agent/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/attribute_configuration.json
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/cat_map.json
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/collector_hostname.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.217334 newrelic-8.8.1/tests/cross_agent/fixtures/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/datastores/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/datastores/datastore_instances.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.221334 newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    48250 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json
--rw-r--r--   0 runner    (1001) docker     (123)    58950 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/trace_context.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.221334 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/cases.json
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-0.9.1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/empty.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/heroku.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/invalid-length.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-lxc-container.txt
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-no-container.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.10-no-container.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/labels.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.225334 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/api_gateway_auth.json
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/batch_get.json
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/batch_submit.json
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudformation_create.json
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudwatch_logs.json
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/codecommit.json
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cognito_sync.json
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis.json
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_analytics.json
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_apache.json
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_invoke.json
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/lex_appointment.json
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/lex_book_car.json
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/s3_put.json
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/scheduled_event.json
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/ses.json
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/smarthome_discovery.json
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/smarthome_turn_off.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/sns.json
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/sqs.json
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.233334 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.query.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.colon_obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.explain.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.obfuscated.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.query.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.237334 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_1logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_2core_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38341 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/malformed_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.237334 newrelic-8.8.1/tests/cross_agent/fixtures/proc_meminfo/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_meminfo/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_meminfo/malformed_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_client_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_cookie.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.237334 newrelic-8.8.1/tests/cross_agent/fixtures/rum_footer_insertion_location/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_footer_insertion_location/close-body-in-comment.html
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_footer_insertion_location/dynamic-iframe.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.241334 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/empty_head
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html
--rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html
--rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.245334 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.245334 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.245334 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql
--rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.obfuscated
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/sql_parsing.json
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/transaction_segment_terms.json
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/url_clean.json
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/url_domain_extraction.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.245334 newrelic-8.8.1/tests/cross_agent/fixtures/utilization/
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization/boot_id.json
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization/utilization_json.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.249334 newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json
--rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_agent_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_aws_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_azure_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_boot_id_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_cat_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_collector_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_datstore_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_gcp_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_labels_and_rollups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_lambda_event_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_pcf_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_rum_client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_sql_obfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_transaction_segment_terms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_utilization_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/cross_agent/test_w3c_trace_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.249334 newrelic-8.8.1/tests/datastore_aioredis/
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_custom_conn_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_get_and_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aioredis/test_uninstrumented_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.249334 newrelic-8.8.1/tests/datastore_aredis/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_custom_conn_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_get_and_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_aredis/test_uninstrumented_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.249334 newrelic-8.8.1/tests/datastore_asyncpg/
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_asyncpg/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_asyncpg/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_asyncpg/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.249334 newrelic-8.8.1/tests/datastore_bmemcached/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_bmemcached/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_bmemcached/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.249334 newrelic-8.8.1/tests/datastore_elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_database_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_instrumented_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_mget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_elasticsearch/test_transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_memcache/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_memcache/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_memcache/test_all_methods_wrapped.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_memcache/test_memcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_memcache/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_memcache/test_span_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_mysql/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_mysql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_mysql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_postgresql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_postgresql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_psycopg2/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_database_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_explain_plans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_forward_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_obfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_rollback.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_slow_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_psycopg2cffi/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2cffi/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2cffi/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_psycopg2cffi/test_explain_plans.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_pylibmc/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pylibmc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pylibmc/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_pymemcache/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pymemcache/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pymemcache/test_memcache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_pymongo/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pymongo/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pymongo/test_pymongo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_pymysql/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pymysql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pymysql/test_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_pyodbc/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pyodbc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pyodbc/test_pyodbc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.253334 newrelic-8.8.1/tests/datastore_pysolr/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pysolr/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_pysolr/test_solr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.261334 newrelic-8.8.1/tests/datastore_redis/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_custom_conn_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_get_and_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_multiple_dbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_rb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_span_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_redis/test_uninstrumented_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.261334 newrelic-8.8.1/tests/datastore_solrpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_solrpy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_solrpy/test_solr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.261334 newrelic-8.8.1/tests/datastore_sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_sqlite/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_sqlite/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/datastore_sqlite/test_obfuscation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.261334 newrelic-8.8.1/tests/external_boto3/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_boto3/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_boto3/test_boto3_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_boto3/test_boto3_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_boto3/test_boto3_sns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_botocore/
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_botocore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_botocore/test_botocore_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_botocore/test_botocore_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_botocore/test_botocore_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_botocore/test_botocore_sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_feedparser/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_feedparser/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_feedparser/packages.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_feedparser/test_feedparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_http/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_http/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_http/test_http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_httplib/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httplib/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httplib/test_httplib.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httplib/test_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httplib/test_urllib2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_httplib2/
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httplib2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httplib2/test_httplib2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_httpx/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httpx/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_httpx/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_requests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_requests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_requests/test_span_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.265334 newrelic-8.8.1/tests/external_urllib3/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_urllib3/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/external_urllib3/test_urllib3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.269334 newrelic-8.8.1/tests/framework_aiohttp/
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_client_async_await.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_client_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_externals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_server_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_aiohttp/test_ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.269334 newrelic-8.8.1/tests/framework_ariadne/
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/schema.graphql
--rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/test_application_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/test_asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_ariadne/test_wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.269334 newrelic-8.8.1/tests/framework_bottle/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_bottle/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_bottle/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_bottle/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.269334 newrelic-8.8.1/tests/framework_cherrypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_cherrypy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_cherrypy/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_cherrypy/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_cherrypy/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_cherrypy/test_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.269334 newrelic-8.8.1/tests/framework_django/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.273334 newrelic-8.8.1/tests/framework_django/dummy_app/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/dummy_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.273334 newrelic-8.8.1/tests/framework_django/dummy_app/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/dummy_app/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/dummy_app/templatetags/custom_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.273334 newrelic-8.8.1/tests/framework_django/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/templates/main.html
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/templates/render_exception.html
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/templates/results.html
--rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/test_asgi_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_django/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.273334 newrelic-8.8.1/tests/framework_falcon/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_falcon/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_falcon/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_falcon/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.273334 newrelic-8.8.1/tests/framework_fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_fastapi/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_fastapi/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_fastapi/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.277334 newrelic-8.8.1/tests/framework_flask/
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_application_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_user_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/_test_views_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_user_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_flask/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.277334 newrelic-8.8.1/tests/framework_graphene/
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphene/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphene/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphene/test_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.277334 newrelic-8.8.1/tests/framework_graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphql/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphql/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphql/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_graphql/test_application_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.277334 newrelic-8.8.1/tests/framework_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/_test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.281334 newrelic-8.8.1/tests/framework_grpc/sample_application/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/sample_application/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/sample_application/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/sample_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/sample_application/sample_application.proto
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_grpc/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.281334 newrelic-8.8.1/tests/framework_pyramid/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_pyramid/_test_append_slash_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_pyramid/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_pyramid/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_pyramid/test_append_slash_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_pyramid/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_pyramid/test_cornice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.285334 newrelic-8.8.1/tests/framework_sanic/
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_sanic/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_sanic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_sanic/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_sanic/test_cross_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.289334 newrelic-8.8.1/tests/framework_starlette/
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/_test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/_test_bg_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/_test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/test_bg_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_starlette/test_graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.289334 newrelic-8.8.1/tests/framework_strawberry/
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_strawberry/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_strawberry/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_strawberry/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_strawberry/test_application_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_strawberry/test_asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.289334 newrelic-8.8.1/tests/framework_tornado/
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_tornado/_target_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_tornado/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_tornado/test_custom_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_tornado/test_externals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_tornado/test_inbound_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/framework_tornado/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.289334 newrelic-8.8.1/tests/logger_logging/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_logging/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_logging/test_local_decorating.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_logging/test_log_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_logging/test_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_logging/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_logging/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.289334 newrelic-8.8.1/tests/logger_loguru/
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_loguru/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_loguru/test_local_decorating.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_loguru/test_log_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_loguru/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_loguru/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/logger_loguru/test_stack_inspection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.289334 newrelic-8.8.1/tests/messagebroker_confluentkafka/
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_confluentkafka/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_confluentkafka/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_confluentkafka/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_confluentkafka/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.293335 newrelic-8.8.1/tests/messagebroker_kafkapython/
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_kafkapython/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_kafkapython/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_kafkapython/test_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_kafkapython/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_kafkapython/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.293335 newrelic-8.8.1/tests/messagebroker_pika/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/minversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_memory_leak.py
--rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_pika_async_connection_consume.py
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_pika_blocking_connection_consume.py
--rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_pika_produce.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/messagebroker_pika/test_pika_supportability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.293335 newrelic-8.8.1/tests/template_genshi/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/template_genshi/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/template_genshi/test_genshi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.293335 newrelic-8.8.1/tests/template_mako/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/template_mako/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/template_mako/test_mako.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.293335 newrelic-8.8.1/tests/testing_support/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/asgi_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/db_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/external_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.293335 newrelic-8.8.1/tests/testing_support/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/fixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/fixture/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    50495 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/mock_external_grpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/mock_external_http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/mock_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/sample_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/sample_asgi_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:30:53.301334 newrelic-8.8.1/tests/testing_support/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_apdex_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_application_error_event_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_application_error_trace_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_application_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_browser_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_code_level_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_cross_process_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_custom_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_custom_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_database_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_database_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_database_trace_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_datastore_trace_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_distributed_trace_accepted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_distributed_tracing_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_error_event_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_error_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_error_trace_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_error_trace_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_external_node_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_function_called.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_internal_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_log_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_log_event_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_log_event_count_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_log_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_log_events_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_messagebroker_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_metric_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_non_transaction_error_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_outbound_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_serverless_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_serverless_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_serverless_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_slow_sql_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_span_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_sql_obfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_synthetics_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_synthetics_transaction_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_time_metrics_outside_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_error_trace_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_event_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_event_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_slow_sql_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_transaction_trace_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_tt_collector_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_tt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-26 21:30:38.000000 newrelic-8.8.1/tests/testing_support/validators/validate_tt_segment_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    26114 2023-06-26 21:30:38.000000 newrelic-8.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.376465 newrelic-8.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.172451 newrelic-8.9.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-27 21:42:09.000000 newrelic-8.9.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 21:42:09.000000 newrelic-8.9.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.172451 newrelic-8.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.172451 newrelic-8.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/ISSUE_TEMPLATE/troubleshooting.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.172451 newrelic-8.9.0/.github/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/containers/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/containers/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/containers/install-python.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/containers/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.172451 newrelic-8.9.0/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/scripts/retry.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.176452 newrelic-8.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/workflows/build-ci-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/workflows/deploy-python.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      964 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/workflows/get-envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/workflows/mega-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    26648 2023-07-27 21:42:09.000000 newrelic-8.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-27 21:42:09.000000 newrelic-8.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-27 21:42:09.000000 newrelic-8.9.0/.mega-linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-07-27 21:42:09.000000 newrelic-8.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-27 21:42:09.000000 newrelic-8.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-27 21:42:09.000000 newrelic-8.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-27 21:42:28.376465 newrelic-8.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-27 21:42:09.000000 newrelic-8.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-27 21:42:09.000000 newrelic-8.9.0/ROADMAP.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-27 21:42:09.000000 newrelic-8.9.0/THIRD_PARTY_NOTICES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-27 21:42:09.000000 newrelic-8.9.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.176452 newrelic-8.9.0/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.180452 newrelic-8.9.0/newrelic/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/admin/debug_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/admin/generate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/admin/license_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/admin/local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/admin/network_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/admin/record_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/admin/run_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/admin/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/admin/server_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/admin/validate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.184452 newrelic-8.9.0/newrelic/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/asgi_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/background_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/cat_header_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/database_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/datastore_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/error_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/external_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/function_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/function_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/generator_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/graphql_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/html_insertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/in_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/memcache_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/message_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/message_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/object_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/out_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/post_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/pre_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/profile_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/solr_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/supportability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26330 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/time_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71295 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/transaction_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35165 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/web_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25411 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/api/wsgi_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.184452 newrelic-8.9.0/newrelic/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/bootstrap/sitecustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.188452 newrelic-8.9.0/newrelic/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/_monotonic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21225 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/agent_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/async_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/async_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64813 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18641 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/encoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/log_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/object_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/object_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/package_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/streaming_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/common/utilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115138 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18465 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.192453 newrelic-8.9.0/newrelic/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/_thread_utilization.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/adaptive_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31544 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/agent_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/agent_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70315 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40694 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/custom_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/database_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/datastore_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/error_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/error_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/external_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/function_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/graphql_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/graphql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/infinite_tracing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/infinite_tracing_v3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/infinite_tracing_v4_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/internal_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/log_event_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/loop_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/memcache_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/message_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/node_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16490 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/profile_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/root_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/rules_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/solr_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/stack_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64178 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/stats_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/string_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/thread_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/trace_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22650 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/core/transaction_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.192453 newrelic-8.9.0/newrelic/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.192453 newrelic-8.9.0/newrelic/extras/framework_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/extras/framework_django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.192453 newrelic-8.9.0/newrelic/extras/framework_django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/extras/framework_django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/extras/framework_django/templatetags/newrelic_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.208454 newrelic-8.9.0/newrelic/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_asgiref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_cheroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_cherrypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_daphne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_flup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_gevent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_gunicorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_hypercorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_meinheld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_paste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_uvicorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_waitress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/adapter_wsgiref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/application_celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/application_gearman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/component_cornice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/component_djangorestframework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/component_flask_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/component_graphqlserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/component_piston.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/component_sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/component_tastypie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/coroutines_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/coroutines_gevent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_cx_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_dbapi2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_ibm_db_dbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_mysqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_oursql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_psycopg2cffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_psycopg2ct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_pymssql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_pymysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_pyodbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/database_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_aioredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_aredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_bmemcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21862 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_memcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_motor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_pyelasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_pylibmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_pymemcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_pysolr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13438 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_solrpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/datastore_umemcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_botocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_facepy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_feedparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_httplib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_httplib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_pywapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_thrift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_urllib2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_urllib3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/external_xmlrpclib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12197 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_ariadne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_cherrypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42753 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_django_py3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_falcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_graphene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17278 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_pylons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10420 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_sanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_starlette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_tornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_web2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/framework_webpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/logger_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/logger_loguru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/memcache_memcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/messagebroker_confluentkafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/messagebroker_kafkapython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/messagebroker_pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/middleware_flask_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/middleware_weberror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/template_genshi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/template_jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/hooks/template_mako.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.208454 newrelic-8.9.0/newrelic/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/network/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/network/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11460 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/newrelic.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.208454 newrelic-8.9.0/newrelic/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/asgiref_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.208454 newrelic-8.9.0/newrelic/packages/isort/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.212454 newrelic-8.9.0/newrelic/packages/isort/stdlibs/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/stdlibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/stdlibs/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/stdlibs/py2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/stdlibs/py27.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/stdlibs/py3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/stdlibs/py310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/stdlibs/py311.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/stdlibs/py36.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/stdlibs/py37.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/stdlibs/py38.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/isort/stdlibs/py39.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34549 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/six.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.212454 newrelic-8.9.0/newrelic/packages/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39128 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/connectionpool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.212454 newrelic-8.9.0/newrelic/packages/urllib3/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.216454 newrelic-8.9.0/newrelic/packages/urllib3/contrib/_securetransport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/contrib/appengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/contrib/securetransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/contrib/socks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/filepost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.216454 newrelic-8.9.0/newrelic/packages/urllib3/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.216454 newrelic-8.9.0/newrelic/packages/urllib3/packages/backports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/packages/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/poolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.216454 newrelic-8.9.0/newrelic/packages/urllib3/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22003 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/ssl_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/ssltransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/urllib3/util/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.220455 newrelic-8.9.0/newrelic/packages/wrapt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/wrapt/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/wrapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95815 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/wrapt/_wrappers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/wrapt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21332 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/wrapt/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/wrapt/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35521 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/packages/wrapt/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.220455 newrelic-8.9.0/newrelic/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/samplers/cpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/samplers/data_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/samplers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/samplers/gc_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-27 21:42:09.000000 newrelic-8.9.0/newrelic/samplers/memory_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-27 21:42:27.000000 newrelic-8.9.0/newrelic/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.176452 newrelic-8.9.0/newrelic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-27 21:42:27.000000 newrelic-8.9.0/newrelic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    55103 2023-07-27 21:42:28.000000 newrelic-8.9.0/newrelic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:42:27.000000 newrelic-8.9.0/newrelic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 21:42:27.000000 newrelic-8.9.0/newrelic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:42:27.000000 newrelic-8.9.0/newrelic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 21:42:27.000000 newrelic-8.9.0/newrelic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-27 21:42:27.000000 newrelic-8.9.0/newrelic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-27 21:42:09.000000 newrelic-8.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.220455 newrelic-8.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       68 2023-07-27 21:42:09.000000 newrelic-8.9.0/scripts/newrelic-admin
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-27 21:42:28.376465 newrelic-8.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-07-27 21:42:09.000000 newrelic-8.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.168451 newrelic-8.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.220455 newrelic-8.9.0/tests/adapter_cheroot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_cheroot/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_cheroot/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.220455 newrelic-8.9.0/tests/adapter_daphne/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_daphne/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_daphne/test_daphne.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.220455 newrelic-8.9.0/tests/adapter_gevent/
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gevent/_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gevent/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gevent/test_patching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gevent/test_pywsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.220455 newrelic-8.9.0/tests/adapter_gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gunicorn/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gunicorn/asgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gunicorn/async_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gunicorn/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gunicorn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gunicorn/test_aiohttp_app_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gunicorn/test_asgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gunicorn/test_gaiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_gunicorn/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.220455 newrelic-8.9.0/tests/adapter_hypercorn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_hypercorn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_hypercorn/test_hypercorn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.224455 newrelic-8.9.0/tests/adapter_uvicorn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_uvicorn/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_uvicorn/test_uvicorn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.224455 newrelic-8.9.0/tests/adapter_waitress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_waitress/_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_waitress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/adapter_waitress/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.232455 newrelic-8.9.0/tests/agent_features/
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/_test_async_coroutine_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/_test_async_coroutine_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/_test_code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_apdex_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32524 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_asgi_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_asgi_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_asgi_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_asgi_w3c_trace_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_async_context_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_async_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35695 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_attributes_in_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_background_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33137 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_browser_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_collector_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30603 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_coroutine_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_coroutine_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_custom_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_custom_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_dead_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_error_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_error_group_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_event_loop_wait_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12523 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_exception_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_function_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24665 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_high_security_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_ignore_expected_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_log_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_logs_in_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_notice_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_priority_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_profile_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_serverless_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24778 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_span_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_stack_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_supportability_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_synthetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_time_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15892 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_transaction_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_transaction_trace_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_w3c_trace_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_web_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_features/test_wsgi_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.232455 newrelic-8.9.0/tests/agent_streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_streaming/_test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_streaming/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17309 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_streaming/test_infinite_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_streaming/test_span_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_streaming/test_stream_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_streaming/test_streaming_rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.232455 newrelic-8.9.0/tests/agent_unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/_test_import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_agent_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20228 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_agent_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_check_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_connect_response_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_distributed_tracing_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_full_uri_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31635 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_harvest_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20941 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_infinite_trace_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_package_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_region_aware_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_sampler_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_serverless_mode_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_trace_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/agent_unittests/test_utilization_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.236456 newrelic-8.9.0/tests/application_celery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/application_celery/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/application_celery/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/application_celery/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/application_celery/test_celery_max_tasks_per_child.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.236456 newrelic-8.9.0/tests/application_gearman/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/application_gearman/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/application_gearman/test_gearman.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.236456 newrelic-8.9.0/tests/component_djangorestframework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_djangorestframework/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_djangorestframework/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_djangorestframework/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_djangorestframework/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_djangorestframework/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_djangorestframework/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.236456 newrelic-8.9.0/tests/component_flask_rest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_flask_rest/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_flask_rest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_flask_rest/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.236456 newrelic-8.9.0/tests/component_graphqlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_graphqlserver/_test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_graphqlserver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_graphqlserver/test_graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.236456 newrelic-8.9.0/tests/component_tastypie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_tastypie/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_tastypie/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_tastypie/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_tastypie/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_tastypie/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_tastypie/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/component_tastypie/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.236456 newrelic-8.9.0/tests/coroutines_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/coroutines_asyncio/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/coroutines_asyncio/test_context_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.240456 newrelic-8.9.0/tests/cross_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.244456 newrelic-8.9.0/tests/cross_agent/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/attribute_configuration.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/cat_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/collector_hostname.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.244456 newrelic-8.9.0/tests/cross_agent/fixtures/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/datastores/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/datastores/datastore_instances.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.244456 newrelic-8.9.0/tests/cross_agent/fixtures/distributed_tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/distributed_tracing/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    48250 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58950 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/distributed_tracing/trace_context.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.248456 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/cases.json
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-0.9.1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/heroku.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/invalid-length.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-lxc-container.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.04-no-container.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/ubuntu-14.10-no-container.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/labels.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.252457 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_auth.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/batch_get.json
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/batch_submit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudformation_create.json
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudwatch_logs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/codecommit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cognito_sync.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_analytics.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_apache.json
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose_invoke.json
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/lex_appointment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/lex_book_car.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/s3_put.json
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/scheduled_event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/ses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/smarthome_discovery.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/smarthome_turn_off.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/sns.json
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/sqs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.268458 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/basic_where.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/current_date.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/date.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_newline.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/embedded_quote.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/floating_point.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/function_with_strings.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/quote_in_table_name.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/subplan.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_integer.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_regex_chars.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/where_with_substring.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case1.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case2.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case3.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case4.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case5.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case6.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case7.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case8.query.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.colon_obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.explain.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.obfuscated.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/with_escape_case9.query.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.276458 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_1logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_1core_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_2core_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38341 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/malformed_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.276458 newrelic-8.9.0/tests/cross_agent/fixtures/proc_meminfo/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_meminfo/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_meminfo/malformed_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_client_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_cookie.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.276458 newrelic-8.9.0/tests/cross_agent/fixtures/rum_footer_insertion_location/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_footer_insertion_location/close-body-in-comment.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_footer_insertion_location/dynamic-iframe.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.292459 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/empty_head
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.308460 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.308460 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.312461 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.obfuscated
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/sql_parsing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/transaction_segment_terms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/url_clean.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/url_domain_extraction.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.312461 newrelic-8.9.0/tests/cross_agent/fixtures/utilization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/utilization/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/utilization/boot_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/utilization/utilization_json.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.312461 newrelic-8.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_agent_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_aws_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_azure_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_boot_id_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_cat_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_collector_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_datstore_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_gcp_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_labels_and_rollups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_lambda_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_pcf_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_rum_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_sql_obfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_transaction_segment_terms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_utilization_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/cross_agent/test_w3c_trace_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.316461 newrelic-8.9.0/tests/datastore_aioredis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aioredis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aioredis/test_custom_conn_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aioredis/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aioredis/test_get_and_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aioredis/test_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aioredis/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aioredis/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aioredis/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aioredis/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aioredis/test_uninstrumented_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.316461 newrelic-8.9.0/tests/datastore_aredis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aredis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aredis/test_custom_conn_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aredis/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aredis/test_get_and_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aredis/test_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aredis/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aredis/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aredis/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_aredis/test_uninstrumented_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.316461 newrelic-8.9.0/tests/datastore_asyncpg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_asyncpg/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_asyncpg/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_asyncpg/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.316461 newrelic-8.9.0/tests/datastore_bmemcached/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_bmemcached/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_bmemcached/test_memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.316461 newrelic-8.9.0/tests/datastore_elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_elasticsearch/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_elasticsearch/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_elasticsearch/test_database_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_elasticsearch/test_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_elasticsearch/test_instrumented_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_elasticsearch/test_mget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_elasticsearch/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_elasticsearch/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_elasticsearch/test_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.320461 newrelic-8.9.0/tests/datastore_memcache/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_memcache/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_memcache/test_all_methods_wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_memcache/test_memcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_memcache/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_memcache/test_span_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.320461 newrelic-8.9.0/tests/datastore_mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_mysql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_mysql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.320461 newrelic-8.9.0/tests/datastore_postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_postgresql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_postgresql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.320461 newrelic-8.9.0/tests/datastore_psycopg2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_database_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_explain_plans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_forward_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_obfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_rollback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_slow_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.320461 newrelic-8.9.0/tests/datastore_psycopg2cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2cffi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2cffi/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_psycopg2cffi/test_explain_plans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.320461 newrelic-8.9.0/tests/datastore_pylibmc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pylibmc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pylibmc/test_memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.320461 newrelic-8.9.0/tests/datastore_pymemcache/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pymemcache/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pymemcache/test_memcache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.324462 newrelic-8.9.0/tests/datastore_pymongo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pymongo/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pymongo/test_pymongo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.324462 newrelic-8.9.0/tests/datastore_pymssql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pymssql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pymssql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.324462 newrelic-8.9.0/tests/datastore_pymysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pymysql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pymysql/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.324462 newrelic-8.9.0/tests/datastore_pyodbc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pyodbc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pyodbc/test_pyodbc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.324462 newrelic-8.9.0/tests/datastore_pysolr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pysolr/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_pysolr/test_solr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.324462 newrelic-8.9.0/tests/datastore_redis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_redis/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_redis/test_custom_conn_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_redis/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_redis/test_get_and_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_redis/test_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_redis/test_multiple_dbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_redis/test_rb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_redis/test_span_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_redis/test_trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_redis/test_uninstrumented_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.328462 newrelic-8.9.0/tests/datastore_rediscluster/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_rediscluster/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_rediscluster/test_uninstrumented_rediscluster_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.328462 newrelic-8.9.0/tests/datastore_solrpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_solrpy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_solrpy/test_solr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.328462 newrelic-8.9.0/tests/datastore_sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_sqlite/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_sqlite/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/datastore_sqlite/test_obfuscation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.328462 newrelic-8.9.0/tests/external_boto3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_boto3/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_boto3/test_boto3_iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_boto3/test_boto3_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_boto3/test_boto3_sns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.328462 newrelic-8.9.0/tests/external_botocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_botocore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_botocore/test_botocore_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_botocore/test_botocore_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_botocore/test_botocore_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_botocore/test_botocore_sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.328462 newrelic-8.9.0/tests/external_feedparser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_feedparser/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_feedparser/packages.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_feedparser/test_feedparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.328462 newrelic-8.9.0/tests/external_http/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_http/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_http/test_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.332462 newrelic-8.9.0/tests/external_httplib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_httplib/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_httplib/test_httplib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_httplib/test_urllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_httplib/test_urllib2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.332462 newrelic-8.9.0/tests/external_httplib2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_httplib2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_httplib2/test_httplib2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.332462 newrelic-8.9.0/tests/external_httpx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_httpx/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_httpx/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.332462 newrelic-8.9.0/tests/external_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_requests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_requests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_requests/test_span_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.332462 newrelic-8.9.0/tests/external_urllib3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_urllib3/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/external_urllib3/test_urllib3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.336462 newrelic-8.9.0/tests/framework_aiohttp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_aiohttp/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_aiohttp/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_aiohttp/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_aiohttp/test_client_async_await.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_aiohttp/test_client_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_aiohttp/test_externals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_aiohttp/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_aiohttp/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_aiohttp/test_server_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_aiohttp/test_ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.336462 newrelic-8.9.0/tests/framework_ariadne/
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_ariadne/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_ariadne/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_ariadne/schema.graphql
+-rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_ariadne/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_ariadne/test_application_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_ariadne/test_asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_ariadne/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.336462 newrelic-8.9.0/tests/framework_bottle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_bottle/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_bottle/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_bottle/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.336462 newrelic-8.9.0/tests/framework_cherrypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_cherrypy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_cherrypy/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_cherrypy/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_cherrypy/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_cherrypy/test_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.340463 newrelic-8.9.0/tests/framework_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.340463 newrelic-8.9.0/tests/framework_django/dummy_app/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/dummy_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.340463 newrelic-8.9.0/tests/framework_django/dummy_app/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/dummy_app/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/dummy_app/templatetags/custom_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.340463 newrelic-8.9.0/tests/framework_django/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/templates/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/templates/render_exception.html
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/templates/results.html
+-rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/test_asgi_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_django/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.340463 newrelic-8.9.0/tests/framework_falcon/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_falcon/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_falcon/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_falcon/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.340463 newrelic-8.9.0/tests/framework_fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_fastapi/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_fastapi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_fastapi/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.344463 newrelic-8.9.0/tests/framework_flask/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/_test_application_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/_test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/_test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/_test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/_test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/_test_user_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/_test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/_test_views_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/test_compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/test_user_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_flask/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.344463 newrelic-8.9.0/tests/framework_graphene/
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_graphene/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_graphene/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17853 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_graphene/test_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.348463 newrelic-8.9.0/tests/framework_graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_graphql/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_graphql/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_graphql/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_graphql/test_application_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.348463 newrelic-8.9.0/tests/framework_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_grpc/_test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_grpc/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.348463 newrelic-8.9.0/tests/framework_grpc/sample_application/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_grpc/sample_application/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_grpc/sample_application/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_grpc/sample_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_grpc/sample_application/sample_application.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_grpc/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_grpc/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_grpc/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_grpc/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.348463 newrelic-8.9.0/tests/framework_pyramid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_pyramid/_test_append_slash_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_pyramid/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_pyramid/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_pyramid/test_append_slash_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_pyramid/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_pyramid/test_cornice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.352463 newrelic-8.9.0/tests/framework_sanic/
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_sanic/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_sanic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13507 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_sanic/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_sanic/test_cross_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.352463 newrelic-8.9.0/tests/framework_starlette/
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_starlette/_test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_starlette/_test_bg_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_starlette/_test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_starlette/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_starlette/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_starlette/test_bg_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_starlette/test_graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.352463 newrelic-8.9.0/tests/framework_strawberry/
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_strawberry/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_strawberry/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_strawberry/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_strawberry/test_application_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_strawberry/test_asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.356464 newrelic-8.9.0/tests/framework_tornado/
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_tornado/_target_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_tornado/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_tornado/test_custom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_tornado/test_externals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_tornado/test_inbound_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/framework_tornado/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.356464 newrelic-8.9.0/tests/logger_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/logger_logging/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/logger_logging/test_local_decorating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/logger_logging/test_log_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/logger_logging/test_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/logger_logging/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/logger_logging/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.356464 newrelic-8.9.0/tests/logger_loguru/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/logger_loguru/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/logger_loguru/test_local_decorating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/logger_loguru/test_log_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/logger_loguru/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/logger_loguru/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/logger_loguru/test_stack_inspection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.356464 newrelic-8.9.0/tests/messagebroker_confluentkafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_confluentkafka/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_confluentkafka/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_confluentkafka/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_confluentkafka/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.360464 newrelic-8.9.0/tests/messagebroker_kafkapython/
+-rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_kafkapython/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_kafkapython/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_kafkapython/test_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_kafkapython/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_kafkapython/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.360464 newrelic-8.9.0/tests/messagebroker_pika/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_pika/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_pika/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_pika/minversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_pika/test_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_pika/test_distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_pika/test_memory_leak.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_pika/test_pika_async_connection_consume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_pika/test_pika_blocking_connection_consume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_pika/test_pika_produce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/messagebroker_pika/test_pika_supportability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.364464 newrelic-8.9.0/tests/template_genshi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/template_genshi/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/template_genshi/test_genshi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.364464 newrelic-8.9.0/tests/template_jinja2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/template_jinja2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/template_jinja2/test_jinja2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.364464 newrelic-8.9.0/tests/template_mako/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/template_mako/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/template_mako/test_mako.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.364464 newrelic-8.9.0/tests/testing_support/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/asgi_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/db_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/external_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.364464 newrelic-8.9.0/tests/testing_support/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/fixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/fixture/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50495 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/mock_external_grpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/mock_external_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/mock_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/sample_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/sample_asgi_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:42:28.376465 newrelic-8.9.0/tests/testing_support/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_apdex_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_application_error_event_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_application_error_trace_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_application_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_browser_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_code_level_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_cross_process_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_custom_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_custom_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_database_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_database_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_database_trace_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_datastore_trace_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_distributed_trace_accepted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_distributed_tracing_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_error_event_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_error_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_error_trace_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_error_trace_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_external_node_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_function_called.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_internal_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_log_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_log_event_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_log_event_count_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_log_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_log_events_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_messagebroker_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_metric_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_non_transaction_error_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_outbound_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_serverless_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_serverless_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_serverless_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_slow_sql_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_span_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_sql_obfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_synthetics_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_synthetics_transaction_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_time_metrics_outside_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_transaction_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_transaction_error_trace_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_transaction_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_transaction_event_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_transaction_event_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_transaction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_transaction_slow_sql_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_transaction_trace_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_tt_collector_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_tt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-27 21:42:09.000000 newrelic-8.9.0/tests/testing_support/validators/validate_tt_segment_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26636 2023-07-27 21:42:09.000000 newrelic-8.9.0/tox.ini
```

### Comparing `newrelic-8.8.1/.devcontainer/devcontainer.json` & `newrelic-8.9.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/.github/ISSUE_TEMPLATE/bug_report.md` & `newrelic-8.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/.github/ISSUE_TEMPLATE/config.yml` & `newrelic-8.9.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `newrelic-8.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/.github/containers/Dockerfile` & `newrelic-8.9.0/.github/containers/Dockerfile`

 * *Files 10% similar despite different names*

```diff
@@ -19,20 +19,23 @@
 RUN export DEBIAN_FRONTEND=noninteractive && \
     apt-get update && \
     apt-get install -y \
         bash \
         build-essential \
         curl \
         expat \
+        freetds-common \
+        freetds-dev \
         gcc \
         git \
         libbz2-dev \
         libcurl4-openssl-dev \
         libffi-dev \
         libgmp-dev \
+        libkrb5-dev \
         liblzma-dev \
         libmpfr-dev \
         libncurses-dev \
         libpq-dev \
         libreadline-dev \
         libsqlite3-dev \
         libssl-dev \
@@ -48,18 +51,30 @@
         unzip \
         wget \
         zip \
         zlib1g \
         zlib1g-dev && \
     rm -rf /var/lib/apt/lists/*
 
+# Build librdkafka from source
+ARG LIBRDKAFKA_VERSION=2.1.1
+RUN cd /tmp && \
+    wget https://github.com/confluentinc/librdkafka/archive/refs/tags/v${LIBRDKAFKA_VERSION}.zip -O ./librdkafka.zip && \
+    unzip ./librdkafka.zip && \
+    rm ./librdkafka.zip && \
+    cd ./librdkafka-${LIBRDKAFKA_VERSION} && \
+    ./configure && \
+    make all install && \
+    cd /tmp && \
+    rm -rf ./librdkafka-${LIBRDKAFKA_VERSION}
+
 # Setup ODBC config
-RUN sed -i 's/Driver=psqlodbca.so/Driver=\/usr\/lib\/x86_64-linux-gnu\/odbc\/psqlodbca.so/g' /etc/odbcinst.ini && \
-    sed -i 's/Driver=psqlodbcw.so/Driver=\/usr\/lib\/x86_64-linux-gnu\/odbc\/psqlodbcw.so/g' /etc/odbcinst.ini && \
-    sed -i 's/Setup=libodbcpsqlS.so/Setup=\/usr\/lib\/x86_64-linux-gnu\/odbc\/libodbcpsqlS.so/g' /etc/odbcinst.ini
+RUN sed -i 's|Driver=psqlodbca.so|Driver=/usr/lib/x86_64-linux-gnu/odbc/psqlodbca.so|g' /etc/odbcinst.ini && \
+    sed -i 's|Driver=psqlodbcw.so|Driver=/usr/lib/x86_64-linux-gnu/odbc/psqlodbcw.so|g' /etc/odbcinst.ini && \
+    sed -i 's|Setup=libodbcpsqlS.so|Setup=/usr/lib/x86_64-linux-gnu/odbc/libodbcpsqlS.so|g' /etc/odbcinst.ini
 
 # Set the locale
 RUN locale-gen --no-purge en_US.UTF-8
 ENV LANG=en_US.UTF-8 \ LANGUAGE=en_US:en \ LC_ALL=en_US.UTF-8
 ENV TZ="Etc/UTC"
 RUN ln -fs "/usr/share/zoneinfo/${TZ}" /etc/localtime && \
     dpkg-reconfigure -f noninteractive tzdata
@@ -72,12 +87,12 @@
 ENV PYENV_ROOT="${HOME}/.pyenv"
 RUN curl https://pyenv.run/ | /bin/bash
 ENV PATH="$PYENV_ROOT/bin:$PYENV_ROOT/shims:${PATH}"
 RUN echo 'eval "$(pyenv init -)"' >>$HOME/.bashrc && \
     pyenv update
 
 # Install Python
-ARG PYTHON_VERSIONS="3.10 3.9 3.8 3.7 3.11 2.7 pypy2.7-7.3.11 pypy3.7"
+ARG PYTHON_VERSIONS="3.10 3.9 3.8 3.7 3.11 2.7 pypy2.7-7.3.12 pypy3.8-7.3.11"
 COPY --chown=1000:1000 --chmod=+x ./install-python.sh /tmp/install-python.sh
 COPY ./requirements.txt /requirements.txt
 RUN /tmp/install-python.sh && \
     rm /tmp/install-python.sh
```

### Comparing `newrelic-8.8.1/.github/containers/Makefile` & `newrelic-8.9.0/.github/containers/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
 .PHONY: default
 default: test
 
 .PHONY: build
 build:
 	@# Perform a shortened build for testing
-	@docker build --build-arg='PYTHON_VERSIONS=3.10 2.7' $(MAKEFILE_DIR) -t ghcr.io/newrelic/newrelic-python-agent-ci:local
+	@docker build $(MAKEFILE_DIR) \
+		-t ghcr.io/newrelic/newrelic-python-agent-ci:local \
+		--build-arg='PYTHON_VERSIONS=3.10 2.7'
 
 .PHONY: test
 test: build
 	@# Ensure python versions are usable
 	@docker run --rm ghcr.io/newrelic/python-agent-ci:local /bin/bash -c '\
 		python3.10 --version && \
 		python2.7 --version && \
@@ -34,11 +36,13 @@
 		echo "Success! Python versions installed."'
 
 .PHONY: run
 run: build
 	@docker run --rm -it \
 		--mount type=bind,source="$(REPO_ROOT)",target=/home/github/python-agent \
 		--workdir=/home/github/python-agent \
+		--add-host=host.docker.internal:host-gateway \
 		-e NEW_RELIC_HOST="${NEW_RELIC_HOST}" \
 		-e NEW_RELIC_LICENSE_KEY="${NEW_RELIC_LICENSE_KEY}" \
 		-e NEW_RELIC_DEVELOPER_MODE="${NEW_RELIC_DEVELOPER_MODE}" \
+		-e GITHUB_ACTIONS="true" \
 		ghcr.io/newrelic/newrelic-python-agent-ci:local /bin/bash
```

### Comparing `newrelic-8.8.1/.github/containers/install-python.sh` & `newrelic-8.9.0/.github/containers/install-python.sh`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-set -e
-
-SCRIPT_DIR=$(dirname "$0")
-PIP_REQUIREMENTS=$(cat /requirements.txt)
+set -eo pipefail
 
 main() {
     # Coerce space separated string to array
     if [[ ${#PYTHON_VERSIONS[@]} -eq 1 ]]; then
         PYTHON_VERSIONS=($PYTHON_VERSIONS)
     fi
 
@@ -46,11 +43,11 @@
     done
     wait
 
     # Set all installed versions as globally accessible
     pyenv global ${PYENV_VERSIONS[@]}
     
     # Install dependencies for main python installation
-    pyenv exec pip install --upgrade $PIP_REQUIREMENTS
+    pyenv exec pip install --upgrade -r /requirements.txt
 }
 
 main
```

### Comparing `newrelic-8.8.1/.github/mergify.yml` & `newrelic-8.9.0/.github/mergify.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/.github/pull_request_template.md` & `newrelic-8.9.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/.github/scripts/retry.sh` & `newrelic-8.9.0/.github/scripts/retry.sh`

 * *Files 9% similar despite different names*

```diff
@@ -35,8 +35,8 @@
     
     # Run wrapped command, and exit on success
     $@ && break
     result=$?
 done
 
 # Exit with status code of wrapped command
-exit $?
+exit $result
```

### Comparing `newrelic-8.8.1/.github/stale.yml` & `newrelic-8.9.0/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/.github/workflows/build-ci-image.yml` & `newrelic-8.9.0/.github/workflows/build-ci-image.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/.github/workflows/deploy-python.yml` & `newrelic-8.9.0/.github/workflows/deploy-python.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/.github/workflows/get-envs.py` & `newrelic-8.9.0/.github/workflows/get-envs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/.github/workflows/mega-linter.yml` & `newrelic-8.9.0/.github/workflows/mega-linter.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/.github/workflows/tests.yml` & `newrelic-8.9.0/.github/workflows/tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -34,21 +34,23 @@
     runs-on: ubuntu-20.04
     needs:
       - python
       - elasticsearchserver07
       - elasticsearchserver08
       - gearman
       - grpc
-      #- kafka
+      - kafka
       - memcached
       - mongodb
+      - mssql
       - mysql
       - postgres
       - rabbitmq
       - redis
+      - rediscluster
       - solr
 
     steps:
       - name: Success
         run: echo "Success!"
 
   # Combine and upload coverage data
@@ -114,15 +116,15 @@
             18,
             19,
             20,
           ]
 
     runs-on: ubuntu-20.04
     container:
-      image: ghcr.io/${{ github.repository }}-ci:latest
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     steps:
       - uses: actions/checkout@v3
 
@@ -159,15 +161,15 @@
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
     container:
-      image: ghcr.io/${{ github.repository }}-ci:latest
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     steps:
       - uses: actions/checkout@v3
 
@@ -204,15 +206,15 @@
     strategy:
       fail-fast: false
       matrix:
         group-number: [1, 2]
 
     runs-on: ubuntu-20.04
     container:
-      image: ghcr.io/${{ github.repository }}-ci:latest
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       postgres:
         image: postgres:9
@@ -253,26 +255,89 @@
       - name: Upload Coverage Artifacts
         uses: actions/upload-artifact@v3
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
+  mssql:
+    env:
+      TOTAL_GROUPS: 1
+
+    strategy:
+      fail-fast: false
+      matrix:
+        group-number: [1]
+
+    runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
+    timeout-minutes: 30
+
+    services:
+      mssql:
+        image: mcr.microsoft.com/azure-sql-edge:latest
+        env:
+          MSSQL_USER: python_agent
+          MSSQL_PASSWORD: python_agent
+          MSSQL_SA_PASSWORD: "python_agent#1234"
+          ACCEPT_EULA: "Y"
+        ports:
+          - 8080:1433
+          - 8081:1433
+        # Set health checks to wait until mysql has started
+        options: >-
+          --health-cmd "/opt/mssql-tools/bin/sqlcmd -U SA -P $MSSQL_SA_PASSWORD -Q 'SELECT 1'"
+          --health-interval 10s
+          --health-timeout 5s
+          --health-retries 5
+
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
+
+      - name: Get Environments
+        id: get-envs
+        run: |
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
+        env:
+          GROUP_NUMBER: ${{ matrix.group-number }}
+
+      - name: Test
+        run: |
+          tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
+        env:
+          TOX_PARALLEL_NO_SPINNER: 1
+          PY_COLORS: 0
+
+      - name: Upload Coverage Artifacts
+        uses: actions/upload-artifact@v3
+        with:
+          name: coverage-${{ github.job }}-${{ strategy.job-index }}
+          path: ./**/.coverage.*
+          retention-days: 1
+
   mysql:
     env:
       TOTAL_GROUPS: 2
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1, 2]
 
     runs-on: ubuntu-20.04
     container:
-      image: ghcr.io/${{ github.repository }}-ci:latest
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       mysql:
         image: mysql:5.6
@@ -316,26 +381,125 @@
       - name: Upload Coverage Artifacts
         uses: actions/upload-artifact@v3
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
+  rediscluster:
+    env:
+      TOTAL_GROUPS: 1
+
+    strategy:
+      fail-fast: false
+      matrix:
+        group-number: [1]
+
+    runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
+    timeout-minutes: 30
+
+    services:
+      redis1:
+        image: hmstepanek/redis-cluster-node:1.0.0
+        ports:
+          - 6379:6379
+          - 16379:16379
+        options: >-
+          --add-host=host.docker.internal:host-gateway
+
+      redis2:
+        image: hmstepanek/redis-cluster-node:1.0.0
+        ports:
+          - 6380:6379
+          - 16380:16379
+        options: >-
+          --add-host=host.docker.internal:host-gateway
+
+      redis3:
+        image: hmstepanek/redis-cluster-node:1.0.0
+        ports:
+          - 6381:6379
+          - 16381:16379
+        options: >-
+          --add-host=host.docker.internal:host-gateway
+
+      redis4:
+        image: hmstepanek/redis-cluster-node:1.0.0
+        ports:
+          - 6382:6379
+          - 16382:16379
+        options: >-
+          --add-host=host.docker.internal:host-gateway
+
+      redis5:
+        image: hmstepanek/redis-cluster-node:1.0.0
+        ports:
+          - 6383:6379
+          - 16383:16379
+        options: >-
+          --add-host=host.docker.internal:host-gateway
+
+      redis6:
+        image: hmstepanek/redis-cluster-node:1.0.0
+        ports:
+          - 6384:6379
+          - 16384:16379
+        options: >-
+          --add-host=host.docker.internal:host-gateway
+
+      cluster-setup:
+        image: hmstepanek/redis-cluster:1.0.0    
+        options: >-
+          --add-host=host.docker.internal:host-gateway
+
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
+
+      - name: Get Environments
+        id: get-envs
+        run: |
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
+        env:
+          GROUP_NUMBER: ${{ matrix.group-number }}
+
+      - name: Test
+        run: |
+          tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
+        env:
+          TOX_PARALLEL_NO_SPINNER: 1
+          PY_COLORS: 0
+
+      - name: Upload Coverage Artifacts
+        uses: actions/upload-artifact@v3
+        with:
+          name: coverage-${{ github.job }}-${{ strategy.job-index }}
+          path: ./**/.coverage.*
+          retention-days: 1
+
   redis:
     env:
       TOTAL_GROUPS: 2
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1, 2]
 
     runs-on: ubuntu-20.04
     container:
-      image: ghcr.io/${{ github.repository }}-ci:latest
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       redis:
         image: redis
@@ -385,15 +549,15 @@
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
     container:
-      image: ghcr.io/${{ github.repository }}-ci:latest
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       solr:
         image: bitnami/solr:8.8.2
@@ -445,15 +609,15 @@
     strategy:
       fail-fast: false
       matrix:
         group-number: [1, 2]
 
     runs-on: ubuntu-20.04
     container:
-      image: ghcr.io/${{ github.repository }}-ci:latest
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       memcached:
         image: memcached
@@ -503,15 +667,15 @@
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
     container:
-      image: ghcr.io/${{ github.repository }}-ci:latest
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       rabbitmq:
         image: rabbitmq
@@ -551,106 +715,96 @@
       - name: Upload Coverage Artifacts
         uses: actions/upload-artifact@v3
         with:
           name: coverage-${{ github.job }}-${{ strategy.job-index }}
           path: ./**/.coverage.*
           retention-days: 1
 
-  # kafka:
-  #   env:
-  #     TOTAL_GROUPS: 4
-
-  #   strategy:
-  #     fail-fast: false
-  #     matrix:
-  #       group-number: [1, 2, 3, 4]
-
-  #   runs-on: ubuntu-20.04
-  #   container:
-  #     image: ghcr.io/${{ github.repository }}-ci:latest
-  #     options: >-
-  #       --add-host=host.docker.internal:host-gateway
-  #   timeout-minutes: 30
-
-  #   services:
-  #     zookeeper:
-  #       image: bitnami/zookeeper:3.7
-  #       env:
-  #         ALLOW_ANONYMOUS_LOGIN: yes
-
-  #       ports:
-  #         - 2181:2181
-
-  #     kafka:
-  #       image: bitnami/kafka:3.2
-  #       ports:
-  #         - 8080:8080
-  #         - 8081:8081
-  #       env:
-  #         ALLOW_PLAINTEXT_LISTENER: yes
-  #         KAFKA_ZOOKEEPER_CONNECT: zookeeper:2181
-  #         KAFKA_CFG_AUTO_CREATE_TOPICS_ENABLE: true
-  #         KAFKA_CFG_LISTENERS: L1://:8080,L2://:8081
-  #         KAFKA_CFG_ADVERTISED_LISTENERS: L1://127.0.0.1:8080,L2://kafka:8081,
-  #         KAFKA_CFG_LISTENER_SECURITY_PROTOCOL_MAP: L1:PLAINTEXT,L2:PLAINTEXT
-  #         KAFKA_CFG_INTER_BROKER_LISTENER_NAME: L2
-
-  #   steps:
-  #     - uses: actions/checkout@v3
-
-  #     - name: Fetch git tags
-  #       run: |
-  #         git config --global --add safe.directory "$GITHUB_WORKSPACE"
-  #         git fetch --tags origin
-
-  #     # Special case packages
-  #     - name: Install librdkafka-dev
-  #       run: |
-  #         # Use lsb-release to find the codename of Ubuntu to use to install the correct library name
-  #         sudo apt-get update
-  #         sudo ln -fs /usr/share/zoneinfo/America/Los_Angeles /etc/localtime
-  #         sudo apt-get install -y wget gnupg2 software-properties-common
-  #         sudo wget -qO - https://packages.confluent.io/deb/7.2/archive.key | sudo apt-key add -
-  #         sudo add-apt-repository "deb https://packages.confluent.io/clients/deb $(lsb_release -cs) main"
-  #         sudo apt-get update
-  #         sudo apt-get install -y librdkafka-dev/$(lsb_release -c | cut -f 2)
-
-  #     - name: Get Environments
-  #       id: get-envs
-  #       run: |
-  #         echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
-  #       env:
-  #         GROUP_NUMBER: ${{ matrix.group-number }}
-
-  #     - name: Test
-  #       run: |
-  #         tox -vv -e ${{ steps.get-envs.outputs.envs }}
-  #       env:
-  #         TOX_PARALLEL_NO_SPINNER: 1
-  #         PY_COLORS: 0
-
-  #     - name: Upload Coverage Artifacts
-  #       uses: actions/upload-artifact@v3
-  #       with:
-  #         name: coverage-${{ github.job }}-${{ strategy.job-index }}
-  #         path: ./**/.coverage.*
-  #         retention-days: 1
+  kafka:
+    env:
+      TOTAL_GROUPS: 4
+
+    strategy:
+      fail-fast: false
+      matrix:
+        group-number: [1, 2, 3, 4]
+
+    runs-on: ubuntu-20.04
+    container:
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
+      options: >-
+        --add-host=host.docker.internal:host-gateway
+    timeout-minutes: 30
+
+    services:
+      zookeeper:
+        image: bitnami/zookeeper:3.7
+        env:
+          ALLOW_ANONYMOUS_LOGIN: yes
+
+        ports:
+          - 2181:2181
+
+      kafka:
+        image: bitnami/kafka:3.2
+        ports:
+          - 8080:8080
+          - 8082:8082
+          - 8083:8083
+        env:
+          KAFKA_ENABLE_KRAFT: no
+          ALLOW_PLAINTEXT_LISTENER: yes
+          KAFKA_ZOOKEEPER_CONNECT: zookeeper:2181
+          KAFKA_CFG_AUTO_CREATE_TOPICS_ENABLE: true
+          KAFKA_CFG_LISTENERS: L1://:8082,L2://:8083,L3://:8080
+          KAFKA_CFG_ADVERTISED_LISTENERS: L1://host.docker.internal:8082,L2://host.docker.internal:8083,L3://kafka:8080
+          KAFKA_CFG_LISTENER_SECURITY_PROTOCOL_MAP: L1:PLAINTEXT,L2:PLAINTEXT,L3:PLAINTEXT
+          KAFKA_CFG_INTER_BROKER_LISTENER_NAME: L3
+
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: Fetch git tags
+        run: |
+          git config --global --add safe.directory "$GITHUB_WORKSPACE"
+          git fetch --tags origin
+
+      - name: Get Environments
+        id: get-envs
+        run: |
+          echo "envs=$(tox -l | grep '^${{ github.job }}\-' | ./.github/workflows/get-envs.py)" >> $GITHUB_OUTPUT
+        env:
+          GROUP_NUMBER: ${{ matrix.group-number }}
+
+      - name: Test
+        run: |
+          tox -vv -e ${{ steps.get-envs.outputs.envs }} -p auto
+        env:
+          TOX_PARALLEL_NO_SPINNER: 1
+          PY_COLORS: 0
+
+      - name: Upload Coverage Artifacts
+        uses: actions/upload-artifact@v3
+        with:
+          name: coverage-${{ github.job }}-${{ strategy.job-index }}
+          path: ./**/.coverage.*
+          retention-days: 1
 
   mongodb:
     env:
       TOTAL_GROUPS: 1
 
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
     container:
-      image: ghcr.io/${{ github.repository }}-ci:latest
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       mongodb:
         image: mongo:3.6.4
@@ -700,15 +854,15 @@
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
     container:
-      image: ghcr.io/${{ github.repository }}-ci:latest
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       elasticsearch:
         image: elasticsearch:7.17.8
@@ -760,15 +914,15 @@
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
     container:
-      image: ghcr.io/${{ github.repository }}-ci:latest
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       elasticsearch:
         image: elasticsearch:8.6.0
@@ -821,15 +975,15 @@
     strategy:
       fail-fast: false
       matrix:
         group-number: [1]
 
     runs-on: ubuntu-20.04
     container:
-      image: ghcr.io/${{ github.repository }}-ci:latest
+      image: ghcr.io/newrelic/newrelic-python-agent-ci:latest
       options: >-
         --add-host=host.docker.internal:host-gateway
     timeout-minutes: 30
 
     services:
       gearman:
         image: artefactual/gearmand
```

### Comparing `newrelic-8.8.1/.gitignore` & `newrelic-8.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/.mega-linter.yml` & `newrelic-8.9.0/.mega-linter.yml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/CONTRIBUTING.rst` & `newrelic-8.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/LICENSE` & `newrelic-8.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/PKG-INFO` & `newrelic-8.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic
-Version: 8.8.1
+Version: 8.9.0
 Summary: New Relic Python Agent
 Home-page: https://docs.newrelic.com/docs/apm/agents/python-agent/
 Author: New Relic
 Author-email: support@newrelic.com
 Maintainer: New Relic
 Maintainer-email: support@newrelic.com
 License: Apache-2.0
```

### Comparing `newrelic-8.8.1/README.rst` & `newrelic-8.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/ROADMAP.md` & `newrelic-8.9.0/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/THIRD_PARTY_NOTICES.md` & `newrelic-8.9.0/THIRD_PARTY_NOTICES.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/codecov.yml` & `newrelic-8.9.0/codecov.yml`

 * *Files 17% similar despite different names*

```diff
@@ -15,10 +15,9 @@
   - "newrelic/hooks/framework_web2py.py"
   - "newrelic/hooks/middleware_weberror.py"
   - "newrelic/hooks/framework_webpy.py"
   - "newrelic/hooks/datastore_motor.py"
   - "newrelic/hooks/database_oursql.py"
   - "newrelic/hooks/database_psycopg2ct.py"
   - "newrelic/hooks/datastore_umemcache.py"
-  # Temporarily disable kafka
-  - "newrelic/hooks/messagebroker_kafkapython.py"
-  - "newrelic/hooks/messagebroker_confluentkafka.py"
+  - "newrelic/admin/*"
+  - "newrelic/console.py"
```

### Comparing `newrelic-8.8.1/newrelic/__init__.py` & `newrelic-8.9.0/newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/admin/__init__.py` & `newrelic-8.9.0/newrelic/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/admin/__main__.py` & `newrelic-8.9.0/newrelic/admin/__main__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/admin/debug_console.py` & `newrelic-8.9.0/newrelic/admin/debug_console.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/admin/generate_config.py` & `newrelic-8.9.0/newrelic/admin/generate_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/admin/license_key.py` & `newrelic-8.9.0/newrelic/admin/license_key.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/admin/local_config.py` & `newrelic-8.9.0/newrelic/admin/local_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/admin/network_config.py` & `newrelic-8.9.0/newrelic/admin/network_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/admin/record_deploy.py` & `newrelic-8.9.0/newrelic/admin/record_deploy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/admin/run_program.py` & `newrelic-8.9.0/newrelic/admin/run_program.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/admin/run_python.py` & `newrelic-8.9.0/newrelic/admin/run_python.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/admin/server_config.py` & `newrelic-8.9.0/newrelic/admin/server_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/admin/validate_config.py` & `newrelic-8.9.0/newrelic/admin/validate_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/agent.py` & `newrelic-8.9.0/newrelic/agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/__init__.py` & `newrelic-8.9.0/newrelic/api/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/application.py` & `newrelic-8.9.0/newrelic/api/application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/asgi_application.py` & `newrelic-8.9.0/newrelic/api/asgi_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/background_task.py` & `newrelic-8.9.0/newrelic/api/background_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,27 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import functools
-import sys
 
 from newrelic.api.application import Application, application_instance
 from newrelic.api.transaction import Transaction, current_transaction
-from newrelic.common.async_proxy import async_proxy, TransactionContext
+from newrelic.common.async_proxy import TransactionContext, async_proxy
 from newrelic.common.object_names import callable_name
 from newrelic.common.object_wrapper import FunctionWrapper, wrap_object
 
 
 class BackgroundTask(Transaction):
-
     def __init__(self, application, name, group=None, source=None):
-
         # Initialise the common transaction base class.
 
         super(BackgroundTask, self).__init__(application, source=source)
 
         # Mark this as a background task even if disabled.
 
         self.background_task = True
@@ -49,15 +46,14 @@
 
         # Name the web transaction from supplied values.
 
         self.set_transaction_name(name, group, priority=1)
 
 
 def BackgroundTaskWrapper(wrapped, application=None, name=None, group=None):
-
     def wrapper(wrapped, instance, args, kwargs):
         if callable(name):
             if instance is not None:
                 _name = name(instance, *args, **kwargs)
             else:
                 _name = name(*args, **kwargs)
 
@@ -103,43 +99,23 @@
 
         if proxy:
             context_manager = TransactionContext(create_transaction)
             return proxy(wrapped(*args, **kwargs), context_manager)
 
         manager = create_transaction(current_transaction(active_only=False))
 
+        # This means that a transaction already exists, so we want to return
         if not manager:
             return wrapped(*args, **kwargs)
-        success = True
 
-        try:
-            manager.__enter__()
-            try:
-                return wrapped(*args, **kwargs)
-            except:
-                success = False
-                if not manager.__exit__(*sys.exc_info()):
-                    raise
-        finally:
-            if success and manager._ref_count == 0:
-                manager._is_finalized = True
-                manager.__exit__(None, None, None)
-            else:
-                manager._request_handler_finalize = True
-                manager._server_adapter_finalize = True
-
-                old_transaction = current_transaction()
-                if old_transaction is not None:
-                    old_transaction.drop_transaction()
+        with manager:
+            return wrapped(*args, **kwargs)
 
     return FunctionWrapper(wrapped, wrapper)
 
 
 def background_task(application=None, name=None, group=None):
-    return functools.partial(BackgroundTaskWrapper,
-            application=application, name=name, group=group)
+    return functools.partial(BackgroundTaskWrapper, application=application, name=name, group=group)
 
 
-def wrap_background_task(module, object_path, application=None,
-        name=None, group=None):
-    wrap_object(module, object_path, BackgroundTaskWrapper,
-            (application, name, group))
+def wrap_background_task(module, object_path, application=None, name=None, group=None):
+    wrap_object(module, object_path, BackgroundTaskWrapper, (application, name, group))
```

### Comparing `newrelic-8.8.1/newrelic/api/cat_header_mixin.py` & `newrelic-8.9.0/newrelic/api/cat_header_mixin.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/database_trace.py` & `newrelic-8.9.0/newrelic/api/database_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/datastore_trace.py` & `newrelic-8.9.0/newrelic/api/datastore_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/error_trace.py` & `newrelic-8.9.0/newrelic/api/error_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/exceptions.py` & `newrelic-8.9.0/newrelic/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/external_trace.py` & `newrelic-8.9.0/newrelic/api/external_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/function_profile.py` & `newrelic-8.9.0/newrelic/api/function_profile.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/function_trace.py` & `newrelic-8.9.0/newrelic/api/function_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/generator_trace.py` & `newrelic-8.9.0/newrelic/api/generator_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/graphql_trace.py` & `newrelic-8.9.0/newrelic/api/graphql_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/html_insertion.py` & `newrelic-8.9.0/newrelic/api/html_insertion.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/import_hook.py` & `newrelic-8.9.0/newrelic/api/import_hook.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/in_function.py` & `newrelic-8.9.0/newrelic/api/in_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/lambda_handler.py` & `newrelic-8.9.0/newrelic/api/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/log.py` & `newrelic-8.9.0/newrelic/api/log.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/memcache_trace.py` & `newrelic-8.9.0/newrelic/api/memcache_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/message_trace.py` & `newrelic-8.9.0/newrelic/api/message_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/message_transaction.py` & `newrelic-8.9.0/newrelic/api/message_transaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import functools
-import sys
 
 from newrelic.api.application import Application, application_instance
 from newrelic.api.background_task import BackgroundTask
 from newrelic.api.message_trace import MessageTrace
 from newrelic.api.transaction import current_transaction
 from newrelic.common.async_proxy import TransactionContext, async_proxy
 from newrelic.common.object_wrapper import FunctionWrapper, wrap_object
@@ -35,15 +34,14 @@
         headers=None,
         queue_name=None,
         reply_to=None,
         correlation_id=None,
         transport_type="AMQP",
         source=None,
     ):
-
         name, group = self.get_transaction_name(library, destination_type, destination_name)
 
         super(MessageTransaction, self).__init__(application, name, group=group, source=source)
 
         self.headers = headers
 
         if headers is not None and self.settings is not None:
@@ -214,38 +212,20 @@
         proxy = async_proxy(wrapped)
         if proxy:
             context_manager = TransactionContext(create_transaction)
             return proxy(wrapped(*args, **kwargs), context_manager)
 
         manager = create_transaction(current_transaction(active_only=False))
 
+        # This means that transaction already exists and we want to return
         if not manager:
             return wrapped(*args, **kwargs)
 
-        success = True
-
-        try:
-            manager.__enter__()
-            try:
-                return wrapped(*args, **kwargs)
-            except:  # Catch all
-                success = False
-                if not manager.__exit__(*sys.exc_info()):
-                    raise
-        finally:
-            if success and manager._ref_count == 0:
-                manager._is_finalized = True
-                manager.__exit__(None, None, None)
-            else:
-                manager._request_handler_finalize = True
-                manager._server_adapter_finalize = True
-
-                old_transaction = current_transaction()
-                if old_transaction is not None:
-                    old_transaction.drop_transaction()
+        with manager:
+            return wrapped(*args, **kwargs)
 
     return FunctionWrapper(wrapped, wrapper)
 
 
 def message_transaction(
     library,
     destination_type,
```

### Comparing `newrelic-8.8.1/newrelic/api/object_wrapper.py` & `newrelic-8.9.0/newrelic/api/object_wrapper.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/out_function.py` & `newrelic-8.9.0/newrelic/api/out_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/post_function.py` & `newrelic-8.9.0/newrelic/api/post_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/pre_function.py` & `newrelic-8.9.0/newrelic/api/pre_function.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/profile_trace.py` & `newrelic-8.9.0/newrelic/api/profile_trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,52 +9,47 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import functools
-import sys
 import os
+import sys
 
-from newrelic.packages import six
-
-from newrelic.api.time_trace import current_trace
+from newrelic import __file__ as AGENT_PACKAGE_FILE
 from newrelic.api.function_trace import FunctionTrace
-from newrelic.common.object_wrapper import FunctionWrapper, wrap_object
+from newrelic.api.time_trace import current_trace
 from newrelic.common.object_names import callable_name
+from newrelic.common.object_wrapper import FunctionWrapper, wrap_object
+from newrelic.packages import six
 
-from newrelic import __file__ as AGENT_PACKAGE_FILE
-AGENT_PACKAGE_DIRECTORY = os.path.dirname(AGENT_PACKAGE_FILE) + '/'
+AGENT_PACKAGE_DIRECTORY = os.path.dirname(AGENT_PACKAGE_FILE) + "/"
 
 
 class ProfileTrace(object):
-
     def __init__(self, depth):
         self.function_traces = []
         self.maximum_depth = depth
         self.current_depth = 0
 
-    def __call__(self, frame, event, arg):
-
-        if event not in ['call', 'c_call', 'return', 'c_return',
-                'exception', 'c_exception']:
+    def __call__(self, frame, event, arg):  # pragma: no cover
+        if event not in ["call", "c_call", "return", "c_return", "exception", "c_exception"]:
             return
 
         parent = current_trace()
 
         if not parent:
             return
 
         # Not sure if setprofile() is reliable in the face of
         # coroutine systems based on greenlets so don't run
         # if we detect may be using greenlets.
 
-        if (hasattr(sys, '_current_frames') and
-                parent.thread_id not in sys._current_frames()):
+        if hasattr(sys, "_current_frames") and parent.thread_id not in sys._current_frames():
             return
 
         co = frame.f_code
         func_name = co.co_name
         func_line_no = frame.f_lineno
         func_filename = co.co_filename
         func = None  # Populate later
@@ -80,15 +75,15 @@
                 try:
                     if obj.__dict__[func_name].func_code is co:
                         return obj.__dict__[func_name]
 
                 except Exception:
                     pass
 
-        if event in ['call', 'c_call']:
+        if event in ["call", "c_call"]:
             # Skip the outermost as we catch that with the root
             # function traces for the profile trace.
 
             if len(self.function_traces) == 0:
                 self.function_traces.append(None)
                 return
 
@@ -96,42 +91,40 @@
                 self.function_traces.append(None)
                 return
 
             if func_filename.startswith(AGENT_PACKAGE_DIRECTORY):
                 self.function_traces.append(None)
                 return
 
-            if event == 'call':
+            if event == "call":
                 func = _callable()
                 if func:
                     name = callable_name(func)
                 else:
-                    name = '%s:%s#%s' % (func_filename, func_name,
-                            func_line_no)
+                    name = "%s:%s#%s" % (func_filename, func_name, func_line_no)
             else:
                 func = arg
                 name = callable_name(arg)
                 if not name:
-                    name = '%s:@%s#%s' % (func_filename, func_name,
-                            func_line_no)
+                    name = "%s:@%s#%s" % (func_filename, func_name, func_line_no)
 
             function_trace = FunctionTrace(name=name, parent=parent)
             function_trace.__enter__()
 
             # Attempt to add source code context for function
             try:
                 if func:
                     function_trace.add_code_level_metrics(func)
             except Exception:
                 pass
 
             self.function_traces.append(function_trace)
             self.current_depth += 1
 
-        elif event in ['return', 'c_return', 'c_exception']:
+        elif event in ["return", "c_return", "c_exception"]:
             if not self.function_traces:
                 return
 
             try:
                 function_trace = self.function_traces.pop()
 
             except IndexError:
@@ -139,17 +132,15 @@
 
             else:
                 if function_trace:
                     function_trace.__exit__(None, None, None)
                     self.current_depth -= 1
 
 
-def ProfileTraceWrapper(wrapped, name=None, group=None, label=None,
-        params=None, depth=3):
-
+def ProfileTraceWrapper(wrapped, name=None, group=None, label=None, params=None, depth=3):
     def wrapper(wrapped, instance, args, kwargs):
         parent = current_trace()
 
         if parent is None:
             return wrapped(*args, **kwargs)
 
         if callable(name):
@@ -188,15 +179,15 @@
             else:
                 _params = params(*args, **kwargs)
 
         else:
             _params = params
 
         with FunctionTrace(_name, _group, _label, _params, parent=parent, source=wrapped):
-            if not hasattr(sys, 'getprofile'):
+            if not hasattr(sys, "getprofile"):
                 return wrapped(*args, **kwargs)
 
             profiler = sys.getprofile()
 
             if profiler:
                 return wrapped(*args, **kwargs)
 
@@ -208,15 +199,12 @@
             finally:
                 sys.setprofile(None)
 
     return FunctionWrapper(wrapped, wrapper)
 
 
 def profile_trace(name=None, group=None, label=None, params=None, depth=3):
-    return functools.partial(ProfileTraceWrapper, name=name,
-            group=group, label=label, params=params, depth=depth)
+    return functools.partial(ProfileTraceWrapper, name=name, group=group, label=label, params=params, depth=depth)
 
 
-def wrap_profile_trace(module, object_path, name=None,
-        group=None, label=None, params=None, depth=3):
-    return wrap_object(module, object_path, ProfileTraceWrapper,
-            (name, group, label, params, depth))
+def wrap_profile_trace(module, object_path, name=None, group=None, label=None, params=None, depth=3):
+    return wrap_object(module, object_path, ProfileTraceWrapper, (name, group, label, params, depth))
```

### Comparing `newrelic-8.8.1/newrelic/api/settings.py` & `newrelic-8.9.0/newrelic/api/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/solr_trace.py` & `newrelic-8.9.0/newrelic/api/solr_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/supportability.py` & `newrelic-8.9.0/newrelic/api/supportability.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/time_trace.py` & `newrelic-8.9.0/newrelic/api/time_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/transaction.py` & `newrelic-8.9.0/newrelic/api/transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -155,21 +155,19 @@
         if transaction:
             return transaction.path
 
         return "Unknown"
 
 
 class Transaction(object):
-
     STATE_PENDING = 0
     STATE_RUNNING = 1
     STATE_STOPPED = 2
 
     def __init__(self, application, enabled=None, source=None):
-
         self._application = application
 
         self._source = source
 
         self.thread_id = None
 
         self._transaction_id = id(self)
@@ -339,15 +337,14 @@
 
     def __del__(self):
         self._dead = True
         if self._state == self.STATE_RUNNING:
             self.__exit__(None, None, None)
 
     def __enter__(self):
-
         assert self._state == self.STATE_PENDING
 
         # Bail out if the transaction is not enabled.
 
         if not self.enabled:
             return self
 
@@ -399,15 +396,14 @@
         if self._source is not None:
             self.add_code_level_metrics(self._source)
             self._source = None  # Remove reference to source
 
         return self
 
     def __exit__(self, exc, value, tb):
-
         # Bail out if the transaction is not enabled.
 
         if not self.enabled:
             return
 
         if self._transaction_id != id(self):
             return
@@ -632,15 +628,14 @@
         # need to lock the profile samples and replace it with
         # an empty list just in case the thread profiler kicks
         # in just as we are trying to record the transaction.
         # If we don't, when processing the samples, addition of
         # new samples can cause an error.
 
         if not self.ignore_transaction:
-
             self._application.record_transaction(node)
 
     @property
     def sampled(self):
         return self._sampled
 
     @property
@@ -925,17 +920,15 @@
                 params, DST_ERROR_COLLECTOR | DST_TRANSACTION_TRACER, self.attribute_filter
             )
         return attributes_request
 
     @property
     def request_parameters(self):
         if (self.capture_params is None) or self.capture_params:
-
             if self._request_params:
-
                 r_attrs = {}
 
                 for k, v in self._request_params.items():
                     new_key = "request.parameters.%s" % k
                     new_val = ",".join(v)
 
                     final_key, final_val = process_user_attribute(new_key, new_val)
@@ -1033,15 +1026,17 @@
 
     def _create_distributed_trace_data(self):
         if not self.enabled:
             return
 
         settings = self._settings
         account_id = settings.account_id
-        trusted_account_key = settings.trusted_account_key
+        trusted_account_key = settings.trusted_account_key or (
+            self._settings.serverless_mode.enabled and self._settings.account_id
+        )
         application_id = settings.primary_application_id
 
         if not (account_id and application_id and trusted_account_key and settings.distributed_tracing.enabled):
             return
 
         self._compute_sampled_and_priority()
         data = dict(
@@ -1091,15 +1086,14 @@
         )
         return self._create_distributed_trace_payload()
 
     def _generate_distributed_trace_headers(self, data=None):
         try:
             data = data or self._create_distributed_trace_data()
             if data:
-
                 traceparent = W3CTraceParent(data).text()
                 yield ("traceparent", traceparent)
 
                 tracestate = NrTraceState(data).text()
                 if self.tracestate:
                     tracestate += "," + self.tracestate
                 yield ("tracestate", tracestate)
@@ -1125,15 +1119,18 @@
         headers.extend(self._generate_distributed_trace_headers())
 
     def _can_accept_distributed_trace_headers(self):
         if not self.enabled:
             return False
 
         settings = self._settings
-        if not (settings.distributed_tracing.enabled and settings.trusted_account_key):
+        trusted_account_key = settings.trusted_account_key or (
+            self._settings.serverless_mode.enabled and self._settings.account_id
+        )
+        if not (settings.distributed_tracing.enabled and trusted_account_key):
             return False
 
         if self._distributed_trace_state:
             if self._distributed_trace_state & ACCEPTED_DISTRIBUTED_TRACE:
                 self._record_supportability("Supportability/DistributedTrace/AcceptPayload/Ignored/Multiple")
             else:
                 self._record_supportability("Supportability/DistributedTrace/AcceptPayload/Ignored/CreateBeforeAccept")
@@ -1171,36 +1168,38 @@
             # Must have either id or tx
             if not any(k in data for k in ("id", "tx")):
                 self._record_supportability("Supportability/DistributedTrace/AcceptPayload/ParseException")
                 return False
 
             settings = self._settings
             account_id = data.get("ac")
+            trusted_account_key = settings.trusted_account_key or (
+                self._settings.serverless_mode.enabled and self._settings.account_id
+            )
 
             # If trust key doesn't exist in the payload, use account_id
             received_trust_key = data.get("tk", account_id)
-            if settings.trusted_account_key != received_trust_key:
+            if trusted_account_key != received_trust_key:
                 self._record_supportability("Supportability/DistributedTrace/AcceptPayload/Ignored/UntrustedAccount")
                 if settings.debug.log_untrusted_distributed_trace_keys:
                     _logger.debug(
                         "Received untrusted key in distributed trace payload. received_trust_key=%r",
                         received_trust_key,
                     )
                 return False
 
             try:
                 data["ti"] = int(data["ti"])
             except:
                 return False
 
-            if "pr" in data:
-                try:
-                    data["pr"] = float(data["pr"])
-                except:
-                    data["pr"] = None
+            try:
+                data["pr"] = float(data["pr"])
+            except Exception:
+                data["pr"] = None
 
             self._accept_distributed_trace_data(data, transport_type)
             self._record_supportability("Supportability/DistributedTrace/AcceptPayload/Success")
             return True
 
         except:
             self._record_supportability("Supportability/DistributedTrace/AcceptPayload/Exception")
@@ -1284,25 +1283,27 @@
                 return False
 
             self._record_supportability("Supportability/TraceContext/TraceParent/Accept/Success")
             if tracestate:
                 tracestate = ensure_str(tracestate)
                 try:
                     vendors = W3CTraceState.decode(tracestate)
-                    tk = self._settings.trusted_account_key
-                    payload = vendors.pop(tk + "@nr", "")
+                    trusted_account_key = self._settings.trusted_account_key or (
+                        self._settings.serverless_mode.enabled and self._settings.account_id
+                    )
+                    payload = vendors.pop(trusted_account_key + "@nr", "")
                     self.tracing_vendors = ",".join(vendors.keys())
                     self.tracestate = vendors.text(limit=31)
                 except:
                     self._record_supportability("Supportability/TraceContext/TraceState/Parse/Exception")
                 else:
                     # Remove trusted new relic header if available and parse
                     if payload:
                         try:
-                            tracestate_data = NrTraceState.decode(payload, tk)
+                            tracestate_data = NrTraceState.decode(payload, trusted_account_key)
                         except:
                             tracestate_data = None
                         if tracestate_data:
                             self.trusted_parent_span = tracestate_data.pop("id", None)
                             data.update(tracestate_data)
                         else:
                             self._record_supportability("Supportability/TraceContext/TraceState/InvalidNrEntry")
@@ -1378,15 +1379,14 @@
     def _generate_response_headers(self, read_length=None):
         nr_headers = []
 
         # Generate metrics and response headers for inbound cross
         # process web external calls.
 
         if self.client_cross_process_id is not None:
-
             # Need to work out queueing time and duration up to this
             # point for inclusion in metrics and response header. If the
             # recording of the transaction had been prematurely stopped
             # via an API call, only return time up until that call was
             # made so it will match what is reported as duration for the
             # transaction.
 
@@ -1422,19 +1422,25 @@
             )
             app_data = json_encode(payload)
 
             nr_headers.append(("X-NewRelic-App-Data", obfuscate(app_data, self._settings.encoding_key)))
 
         return nr_headers
 
-    def get_response_metadata(self):
+    # This function is CAT related and has been deprecated.
+    # Eventually, this will be removed.  Until then, coverage
+    # does not need to factor this function into its analysis.
+    def get_response_metadata(self):  # pragma: no cover
         nr_headers = dict(self._generate_response_headers())
         return convert_to_cat_metadata_value(nr_headers)
 
-    def process_request_metadata(self, cat_linking_value):
+    # This function is CAT related and has been deprecated.
+    # Eventually, this will be removed.  Until then, coverage
+    # does not need to factor this function into its analysis.
+    def process_request_metadata(self, cat_linking_value):  # pragma: no cover
         try:
             payload = base64_decode(cat_linking_value)
         except:
             # `cat_linking_value` should always be able to be base64_decoded.
             # If this is encountered, the data being sent is corrupt. No
             # exception should be raised.
             return
@@ -1443,15 +1449,14 @@
         # TODO: All the external CAT APIs really need to
         # be refactored into the transaction class.
         encoded_cross_process_id = nr_headers.get("X-NewRelic-ID")
         encoded_txn_header = nr_headers.get("X-NewRelic-Transaction")
         return self._process_incoming_cat_headers(encoded_cross_process_id, encoded_txn_header)
 
     def set_transaction_name(self, name, group=None, priority=None):
-
         # Always perform this operation even if the transaction
         # is not active at the time as will be called from
         # constructor. If path has been frozen do not allow
         # name/group to be overridden. New priority then must be
         # same or greater than existing priority. If no priority
         # always override the existing name/group if not frozen.
 
@@ -1513,15 +1518,17 @@
             level=level,
             message=message,
             attributes=get_linking_metadata(),
         )
 
         self._log_events.add(event, priority=priority)
 
-    def record_exception(self, exc=None, value=None, tb=None, params=None, ignore_errors=None):
+    # This function has been deprecated (and will be removed eventually)
+    # and therefore does not need to be included in coverage analysis
+    def record_exception(self, exc=None, value=None, tb=None, params=None, ignore_errors=None):  # pragma: no cover
         # Deprecation Warning
         warnings.warn(
             ("The record_exception function is deprecated. Please use the new api named notice_error instead."),
             DeprecationWarning,
         )
 
         self.notice_error(error=(exc, value, tb), attributes=params, ignore=ignore_errors)
@@ -1680,23 +1687,27 @@
 
         # items is a list of (name, value) tuples.
         for name, value in items:
             result &= self.add_custom_attribute(name, value)
 
         return result
 
-    def add_custom_parameter(self, name, value):
+    # This function has been deprecated (and will be removed eventually)
+    # and therefore does not need to be included in coverage analysis
+    def add_custom_parameter(self, name, value):  # pragma: no cover
         # Deprecation warning
         warnings.warn(
             ("The add_custom_parameter API has been deprecated. " "Please use the add_custom_attribute API."),
             DeprecationWarning,
         )
         return self.add_custom_attribute(name, value)
 
-    def add_custom_parameters(self, items):
+    # This function has been deprecated (and will be removed eventually)
+    # and therefore does not need to be included in coverage analysis
+    def add_custom_parameters(self, items):  # pragma: no cover
         # Deprecation warning
         warnings.warn(
             ("The add_custom_parameters API has been deprecated. " "Please use the add_custom_attributes API."),
             DeprecationWarning,
         )
         return self.add_custom_attributes(items)
 
@@ -1792,27 +1803,31 @@
     transaction = current_transaction()
     if transaction:
         return transaction.add_custom_attributes(items)
     else:
         return False
 
 
-def add_custom_parameter(key, value):
+# This function has been deprecated (and will be removed eventually)
+# and therefore does not need to be included in coverage analysis
+def add_custom_parameter(key, value):  # pragma: no cover
     # Deprecation warning
     warnings.warn(
-        ("The add_custom_parameter API has been deprecated. " "Please use the add_custom_attribute API."),
+        ("The add_custom_parameter API has been deprecated. Please use the add_custom_attribute API."),
         DeprecationWarning,
     )
     return add_custom_attribute(key, value)
 
 
-def add_custom_parameters(items):
+# This function has been deprecated (and will be removed eventually)
+# and therefore does not need to be included in coverage analysis
+def add_custom_parameters(items):  # pragma: no cover
     # Deprecation warning
     warnings.warn(
-        ("The add_custom_parameters API has been deprecated. " "Please use the add_custom_attributes API."),
+        ("The add_custom_parameters API has been deprecated. Please use the add_custom_attributes API."),
         DeprecationWarning,
     )
     return add_custom_attributes(items)
 
 
 def set_user_id(user_id):
     transaction = current_transaction()
```

### Comparing `newrelic-8.8.1/newrelic/api/transaction_name.py` & `newrelic-8.9.0/newrelic/api/transaction_name.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/web_transaction.py` & `newrelic-8.9.0/newrelic/api/web_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/api/wsgi_application.py` & `newrelic-8.9.0/newrelic/api/wsgi_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/bootstrap/__init__.py` & `newrelic-8.9.0/newrelic/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/bootstrap/sitecustomize.py` & `newrelic-8.9.0/newrelic/bootstrap/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/__init__.py` & `newrelic-8.9.0/newrelic/common/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/_monotonic.c` & `newrelic-8.9.0/newrelic/common/_monotonic.c`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/agent_http.py` & `newrelic-8.9.0/newrelic/common/agent_http.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/async_proxy.py` & `newrelic-8.9.0/newrelic/common/async_proxy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/async_wrapper.py` & `newrelic-8.9.0/newrelic/common/async_wrapper.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/cacert.pem` & `newrelic-8.9.0/newrelic/common/cacert.pem`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/certs.py` & `newrelic-8.9.0/newrelic/common/certs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/coroutine.py` & `newrelic-8.9.0/newrelic/common/coroutine.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/encoding_utils.py` & `newrelic-8.9.0/newrelic/common/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/log_file.py` & `newrelic-8.9.0/newrelic/common/log_file.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/object_names.py` & `newrelic-8.9.0/newrelic/common/object_names.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/object_wrapper.py` & `newrelic-8.9.0/newrelic/common/object_wrapper.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/package_version_utils.py` & `newrelic-8.9.0/newrelic/common/package_version_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/signature.py` & `newrelic-8.9.0/newrelic/common/signature.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/stopwatch.py` & `newrelic-8.9.0/newrelic/common/stopwatch.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/streaming_utils.py` & `newrelic-8.9.0/newrelic/common/streaming_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/system_info.py` & `newrelic-8.9.0/newrelic/common/system_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/common/utilization.py` & `newrelic-8.9.0/newrelic/common/utilization.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/config.py` & `newrelic-8.9.0/newrelic/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,22 @@
 
 # Cache of the parsed global settings found in the configuration
 # file. We cache these so can dump them out to the log file once
 # all the settings have been read.
 
 _cache_object = []
 
+
+def _reset_config_parser():
+    global _config_object
+    global _cache_object
+    _config_object = ConfigParser.RawConfigParser()
+    _cache_object = []
+
+
 # Mechanism for extracting settings from the configuration for use in
 # instrumentation modules and extensions.
 
 
 def extra_settings(section, types=None, defaults=None):
     if types is None:
         types = {}
@@ -546,14 +554,19 @@
 # Loading of configuration from specified file and for specified
 # deployment environment. Can also indicate whether configuration
 # and instrumentation errors should raise an exception or not.
 
 _configuration_done = False
 
 
+def _reset_configuration_done():
+    global _configuration_done
+    _configuration_done = False
+
+
 def _process_app_name_setting():
     # Do special processing to handle the case where the application
     # name was actually a semicolon separated list of names. In this
     # case the first application name is the primary and the others are
     # linked applications the application also reports to. What we need
     # to do is explicitly retrieve the application object for the
     # primary application name and link it with the other applications.
@@ -1234,15 +1247,14 @@
     return _instrument
 
 
 def _process_wsgi_application_configuration():
     for section in _config_object.sections():
         if not section.startswith("wsgi-application:"):
             continue
-
         enabled = False
 
         try:
             enabled = _config_object.getboolean(section, "enabled")
         except ConfigParser.NoOptionError:
             pass
         except Exception:
@@ -2834,14 +2846,18 @@
         "redis.connection",
         "newrelic.hooks.datastore_redis",
         "instrument_redis_connection",
     )
     _process_module_definition("redis.client", "newrelic.hooks.datastore_redis", "instrument_redis_client")
 
     _process_module_definition(
+        "redis.commands.cluster", "newrelic.hooks.datastore_redis", "instrument_redis_commands_cluster"
+    )
+
+    _process_module_definition(
         "redis.commands.core", "newrelic.hooks.datastore_redis", "instrument_redis_commands_core"
     )
 
     _process_module_definition(
         "redis.commands.sentinel", "newrelic.hooks.datastore_redis", "instrument_redis_commands_sentinel"
     )
 
@@ -3102,14 +3118,19 @@
 
         _process_module_definition(target, module, function)
 
 
 _instrumentation_done = False
 
 
+def _reset_instrumentation_done():
+    global _instrumentation_done
+    _instrumentation_done = False
+
+
 def _setup_instrumentation():
     global _instrumentation_done
 
     if _instrumentation_done:
         return
 
     _instrumentation_done = True
```

### Comparing `newrelic-8.8.1/newrelic/console.py` & `newrelic-8.9.0/newrelic/console.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/__init__.py` & `newrelic-8.9.0/newrelic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/_thread_utilization.c` & `newrelic-8.9.0/newrelic/core/_thread_utilization.c`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/adaptive_sampler.py` & `newrelic-8.9.0/newrelic/core/adaptive_sampler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/agent.py` & `newrelic-8.9.0/newrelic/core/agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/agent_protocol.py` & `newrelic-8.9.0/newrelic/core/agent_protocol.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/agent_streaming.py` & `newrelic-8.9.0/newrelic/core/agent_streaming.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/application.py` & `newrelic-8.9.0/newrelic/core/application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/attribute.py` & `newrelic-8.9.0/newrelic/core/attribute.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/attribute_filter.py` & `newrelic-8.9.0/newrelic/core/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/code_level_metrics.py` & `newrelic-8.9.0/newrelic/core/code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/config.py` & `newrelic-8.9.0/newrelic/core/config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/context.py` & `newrelic-8.9.0/newrelic/core/context.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/custom_event.py` & `newrelic-8.9.0/newrelic/core/custom_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/data_collector.py` & `newrelic-8.9.0/newrelic/core/data_collector.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/database_node.py` & `newrelic-8.9.0/newrelic/core/database_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/database_utils.py` & `newrelic-8.9.0/newrelic/core/database_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/datastore_node.py` & `newrelic-8.9.0/newrelic/core/datastore_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/environment.py` & `newrelic-8.9.0/newrelic/core/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,23 @@
         # Exclude lib.sub_paths as independent modules except for newrelic.hooks.
         nr_hook = name.startswith("newrelic.hooks.")
         if "." in name and not nr_hook or name.startswith("_"):
             continue
 
         # If the module isn't actually loaded (such as failed relative imports
         # in Python 2.7), the module will be None and should not be reported.
-        if not module:
+        try:
+            if not module:
+                continue
+        except Exception:
+            # if the application uses generalimport to manage optional depedencies,
+            # it's possible that generalimport.MissingOptionalDependency is raised.
+            # In this case, we should not report the module as it is not actually loaded and
+            # is not a runtime dependency of the application.
+            #
             continue
 
         # Exclude standard library/built-in modules.
         if name in stdlib_builtin_module_names:
             continue
 
         try:
```

### Comparing `newrelic-8.8.1/newrelic/core/error_collector.py` & `newrelic-8.9.0/newrelic/core/error_collector.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/error_node.py` & `newrelic-8.9.0/newrelic/core/error_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/external_node.py` & `newrelic-8.9.0/newrelic/core/external_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/function_node.py` & `newrelic-8.9.0/newrelic/core/function_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/graphql_node.py` & `newrelic-8.9.0/newrelic/core/graphql_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/graphql_utils.py` & `newrelic-8.9.0/newrelic/core/graphql_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/infinite_tracing_pb2.py` & `newrelic-8.9.0/newrelic/core/infinite_tracing_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/infinite_tracing_v3_pb2.py` & `newrelic-8.9.0/newrelic/core/infinite_tracing_v3_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/infinite_tracing_v4_pb2.py` & `newrelic-8.9.0/newrelic/core/infinite_tracing_v4_pb2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/internal_metrics.py` & `newrelic-8.9.0/newrelic/core/internal_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/log_event_node.py` & `newrelic-8.9.0/newrelic/core/log_event_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/loop_node.py` & `newrelic-8.9.0/newrelic/core/loop_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/memcache_node.py` & `newrelic-8.9.0/newrelic/core/memcache_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/message_node.py` & `newrelic-8.9.0/newrelic/core/message_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/metric.py` & `newrelic-8.9.0/newrelic/core/metric.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/node_mixin.py` & `newrelic-8.9.0/newrelic/core/node_mixin.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/profile_sessions.py` & `newrelic-8.9.0/newrelic/core/profile_sessions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/root_node.py` & `newrelic-8.9.0/newrelic/core/root_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/rules_engine.py` & `newrelic-8.9.0/newrelic/core/rules_engine.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/solr_node.py` & `newrelic-8.9.0/newrelic/core/solr_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/stack_trace.py` & `newrelic-8.9.0/newrelic/core/stack_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/stats_engine.py` & `newrelic-8.9.0/newrelic/core/stats_engine.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/string_table.py` & `newrelic-8.9.0/newrelic/core/string_table.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/thread_utilization.py` & `newrelic-8.9.0/newrelic/core/thread_utilization.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/trace_cache.py` & `newrelic-8.9.0/newrelic/core/trace_cache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/trace_node.py` & `newrelic-8.9.0/newrelic/core/trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/core/transaction_node.py` & `newrelic-8.9.0/newrelic/core/transaction_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/extras/__init__.py` & `newrelic-8.9.0/newrelic/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/extras/framework_django/__init__.py` & `newrelic-8.9.0/newrelic/extras/framework_django/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/extras/framework_django/templatetags/__init__.py` & `newrelic-8.9.0/newrelic/extras/framework_django/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/extras/framework_django/templatetags/newrelic_tags.py` & `newrelic-8.9.0/newrelic/extras/framework_django/templatetags/newrelic_tags.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/__init__.py` & `newrelic-8.9.0/newrelic/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_asgiref.py` & `newrelic-8.9.0/newrelic/hooks/adapter_asgiref.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_cheroot.py` & `newrelic-8.9.0/newrelic/hooks/adapter_cheroot.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_cherrypy.py` & `newrelic-8.9.0/newrelic/hooks/adapter_cherrypy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_daphne.py` & `newrelic-8.9.0/newrelic/hooks/adapter_daphne.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_flup.py` & `newrelic-8.9.0/newrelic/hooks/adapter_flup.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_gevent.py` & `newrelic-8.9.0/newrelic/hooks/adapter_gevent.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_gunicorn.py` & `newrelic-8.9.0/newrelic/hooks/adapter_gunicorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_hypercorn.py` & `newrelic-8.9.0/newrelic/hooks/adapter_hypercorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_meinheld.py` & `newrelic-8.9.0/newrelic/hooks/adapter_meinheld.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_paste.py` & `newrelic-8.9.0/newrelic/hooks/adapter_paste.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_uvicorn.py` & `newrelic-8.9.0/newrelic/hooks/adapter_uvicorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_waitress.py` & `newrelic-8.9.0/newrelic/hooks/adapter_waitress.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/adapter_wsgiref.py` & `newrelic-8.9.0/newrelic/hooks/adapter_wsgiref.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/application_celery.py` & `newrelic-8.9.0/newrelic/hooks/application_celery.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/application_gearman.py` & `newrelic-8.9.0/newrelic/hooks/application_gearman.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/component_cornice.py` & `newrelic-8.9.0/newrelic/hooks/component_cornice.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/component_djangorestframework.py` & `newrelic-8.9.0/newrelic/hooks/component_djangorestframework.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/component_flask_rest.py` & `newrelic-8.9.0/newrelic/hooks/component_flask_rest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/component_graphqlserver.py` & `newrelic-8.9.0/newrelic/hooks/component_graphqlserver.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/component_piston.py` & `newrelic-8.9.0/newrelic/hooks/component_piston.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/component_sentry.py` & `newrelic-8.9.0/newrelic/hooks/component_sentry.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/component_tastypie.py` & `newrelic-8.9.0/newrelic/hooks/component_tastypie.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/coroutines_asyncio.py` & `newrelic-8.9.0/newrelic/hooks/coroutines_asyncio.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/coroutines_gevent.py` & `newrelic-8.9.0/newrelic/hooks/coroutines_gevent.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_asyncpg.py` & `newrelic-8.9.0/newrelic/hooks/database_asyncpg.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_cx_oracle.py` & `newrelic-8.9.0/newrelic/hooks/database_cx_oracle.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_dbapi2.py` & `newrelic-8.9.0/newrelic/hooks/database_dbapi2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_ibm_db_dbi.py` & `newrelic-8.9.0/newrelic/hooks/database_ibm_db_dbi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_mysql.py` & `newrelic-8.9.0/newrelic/hooks/database_mysql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_mysqldb.py` & `newrelic-8.9.0/newrelic/hooks/database_mysqldb.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_oursql.py` & `newrelic-8.9.0/newrelic/hooks/database_oursql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_postgresql.py` & `newrelic-8.9.0/newrelic/hooks/database_postgresql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_psycopg2.py` & `newrelic-8.9.0/newrelic/hooks/database_psycopg2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_psycopg2cffi.py` & `newrelic-8.9.0/newrelic/hooks/database_psycopg2cffi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_psycopg2ct.py` & `newrelic-8.9.0/newrelic/hooks/database_psycopg2ct.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_pymssql.py` & `newrelic-8.9.0/newrelic/hooks/database_pymssql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_pymysql.py` & `newrelic-8.9.0/newrelic/hooks/database_pymysql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_pyodbc.py` & `newrelic-8.9.0/newrelic/hooks/database_pyodbc.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/database_sqlite.py` & `newrelic-8.9.0/newrelic/hooks/database_sqlite.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_aioredis.py` & `newrelic-8.9.0/newrelic/hooks/datastore_aioredis.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_aredis.py` & `newrelic-8.9.0/newrelic/hooks/datastore_aredis.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_bmemcached.py` & `newrelic-8.9.0/newrelic/hooks/datastore_bmemcached.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_elasticsearch.py` & `newrelic-8.9.0/newrelic/hooks/datastore_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_memcache.py` & `newrelic-8.9.0/newrelic/hooks/datastore_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_motor.py` & `newrelic-8.9.0/newrelic/hooks/datastore_motor.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_pyelasticsearch.py` & `newrelic-8.9.0/newrelic/hooks/datastore_pyelasticsearch.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_pylibmc.py` & `newrelic-8.9.0/newrelic/hooks/datastore_pylibmc.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_pymemcache.py` & `newrelic-8.9.0/newrelic/hooks/datastore_pymemcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_pymongo.py` & `newrelic-8.9.0/newrelic/hooks/datastore_pymongo.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_pysolr.py` & `newrelic-8.9.0/newrelic/hooks/datastore_pysolr.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_redis.py` & `newrelic-8.9.0/newrelic/hooks/datastore_redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -593,14 +593,18 @@
     _instrument_redis_commands_module(module, "BFCommands")
     _instrument_redis_commands_module(module, "CFCommands")
     _instrument_redis_commands_module(module, "CMSCommands")
     _instrument_redis_commands_module(module, "TDigestCommands")
     _instrument_redis_commands_module(module, "TOPKCommands")
 
 
+def instrument_redis_commands_cluster(module):
+    _instrument_redis_commands_module(module, "RedisClusterCommands")
+
+
 def _instrument_redis_commands_module(module, class_name):
     for name in _redis_client_methods:
         if hasattr(module, class_name):
             class_instance = getattr(module, class_name)
             if hasattr(class_instance, name):
                 _wrap_Redis_method_wrapper_(module, class_name, name)
```

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_solrpy.py` & `newrelic-8.9.0/newrelic/hooks/datastore_solrpy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/datastore_umemcache.py` & `newrelic-8.9.0/newrelic/hooks/datastore_umemcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_botocore.py` & `newrelic-8.9.0/newrelic/hooks/external_botocore.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_dropbox.py` & `newrelic-8.9.0/newrelic/hooks/external_dropbox.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_facepy.py` & `newrelic-8.9.0/newrelic/hooks/external_facepy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_feedparser.py` & `newrelic-8.9.0/newrelic/hooks/external_feedparser.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_httplib.py` & `newrelic-8.9.0/newrelic/hooks/external_httplib.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_httplib2.py` & `newrelic-8.9.0/newrelic/hooks/external_httplib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_httpx.py` & `newrelic-8.9.0/newrelic/hooks/external_httpx.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_pywapi.py` & `newrelic-8.9.0/newrelic/hooks/external_pywapi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_requests.py` & `newrelic-8.9.0/newrelic/hooks/external_requests.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_thrift.py` & `newrelic-8.9.0/newrelic/hooks/external_thrift.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_urllib.py` & `newrelic-8.9.0/newrelic/hooks/external_urllib.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_urllib2.py` & `newrelic-8.9.0/newrelic/hooks/external_urllib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_urllib3.py` & `newrelic-8.9.0/newrelic/hooks/external_urllib3.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/external_xmlrpclib.py` & `newrelic-8.9.0/newrelic/hooks/external_xmlrpclib.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_aiohttp.py` & `newrelic-8.9.0/newrelic/hooks/framework_aiohttp.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_ariadne.py` & `newrelic-8.9.0/newrelic/hooks/framework_ariadne.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_bottle.py` & `newrelic-8.9.0/newrelic/hooks/framework_bottle.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_cherrypy.py` & `newrelic-8.9.0/newrelic/hooks/framework_cherrypy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_django.py` & `newrelic-8.9.0/newrelic/hooks/framework_django.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_django_py3.py` & `newrelic-8.9.0/newrelic/hooks/framework_django_py3.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_falcon.py` & `newrelic-8.9.0/newrelic/hooks/framework_falcon.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_fastapi.py` & `newrelic-8.9.0/newrelic/hooks/framework_fastapi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_flask.py` & `newrelic-8.9.0/newrelic/hooks/framework_flask.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_graphene.py` & `newrelic-8.9.0/newrelic/hooks/framework_graphene.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_graphql.py` & `newrelic-8.9.0/newrelic/hooks/framework_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_grpc.py` & `newrelic-8.9.0/newrelic/hooks/framework_grpc.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_pylons.py` & `newrelic-8.9.0/newrelic/hooks/framework_pylons.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_pyramid.py` & `newrelic-8.9.0/newrelic/hooks/framework_pyramid.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_sanic.py` & `newrelic-8.9.0/newrelic/hooks/framework_sanic.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_starlette.py` & `newrelic-8.9.0/newrelic/hooks/framework_starlette.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_strawberry.py` & `newrelic-8.9.0/newrelic/hooks/framework_strawberry.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_tornado.py` & `newrelic-8.9.0/newrelic/hooks/framework_tornado.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_web2py.py` & `newrelic-8.9.0/newrelic/hooks/framework_web2py.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/framework_webpy.py` & `newrelic-8.9.0/newrelic/hooks/framework_webpy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/logger_logging.py` & `newrelic-8.9.0/newrelic/hooks/logger_logging.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/logger_loguru.py` & `newrelic-8.9.0/newrelic/hooks/logger_loguru.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/memcache_memcache.py` & `newrelic-8.9.0/newrelic/hooks/memcache_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/messagebroker_confluentkafka.py` & `newrelic-8.9.0/newrelic/hooks/messagebroker_confluentkafka.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/messagebroker_kafkapython.py` & `newrelic-8.9.0/newrelic/hooks/messagebroker_kafkapython.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/messagebroker_pika.py` & `newrelic-8.9.0/newrelic/hooks/messagebroker_pika.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/middleware_flask_compress.py` & `newrelic-8.9.0/newrelic/hooks/middleware_flask_compress.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/middleware_weberror.py` & `newrelic-8.9.0/newrelic/hooks/middleware_weberror.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/template_genshi.py` & `newrelic-8.9.0/newrelic/hooks/template_genshi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/template_jinja2.py` & `newrelic-8.9.0/newrelic/hooks/template_jinja2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/hooks/template_mako.py` & `newrelic-8.9.0/newrelic/hooks/template_mako.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/network/__init__.py` & `newrelic-8.9.0/newrelic/network/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/network/addresses.py` & `newrelic-8.9.0/newrelic/network/addresses.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/network/exceptions.py` & `newrelic-8.9.0/newrelic/network/exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/newrelic.ini` & `newrelic-8.9.0/newrelic/newrelic.ini`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/asgiref_compatibility.py` & `newrelic-8.9.0/newrelic/packages/asgiref_compatibility.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/isort/LICENSE` & `newrelic-8.9.0/newrelic/packages/isort/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/isort/stdlibs/py27.py` & `newrelic-8.9.0/newrelic/packages/isort/stdlibs/py27.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/isort/stdlibs/py310.py` & `newrelic-8.9.0/newrelic/packages/isort/stdlibs/py310.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/isort/stdlibs/py311.py` & `newrelic-8.9.0/newrelic/packages/isort/stdlibs/py311.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/isort/stdlibs/py36.py` & `newrelic-8.9.0/newrelic/packages/isort/stdlibs/py36.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/isort/stdlibs/py37.py` & `newrelic-8.9.0/newrelic/packages/isort/stdlibs/py37.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/isort/stdlibs/py38.py` & `newrelic-8.9.0/newrelic/packages/isort/stdlibs/py38.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/isort/stdlibs/py39.py` & `newrelic-8.9.0/newrelic/packages/isort/stdlibs/py39.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/six.py` & `newrelic-8.9.0/newrelic/packages/six.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/LICENSE.txt` & `newrelic-8.9.0/newrelic/packages/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/__init__.py` & `newrelic-8.9.0/newrelic/packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/_collections.py` & `newrelic-8.9.0/newrelic/packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/connection.py` & `newrelic-8.9.0/newrelic/packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/connectionpool.py` & `newrelic-8.9.0/newrelic/packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/contrib/_appengine_environ.py` & `newrelic-8.9.0/newrelic/packages/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/contrib/_securetransport/bindings.py` & `newrelic-8.9.0/newrelic/packages/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/contrib/_securetransport/low_level.py` & `newrelic-8.9.0/newrelic/packages/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/contrib/appengine.py` & `newrelic-8.9.0/newrelic/packages/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/contrib/ntlmpool.py` & `newrelic-8.9.0/newrelic/packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/contrib/pyopenssl.py` & `newrelic-8.9.0/newrelic/packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/contrib/securetransport.py` & `newrelic-8.9.0/newrelic/packages/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/contrib/socks.py` & `newrelic-8.9.0/newrelic/packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/exceptions.py` & `newrelic-8.9.0/newrelic/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/fields.py` & `newrelic-8.9.0/newrelic/packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/filepost.py` & `newrelic-8.9.0/newrelic/packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/packages/backports/makefile.py` & `newrelic-8.9.0/newrelic/packages/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/packages/six.py` & `newrelic-8.9.0/newrelic/packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/poolmanager.py` & `newrelic-8.9.0/newrelic/packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/request.py` & `newrelic-8.9.0/newrelic/packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/response.py` & `newrelic-8.9.0/newrelic/packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/util/__init__.py` & `newrelic-8.9.0/newrelic/packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/util/connection.py` & `newrelic-8.9.0/newrelic/packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/util/proxy.py` & `newrelic-8.9.0/newrelic/packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/util/request.py` & `newrelic-8.9.0/newrelic/packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/util/response.py` & `newrelic-8.9.0/newrelic/packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/util/retry.py` & `newrelic-8.9.0/newrelic/packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/util/ssl_.py` & `newrelic-8.9.0/newrelic/packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/util/ssl_match_hostname.py` & `newrelic-8.9.0/newrelic/packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/util/ssltransport.py` & `newrelic-8.9.0/newrelic/packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/util/timeout.py` & `newrelic-8.9.0/newrelic/packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/util/url.py` & `newrelic-8.9.0/newrelic/packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/urllib3/util/wait.py` & `newrelic-8.9.0/newrelic/packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/wrapt/LICENSE` & `newrelic-8.9.0/newrelic/packages/wrapt/LICENSE`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/wrapt/__init__.py` & `newrelic-8.9.0/newrelic/packages/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/wrapt/_wrappers.c` & `newrelic-8.9.0/newrelic/packages/wrapt/_wrappers.c`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/wrapt/arguments.py` & `newrelic-8.9.0/newrelic/packages/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/wrapt/decorators.py` & `newrelic-8.9.0/newrelic/packages/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/wrapt/importer.py` & `newrelic-8.9.0/newrelic/packages/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/packages/wrapt/wrappers.py` & `newrelic-8.9.0/newrelic/packages/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/samplers/__init__.py` & `newrelic-8.9.0/newrelic/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/samplers/cpu_usage.py` & `newrelic-8.9.0/newrelic/samplers/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/samplers/data_sampler.py` & `newrelic-8.9.0/newrelic/samplers/data_sampler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/samplers/decorators.py` & `newrelic-8.9.0/newrelic/samplers/decorators.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/samplers/gc_data.py` & `newrelic-8.9.0/newrelic/samplers/gc_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic/samplers/memory_usage.py` & `newrelic-8.9.0/newrelic/samplers/memory_usage.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/newrelic.egg-info/PKG-INFO` & `newrelic-8.9.0/newrelic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic
-Version: 8.8.1
+Version: 8.9.0
 Summary: New Relic Python Agent
 Home-page: https://docs.newrelic.com/docs/apm/agents/python-agent/
 Author: New Relic
 Author-email: support@newrelic.com
 Maintainer: New Relic
 Maintainer-email: support@newrelic.com
 License: Apache-2.0
```

### Comparing `newrelic-8.8.1/newrelic.egg-info/SOURCES.txt` & `newrelic-8.9.0/newrelic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 .github/mergify.yml
 .github/pull_request_template.md
 .github/stale.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/troubleshooting.md
-.github/actions/setup-python-matrix/action.yml
 .github/containers/Dockerfile
 .github/containers/Makefile
 .github/containers/install-python.sh
 .github/containers/requirements.txt
 .github/scripts/retry.sh
 .github/workflows/build-ci-image.yml
 .github/workflows/deploy-python.yml
@@ -375,28 +374,30 @@
 tests/agent_features/test_cat.py
 tests/agent_features/test_code_level_metrics.py
 tests/agent_features/test_collector_payloads.py
 tests/agent_features/test_configuration.py
 tests/agent_features/test_coroutine_trace.py
 tests/agent_features/test_coroutine_transaction.py
 tests/agent_features/test_custom_events.py
+tests/agent_features/test_custom_metrics.py
 tests/agent_features/test_dead_transactions.py
 tests/agent_features/test_distributed_tracing.py
 tests/agent_features/test_error_events.py
 tests/agent_features/test_error_group_callback.py
 tests/agent_features/test_event_loop_wait_time.py
 tests/agent_features/test_exception_messages.py
 tests/agent_features/test_function_trace.py
 tests/agent_features/test_high_security_mode.py
 tests/agent_features/test_ignore_expected_errors.py
 tests/agent_features/test_lambda_handler.py
 tests/agent_features/test_log_events.py
 tests/agent_features/test_logs_in_context.py
 tests/agent_features/test_notice_error.py
 tests/agent_features/test_priority_sampling.py
+tests/agent_features/test_profile_trace.py
 tests/agent_features/test_serverless_mode.py
 tests/agent_features/test_span_events.py
 tests/agent_features/test_stack_trace.py
 tests/agent_features/test_supportability_metrics.py
 tests/agent_features/test_synthetics.py
 tests/agent_features/test_time_trace.py
 tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py
@@ -825,14 +826,16 @@
 tests/datastore_psycopg2cffi/test_explain_plans.py
 tests/datastore_pylibmc/conftest.py
 tests/datastore_pylibmc/test_memcache.py
 tests/datastore_pymemcache/conftest.py
 tests/datastore_pymemcache/test_memcache.py
 tests/datastore_pymongo/conftest.py
 tests/datastore_pymongo/test_pymongo.py
+tests/datastore_pymssql/conftest.py
+tests/datastore_pymssql/test_database.py
 tests/datastore_pymysql/conftest.py
 tests/datastore_pymysql/test_database.py
 tests/datastore_pyodbc/conftest.py
 tests/datastore_pyodbc/test_pyodbc.py
 tests/datastore_pysolr/conftest.py
 tests/datastore_pysolr/test_solr.py
 tests/datastore_redis/conftest.py
@@ -841,14 +844,16 @@
 tests/datastore_redis/test_get_and_set.py
 tests/datastore_redis/test_instance_info.py
 tests/datastore_redis/test_multiple_dbs.py
 tests/datastore_redis/test_rb.py
 tests/datastore_redis/test_span_event.py
 tests/datastore_redis/test_trace_node.py
 tests/datastore_redis/test_uninstrumented_methods.py
+tests/datastore_rediscluster/conftest.py
+tests/datastore_rediscluster/test_uninstrumented_rediscluster_methods.py
 tests/datastore_solrpy/conftest.py
 tests/datastore_solrpy/test_solr.py
 tests/datastore_sqlite/conftest.py
 tests/datastore_sqlite/test_database.py
 tests/datastore_sqlite/test_obfuscation.py
 tests/external_boto3/conftest.py
 tests/external_boto3/test_boto3_iam.py
@@ -1015,14 +1020,16 @@
 tests/messagebroker_pika/test_pika_async_connection_consume.py
 tests/messagebroker_pika/test_pika_blocking_connection_consume.py
 tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py
 tests/messagebroker_pika/test_pika_produce.py
 tests/messagebroker_pika/test_pika_supportability.py
 tests/template_genshi/conftest.py
 tests/template_genshi/test_genshi.py
+tests/template_jinja2/conftest.py
+tests/template_jinja2/test_jinja2.py
 tests/template_mako/conftest.py
 tests/template_mako/test_mako.py
 tests/testing_support/__init__.py
 tests/testing_support/asgi_testing.py
 tests/testing_support/db_settings.py
 tests/testing_support/external_fixtures.py
 tests/testing_support/fixtures.py
```

### Comparing `newrelic-8.8.1/setup.py` & `newrelic-8.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_cheroot/conftest.py` & `newrelic-8.9.0/tests/adapter_cheroot/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_cheroot/test_wsgi.py` & `newrelic-8.9.0/tests/adapter_cheroot/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_daphne/conftest.py` & `newrelic-8.9.0/tests/adapter_daphne/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_daphne/test_daphne.py` & `newrelic-8.9.0/tests/adapter_daphne/test_daphne.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_gevent/_application.py` & `newrelic-8.9.0/tests/adapter_gevent/_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_gevent/conftest.py` & `newrelic-8.9.0/tests/adapter_gevent/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_gevent/test_patching.py` & `newrelic-8.9.0/tests/adapter_gevent/test_patching.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_gevent/test_pywsgi.py` & `newrelic-8.9.0/tests/adapter_gevent/test_pywsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_gunicorn/app.py` & `newrelic-8.9.0/tests/adapter_gunicorn/app.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_gunicorn/asgi_app.py` & `newrelic-8.9.0/tests/adapter_gunicorn/asgi_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_gunicorn/async_app.py` & `newrelic-8.9.0/tests/adapter_gunicorn/async_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_gunicorn/conftest.py` & `newrelic-8.9.0/tests/adapter_gunicorn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_gunicorn/test_aiohttp_app_factory.py` & `newrelic-8.9.0/tests/adapter_gunicorn/test_aiohttp_app_factory.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_gunicorn/test_asgi_app.py` & `newrelic-8.9.0/tests/adapter_gunicorn/test_asgi_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_gunicorn/test_gaiohttp.py` & `newrelic-8.9.0/tests/adapter_gunicorn/test_gaiohttp.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_gunicorn/worker.py` & `newrelic-8.9.0/tests/adapter_gunicorn/worker.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_hypercorn/conftest.py` & `newrelic-8.9.0/tests/adapter_hypercorn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_hypercorn/test_hypercorn.py` & `newrelic-8.9.0/tests/adapter_hypercorn/test_hypercorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_uvicorn/conftest.py` & `newrelic-8.9.0/tests/adapter_uvicorn/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_uvicorn/test_uvicorn.py` & `newrelic-8.9.0/tests/adapter_uvicorn/test_uvicorn.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_waitress/_application.py` & `newrelic-8.9.0/tests/adapter_waitress/_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_waitress/conftest.py` & `newrelic-8.9.0/tests/adapter_waitress/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/adapter_waitress/test_wsgi.py` & `newrelic-8.9.0/tests/adapter_waitress/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/_test_async_coroutine_trace.py` & `newrelic-8.9.0/tests/agent_features/_test_async_coroutine_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/_test_async_coroutine_transaction.py` & `newrelic-8.9.0/tests/agent_features/_test_async_coroutine_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/_test_code_level_metrics.py` & `newrelic-8.9.0/tests/agent_features/_test_code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/conftest.py` & `newrelic-8.9.0/tests/agent_features/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_apdex_metrics.py` & `newrelic-8.9.0/tests/framework_fastapi/test_application.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,29 +8,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import webtest
+import logging
 
-from testing_support.validators.validate_apdex_metrics import (
-        validate_apdex_metrics)
-from testing_support.sample_applications import simple_app
+import pytest
+from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
+from testing_support.validators.validate_code_level_metrics import validate_code_level_metrics
 
 
-normal_application = webtest.TestApp(simple_app)
-
+@pytest.mark.parametrize(
+    "endpoint,transaction_name",
+    (
+        ("/sync", "_target_application:sync"),
+        ("/async", "_target_application:non_sync"),
+    ),
+)
+def test_application(caplog, app, endpoint, transaction_name):
+    caplog.set_level(logging.ERROR)
 
-# NOTE: This test validates that the server-side apdex_t is set to 0.5
-# If the server-side configuration changes, this test will start to fail.
+    @validate_transaction_metrics(transaction_name, scoped_metrics=[("Function/" + transaction_name, 1)])
+    @validate_code_level_metrics(*transaction_name.split(":"))
+    def _test():
+        response = app.get(endpoint)
+        assert response.status == 200
 
+        # Catch context propagation error messages
+        assert not caplog.records
 
-@validate_apdex_metrics(
-    name='',
-    group='Uri',
-    apdex_t_min=0.5,
-    apdex_t_max=0.5,
-)
-def test_apdex():
-    normal_application.get('/')
+    _test()
```

### Comparing `newrelic-8.8.1/tests/agent_features/test_asgi_browser.py` & `newrelic-8.9.0/tests/agent_features/test_asgi_browser.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_asgi_distributed_tracing.py` & `newrelic-8.9.0/tests/agent_features/test_asgi_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_asgi_transaction.py` & `newrelic-8.9.0/tests/agent_features/test_asgi_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_asgi_w3c_trace_context.py` & `newrelic-8.9.0/tests/agent_features/test_asgi_w3c_trace_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_async_context_propagation.py` & `newrelic-8.9.0/tests/agent_features/test_async_context_propagation.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_async_timing.py` & `newrelic-8.9.0/tests/agent_features/test_async_timing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_attribute.py` & `newrelic-8.9.0/tests/agent_features/test_attribute.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_attributes_in_action.py` & `newrelic-8.9.0/tests/agent_features/test_attributes_in_action.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_background_task.py` & `newrelic-8.9.0/tests/agent_features/test_background_task.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_browser.py` & `newrelic-8.9.0/tests/agent_features/test_browser.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_browser_middleware.py` & `newrelic-8.9.0/tests/agent_features/test_browser_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_cat.py` & `newrelic-8.9.0/tests/agent_features/test_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_code_level_metrics.py` & `newrelic-8.9.0/tests/agent_features/test_code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_collector_payloads.py` & `newrelic-8.9.0/tests/agent_features/test_collector_payloads.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_coroutine_trace.py` & `newrelic-8.9.0/tests/agent_features/test_coroutine_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_coroutine_transaction.py` & `newrelic-8.9.0/tests/agent_features/test_coroutine_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_custom_events.py` & `newrelic-8.9.0/tests/agent_features/test_custom_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_dead_transactions.py` & `newrelic-8.9.0/tests/agent_features/test_dead_transactions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_distributed_tracing.py` & `newrelic-8.9.0/tests/agent_features/test_distributed_tracing.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,16 +26,20 @@
 )
 from testing_support.validators.validate_transaction_metrics import (
     validate_transaction_metrics,
 )
 
 from newrelic.api.application import application_instance
 from newrelic.api.background_task import BackgroundTask, background_task
+from newrelic.api.external_trace import ExternalTrace
 from newrelic.api.time_trace import current_trace
 from newrelic.api.transaction import (
+    accept_distributed_trace_headers,
+    accept_distributed_trace_payload,
+    create_distributed_trace_payload,
     current_span_id,
     current_trace_id,
     current_transaction,
 )
 from newrelic.api.web_transaction import WSGIWebTransaction
 from newrelic.api.wsgi_application import wsgi_application
 
@@ -181,18 +185,18 @@
                 "ti": 1518469636035,
                 "tx": "7d3efb1b173fecfa",
             },
         }
         payload["d"]["pa"] = "5e5733a911cfbc73"
 
         if accept_payload:
-            result = txn.accept_distributed_trace_payload(payload)
+            result = accept_distributed_trace_payload(payload)
             assert result
         else:
-            txn._create_distributed_trace_payload()
+            create_distributed_trace_payload()
 
         try:
             raise ValueError("cookies")
         except ValueError:
             txn.notice_error()
 
     _test()
@@ -315,30 +319,28 @@
         (True, False, False, TRACE_CONTEXT_ACCEPTED),
         (True, False, True, TRACE_CONTEXT_ACCEPTED),
         (True, True, False, TRACE_CONTEXT_ACCEPTED),
     ],
 )
 @override_application_settings(_override_settings)
 def test_distributed_tracing_backwards_compatibility(traceparent, tracestate, newrelic, metrics):
-
     headers = []
     if traceparent:
         headers.append(("traceparent", TRACEPARENT))
     if tracestate:
         headers.append(("tracestate", TRACESTATE))
     if newrelic:
         headers.append(("newrelic", json.dumps(payload)))
 
     @validate_transaction_metrics(
         "test_distributed_tracing_backwards_compatibility", background_task=True, rollup_metrics=metrics
     )
     @background_task(name="test_distributed_tracing_backwards_compatibility")
     def _test():
-        transaction = current_transaction()
-        transaction.accept_distributed_trace_headers(headers)
+        accept_distributed_trace_headers(headers)
 
     _test()
 
 
 @background_task(name="test_current_trace_id_api_inside_transaction")
 def test_current_trace_id_api_inside_transaction():
     trace_id = current_trace_id()
@@ -356,7 +358,69 @@
     span_id = current_span_id()
     assert span_id == current_trace().guid
 
 
 def test_current_span_id_outside_transaction():
     span_id = current_span_id()
     assert span_id is None
+
+
+@pytest.mark.parametrize("trusted_account_key", ("1", None), ids=("tk_set", "tk_unset"))
+def test_outbound_dt_payload_generation(trusted_account_key):
+    @override_application_settings(
+        {
+            "distributed_tracing.enabled": True,
+            "account_id": "1",
+            "trusted_account_key": trusted_account_key,
+            "primary_application_id": "1",
+        }
+    )
+    @background_task(name="test_outbound_dt_payload_generation")
+    def _test_outbound_dt_payload_generation():
+        transaction = current_transaction()
+        payload = ExternalTrace.generate_request_headers(transaction)
+        if trusted_account_key:
+            assert payload
+            # Ensure trusted account key present as vendor
+            assert dict(payload)["tracestate"].startswith("1@nr=")
+        else:
+            assert not payload
+
+    _test_outbound_dt_payload_generation()
+
+
+@pytest.mark.parametrize("trusted_account_key", ("1", None), ids=("tk_set", "tk_unset"))
+def test_inbound_dt_payload_acceptance(trusted_account_key):
+    @override_application_settings(
+        {
+            "distributed_tracing.enabled": True,
+            "account_id": "1",
+            "trusted_account_key": trusted_account_key,
+            "primary_application_id": "1",
+        }
+    )
+    @background_task(name="_test_inbound_dt_payload_acceptance")
+    def _test_inbound_dt_payload_acceptance():
+        transaction = current_transaction()
+
+        payload = {
+            "v": [0, 1],
+            "d": {
+                "ty": "Mobile",
+                "ac": "1",
+                "tk": "1",
+                "ap": "2827902",
+                "pa": "5e5733a911cfbc73",
+                "id": "7d3efb1b173fecfa",
+                "tr": "d6b4ba0c3a712ca",
+                "ti": 1518469636035,
+                "tx": "8703ff3d88eefe9d",
+            },
+        }
+
+        result = transaction.accept_distributed_trace_payload(payload)
+        if trusted_account_key:
+            assert result
+        else:
+            assert not result
+
+    _test_inbound_dt_payload_acceptance()
```

### Comparing `newrelic-8.8.1/tests/agent_features/test_error_events.py` & `newrelic-8.9.0/tests/agent_features/test_error_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_error_group_callback.py` & `newrelic-8.9.0/tests/agent_features/test_error_group_callback.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_event_loop_wait_time.py` & `newrelic-8.9.0/tests/agent_features/test_event_loop_wait_time.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_exception_messages.py` & `newrelic-8.9.0/tests/agent_features/test_exception_messages.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_function_trace.py` & `newrelic-8.9.0/tests/agent_features/test_function_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_high_security_mode.py` & `newrelic-8.9.0/tests/agent_features/test_high_security_mode.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_ignore_expected_errors.py` & `newrelic-8.9.0/tests/agent_features/test_ignore_expected_errors.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_lambda_handler.py` & `newrelic-8.9.0/tests/agent_features/test_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_log_events.py` & `newrelic-8.9.0/tests/agent_features/test_log_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_logs_in_context.py` & `newrelic-8.9.0/tests/agent_features/test_logs_in_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_notice_error.py` & `newrelic-8.9.0/tests/agent_features/test_notice_error.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_priority_sampling.py` & `newrelic-8.9.0/tests/agent_features/test_priority_sampling.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_serverless_mode.py` & `newrelic-8.9.0/tests/agent_features/test_serverless_mode.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,60 +9,61 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
+
 import pytest
+from testing_support.fixtures import override_generic_settings
+from testing_support.validators.validate_serverless_data import validate_serverless_data
+from testing_support.validators.validate_serverless_metadata import (
+    validate_serverless_metadata,
+)
+from testing_support.validators.validate_serverless_payload import (
+    validate_serverless_payload,
+)
 
 from newrelic.api.application import application_instance
 from newrelic.api.background_task import background_task
 from newrelic.api.external_trace import ExternalTrace
 from newrelic.api.lambda_handler import lambda_handler
 from newrelic.api.transaction import current_transaction
 from newrelic.core.config import global_settings
 
-from testing_support.fixtures import override_generic_settings
-from testing_support.validators.validate_serverless_data import (
-        validate_serverless_data)
-from testing_support.validators.validate_serverless_payload import (
-        validate_serverless_payload)
-from testing_support.validators.validate_serverless_metadata import (
-        validate_serverless_metadata)
-
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def serverless_application(request):
     settings = global_settings()
     orig = settings.serverless_mode.enabled
     settings.serverless_mode.enabled = True
 
-    application_name = 'Python Agent Test (test_serverless_mode:%s)' % (
-            request.node.name)
+    application_name = "Python Agent Test (test_serverless_mode:%s)" % (request.node.name)
     application = application_instance(application_name)
     application.activate()
 
     yield application
 
     settings.serverless_mode.enabled = orig
 
 
 def test_serverless_payload(capsys, serverless_application):
-
-    @override_generic_settings(serverless_application.settings, {
-        'distributed_tracing.enabled': True,
-    })
+    @override_generic_settings(
+        serverless_application.settings,
+        {
+            "distributed_tracing.enabled": True,
+        },
+    )
     @validate_serverless_data(
-            expected_methods=('metric_data', 'analytic_event_data'),
-            forgone_methods=('preconnect', 'connect', 'get_agent_commands'))
+        expected_methods=("metric_data", "analytic_event_data"),
+        forgone_methods=("preconnect", "connect", "get_agent_commands"),
+    )
     @validate_serverless_payload()
-    @background_task(
-            application=serverless_application,
-            name='test_serverless_payload')
+    @background_task(application=serverless_application, name="test_serverless_payload")
     def _test():
         transaction = current_transaction()
         assert transaction.settings.serverless_mode.enabled
 
     _test()
 
     out, err = capsys.readouterr()
@@ -71,106 +72,109 @@
     assert out
 
     # Verify that the payload is loadable JSON
     payload = json.loads(out)
 
 
 def test_no_cat_headers(serverless_application):
-    @background_task(
-            application=serverless_application,
-            name='test_cat_headers')
+    @background_task(application=serverless_application, name="test_cat_headers")
     def _test_cat_headers():
         transaction = current_transaction()
 
         payload = ExternalTrace.generate_request_headers(transaction)
         assert not payload
 
-        trace = ExternalTrace('testlib', 'http://example.com')
-        response_headers = [('X-NewRelic-App-Data', 'Cookies')]
+        trace = ExternalTrace("testlib", "http://example.com")
+        response_headers = [("X-NewRelic-App-Data", "Cookies")]
         with trace:
             trace.process_response_headers(response_headers)
 
         assert transaction.settings.cross_application_tracer.enabled is False
 
     _test_cat_headers()
 
 
-def test_dt_outbound(serverless_application):
-    @override_generic_settings(serverless_application.settings, {
-        'distributed_tracing.enabled': True,
-        'account_id': '1',
-        'trusted_account_key': '1',
-        'primary_application_id': '1',
-    })
-    @background_task(
-            application=serverless_application,
-            name='test_dt_outbound')
-    def _test_dt_outbound():
+@pytest.mark.parametrize("trusted_account_key", ("1", None), ids=("tk_set", "tk_unset"))
+def test_outbound_dt_payload_generation(serverless_application, trusted_account_key):
+    @override_generic_settings(
+        serverless_application.settings,
+        {
+            "distributed_tracing.enabled": True,
+            "account_id": "1",
+            "trusted_account_key": trusted_account_key,
+            "primary_application_id": "1",
+        },
+    )
+    @background_task(application=serverless_application, name="test_outbound_dt_payload_generation")
+    def _test_outbound_dt_payload_generation():
         transaction = current_transaction()
         payload = ExternalTrace.generate_request_headers(transaction)
         assert payload
+        # Ensure trusted account key or account ID present as vendor
+        assert dict(payload)["tracestate"].startswith("1@nr=")
 
-    _test_dt_outbound()
+    _test_outbound_dt_payload_generation()
 
 
-def test_dt_inbound(serverless_application):
-    @override_generic_settings(serverless_application.settings, {
-        'distributed_tracing.enabled': True,
-        'account_id': '1',
-        'trusted_account_key': '1',
-        'primary_application_id': '1',
-    })
-    @background_task(
-            application=serverless_application,
-            name='test_dt_inbound')
-    def _test_dt_inbound():
+@pytest.mark.parametrize("trusted_account_key", ("1", None), ids=("tk_set", "tk_unset"))
+def test_inbound_dt_payload_acceptance(serverless_application, trusted_account_key):
+    @override_generic_settings(
+        serverless_application.settings,
+        {
+            "distributed_tracing.enabled": True,
+            "account_id": "1",
+            "trusted_account_key": trusted_account_key,
+            "primary_application_id": "1",
+        },
+    )
+    @background_task(application=serverless_application, name="test_inbound_dt_payload_acceptance")
+    def _test_inbound_dt_payload_acceptance():
         transaction = current_transaction()
 
         payload = {
-            'v': [0, 1],
-            'd': {
-                'ty': 'Mobile',
-                'ac': '1',
-                'tk': '1',
-                'ap': '2827902',
-                'pa': '5e5733a911cfbc73',
-                'id': '7d3efb1b173fecfa',
-                'tr': 'd6b4ba0c3a712ca',
-                'ti': 1518469636035,
-                'tx': '8703ff3d88eefe9d',
-            }
+            "v": [0, 1],
+            "d": {
+                "ty": "Mobile",
+                "ac": "1",
+                "tk": "1",
+                "ap": "2827902",
+                "pa": "5e5733a911cfbc73",
+                "id": "7d3efb1b173fecfa",
+                "tr": "d6b4ba0c3a712ca",
+                "ti": 1518469636035,
+                "tx": "8703ff3d88eefe9d",
+            },
         }
 
         result = transaction.accept_distributed_trace_payload(payload)
         assert result
 
-    _test_dt_inbound()
+    _test_inbound_dt_payload_acceptance()
 
 
-@pytest.mark.parametrize('arn_set', (True, False))
+@pytest.mark.parametrize("arn_set", (True, False))
 def test_payload_metadata_arn(serverless_application, arn_set):
-
     # If the session object gathers the arn from the settings object before the
     # lambda handler records it there, then this test will fail.
 
     settings = global_settings()
     original_metadata = settings.aws_lambda_metadata.copy()
 
     arn = None
     if arn_set:
-        arn = 'arrrrrrrrrrRrrrrrrrn'
+        arn = "arrrrrrrrrrRrrrrrrrn"
 
-    settings.aws_lambda_metadata.update({'arn': arn, 'function_version': '$LATEST'})
+    settings.aws_lambda_metadata.update({"arn": arn, "function_version": "$LATEST"})
 
     class Context(object):
         invoked_function_arn = arn
 
-    @validate_serverless_metadata(exact_metadata={'arn': arn})
+    @validate_serverless_metadata(exact_metadata={"arn": arn})
     @lambda_handler(application=serverless_application)
     def handler(event, context):
-        assert settings.aws_lambda_metadata['arn'] == arn
+        assert settings.aws_lambda_metadata["arn"] == arn
         return {}
 
     try:
         handler({}, Context)
     finally:
         settings.aws_lambda_metadata = original_metadata
```

### Comparing `newrelic-8.8.1/tests/agent_features/test_span_events.py` & `newrelic-8.9.0/tests/agent_features/test_span_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_stack_trace.py` & `newrelic-8.9.0/tests/agent_features/test_stack_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_supportability_metrics.py` & `newrelic-8.9.0/tests/agent_features/test_supportability_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_synthetics.py` & `newrelic-8.9.0/tests/agent_features/test_synthetics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_time_trace.py` & `newrelic-8.9.0/tests/agent_features/test_time_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py` & `newrelic-8.9.0/tests/agent_features/test_transaction_event_data_and_some_browser_stuff_too.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_transaction_name.py` & `newrelic-8.9.0/tests/agent_features/test_transaction_name.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_transaction_trace_segments.py` & `newrelic-8.9.0/tests/agent_features/test_transaction_trace_segments.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_w3c_trace_context.py` & `newrelic-8.9.0/tests/agent_features/test_w3c_trace_context.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_web_transaction.py` & `newrelic-8.9.0/tests/agent_features/test_web_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_features/test_wsgi_attributes.py` & `newrelic-8.9.0/tests/agent_features/test_wsgi_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_streaming/_test_handler.py` & `newrelic-8.9.0/tests/agent_streaming/_test_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_streaming/conftest.py` & `newrelic-8.9.0/tests/agent_streaming/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_streaming/test_infinite_tracing.py` & `newrelic-8.9.0/tests/agent_streaming/test_infinite_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_streaming/test_span_events.py` & `newrelic-8.9.0/tests/agent_streaming/test_span_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_streaming/test_stream_buffer.py` & `newrelic-8.9.0/tests/agent_streaming/test_stream_buffer.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_streaming/test_streaming_rpc.py` & `newrelic-8.9.0/tests/agent_streaming/test_streaming_rpc.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/_test_import_hook.py` & `newrelic-8.9.0/tests/agent_unittests/_test_import_hook.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/cert.pem` & `newrelic-8.9.0/tests/agent_unittests/cert.pem`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/conftest.py` & `newrelic-8.9.0/tests/agent_unittests/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_agent.py` & `newrelic-8.9.0/tests/agent_unittests/test_agent.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_agent_connect.py` & `newrelic-8.9.0/tests/agent_unittests/test_agent_connect.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_agent_protocol.py` & `newrelic-8.9.0/tests/agent_unittests/test_agent_protocol.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_check_environment.py` & `newrelic-8.9.0/tests/agent_unittests/test_check_environment.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_connect_response_fields.py` & `newrelic-8.9.0/tests/agent_unittests/test_connect_response_fields.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_distributed_tracing_settings.py` & `newrelic-8.9.0/tests/agent_unittests/test_distributed_tracing_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_environment.py` & `newrelic-8.9.0/tests/agent_unittests/test_environment.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_full_uri_payloads.py` & `newrelic-8.9.0/tests/agent_unittests/test_full_uri_payloads.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_harvest_loop.py` & `newrelic-8.9.0/tests/agent_unittests/test_harvest_loop.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_http_client.py` & `newrelic-8.9.0/tests/agent_unittests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_import_hook.py` & `newrelic-8.9.0/tests/agent_unittests/test_import_hook.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_infinite_trace_settings.py` & `newrelic-8.9.0/tests/agent_unittests/test_infinite_trace_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_package_version_utils.py` & `newrelic-8.9.0/tests/agent_unittests/test_package_version_utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_region_aware_settings.py` & `newrelic-8.9.0/tests/agent_unittests/test_region_aware_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_sampler_metrics.py` & `newrelic-8.9.0/tests/agent_unittests/test_sampler_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_serverless_mode_settings.py` & `newrelic-8.9.0/tests/agent_unittests/test_serverless_mode_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_signature.py` & `newrelic-8.9.0/tests/agent_unittests/test_signature.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_trace_cache.py` & `newrelic-8.9.0/tests/agent_unittests/test_trace_cache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/agent_unittests/test_utilization_settings.py` & `newrelic-8.9.0/tests/agent_unittests/test_utilization_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/application_celery/conftest.py` & `newrelic-8.9.0/tests/application_celery/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/application_celery/tasks.py` & `newrelic-8.9.0/tests/application_celery/tasks.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/application_celery/test_celery.py` & `newrelic-8.9.0/tests/application_celery/test_celery.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/application_celery/test_celery_max_tasks_per_child.py` & `newrelic-8.9.0/tests/application_celery/test_celery_max_tasks_per_child.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/application_gearman/conftest.py` & `newrelic-8.9.0/tests/application_gearman/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/application_gearman/test_gearman.py` & `newrelic-8.9.0/tests/application_gearman/test_gearman.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_djangorestframework/conftest.py` & `newrelic-8.9.0/tests/component_djangorestframework/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_djangorestframework/settings.py` & `newrelic-8.9.0/tests/component_djangorestframework/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_djangorestframework/test_application.py` & `newrelic-8.9.0/tests/component_djangorestframework/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_djangorestframework/urls.py` & `newrelic-8.9.0/tests/component_djangorestframework/urls.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_djangorestframework/views.py` & `newrelic-8.9.0/tests/component_djangorestframework/views.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_djangorestframework/wsgi.py` & `newrelic-8.9.0/tests/component_djangorestframework/wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_flask_rest/_test_application.py` & `newrelic-8.9.0/tests/component_flask_rest/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_flask_rest/conftest.py` & `newrelic-8.9.0/tests/component_flask_rest/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_flask_rest/test_application.py` & `newrelic-8.9.0/tests/component_flask_rest/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_graphqlserver/_test_graphql.py` & `newrelic-8.9.0/tests/component_graphqlserver/_test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_graphqlserver/conftest.py` & `newrelic-8.9.0/tests/component_graphqlserver/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_graphqlserver/test_graphql.py` & `newrelic-8.9.0/tests/component_graphqlserver/test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_tastypie/api.py` & `newrelic-8.9.0/tests/component_tastypie/api.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_tastypie/conftest.py` & `newrelic-8.9.0/tests/component_tastypie/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_tastypie/settings.py` & `newrelic-8.9.0/tests/component_tastypie/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_tastypie/test_application.py` & `newrelic-8.9.0/tests/component_tastypie/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_tastypie/urls.py` & `newrelic-8.9.0/tests/component_tastypie/urls.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_tastypie/views.py` & `newrelic-8.9.0/tests/component_tastypie/views.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/component_tastypie/wsgi.py` & `newrelic-8.9.0/tests/component_tastypie/wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/coroutines_asyncio/conftest.py` & `newrelic-8.9.0/tests/coroutines_asyncio/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/coroutines_asyncio/test_context_propagation.py` & `newrelic-8.9.0/tests/coroutines_asyncio/test_context_propagation.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/conftest.py` & `newrelic-8.9.0/tests/cross_agent/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/README.md` & `newrelic-8.9.0/tests/cross_agent/fixtures/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/attribute_configuration.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/attribute_configuration.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/cat_map.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/cat_map.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/collector_hostname.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/collector_hostname.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/datastores/README.md` & `newrelic-8.9.0/tests/cross_agent/fixtures/datastores/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/datastores/datastore_instances.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/datastores/datastore_instances.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/README.md` & `newrelic-8.9.0/tests/cross_agent/fixtures/distributed_tracing/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/distributed_tracing/distributed_tracing.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/distributed_tracing/trace_context.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/distributed_tracing/trace_context.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/cases.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/cases.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.0.0.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-lxc-driver.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-fs.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.1.2-native-driver-systemd.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-1.3.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-custom-prefix.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/docker-too-long.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/docker_container_id/invalid-characters.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/labels.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/labels.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_end_session.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_intent_answer.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/alexa_start_session.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/api_gateway_proxy.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_ab.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_access_request_header.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_modify.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_multi_remote.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_redirect.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/cloudfront_simple_remote.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/codecommit.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/codecommit.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/codepipeline.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/config_change_oversized.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/config_change_triggered.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/config_periodic.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/dynamodb_update.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/firehose_stream_source.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/firehose_syslog.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/kinesis_firehose.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/rekognition_s3.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/s3_delete.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/s3_put.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/s3_put.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/ses.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/ses.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/sns.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/sns.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source/sqs.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source/sqs.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/lambda_event_source.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/lambda_event_source.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md` & `newrelic-8.9.0/tests/cross_agent/fixtures/postgres_explain_obfuscation/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/1pack_4core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_12core_24logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_20core_40logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_2logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_2core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/2pack_4core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/4pack_4core_4logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/8pack_8core_8logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/README.md` & `newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/proc_cpuinfo/Xpack_Xcore_2logical.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt` & `newrelic-8.9.0/tests/cross_agent/fixtures/proc_meminfo/meminfo_4096MB.txt`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rules.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/rules.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_client_config.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_client_config.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_cookie.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_cookie.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_footer_insertion_location/close-body-in-comment.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_footer_insertion_location/close-body-in-comment.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_footer_insertion_location/dynamic-iframe.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_footer_insertion_location/dynamic-iframe.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/basic.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/body_with_attributes.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_after_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_before_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/charset_tag_with_spaces.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments1.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/comments2.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_after_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/content_type_charset_tag_before_x_ua_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes1.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes2.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_quotes_mismatch.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes1.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/gt_in_single_quotes_mismatch.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/head_with_attributes.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/incomplete_non_meta_tags.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_end_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_html_and_no_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/no_start_header.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script1.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/script2.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiline.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_multiple_tags.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_spaces_around_equals.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_others.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html` & `newrelic-8.9.0/tests/cross_agent/fixtures/rum_loader_insertion_location/x_ua_meta_tag_with_spaces.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/README.md` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/back_quoted_identifiers.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/comment_delimiters_in_strings.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/double_quoted_identifiers.postgres.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_line_comment_in_string.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_cstyle.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_doubledash.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/end_of_query_comment_hash.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/escape_string_constants.postgres.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_double_quoted_string.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/malformed/unterminated_single_quoted_string.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/multiple_literal_types.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/numbers_in_identifiers.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/numeric_literals.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/end_of_line_comments_with_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_comments_and_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_comments_and_newlines.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/mixed_quotes_end_of_line_comments.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/pathological/quote_delimiters_in_comments.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/sql_obfuscation.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_double_quoted.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_single_quoted.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_backslash_and_twin_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_double_quote.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_newline.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_embedded_single_quote.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_escaped_quotes.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_backslash.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash.mysql.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_backslash_single_quoted.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_trailing_escaped_quote.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_obfuscation/string_with_twin_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/sql_parsing.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/sql_parsing.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/transaction_segment_terms.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/transaction_segment_terms.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/url_clean.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/url_clean.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/url_domain_extraction.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/url_domain_extraction.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/utilization/README.md` & `newrelic-8.9.0/tests/cross_agent/fixtures/utilization/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/utilization/boot_id.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/utilization/boot_id.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/utilization/utilization_json.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/utilization/utilization_json.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/README.md` & `newrelic-8.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/README.md`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/aws.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/azure.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/gcp.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json` & `newrelic-8.9.0/tests/cross_agent/fixtures/utilization_vendor_specific/pcf.json`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_agent_attributes.py` & `newrelic-8.9.0/tests/cross_agent/test_agent_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_aws_utilization_data.py` & `newrelic-8.9.0/tests/cross_agent/test_aws_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_azure_utilization_data.py` & `newrelic-8.9.0/tests/cross_agent/test_azure_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_boot_id_utilization_data.py` & `newrelic-8.9.0/tests/cross_agent/test_boot_id_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_cat_map.py` & `newrelic-8.9.0/tests/cross_agent/test_cat_map.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_collector_hostname.py` & `newrelic-8.9.0/tests/cross_agent/test_collector_hostname.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_datstore_instance.py` & `newrelic-8.9.0/tests/cross_agent/test_datstore_instance.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_distributed_tracing.py` & `newrelic-8.9.0/tests/cross_agent/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_docker.py` & `newrelic-8.9.0/tests/cross_agent/test_docker.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_gcp_utilization_data.py` & `newrelic-8.9.0/tests/cross_agent/test_gcp_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_labels_and_rollups.py` & `newrelic-8.9.0/tests/cross_agent/test_labels_and_rollups.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_lambda_event_source.py` & `newrelic-8.9.0/tests/cross_agent/test_lambda_event_source.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_pcf_utilization_data.py` & `newrelic-8.9.0/tests/cross_agent/test_pcf_utilization_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_rules.py` & `newrelic-8.9.0/tests/cross_agent/test_rules.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_rum_client_config.py` & `newrelic-8.9.0/tests/cross_agent/test_rum_client_config.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_sql_obfuscation.py` & `newrelic-8.9.0/tests/cross_agent/test_sql_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_system_info.py` & `newrelic-8.9.0/tests/cross_agent/test_system_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_transaction_segment_terms.py` & `newrelic-8.9.0/tests/cross_agent/test_transaction_segment_terms.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_utilization_configs.py` & `newrelic-8.9.0/tests/cross_agent/test_utilization_configs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/cross_agent/test_w3c_trace_context.py` & `newrelic-8.9.0/tests/cross_agent/test_w3c_trace_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,244 +10,263 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
+
 import pytest
 import webtest
-from newrelic.packages import six
-
-from newrelic.api.transaction import current_transaction
+from testing_support.fixtures import override_application_settings, validate_attributes
+from testing_support.validators.validate_span_events import validate_span_events
+from testing_support.validators.validate_transaction_event_attributes import (
+    validate_transaction_event_attributes,
+)
+from testing_support.validators.validate_transaction_metrics import (
+    validate_transaction_metrics,
+)
+
+from newrelic.api.transaction import (
+    accept_distributed_trace_headers,
+    current_transaction,
+    insert_distributed_trace_headers,
+)
 from newrelic.api.wsgi_application import wsgi_application
-from newrelic.common.object_wrapper import transient_function_wrapper
-from testing_support.validators.validate_span_events import (
-        validate_span_events)
-from testing_support.fixtures import (override_application_settings,
-        validate_attributes)
 from newrelic.common.encoding_utils import W3CTraceState
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
-from testing_support.validators.validate_transaction_event_attributes import validate_transaction_event_attributes
+from newrelic.common.object_wrapper import transient_function_wrapper
+from newrelic.packages import six
 
 CURRENT_DIR = os.path.dirname(os.path.realpath(__file__))
-JSON_DIR = os.path.normpath(os.path.join(CURRENT_DIR, 'fixtures',
-    'distributed_tracing'))
+JSON_DIR = os.path.normpath(os.path.join(CURRENT_DIR, "fixtures", "distributed_tracing"))
 
-_parameters_list = ('test_name', 'trusted_account_key', 'account_id',
-        'web_transaction', 'raises_exception', 'force_sampled_true',
-        'span_events_enabled', 'transport_type', 'inbound_headers',
-        'outbound_payloads', 'intrinsics', 'expected_metrics')
+_parameters_list = (
+    "test_name",
+    "trusted_account_key",
+    "account_id",
+    "web_transaction",
+    "raises_exception",
+    "force_sampled_true",
+    "span_events_enabled",
+    "transport_type",
+    "inbound_headers",
+    "outbound_payloads",
+    "intrinsics",
+    "expected_metrics",
+)
 
-_parameters = ','.join(_parameters_list)
+_parameters = ",".join(_parameters_list)
 
 
 XFAIL_TESTS = [
-    'spans_disabled_root',
-    'missing_traceparent',
-    'missing_traceparent_and_tracestate',
-    'w3c_and_newrelc_headers_present_error_parsing_traceparent'
+    "spans_disabled_root",
+    "missing_traceparent",
+    "missing_traceparent_and_tracestate",
+    "w3c_and_newrelc_headers_present_error_parsing_traceparent",
 ]
 
+
 def load_tests():
     result = []
-    path = os.path.join(JSON_DIR, 'trace_context.json')
-    with open(path, 'r') as fh:
+    path = os.path.join(JSON_DIR, "trace_context.json")
+    with open(path, "r") as fh:
         tests = json.load(fh)
 
     for test in tests:
         values = (test.get(param, None) for param in _parameters_list)
-        param = pytest.param(*values, id=test.get('test_name'))
+        param = pytest.param(*values, id=test.get("test_name"))
         result.append(param)
 
     return result
 
 
 ATTR_MAP = {
-    'traceparent.version': 0,
-    'traceparent.trace_id': 1,
-    'traceparent.parent_id': 2,
-    'traceparent.trace_flags': 3,
-    'tracestate.version': 0,
-    'tracestate.parent_type': 1,
-    'tracestate.parent_account_id': 2,
-    'tracestate.parent_application_id': 3,
-    'tracestate.span_id': 4,
-    'tracestate.transaction_id': 5,
-    'tracestate.sampled': 6,
-    'tracestate.priority': 7,
-    'tracestate.timestamp': 8,
-    'tracestate.tenant_id': None,
+    "traceparent.version": 0,
+    "traceparent.trace_id": 1,
+    "traceparent.parent_id": 2,
+    "traceparent.trace_flags": 3,
+    "tracestate.version": 0,
+    "tracestate.parent_type": 1,
+    "tracestate.parent_account_id": 2,
+    "tracestate.parent_application_id": 3,
+    "tracestate.span_id": 4,
+    "tracestate.transaction_id": 5,
+    "tracestate.sampled": 6,
+    "tracestate.priority": 7,
+    "tracestate.timestamp": 8,
+    "tracestate.tenant_id": None,
 }
 
 
 def validate_outbound_payload(actual, expected, trusted_account_key):
-    traceparent = ''
-    tracestate = ''
+    traceparent = ""
+    tracestate = ""
     for key, value in actual:
-        if key == 'traceparent':
-            traceparent = value.split('-')
-        elif key == 'tracestate':
+        if key == "traceparent":
+            traceparent = value.split("-")
+        elif key == "tracestate":
             vendors = W3CTraceState.decode(value)
-            nr_entry = vendors.pop(trusted_account_key + '@nr', '')
-            tracestate = nr_entry.split('-')
-    exact_values = expected.get('exact', {})
-    expected_attrs = expected.get('expected', [])
-    unexpected_attrs = expected.get('unexpected', [])
-    expected_vendors = expected.get('vendors', [])
+            nr_entry = vendors.pop(trusted_account_key + "@nr", "")
+            tracestate = nr_entry.split("-")
+    exact_values = expected.get("exact", {})
+    expected_attrs = expected.get("expected", [])
+    unexpected_attrs = expected.get("unexpected", [])
+    expected_vendors = expected.get("vendors", [])
     for key, value in exact_values.items():
-        header = traceparent if key.startswith('traceparent.') else tracestate
+        header = traceparent if key.startswith("traceparent.") else tracestate
         attr = ATTR_MAP[key]
         if attr is not None:
             if isinstance(value, bool):
                 assert header[attr] == str(int(value))
             elif isinstance(value, int):
                 assert int(header[attr]) == value
             else:
                 assert header[attr] == str(value)
 
     for key in expected_attrs:
-        header = traceparent if key.startswith('traceparent.') else tracestate
+        header = traceparent if key.startswith("traceparent.") else tracestate
         attr = ATTR_MAP[key]
         if attr is not None:
             assert header[attr], key
 
     for key in unexpected_attrs:
-        header = traceparent if key.startswith('traceparent.') else tracestate
+        header = traceparent if key.startswith("traceparent.") else tracestate
         attr = ATTR_MAP[key]
         if attr is not None:
             assert not header[attr], key
 
     for vendor in expected_vendors:
         assert vendor in vendors
 
 
 @wsgi_application()
 def target_wsgi_application(environ, start_response):
     transaction = current_transaction()
 
-    if not environ['.web_transaction']:
+    if not environ[".web_transaction"]:
         transaction.background_task = True
 
-    if environ['.raises_exception']:
+    if environ[".raises_exception"]:
         try:
             raise ValueError("oops")
         except:
             transaction.notice_error()
 
-    if '.inbound_headers' in environ:
-        transaction.accept_distributed_trace_headers(
-            environ['.inbound_headers'],
-            transport_type=environ['.transport_type'],
+    if ".inbound_headers" in environ:
+        accept_distributed_trace_headers(
+            environ[".inbound_headers"],
+            transport_type=environ[".transport_type"],
         )
 
     payloads = []
-    for _ in range(environ['.outbound_calls']):
+    for _ in range(environ[".outbound_calls"]):
         payloads.append([])
-        transaction.insert_distributed_trace_headers(payloads[-1])
+        insert_distributed_trace_headers(payloads[-1])
 
-    start_response('200 OK', [('Content-Type', 'application/json')])
-    return [json.dumps(payloads).encode('utf-8')]
+    start_response("200 OK", [("Content-Type", "application/json")])
+    return [json.dumps(payloads).encode("utf-8")]
 
 
 test_application = webtest.TestApp(target_wsgi_application)
 
 
 def override_compute_sampled(override):
-    @transient_function_wrapper('newrelic.core.adaptive_sampler',
-            'AdaptiveSampler.compute_sampled')
+    @transient_function_wrapper("newrelic.core.adaptive_sampler", "AdaptiveSampler.compute_sampled")
     def _override_compute_sampled(wrapped, instance, args, kwargs):
         if override:
             return True
         return wrapped(*args, **kwargs)
+
     return _override_compute_sampled
 
 
 @pytest.mark.parametrize(_parameters, load_tests())
-def test_trace_context(test_name, trusted_account_key, account_id,
-        web_transaction, raises_exception, force_sampled_true,
-        span_events_enabled, transport_type, inbound_headers,
-        outbound_payloads, intrinsics, expected_metrics):
-
+def test_trace_context(
+    test_name,
+    trusted_account_key,
+    account_id,
+    web_transaction,
+    raises_exception,
+    force_sampled_true,
+    span_events_enabled,
+    transport_type,
+    inbound_headers,
+    outbound_payloads,
+    intrinsics,
+    expected_metrics,
+):
     if test_name in XFAIL_TESTS:
         pytest.xfail("Waiting on cross agent tests update.")
     # Prepare assertions
     if not intrinsics:
         intrinsics = {}
 
-    common = intrinsics.get('common', {})
-    common_required = common.get('expected', [])
-    common_forgone = common.get('unexpected', [])
-    common_exact = common.get('exact', {})
-
-    txn_intrinsics = intrinsics.get('Transaction', {})
-    txn_event_required = {'agent': [], 'user': [],
-            'intrinsic': txn_intrinsics.get('expected', [])}
-    txn_event_required['intrinsic'].extend(common_required)
-    txn_event_forgone = {'agent': [], 'user': [],
-            'intrinsic': txn_intrinsics.get('unexpected', [])}
-    txn_event_forgone['intrinsic'].extend(common_forgone)
-    txn_event_exact = {'agent': {}, 'user': {},
-            'intrinsic': txn_intrinsics.get('exact', {})}
-    txn_event_exact['intrinsic'].update(common_exact)
+    common = intrinsics.get("common", {})
+    common_required = common.get("expected", [])
+    common_forgone = common.get("unexpected", [])
+    common_exact = common.get("exact", {})
+
+    txn_intrinsics = intrinsics.get("Transaction", {})
+    txn_event_required = {"agent": [], "user": [], "intrinsic": txn_intrinsics.get("expected", [])}
+    txn_event_required["intrinsic"].extend(common_required)
+    txn_event_forgone = {"agent": [], "user": [], "intrinsic": txn_intrinsics.get("unexpected", [])}
+    txn_event_forgone["intrinsic"].extend(common_forgone)
+    txn_event_exact = {"agent": {}, "user": {}, "intrinsic": txn_intrinsics.get("exact", {})}
+    txn_event_exact["intrinsic"].update(common_exact)
 
     override_settings = {
-        'distributed_tracing.enabled': True,
-        'span_events.enabled': span_events_enabled,
-        'account_id': account_id,
-        'trusted_account_key': trusted_account_key,
+        "distributed_tracing.enabled": True,
+        "span_events.enabled": span_events_enabled,
+        "account_id": account_id,
+        "trusted_account_key": trusted_account_key,
     }
 
     extra_environ = {
-        '.web_transaction': web_transaction,
-        '.raises_exception': raises_exception,
-        '.transport_type': transport_type,
-        '.outbound_calls': outbound_payloads and len(outbound_payloads) or 0,
+        ".web_transaction": web_transaction,
+        ".raises_exception": raises_exception,
+        ".transport_type": transport_type,
+        ".outbound_calls": outbound_payloads and len(outbound_payloads) or 0,
     }
 
     inbound_headers = inbound_headers and inbound_headers[0] or None
-    if transport_type != 'HTTP':
-        extra_environ['.inbound_headers'] = inbound_headers
+    if transport_type != "HTTP":
+        extra_environ[".inbound_headers"] = inbound_headers
         inbound_headers = None
     elif six.PY2 and inbound_headers:
-        inbound_headers = {
-                k.encode('utf-8'): v.encode('utf-8')
-                for k, v in inbound_headers.items()}
-
-    @validate_transaction_metrics(test_name,
-            group="Uri",
-            rollup_metrics=expected_metrics,
-            background_task=not web_transaction)
-    @validate_transaction_event_attributes(
-            txn_event_required, txn_event_forgone, txn_event_exact)
-    @validate_attributes('intrinsic', common_required, common_forgone)
+        inbound_headers = {k.encode("utf-8"): v.encode("utf-8") for k, v in inbound_headers.items()}
+
+    @validate_transaction_metrics(
+        test_name, group="Uri", rollup_metrics=expected_metrics, background_task=not web_transaction
+    )
+    @validate_transaction_event_attributes(txn_event_required, txn_event_forgone, txn_event_exact)
+    @validate_attributes("intrinsic", common_required, common_forgone)
     @override_application_settings(override_settings)
     @override_compute_sampled(force_sampled_true)
     def _test():
         return test_application.get(
-            '/' + test_name,
+            "/" + test_name,
             headers=inbound_headers,
             extra_environ=extra_environ,
         )
 
-    if 'Span' in intrinsics:
-        span_intrinsics = intrinsics.get('Span')
-        span_expected = span_intrinsics.get('expected', [])
+    if "Span" in intrinsics:
+        span_intrinsics = intrinsics.get("Span")
+        span_expected = span_intrinsics.get("expected", [])
         span_expected.extend(common_required)
-        span_unexpected = span_intrinsics.get('unexpected', [])
+        span_unexpected = span_intrinsics.get("unexpected", [])
         span_unexpected.extend(common_forgone)
-        span_exact = span_intrinsics.get('exact', {})
+        span_exact = span_intrinsics.get("exact", {})
         span_exact.update(common_exact)
 
-        _test = validate_span_events(exact_intrinsics=span_exact,
-            expected_intrinsics=span_expected,
-            unexpected_intrinsics=span_unexpected)(_test)
+        _test = validate_span_events(
+            exact_intrinsics=span_exact, expected_intrinsics=span_expected, unexpected_intrinsics=span_unexpected
+        )(_test)
     elif not span_events_enabled:
         _test = validate_span_events(count=0)(_test)
 
     response = _test()
-    assert response.status == '200 OK'
+    assert response.status == "200 OK"
     payloads = response.json
     if outbound_payloads:
         assert len(payloads) == len(outbound_payloads)
         for actual, expected in zip(payloads, outbound_payloads):
             validate_outbound_payload(actual, expected, trusted_account_key)
```

### Comparing `newrelic-8.8.1/tests/datastore_aioredis/conftest.py` & `newrelic-8.9.0/tests/datastore_aioredis/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aioredis/test_custom_conn_pool.py` & `newrelic-8.9.0/tests/datastore_aioredis/test_custom_conn_pool.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aioredis/test_execute_command.py` & `newrelic-8.9.0/tests/datastore_aioredis/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aioredis/test_get_and_set.py` & `newrelic-8.9.0/tests/datastore_aioredis/test_get_and_set.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aioredis/test_instance_info.py` & `newrelic-8.9.0/tests/datastore_aioredis/test_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aioredis/test_multiple_dbs.py` & `newrelic-8.9.0/tests/datastore_aioredis/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aioredis/test_span_event.py` & `newrelic-8.9.0/tests/datastore_aioredis/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aioredis/test_trace_node.py` & `newrelic-8.9.0/tests/datastore_aioredis/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aioredis/test_transactions.py` & `newrelic-8.9.0/tests/datastore_aioredis/test_transactions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aioredis/test_uninstrumented_methods.py` & `newrelic-8.9.0/tests/datastore_aioredis/test_uninstrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aredis/conftest.py` & `newrelic-8.9.0/tests/datastore_aredis/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aredis/test_custom_conn_pool.py` & `newrelic-8.9.0/tests/datastore_aredis/test_custom_conn_pool.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aredis/test_execute_command.py` & `newrelic-8.9.0/tests/datastore_aredis/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aredis/test_get_and_set.py` & `newrelic-8.9.0/tests/datastore_aredis/test_get_and_set.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aredis/test_instance_info.py` & `newrelic-8.9.0/tests/datastore_aredis/test_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aredis/test_multiple_dbs.py` & `newrelic-8.9.0/tests/datastore_aredis/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aredis/test_span_event.py` & `newrelic-8.9.0/tests/datastore_aredis/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aredis/test_trace_node.py` & `newrelic-8.9.0/tests/datastore_aredis/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_aredis/test_uninstrumented_methods.py` & `newrelic-8.9.0/tests/datastore_aredis/test_uninstrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_asyncpg/conftest.py` & `newrelic-8.9.0/tests/datastore_asyncpg/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_asyncpg/test_multiple_dbs.py` & `newrelic-8.9.0/tests/datastore_asyncpg/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_asyncpg/test_query.py` & `newrelic-8.9.0/tests/datastore_asyncpg/test_query.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_bmemcached/conftest.py` & `newrelic-8.9.0/tests/datastore_bmemcached/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_bmemcached/test_memcache.py` & `newrelic-8.9.0/tests/datastore_bmemcached/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_elasticsearch/conftest.py` & `newrelic-8.9.0/tests/datastore_elasticsearch/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_elasticsearch/test_connection.py` & `newrelic-8.9.0/tests/datastore_elasticsearch/test_connection.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_elasticsearch/test_database_duration.py` & `newrelic-8.9.0/tests/datastore_elasticsearch/test_database_duration.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_elasticsearch/test_elasticsearch.py` & `newrelic-8.9.0/tests/datastore_elasticsearch/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_elasticsearch/test_instrumented_methods.py` & `newrelic-8.9.0/tests/datastore_elasticsearch/test_instrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_elasticsearch/test_mget.py` & `newrelic-8.9.0/tests/datastore_elasticsearch/test_mget.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_elasticsearch/test_multiple_dbs.py` & `newrelic-8.9.0/tests/datastore_elasticsearch/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_elasticsearch/test_trace_node.py` & `newrelic-8.9.0/tests/datastore_elasticsearch/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_elasticsearch/test_transport.py` & `newrelic-8.9.0/tests/datastore_elasticsearch/test_transport.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_memcache/conftest.py` & `newrelic-8.9.0/tests/datastore_memcache/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_memcache/test_all_methods_wrapped.py` & `newrelic-8.9.0/tests/datastore_memcache/test_all_methods_wrapped.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_memcache/test_memcache.py` & `newrelic-8.9.0/tests/datastore_memcache/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_memcache/test_multiple_dbs.py` & `newrelic-8.9.0/tests/datastore_memcache/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_memcache/test_span_event.py` & `newrelic-8.9.0/tests/datastore_memcache/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_mysql/conftest.py` & `newrelic-8.9.0/tests/datastore_mysql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_mysql/test_database.py` & `newrelic-8.9.0/tests/datastore_mysql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_postgresql/conftest.py` & `newrelic-8.9.0/tests/datastore_postgresql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_postgresql/test_database.py` & `newrelic-8.9.0/tests/datastore_postgresql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/conftest.py` & `newrelic-8.9.0/tests/datastore_psycopg2/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_as_string.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_as_string.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_async.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_cursor.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_cursor.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_database_instance_info.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_database_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_explain_plans.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_explain_plans.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_forward_compat.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_forward_compat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_multiple_dbs.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_obfuscation.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_register.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_register.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_rollback.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_rollback.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_slow_sql.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_slow_sql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_span_event.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/test_trace_node.py` & `newrelic-8.9.0/tests/datastore_psycopg2/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2/utils.py` & `newrelic-8.9.0/tests/datastore_psycopg2/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2cffi/conftest.py` & `newrelic-8.9.0/tests/datastore_psycopg2cffi/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2cffi/test_database.py` & `newrelic-8.9.0/tests/datastore_psycopg2cffi/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_psycopg2cffi/test_explain_plans.py` & `newrelic-8.9.0/tests/datastore_psycopg2cffi/test_explain_plans.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_pylibmc/conftest.py` & `newrelic-8.9.0/tests/datastore_pylibmc/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_pylibmc/test_memcache.py` & `newrelic-8.9.0/tests/datastore_pylibmc/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_pymemcache/conftest.py` & `newrelic-8.9.0/tests/datastore_pymemcache/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_pymemcache/test_memcache.py` & `newrelic-8.9.0/tests/datastore_pymemcache/test_memcache.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_pymongo/conftest.py` & `newrelic-8.9.0/tests/datastore_pymongo/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_pymongo/test_pymongo.py` & `newrelic-8.9.0/tests/datastore_pymongo/test_pymongo.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_pymysql/conftest.py` & `newrelic-8.9.0/tests/datastore_pymysql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_pymysql/test_database.py` & `newrelic-8.9.0/tests/datastore_pymysql/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_pyodbc/conftest.py` & `newrelic-8.9.0/tests/datastore_pyodbc/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_pyodbc/test_pyodbc.py` & `newrelic-8.9.0/tests/datastore_pyodbc/test_pyodbc.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_pysolr/conftest.py` & `newrelic-8.9.0/tests/datastore_pysolr/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_pysolr/test_solr.py` & `newrelic-8.9.0/tests/datastore_pysolr/test_solr.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_redis/conftest.py` & `newrelic-8.9.0/tests/datastore_redis/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_redis/test_custom_conn_pool.py` & `newrelic-8.9.0/tests/datastore_redis/test_custom_conn_pool.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_redis/test_execute_command.py` & `newrelic-8.9.0/tests/datastore_redis/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_redis/test_get_and_set.py` & `newrelic-8.9.0/tests/datastore_redis/test_get_and_set.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_redis/test_instance_info.py` & `newrelic-8.9.0/tests/datastore_redis/test_instance_info.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_redis/test_multiple_dbs.py` & `newrelic-8.9.0/tests/datastore_redis/test_multiple_dbs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_redis/test_rb.py` & `newrelic-8.9.0/tests/datastore_redis/test_rb.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_redis/test_span_event.py` & `newrelic-8.9.0/tests/datastore_redis/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_redis/test_trace_node.py` & `newrelic-8.9.0/tests/datastore_redis/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_redis/test_uninstrumented_methods.py` & `newrelic-8.9.0/tests/datastore_redis/test_uninstrumented_methods.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_solrpy/conftest.py` & `newrelic-8.9.0/tests/datastore_solrpy/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_solrpy/test_solr.py` & `newrelic-8.9.0/tests/datastore_solrpy/test_solr.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_sqlite/conftest.py` & `newrelic-8.9.0/tests/datastore_sqlite/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_sqlite/test_database.py` & `newrelic-8.9.0/tests/datastore_sqlite/test_database.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/datastore_sqlite/test_obfuscation.py` & `newrelic-8.9.0/tests/datastore_sqlite/test_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_boto3/conftest.py` & `newrelic-8.9.0/tests/external_boto3/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_boto3/test_boto3_iam.py` & `newrelic-8.9.0/tests/external_boto3/test_boto3_iam.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_boto3/test_boto3_s3.py` & `newrelic-8.9.0/tests/external_boto3/test_boto3_s3.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_boto3/test_boto3_sns.py` & `newrelic-8.9.0/tests/external_boto3/test_boto3_sns.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_botocore/conftest.py` & `newrelic-8.9.0/tests/external_botocore/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_botocore/test_botocore_dynamodb.py` & `newrelic-8.9.0/tests/external_botocore/test_botocore_dynamodb.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_botocore/test_botocore_ec2.py` & `newrelic-8.9.0/tests/external_botocore/test_botocore_ec2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_botocore/test_botocore_s3.py` & `newrelic-8.9.0/tests/external_botocore/test_botocore_s3.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_botocore/test_botocore_sqs.py` & `newrelic-8.9.0/tests/external_botocore/test_botocore_sqs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_feedparser/conftest.py` & `newrelic-8.9.0/tests/external_feedparser/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_feedparser/packages.xml` & `newrelic-8.9.0/tests/external_feedparser/packages.xml`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_feedparser/test_feedparser.py` & `newrelic-8.9.0/tests/external_feedparser/test_feedparser.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_http/conftest.py` & `newrelic-8.9.0/tests/external_http/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_http/test_http.py` & `newrelic-8.9.0/tests/external_http/test_http.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_httplib/conftest.py` & `newrelic-8.9.0/tests/external_httplib/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_httplib/test_httplib.py` & `newrelic-8.9.0/tests/external_httplib/test_httplib.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_httplib/test_urllib.py` & `newrelic-8.9.0/tests/external_httplib/test_urllib.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_httplib/test_urllib2.py` & `newrelic-8.9.0/tests/external_httplib/test_urllib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_httplib2/conftest.py` & `newrelic-8.9.0/tests/external_httplib2/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_httplib2/test_httplib2.py` & `newrelic-8.9.0/tests/external_httplib2/test_httplib2.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_httpx/conftest.py` & `newrelic-8.9.0/tests/external_httpx/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_httpx/test_client.py` & `newrelic-8.9.0/tests/external_httpx/test_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_requests/conftest.py` & `newrelic-8.9.0/tests/external_requests/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_requests/test_requests.py` & `newrelic-8.9.0/tests/external_requests/test_requests.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_requests/test_span_event.py` & `newrelic-8.9.0/tests/external_requests/test_span_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_urllib3/conftest.py` & `newrelic-8.9.0/tests/external_urllib3/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/external_urllib3/test_urllib3.py` & `newrelic-8.9.0/tests/external_urllib3/test_urllib3.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_aiohttp/_target_application.py` & `newrelic-8.9.0/tests/framework_aiohttp/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_aiohttp/conftest.py` & `newrelic-8.9.0/tests/framework_aiohttp/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_aiohttp/test_client.py` & `newrelic-8.9.0/tests/framework_aiohttp/test_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_aiohttp/test_client_async_await.py` & `newrelic-8.9.0/tests/framework_aiohttp/test_client_async_await.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_aiohttp/test_client_cat.py` & `newrelic-8.9.0/tests/framework_aiohttp/test_client_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_aiohttp/test_externals.py` & `newrelic-8.9.0/tests/framework_aiohttp/test_externals.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_aiohttp/test_middleware.py` & `newrelic-8.9.0/tests/framework_aiohttp/test_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_aiohttp/test_server.py` & `newrelic-8.9.0/tests/framework_aiohttp/test_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_aiohttp/test_server_cat.py` & `newrelic-8.9.0/tests/framework_aiohttp/test_server_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_aiohttp/test_ws.py` & `newrelic-8.9.0/tests/framework_aiohttp/test_ws.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_ariadne/_target_application.py` & `newrelic-8.9.0/tests/framework_ariadne/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_ariadne/conftest.py` & `newrelic-8.9.0/tests/framework_ariadne/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_ariadne/schema.graphql` & `newrelic-8.9.0/tests/framework_ariadne/schema.graphql`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_ariadne/test_application.py` & `newrelic-8.9.0/tests/framework_ariadne/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_ariadne/test_application_async.py` & `newrelic-8.9.0/tests/framework_ariadne/test_application_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_ariadne/test_asgi.py` & `newrelic-8.9.0/tests/framework_ariadne/test_asgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_ariadne/test_wsgi.py` & `newrelic-8.9.0/tests/framework_ariadne/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_bottle/_target_application.py` & `newrelic-8.9.0/tests/framework_bottle/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_bottle/conftest.py` & `newrelic-8.9.0/tests/framework_bottle/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_bottle/test_application.py` & `newrelic-8.9.0/tests/framework_bottle/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_cherrypy/conftest.py` & `newrelic-8.9.0/tests/framework_cherrypy/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_cherrypy/test_application.py` & `newrelic-8.9.0/tests/framework_cherrypy/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_cherrypy/test_dispatch.py` & `newrelic-8.9.0/tests/framework_cherrypy/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_cherrypy/test_resource.py` & `newrelic-8.9.0/tests/framework_cherrypy/test_resource.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_cherrypy/test_routes.py` & `newrelic-8.9.0/tests/framework_cherrypy/test_routes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/_target_application.py` & `newrelic-8.9.0/tests/framework_django/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/conftest.py` & `newrelic-8.9.0/tests/framework_django/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/dummy_app/__init__.py` & `newrelic-8.9.0/tests/framework_django/dummy_app/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/dummy_app/templatetags/__init__.py` & `newrelic-8.9.0/tests/framework_django/dummy_app/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/dummy_app/templatetags/custom_tags.py` & `newrelic-8.9.0/tests/framework_django/dummy_app/templatetags/custom_tags.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/middleware.py` & `newrelic-8.9.0/tests/framework_django/middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/settings.py` & `newrelic-8.9.0/tests/framework_django/settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/templates/main.html` & `newrelic-8.9.0/tests/framework_django/templates/main.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/templates/render_exception.html` & `newrelic-8.9.0/tests/framework_django/templates/render_exception.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/templates/results.html` & `newrelic-8.9.0/tests/framework_django/templates/results.html`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/test_application.py` & `newrelic-8.9.0/tests/framework_django/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/test_asgi_application.py` & `newrelic-8.9.0/tests/framework_django/test_asgi_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/urls.py` & `newrelic-8.9.0/tests/framework_django/urls.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/views.py` & `newrelic-8.9.0/tests/framework_django/views.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_django/wsgi.py` & `newrelic-8.9.0/tests/framework_django/wsgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_falcon/_target_application.py` & `newrelic-8.9.0/tests/framework_falcon/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_falcon/conftest.py` & `newrelic-8.9.0/tests/framework_falcon/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_falcon/test_application.py` & `newrelic-8.9.0/tests/framework_falcon/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_fastapi/_target_application.py` & `newrelic-8.9.0/tests/framework_fastapi/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_fastapi/conftest.py` & `newrelic-8.9.0/tests/framework_fastapi/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_fastapi/test_application.py` & `newrelic-8.9.0/tests/agent_features/test_apdex_metrics.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,34 +8,46 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import logging
+import webtest
+from testing_support.sample_applications import simple_app
+from testing_support.validators.validate_apdex_metrics import validate_apdex_metrics
 
-import pytest
-from testing_support.validators.validate_transaction_metrics import validate_transaction_metrics
-from testing_support.validators.validate_code_level_metrics import validate_code_level_metrics
+from newrelic.api.transaction import current_transaction, suppress_apdex_metric
+from newrelic.api.wsgi_application import wsgi_application
 
+normal_application = webtest.TestApp(simple_app)
 
-@pytest.mark.parametrize(
-    "endpoint,transaction_name",
-    (
-        ("/sync", "_target_application:sync"),
-        ("/async", "_target_application:non_sync"),
-    ),
+# NOTE: This test validates that the server-side apdex_t is set to 0.5
+# If the server-side configuration changes, this test will start to fail.
+
+
+@validate_apdex_metrics(
+    name="",
+    group="Uri",
+    apdex_t_min=0.5,
+    apdex_t_max=0.5,
 )
-def test_application(caplog, app, endpoint, transaction_name):
-    caplog.set_level(logging.ERROR)
+def test_apdex():
+    normal_application.get("/")
 
-    @validate_transaction_metrics(transaction_name, scoped_metrics=[("Function/" + transaction_name, 1)])
-    @validate_code_level_metrics(*transaction_name.split(":"))
-    def _test():
-        response = app.get(endpoint)
-        assert response.status == 200
 
-        # Catch context propagation error messages
-        assert not caplog.records
+# This has to be a Web Transaction.
+# The apdex measurement only applies to Web Transactions
+def test_apdex_suppression():
+    @wsgi_application()
+    def simple_apdex_supression_app(environ, start_response):
+        suppress_apdex_metric()
+
+        start_response(status="200 OK", response_headers=[])
+        transaction = current_transaction()
+
+        assert transaction.suppress_apdex
+        assert transaction.apdex == 0
+        return []
 
-    _test()
+    apdex_suppression_app = webtest.TestApp(simple_apdex_supression_app)
+    apdex_suppression_app.get("/")
```

### Comparing `newrelic-8.8.1/tests/framework_flask/_test_application.py` & `newrelic-8.9.0/tests/framework_flask/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/_test_application_async.py` & `newrelic-8.9.0/tests/framework_flask/_test_application_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/_test_blueprints.py` & `newrelic-8.9.0/tests/framework_flask/_test_blueprints.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/_test_compress.py` & `newrelic-8.9.0/tests/framework_flask/_test_compress.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/_test_middleware.py` & `newrelic-8.9.0/tests/framework_flask/_test_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/_test_not_found.py` & `newrelic-8.9.0/tests/framework_flask/_test_not_found.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/_test_user_exceptions.py` & `newrelic-8.9.0/tests/framework_flask/_test_user_exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/_test_views.py` & `newrelic-8.9.0/tests/framework_flask/_test_views.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/_test_views_async.py` & `newrelic-8.9.0/tests/framework_flask/_test_views_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/conftest.py` & `newrelic-8.9.0/tests/framework_flask/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/test_application.py` & `newrelic-8.9.0/tests/framework_flask/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/test_blueprints.py` & `newrelic-8.9.0/tests/framework_flask/test_blueprints.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/test_compress.py` & `newrelic-8.9.0/tests/framework_flask/test_compress.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/test_middleware.py` & `newrelic-8.9.0/tests/framework_flask/test_middleware.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/test_not_found.py` & `newrelic-8.9.0/tests/framework_flask/test_not_found.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/test_user_exceptions.py` & `newrelic-8.9.0/tests/framework_flask/test_user_exceptions.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_flask/test_views.py` & `newrelic-8.9.0/tests/framework_flask/test_views.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_graphene/_target_application.py` & `newrelic-8.9.0/tests/framework_graphene/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_graphene/conftest.py` & `newrelic-8.9.0/tests/framework_graphene/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_graphene/test_application.py` & `newrelic-8.9.0/tests/framework_graphene/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_graphql/_target_application.py` & `newrelic-8.9.0/tests/framework_graphql/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_graphql/conftest.py` & `newrelic-8.9.0/tests/framework_graphql/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_graphql/test_application.py` & `newrelic-8.9.0/tests/framework_graphql/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_graphql/test_application_async.py` & `newrelic-8.9.0/tests/framework_graphql/test_application_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_grpc/_test_common.py` & `newrelic-8.9.0/tests/framework_grpc/_test_common.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_grpc/conftest.py` & `newrelic-8.9.0/tests/framework_grpc/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_grpc/sample_application/__init__.py` & `newrelic-8.9.0/tests/framework_grpc/sample_application/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_grpc/sample_application/sample_application.proto` & `newrelic-8.9.0/tests/framework_grpc/sample_application/sample_application.proto`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_grpc/test_clients.py` & `newrelic-8.9.0/tests/framework_grpc/test_clients.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_grpc/test_distributed_tracing.py` & `newrelic-8.9.0/tests/framework_grpc/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_grpc/test_get_url.py` & `newrelic-8.9.0/tests/framework_grpc/test_get_url.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_grpc/test_server.py` & `newrelic-8.9.0/tests/framework_grpc/test_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_pyramid/_test_append_slash_app.py` & `newrelic-8.9.0/tests/framework_pyramid/_test_append_slash_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_pyramid/_test_application.py` & `newrelic-8.9.0/tests/framework_pyramid/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_pyramid/conftest.py` & `newrelic-8.9.0/tests/framework_pyramid/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_pyramid/test_append_slash_app.py` & `newrelic-8.9.0/tests/framework_pyramid/test_append_slash_app.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_pyramid/test_application.py` & `newrelic-8.9.0/tests/framework_pyramid/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_pyramid/test_cornice.py` & `newrelic-8.9.0/tests/framework_pyramid/test_cornice.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_sanic/_target_application.py` & `newrelic-8.9.0/tests/framework_sanic/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_sanic/conftest.py` & `newrelic-8.9.0/tests/framework_sanic/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_sanic/test_application.py` & `newrelic-8.9.0/tests/framework_sanic/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_sanic/test_cross_application.py` & `newrelic-8.9.0/tests/framework_sanic/test_cross_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_starlette/_test_application.py` & `newrelic-8.9.0/tests/framework_starlette/_test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_starlette/_test_bg_tasks.py` & `newrelic-8.9.0/tests/framework_starlette/_test_bg_tasks.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_starlette/_test_graphql.py` & `newrelic-8.9.0/tests/framework_starlette/_test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_starlette/conftest.py` & `newrelic-8.9.0/tests/framework_starlette/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_starlette/test_application.py` & `newrelic-8.9.0/tests/framework_starlette/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_starlette/test_bg_tasks.py` & `newrelic-8.9.0/tests/framework_starlette/test_bg_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,19 +85,28 @@
     def _test():
         app = target_application["basehttp"]
         response = app.get("/" + route)
         assert response.status == 200
 
     # The bug was fixed in version 0.21.0 but re-occured in 0.23.1.
     # The bug was also not present on 0.20.1 to 0.23.1 if using Python3.7.
-    BUG_COMPLETELY_FIXED = (0, 21, 0) <= starlette_version < (0, 23, 1) or (
-        (0, 20, 1) <= starlette_version < (0, 23, 1) and sys.version_info[:2] > (3, 7)
+    # The bug was fixed again in version 0.29.0
+    BUG_COMPLETELY_FIXED = any(
+        (
+            (0, 21, 0) <= starlette_version < (0, 23, 1),
+            (0, 20, 1) <= starlette_version < (0, 23, 1) and sys.version_info[:2] > (3, 7),
+            starlette_version >= (0, 29, 0),
+        )
+    )
+    BUG_PARTIALLY_FIXED = any(
+        (
+            (0, 20, 1) <= starlette_version < (0, 21, 0),
+            (0, 23, 1) <= starlette_version < (0, 29, 0),
+        )
     )
-    BUG_PARTIALLY_FIXED = (0, 20, 1) <= starlette_version < (0, 21, 0) or starlette_version >= (0, 23, 1)
-
     if BUG_COMPLETELY_FIXED:
         # Assert both web transaction and background task transactions are present.
         _test = validate_transaction_metrics(
             "_test_bg_tasks:run_%s_bg_task" % route, index=-2, scoped_metrics=[route_metric]
         )(_test)
         _test = validate_transaction_metrics("_test_bg_tasks:%s_bg_task" % route, background_task=True)(_test)
         _test = validate_transaction_count(2)(_test)
```

### Comparing `newrelic-8.8.1/tests/framework_starlette/test_graphql.py` & `newrelic-8.9.0/tests/framework_starlette/test_graphql.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_strawberry/_target_application.py` & `newrelic-8.9.0/tests/framework_strawberry/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_strawberry/conftest.py` & `newrelic-8.9.0/tests/framework_strawberry/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_strawberry/test_application.py` & `newrelic-8.9.0/tests/framework_strawberry/test_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_strawberry/test_application_async.py` & `newrelic-8.9.0/tests/framework_strawberry/test_application_async.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_strawberry/test_asgi.py` & `newrelic-8.9.0/tests/framework_strawberry/test_asgi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_tornado/_target_application.py` & `newrelic-8.9.0/tests/framework_tornado/_target_application.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_tornado/conftest.py` & `newrelic-8.9.0/tests/framework_tornado/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_tornado/test_custom_handler.py` & `newrelic-8.9.0/tests/framework_tornado/test_custom_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_tornado/test_externals.py` & `newrelic-8.9.0/tests/framework_tornado/test_externals.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_tornado/test_inbound_cat.py` & `newrelic-8.9.0/tests/framework_tornado/test_inbound_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/framework_tornado/test_server.py` & `newrelic-8.9.0/tests/framework_tornado/test_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/logger_logging/conftest.py` & `newrelic-8.9.0/tests/logger_logging/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/logger_logging/test_local_decorating.py` & `newrelic-8.9.0/tests/logger_logging/test_local_decorating.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/logger_logging/test_log_forwarding.py` & `newrelic-8.9.0/tests/logger_logging/test_log_forwarding.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/logger_logging/test_logging_handler.py` & `newrelic-8.9.0/tests/logger_logging/test_logging_handler.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/logger_logging/test_metrics.py` & `newrelic-8.9.0/tests/logger_logging/test_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/logger_logging/test_settings.py` & `newrelic-8.9.0/tests/logger_logging/test_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/logger_loguru/conftest.py` & `newrelic-8.9.0/tests/logger_loguru/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/logger_loguru/test_local_decorating.py` & `newrelic-8.9.0/tests/logger_loguru/test_local_decorating.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/logger_loguru/test_log_forwarding.py` & `newrelic-8.9.0/tests/logger_loguru/test_log_forwarding.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/logger_loguru/test_metrics.py` & `newrelic-8.9.0/tests/logger_loguru/test_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/logger_loguru/test_settings.py` & `newrelic-8.9.0/tests/logger_loguru/test_settings.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/logger_loguru/test_stack_inspection.py` & `newrelic-8.9.0/tests/logger_loguru/test_stack_inspection.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_confluentkafka/conftest.py` & `newrelic-8.9.0/tests/messagebroker_confluentkafka/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,44 +80,44 @@
     yield producer
 
     if hasattr(producer, "purge"):
         producer.purge()
 
 
 @pytest.fixture(scope="function")
-def consumer(topic, producer, client_type, json_deserializer):
+def consumer(group_id, topic, producer, client_type, json_deserializer):
     from confluent_kafka import Consumer, DeserializingConsumer
 
     if client_type == "cimpl":
         consumer = Consumer(
             {
                 "bootstrap.servers": BROKER,
                 "auto.offset.reset": "earliest",
                 "heartbeat.interval.ms": 1000,
-                "group.id": "test",
+                "group.id": group_id,
             }
         )
     elif client_type == "serializer_function":
         consumer = DeserializingConsumer(
             {
                 "bootstrap.servers": BROKER,
                 "auto.offset.reset": "earliest",
                 "heartbeat.interval.ms": 1000,
-                "group.id": "test",
+                "group.id": group_id,
                 "value.deserializer": lambda v, c: json.loads(v.decode("utf-8")),
                 "key.deserializer": lambda v, c: json.loads(v.decode("utf-8")) if v is not None else None,
             }
         )
     elif client_type == "serializer_object":
         consumer = DeserializingConsumer(
             {
                 "bootstrap.servers": BROKER,
                 "auto.offset.reset": "earliest",
                 "heartbeat.interval.ms": 1000,
-                "group.id": "test",
+                "group.id": group_id,
                 "value.deserializer": json_deserializer,
                 "key.deserializer": json_deserializer,
             }
         )
 
     consumer.subscribe([topic])
 
@@ -177,14 +177,19 @@
         f.result()  # Block until topic is created.
 
     yield topic
 
     admin.delete_topics(new_topics)
 
 
+@pytest.fixture(scope="session")
+def group_id():
+    return str(uuid.uuid4())
+
+
 @pytest.fixture()
 def send_producer_message(topic, producer, serialize, client_type):
     callback_called = []
 
     def producer_callback(err, msg):
         callback_called.append(True)
```

### Comparing `newrelic-8.8.1/tests/messagebroker_confluentkafka/test_consumer.py` & `newrelic-8.9.0/tests/messagebroker_confluentkafka/test_consumer.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_confluentkafka/test_producer.py` & `newrelic-8.9.0/tests/messagebroker_confluentkafka/test_producer.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_confluentkafka/test_serialization.py` & `newrelic-8.9.0/tests/messagebroker_confluentkafka/test_serialization.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_kafkapython/conftest.py` & `newrelic-8.9.0/tests/messagebroker_kafkapython/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,56 +82,56 @@
         )
 
     yield producer
     producer.close()
 
 
 @pytest.fixture(scope="function")
-def consumer(topic, producer, client_type, json_deserializer, json_callable_deserializer):
+def consumer(group_id, topic, producer, client_type, json_deserializer, json_callable_deserializer):
     if client_type == "no_serializer":
         consumer = kafka.KafkaConsumer(
             topic,
             bootstrap_servers=BROKER,
             auto_offset_reset="earliest",
             consumer_timeout_ms=100,
             heartbeat_interval_ms=1000,
-            group_id="test",
+            group_id=group_id,
         )
     elif client_type == "serializer_function":
         consumer = kafka.KafkaConsumer(
             topic,
             bootstrap_servers=BROKER,
             key_deserializer=lambda v: json.loads(v.decode("utf-8")) if v else None,
             value_deserializer=lambda v: json.loads(v.decode("utf-8")) if v else None,
             auto_offset_reset="earliest",
             consumer_timeout_ms=100,
             heartbeat_interval_ms=1000,
-            group_id="test",
+            group_id=group_id,
         )
     elif client_type == "callable_object":
         consumer = kafka.KafkaConsumer(
             topic,
             bootstrap_servers=BROKER,
             key_deserializer=json_callable_deserializer,
             value_deserializer=json_callable_deserializer,
             auto_offset_reset="earliest",
             consumer_timeout_ms=100,
             heartbeat_interval_ms=1000,
-            group_id="test",
+            group_id=group_id,
         )
     elif client_type == "serializer_object":
         consumer = kafka.KafkaConsumer(
             topic,
             bootstrap_servers=BROKER,
             key_deserializer=json_deserializer,
             value_deserializer=json_deserializer,
             auto_offset_reset="earliest",
             consumer_timeout_ms=100,
             heartbeat_interval_ms=1000,
-            group_id="test",
+            group_id=group_id,
         )
 
     yield consumer
     consumer.close()
 
 
 @pytest.fixture(scope="session")
@@ -198,14 +198,19 @@
     admin.create_topics(new_topics)
 
     yield topic
 
     admin.delete_topics([topic])
 
 
+@pytest.fixture(scope="session")
+def group_id():
+    return str(uuid.uuid4())
+
+
 @pytest.fixture()
 def send_producer_message(topic, producer, serialize):
     def _test():
         producer.send(topic, key=serialize("bar"), value=serialize({"foo": 1}))
         producer.flush()
 
     return _test
```

### Comparing `newrelic-8.8.1/tests/messagebroker_kafkapython/test_consumer.py` & `newrelic-8.9.0/tests/messagebroker_kafkapython/test_consumer.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_kafkapython/test_heartbeat.py` & `newrelic-8.9.0/tests/messagebroker_kafkapython/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_kafkapython/test_producer.py` & `newrelic-8.9.0/tests/messagebroker_kafkapython/test_producer.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_kafkapython/test_serialization.py` & `newrelic-8.9.0/tests/messagebroker_kafkapython/test_serialization.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_pika/compat.py` & `newrelic-8.9.0/tests/messagebroker_pika/compat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_pika/conftest.py` & `newrelic-8.9.0/tests/messagebroker_pika/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_pika/minversion.py` & `newrelic-8.9.0/tests/messagebroker_pika/minversion.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_pika/test_cat.py` & `newrelic-8.9.0/tests/messagebroker_pika/test_cat.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_pika/test_distributed_tracing.py` & `newrelic-8.9.0/tests/messagebroker_pika/test_distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_pika/test_memory_leak.py` & `newrelic-8.9.0/tests/messagebroker_pika/test_memory_leak.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_pika/test_pika_async_connection_consume.py` & `newrelic-8.9.0/tests/messagebroker_pika/test_pika_async_connection_consume.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_pika/test_pika_blocking_connection_consume.py` & `newrelic-8.9.0/tests/messagebroker_pika/test_pika_blocking_connection_consume.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py` & `newrelic-8.9.0/tests/messagebroker_pika/test_pika_blocking_connection_consume_generator.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_pika/test_pika_produce.py` & `newrelic-8.9.0/tests/messagebroker_pika/test_pika_produce.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/messagebroker_pika/test_pika_supportability.py` & `newrelic-8.9.0/tests/messagebroker_pika/test_pika_supportability.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/template_genshi/conftest.py` & `newrelic-8.9.0/tests/template_genshi/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/template_genshi/test_genshi.py` & `newrelic-8.9.0/tests/template_genshi/test_genshi.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/template_mako/conftest.py` & `newrelic-8.9.0/tests/template_mako/conftest.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/template_mako/test_mako.py` & `newrelic-8.9.0/tests/template_mako/test_mako.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/__init__.py` & `newrelic-8.9.0/tests/testing_support/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/asgi_testing.py` & `newrelic-8.9.0/tests/testing_support/asgi_testing.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/db_settings.py` & `newrelic-8.9.0/tests/testing_support/db_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         }
         for instance_num in range(instances)
     ]
     return settings
 
 
 def mysql_settings():
-    """Return a list of dict of settings for connecting to postgresql.
+    """Return a list of dict of settings for connecting to MySQL.
 
     Will return the correct settings, depending on which of the environments it
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
         1. Local
         2. Github Actions
@@ -68,14 +68,40 @@
             "namespace": str(os.getpid()),
         }
         for instance_num in range(instances)
     ]
     return settings
 
 
+def mssql_settings():
+    """Return a list of dict of settings for connecting to MS SQL.
+
+    Will return the correct settings, depending on which of the environments it
+    is running in. It attempts to set variables in the following order, where
+    later environments override earlier ones.
+
+        1. Local
+        2. Github Actions
+    """
+
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "127.0.0.1"
+    instances = 1
+    settings = [
+        {
+            "user": "SA",
+            "password": "python_agent#1234",
+            "host": host,
+            "port": 8080 + instance_num,
+            "namespace": str(os.getpid()),
+        }
+        for instance_num in range(instances)
+    ]
+    return settings
+
+
 def redis_settings():
     """Return a list of dict of settings for connecting to redis.
 
     Will return the correct settings, depending on which of the environments it
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
@@ -91,14 +117,39 @@
             "port": 8080 + instance_num,
         }
         for instance_num in range(instances)
     ]
     return settings
 
 
+def redis_cluster_settings():
+    """Return a list of dict of settings for connecting to redis cluster.
+
+    Will return the correct settings, depending on which of the environments it
+    is running in. It attempts to set variables in the following order, where
+    later environments override earlier ones.
+
+        1. Local
+        2. Github Actions
+    """
+
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "localhost"
+    instances = 1
+    base_port = 6379
+
+    settings = [
+        {
+            "host": host,
+            "port": base_port + instance_num,
+        }
+        for instance_num in range(instances)
+    ]
+    return settings
+
+
 def memcached_settings():
     """Return a list of dict of settings for connecting to memcached.
 
     Will return the correct settings, depending on which of the environments it
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
@@ -217,20 +268,21 @@
     is running in. It attempts to set variables in the following order, where
     later environments override earlier ones.
 
         1. Local
         2. Github Actions
     """
 
-    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "localhost"
+    host = "host.docker.internal" if "GITHUB_ACTIONS" in os.environ else "127.0.0.1"
+    base_port = 8082 if "GITHUB_ACTIONS" in os.environ else 8080
     instances = 2
     settings = [
         {
             "host": host,
-            "port": 8080 + instance_num,
+            "port": base_port + instance_num,
         }
         for instance_num in range(instances)
     ]
     return settings
 
 
 def gearman_settings():
```

### Comparing `newrelic-8.8.1/tests/testing_support/external_fixtures.py` & `newrelic-8.9.0/tests/testing_support/external_fixtures.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/fixture/__init__.py` & `newrelic-8.9.0/tests/testing_support/fixture/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/fixture/event_loop.py` & `newrelic-8.9.0/tests/testing_support/fixture/event_loop.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/fixtures.py` & `newrelic-8.9.0/tests/testing_support/fixtures.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/mock_external_grpc_server.py` & `newrelic-8.9.0/tests/testing_support/mock_external_grpc_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/mock_external_http_server.py` & `newrelic-8.9.0/tests/testing_support/mock_external_http_server.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/mock_http_client.py` & `newrelic-8.9.0/tests/testing_support/mock_http_client.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/sample_applications.py` & `newrelic-8.9.0/tests/testing_support/sample_applications.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/sample_asgi_applications.py` & `newrelic-8.9.0/tests/testing_support/sample_asgi_applications.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/util.py` & `newrelic-8.9.0/tests/testing_support/util.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/__init__.py` & `newrelic-8.9.0/tests/testing_support/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_apdex_metrics.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_apdex_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_application_error_event_count.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_application_error_event_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_application_error_trace_count.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_application_error_trace_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_application_errors.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_application_errors.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_browser_attributes.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_browser_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_code_level_metrics.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_code_level_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_cross_process_headers.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_cross_process_headers.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_custom_event_collector_json.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_custom_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_custom_metrics_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_custom_parameters.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_custom_parameters.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_database_duration.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_database_duration.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_database_node.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_database_node.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_database_trace_inputs.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_database_trace_inputs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_datastore_trace_inputs.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_datastore_trace_inputs.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_distributed_trace_accepted.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_distributed_trace_accepted.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_distributed_tracing_header.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_distributed_tracing_header.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_error_event_attributes.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_error_event_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_error_event_attributes_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_error_event_collector_json.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_error_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_error_trace_attributes.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_error_trace_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_error_trace_attributes_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_error_trace_collector_json.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_error_trace_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_external_node_params.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_external_node_params.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_function_called.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_function_called.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_internal_metrics.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_internal_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_log_event_collector_json.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_log_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_log_event_count.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_log_event_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_log_event_count_outside_transaction.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_log_event_count_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_log_events.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_log_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_log_events_outside_transaction.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_log_events_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_messagebroker_headers.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_messagebroker_headers.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_metric_payload.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_metric_payload.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_non_transaction_error_event.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_non_transaction_error_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_outbound_headers.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_outbound_headers.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_serverless_data.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_serverless_data.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_serverless_metadata.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_serverless_metadata.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_serverless_payload.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_serverless_payload.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_slow_sql_collector_json.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_slow_sql_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_span_events.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_span_events.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_sql_obfuscation.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_sql_obfuscation.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_synthetics_event.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_synthetics_event.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_synthetics_transaction_trace.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_synthetics_transaction_trace.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_time_metrics_outside_transaction.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_time_metrics_outside_transaction.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_count.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_transaction_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_error_trace_attributes.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_transaction_error_trace_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_errors.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_transaction_errors.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_event_attributes.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_transaction_event_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_event_collector_json.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_transaction_event_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_metrics.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_transaction_metrics.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_slow_sql_count.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_transaction_slow_sql_count.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_transaction_trace_attributes.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_transaction_trace_attributes.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_tt_collector_json.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_tt_collector_json.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_tt_parameters.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_tt_parameters.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tests/testing_support/validators/validate_tt_segment_params.py` & `newrelic-8.9.0/tests/testing_support/validators/validate_tt_segment_params.py`

 * *Files identical despite different names*

### Comparing `newrelic-8.8.1/tox.ini` & `newrelic-8.9.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -12,168 +12,172 @@
 ;           framework_aiohttp: tests/framework_aiohttp
 ;        deps =
 ;           adapter_gunicorn-gunicornlatest: gunicorn
 ;           datastore_asyncpg: asyncpg
 ;           framework_aiohttp-aiohttp01: aiohttp<2
 ;           framework_aiohttp-aiohttp0202: aiohttp<2.3
 ; 3. Python version required. Uses the standard tox definitions. (https://tox.readthedocs.io/en/latest/config.html#tox-environments)
-;    Examples: py27,py37,py38,py39,pypy27,pypy37
+;    Examples: py27,py37,py38,py39,pypy27,pypy38
 ; 4. Library and version (Optional). Used when testing multiple versions of the library, and may be omitted when only testing a single version.
 ;    Versions should be specified with 2 digits per version number, so <3 becomes 02 and <3.5 becomes 0304. latest and master are also acceptable versions.
 ;    Examples: uvicorn03, CherryPy0302, uvicornlatest
 ;       deps =
 ;           adapter_uvicorn-uvicorn03: uvicorn<0.4
 ;           adapter_uvicorn-uvicornlatest: uvicorn
 ;           framework_cherrypy-CherryPy0302: CherryPy<3.3.0
 ;           framework_cherrypy-CherryPy0303: CherryPy<3.4.0
 ; 5. With or without New Relic C extensions (Optional). Used for testing agent features.
 ;    Examples: with_extensions, without_extensions
 ;       envlist =
-;           python-agent_features-pypy37-without_extensions,
+;           python-agent_features-pypy38-without_extensions,
 ;           python-agent_streaming-py37-{with,without}_extensions,
 ;
 ; Full Format:
 ;   services_required-tests_folder-python_version-library_and_version[optional]-with/without_c_extensions[optional]
 ;
 ; Full Examples:
 ;   - memcached-datastore_bmemcached-py37-memcached030
 ;   - python-agent_unittests-py38-with_extensions
 ;   - python-adapter_gevent-py27
 
 [tox]
 requires = virtualenv<20.22.0
 setupdir = {toxinidir}
+; Fail tests when interpreters are missing.
+skip_missing_interpreters = false
 envlist =
     python-adapter_cheroot-{py27,py37,py38,py39,py310,py311},
     python-adapter_daphne-{py37,py38,py39,py310,py311}-daphnelatest,
     python-adapter_daphne-py38-daphne{0204,0205},
     python-adapter_gevent-{py27,py37,py38,py310,py311},
     python-adapter_gunicorn-{py37,py38,py39,py310,py311}-aiohttp3-gunicornlatest,
     python-adapter_hypercorn-{py37,py38,py39,py310,py311}-hypercornlatest,
     python-adapter_hypercorn-py38-hypercorn{0010,0011,0012,0013},
     python-adapter_uvicorn-py37-uvicorn03,
     python-adapter_uvicorn-{py37,py38,py39,py310,py311}-uvicornlatest,
     python-adapter_waitress-{py37,py38,py39}-waitress010404,
     python-adapter_waitress-{py37,py38,py39,py310}-waitress02,
     python-adapter_waitress-{py37,py38,py39,py310,py311}-waitresslatest,
     python-agent_features-{py27,py37,py38,py39,py310,py311}-{with,without}_extensions,
-    python-agent_features-{pypy27,pypy37}-without_extensions,
+    python-agent_features-{pypy27,pypy38}-without_extensions,
     python-agent_streaming-py27-grpc0125-{with,without}_extensions,
     python-agent_streaming-{py37,py38,py39,py310,py311}-protobuf04-{with,without}_extensions,
     python-agent_streaming-py39-protobuf{03,0319}-{with,without}_extensions,
     python-agent_unittests-{py27,py37,py38,py39,py310,py311}-{with,without}_extensions,
-    python-agent_unittests-{pypy27,pypy37}-without_extensions,
-    python-application_celery-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
+    python-agent_unittests-{pypy27,pypy38}-without_extensions,
+    python-application_celery-{py27,py37,py38,py39,py310,py311,pypy27,pypy38},
     gearman-application_gearman-{py27,pypy27},
     python-component_djangorestframework-py27-djangorestframework0300,
     python-component_djangorestframework-{py37,py38,py39,py310,py311}-djangorestframeworklatest,
-    python-component_flask_rest-{py37,py38,py39,pypy37}-flaskrestxlatest,
+    python-component_flask_rest-{py37,py38,py39,pypy38}-flaskrestxlatest,
     python-component_flask_rest-{py27,pypy27}-flaskrestx051,
     python-component_graphqlserver-{py37,py38,py39,py310,py311},
     python-component_tastypie-{py27,pypy27}-tastypie0143,
-    python-component_tastypie-{py37,py38,py39,pypy37}-tastypie{0143,latest},
-    python-coroutines_asyncio-{py37,py38,py39,py310,py311,pypy37},
+    python-component_tastypie-{py37,py38,py39,pypy38}-tastypie{0143,latest},
+    python-coroutines_asyncio-{py37,py38,py39,py310,py311,pypy38},
     python-cross_agent-{py27,py37,py38,py39,py310,py311}-{with,without}_extensions,
     python-cross_agent-pypy27-without_extensions,
     postgres-datastore_asyncpg-{py37,py38,py39,py310,py311},
     memcached-datastore_bmemcached-{pypy27,py27,py37,py38,py39,py310,py311}-memcached030,
-    elasticsearchserver07-datastore_elasticsearch-{py27,py37,py38,py39,py310,py311,pypy27,pypy37}-elasticsearch07,
-    elasticsearchserver08-datastore_elasticsearch-{py37,py38,py39,py310,py311,pypy37}-elasticsearch08,
-    memcached-datastore_memcache-{py27,py37,py38,py39,py310,py311,pypy27,pypy37}-memcached01,
+    elasticsearchserver07-datastore_elasticsearch-{py27,py37,py38,py39,py310,py311,pypy27,pypy38}-elasticsearch07,
+    elasticsearchserver08-datastore_elasticsearch-{py37,py38,py39,py310,py311,pypy38}-elasticsearch08,
+    memcached-datastore_memcache-{py27,py37,py38,py39,py310,py311,pypy27,pypy38}-memcached01,
     mysql-datastore_mysql-mysql080023-py27,
     mysql-datastore_mysql-mysqllatest-{py37,py38,py39,py310,py311},
     postgres-datastore_postgresql-{py37,py38,py39},
     postgres-datastore_psycopg2-{py27,py37,py38,py39,py310,py311}-psycopg2latest
     postgres-datastore_psycopg2cffi-{py27,pypy27,py37,py38,py39,py310,py311}-psycopg2cffilatest,
     postgres-datastore_pyodbc-{py27,py37,py311}-pyodbclatest
     memcached-datastore_pylibmc-{py27,py37},
-    memcached-datastore_pymemcache-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
+    memcached-datastore_pymemcache-{py27,py37,py38,py39,py310,py311,pypy27,pypy38},
     mongodb-datastore_pymongo-{py27,py37,py38,py39,py310,py311,pypy27}-pymongo{03},
-    mongodb-datastore_pymongo-{py37,py38,py39,py310,py311,pypy27,pypy37}-pymongo04,
-    mysql-datastore_pymysql-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
-    solr-datastore_pysolr-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
-    redis-datastore_redis-{py27,py37,py38,pypy27,pypy37}-redis03,
-    redis-datastore_redis-{py37,py38,py39,py310,py311,pypy37}-redis{0400,latest},
-    redis-datastore_aioredis-{py37,py38,py39,py310,pypy37}-aioredislatest,
-    redis-datastore_aioredis-{py37,py38,py39,py310,py311,pypy37}-redislatest,
-    redis-datastore_aredis-{py37,py38,py39,pypy37}-aredislatest,
-    solr-datastore_solrpy-{py27,pypy27}-solrpy{00,01},
-    python-datastore_sqlite-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
+    mongodb-datastore_pymongo-{py37,py38,py39,py310,py311,pypy27,pypy38}-pymongo04,
+    mssql-datastore_pymssql-{py37,py38,py39,py310,py311},
+    mysql-datastore_pymysql-{py27,py37,py38,py39,py310,py311,pypy27,pypy38},
+    solr-datastore_pysolr-{py27,py37,py38,py39,py310,py311,pypy27,pypy38},
+    redis-datastore_redis-{py27,py37,py38,pypy27,pypy38}-redis03,
+    redis-datastore_redis-{py37,py38,py39,py310,py311,pypy38}-redis{0400,latest},
+    rediscluster-datastore_rediscluster-{py37,py311,pypy38}-redis{latest},
+    redis-datastore_aioredis-{py37,py38,py39,py310,pypy38}-aioredislatest,
+    redis-datastore_aioredis-{py37,py38,py39,py310,py311,pypy38}-redislatest,
+    redis-datastore_aredis-{py37,py38,py39,pypy38}-aredislatest,
+    python-datastore_sqlite-{py27,py37,py38,py39,py310,py311,pypy27,pypy38},
     python-external_boto3-{py27,py37,py38,py39,py310,py311}-boto01,
     python-external_botocore-{py37,py38,py39,py310,py311}-botocorelatest,
     python-external_botocore-{py311}-botocore128,
     python-external_botocore-py310-botocore0125,
     python-external_feedparser-py27-feedparser{05,06},
     python-external_http-{py27,py37,py38,py39,py310,py311,pypy27},
-    python-external_httplib-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
-    python-external_httplib2-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
+    python-external_httplib-{py27,py37,py38,py39,py310,py311,pypy27,pypy38},
+    python-external_httplib2-{py27,py37,py38,py39,py310,py311,pypy27,pypy38},
     python-external_httpx-{py37,py38,py39,py310,py311},
-    python-external_requests-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
+    python-external_requests-{py27,py37,py38,py39,py310,py311,pypy27,pypy38},
     python-external_urllib3-{py27,py37,pypy27}-urllib3{0109},
-    python-external_urllib3-{py27,py37,py38,py39,py310,py311,pypy27,pypy37}-urllib3latest,
-    python-framework_aiohttp-{py37,py38,py39,py310,py311,pypy37}-aiohttp03,
+    python-external_urllib3-{py27,py37,py38,py39,py310,py311,pypy27,pypy38}-urllib3latest,
+    python-framework_aiohttp-{py37,py38,py39,py310,py311,pypy38}-aiohttp03,
     python-framework_ariadne-{py37,py38,py39,py310,py311}-ariadnelatest,
     python-framework_ariadne-py37-ariadne{0011,0012,0013},
     python-framework_bottle-py27-bottle{0008,0009,0010},
-    python-framework_bottle-{py27,py37,py38,py39,pypy37}-bottle{0011,0012},
+    python-framework_bottle-{py27,py37,py38,py39,pypy38}-bottle{0011,0012},
     python-framework_bottle-{py310,py311}-bottle0012,
     python-framework_bottle-pypy27-bottle{0008,0009,0010,0011,0012},
     ; CherryPy still uses inspect.getargspec, deprecated in favor of inspect.getfullargspec.  Not supported in 3.11
-    python-framework_cherrypy-{py37,py38,py39,py310,py311,pypy37}-CherryPylatest,
+    python-framework_cherrypy-{py37,py38,py39,py310,py311,pypy38}-CherryPylatest,
     python-framework_django-{pypy27,py27}-Django0103,
     python-framework_django-{pypy27,py27,py37}-Django0108,
     python-framework_django-{py39}-Django{0200,0201,0202,0300,0301,latest},
     python-framework_django-{py37,py38,py39,py310,py311}-Django0302,
-    python-framework_falcon-{py27,py37,py38,py39,pypy27,pypy37}-falcon0103,
-    python-framework_falcon-{py37,py38,py39,py310,pypy37}-falcon{0200,master},
+    python-framework_falcon-{py27,py37,py38,py39,pypy27,pypy38}-falcon0103,
+    python-framework_falcon-{py37,py38,py39,py310,pypy38}-falcon{0200,master},
     # Falcon master branch failing on 3.11 currently.
     python-framework_falcon-py311-falcon0200,
     python-framework_fastapi-{py37,py38,py39,py310,py311},
     python-framework_flask-{pypy27,py27}-flask0012,
-    python-framework_flask-{pypy27,py27,py37,py38,py39,py310,py311,pypy37}-flask0101,
+    python-framework_flask-{pypy27,py27,py37,py38,py39,py310,py311,pypy38}-flask0101,
     ; temporarily disabling flaskmaster tests
-    python-framework_flask-{py37,py38,py39,py310,py311,pypy37}-flask{latest},
+    python-framework_flask-{py37,py38,py39,py310,py311,pypy38}-flask{latest},
     python-framework_graphene-{py37,py38,py39,py310,py311}-graphenelatest,
-    python-framework_graphene-{py27,py37,py38,py39,pypy27,pypy37}-graphene{0200,0201},
+    python-framework_graphene-{py27,py37,py38,py39,pypy27,pypy38}-graphene{0200,0201},
     python-framework_graphene-{py310,py311}-graphene0201,
-    python-framework_graphql-{py27,py37,py38,py39,py310,py311,pypy27,pypy37}-graphql02,
-    python-framework_graphql-{py37,py38,py39,py310,py311,pypy37}-graphql03,
+    python-framework_graphql-{py27,py37,py38,py39,py310,py311,pypy27,pypy38}-graphql02,
+    python-framework_graphql-{py37,py38,py39,py310,py311,pypy38}-graphql03,
     ; temporarily disabling graphqlmaster tests
     python-framework_graphql-py37-graphql{0202,0203,0300,0301,0302},
     grpc-framework_grpc-py27-grpc0125,
     grpc-framework_grpc-{py37,py38,py39,py310,py311}-grpclatest,
     python-framework_pyramid-{pypy27,py27,py38}-Pyramid0104,
-    python-framework_pyramid-{pypy27,py27,pypy37,py37,py38,py39,py310,py311}-Pyramid0110-cornice,
-    python-framework_pyramid-{py37,py38,py39,py310,py311,pypy37}-Pyramidlatest,
-    python-framework_sanic-{py38,pypy37}-sanic{190301,1906,1912,200904,210300,2109,2112,2203,2290},
-    python-framework_sanic-{py37,py38,py39,py310,py311,pypy37}-saniclatest,
-    python-framework_starlette-{py310,pypy37}-starlette{0014,0015,0019},
+    python-framework_pyramid-{pypy27,py27,pypy38,py37,py38,py39,py310,py311}-Pyramid0110-cornice,
+    python-framework_pyramid-{py37,py38,py39,py310,py311,pypy38}-Pyramidlatest,
+    python-framework_sanic-{py38,pypy38}-sanic{190301,1906,1912,200904,210300,2109,2112,2203,2290},
+    python-framework_sanic-{py37,py38,py39,py310,py311,pypy38}-saniclatest,
+    python-framework_starlette-{py310,pypy38}-starlette{0014,0015,0019,0028},
     python-framework_starlette-{py37,py38}-starlette{002001},
-    python-framework_starlette-{py37,py38,py39,py310,py311,pypy37}-starlettelatest,
+    python-framework_starlette-{py37,py38,py39,py310,py311,pypy38}-starlettelatest,
     python-framework_strawberry-{py37,py38,py39,py310,py311}-strawberrylatest,
-    python-logger_logging-{py27,py37,py38,py39,py310,py311,pypy27,pypy37},
-    python-logger_loguru-{py37,py38,py39,py310,py311,pypy37}-logurulatest,
+    python-logger_logging-{py27,py37,py38,py39,py310,py311,pypy27,pypy38},
+    python-logger_loguru-{py37,py38,py39,py310,py311,pypy38}-logurulatest,
     python-logger_loguru-py39-loguru{06,05,04,03},
-    python-framework_tornado-{py37,py38,py39,py310,py311,pypy37}-tornado0600,
+    python-framework_tornado-{py38,py39,py310,py311}-tornadolatest,
     python-framework_tornado-{py38,py39,py310,py311}-tornadomaster,
-    rabbitmq-messagebroker_pika-{py27,py37,py38,py39,pypy27,pypy37}-pika0.13,
-    rabbitmq-messagebroker_pika-{py37,py38,py39,py310,py311,pypy37}-pikalatest,
-    kafka-messagebroker_confluentkafka-{py27,py37,py38,py39,py310,py311}-confluentkafkalatest,
+    rabbitmq-messagebroker_pika-{py27,py37,py38,py39,pypy27,pypy38}-pika0.13,
+    rabbitmq-messagebroker_pika-{py37,py38,py39,py310,py311,pypy38}-pikalatest,
+    kafka-messagebroker_confluentkafka-{py37,py38,py39,py310,py311}-confluentkafkalatest,
     kafka-messagebroker_confluentkafka-{py27,py39}-confluentkafka{0107,0106},
     ; confluent-kafka had a bug in 1.8.2's setup.py file which was incompatible with 2.7.
     kafka-messagebroker_confluentkafka-{py39}-confluentkafka{0108},
-    kafka-messagebroker_kafkapython-{pypy27,py27,py37,py38,pypy37}-kafkapythonlatest,
+    kafka-messagebroker_kafkapython-{pypy27,py27,py37,py38,pypy38}-kafkapythonlatest,
     kafka-messagebroker_kafkapython-{py27,py38}-kafkapython{020001,020000,0104},
     python-template_genshi-{py27,py37,py311}-genshilatest
+    python-template_jinja2-{py37,py311}-jinja2latest
     python-template_mako-{py27,py37,py310,py311}
 
 [testenv]
 deps =
     # Base Dependencies
-    {py37,py38,py39,py310,py311,pypy37}: pytest==7.2.2
+    {py37,py38,py39,py310,py311,pypy38}: pytest==7.2.2
     {py27,pypy27}: pytest==4.6.11
     iniconfig
     coverage
     WebTest==2.0.35
 
     # Test Suite Dependencies
     adapter_cheroot: cheroot
@@ -191,21 +195,22 @@
     adapter_hypercorn-hypercorn0013: hypercorn<0.14
     adapter_hypercorn-hypercorn0012: hypercorn<0.13
     adapter_hypercorn-hypercorn0011: hypercorn<0.12
     adapter_hypercorn-hypercorn0010: hypercorn<0.11
     adapter_uvicorn-uvicorn03: uvicorn<0.4
     adapter_uvicorn-uvicorn014: uvicorn<0.15
     adapter_uvicorn-uvicornlatest: uvicorn
+    adapter_uvicorn: typing-extensions
     adapter_waitress: WSGIProxy2
     adapter_waitress-waitress010404: waitress<1.4.5
     adapter_waitress-waitress02: waitress<2.1
     adapter_waitress-waitresslatest: waitress
     agent_features: beautifulsoup4
     application_celery: celery<6.0
-    application_celery-{py37,pypy37}: importlib-metadata<5.0
+    application_celery-{py37,pypy38}: importlib-metadata<5.0
     application_gearman: gearman<3.0.0
     component_djangorestframework-djangorestframework0300: Django<1.9
     component_djangorestframework-djangorestframework0300: djangorestframework<3.1
     component_djangorestframework-djangorestframeworklatest: Django
     component_djangorestframework-djangorestframeworklatest: djangorestframework
     component_flask_rest: flask
     component_flask_rest: flask-restful
@@ -216,16 +221,16 @@
     component_graphqlserver: graphql-server[sanic,flask]==3.0.0b5
     component_graphqlserver: sanic>20
     component_graphqlserver: Flask
     component_graphqlserver: markupsafe<2.1
     component_graphqlserver: jinja2<3.1
     component_tastypie-tastypie0143: django-tastypie<0.14.4
     component_tastypie-{py27,pypy27}-tastypie0143: django<1.12
-    component_tastypie-{py37,py38,py39,py310,py311,pypy37}-tastypie0143: django<3.0.1
-    component_tastypie-{py37,py38,py39,py310,py311,pypy37}-tastypie0143: asgiref<3.7.1  # asgiref==3.7.1 only suppport Python 3.10+
+    component_tastypie-{py37,py38,py39,py310,py311,pypy38}-tastypie0143: django<3.0.1
+    component_tastypie-{py37,py38,py39,py310,py311,pypy38}-tastypie0143: asgiref<3.7.1  # asgiref==3.7.1 only suppport Python 3.10+
     component_tastypie-tastypielatest: django-tastypie
     component_tastypie-tastypielatest: django<4.1
     component_tastypie-tastypielatest: asgiref<3.7.1  # asgiref==3.7.1 only suppport Python 3.10+
     coroutines_asyncio-{py37,py38,py39,py310,py311}: uvloop
     cross_agent: mock==1.0.1
     cross_agent: requests
     datastore_asyncpg: asyncpg
@@ -242,25 +247,25 @@
     datastore_psycopg2-psycopg2latest: psycopg2-binary
     datastore_psycopg2cffi-psycopg2cffilatest: psycopg2cffi
     datastore_pyodbc-pyodbclatest: pyodbc
     datastore_pylibmc: pylibmc
     datastore_pymemcache: pymemcache
     datastore_pymongo-pymongo03: pymongo<4.0
     datastore_pymongo-pymongo04: pymongo<5.0
+    datastore_pymssql: pymssql
     datastore_pymysql: PyMySQL<0.11
     datastore_pysolr: pysolr<4.0
     datastore_redis-redislatest: redis
+    datastore_rediscluster-redislatest: redis
     datastore_redis-redis0400: redis<4.1
     datastore_redis-redis03: redis<4.0
     datastore_redis-{py27,pypy27}: rb
     datastore_aioredis-redislatest: redis
     datastore_aioredis-aioredislatest: aioredis
     datastore_aredis-aredislatest: aredis
-    datastore_solrpy-solrpy00: solrpy<1.0
-    datastore_solrpy-solrpy01: solrpy<2.0
     external_boto3-boto01: boto3<2.0
     external_boto3-boto01: moto<2.0
     external_boto3-py27: rsa<4.7.1
     external_botocore-botocorelatest: botocore
     external_botocore-botocore128: botocore<1.29
     external_botocore-botocore0125: botocore<1.26
     external_botocore-{py37,py38,py39,py310,py311}: moto[awslambda,ec2,iam]<3.0
@@ -350,19 +355,20 @@
     framework_sanic-sanic{1812,190301,1906}: aiohttp
     framework_sanic-sanic{1812,190301,1906,1912,200904,210300,2109,2112,2203,2290}: websockets<11
     framework_starlette: graphene<3
     framework_starlette-starlette0014: starlette<0.15
     framework_starlette-starlette0015: starlette<0.16
     framework_starlette-starlette0019: starlette<0.20
     framework_starlette-starlette002001: starlette==0.20.1
+    framework_starlette-starlette0028: starlette<0.29
     framework_starlette-starlettelatest: starlette
     framework_strawberry: starlette
     framework_strawberry-strawberrylatest: strawberry-graphql
     framework_tornado: pycurl
-    framework_tornado-tornado0600: tornado<6.1
+    framework_tornado-tornadolatest: tornado
     framework_tornado-tornadomaster: https://github.com/tornadoweb/tornado/archive/master.zip
     logger_loguru-logurulatest: loguru
     logger_loguru-loguru06: loguru<0.7
     logger_loguru-loguru05: loguru<0.6
     logger_loguru-loguru04: loguru<0.5
     logger_loguru-loguru03: loguru<0.4
     messagebroker_pika-pika0.13: pika<0.14
@@ -374,43 +380,44 @@
     messagebroker_confluentkafka-confluentkafka0107: confluent-kafka<1.8
     messagebroker_confluentkafka-confluentkafka0106: confluent-kafka<1.7
     messagebroker_kafkapython-kafkapythonlatest: kafka-python
     messagebroker_kafkapython-kafkapython020001: kafka-python<2.0.2
     messagebroker_kafkapython-kafkapython020000: kafka-python<2.0.1
     messagebroker_kafkapython-kafkapython0104: kafka-python<1.5
     template_genshi-genshilatest: genshi
+    template_jinja2-jinja2latest: Jinja2
     template_mako: mako
 
 setenv =
     PYTHONPATH={toxinidir}/tests
     TOX_ENV_DIR={envdir}
     COVERAGE_FILE={envdir}/.coverage.{envname}
     COVERAGE_RCFILE={toxinidir}/tox.ini
     with_extensions: NEW_RELIC_EXTENSIONS = true
     without_extensions: NEW_RELIC_EXTENSIONS = false
     agent_features: NEW_RELIC_APDEX_T = 1000
     framework_grpc: PYTHONPATH={toxinidir}/tests/:{toxinidir}/tests/framework_grpc/sample_application
-    framework_tornado: PYCURL_SSL_LIBRARY=openssl
-    framework_tornado: LDFLAGS=-L/usr/local/opt/openssl/lib
-    framework_tornado: CPPFLAGS=-I/usr/local/opt/openssl/include
+    framework_tornado-{py38,py39,py310,py311}: PYCURL_SSL_LIBRARY=openssl
+    framework_tornado-{py38,py39,py310,py311}: LDFLAGS=-L/usr/local/opt/openssl/lib
+    framework_tornado-{py38,py39,py310,py311}: CPPFLAGS=-I/usr/local/opt/openssl/include
 
 passenv =
     NEW_RELIC_DEVELOPER_MODE
     NEW_RELIC_LICENSE_KEY
     NEW_RELIC_HOST
     GITHUB_ACTIONS
 
 commands =
     framework_grpc: python -m grpc_tools.protoc \
     framework_grpc:     --proto_path={toxinidir}/tests/framework_grpc/sample_application \
     framework_grpc:     --python_out={toxinidir}/tests/framework_grpc/sample_application \
     framework_grpc:     --grpc_python_out={toxinidir}/tests/framework_grpc/sample_application \
     framework_grpc:     /{toxinidir}/tests/framework_grpc/sample_application/sample_application.proto
 
-    framework_tornado: pip install --ignore-installed --config-settings="--build-option=--with-openssl" pycurl
+    framework_tornado-{py38,py39,py310,py311}: pip install --ignore-installed --config-settings="--build-option=--with-openssl" pycurl
     coverage run -m pytest -v []
 
 allowlist_externals={toxinidir}/.github/scripts/*
 
 install_command=
     {toxinidir}/.github/scripts/retry.sh 3 pip install {opts} {packages}
 
@@ -444,20 +451,21 @@
     datastore_postgresql: tests/datastore_postgresql
     datastore_psycopg2: tests/datastore_psycopg2
     datastore_pyodbc: tests/datastore_pyodbc
     datastore_psycopg2cffi: tests/datastore_psycopg2cffi
     datastore_pylibmc: tests/datastore_pylibmc
     datastore_pymemcache: tests/datastore_pymemcache
     datastore_pymongo: tests/datastore_pymongo
+    datastore_pymssql: tests/datastore_pymssql
     datastore_pymysql: tests/datastore_pymysql
     datastore_pysolr: tests/datastore_pysolr
     datastore_redis: tests/datastore_redis
+    datastore_rediscluster: tests/datastore_rediscluster
     datastore_aioredis: tests/datastore_aioredis
     datastore_aredis: tests/datastore_aredis
-    datastore_solrpy: tests/datastore_solrpy
     datastore_sqlite: tests/datastore_sqlite
     external_boto3: tests/external_boto3
     external_botocore: tests/external_botocore
     external_feedparser: tests/external_feedparser
     external_http: tests/external_http
     external_httplib: tests/external_httplib
     external_httplib2: tests/external_httplib2
@@ -482,14 +490,15 @@
     framework_tornado: tests/framework_tornado
     logger_logging: tests/logger_logging
     logger_loguru: tests/logger_loguru
     messagebroker_pika: tests/messagebroker_pika
     messagebroker_confluentkafka: tests/messagebroker_confluentkafka
     messagebroker_kafkapython: tests/messagebroker_kafkapython
     template_genshi: tests/template_genshi
+    template_jinja2: tests/template_jinja2
     template_mako: tests/template_mako
 
 [pytest]
 usefixtures =
     collector_available_fixture
     collector_agent_registration
```

