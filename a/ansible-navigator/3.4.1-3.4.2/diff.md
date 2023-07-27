# Comparing `tmp/ansible-navigator-3.4.1.tar.gz` & `tmp/ansible-navigator-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-navigator-3.4.1.tar", last modified: Mon Jul 24 13:07:42 2023, max compression
+gzip compressed data, was "ansible-navigator-3.4.2.tar", last modified: Thu Jul 27 17:06:15 2023, max compression
```

## Comparing `ansible-navigator-3.4.1.tar` & `ansible-navigator-3.4.2.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.290742 ansible-navigator-3.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.202743 ansible-navigator-3.4.1/.config/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.config/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.darglint
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.202743 ansible-navigator-3.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.206743 ansible-navigator-3.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/ISSUE_TEMPLATE/documentation_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/chronographer.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.206743 ansible-navigator-3.4.1/.github/images/
--rw-r--r--   0 runner    (1001) docker     (123)    55005 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/images/test_tree_view.png
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.206743 ansible-navigator-3.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.prettierrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.206743 ansible-navigator-3.4.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-24 13:07:42.290742 ansible-navigator-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.210743 ansible-navigator-3.4.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.210743 ansible-navigator-3.4.1/docs/.generated/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/.generated/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.210743 ansible-navigator-3.4.1/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/_ext/regenerate_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.214743 ansible-navigator-3.4.1/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/contributing/code-of-conduct.md
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/contributing/guidelines.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.214743 ansible-navigator-3.4.1/docs/contributing/images/
--rw-r--r--   0 runner    (1001) docker     (123)    55005 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/contributing/images/test_tree_view.png
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/contributing/security.md
--rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/settings.md
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/docs/subcommands.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.222743 ansible-navigator-3.4.1/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.asottile_tm_tokenize.all.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.dark_vs.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.source.json.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.source.shell.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.source.yaml.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.text.html.basic.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.text.html.derivative.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.text.html.markdown.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/licenses/LICENSE.text.log.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:07:42.290742 ansible-navigator-3.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.186743 ansible-navigator-3.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.230743 ansible-navigator-3.4.1/src/ansible_navigator/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 13:07:41.000000 ansible-navigator-3.4.1/src/ansible_navigator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/_version_doc_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/action_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/action_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/action_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.250743 ansible-navigator-3.4.1/src/ansible_navigator/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/back.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    27759 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    14363 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/help_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    21313 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/open_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/quit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/rerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    36365 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/sample_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/sample_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/sample_working.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/serialize_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/serialize_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/actions/write_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/app_public.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.250743 ansible-navigator-3.4.1/src/ansible_navigator/command_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/command_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/command_runner/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.258742 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19986 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/defs_presentable.py
--rw-r--r--   0 runner    (1001) docker     (123)    31838 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    49073 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/content_defs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.262743 ansible-navigator-3.4.1/src/ansible_navigator/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/ansible-navigator.json
--rw-r--r--   0 runner    (1001) docker     (123)    23668 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/catalog_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.262743 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/html.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/log.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/source.json.json
--rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/source.shell.json
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/source.yaml.json
--rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.html.basic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.html.derivative.json
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.html.markdown.json
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.log.json
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/help.md
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/image_introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/images_dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/settings-sample.template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/settings-schema.partial.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.262743 ansible-navigator-3.4.1/src/ansible_navigator/data/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/themes/dark_vs.json
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/themes/terminal_colors.json
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/data/welcome.md
--rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.266743 ansible-navigator-3.4.1/src/ansible_navigator/image_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/image_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/image_manager/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/image_manager/introspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/image_manager/puller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.266743 ansible-navigator-3.4.1/src/ansible_navigator/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/ansible_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/ansible_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/ansible_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/command_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/runner/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.278742 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/fchainmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/grammars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/reg.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.286743 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/curses_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/curses_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_curses_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_working.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_working.py
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/menu_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/sentinels.py
--rw-r--r--   0 runner    (1001) docker     (123)    33458 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/ui_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/ui_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.290742 ansible-navigator-3.4.1/src/ansible_navigator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/dict_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/dot_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/packaged_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/print.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.290742 ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/settings_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/src/ansible_navigator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:07:42.234742 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-24 13:07:41.000000 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-24 13:07:42.000000 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:07:41.000000 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 13:07:41.000000 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-24 13:07:41.000000 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 13:07:41.000000 ansible-navigator-3.4.1/src/ansible_navigator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-24 13:07:13.000000 ansible-navigator-3.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:15.006797 ansible-navigator-3.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.970796 ansible-navigator-3.4.2/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.970796 ansible-navigator-3.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.974796 ansible-navigator-3.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/ISSUE_TEMPLATE/documentation_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/chronographer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.974796 ansible-navigator-3.4.2/.github/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    55005 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/images/test_tree_view.png
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.974796 ansible-navigator-3.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.prettierrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.974796 ansible-navigator-3.4.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-27 17:06:15.006797 ansible-navigator-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.974796 ansible-navigator-3.4.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.974796 ansible-navigator-3.4.2/docs/.generated/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/docs/.generated/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.974796 ansible-navigator-3.4.2/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/docs/_ext/regenerate_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.974796 ansible-navigator-3.4.2/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/docs/contributing/code-of-conduct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/docs/contributing/guidelines.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.974796 ansible-navigator-3.4.2/docs/contributing/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    55005 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/docs/contributing/images/test_tree_view.png
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/docs/contributing/security.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13957 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/docs/settings.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/docs/subcommands.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.974796 ansible-navigator-3.4.2/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/licenses/LICENSE.asottile_tm_tokenize.all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/licenses/LICENSE.dark_vs.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/licenses/LICENSE.source.json.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/licenses/LICENSE.source.shell.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/licenses/LICENSE.source.yaml.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/licenses/LICENSE.text.html.basic.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/licenses/LICENSE.text.html.derivative.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/licenses/LICENSE.text.html.markdown.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/licenses/LICENSE.text.log.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:06:15.006797 ansible-navigator-3.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.966796 ansible-navigator-3.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.978797 ansible-navigator-3.4.2/src/ansible_navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 17:06:14.000000 ansible-navigator-3.4.2/src/ansible_navigator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/_version_doc_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/action_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/action_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/action_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.986796 ansible-navigator-3.4.2/src/ansible_navigator/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/back.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27768 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14363 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/help_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21537 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21313 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/quit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36365 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/sample_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/sample_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/sample_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/serialize_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/serialize_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/actions/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/app_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.986796 ansible-navigator-3.4.2/src/ansible_navigator/command_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/command_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/command_runner/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.986796 ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19986 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/defs_presentable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31838 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49073 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/content_defs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.994797 ansible-navigator-3.4.2/src/ansible_navigator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/ansible-navigator.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23668 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/catalog_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.998797 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/html.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/log.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/source.json.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/source.shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/source.yaml.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/text.html.basic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/text.html.derivative.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/text.html.markdown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/text.log.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/help.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/image_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/images_dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/settings-sample.template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/settings-schema.partial.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.998797 ansible-navigator-3.4.2/src/ansible_navigator/data/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/themes/dark_vs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/themes/terminal_colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/data/welcome.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.998797 ansible-navigator-3.4.2/src/ansible_navigator/image_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/image_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/image_manager/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/image_manager/introspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/image_manager/puller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.998797 ansible-navigator-3.4.2/src/ansible_navigator/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/runner/ansible_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/runner/ansible_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/runner/ansible_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/runner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/runner/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/runner/command_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/runner/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.998797 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/fchainmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/grammars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:15.002797 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/curses_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/curses_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_curses_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_handler_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_handler_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_handler_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_handler_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_handler_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/menu_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/sentinels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33458 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/ui_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/ui_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:15.006797 ansible-navigator-3.4.2/src/ansible_navigator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/dict_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/dot_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/packaged_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:15.006797 ansible-navigator-3.4.2/src/ansible_navigator/utils/version_migration/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/version_migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/version_migration/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/version_migration/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/version_migration/settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/src/ansible_navigator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:06:14.978797 ansible-navigator-3.4.2/src/ansible_navigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-27 17:06:14.000000 ansible-navigator-3.4.2/src/ansible_navigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-27 17:06:14.000000 ansible-navigator-3.4.2/src/ansible_navigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:06:14.000000 ansible-navigator-3.4.2/src/ansible_navigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 17:06:14.000000 ansible-navigator-3.4.2/src/ansible_navigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-27 17:06:14.000000 ansible-navigator-3.4.2/src/ansible_navigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 17:06:14.000000 ansible-navigator-3.4.2/src/ansible_navigator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-27 17:05:53.000000 ansible-navigator-3.4.2/tox.ini
```

### Comparing `ansible-navigator-3.4.1/.config/dictionary.txt` & `ansible-navigator-3.4.2/.config/dictionary.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.flake8` & `ansible-navigator-3.4.2/.flake8`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.git_archival.txt` & `ansible-navigator-3.4.2/.git_archival.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.github/CONTRIBUTING.md` & `ansible-navigator-3.4.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `ansible-navigator-3.4.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.github/SECURITY.md` & `ansible-navigator-3.4.2/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.github/dependabot.yml` & `ansible-navigator-3.4.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.github/images/test_tree_view.png` & `ansible-navigator-3.4.2/.github/images/test_tree_view.png`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.github/workflows/release.yml` & `ansible-navigator-3.4.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.github/workflows/tox.yml` & `ansible-navigator-3.4.2/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.gitignore` & `ansible-navigator-3.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.pre-commit-config.yaml` & `ansible-navigator-3.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.prettierignore` & `ansible-navigator-3.4.2/.prettierignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.vscode/launch.json` & `ansible-navigator-3.4.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/.vscode/settings.json` & `ansible-navigator-3.4.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/LICENSE` & `ansible-navigator-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/PKG-INFO` & `ansible-navigator-3.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.4.1
+Version: 3.4.2
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
```

### Comparing `ansible-navigator-3.4.1/README.md` & `ansible-navigator-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/cspell.config.yaml` & `ansible-navigator-3.4.2/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/docs/_ext/regenerate_docs.py` & `ansible-navigator-3.4.2/docs/_ext/regenerate_docs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/docs/contributing/guidelines.md` & `ansible-navigator-3.4.2/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/docs/contributing/images/test_tree_view.png` & `ansible-navigator-3.4.2/docs/contributing/images/test_tree_view.png`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/docs/contributing/security.md` & `ansible-navigator-3.4.2/docs/contributing/security.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/docs/faq.md` & `ansible-navigator-3.4.2/docs/faq.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/docs/index.md` & `ansible-navigator-3.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/docs/installation.md` & `ansible-navigator-3.4.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/docs/settings.md` & `ansible-navigator-3.4.2/docs/settings.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/docs/subcommands.md` & `ansible-navigator-3.4.2/docs/subcommands.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/licenses/LICENSE.asottile_tm_tokenize.all.txt` & `ansible-navigator-3.4.2/licenses/LICENSE.asottile_tm_tokenize.all.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/licenses/LICENSE.dark_vs.json.txt` & `ansible-navigator-3.4.2/licenses/LICENSE.dark_vs.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/licenses/LICENSE.source.json.json.txt` & `ansible-navigator-3.4.2/licenses/LICENSE.source.json.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/licenses/LICENSE.source.shell.json.txt` & `ansible-navigator-3.4.2/licenses/LICENSE.source.shell.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/licenses/LICENSE.source.yaml.json.txt` & `ansible-navigator-3.4.2/licenses/LICENSE.source.yaml.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/licenses/LICENSE.text.html.markdown.json.txt` & `ansible-navigator-3.4.2/licenses/LICENSE.text.html.markdown.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/licenses/LICENSE.text.log.json.txt` & `ansible-navigator-3.4.2/licenses/LICENSE.text.log.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/mkdocs.yml` & `ansible-navigator-3.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/mypy.ini` & `ansible-navigator-3.4.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/pyproject.toml` & `ansible-navigator-3.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/requirements.txt` & `ansible-navigator-3.4.2/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # To update, run:
 #
 #    pip-compile --extra=docs --extra=test --no-annotate --output-file=requirements.txt --resolver=backtracking --strip-extras --unsafe-package=resolvelib --unsafe-package=ruamel-yaml-clib pyproject.toml
 #
 ansible-builder==3.0.0
 ansible-core==2.15.1
+ansible-lint==6.17.2
 ansible-runner==2.3.3
 attrs==23.1.0
 beautifulsoup4==4.12.2
 bindep==2.11.0
 cairocffi==1.6.0
 cairosvg==2.7.0
 certifi==2023.5.7
```

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/_version_doc_cache.py` & `ansible-navigator-3.4.2/src/ansible_navigator/_version_doc_cache.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/action_base.py` & `ansible-navigator-3.4.2/src/ansible_navigator/action_base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/action_defs.py` & `ansible-navigator-3.4.2/src/ansible_navigator/action_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/action_runner.py` & `ansible-navigator-3.4.2/src/ansible_navigator/action_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/__init__.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/_actions.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/_actions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/back.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/back.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/builder.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/builder.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/collections.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
             self._collection_cache_path,
         ]
 
         kwargs["cmdline"] = pass_through_arg
 
         if self._args.execution_environment:
             self._logger.debug("running collections command with execution environment enabled")
-            python_exec_path = "python3"
+            python_exec_path = "/usr/bin/python3"
             utils_lib = os.path.join(
                 os.path.dirname(__file__),
                 "..",
                 "utils",
             )
 
             container_volume_mounts = [
```

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/config.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/doc.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/exec.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/exec.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/filter.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/filter.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/help_doc.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/help_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/images.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/images.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,15 +547,15 @@
         """Run runner to collect image details.
 
         :param image_name: The full image name
         :returns: Output, errors and the return code
         """
         cache_path = self._args.internals.cache_path
         container_volume_mounts = [f"{cache_path}:{cache_path}"]
-        python_exec_path = "python3"
+        python_exec_path = "/usr/bin/python3"
 
         kwargs = {
             "cmdline": [f"{cache_path}/image_introspect.py"],
             "container_engine": self._args.container_engine,
             "container_volume_mounts": container_volume_mounts,
             "execution_environment_image": image_name,
             "execution_environment": True,
```

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/inventory.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/lint.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/lint.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/log.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/log.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/open_file.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/open_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/quit.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/quit.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/refresh.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/refresh.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/rerun.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/rerun.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/run.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/run.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/sample_form.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/sample_form.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/sample_notification.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/sample_notification.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/sample_working.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/sample_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/save.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/save.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/select.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/select.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/serialize_json.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/serialize_json.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/serialize_yaml.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/serialize_yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/settings.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/settings.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/stdout.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/stdout.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/template.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/template.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/welcome.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/welcome.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/actions/write_file.py` & `ansible-navigator-3.4.2/src/ansible_navigator/actions/write_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/app_public.py` & `ansible-navigator-3.4.2/src/ansible_navigator/app_public.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/cli.py` & `ansible-navigator-3.4.2/src/ansible_navigator/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/command_runner/command_runner.py` & `ansible-navigator-3.4.2/src/ansible_navigator/command_runner/command_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/__init__.py` & `ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/configurator.py` & `ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/configurator.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/definitions.py` & `ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/defs_presentable.py` & `ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/defs_presentable.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/navigator_configuration.py` & `ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/navigator_configuration.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py` & `ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/parser.py` & `ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/transform.py` & `ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/transform.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/configuration_subsystem/utils.py` & `ansible-navigator-3.4.2/src/ansible_navigator/configuration_subsystem/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/constants.py` & `ansible-navigator-3.4.2/src/ansible_navigator/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/content_defs.py` & `ansible-navigator-3.4.2/src/ansible_navigator/content_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/ansible-navigator.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/ansible-navigator.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/catalog_collections.py` & `ansible-navigator-3.4.2/src/ansible_navigator/data/catalog_collections.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/JSON.tmLanguage.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/JSON.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/html.tmLanguage.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/html.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/log.tmLanguage.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/log.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/markdown.tmLanguage.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/markdown.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/source.json.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/source.json.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/source.shell.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/source.shell.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/source.yaml.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/source.yaml.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.html.basic.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/text.html.basic.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.html.derivative.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/text.html.derivative.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.html.markdown.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/text.html.markdown.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/text.log.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/text.log.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/grammar/yaml.tmLanguage.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/grammar/yaml.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/help.md` & `ansible-navigator-3.4.2/src/ansible_navigator/data/help.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/image_introspect.py` & `ansible-navigator-3.4.2/src/ansible_navigator/data/image_introspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,20 +276,26 @@
 
     @property
     def commands(self) -> list[Command]:
         """Define the pip command to list installed pip packages.
 
         :returns: The defined command
         """
-        pre = Command(id_="pip_freeze", command="python3 -m pip freeze", parse=self.parse_freeze)
+        pre = Command(
+            id_="pip_freeze", command="/usr/bin/python3 -m pip freeze", parse=self.parse_freeze
+        )
         run_command(pre)
         pre.parse(pre)
-        pkgs = " ".join(pkg for pkg in pre.details[0])
+        pkgs = " ".join(pkg for pkg in pre.details[0]) if pre.details else ""
         return [
-            Command(id_="python_packages", command=f"python3 -m pip show {pkgs}", parse=self.parse),
+            Command(
+                id_="python_packages",
+                command=f"/usr/bin/python3 -m pip show {pkgs}",
+                parse=self.parse,
+            ),
         ]
 
     def parse(self, command):
         """Parse the output of the pip command.
 
         :param command: The result of running the command
         """
```

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/settings-sample.template.yml` & `ansible-navigator-3.4.2/src/ansible_navigator/data/settings-sample.template.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/settings-schema.partial.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/settings-schema.partial.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/themes/dark_vs.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/themes/dark_vs.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/themes/terminal_colors.json` & `ansible-navigator-3.4.2/src/ansible_navigator/data/themes/terminal_colors.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/data/welcome.md` & `ansible-navigator-3.4.2/src/ansible_navigator/data/welcome.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/diagnostics.py` & `ansible-navigator-3.4.2/src/ansible_navigator/diagnostics.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/image_manager/inspector.py` & `ansible-navigator-3.4.2/src/ansible_navigator/image_manager/inspector.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/image_manager/introspector.py` & `ansible-navigator-3.4.2/src/ansible_navigator/image_manager/introspector.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/image_manager/puller.py` & `ansible-navigator-3.4.2/src/ansible_navigator/image_manager/puller.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/initialization.py` & `ansible-navigator-3.4.2/src/ansible_navigator/initialization.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/logger.py` & `ansible-navigator-3.4.2/src/ansible_navigator/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/runner/ansible_config.py` & `ansible-navigator-3.4.2/src/ansible_navigator/runner/ansible_config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/runner/ansible_doc.py` & `ansible-navigator-3.4.2/src/ansible_navigator/runner/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/runner/ansible_inventory.py` & `ansible-navigator-3.4.2/src/ansible_navigator/runner/ansible_inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/runner/base.py` & `ansible-navigator-3.4.2/src/ansible_navigator/runner/base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/runner/command.py` & `ansible-navigator-3.4.2/src/ansible_navigator/runner/command.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/runner/command_async.py` & `ansible-navigator-3.4.2/src/ansible_navigator/runner/command_async.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/runner/command_base.py` & `ansible-navigator-3.4.2/src/ansible_navigator/runner/command_base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/steps.py` & `ansible-navigator-3.4.2/src/ansible_navigator/steps.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/LICENSE` & `ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/compiler.py` & `ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/compiler.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/fchainmap.py` & `ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/fchainmap.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/grammars.py` & `ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/grammars.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/reg.py` & `ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/reg.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/rules.py` & `ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/rules.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/state.py` & `ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/state.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/tm_tokenize/tokenize.py` & `ansible-navigator-3.4.2/src/ansible_navigator/tm_tokenize/tokenize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/__init__.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/colorize.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/colorize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/curses_defs.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/curses_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/curses_window.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/curses_window.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_button.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_checks.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_curses_information.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_curses_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_information.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_option.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_option.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_radio.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_radio.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_text.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/field_working.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/field_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_button.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_handler_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_information.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_handler_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_options.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_handler_options.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_text.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_handler_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_handler_working.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_handler_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/form_utils.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/form_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/menu_builder.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/menu_builder.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/sentinels.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/sentinels.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/ui.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/ui.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/ui_config.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/ui_config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/ui_constants.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/ui_constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/utils.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/ui_framework/validators.py` & `ansible-navigator-3.4.2/src/ansible_navigator/ui_framework/validators.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/ansi.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/definitions.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/dict_merge.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/dict_merge.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/dot_paths.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/dot_paths.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/functions.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/functions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/json_schema.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/key_value_store.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/key_value_store.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/packaged_data.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/packaged_data.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/print.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/print.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/serialize.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/definitions.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/version_migration/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/migrate.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/version_migration/migrate.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/settings_file.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/version_migration/settings_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py` & `ansible-navigator-3.4.2/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator.egg-info/PKG-INFO` & `ansible-navigator-3.4.2/src/ansible_navigator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.4.1
+Version: 3.4.2
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
```

### Comparing `ansible-navigator-3.4.1/src/ansible_navigator.egg-info/SOURCES.txt` & `ansible-navigator-3.4.2/src/ansible_navigator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.4.1/tox.ini` & `ansible-navigator-3.4.2/tox.ini`

 * *Files identical despite different names*

