# Comparing `tmp/freva_deployment-2305.0.3.tar.gz` & `tmp/freva_deployment-2307.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freva_deployment-2305.0.3.tar", last modified: Tue May  9 14:30:12 2023, max compression
+gzip compressed data, was "freva_deployment-2307.0.0.tar", last modified: Thu Jul 27 20:14:46 2023, max compression
```

## Comparing `freva_deployment-2305.0.3.tar` & `freva_deployment-2307.0.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.074506 freva_deployment-2305.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-05-09 14:30:12.070506 freva_deployment-2305.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.062506 freva_deployment-2305.0.3/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.066506 freva_deployment-2305.0.3/assets/config/
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/config/create_tables.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/config/evaluation_system.conf.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/config/inventory.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.066506 freva_deployment-2305.0.3/assets/db_service/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/db_service/password_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/db_service/reset_root_pw.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.066506 freva_deployment-2305.0.3/assets/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/playbooks/core-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/playbooks/db-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/playbooks/server-map-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/playbooks/solr-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/playbooks/vault-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/playbooks/web-server-playbook.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.066506 freva_deployment-2305.0.3/assets/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/scripts/create_cron.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/scripts/create_systemd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/scripts/docker-or-podman
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/scripts/dump_sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.066506 freva_deployment-2305.0.3/assets/servers/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/servers/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.066506 freva_deployment-2305.0.3/assets/servers/freva/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/servers/freva/servers.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/servers/restservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.066506 freva_deployment-2305.0.3/assets/vault/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/vault/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/vault/deploy_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/vault/policy-file.hcl
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/vault/runserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/vault/vault-server-no-tls.hcl
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/vault/vault-server-tls.hcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.070506 freva_deployment-2305.0.3/assets/web/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2305 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/web/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/web/docker_cmd.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/web/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/assets/web/freva_web.conf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 14:30:12.074506 freva_deployment-2305.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.062506 freva_deployment-2305.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.070506 freva_deployment-2305.0.3/src/freva_deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.070506 freva_deployment-2305.0.3/src/freva_deployment/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/cli/_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/cli/_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/cli/_server_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/cli/_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.070506 freva_deployment-2305.0.3/src/freva_deployment/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.070506 freva_deployment-2305.0.3/src/freva_deployment/ui/deployment_tui/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/ui/deployment_tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/ui/deployment_tui/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    33822 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/ui/deployment_tui/deploy_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/ui/deployment_tui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-05-09 14:29:58.000000 freva_deployment-2305.0.3/src/freva_deployment/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:30:12.070506 freva_deployment-2305.0.3/src/freva_deployment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-05-09 14:30:12.000000 freva_deployment-2305.0.3/src/freva_deployment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-09 14:30:12.000000 freva_deployment-2305.0.3/src/freva_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:30:12.000000 freva_deployment-2305.0.3/src/freva_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 14:30:12.000000 freva_deployment-2305.0.3/src/freva_deployment.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-09 14:30:12.000000 freva_deployment-2305.0.3/src/freva_deployment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 14:30:12.000000 freva_deployment-2305.0.3/src/freva_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.876887 freva_deployment-2307.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-07-27 20:14:46.876887 freva_deployment-2307.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.860888 freva_deployment-2307.0.0/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.864888 freva_deployment-2307.0.0/assets/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/config/create_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/config/evaluation_system.conf.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/config/inventory.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.864888 freva_deployment-2307.0.0/assets/db_service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/db_service/password_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/db_service/reset_root_pw.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.864888 freva_deployment-2307.0.0/assets/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/playbooks/core-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/playbooks/db-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/playbooks/server-map-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/playbooks/solr-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/playbooks/vault-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/playbooks/web-server-playbook.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.868888 freva_deployment-2307.0.0/assets/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/scripts/create_cron.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/scripts/create_systemd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/scripts/docker-or-podman
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/scripts/dump_sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.868888 freva_deployment-2307.0.0/assets/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/servers/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.868888 freva_deployment-2307.0.0/assets/servers/freva/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/servers/freva/servers.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/servers/restservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.868888 freva_deployment-2307.0.0/assets/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/vault/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/vault/deploy_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/vault/policy-file.hcl
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/vault/runserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/vault/vault-server-no-tls.hcl
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/vault/vault-server-tls.hcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.872887 freva_deployment-2307.0.0/assets/web/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2305 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/web/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/web/docker_cmd.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/web/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/assets/web/freva_web.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:14:46.876887 freva_deployment-2307.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.860888 freva_deployment-2307.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.872887 freva_deployment-2307.0.0/src/freva_deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.876887 freva_deployment-2307.0.0/src/freva_deployment/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/cli/_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/cli/_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/cli/_server_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/cli/_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.876887 freva_deployment-2307.0.0/src/freva_deployment/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.876887 freva_deployment-2307.0.0/src/freva_deployment/ui/deployment_tui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/ui/deployment_tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/ui/deployment_tui/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33822 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/ui/deployment_tui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-07-27 20:14:37.000000 freva_deployment-2307.0.0/src/freva_deployment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:14:46.872887 freva_deployment-2307.0.0/src/freva_deployment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-07-27 20:14:46.000000 freva_deployment-2307.0.0/src/freva_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-27 20:14:46.000000 freva_deployment-2307.0.0/src/freva_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:14:46.000000 freva_deployment-2307.0.0/src/freva_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-27 20:14:46.000000 freva_deployment-2307.0.0/src/freva_deployment.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 20:14:46.000000 freva_deployment-2307.0.0/src/freva_deployment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 20:14:46.000000 freva_deployment-2307.0.0/src/freva_deployment.egg-info/top_level.txt
```

### Comparing `freva_deployment-2305.0.3/PKG-INFO` & `freva_deployment-2307.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva_deployment
-Version: 2305.0.3
+Version: 2307.0.0
 Summary: Deploy freva and its services on different machines.
 Home-page: https://github.com/FREVA-CLINT/freva.git
 Author: Martin Bergemann
 Author-email: martin.bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: GPLv3
 Project-URL: Documentation, https://freva-deployment.readthedocs.io/en/latest/
```

### Comparing `freva_deployment-2305.0.3/README.md` & `freva_deployment-2307.0.0/README.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/config/create_tables.sql` & `freva_deployment-2307.0.0/assets/config/create_tables.sql`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/config/evaluation_system.conf.tmpl` & `freva_deployment-2307.0.0/assets/config/evaluation_system.conf.tmpl`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/config/inventory.toml` & `freva_deployment-2307.0.0/assets/config/inventory.toml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/db_service/password_rotate.py` & `freva_deployment-2307.0.0/assets/db_service/password_rotate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/playbooks/core-server-playbook.yml` & `freva_deployment-2307.0.0/assets/playbooks/core-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/playbooks/db-server-playbook.yml` & `freva_deployment-2307.0.0/assets/playbooks/db-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/playbooks/server-map-playbook.yml` & `freva_deployment-2307.0.0/assets/playbooks/server-map-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/playbooks/solr-server-playbook.yml` & `freva_deployment-2307.0.0/assets/playbooks/solr-server-playbook.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     - docker_cmd: >
         -e CORE=files
         -e NUM_BACKUPS=7
         -e SOLR_HEAP={{solr_mem}}
         -v /opt/freva/{{project_name}}/solr_service:/var/solr/data:z
         -v /root/freva-service-config/solr/managed-schema.xml:/opt/solr/managed-schema.xml:z
         -v /root/freva-service-config/solr/create_cores.sh:/docker-entrypoint-initdb.d/create_cores.sh:z
+        -v /root/freva-service-config/solr/synonyms.txt:/opt/solr/synonyms.txt:z
         -v /root/freva-service-config/solr/daily_backup.sh:/usr/local/bin/daily_backup:z
         --name {{ solr_name }}
         -p {{ solr_port }}:8983 -t
         -t solr:latest
   tasks:
     - name: Copying docker/podman wrapper script
       copy:
```

### Comparing `freva_deployment-2305.0.3/assets/playbooks/vault-server-playbook.yml` & `freva_deployment-2307.0.0/assets/playbooks/vault-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/playbooks/web-server-playbook.yml` & `freva_deployment-2307.0.0/assets/playbooks/web-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/scripts/create_systemd.py` & `freva_deployment-2307.0.0/assets/scripts/create_systemd.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/scripts/docker-or-podman` & `freva_deployment-2307.0.0/assets/scripts/docker-or-podman`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/servers/Dockerfile` & `freva_deployment-2307.0.0/assets/servers/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/servers/restservice.py` & `freva_deployment-2307.0.0/assets/servers/restservice.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/vault/Dockerfile` & `freva_deployment-2307.0.0/assets/vault/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/vault/deploy_vault.py` & `freva_deployment-2307.0.0/assets/vault/deploy_vault.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/vault/runserver.py` & `freva_deployment-2307.0.0/assets/vault/runserver.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/vault/vault-server-tls.hcl` & `freva_deployment-2307.0.0/assets/vault/vault-server-tls.hcl`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/web/Dockerfile` & `freva_deployment-2307.0.0/assets/web/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/assets/web/freva_web.conf` & `freva_deployment-2307.0.0/assets/web/freva_web.conf`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/setup.py` & `freva_deployment-2307.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/src/freva_deployment/cli/_deploy.py` & `freva_deployment-2307.0.0/src/freva_deployment/cli/_deploy.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/src/freva_deployment/cli/_migrate.py` & `freva_deployment-2307.0.0/src/freva_deployment/cli/_migrate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/src/freva_deployment/cli/_server_map.py` & `freva_deployment-2307.0.0/src/freva_deployment/cli/_server_map.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/src/freva_deployment/cli/_service.py` & `freva_deployment-2307.0.0/src/freva_deployment/cli/_service.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/src/freva_deployment/deploy.py` & `freva_deployment-2307.0.0/src/freva_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/src/freva_deployment/ui/deployment_tui/__init__.py` & `freva_deployment-2307.0.0/src/freva_deployment/ui/deployment_tui/__init__.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/src/freva_deployment/ui/deployment_tui/base.py` & `freva_deployment-2307.0.0/src/freva_deployment/ui/deployment_tui/base.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/src/freva_deployment/ui/deployment_tui/deploy_forms.py` & `freva_deployment-2307.0.0/src/freva_deployment/ui/deployment_tui/deploy_forms.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/src/freva_deployment/ui/deployment_tui/main_window.py` & `freva_deployment-2307.0.0/src/freva_deployment/ui/deployment_tui/main_window.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/src/freva_deployment/utils.py` & `freva_deployment-2307.0.0/src/freva_deployment/utils.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2305.0.3/src/freva_deployment.egg-info/PKG-INFO` & `freva_deployment-2307.0.0/src/freva_deployment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva-deployment
-Version: 2305.0.3
+Version: 2307.0.0
 Summary: Deploy freva and its services on different machines.
 Home-page: https://github.com/FREVA-CLINT/freva.git
 Author: Martin Bergemann
 Author-email: martin.bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: GPLv3
 Project-URL: Documentation, https://freva-deployment.readthedocs.io/en/latest/
```

### Comparing `freva_deployment-2305.0.3/src/freva_deployment.egg-info/SOURCES.txt` & `freva_deployment-2307.0.0/src/freva_deployment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

