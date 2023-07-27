# Comparing `tmp/kopf-1.36.1.tar.gz` & `tmp/kopf-1.36.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kopf-1.36.1.tar", last modified: Sat May  6 17:02:19 2023, max compression
+gzip compressed data, was "kopf-1.36.2.tar", last modified: Thu Jul 27 10:50:48 2023, max compression
```

## Comparing `kopf-1.36.1.tar` & `kopf-1.36.2.tar`

### file list

```diff
@@ -1,475 +1,475 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.741712 kopf-1.36.1/
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-06 17:02:08.000000 kopf-1.36.1/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.689712 kopf-1.36.1/.github/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.689712 kopf-1.36.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/ISSUE_TEMPLATE/bug-report.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/ISSUE_TEMPLATE/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/ISSUE_TEMPLATE/feature-request.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/ISSUE_TEMPLATE/question.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.689712 kopf-1.36.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     4336 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     5113 2023-05-06 17:02:08.000000 kopf-1.36.1/.github/workflows/thorough.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-05-06 17:02:08.000000 kopf-1.36.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-05-06 17:02:08.000000 kopf-1.36.1/.importlinter
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-06 17:02:08.000000 kopf-1.36.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-06 17:02:08.000000 kopf-1.36.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-05-06 17:02:08.000000 kopf-1.36.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-05-06 17:02:08.000000 kopf-1.36.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-05-06 17:02:08.000000 kopf-1.36.1/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (122)     3973 2023-05-06 17:02:08.000000 kopf-1.36.1/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-05-06 17:02:08.000000 kopf-1.36.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-06 17:02:08.000000 kopf-1.36.1/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (122)     9006 2023-05-06 17:02:19.741712 kopf-1.36.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7612 2023-05-06 17:02:08.000000 kopf-1.36.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-06 17:02:08.000000 kopf-1.36.1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (122)     3588 2023-05-06 17:02:08.000000 kopf-1.36.1/_importlinter_conditional.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (122)    30976 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/admission.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5034 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/alternatives.rst
--rw-r--r--   0 runner    (1001) docker     (122)   815980 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/architecture-layers.png
--rw-r--r--   0 runner    (1001) docker     (122)     6656 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/architecture-layers.xml
--rw-r--r--   0 runner    (1001) docker     (122)     5384 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/async.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7474 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/authentication.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3295 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/concepts.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2728 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)    21375 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/continuity.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4318 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)    13470 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/daemons.rst
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/deployment-depl.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/deployment-rbac.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5143 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/embedding.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (122)    12679 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/filters.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10116 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/handlers.rst
--rw-r--r--   0 runner    (1001) docker     (122)    12768 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/hierarchies.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/idempotence.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    19300 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/indexing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (122)    12007 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/kwargs.rst
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/loading.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/memos.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/minikube.rst
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/naming.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6472 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/peering.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3244 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/probing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/reconciliation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7396 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/resources.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/results.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/scopes.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/shutdown.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/startup.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6679 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/timers.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/tips-and-tricks.rst
--rw-r--r--   0 runner    (1001) docker     (122)      862 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/vision.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/docs/walkthrough/
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/cleanup.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/creation.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2458 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/deletion.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4314 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/diffs.rst
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/prerequisites.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3015 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/problem.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/resources.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6290 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/starting.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-05-06 17:02:08.000000 kopf-1.36.1/docs/walkthrough/updates.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/examples/01-minimal/
--rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/01-minimal/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/01-minimal/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/examples/02-children/
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/02-children/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      987 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/02-children/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/examples/03-exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)      977 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/03-exceptions/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/03-exceptions/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.697712 kopf-1.36.1/examples/04-events/
--rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/04-events/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/04-events/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/05-handlers/
--rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/05-handlers/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/05-handlers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/06-peering/
--rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/06-peering/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/06-peering/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/07-subhandlers/
--rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/07-subhandlers/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/07-subhandlers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/08-events/
--rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/08-events/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/08-events/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/09-testing/
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/09-testing/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/09-testing/example.py
--rw-r--r--   0 runner    (1001) docker     (122)     2217 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/09-testing/test_example_09.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/10-builtins/
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/10-builtins/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/10-builtins/example.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/10-builtins/test_example_10.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/11-filtering-handlers/
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/11-filtering-handlers/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/11-filtering-handlers/example.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/11-filtering-handlers/test_example_11.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/12-embedded/
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/12-embedded/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/12-embedded/example.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/12-embedded/test_nothing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/13-hooks/
--rw-r--r--   0 runner    (1001) docker     (122)     3494 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/13-hooks/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/13-hooks/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/14-daemons/
--rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/14-daemons/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/15-timers/
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/15-timers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/16-indexing/
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/16-indexing/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/17-admission/
--rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/17-admission/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.701712 kopf-1.36.1/examples/99-all-at-once/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/99-all-at-once/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     3291 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/99-all-at-once/example.py
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/crd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/obj.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-06 17:02:08.000000 kopf-1.36.1/examples/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.705712 kopf-1.36.1/kopf/
--rw-r--r--   0 runner    (1001) docker     (122)     5798 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.705712 kopf-1.36.1/kopf/_cogs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.705712 kopf-1.36.1/kopf/_cogs/aiokits/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aioadapters.py
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aiobindings.py
--rw-r--r--   0 runner    (1001) docker     (122)     7613 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aioenums.py
--rw-r--r--   0 runner    (1001) docker     (122)    16483 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aiotasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aiotime.py
--rw-r--r--   0 runner    (1001) docker     (122)     5412 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aiotoggles.py
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/aiokits/aiovalues.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.709712 kopf-1.36.1/kopf/_cogs/clients/
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8911 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     8087 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/creating.py
--rw-r--r--   0 runner    (1001) docker     (122)     4603 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4085 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/fetching.py
--rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/patching.py
--rw-r--r--   0 runner    (1001) docker     (122)     4479 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/scanning.py
--rw-r--r--   0 runner    (1001) docker     (122)    11684 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/clients/watching.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.709712 kopf-1.36.1/kopf/_cogs/configs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16266 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/configs/configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    13196 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/configs/conventions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9210 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/configs/diffbase.py
--rw-r--r--   0 runner    (1001) docker     (122)    15586 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/configs/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.709712 kopf-1.36.1/kopf/_cogs/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/helpers/hostnames.py
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/helpers/loaders.py
--rw-r--r--   0 runner    (1001) docker     (122)     1672 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/helpers/thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (122)      906 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/helpers/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/helpers/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.709712 kopf-1.36.1/kopf/_cogs/structs/
--rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8109 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/bodies.py
--rw-r--r--   0 runner    (1001) docker     (122)    16065 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)    12021 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/dicts.py
--rw-r--r--   0 runner    (1001) docker     (122)     6222 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/diffs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/ephemera.py
--rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/finalizers.py
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/ids.py
--rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/patches.py
--rw-r--r--   0 runner    (1001) docker     (122)    22210 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/references.py
--rw-r--r--   0 runner    (1001) docker     (122)     3752 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_cogs/structs/reviews.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.709712 kopf-1.36.1/kopf/_core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.713712 kopf-1.36.1/kopf/_core/actions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6146 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/application.py
--rw-r--r--   0 runner    (1001) docker     (122)    14779 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/execution.py
--rw-r--r--   0 runner    (1001) docker     (122)     5963 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/invocation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/lifecycles.py
--rw-r--r--   0 runner    (1001) docker     (122)     8220 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/loggers.py
--rw-r--r--   0 runner    (1001) docker     (122)    15223 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/progression.py
--rw-r--r--   0 runner    (1001) docker     (122)     3486 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/actions/throttlers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.713712 kopf-1.36.1/kopf/_core/engines/
--rw-r--r--   0 runner    (1001) docker     (122)      377 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5628 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/activities.py
--rw-r--r--   0 runner    (1001) docker     (122)    19689 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/admission.py
--rw-r--r--   0 runner    (1001) docker     (122)    26590 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/daemons.py
--rw-r--r--   0 runner    (1001) docker     (122)    12333 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/indexing.py
--rw-r--r--   0 runner    (1001) docker     (122)    12443 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/peering.py
--rw-r--r--   0 runner    (1001) docker     (122)     8534 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/posting.py
--rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/engines/probing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.713712 kopf-1.36.1/kopf/_core/intents/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10586 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)    11464 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/causes.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)    10892 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/piggybacking.py
--rw-r--r--   0 runner    (1001) docker     (122)    21818 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/registries.py
--rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/intents/stoppers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.713712 kopf-1.36.1/kopf/_core/reactor/
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/inventory.py
--rw-r--r--   0 runner    (1001) docker     (122)    15421 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/observation.py
--rw-r--r--   0 runner    (1001) docker     (122)    11714 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/orchestration.py
--rw-r--r--   0 runner    (1001) docker     (122)    20921 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/processing.py
--rw-r--r--   0 runner    (1001) docker     (122)    17116 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/queueing.py
--rw-r--r--   0 runner    (1001) docker     (122)    24225 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/running.py
--rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_core/reactor/subhandling.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.717712 kopf-1.36.1/kopf/_kits/
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_kits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11261 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_kits/hierarchies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_kits/loops.py
--rw-r--r--   0 runner    (1001) docker     (122)     6247 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_kits/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_kits/webhacks.py
--rw-r--r--   0 runner    (1001) docker     (122)    30289 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/_kits/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (122)     7565 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    42263 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/on.py
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-06 17:02:08.000000 kopf-1.36.1/kopf/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.705712 kopf-1.36.1/kopf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9006 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12417 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 17:02:19.000000 kopf-1.36.1/kopf.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-05-06 17:02:08.000000 kopf-1.36.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-05-06 17:02:08.000000 kopf-1.36.1/peering.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-06 17:02:08.000000 kopf-1.36.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-05-06 17:02:08.000000 kopf-1.36.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-06 17:02:19.741712 kopf-1.36.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-05-06 17:02:08.000000 kopf-1.36.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.717712 kopf-1.36.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.717712 kopf-1.36.1/tests/admission/
--rw-r--r--   0 runner    (1001) docker     (122)     4592 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     8414 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_admission_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3009 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_admission_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_certificates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_jsonpatch.py
--rw-r--r--   0 runner    (1001) docker     (122)     9185 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_managed_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_serving_ephemeral_memos.py
--rw-r--r--   0 runner    (1001) docker     (122)     7830 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_serving_handler_selection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_serving_kwargs_passthrough.py
--rw-r--r--   0 runner    (1001) docker     (122)     6849 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_serving_responses.py
--rw-r--r--   0 runner    (1001) docker     (122)     4211 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_webhook_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_webhook_ngrok.py
--rw-r--r--   0 runner    (1001) docker     (122)     5264 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/admission/test_webhook_server.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.721712 kopf-1.36.1/tests/apis/
--rw-r--r--   0 runner    (1001) docker     (122)    10028 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/apis/test_api_requests.py
--rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/apis/test_default_namespace.py
--rw-r--r--   0 runner    (1001) docker     (122)     9346 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/apis/test_error_retries.py
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/apis/test_iterjsonlines.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.721712 kopf-1.36.1/tests/authentication/
--rw-r--r--   0 runner    (1001) docker     (122)     2429 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_connectioninfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     8916 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)    10189 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_login_kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (122)     3488 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_login_serviceaccount.py
--rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_reauthentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_tempfiles.py
--rw-r--r--   0 runner    (1001) docker     (122)     7474 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/authentication/test_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.721712 kopf-1.36.1/tests/basic-structs/
--rw-r--r--   0 runner    (1001) docker     (122)     3317 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/basic-structs/test_causes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2892 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/basic-structs/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1590 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/basic-structs/test_memories.py
--rw-r--r--   0 runner    (1001) docker     (122)     1858 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/basic-structs/test_memos.py
--rw-r--r--   0 runner    (1001) docker     (122)    11433 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/basic-structs/test_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.721712 kopf-1.36.1/tests/causation/
--rw-r--r--   0 runner    (1001) docker     (122)     8417 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/causation/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)    12825 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/causation/test_kwargs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.721712 kopf-1.36.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     1527 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/cli/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/cli/test_help.py
--rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/cli/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/cli/test_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/cli/test_preloading.py
--rw-r--r--   0 runner    (1001) docker     (122)    24579 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.725712 kopf-1.36.1/tests/dicts/
--rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_cherrypicking.py
--rw-r--r--   0 runner    (1001) docker     (122)     5085 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_dictviews.py
--rw-r--r--   0 runner    (1001) docker     (122)      953 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_ensuring.py
--rw-r--r--   0 runner    (1001) docker     (122)      918 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_removing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5402 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_resolving.py
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/dicts/test_walking.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.725712 kopf-1.36.1/tests/diffs/
--rw-r--r--   0 runner    (1001) docker     (122)     5355 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/diffs/test_calculation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/diffs/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/diffs/test_reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.725712 kopf-1.36.1/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/e2e/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     9649 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/e2e/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.725712 kopf-1.36.1/tests/handling/
--rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.725712 kopf-1.36.1/tests/handling/daemons/
--rw-r--r--   0 runner    (1001) docker     (122)     3893 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5763 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_daemon_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_daemon_filtration.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_daemon_rematching.py
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_daemon_spawning.py
--rw-r--r--   0 runner    (1001) docker     (122)    10261 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_daemon_termination.py
--rw-r--r--   0 runner    (1001) docker     (122)     6267 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_timer_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_timer_filtration.py
--rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_timer_intervals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/daemons/test_timer_triggering.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.729712 kopf-1.36.1/tests/handling/indexing/
--rw-r--r--   0 runner    (1001) docker     (122)      621 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/indexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3817 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/indexing/test_blocking_until_indexed.py
--rw-r--r--   0 runner    (1001) docker     (122)     8776 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/indexing/test_index_exclusion.py
--rw-r--r--   0 runner    (1001) docker     (122)     4899 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/indexing/test_index_population.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.729712 kopf-1.36.1/tests/handling/subhandling/
--rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/subhandling/test_subhandling.py
--rw-r--r--   0 runner    (1001) docker     (122)     6167 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_activity_triggering.py
--rw-r--r--   0 runner    (1001) docker     (122)     7416 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_cause_handling.py
--rw-r--r--   0 runner    (1001) docker     (122)     5422 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_cause_logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_delays.py
--rw-r--r--   0 runner    (1001) docker     (122)     6120 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_event_handling.py
--rw-r--r--   0 runner    (1001) docker     (122)     4818 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_multistep.py
--rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_no_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1879 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_parametrization.py
--rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_retrying_limits.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/handling/test_timing_consistency.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.729712 kopf-1.36.1/tests/hierarchies/
--rw-r--r--   0 runner    (1001) docker     (122)      916 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4710 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/test_contextual_owner.py
--rw-r--r--   0 runner    (1001) docker     (122)     9396 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/test_labelling.py
--rw-r--r--   0 runner    (1001) docker     (122)    11783 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/test_name_harmonizing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5895 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/test_namespace_adjusting.py
--rw-r--r--   0 runner    (1001) docker     (122)    10983 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/test_owner_referencing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/hierarchies/test_type_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.729712 kopf-1.36.1/tests/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)     5298 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/invocations/test_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.729712 kopf-1.36.1/tests/k8s/
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_creating.py
--rw-r--r--   0 runner    (1001) docker     (122)     3882 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     5785 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_list_objs.py
--rw-r--r--   0 runner    (1001) docker     (122)     9822 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_patching.py
--rw-r--r--   0 runner    (1001) docker     (122)    13308 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_scanning.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_watching_bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_watching_continuously.py
--rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_watching_infinitely.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/k8s/test_watching_with_freezes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.729712 kopf-1.36.1/tests/lifecycles/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/lifecycles/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/lifecycles/test_global_defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)     3691 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/lifecycles/test_handler_selection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/lifecycles/test_real_invocation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/logging/
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/logging/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/logging/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/logging/test_formatters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/logging/test_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/observation/
--rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/observation/test_processing_of_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     8698 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/observation/test_processing_of_resources.py
--rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/observation/test_revision_of_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     8324 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/observation/test_revision_of_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/orchestration/
--rw-r--r--   0 runner    (1001) docker     (122)     8535 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/orchestration/test_task_adjustments.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/peering/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    11445 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/test_freeze_mode.py
--rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/test_id_generation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/test_keepalive.py
--rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/test_peer_patching.py
--rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/test_peers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/peering/test_resource_guessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/persistence/
--rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/persistence/test_annotations_hashing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5597 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/persistence/test_essences.py
--rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/persistence/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (122)    33091 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/persistence/test_states.py
--rw-r--r--   0 runner    (1001) docker     (122)     6181 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/persistence/test_storing_of_diffbase.py
--rw-r--r--   0 runner    (1001) docker     (122)    12624 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/persistence/test_storing_of_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/posting/
--rw-r--r--   0 runner    (1001) docker     (122)      485 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/posting/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     4163 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/posting/test_log2k8s.py
--rw-r--r--   0 runner    (1001) docker     (122)     4642 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/posting/test_poster.py
--rw-r--r--   0 runner    (1001) docker     (122)     3613 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/posting/test_threadsafety.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.733712 kopf-1.36.1/tests/primitives/
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/primitives/test_conditions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/primitives/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/primitives/test_flags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2783 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/primitives/test_toggles.py
--rw-r--r--   0 runner    (1001) docker     (122)     9213 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/primitives/test_togglesets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.737712 kopf-1.36.1/tests/reactor/
--rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/reactor/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5877 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/reactor/test_patching_inconsistencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    10090 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/reactor/test_queueing.py
--rw-r--r--   0 runner    (1001) docker     (122)      877 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/reactor/test_uids.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.737712 kopf-1.36.1/tests/references/
--rw-r--r--   0 runner    (1001) docker     (122)     3005 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/references/test_backbone.py
--rw-r--r--   0 runner    (1001) docker     (122)     2942 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/references/test_namespace_matching.py
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/references/test_namespace_selection.py
--rw-r--r--   0 runner    (1001) docker     (122)     7038 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/references/test_selector_matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     8577 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/references/test_selector_parsing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/references/test_selector_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.737712 kopf-1.36.1/tests/registries/
--rw-r--r--   0 runner    (1001) docker     (122)     6122 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (122)    23936 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_default_registry.py
--rw-r--r--   0 runner    (1001) docker     (122)     6010 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_handler_getting.py
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_id_detection.py
--rw-r--r--   0 runner    (1001) docker     (122)    29077 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_matching_for_changing.py
--rw-r--r--   0 runner    (1001) docker     (122)    17265 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_matching_for_indexing.py
--rw-r--r--   0 runner    (1001) docker     (122)    17733 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_matching_for_spawning.py
--rw-r--r--   0 runner    (1001) docker     (122)    17321 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_matching_for_watching.py
--rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_matching_of_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_matching_of_resources.py
--rw-r--r--   0 runner    (1001) docker     (122)     4642 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_requires_finalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2184 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_resumes_mixed_in.py
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/registries/test_subhandlers_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.737712 kopf-1.36.1/tests/settings/
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/settings/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/settings/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_absent_modules.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (122)     1985 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_filtering_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_finalizers.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_it.py
--rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_liveness.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/test_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.737712 kopf-1.36.1/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/testing/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.741712 kopf-1.36.1/tests/timing/
--rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/timing/test_sleeping.py
--rw-r--r--   0 runner    (1001) docker     (122)    11112 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/timing/test_throttling.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.685712 kopf-1.36.1/tests/utilities/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.741712 kopf-1.36.1/tests/utilities/aiotasks/
--rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_coro_cancellation.py
--rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_task_creation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_task_guarding.py
--rw-r--r--   0 runner    (1001) docker     (122)      505 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_task_selection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_task_stopping.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-06 17:02:08.000000 kopf-1.36.1/tests/utilities/aiotasks/test_task_waiting.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 17:02:19.741712 kopf-1.36.1/tools/
--rwxr-xr-x   0 runner    (1001) docker     (122)      717 2023-05-06 17:02:08.000000 kopf-1.36.1/tools/install-kind.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      504 2023-05-06 17:02:08.000000 kopf-1.36.1/tools/install-kubectl.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      945 2023-05-06 17:02:08.000000 kopf-1.36.1/tools/install-minikube.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.344722 kopf-1.36.2/
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-27 10:50:37.000000 kopf-1.36.2/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.204723 kopf-1.36.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-27 10:50:37.000000 kopf-1.36.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-27 10:50:37.000000 kopf-1.36.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.208722 kopf-1.36.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-07-27 10:50:37.000000 kopf-1.36.2/.github/ISSUE_TEMPLATE/bug-report.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-07-27 10:50:37.000000 kopf-1.36.2/.github/ISSUE_TEMPLATE/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-07-27 10:50:37.000000 kopf-1.36.2/.github/ISSUE_TEMPLATE/feature-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-07-27 10:50:37.000000 kopf-1.36.2/.github/ISSUE_TEMPLATE/question.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-27 10:50:37.000000 kopf-1.36.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-07-27 10:50:37.000000 kopf-1.36.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.208722 kopf-1.36.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     4336 2023-07-27 10:50:37.000000 kopf-1.36.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-07-27 10:50:37.000000 kopf-1.36.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-07-27 10:50:37.000000 kopf-1.36.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     5113 2023-07-27 10:50:37.000000 kopf-1.36.2/.github/workflows/thorough.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-07-27 10:50:37.000000 kopf-1.36.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     2897 2023-07-27 10:50:37.000000 kopf-1.36.2/.importlinter
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-07-27 10:50:37.000000 kopf-1.36.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-07-27 10:50:37.000000 kopf-1.36.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-27 10:50:37.000000 kopf-1.36.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1595 2023-07-27 10:50:37.000000 kopf-1.36.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-27 10:50:37.000000 kopf-1.36.2/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3973 2023-07-27 10:50:37.000000 kopf-1.36.2/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-07-27 10:50:37.000000 kopf-1.36.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-27 10:50:37.000000 kopf-1.36.2/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (122)     9006 2023-07-27 10:50:48.344722 kopf-1.36.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7612 2023-07-27 10:50:37.000000 kopf-1.36.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-07-27 10:50:37.000000 kopf-1.36.2/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3588 2023-07-27 10:50:37.000000 kopf-1.36.2/_importlinter_conditional.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.228722 kopf-1.36.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (122)    30976 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/admission.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5034 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/alternatives.rst
+-rw-r--r--   0 runner    (1001) docker     (122)   815980 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/architecture-layers.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6656 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/architecture-layers.xml
+-rw-r--r--   0 runner    (1001) docker     (122)     5384 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/async.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7474 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3295 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2728 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21375 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2742 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/continuity.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4318 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    13470 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/daemons.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/deployment-depl.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/deployment-rbac.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5143 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12679 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/filters.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10116 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12768 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/hierarchies.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/idempotence.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    19300 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/indexing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12007 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/kwargs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/loading.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/memos.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/minikube.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/naming.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6472 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/peering.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3244 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/probing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/reconciliation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7396 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/results.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/scopes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/shutdown.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/startup.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6679 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/timers.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/tips-and-tricks.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1468 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/vision.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.232722 kopf-1.36.2/docs/walkthrough/
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/walkthrough/cleanup.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/walkthrough/creation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2458 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/walkthrough/deletion.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4314 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/walkthrough/diffs.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/walkthrough/prerequisites.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3015 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/walkthrough/problem.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/walkthrough/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6290 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/walkthrough/starting.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-07-27 10:50:37.000000 kopf-1.36.2/docs/walkthrough/updates.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.232722 kopf-1.36.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.232722 kopf-1.36.2/examples/01-minimal/
+-rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/01-minimal/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/01-minimal/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.236723 kopf-1.36.2/examples/02-children/
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/02-children/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      987 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/02-children/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.236723 kopf-1.36.2/examples/03-exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/03-exceptions/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1160 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/03-exceptions/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.236723 kopf-1.36.2/examples/04-events/
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/04-events/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/04-events/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.236723 kopf-1.36.2/examples/05-handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/05-handlers/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/05-handlers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.236723 kopf-1.36.2/examples/06-peering/
+-rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/06-peering/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/06-peering/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.236723 kopf-1.36.2/examples/07-subhandlers/
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/07-subhandlers/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/07-subhandlers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.236723 kopf-1.36.2/examples/08-events/
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/08-events/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/08-events/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.240723 kopf-1.36.2/examples/09-testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/09-testing/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/09-testing/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2217 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/09-testing/test_example_09.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.240723 kopf-1.36.2/examples/10-builtins/
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/10-builtins/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/10-builtins/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/10-builtins/test_example_10.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.240723 kopf-1.36.2/examples/11-filtering-handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/11-filtering-handlers/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/11-filtering-handlers/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/11-filtering-handlers/test_example_11.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.240723 kopf-1.36.2/examples/12-embedded/
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/12-embedded/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/12-embedded/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/12-embedded/test_nothing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.240723 kopf-1.36.2/examples/13-hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)     3494 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/13-hooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/13-hooks/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.244722 kopf-1.36.2/examples/14-daemons/
+-rw-r--r--   0 runner    (1001) docker     (122)     1645 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/14-daemons/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.244722 kopf-1.36.2/examples/15-timers/
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/15-timers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.244722 kopf-1.36.2/examples/16-indexing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/16-indexing/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.244722 kopf-1.36.2/examples/17-admission/
+-rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/17-admission/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.244722 kopf-1.36.2/examples/99-all-at-once/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/99-all-at-once/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3291 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/99-all-at-once/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/crd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/obj.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-27 10:50:37.000000 kopf-1.36.2/examples/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.248722 kopf-1.36.2/kopf/
+-rw-r--r--   0 runner    (1001) docker     (122)     5798 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.252722 kopf-1.36.2/kopf/_cogs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.256722 kopf-1.36.2/kopf/_cogs/aiokits/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/aiokits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/aiokits/aioadapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/aiokits/aiobindings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7613 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/aiokits/aioenums.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16483 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/aiokits/aiotasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/aiokits/aiotime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5412 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/aiokits/aiotoggles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/aiokits/aiovalues.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.264722 kopf-1.36.2/kopf/_cogs/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8911 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/clients/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8087 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/clients/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/clients/creating.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4603 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/clients/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4085 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/clients/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/clients/fetching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2898 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/clients/patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4481 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/clients/scanning.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11684 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/clients/watching.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.264722 kopf-1.36.2/kopf/_cogs/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16266 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/configs/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13196 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/configs/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9210 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/configs/diffbase.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15586 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/configs/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.264722 kopf-1.36.2/kopf/_cogs/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/helpers/hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/helpers/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1672 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/helpers/thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)      906 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/helpers/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/helpers/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.268722 kopf-1.36.2/kopf/_cogs/structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8109 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/structs/bodies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16065 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/structs/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12021 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/structs/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6222 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/structs/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2716 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/structs/ephemera.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1516 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/structs/finalizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/structs/ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3894 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/structs/patches.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22210 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/structs/references.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3752 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_cogs/structs/reviews.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.268722 kopf-1.36.2/kopf/_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.272722 kopf-1.36.2/kopf/_core/actions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6146 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/actions/application.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14779 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/actions/execution.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5963 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/actions/invocation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/actions/lifecycles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8220 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/actions/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15223 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/actions/progression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3486 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/actions/throttlers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.272722 kopf-1.36.2/kopf/_core/engines/
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5628 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/engines/activities.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19689 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/engines/admission.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26590 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/engines/daemons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12333 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/engines/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12443 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/engines/peering.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8534 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/engines/posting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/engines/probing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.276722 kopf-1.36.2/kopf/_core/intents/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/intents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10586 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/intents/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11464 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/intents/causes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/intents/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/intents/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10892 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/intents/piggybacking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21818 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/intents/registries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1687 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/intents/stoppers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.280722 kopf-1.36.2/kopf/_core/reactor/
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/reactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5756 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/reactor/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15421 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/reactor/observation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11714 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/reactor/orchestration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20921 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/reactor/processing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17116 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/reactor/queueing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24225 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/reactor/running.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_core/reactor/subhandling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.284722 kopf-1.36.2/kopf/_kits/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_kits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11261 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_kits/hierarchies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_kits/loops.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6247 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_kits/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_kits/webhacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30289 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/_kits/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7565 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42263 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/on.py
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-27 10:50:37.000000 kopf-1.36.2/kopf/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.252722 kopf-1.36.2/kopf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9006 2023-07-27 10:50:48.000000 kopf-1.36.2/kopf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12417 2023-07-27 10:50:48.000000 kopf-1.36.2/kopf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 10:50:48.000000 kopf-1.36.2/kopf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-07-27 10:50:48.000000 kopf-1.36.2/kopf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-07-27 10:50:48.000000 kopf-1.36.2/kopf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-27 10:50:48.000000 kopf-1.36.2/kopf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 10:50:48.000000 kopf-1.36.2/kopf.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-27 10:50:37.000000 kopf-1.36.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-07-27 10:50:37.000000 kopf-1.36.2/peering.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-27 10:50:37.000000 kopf-1.36.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-27 10:50:37.000000 kopf-1.36.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 10:50:48.344722 kopf-1.36.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2743 2023-07-27 10:50:37.000000 kopf-1.36.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.288722 kopf-1.36.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.292722 kopf-1.36.2/tests/admission/
+-rw-r--r--   0 runner    (1001) docker     (122)     4592 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8414 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/test_admission_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3009 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/test_admission_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/test_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/test_jsonpatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9185 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/test_managed_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/test_serving_ephemeral_memos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7830 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/test_serving_handler_selection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/test_serving_kwargs_passthrough.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6849 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/test_serving_responses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4211 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/test_webhook_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/test_webhook_ngrok.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5264 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/admission/test_webhook_server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.296722 kopf-1.36.2/tests/apis/
+-rw-r--r--   0 runner    (1001) docker     (122)    10028 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/apis/test_api_requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/apis/test_default_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9346 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/apis/test_error_retries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/apis/test_iterjsonlines.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.300722 kopf-1.36.2/tests/authentication/
+-rw-r--r--   0 runner    (1001) docker     (122)     2429 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/authentication/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/authentication/test_connectioninfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8916 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/authentication/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10189 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/authentication/test_login_kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3488 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/authentication/test_login_serviceaccount.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/authentication/test_reauthentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/authentication/test_tempfiles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7474 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/authentication/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.300722 kopf-1.36.2/tests/basic-structs/
+-rw-r--r--   0 runner    (1001) docker     (122)     3317 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/basic-structs/test_causes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2892 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/basic-structs/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1590 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/basic-structs/test_memories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1858 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/basic-structs/test_memos.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11433 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/basic-structs/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.300722 kopf-1.36.2/tests/causation/
+-rw-r--r--   0 runner    (1001) docker     (122)     8417 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/causation/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12825 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/causation/test_kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.304722 kopf-1.36.2/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     1527 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/cli/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/cli/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/cli/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/cli/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/cli/test_preloading.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24579 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.308722 kopf-1.36.2/tests/dicts/
+-rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/dicts/test_cherrypicking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5085 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/dicts/test_dictviews.py
+-rw-r--r--   0 runner    (1001) docker     (122)      953 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/dicts/test_ensuring.py
+-rw-r--r--   0 runner    (1001) docker     (122)      918 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/dicts/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/dicts/test_removing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5402 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/dicts/test_resolving.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/dicts/test_walking.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.308722 kopf-1.36.2/tests/diffs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5355 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/diffs/test_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/diffs/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/diffs/test_reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.308722 kopf-1.36.2/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (122)     1537 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/e2e/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9649 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/e2e/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.316722 kopf-1.36.2/tests/handling/
+-rw-r--r--   0 runner    (1001) docker     (122)     7457 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.316722 kopf-1.36.2/tests/handling/daemons/
+-rw-r--r--   0 runner    (1001) docker     (122)     3893 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/daemons/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5763 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/daemons/test_daemon_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2502 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/daemons/test_daemon_filtration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/daemons/test_daemon_rematching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/daemons/test_daemon_spawning.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10261 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/daemons/test_daemon_termination.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6267 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/daemons/test_timer_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/daemons/test_timer_filtration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/daemons/test_timer_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1454 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/daemons/test_timer_triggering.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.316722 kopf-1.36.2/tests/handling/indexing/
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/indexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3817 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/indexing/test_blocking_until_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8776 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/indexing/test_index_exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4899 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/indexing/test_index_population.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.316722 kopf-1.36.2/tests/handling/subhandling/
+-rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/subhandling/test_subhandling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6167 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/test_activity_triggering.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7416 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/test_cause_handling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5422 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/test_cause_logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/test_delays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6120 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/test_event_handling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4818 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/test_multistep.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/test_no_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1879 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/test_parametrization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/test_retrying_limits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/handling/test_timing_consistency.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.320722 kopf-1.36.2/tests/hierarchies/
+-rw-r--r--   0 runner    (1001) docker     (122)      916 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/hierarchies/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4710 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/hierarchies/test_contextual_owner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9396 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/hierarchies/test_labelling.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11783 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/hierarchies/test_name_harmonizing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5895 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/hierarchies/test_namespace_adjusting.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10983 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/hierarchies/test_owner_referencing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/hierarchies/test_type_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.320722 kopf-1.36.2/tests/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)     5298 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/invocations/test_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.320722 kopf-1.36.2/tests/k8s/
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/k8s/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2637 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/k8s/test_creating.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3882 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/k8s/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5785 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/k8s/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/k8s/test_list_objs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9822 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/k8s/test_patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13308 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/k8s/test_scanning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/k8s/test_watching_bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/k8s/test_watching_continuously.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/k8s/test_watching_infinitely.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/k8s/test_watching_with_freezes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.320722 kopf-1.36.2/tests/lifecycles/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/lifecycles/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/lifecycles/test_global_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3691 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/lifecycles/test_handler_selection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/lifecycles/test_real_invocation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.324722 kopf-1.36.2/tests/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/logging/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/logging/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/logging/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/logging/test_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.324722 kopf-1.36.2/tests/observation/
+-rw-r--r--   0 runner    (1001) docker     (122)     2144 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/observation/test_processing_of_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8698 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/observation/test_processing_of_resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/observation/test_revision_of_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8324 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/observation/test_revision_of_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.324722 kopf-1.36.2/tests/orchestration/
+-rw-r--r--   0 runner    (1001) docker     (122)     8535 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/orchestration/test_task_adjustments.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.328722 kopf-1.36.2/tests/peering/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/peering/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11445 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/peering/test_freeze_mode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4300 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/peering/test_id_generation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/peering/test_keepalive.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/peering/test_peer_patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/peering/test_peers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/peering/test_resource_guessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.328722 kopf-1.36.2/tests/persistence/
+-rw-r--r--   0 runner    (1001) docker     (122)     7354 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/persistence/test_annotations_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5597 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/persistence/test_essences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/persistence/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33091 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/persistence/test_states.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6181 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/persistence/test_storing_of_diffbase.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12624 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/persistence/test_storing_of_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.328722 kopf-1.36.2/tests/posting/
+-rw-r--r--   0 runner    (1001) docker     (122)      485 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/posting/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4163 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/posting/test_log2k8s.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4642 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/posting/test_poster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3613 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/posting/test_threadsafety.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.332722 kopf-1.36.2/tests/primitives/
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/primitives/test_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/primitives/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/primitives/test_flags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2783 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/primitives/test_toggles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9213 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/primitives/test_togglesets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.332722 kopf-1.36.2/tests/reactor/
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/reactor/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5877 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/reactor/test_patching_inconsistencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10090 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/reactor/test_queueing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/reactor/test_uids.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.336722 kopf-1.36.2/tests/references/
+-rw-r--r--   0 runner    (1001) docker     (122)     3005 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/references/test_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2942 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/references/test_namespace_matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/references/test_namespace_selection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7038 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/references/test_selector_matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8577 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/references/test_selector_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/references/test_selector_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.340722 kopf-1.36.2/tests/registries/
+-rw-r--r--   0 runner    (1001) docker     (122)     6122 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23936 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_default_registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6010 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_handler_getting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_id_detection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29077 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_matching_for_changing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17265 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_matching_for_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17733 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_matching_for_spawning.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17321 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_matching_for_watching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_matching_of_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_matching_of_resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4642 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_requires_finalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2184 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_resumes_mixed_in.py
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/registries/test_subhandlers_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.340722 kopf-1.36.2/tests/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/settings/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/settings/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/test_absent_modules.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1985 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/test_filtering_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/test_finalizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/test_it.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/test_liveness.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/test_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.340722 kopf-1.36.2/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)     3534 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/testing/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.340722 kopf-1.36.2/tests/timing/
+-rw-r--r--   0 runner    (1001) docker     (122)     2072 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/timing/test_sleeping.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11112 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/timing/test_throttling.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.196723 kopf-1.36.2/tests/utilities/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.344722 kopf-1.36.2/tests/utilities/aiotasks/
+-rw-r--r--   0 runner    (1001) docker     (122)     2495 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/utilities/aiotasks/test_coro_cancellation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5145 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/utilities/aiotasks/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/utilities/aiotasks/test_task_creation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/utilities/aiotasks/test_task_guarding.py
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/utilities/aiotasks/test_task_selection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/utilities/aiotasks/test_task_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-07-27 10:50:37.000000 kopf-1.36.2/tests/utilities/aiotasks/test_task_waiting.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 10:50:48.344722 kopf-1.36.2/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      717 2023-07-27 10:50:37.000000 kopf-1.36.2/tools/install-kind.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      504 2023-07-27 10:50:37.000000 kopf-1.36.2/tools/install-kubectl.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      945 2023-07-27 10:50:37.000000 kopf-1.36.2/tools/install-minikube.sh
```

### Comparing `kopf-1.36.1/.github/ISSUE_TEMPLATE/bug-report.yaml` & `kopf-1.36.2/.github/ISSUE_TEMPLATE/bug-report.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/.github/ISSUE_TEMPLATE/feature-request.yaml` & `kopf-1.36.2/.github/ISSUE_TEMPLATE/feature-request.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/.github/ISSUE_TEMPLATE/question.yaml` & `kopf-1.36.2/.github/ISSUE_TEMPLATE/question.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/.github/workflows/ci.yaml` & `kopf-1.36.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/.github/workflows/codeql.yml` & `kopf-1.36.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/.github/workflows/publish.yaml` & `kopf-1.36.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/.github/workflows/thorough.yaml` & `kopf-1.36.2/.github/workflows/thorough.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/.importlinter` & `kopf-1.36.2/.importlinter`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/.pre-commit-config.yaml` & `kopf-1.36.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/CODE_OF_CONDUCT.md` & `kopf-1.36.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/CONTRIBUTING.md` & `kopf-1.36.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/CONTRIBUTORS.md` & `kopf-1.36.2/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/DEVELOPMENT.md` & `kopf-1.36.2/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/LICENSE` & `kopf-1.36.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/PKG-INFO` & `kopf-1.36.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kopf
-Version: 1.36.1
+Version: 1.36.2
 Summary: Kubernetes Operator Pythonic Framework (Kopf)
 Home-page: https://github.com/nolar/kopf
 Author: Sergey Vasilyev
 Author-email: nolar@nolar.info
 Maintainer: Sergey Vasilyev
 Maintainer-email: nolar@nolar.info
 License: MIT
```

### Comparing `kopf-1.36.1/README.md` & `kopf-1.36.2/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/_importlinter_conditional.py` & `kopf-1.36.2/_importlinter_conditional.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/admission.rst` & `kopf-1.36.2/docs/admission.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/alternatives.rst` & `kopf-1.36.2/docs/alternatives.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/architecture-layers.png` & `kopf-1.36.2/docs/architecture-layers.png`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/architecture-layers.xml` & `kopf-1.36.2/docs/architecture-layers.xml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/architecture.rst` & `kopf-1.36.2/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/async.rst` & `kopf-1.36.2/docs/async.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/authentication.rst` & `kopf-1.36.2/docs/authentication.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/cli.rst` & `kopf-1.36.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/concepts.rst` & `kopf-1.36.2/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/conf.py` & `kopf-1.36.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/configuration.rst` & `kopf-1.36.2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/continuity.rst` & `kopf-1.36.2/docs/continuity.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/contributing.rst` & `kopf-1.36.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/daemons.rst` & `kopf-1.36.2/docs/daemons.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/deployment-rbac.yaml` & `kopf-1.36.2/docs/deployment-rbac.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/deployment.rst` & `kopf-1.36.2/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/embedding.rst` & `kopf-1.36.2/docs/embedding.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/errors.rst` & `kopf-1.36.2/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/events.rst` & `kopf-1.36.2/docs/events.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/filters.rst` & `kopf-1.36.2/docs/filters.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/handlers.rst` & `kopf-1.36.2/docs/handlers.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/hierarchies.rst` & `kopf-1.36.2/docs/hierarchies.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/idempotence.rst` & `kopf-1.36.2/docs/idempotence.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/index.rst` & `kopf-1.36.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/indexing.rst` & `kopf-1.36.2/docs/indexing.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/install.rst` & `kopf-1.36.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/kwargs.rst` & `kopf-1.36.2/docs/kwargs.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/loading.rst` & `kopf-1.36.2/docs/loading.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/memos.rst` & `kopf-1.36.2/docs/memos.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/minikube.rst` & `kopf-1.36.2/docs/minikube.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/peering.rst` & `kopf-1.36.2/docs/peering.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/probing.rst` & `kopf-1.36.2/docs/probing.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/reconciliation.rst` & `kopf-1.36.2/docs/reconciliation.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/resources.rst` & `kopf-1.36.2/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/results.rst` & `kopf-1.36.2/docs/results.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/scopes.rst` & `kopf-1.36.2/docs/scopes.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/shutdown.rst` & `kopf-1.36.2/docs/shutdown.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/startup.rst` & `kopf-1.36.2/docs/startup.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/testing.rst` & `kopf-1.36.2/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/timers.rst` & `kopf-1.36.2/docs/timers.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/tips-and-tricks.rst` & `kopf-1.36.2/docs/tips-and-tricks.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/troubleshooting.rst` & `kopf-1.36.2/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/vision.rst` & `kopf-1.36.2/docs/vision.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/walkthrough/creation.rst` & `kopf-1.36.2/docs/walkthrough/creation.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/walkthrough/deletion.rst` & `kopf-1.36.2/docs/walkthrough/deletion.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/walkthrough/diffs.rst` & `kopf-1.36.2/docs/walkthrough/diffs.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/walkthrough/prerequisites.rst` & `kopf-1.36.2/docs/walkthrough/prerequisites.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/walkthrough/problem.rst` & `kopf-1.36.2/docs/walkthrough/problem.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/walkthrough/resources.rst` & `kopf-1.36.2/docs/walkthrough/resources.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/walkthrough/starting.rst` & `kopf-1.36.2/docs/walkthrough/starting.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/docs/walkthrough/updates.rst` & `kopf-1.36.2/docs/walkthrough/updates.rst`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/01-minimal/README.md` & `kopf-1.36.2/examples/01-minimal/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/02-children/README.md` & `kopf-1.36.2/examples/02-children/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/02-children/example.py` & `kopf-1.36.2/examples/02-children/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/03-exceptions/README.md` & `kopf-1.36.2/examples/03-exceptions/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/03-exceptions/example.py` & `kopf-1.36.2/examples/03-exceptions/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/04-events/README.md` & `kopf-1.36.2/examples/04-events/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/04-events/example.py` & `kopf-1.36.2/examples/04-events/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/05-handlers/README.md` & `kopf-1.36.2/examples/05-handlers/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/05-handlers/example.py` & `kopf-1.36.2/examples/05-handlers/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/06-peering/README.md` & `kopf-1.36.2/examples/06-peering/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/07-subhandlers/README.md` & `kopf-1.36.2/examples/07-subhandlers/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/08-events/README.md` & `kopf-1.36.2/examples/08-events/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/09-testing/test_example_09.py` & `kopf-1.36.2/examples/09-testing/test_example_09.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/10-builtins/README.md` & `kopf-1.36.2/examples/10-builtins/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/10-builtins/example.py` & `kopf-1.36.2/examples/10-builtins/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/10-builtins/test_example_10.py` & `kopf-1.36.2/examples/10-builtins/test_example_10.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/11-filtering-handlers/README.md` & `kopf-1.36.2/examples/11-filtering-handlers/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/11-filtering-handlers/example.py` & `kopf-1.36.2/examples/11-filtering-handlers/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/11-filtering-handlers/test_example_11.py` & `kopf-1.36.2/examples/11-filtering-handlers/test_example_11.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/12-embedded/README.md` & `kopf-1.36.2/examples/12-embedded/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/12-embedded/example.py` & `kopf-1.36.2/examples/12-embedded/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/13-hooks/README.md` & `kopf-1.36.2/examples/13-hooks/README.md`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/13-hooks/example.py` & `kopf-1.36.2/examples/13-hooks/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/14-daemons/example.py` & `kopf-1.36.2/examples/14-daemons/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/16-indexing/example.py` & `kopf-1.36.2/examples/16-indexing/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/17-admission/example.py` & `kopf-1.36.2/examples/17-admission/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/99-all-at-once/example.py` & `kopf-1.36.2/examples/99-all-at-once/example.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/examples/crd.yaml` & `kopf-1.36.2/examples/crd.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/__init__.py` & `kopf-1.36.2/kopf/__init__.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/aiokits/aioadapters.py` & `kopf-1.36.2/kopf/_cogs/aiokits/aioadapters.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/aiokits/aiobindings.py` & `kopf-1.36.2/kopf/_cogs/aiokits/aiobindings.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/aiokits/aioenums.py` & `kopf-1.36.2/kopf/_cogs/aiokits/aioenums.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/aiokits/aiotasks.py` & `kopf-1.36.2/kopf/_cogs/aiokits/aiotasks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/aiokits/aiotime.py` & `kopf-1.36.2/kopf/_cogs/aiokits/aiotime.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/aiokits/aiotoggles.py` & `kopf-1.36.2/kopf/_cogs/aiokits/aiotoggles.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/aiokits/aiovalues.py` & `kopf-1.36.2/kopf/_cogs/aiokits/aiovalues.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/clients/__init__.py` & `kopf-1.36.2/kopf/_cogs/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/clients/api.py` & `kopf-1.36.2/kopf/_cogs/clients/api.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/clients/auth.py` & `kopf-1.36.2/kopf/_cogs/clients/auth.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/clients/creating.py` & `kopf-1.36.2/kopf/_cogs/clients/creating.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/clients/errors.py` & `kopf-1.36.2/kopf/_cogs/clients/errors.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/clients/events.py` & `kopf-1.36.2/kopf/_cogs/clients/events.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/clients/fetching.py` & `kopf-1.36.2/kopf/_cogs/clients/fetching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/clients/patching.py` & `kopf-1.36.2/kopf/_cogs/clients/patching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/clients/scanning.py` & `kopf-1.36.2/kopf/_cogs/clients/scanning.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,12 +114,12 @@
                 subresources=frozenset(
                     subresource['name'].split('/', 1)[-1]
                     for subresource in rsp.get('resources', [])
                     if subresource['name'].startswith(f'{resource["name"]}/')
                 ),
                 namespaced=resource['namespaced'],
                 preferred=preferred,
-                verbs=frozenset(resource.get('verbs', [])),
+                verbs=frozenset(resource.get('verbs') or []),
             )
             for resource in rsp.get('resources', [])
             if '/' not in resource['name']
         }
```

### Comparing `kopf-1.36.1/kopf/_cogs/clients/watching.py` & `kopf-1.36.2/kopf/_cogs/clients/watching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/configs/configuration.py` & `kopf-1.36.2/kopf/_cogs/configs/configuration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/configs/conventions.py` & `kopf-1.36.2/kopf/_cogs/configs/conventions.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/configs/diffbase.py` & `kopf-1.36.2/kopf/_cogs/configs/diffbase.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/configs/progress.py` & `kopf-1.36.2/kopf/_cogs/configs/progress.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/helpers/__init__.py` & `kopf-1.36.2/kopf/_cogs/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/helpers/hostnames.py` & `kopf-1.36.2/kopf/_cogs/helpers/hostnames.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/helpers/loaders.py` & `kopf-1.36.2/kopf/_cogs/helpers/loaders.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/helpers/thirdparty.py` & `kopf-1.36.2/kopf/_cogs/helpers/thirdparty.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/helpers/typedefs.py` & `kopf-1.36.2/kopf/_cogs/helpers/typedefs.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/helpers/versions.py` & `kopf-1.36.2/kopf/_cogs/helpers/versions.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/structs/bodies.py` & `kopf-1.36.2/kopf/_cogs/structs/bodies.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/structs/credentials.py` & `kopf-1.36.2/kopf/_cogs/structs/credentials.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/structs/dicts.py` & `kopf-1.36.2/kopf/_cogs/structs/dicts.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/structs/diffs.py` & `kopf-1.36.2/kopf/_cogs/structs/diffs.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/structs/ephemera.py` & `kopf-1.36.2/kopf/_cogs/structs/ephemera.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/structs/finalizers.py` & `kopf-1.36.2/kopf/_cogs/structs/finalizers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/structs/patches.py` & `kopf-1.36.2/kopf/_cogs/structs/patches.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/structs/references.py` & `kopf-1.36.2/kopf/_cogs/structs/references.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_cogs/structs/reviews.py` & `kopf-1.36.2/kopf/_cogs/structs/reviews.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/actions/application.py` & `kopf-1.36.2/kopf/_core/actions/application.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/actions/execution.py` & `kopf-1.36.2/kopf/_core/actions/execution.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/actions/invocation.py` & `kopf-1.36.2/kopf/_core/actions/invocation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/actions/lifecycles.py` & `kopf-1.36.2/kopf/_core/actions/lifecycles.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/actions/loggers.py` & `kopf-1.36.2/kopf/_core/actions/loggers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/actions/progression.py` & `kopf-1.36.2/kopf/_core/actions/progression.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/actions/throttlers.py` & `kopf-1.36.2/kopf/_core/actions/throttlers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/engines/activities.py` & `kopf-1.36.2/kopf/_core/engines/activities.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/engines/admission.py` & `kopf-1.36.2/kopf/_core/engines/admission.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/engines/daemons.py` & `kopf-1.36.2/kopf/_core/engines/daemons.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/engines/indexing.py` & `kopf-1.36.2/kopf/_core/engines/indexing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/engines/peering.py` & `kopf-1.36.2/kopf/_core/engines/peering.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/engines/posting.py` & `kopf-1.36.2/kopf/_core/engines/posting.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/engines/probing.py` & `kopf-1.36.2/kopf/_core/engines/probing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/intents/callbacks.py` & `kopf-1.36.2/kopf/_core/intents/callbacks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/intents/causes.py` & `kopf-1.36.2/kopf/_core/intents/causes.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/intents/filters.py` & `kopf-1.36.2/kopf/_core/intents/filters.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/intents/handlers.py` & `kopf-1.36.2/kopf/_core/intents/handlers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/intents/piggybacking.py` & `kopf-1.36.2/kopf/_core/intents/piggybacking.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/intents/registries.py` & `kopf-1.36.2/kopf/_core/intents/registries.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/intents/stoppers.py` & `kopf-1.36.2/kopf/_core/intents/stoppers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/reactor/inventory.py` & `kopf-1.36.2/kopf/_core/reactor/inventory.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/reactor/observation.py` & `kopf-1.36.2/kopf/_core/reactor/observation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/reactor/orchestration.py` & `kopf-1.36.2/kopf/_core/reactor/orchestration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/reactor/processing.py` & `kopf-1.36.2/kopf/_core/reactor/processing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/reactor/queueing.py` & `kopf-1.36.2/kopf/_core/reactor/queueing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/reactor/running.py` & `kopf-1.36.2/kopf/_core/reactor/running.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_core/reactor/subhandling.py` & `kopf-1.36.2/kopf/_core/reactor/subhandling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_kits/__init__.py` & `kopf-1.36.2/kopf/_kits/__init__.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_kits/hierarchies.py` & `kopf-1.36.2/kopf/_kits/hierarchies.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_kits/loops.py` & `kopf-1.36.2/kopf/_kits/loops.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_kits/runner.py` & `kopf-1.36.2/kopf/_kits/runner.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_kits/webhacks.py` & `kopf-1.36.2/kopf/_kits/webhacks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/_kits/webhooks.py` & `kopf-1.36.2/kopf/_kits/webhooks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/cli.py` & `kopf-1.36.2/kopf/cli.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf/on.py` & `kopf-1.36.2/kopf/on.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/kopf.egg-info/PKG-INFO` & `kopf-1.36.2/kopf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kopf
-Version: 1.36.1
+Version: 1.36.2
 Summary: Kubernetes Operator Pythonic Framework (Kopf)
 Home-page: https://github.com/nolar/kopf
 Author: Sergey Vasilyev
 Author-email: nolar@nolar.info
 Maintainer: Sergey Vasilyev
 Maintainer-email: nolar@nolar.info
 License: MIT
```

### Comparing `kopf-1.36.1/kopf.egg-info/SOURCES.txt` & `kopf-1.36.2/kopf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/peering.yaml` & `kopf-1.36.2/peering.yaml`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/requirements.txt` & `kopf-1.36.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/setup.py` & `kopf-1.36.2/setup.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/conftest.py` & `kopf-1.36.2/tests/admission/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/test_admission_manager.py` & `kopf-1.36.2/tests/admission/test_admission_manager.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/test_admission_server.py` & `kopf-1.36.2/tests/admission/test_admission_server.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/test_certificates.py` & `kopf-1.36.2/tests/admission/test_certificates.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/test_jsonpatch.py` & `kopf-1.36.2/tests/admission/test_jsonpatch.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/test_managed_webhooks.py` & `kopf-1.36.2/tests/admission/test_managed_webhooks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/test_serving_ephemeral_memos.py` & `kopf-1.36.2/tests/admission/test_serving_ephemeral_memos.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/test_serving_handler_selection.py` & `kopf-1.36.2/tests/admission/test_serving_handler_selection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/test_serving_kwargs_passthrough.py` & `kopf-1.36.2/tests/admission/test_serving_kwargs_passthrough.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/test_serving_responses.py` & `kopf-1.36.2/tests/admission/test_serving_responses.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/test_webhook_detection.py` & `kopf-1.36.2/tests/admission/test_webhook_detection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/test_webhook_ngrok.py` & `kopf-1.36.2/tests/admission/test_webhook_ngrok.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/admission/test_webhook_server.py` & `kopf-1.36.2/tests/admission/test_webhook_server.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/apis/test_api_requests.py` & `kopf-1.36.2/tests/apis/test_api_requests.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/apis/test_error_retries.py` & `kopf-1.36.2/tests/apis/test_error_retries.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/apis/test_iterjsonlines.py` & `kopf-1.36.2/tests/apis/test_iterjsonlines.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/authentication/test_authentication.py` & `kopf-1.36.2/tests/authentication/test_authentication.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/authentication/test_connectioninfo.py` & `kopf-1.36.2/tests/authentication/test_connectioninfo.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/authentication/test_credentials.py` & `kopf-1.36.2/tests/authentication/test_credentials.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/authentication/test_login_kubeconfig.py` & `kopf-1.36.2/tests/authentication/test_login_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/authentication/test_login_serviceaccount.py` & `kopf-1.36.2/tests/authentication/test_login_serviceaccount.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/authentication/test_reauthentication.py` & `kopf-1.36.2/tests/authentication/test_reauthentication.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/authentication/test_tempfiles.py` & `kopf-1.36.2/tests/authentication/test_tempfiles.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/authentication/test_vault.py` & `kopf-1.36.2/tests/authentication/test_vault.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/basic-structs/test_causes.py` & `kopf-1.36.2/tests/basic-structs/test_causes.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/basic-structs/test_handlers.py` & `kopf-1.36.2/tests/basic-structs/test_handlers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/basic-structs/test_memories.py` & `kopf-1.36.2/tests/basic-structs/test_memories.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/basic-structs/test_memos.py` & `kopf-1.36.2/tests/basic-structs/test_memos.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/basic-structs/test_resource.py` & `kopf-1.36.2/tests/basic-structs/test_resource.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/causation/test_detection.py` & `kopf-1.36.2/tests/causation/test_detection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/causation/test_kwargs.py` & `kopf-1.36.2/tests/causation/test_kwargs.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/cli/conftest.py` & `kopf-1.36.2/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/cli/test_help.py` & `kopf-1.36.2/tests/cli/test_help.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/cli/test_logging.py` & `kopf-1.36.2/tests/cli/test_logging.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/cli/test_options.py` & `kopf-1.36.2/tests/cli/test_options.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/cli/test_preloading.py` & `kopf-1.36.2/tests/cli/test_preloading.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/conftest.py` & `kopf-1.36.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/dicts/test_cherrypicking.py` & `kopf-1.36.2/tests/dicts/test_cherrypicking.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/dicts/test_dictviews.py` & `kopf-1.36.2/tests/dicts/test_dictviews.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/dicts/test_ensuring.py` & `kopf-1.36.2/tests/dicts/test_ensuring.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/dicts/test_parsing.py` & `kopf-1.36.2/tests/dicts/test_parsing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/dicts/test_removing.py` & `kopf-1.36.2/tests/dicts/test_removing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/dicts/test_resolving.py` & `kopf-1.36.2/tests/dicts/test_resolving.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/dicts/test_walking.py` & `kopf-1.36.2/tests/dicts/test_walking.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/diffs/test_calculation.py` & `kopf-1.36.2/tests/diffs/test_calculation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/diffs/test_protocols.py` & `kopf-1.36.2/tests/diffs/test_protocols.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/diffs/test_reduction.py` & `kopf-1.36.2/tests/diffs/test_reduction.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/e2e/conftest.py` & `kopf-1.36.2/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/e2e/test_examples.py` & `kopf-1.36.2/tests/e2e/test_examples.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/conftest.py` & `kopf-1.36.2/tests/handling/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/daemons/conftest.py` & `kopf-1.36.2/tests/handling/daemons/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/daemons/test_daemon_errors.py` & `kopf-1.36.2/tests/handling/daemons/test_daemon_errors.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/daemons/test_daemon_filtration.py` & `kopf-1.36.2/tests/handling/daemons/test_daemon_filtration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/daemons/test_daemon_rematching.py` & `kopf-1.36.2/tests/handling/daemons/test_daemon_rematching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/daemons/test_daemon_spawning.py` & `kopf-1.36.2/tests/handling/daemons/test_daemon_spawning.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/daemons/test_daemon_termination.py` & `kopf-1.36.2/tests/handling/daemons/test_daemon_termination.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/daemons/test_timer_errors.py` & `kopf-1.36.2/tests/handling/daemons/test_timer_errors.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/daemons/test_timer_filtration.py` & `kopf-1.36.2/tests/handling/daemons/test_timer_filtration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/daemons/test_timer_intervals.py` & `kopf-1.36.2/tests/handling/daemons/test_timer_intervals.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/daemons/test_timer_triggering.py` & `kopf-1.36.2/tests/handling/daemons/test_timer_triggering.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/indexing/conftest.py` & `kopf-1.36.2/tests/handling/indexing/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/indexing/test_blocking_until_indexed.py` & `kopf-1.36.2/tests/handling/indexing/test_blocking_until_indexed.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/indexing/test_index_exclusion.py` & `kopf-1.36.2/tests/handling/indexing/test_index_exclusion.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/indexing/test_index_population.py` & `kopf-1.36.2/tests/handling/indexing/test_index_population.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/subhandling/test_subhandling.py` & `kopf-1.36.2/tests/handling/subhandling/test_subhandling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/test_activity_triggering.py` & `kopf-1.36.2/tests/handling/test_activity_triggering.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/test_cause_handling.py` & `kopf-1.36.2/tests/handling/test_cause_handling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/test_cause_logging.py` & `kopf-1.36.2/tests/handling/test_cause_logging.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/test_delays.py` & `kopf-1.36.2/tests/handling/test_delays.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/test_error_handling.py` & `kopf-1.36.2/tests/handling/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/test_event_handling.py` & `kopf-1.36.2/tests/handling/test_event_handling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/test_multistep.py` & `kopf-1.36.2/tests/handling/test_multistep.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/test_no_handlers.py` & `kopf-1.36.2/tests/handling/test_no_handlers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/test_parametrization.py` & `kopf-1.36.2/tests/handling/test_parametrization.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/test_retrying_limits.py` & `kopf-1.36.2/tests/handling/test_retrying_limits.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/handling/test_timing_consistency.py` & `kopf-1.36.2/tests/handling/test_timing_consistency.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/hierarchies/conftest.py` & `kopf-1.36.2/tests/hierarchies/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/hierarchies/test_contextual_owner.py` & `kopf-1.36.2/tests/hierarchies/test_contextual_owner.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/hierarchies/test_labelling.py` & `kopf-1.36.2/tests/hierarchies/test_labelling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/hierarchies/test_name_harmonizing.py` & `kopf-1.36.2/tests/hierarchies/test_name_harmonizing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/hierarchies/test_namespace_adjusting.py` & `kopf-1.36.2/tests/hierarchies/test_namespace_adjusting.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/hierarchies/test_owner_referencing.py` & `kopf-1.36.2/tests/hierarchies/test_owner_referencing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/hierarchies/test_type_validation.py` & `kopf-1.36.2/tests/hierarchies/test_type_validation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/invocations/test_callbacks.py` & `kopf-1.36.2/tests/invocations/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/k8s/test_creating.py` & `kopf-1.36.2/tests/k8s/test_creating.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/k8s/test_errors.py` & `kopf-1.36.2/tests/k8s/test_errors.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/k8s/test_events.py` & `kopf-1.36.2/tests/k8s/test_events.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/k8s/test_list_objs.py` & `kopf-1.36.2/tests/k8s/test_list_objs.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/k8s/test_patching.py` & `kopf-1.36.2/tests/k8s/test_patching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/k8s/test_scanning.py` & `kopf-1.36.2/tests/k8s/test_scanning.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/k8s/test_watching_bookmarks.py` & `kopf-1.36.2/tests/k8s/test_watching_bookmarks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/k8s/test_watching_continuously.py` & `kopf-1.36.2/tests/k8s/test_watching_continuously.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/k8s/test_watching_infinitely.py` & `kopf-1.36.2/tests/k8s/test_watching_infinitely.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/k8s/test_watching_with_freezes.py` & `kopf-1.36.2/tests/k8s/test_watching_with_freezes.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/lifecycles/test_global_defaults.py` & `kopf-1.36.2/tests/lifecycles/test_global_defaults.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/lifecycles/test_handler_selection.py` & `kopf-1.36.2/tests/lifecycles/test_handler_selection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/lifecycles/test_real_invocation.py` & `kopf-1.36.2/tests/lifecycles/test_real_invocation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/logging/conftest.py` & `kopf-1.36.2/tests/logging/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/logging/test_configuration.py` & `kopf-1.36.2/tests/logging/test_configuration.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/logging/test_formatters.py` & `kopf-1.36.2/tests/logging/test_formatters.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/logging/test_loggers.py` & `kopf-1.36.2/tests/logging/test_loggers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/observation/test_processing_of_namespaces.py` & `kopf-1.36.2/tests/observation/test_processing_of_namespaces.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/observation/test_processing_of_resources.py` & `kopf-1.36.2/tests/observation/test_processing_of_resources.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/observation/test_revision_of_namespaces.py` & `kopf-1.36.2/tests/observation/test_revision_of_namespaces.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/observation/test_revision_of_resources.py` & `kopf-1.36.2/tests/observation/test_revision_of_resources.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/orchestration/test_task_adjustments.py` & `kopf-1.36.2/tests/orchestration/test_task_adjustments.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/peering/test_freeze_mode.py` & `kopf-1.36.2/tests/peering/test_freeze_mode.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/peering/test_id_generation.py` & `kopf-1.36.2/tests/peering/test_id_generation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/peering/test_keepalive.py` & `kopf-1.36.2/tests/peering/test_keepalive.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/peering/test_peer_patching.py` & `kopf-1.36.2/tests/peering/test_peer_patching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/peering/test_peers.py` & `kopf-1.36.2/tests/peering/test_peers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/peering/test_resource_guessing.py` & `kopf-1.36.2/tests/peering/test_resource_guessing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/persistence/test_annotations_hashing.py` & `kopf-1.36.2/tests/persistence/test_annotations_hashing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/persistence/test_essences.py` & `kopf-1.36.2/tests/persistence/test_essences.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/persistence/test_outcomes.py` & `kopf-1.36.2/tests/persistence/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/persistence/test_states.py` & `kopf-1.36.2/tests/persistence/test_states.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/persistence/test_storing_of_diffbase.py` & `kopf-1.36.2/tests/persistence/test_storing_of_diffbase.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/persistence/test_storing_of_progress.py` & `kopf-1.36.2/tests/persistence/test_storing_of_progress.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/posting/test_log2k8s.py` & `kopf-1.36.2/tests/posting/test_log2k8s.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/posting/test_poster.py` & `kopf-1.36.2/tests/posting/test_poster.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/posting/test_threadsafety.py` & `kopf-1.36.2/tests/posting/test_threadsafety.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/primitives/test_conditions.py` & `kopf-1.36.2/tests/primitives/test_conditions.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/primitives/test_containers.py` & `kopf-1.36.2/tests/primitives/test_containers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/primitives/test_flags.py` & `kopf-1.36.2/tests/primitives/test_flags.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/primitives/test_toggles.py` & `kopf-1.36.2/tests/primitives/test_toggles.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/primitives/test_togglesets.py` & `kopf-1.36.2/tests/primitives/test_togglesets.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/reactor/conftest.py` & `kopf-1.36.2/tests/reactor/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/reactor/test_patching_inconsistencies.py` & `kopf-1.36.2/tests/reactor/test_patching_inconsistencies.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/reactor/test_queueing.py` & `kopf-1.36.2/tests/reactor/test_queueing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/reactor/test_uids.py` & `kopf-1.36.2/tests/reactor/test_uids.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/references/test_backbone.py` & `kopf-1.36.2/tests/references/test_backbone.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/references/test_namespace_matching.py` & `kopf-1.36.2/tests/references/test_namespace_matching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/references/test_namespace_selection.py` & `kopf-1.36.2/tests/references/test_namespace_selection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/references/test_selector_matching.py` & `kopf-1.36.2/tests/references/test_selector_matching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/references/test_selector_parsing.py` & `kopf-1.36.2/tests/references/test_selector_parsing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/references/test_selector_properties.py` & `kopf-1.36.2/tests/references/test_selector_properties.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/conftest.py` & `kopf-1.36.2/tests/registries/conftest.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_creation.py` & `kopf-1.36.2/tests/registries/test_creation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_decorators.py` & `kopf-1.36.2/tests/registries/test_decorators.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_handler_getting.py` & `kopf-1.36.2/tests/registries/test_handler_getting.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_id_detection.py` & `kopf-1.36.2/tests/registries/test_id_detection.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_matching_for_changing.py` & `kopf-1.36.2/tests/registries/test_matching_for_changing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_matching_for_indexing.py` & `kopf-1.36.2/tests/registries/test_matching_for_indexing.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_matching_for_spawning.py` & `kopf-1.36.2/tests/registries/test_matching_for_spawning.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_matching_for_watching.py` & `kopf-1.36.2/tests/registries/test_matching_for_watching.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_matching_of_callbacks.py` & `kopf-1.36.2/tests/registries/test_matching_of_callbacks.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_matching_of_resources.py` & `kopf-1.36.2/tests/registries/test_matching_of_resources.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_requires_finalizer.py` & `kopf-1.36.2/tests/registries/test_requires_finalizer.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_resumes_mixed_in.py` & `kopf-1.36.2/tests/registries/test_resumes_mixed_in.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/registries/test_subhandlers_ids.py` & `kopf-1.36.2/tests/registries/test_subhandlers_ids.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/settings/test_defaults.py` & `kopf-1.36.2/tests/settings/test_defaults.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/settings/test_executor.py` & `kopf-1.36.2/tests/settings/test_executor.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/test_async.py` & `kopf-1.36.2/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/test_filtering_helpers.py` & `kopf-1.36.2/tests/test_filtering_helpers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/test_finalizers.py` & `kopf-1.36.2/tests/test_finalizers.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/test_liveness.py` & `kopf-1.36.2/tests/test_liveness.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/test_thirdparty.py` & `kopf-1.36.2/tests/test_thirdparty.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/test_versions.py` & `kopf-1.36.2/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/testing/test_runner.py` & `kopf-1.36.2/tests/testing/test_runner.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/timing/test_sleeping.py` & `kopf-1.36.2/tests/timing/test_sleeping.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/timing/test_throttling.py` & `kopf-1.36.2/tests/timing/test_throttling.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/utilities/aiotasks/test_coro_cancellation.py` & `kopf-1.36.2/tests/utilities/aiotasks/test_coro_cancellation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/utilities/aiotasks/test_scheduler.py` & `kopf-1.36.2/tests/utilities/aiotasks/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/utilities/aiotasks/test_task_creation.py` & `kopf-1.36.2/tests/utilities/aiotasks/test_task_creation.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/utilities/aiotasks/test_task_guarding.py` & `kopf-1.36.2/tests/utilities/aiotasks/test_task_guarding.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tests/utilities/aiotasks/test_task_stopping.py` & `kopf-1.36.2/tests/utilities/aiotasks/test_task_stopping.py`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tools/install-kind.sh` & `kopf-1.36.2/tools/install-kind.sh`

 * *Files identical despite different names*

### Comparing `kopf-1.36.1/tools/install-minikube.sh` & `kopf-1.36.2/tools/install-minikube.sh`

 * *Files identical despite different names*

