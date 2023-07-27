# Comparing `tmp/onefuzz-8.5.0.tar.gz` & `tmp/onefuzz-8.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\onefuzz-8.5.0.tar", last modified: Mon Jul 17 15:58:15 2023, max compression
+gzip compressed data, was "dist\onefuzz-8.6.0.tar", last modified: Wed Jul 26 23:07:44 2023, max compression
```

## Comparing `onefuzz-8.5.0.tar` & `onefuzz-8.6.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/
--rw-rw-rw-   0        0        0     1162 2023-07-17 15:57:13.000000 onefuzz-8.5.0/LICENSE
--rw-rw-rw-   0        0        0      162 2023-07-17 15:57:13.000000 onefuzz-8.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2335 2023-07-17 15:58:15.000000 onefuzz-8.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1742 2023-07-17 15:57:13.000000 onefuzz-8.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/azure-functions-example/
--rw-rw-rw-   0        0        0      297 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/azure-functions-example/README.md
--rw-rw-rw-   0        0        0      141 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/azure-functions-example/host.json
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/azure-functions-example/info/
--rw-rw-rw-   0        0        0      391 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/azure-functions-example/info/__init__.py
--rw-rw-rw-   0        0        0      319 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/azure-functions-example/info/function.json
--rw-rw-rw-   0        0        0       57 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/azure-functions-example/requirements.txt
--rw-rw-rw-   0        0        0     7557 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/domato.py
--rw-rw-rw-   0        0        0      773 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/get-running.py
--rw-rw-rw-   0        0        0     4649 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/honggfuzz.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/llvm-source-coverage/
--rw-rw-rw-   0        0        0       41 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/.gitignore
--rw-rw-rw-   0        0        0     7347 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/llvm-source-coverage/inputs/
--rw-rw-rw-   0        0        0        4 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/inputs/input.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/llvm-source-coverage/setup/
--rw-rw-rw-   0        0        0      398 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/setup/Makefile
--rw-rw-rw-   0        0        0     1556 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/setup/simple.c
--rw-rw-rw-   0        0        0     3277 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
--rw-rw-rw-   0        0        0     2963 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/source-coverage.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/llvm-source-coverage/tools/
--rw-rw-rw-   0        0        0     1177 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/tools/source-coverage.sh
--rw-rw-rw-   0        0        0     2800 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/oss-fuzz-target.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/extra/
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/extra/pyinstaller/
--rw-rw-rw-   0        0        0      200 2023-07-17 15:57:13.000000 onefuzz-8.5.0/extra/pyinstaller/hook-onefuzz.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz/
--rw-rw-rw-   0        0        0      129 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/__init__.py
--rw-rw-rw-   0        0        0      902 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/__main__.py
--rw-rw-rw-   0        0        0      126 2023-07-17 15:57:14.000000 onefuzz-8.5.0/onefuzz/__version__.py
--rw-rw-rw-   0        0        0    69081 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/api.py
--rw-rw-rw-   0        0        0     1059 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/azcopy.py
--rw-rw-rw-   0        0        0     2982 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/azure_identity_credential_adapter.py
--rw-rw-rw-   0        0        0    22909 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/backend.py
--rw-rw-rw-   0        0        0    20501 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/onefuzz/data/
--rw-rw-rw-   0        0        0     1232 2023-07-17 15:58:13.000000 onefuzz-8.5.0/onefuzz/data/licenses.json
--rw-rw-rw-   0        0        0     1004 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/data/privacy.txt
--rw-rw-rw-   0        0        0    31463 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/onefuzz/job_templates/
--rw-rw-rw-   0        0        0        0 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/__init__.py
--rw-rw-rw-   0        0        0     4095 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/builder.py
--rw-rw-rw-   0        0        0     1723 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/cache.py
--rw-rw-rw-   0        0        0     6161 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/handlers.py
--rw-rw-rw-   0        0        0     3596 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/job_monitor.py
--rw-rw-rw-   0        0        0     3159 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/main.py
--rw-rw-rw-   0        0        0     1851 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/manage.py
--rw-rw-rw-   0        0        0      768 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/opentelemetry_exporter.py
--rw-rw-rw-   0        0        0     1682 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/rdp.py
--rw-rw-rw-   0        0        0     3522 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/ssh.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/onefuzz/status/
--rw-rw-rw-   0        0        0        0 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/__init__.py
--rw-rw-rw-   0        0        0    13902 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/cache.py
--rw-rw-rw-   0        0        0     5152 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/cmd.py
--rw-rw-rw-   0        0        0      905 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/raw.py
--rw-rw-rw-   0        0        0     1856 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/signalr.py
--rw-rw-rw-   0        0        0     3009 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/top.py
--rw-rw-rw-   0        0        0     6255 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/top_view.py
--rw-rw-rw-   0        0        0     2882 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/template.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/onefuzz/templates/
--rw-rw-rw-   0        0        0    10701 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/templates/__init__.py
--rw-rw-rw-   0        0        0     7003 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/templates/afl.py
--rw-rw-rw-   0        0        0    43054 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/templates/libfuzzer.py
--rw-rw-rw-   0        0        0     8812 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/templates/ossfuzz.py
--rw-rw-rw-   0        0        0     9630 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/templates/radamsa.py
--rw-rw-rw-   0        0        0    10709 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/templates/regression.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/onefuzz.egg-info/
--rw-rw-rw-   0        0        0     2335 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2015 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      443 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2023-07-17 15:57:13.000000 onefuzz-8.5.0/requirements-dev.txt
--rw-rw-rw-   0        0        0      101 2023-07-17 15:57:13.000000 onefuzz-8.5.0/requirements-lint.txt
--rw-rw-rw-   0        0        0      607 2023-07-17 15:57:14.000000 onefuzz-8.5.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 15:58:15.000000 onefuzz-8.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-07-17 15:57:13.000000 onefuzz-8.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/tests/
--rw-rw-rw-   0        0        0        0 2023-07-17 15:57:13.000000 onefuzz-8.5.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-07-17 15:57:13.000000 onefuzz-8.5.0/tests/test_template_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/
+-rw-rw-rw-   0        0        0     1162 2023-07-26 23:07:11.000000 onefuzz-8.6.0/LICENSE
+-rw-rw-rw-   0        0        0      162 2023-07-26 23:07:11.000000 onefuzz-8.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2335 2023-07-26 23:07:44.000000 onefuzz-8.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1742 2023-07-26 23:07:11.000000 onefuzz-8.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/azure-functions-example/
+-rw-rw-rw-   0        0        0      297 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/azure-functions-example/README.md
+-rw-rw-rw-   0        0        0      141 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/azure-functions-example/host.json
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/azure-functions-example/info/
+-rw-rw-rw-   0        0        0      391 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/azure-functions-example/info/__init__.py
+-rw-rw-rw-   0        0        0      319 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/azure-functions-example/info/function.json
+-rw-rw-rw-   0        0        0       57 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/azure-functions-example/requirements.txt
+-rw-rw-rw-   0        0        0     7557 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/domato.py
+-rw-rw-rw-   0        0        0      773 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/get-running.py
+-rw-rw-rw-   0        0        0     4649 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/honggfuzz.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/llvm-source-coverage/
+-rw-rw-rw-   0        0        0       41 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/.gitignore
+-rw-rw-rw-   0        0        0     7347 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/llvm-source-coverage/inputs/
+-rw-rw-rw-   0        0        0        4 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/inputs/input.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/llvm-source-coverage/setup/
+-rw-rw-rw-   0        0        0      398 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/setup/Makefile
+-rw-rw-rw-   0        0        0     1556 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/setup/simple.c
+-rw-rw-rw-   0        0        0     3277 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
+-rw-rw-rw-   0        0        0     2963 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/source-coverage.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/examples/llvm-source-coverage/tools/
+-rw-rw-rw-   0        0        0     1177 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/llvm-source-coverage/tools/source-coverage.sh
+-rw-rw-rw-   0        0        0     2800 2023-07-26 23:07:11.000000 onefuzz-8.6.0/examples/oss-fuzz-target.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/extra/
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/extra/pyinstaller/
+-rw-rw-rw-   0        0        0      200 2023-07-26 23:07:11.000000 onefuzz-8.6.0/extra/pyinstaller/hook-onefuzz.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz/
+-rw-rw-rw-   0        0        0      129 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/__init__.py
+-rw-rw-rw-   0        0        0      902 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/__main__.py
+-rw-rw-rw-   0        0        0      126 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/__version__.py
+-rw-rw-rw-   0        0        0    70921 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/api.py
+-rw-rw-rw-   0        0        0     1521 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/azcopy.py
+-rw-rw-rw-   0        0        0     2982 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/azure_identity_credential_adapter.py
+-rw-rw-rw-   0        0        0    22928 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/backend.py
+-rw-rw-rw-   0        0        0    20501 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz/data/
+-rw-rw-rw-   0        0        0     1232 2023-07-26 23:07:43.000000 onefuzz-8.6.0/onefuzz/data/licenses.json
+-rw-rw-rw-   0        0        0     1004 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/data/privacy.txt
+-rw-rw-rw-   0        0        0    31472 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz/job_templates/
+-rw-rw-rw-   0        0        0        0 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/__init__.py
+-rw-rw-rw-   0        0        0     4095 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/builder.py
+-rw-rw-rw-   0        0        0     1723 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/cache.py
+-rw-rw-rw-   0        0        0     6161 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/handlers.py
+-rw-rw-rw-   0        0        0     3596 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/job_monitor.py
+-rw-rw-rw-   0        0        0     3159 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/main.py
+-rw-rw-rw-   0        0        0     1851 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/job_templates/manage.py
+-rw-rw-rw-   0        0        0      768 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/opentelemetry_exporter.py
+-rw-rw-rw-   0        0        0     1682 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/rdp.py
+-rw-rw-rw-   0        0        0     3522 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/ssh.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz/status/
+-rw-rw-rw-   0        0        0        0 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/__init__.py
+-rw-rw-rw-   0        0        0    13902 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/cache.py
+-rw-rw-rw-   0        0        0     5152 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/cmd.py
+-rw-rw-rw-   0        0        0      905 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/raw.py
+-rw-rw-rw-   0        0        0     1856 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/signalr.py
+-rw-rw-rw-   0        0        0     3009 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/top.py
+-rw-rw-rw-   0        0        0     6255 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/status/top_view.py
+-rw-rw-rw-   0        0        0     2882 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/template.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz/templates/
+-rw-rw-rw-   0        0        0    10701 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/templates/__init__.py
+-rw-rw-rw-   0        0        0     7003 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/templates/afl.py
+-rw-rw-rw-   0        0        0    43098 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/templates/libfuzzer.py
+-rw-rw-rw-   0        0        0     8812 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/templates/ossfuzz.py
+-rw-rw-rw-   0        0        0     9630 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/templates/radamsa.py
+-rw-rw-rw-   0        0        0    10709 2023-07-26 23:07:11.000000 onefuzz-8.6.0/onefuzz/templates/regression.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/
+-rw-rw-rw-   0        0        0     2335 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2015 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      443 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 23:07:44.000000 onefuzz-8.6.0/onefuzz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2023-07-26 23:07:11.000000 onefuzz-8.6.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0      101 2023-07-26 23:07:11.000000 onefuzz-8.6.0/requirements-lint.txt
+-rw-rw-rw-   0        0        0      607 2023-07-26 23:07:11.000000 onefuzz-8.6.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 23:07:44.000000 onefuzz-8.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-07-26 23:07:11.000000 onefuzz-8.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 23:07:44.000000 onefuzz-8.6.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-26 23:07:11.000000 onefuzz-8.6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-07-26 23:07:11.000000 onefuzz-8.6.0/tests/test_template_helper.py
```

### Comparing `onefuzz-8.5.0/LICENSE` & `onefuzz-8.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/PKG-INFO` & `onefuzz-8.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 8.5.0
+Version: 8.6.0
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-8.5.0/README.md` & `onefuzz-8.6.0/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/examples/domato.py` & `onefuzz-8.6.0/examples/domato.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/examples/get-running.py` & `onefuzz-8.6.0/examples/get-running.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/examples/honggfuzz.py` & `onefuzz-8.6.0/examples/honggfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/examples/llvm-source-coverage/README.md` & `onefuzz-8.6.0/examples/llvm-source-coverage/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/examples/llvm-source-coverage/setup/simple.c` & `onefuzz-8.6.0/examples/llvm-source-coverage/setup/simple.c`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py` & `onefuzz-8.6.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/examples/llvm-source-coverage/source-coverage.py` & `onefuzz-8.6.0/examples/llvm-source-coverage/source-coverage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/examples/llvm-source-coverage/tools/source-coverage.sh` & `onefuzz-8.6.0/examples/llvm-source-coverage/tools/source-coverage.sh`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/examples/oss-fuzz-target.py` & `onefuzz-8.6.0/examples/oss-fuzz-target.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/__main__.py` & `onefuzz-8.6.0/onefuzz/__main__.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/api.py` & `onefuzz-8.6.0/onefuzz/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -553,31 +553,68 @@
         include_setup: bool = False,
         output_dir: primitives.Directory = primitives.Directory("."),
     ) -> None:
         """downloads the files necessary to locally repro the crash from a given report"""
         report_bytes = self.onefuzz.containers.files.get(report_container, report_name)
         report = json.loads(report_bytes)
 
+        crash_info = {
+            "input_blob_container": primitives.Container(""),
+            "input_blob_name": "",
+            "job_id": "",
+        }
+        if "input_blob" in report:
+            crash_info["input_blob_container"] = report["input_blob"]["container"]
+            crash_info["input_blob_name"] = report["input_blob"]["name"]
+            crash_info["job_id"] = report["job_id"]
+        elif "crash_test_result" in report and "original_crash_test_result" in report:
+            if report["original_crash_test_result"]["crash_report"] is None:
+                self.logger.error(
+                    "No crash report found in the original crash test result, repro files cannot be retrieved"
+                )
+                return
+            elif report["crash_test_result"]["crash_report"] is None:
+                self.logger.info(
+                    "No crash report found in the new crash test result, falling back on the original crash test result for job_id"
+                    "Note: if using --include_setup, the downloaded fuzzer binaries may be out-of-date"
+                )
+
+            original_report = report["original_crash_test_result"]["crash_report"]
+            new_report = (
+                report["crash_test_result"]["crash_report"] or original_report
+            )  # fallback on original_report
+
+            crash_info["input_blob_container"] = original_report["input_blob"][
+                "container"
+            ]
+            crash_info["input_blob_name"] = original_report["input_blob"]["name"]
+            crash_info["job_id"] = new_report["job_id"]
+        else:
+            self.logger.error(
+                "Encountered an unhandled report format, repro files cannot be retrieved"
+            )
+            return
+
         self.logger.info(
             "downloading files necessary to locally repro crash %s",
-            report["input_blob"]["name"],
+            crash_info["input_blob_name"],
         )
-
         self.onefuzz.containers.files.download(
-            report["input_blob"]["container"],
-            report["input_blob"]["name"],
-            os.path.join(output_dir, report["input_blob"]["name"]),
+            primitives.Container(crash_info["input_blob_container"]),
+            crash_info["input_blob_name"],
+            os.path.join(output_dir, crash_info["input_blob_name"]),
         )
 
         if include_setup:
             setup_container = list(
                 self.onefuzz.jobs.containers.list(
-                    report["job_id"], enums.ContainerType.setup
+                    crash_info["job_id"], enums.ContainerType.setup
                 )
             )[0]
+
             self.onefuzz.containers.files.download_dir(
                 primitives.Container(setup_container), output_dir
             )
 
     def create(
         self, container: primitives.Container, path: str, duration: int = 24
     ) -> models.Repro:
```

### Comparing `onefuzz-8.5.0/onefuzz/azcopy.py` & `onefuzz-8.6.0/onefuzz/azcopy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 import os
 import shutil
 import subprocess  # nosec
 
 
 def find_azcopy() -> str:
     azcopy = os.environ.get("AZCOPY")
+    binary_name = "azcopy" if os.name == "posix" else "azcopy.exe"
 
     if azcopy:
         if not os.path.exists(azcopy):
             raise Exception(f"AZCOPY environment variable is invalid: {azcopy}")
+        elif os.path.isdir(azcopy):
+            contains_azcopy = os.path.isfile(os.path.join(azcopy, binary_name))
+
+            if contains_azcopy:
+                azcopy = os.path.join(azcopy, binary_name)
+            else:
+                raise Exception(
+                    f"The directory specified by AZCOPY doesn't contain the file '{binary_name}': {azcopy}"
+                )
     else:
         azcopy = shutil.which("azcopy")
 
     if not azcopy:
         raise Exception(
             "unable to find 'azcopy' in path or AZCOPY environment variable"
         )
```

### Comparing `onefuzz-8.5.0/onefuzz/azure_identity_credential_adapter.py` & `onefuzz-8.6.0/onefuzz/azure_identity_credential_adapter.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/backend.py` & `onefuzz-8.6.0/onefuzz/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     def __init__(
         self,
         config: BackendConfig,
         config_path: Optional[str] = None,
         token_path: Optional[str] = None,
         client_secret: Optional[str] = None,
     ):
-        RequestsInstrumentor().instrument()
+        RequestsInstrumentor().instrument(skip_dep_check=True)
         self.config_path = os.path.expanduser(config_path or DEFAULT_CONFIG_PATH)
         self.token_path = os.path.expanduser(token_path or DEFAULT_TOKEN_PATH)
         self.client_secret = client_secret
         self.config = config
         self.token_cache: Optional[msal.SerializableTokenCache] = None
         self.init_cache()
         self.app: Optional[msal.ClientApplication] = None
```

### Comparing `onefuzz-8.5.0/onefuzz/cli.py` & `onefuzz-8.6.0/onefuzz/cli.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/data/licenses.json` & `onefuzz-8.6.0/onefuzz/data/licenses.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {'4': "{'Version': '2023.6'}"}*

```diff
@@ -23,15 +23,15 @@
         "URL": "https://www.pyinstaller.org/",
         "Version": "5.13.0"
     },
     {
         "License": "UNKNOWN",
         "Name": "pyinstaller-hooks-contrib",
         "URL": "https://github.com/pyinstaller/pyinstaller-hooks-contrib",
-        "Version": "2023.5"
+        "Version": "2023.6"
     },
     {
         "License": "BSD-3-Clause",
         "Name": "pywin32-ctypes",
         "URL": "https://github.com/enthought/pywin32-ctypes",
         "Version": "0.2.2"
     },
```

### Comparing `onefuzz-8.5.0/onefuzz/data/privacy.txt` & `onefuzz-8.6.0/onefuzz/data/privacy.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/debug.py` & `onefuzz-8.6.0/onefuzz/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -818,37 +818,34 @@
         self,
         notificationConfig: models.NotificationConfig,
         task_id: Optional[UUID] = None,
         report: Optional[Report] = None,
     ) -> responses.NotificationTestResponse:
         """Test a notification template"""
 
-        if task_id is None and report is None:
-            raise Exception("must specify either task_id or report")
-
-        endpoint = Endpoint(self.onefuzz)
         if task_id is not None:
             task = self.onefuzz.tasks.get(task_id)
-            input_blob_ref = BlobRef(
-                account="dummy-storage-account",
-                container="test-notification-crashes",
-                name="fake-crash-sample",
-            )
-
-        if report is None:
-            report = self._create_report(
-                task.job_id, task.task_id, "fake_target.exe", input_blob_ref
-            )
-
-        if task is not None:
-            report.task_id = task.task_id
-            report.job_id = task.job_id
+            if report is None:
+                input_blob_ref = BlobRef(
+                    account="dummy-storage-account",
+                    container="test-notification-crashes",
+                    name="fake-crash-sample",
+                )
+                report = self._create_report(
+                    task.job_id, task.task_id, "fake_target.exe", input_blob_ref
+                )
+            else:
+                report.task_id = task.task_id
+                report.job_id = task.job_id
+        elif report is None:
+            raise Exception("must specify either task_id or report")
 
         report.report_url = "https://dummy-container.blob.core.windows.net/dummy-reports/dummy-report.json"
 
+        endpoint = Endpoint(self.onefuzz)
         return endpoint._req_model(
             "POST",
             responses.NotificationTestResponse,
             data=requests.NotificationTest(
                 report=report,
                 notification=models.Notification(
                     container=Container("test-notification-reports"),
```

### Comparing `onefuzz-8.5.0/onefuzz/job_templates/builder.py` & `onefuzz-8.6.0/onefuzz/job_templates/builder.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/job_templates/cache.py` & `onefuzz-8.6.0/onefuzz/job_templates/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/job_templates/handlers.py` & `onefuzz-8.6.0/onefuzz/job_templates/handlers.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/job_templates/job_monitor.py` & `onefuzz-8.6.0/onefuzz/job_templates/job_monitor.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/job_templates/main.py` & `onefuzz-8.6.0/onefuzz/job_templates/main.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/job_templates/manage.py` & `onefuzz-8.6.0/onefuzz/job_templates/manage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/opentelemetry_exporter.py` & `onefuzz-8.6.0/onefuzz/opentelemetry_exporter.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/rdp.py` & `onefuzz-8.6.0/onefuzz/rdp.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/ssh.py` & `onefuzz-8.6.0/onefuzz/ssh.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/status/cache.py` & `onefuzz-8.6.0/onefuzz/status/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/status/cmd.py` & `onefuzz-8.6.0/onefuzz/status/cmd.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/status/raw.py` & `onefuzz-8.6.0/onefuzz/status/raw.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/status/signalr.py` & `onefuzz-8.6.0/onefuzz/status/signalr.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/status/top.py` & `onefuzz-8.6.0/onefuzz/status/top.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/status/top_view.py` & `onefuzz-8.6.0/onefuzz/status/top_view.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/template.py` & `onefuzz-8.6.0/onefuzz/template.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/templates/__init__.py` & `onefuzz-8.6.0/onefuzz/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/templates/afl.py` & `onefuzz-8.6.0/onefuzz/templates/afl.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/templates/libfuzzer.py` & `onefuzz-8.6.0/onefuzz/templates/libfuzzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,14 +496,15 @@
             module_allowlist=module_allowlist_blob_name,
             source_allowlist=source_allowlist_blob_name,
             analyzer_exe=analyzer_exe,
             analyzer_options=analyzer_options,
             analyzer_env=analyzer_env,
             tools=tools,
             task_env=task_env,
+            target_timeout=target_timeout,
         )
 
         self.logger.info("done creating tasks")
         helper.wait()
         return helper.job
 
     def merge(
```

### Comparing `onefuzz-8.5.0/onefuzz/templates/ossfuzz.py` & `onefuzz-8.6.0/onefuzz/templates/ossfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/templates/radamsa.py` & `onefuzz-8.6.0/onefuzz/templates/radamsa.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz/templates/regression.py` & `onefuzz-8.6.0/onefuzz/templates/regression.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/onefuzz.egg-info/PKG-INFO` & `onefuzz-8.6.0/onefuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 8.5.0
+Version: 8.6.0
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-8.5.0/onefuzz.egg-info/SOURCES.txt` & `onefuzz-8.6.0/onefuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/requirements.txt` & `onefuzz-8.6.0/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 PyJWT>=2.4.0
 opentelemetry-api==1.16.0
 opentelemetry-sdk==1.16.0
 opentelemetry-instrumentation-requests==0.37b0
 # install rsa version >=4.7 to fix CVE-2020-25658
 rsa>=4.7
 # onefuzztypes version is set during build
-onefuzztypes==8.5.0
+onefuzztypes==8.6.0
```

### Comparing `onefuzz-8.5.0/setup.py` & `onefuzz-8.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.5.0/tests/test_template_helper.py` & `onefuzz-8.6.0/tests/test_template_helper.py`

 * *Files identical despite different names*

