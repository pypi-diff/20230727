# Comparing `tmp/django-sso-app-0.9.4.tar.gz` & `tmp/django-sso-app-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sso-app-0.9.4.tar", last modified: Mon Feb 22 16:52:33 2021, max compression
+gzip compressed data, was "django-sso-app-0.9.6.tar", last modified: Tue Mar  9 15:17:01 2021, max compression
```

## Comparing `django-sso-app-0.9.4.tar` & `django-sso-app-0.9.6.tar`

### file list

```diff
@@ -1,521 +1,521 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.459590 django-sso-app-0.9.4/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.418590 django-sso-app-0.9.4/.certs/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-09-15 12:15:30.000000 django-sso-app-0.9.4/.certs/.gitkeep
--rw-rw-r--   0 user      (1000) user      (1000)      104 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/.coveragerc
--rw-rw-r--   0 user      (1000) user      (1000)      138 2021-01-11 13:05:40.000000 django-sso-app-0.9.4/.dockerignore
--rw-rw-r--   0 user      (1000) user      (1000)      631 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/.editorconfig
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.408590 django-sso-app-0.9.4/.envs/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.418590 django-sso-app-0.9.4/.envs/.local/
--rw-rw-r--   0 user      (1000) user      (1000)      594 2021-01-25 18:54:32.000000 django-sso-app-0.9.4/.envs/.local/.django
--rw-rw-r--   0 user      (1000) user      (1000)      225 2020-09-15 12:09:20.000000 django-sso-app-0.9.4/.envs/.local/.postgres
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.418590 django-sso-app-0.9.4/.envs/.production/
--rw-r--r--   0 user      (1000) user      (1000)     1509 2021-01-25 18:59:11.000000 django-sso-app-0.9.4/.envs/.production/.django
--rw-r--r--   0 user      (1000) user      (1000)      225 2021-01-25 18:59:11.000000 django-sso-app-0.9.4/.envs/.production/.postgres
--rw-rw-r--   0 user      (1000) user      (1000)       12 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/.gitattributes
--rw-rw-r--   0 user      (1000) user      (1000)     5306 2021-01-25 18:57:01.000000 django-sso-app-0.9.4/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)      437 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/.pre-commit-config.yaml
--rw-rw-r--   0 user      (1000) user      (1000)      258 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/.pylintrc
--rw-rw-r--   0 user      (1000) user      (1000)       13 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/CONTRIBUTORS.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1081 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      704 2021-02-22 15:24:07.000000 django-sso-app-0.9.4/Makefile
--rw-r--r--   0 user      (1000) user      (1000)    10781 2021-02-22 16:52:33.460590 django-sso-app-0.9.4/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     8012 2021-02-22 16:41:44.000000 django-sso-app-0.9.4/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.408590 django-sso-app-0.9.4/compose/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.408590 django-sso-app-0.9.4/compose/local/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.419590 django-sso-app-0.9.4/compose/local/django/
--rw-rw-r--   0 user      (1000) user      (1000)     1391 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/local/django/Dockerfile
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.408590 django-sso-app-0.9.4/compose/local/django/celery/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.419590 django-sso-app-0.9.4/compose/local/django/celery/beat/
--rw-rw-r--   0 user      (1000) user      (1000)      111 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/local/django/celery/beat/start
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.419590 django-sso-app-0.9.4/compose/local/django/celery/flower/
--rw-rw-r--   0 user      (1000) user      (1000)      196 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/local/django/celery/flower/start
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.419590 django-sso-app-0.9.4/compose/local/django/celery/worker/
--rw-rw-r--   0 user      (1000) user      (1000)       88 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/local/django/celery/worker/start
--rw-rw-r--   0 user      (1000) user      (1000)      131 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/local/django/start
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.409590 django-sso-app-0.9.4/compose/production/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.419590 django-sso-app-0.9.4/compose/production/django/
--rw-rw-r--   0 user      (1000) user      (1000)     2597 2020-12-16 12:42:54.000000 django-sso-app-0.9.4/compose/production/django/Dockerfile
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.409590 django-sso-app-0.9.4/compose/production/django/celery/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.419590 django-sso-app-0.9.4/compose/production/django/celery/beat/
--rw-rw-r--   0 user      (1000) user      (1000)      117 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/django/celery/beat/start
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.420590 django-sso-app-0.9.4/compose/production/django/celery/flower/
--rw-rw-r--   0 user      (1000) user      (1000)      246 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/django/celery/flower/start
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.420590 django-sso-app-0.9.4/compose/production/django/celery/worker/
--rw-rw-r--   0 user      (1000) user      (1000)      119 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/django/celery/worker/start
--rw-rw-r--   0 user      (1000) user      (1000)      814 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/django/entrypoint
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.420590 django-sso-app-0.9.4/compose/production/django/maintenance/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.420590 django-sso-app-0.9.4/compose/production/django/maintenance/_sourced/
--rw-rw-r--   0 user      (1000) user      (1000)       77 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/django/maintenance/_sourced/constants.sh
--rw-rw-r--   0 user      (1000) user      (1000)      322 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/django/maintenance/_sourced/countdown.sh
--rw-rw-r--   0 user      (1000) user      (1000)      458 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/django/maintenance/_sourced/messages.sh
--rw-rw-r--   0 user      (1000) user      (1000)      293 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/django/maintenance/_sourced/yes_no.sh
--rw-rw-r--   0 user      (1000) user      (1000)      994 2020-09-16 12:36:28.000000 django-sso-app-0.9.4/compose/production/django/maintenance/backup
--rw-rw-r--   0 user      (1000) user      (1000)      392 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/django/maintenance/backups
--rw-rw-r--   0 user      (1000) user      (1000)      995 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/django/maintenance/restore
--rw-rw-r--   0 user      (1000) user      (1000)      131 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/django/start
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.421590 django-sso-app-0.9.4/compose/production/nginx/
--rw-rw-r--   0 user      (1000) user      (1000)       68 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/nginx/Dockerfile
--rw-rw-r--   0 user      (1000) user      (1000)     2127 2021-01-08 16:32:37.000000 django-sso-app-0.9.4/compose/production/nginx/nginx.conf
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.421590 django-sso-app-0.9.4/compose/production/postgres/
--rw-rw-r--   0 user      (1000) user      (1000)      228 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/postgres/Dockerfile
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.421590 django-sso-app-0.9.4/compose/production/postgres/maintenance/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.422590 django-sso-app-0.9.4/compose/production/postgres/maintenance/_sourced/
--rw-rw-r--   0 user      (1000) user      (1000)       77 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/postgres/maintenance/_sourced/constants.sh
--rw-rw-r--   0 user      (1000) user      (1000)      322 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/postgres/maintenance/_sourced/countdown.sh
--rw-rw-r--   0 user      (1000) user      (1000)      458 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/postgres/maintenance/_sourced/messages.sh
--rw-rw-r--   0 user      (1000) user      (1000)      293 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/postgres/maintenance/_sourced/yes_no.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1009 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/postgres/maintenance/backup
--rw-rw-r--   0 user      (1000) user      (1000)      392 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/postgres/maintenance/backups
--rw-rw-r--   0 user      (1000) user      (1000)     1635 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/postgres/maintenance/restore
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.422590 django-sso-app-0.9.4/compose/production/supervisor/
--rw-rw-r--   0 user      (1000) user      (1000)      128 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/supervisor/start-supervisor
--rw-rw-r--   0 user      (1000) user      (1000)      606 2020-09-15 14:16:37.000000 django-sso-app-0.9.4/compose/production/supervisor/supervisord.conf
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.422590 django-sso-app-0.9.4/compose/production/traefik/
--rw-rw-r--   0 user      (1000) user      (1000)      188 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/traefik/Dockerfile
--rw-rw-r--   0 user      (1000) user      (1000)     1809 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/compose/production/traefik/traefik.yml
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.423590 django-sso-app-0.9.4/docs/
--rw-rw-r--   0 user      (1000) user      (1000)      634 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/docs/Makefile
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.423590 django-sso-app-0.9.4/docs/_static/
--rw-rw-r--   0 user      (1000) user      (1000)       18 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/docs/_static/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)       41 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/docs/authors.rst
--rw-rw-r--   0 user      (1000) user      (1000)       43 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/docs/changelog.rst
--rw-rw-r--   0 user      (1000) user      (1000)     9679 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/docs/conf.py
--rw-rw-r--   0 user      (1000) user      (1000)     2235 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/docs/index.rst
--rw-rw-r--   0 user      (1000) user      (1000)       67 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/docs/license.rst
--rw-rw-r--   0 user      (1000) user      (1000)     1497 2020-09-15 12:14:00.000000 django-sso-app-0.9.4/local.yml
--rw-rw-r--   0 user      (1000) user      (1000)     1887 2021-01-25 18:50:02.000000 django-sso-app-0.9.4/production.yml
--rw-rw-r--   0 user      (1000) user      (1000)      105 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/pytest.ini
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.423590 django-sso-app-0.9.4/requirements/
--rw-rw-r--   0 user      (1000) user      (1000)     1151 2021-01-09 17:32:51.000000 django-sso-app-0.9.4/requirements/base.txt
--rw-rw-r--   0 user      (1000) user      (1000)      469 2021-01-09 17:10:50.000000 django-sso-app-0.9.4/requirements/extra.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1556 2021-01-09 17:13:29.000000 django-sso-app-0.9.4/requirements/local.txt
--rw-rw-r--   0 user      (1000) user      (1000)      452 2021-01-09 17:12:46.000000 django-sso-app-0.9.4/requirements/production.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1867 2021-02-22 16:52:33.461589 django-sso-app-0.9.4/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      578 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.423590 django-sso-app-0.9.4/src/
--rw-rw-r--   0 user      (1000) user      (1000)       43 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/compilemessages.sh
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.425590 django-sso-app-0.9.4/src/django_sso_app/
--rw-rw-r--   0 user      (1000) user      (1000)     2675 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)      441 2021-02-22 15:24:07.000000 django-sso-app-0.9.4/src/django_sso_app/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.426590 django-sso-app-0.9.4/src/django_sso_app/app/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/app/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      288 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/app/settings.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.426590 django-sso-app-0.9.4/src/django_sso_app/app/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/app/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2245 2021-01-11 19:30:54.000000 django-sso-app-0.9.4/src/django_sso_app/app/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)      535 2021-01-11 19:30:54.000000 django-sso-app-0.9.4/src/django_sso_app/app/views.py
--rw-rw-r--   0 user      (1000) user      (1000)      122 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/app_settings.py
--rw-rw-r--   0 user      (1000) user      (1000)      874 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/apps.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.427590 django-sso-app-0.9.4/src/django_sso_app/backend/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.427590 django-sso-app-0.9.4/src/django_sso_app/backend/api/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/api/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2814 2020-11-16 13:37:01.000000 django-sso-app-0.9.4/src/django_sso_app/backend/api/views.py
--rw-rw-r--   0 user      (1000) user      (1000)      310 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/conftest.py
--rw-rw-r--   0 user      (1000) user      (1000)     1521 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/context_processors.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.427590 django-sso-app-0.9.4/src/django_sso_app/backend/fixtures/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/fixtures/.gitkeep
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.428590 django-sso-app-0.9.4/src/django_sso_app/backend/pages/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/pages/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      758 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/pages/admin.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.428590 django-sso-app-0.9.4/src/django_sso_app/backend/pages/migrations/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/pages/migrations/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.410590 django-sso-app-0.9.4/src/django_sso_app/backend/pages/templates/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.428590 django-sso-app-0.9.4/src/django_sso_app/backend/pages/templates/flatpages/
--rw-rw-r--   0 user      (1000) user      (1000)      243 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/pages/templates/flatpages/default.html
--rw-rw-r--   0 user      (1000) user      (1000)      297 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/pages/views.py
--rw-r--r--   0 user      (1000) user      (1000)     3106 2021-02-10 11:06:45.000000 django-sso-app-0.9.4/src/django_sso_app/backend/settings.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.411590 django-sso-app-0.9.4/src/django_sso_app/backend/static/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.428590 django-sso-app-0.9.4/src/django_sso_app/backend/static/css/
--rw-rw-r--   0 user      (1000) user      (1000)     1330 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/static/css/accounts.css
--rw-rw-r--   0 user      (1000) user      (1000)       52 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/static/css/project.css
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.428590 django-sso-app-0.9.4/src/django_sso_app/backend/static/fonts/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/static/fonts/.gitkeep
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.410590 django-sso-app-0.9.4/src/django_sso_app/backend/static/images/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.428590 django-sso-app-0.9.4/src/django_sso_app/backend/static/images/favicons/
--rw-rw-r--   0 user      (1000) user      (1000)     8348 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/static/images/favicons/favicon.ico
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.428590 django-sso-app-0.9.4/src/django_sso_app/backend/static/js/
--rw-rw-r--   0 user      (1000) user      (1000)       46 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/static/js/accounts.js
--rw-rw-r--   0 user      (1000) user      (1000)       45 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/static/js/project.js
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.429590 django-sso-app-0.9.4/src/django_sso_app/backend/static/sass/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/static/sass/custom_bootstrap_vars.scss
--rw-rw-r--   0 user      (1000) user      (1000)      610 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/static/sass/project.scss
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.429590 django-sso-app-0.9.4/src/django_sso_app/backend/templates/
--rw-rw-r--   0 user      (1000) user      (1000)      194 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/403.html
--rw-rw-r--   0 user      (1000) user      (1000)      192 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/404.html
--rw-rw-r--   0 user      (1000) user      (1000)      313 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/500.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.431590 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/
--rw-rw-r--   0 user      (1000) user      (1000)      252 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/account_inactive.html
--rw-rw-r--   0 user      (1000) user      (1000)     1304 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/base.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.432590 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/email/
--rw-rw-r--   0 user      (1000) user      (1000)    14036 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/email/base_email.html
--rw-rw-r--   0 user      (1000) user      (1000)      602 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/email/email_confirmation_message.html
--rw-rw-r--   0 user      (1000) user      (1000)       62 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/email/email_confirmation_signup_message.html
--rw-rw-r--   0 user      (1000) user      (1000)     1100 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/email/password_reset_key_message.html
--rw-rw-r--   0 user      (1000) user      (1000)     2639 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/email.html
--rw-rw-r--   0 user      (1000) user      (1000)      968 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/email_confirm.html
--rw-rw-r--   0 user      (1000) user      (1000)     1529 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/login.html
--rw-rw-r--   0 user      (1000) user      (1000)      558 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/logout.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.432590 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/partials/
--rw-rw-r--   0 user      (1000) user      (1000)      882 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/partials/mapbox_initscript.html
--rw-rw-r--   0 user      (1000) user      (1000)      501 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/password_change.html
--rw-rw-r--   0 user      (1000) user      (1000)      870 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/password_reset.html
--rw-rw-r--   0 user      (1000) user      (1000)      484 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/password_reset_done.html
--rw-rw-r--   0 user      (1000) user      (1000)      992 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/password_reset_from_key.html
--rw-rw-r--   0 user      (1000) user      (1000)      261 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/password_reset_from_key_done.html
--rw-rw-r--   0 user      (1000) user      (1000)      486 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/password_set.html
--rw-rw-r--   0 user      (1000) user      (1000)     1425 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/profile.html
--rw-rw-r--   0 user      (1000) user      (1000)     1604 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/profile_complete.html
--rw-rw-r--   0 user      (1000) user      (1000)     1602 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/profile_update.html
--rw-rw-r--   0 user      (1000) user      (1000)     1030 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/signup.html
--rw-rw-r--   0 user      (1000) user      (1000)      274 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/signup_closed.html
--rw-rw-r--   0 user      (1000) user      (1000)      447 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/verification_sent.html
--rw-rw-r--   0 user      (1000) user      (1000)      807 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/verified_email_required.html
--rw-rw-r--   0 user      (1000) user      (1000)     2534 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/base.html
--rw-rw-r--   0 user      (1000) user      (1000)      833 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/cookie_consent.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.432590 django-sso-app-0.9.4/src/django_sso_app/backend/templates/flatpages/
--rw-rw-r--   0 user      (1000) user      (1000)      226 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/flatpages/default.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.432590 django-sso-app-0.9.4/src/django_sso_app/backend/templates/pages/
--rw-rw-r--   0 user      (1000) user      (1000)      296 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/pages/home.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.432590 django-sso-app-0.9.4/src/django_sso_app/backend/templates/partials/
--rw-rw-r--   0 user      (1000) user      (1000)      355 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/partials/google_analytics_site_tag.html
--rw-rw-r--   0 user      (1000) user      (1000)     1328 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/partials/nav_footer.html
--rw-rw-r--   0 user      (1000) user      (1000)     1895 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/partials/nav_pills.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.433590 django-sso-app-0.9.4/src/django_sso_app/backend/templates/polyfills/
--rw-rw-r--   0 user      (1000) user      (1000)      850 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/polyfills/console_polyfill.html
--rw-rw-r--   0 user      (1000) user      (1000)      575 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/polyfills/custom_event_polyfill.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.433590 django-sso-app-0.9.4/src/django_sso_app/backend/templates/users/
--rw-rw-r--   0 user      (1000) user      (1000)      763 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/users/user_detail.html
--rw-rw-r--   0 user      (1000) user      (1000)      615 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/templates/users/user_form.html
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.433590 django-sso-app-0.9.4/src/django_sso_app/backend/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2184 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/urls.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.434590 django-sso-app-0.9.4/src/django_sso_app/backend/users/
--rw-rw-r--   0 user      (1000) user      (1000)       68 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      192 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/admin.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.434590 django-sso-app-0.9.4/src/django_sso_app/backend/users/api/
--rw-rw-r--   0 user      (1000) user      (1000)       69 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/api/serializers.py
--rw-rw-r--   0 user      (1000) user      (1000)       99 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/api/views.py
--rw-rw-r--   0 user      (1000) user      (1000)      320 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/apps.py
--rw-rw-r--   0 user      (1000) user      (1000)      298 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/forms.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.434590 django-sso-app-0.9.4/src/django_sso_app/backend/users/migrations/
--rw-rw-r--   0 user      (1000) user      (1000)     4722 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/migrations/0001_initial.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/migrations/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      536 2021-02-03 16:34:19.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/models.py
--rw-rw-r--   0 user      (1000) user      (1000)      238 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/tasks.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.435590 django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      838 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/factories.py
--rw-rw-r--   0 user      (1000) user      (1000)     1143 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/test_forms.py
--rw-rw-r--   0 user      (1000) user      (1000)      215 2021-02-03 16:34:19.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/test_models.py
--rw-rw-r--   0 user      (1000) user      (1000)      523 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/test_tasks.py
--rw-rw-r--   0 user      (1000) user      (1000)      672 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/test_urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     1353 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/test_views.py
--rw-rw-r--   0 user      (1000) user      (1000)      380 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     1296 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/users/views.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.435590 django-sso-app-0.9.4/src/django_sso_app/backend/utils/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/utils/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      372 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backend/utils/context_processors.py
--rw-rw-r--   0 user      (1000) user      (1000)     1269 2021-02-22 16:45:30.000000 django-sso-app-0.9.4/src/django_sso_app/backend/views.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.435590 django-sso-app-0.9.4/src/django_sso_app/backups/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/backups/.gitkeep
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.436590 django-sso-app-0.9.4/src/django_sso_app/config/
--rw-rw-r--   0 user      (1000) user      (1000)      178 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/config/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      593 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/config/celery_app.py
--rw-rw-r--   0 user      (1000) user      (1000)       60 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/config/extra_urls.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.437590 django-sso-app-0.9.4/src/django_sso_app/config/settings/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/config/settings/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    19226 2021-02-22 16:38:02.000000 django-sso-app-0.9.4/src/django_sso_app/config/settings/base.py
--rw-rw-r--   0 user      (1000) user      (1000)       34 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/config/settings/extra.py
--rw-rw-r--   0 user      (1000) user      (1000)      241 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/config/settings/languages.py
--rw-rw-r--   0 user      (1000) user      (1000)     3286 2021-02-05 09:02:12.000000 django-sso-app-0.9.4/src/django_sso_app/config/settings/local.py
--rw-rw-r--   0 user      (1000) user      (1000)     7711 2021-02-10 13:08:31.000000 django-sso-app-0.9.4/src/django_sso_app/config/settings/production.py
--rw-rw-r--   0 user      (1000) user      (1000)     1773 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/config/settings/test.py
--rw-rw-r--   0 user      (1000) user      (1000)     4944 2021-02-22 16:47:00.000000 django-sso-app-0.9.4/src/django_sso_app/config/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     1708 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/config/wsgi.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.439590 django-sso-app-0.9.4/src/django_sso_app/core/
--rw-rw-r--   0 user      (1000) user      (1000)        1 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5433 2021-02-08 20:23:44.000000 django-sso-app-0.9.4/src/django_sso_app/core/adapter.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.439590 django-sso-app-0.9.4/src/django_sso_app/core/api/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/api/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      480 2021-02-08 07:11:37.000000 django-sso-app-0.9.4/src/django_sso_app/core/api/authentication.py
--rw-rw-r--   0 user      (1000) user      (1000)     5399 2021-02-08 11:49:53.000000 django-sso-app-0.9.4/src/django_sso_app/core/api/serializers.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.439590 django-sso-app-0.9.4/src/django_sso_app/core/api/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/api/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9876 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/api/tests/test_views.py
--rw-rw-r--   0 user      (1000) user      (1000)     1096 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/api/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)      450 2021-02-05 16:56:38.000000 django-sso-app-0.9.4/src/django_sso_app/core/api/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)    16944 2021-02-09 11:51:11.000000 django-sso-app-0.9.4/src/django_sso_app/core/api/views.py
--rw-rw-r--   0 user      (1000) user      (1000)    11543 2021-02-09 15:06:14.000000 django-sso-app-0.9.4/src/django_sso_app/core/app_settings.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.440590 django-sso-app-0.9.4/src/django_sso_app/core/apps/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.440590 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)       72 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/functions.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.440590 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/kong/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/kong/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      366 2021-02-22 14:36:11.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/kong/functions.py
--rw-rw-r--   0 user      (1000) user      (1000)    10305 2021-02-22 14:36:11.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/kong/utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.441590 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/signals/
--rw-rw-r--   0 user      (1000) user      (1000)      366 2020-12-14 18:02:06.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/signals/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/signals/app.py
--rw-rw-r--   0 user      (1000) user      (1000)     5679 2021-02-09 12:16:18.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/signals/backend.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.441590 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      350 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/tests/test_views.py
--rw-rw-r--   0 user      (1000) user      (1000)       26 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.442590 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      312 2021-02-22 13:57:45.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/admin.py
--rw-rw-r--   0 user      (1000) user      (1000)     1668 2021-02-03 16:22:56.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/models.py
--rw-rw-r--   0 user      (1000) user      (1000)      633 2021-02-03 16:22:56.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/serializers.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.442590 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/signals/
--rw-rw-r--   0 user      (1000) user      (1000)      310 2020-12-14 18:02:06.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/signals/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/signals/app.py
--rw-rw-r--   0 user      (1000) user      (1000)     4391 2021-02-09 12:09:42.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/signals/backend.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.442590 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      159 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/tests/test_models.py
--rw-rw-r--   0 user      (1000) user      (1000)      433 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     4597 2021-02-10 10:48:09.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     1084 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/views.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.443590 django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)       48 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/models.py
--rw-rw-r--   0 user      (1000) user      (1000)      269 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/serializers.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.443590 django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/signals/
--rw-rw-r--   0 user      (1000) user      (1000)      310 2020-12-14 18:02:06.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/signals/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/signals/app.py
--rw-rw-r--   0 user      (1000) user      (1000)     1244 2020-12-14 11:54:57.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/signals/backend.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.443590 django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1445 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/tests/test_models.py
--rw-r--r--   0 user      (1000) user      (1000)      280 2021-02-08 14:20:10.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.444590 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      476 2021-02-03 16:23:55.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/models.py
--rw-rw-r--   0 user      (1000) user      (1000)      244 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/serializers.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.444590 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/signals/
--rw-rw-r--   0 user      (1000) user      (1000)      310 2020-12-14 18:02:06.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/signals/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2021-02-05 10:00:47.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/signals/app.py
--rw-r--r--   0 user      (1000) user      (1000)     3103 2021-02-09 10:05:31.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/signals/backend.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.444590 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1580 2021-02-08 15:26:47.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/tests/test_models.py
--rw-r--r--   0 user      (1000) user      (1000)     1470 2021-02-08 17:06:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/tests/test_views.py
--rw-rw-r--   0 user      (1000) user      (1000)      398 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     2815 2021-02-10 12:48:31.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)      709 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/views.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.445590 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      385 2021-02-22 15:24:07.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/admin.py
--rw-rw-r--   0 user      (1000) user      (1000)     1839 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/functions.py
--rw-r--r--   0 user      (1000) user      (1000)     1689 2021-02-22 15:26:02.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/models.py
--rw-rw-r--   0 user      (1000) user      (1000)      417 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/settings.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/signals.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.446590 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)       79 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/tests/test_models.py
--rw-rw-r--   0 user      (1000) user      (1000)     2947 2021-02-22 15:25:28.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/tests/test_views.py
--rw-rw-r--   0 user      (1000) user      (1000)      335 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     2252 2021-02-09 10:27:30.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     5755 2021-02-22 15:25:28.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/views.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.447590 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/
--rw-rw-r--   0 user      (1000) user      (1000)      115 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/README.md
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      317 2021-02-22 14:25:29.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/admin.py
--rw-rw-r--   0 user      (1000) user      (1000)      354 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/filters.py
--rw-rw-r--   0 user      (1000) user      (1000)     3926 2021-02-22 14:37:16.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/forms.py
--rw-rw-r--   0 user      (1000) user      (1000)     9587 2021-02-22 14:37:16.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/models.py
--rw-rw-r--   0 user      (1000) user      (1000)     5109 2021-02-22 14:37:16.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/serializers.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.447590 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/signals/
--rw-rw-r--   0 user      (1000) user      (1000)      310 2020-12-14 18:02:06.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/signals/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      967 2021-02-08 12:09:04.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/signals/app.py
--rw-rw-r--   0 user      (1000) user      (1000)     2685 2021-02-09 12:05:29.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/signals/backend.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.447590 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1704 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/tests/test_models.py
--rw-rw-r--   0 user      (1000) user      (1000)     7522 2021-02-09 12:02:56.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/tests/test_views.py
--rw-rw-r--   0 user      (1000) user      (1000)      796 2021-02-09 12:03:15.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/urls.py
--rw-r--r--   0 user      (1000) user      (1000)     6609 2021-02-10 13:15:06.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     5669 2021-02-09 12:02:56.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/views.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.448590 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1785 2021-02-22 14:37:16.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/admin.py
--rw-rw-r--   0 user      (1000) user      (1000)     4774 2021-02-08 19:29:16.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/models.py
--rw-rw-r--   0 user      (1000) user      (1000)     3370 2021-02-03 16:22:56.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/serializers.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.449590 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/signals/
--rw-rw-r--   0 user      (1000) user      (1000)      310 2020-12-14 18:02:06.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/signals/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/signals/app.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2021-02-08 19:32:35.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/signals/backend.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.449590 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9310 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/tests/test_views.py
--rw-rw-r--   0 user      (1000) user      (1000)     1256 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     1907 2021-02-09 12:02:56.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     5431 2021-02-09 12:16:18.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/services/views.py
--rw-rw-r--   0 user      (1000) user      (1000)      121 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/settings.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.449590 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      216 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/admin.py
--rw-rw-r--   0 user      (1000) user      (1000)      613 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/models.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.450590 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/signals/
--rw-r--r--   0 user      (1000) user      (1000)      310 2021-02-09 09:59:08.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/signals/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      445 2021-02-09 10:01:20.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/signals/app.py
--rw-rw-r--   0 user      (1000) user      (1000)      445 2021-02-09 10:01:20.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/signals/backend.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.450590 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    13414 2021-02-10 13:21:04.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/tests/test_app.py
--rw-rw-r--   0 user      (1000) user      (1000)     4950 2021-02-04 14:26:10.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/tests/test_backend.py
--rw-rw-r--   0 user      (1000) user      (1000)     5593 2021-02-05 16:31:31.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/status/tests/test_views.py
--rw-rw-r--   0 user      (1000) user      (1000)     1749 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/tests.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.451590 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/
--rw-rw-r--   0 user      (1000) user      (1000)      425 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/README.md
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1156 2021-02-22 14:32:12.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/admin.py
--rw-rw-r--   0 user      (1000) user      (1000)      482 2020-12-03 12:01:22.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/filters.py
--rw-rw-r--   0 user      (1000) user      (1000)     1384 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/forms.py
--rw-rw-r--   0 user      (1000) user      (1000)     5334 2021-02-22 14:36:11.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/models.py
--rw-rw-r--   0 user      (1000) user      (1000)    14153 2021-02-09 12:16:18.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/serializers.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.452590 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/signals/
--rw-rw-r--   0 user      (1000) user      (1000)      310 2020-12-14 18:02:06.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/signals/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/signals/app.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-12-14 12:46:06.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/signals/backend.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.452590 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      712 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/tests/test_models.py
--rw-rw-r--   0 user      (1000) user      (1000)    16218 2021-02-05 17:22:26.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/tests/test_views.py
--rw-rw-r--   0 user      (1000) user      (1000)     1076 2020-10-14 14:57:25.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     8801 2021-02-10 11:34:17.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     7352 2021-02-09 12:16:18.000000 django-sso-app-0.9.4/src/django_sso_app/core/apps/users/views.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.452590 django-sso-app-0.9.4/src/django_sso_app/core/authentication/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/authentication/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.452590 django-sso-app-0.9.4/src/django_sso_app/core/authentication/backends/
--rw-rw-r--   0 user      (1000) user      (1000)     2368 2021-02-05 17:15:23.000000 django-sso-app-0.9.4/src/django_sso_app/core/authentication/backends/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6389 2021-02-10 13:11:14.000000 django-sso-app-0.9.4/src/django_sso_app/core/authentication/backends/app.py
--rw-rw-r--   0 user      (1000) user      (1000)     2392 2021-02-08 14:06:49.000000 django-sso-app-0.9.4/src/django_sso_app/core/authentication/backends/backend.py
--rw-r--r--   0 user      (1000) user      (1000)      731 2021-02-08 20:14:47.000000 django-sso-app-0.9.4/src/django_sso_app/core/authentication/backends/login.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.453590 django-sso-app-0.9.4/src/django_sso_app/core/authentication/middleware/
--rw-rw-r--   0 user      (1000) user      (1000)    10065 2021-02-10 12:16:18.000000 django-sso-app-0.9.4/src/django_sso_app/core/authentication/middleware/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2306 2021-02-10 12:21:39.000000 django-sso-app-0.9.4/src/django_sso_app/core/authentication/middleware/app.py
--rw-rw-r--   0 user      (1000) user      (1000)     1864 2021-02-08 14:06:49.000000 django-sso-app-0.9.4/src/django_sso_app/core/authentication/middleware/backend.py
--rw-rw-r--   0 user      (1000) user      (1000)     3408 2021-02-10 12:20:01.000000 django-sso-app-0.9.4/src/django_sso_app/core/authentication/middleware/base.py
--rw-rw-r--   0 user      (1000) user      (1000)      835 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/context_processors.py
--rw-rw-r--   0 user      (1000) user      (1000)      810 2021-02-08 20:04:37.000000 django-sso-app-0.9.4/src/django_sso_app/core/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     5798 2021-02-22 14:36:11.000000 django-sso-app-0.9.4/src/django_sso_app/core/forms.py
--rw-rw-r--   0 user      (1000) user      (1000)     1386 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/functions.py
--rw-rw-r--   0 user      (1000) user      (1000)      720 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/loader.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.453590 django-sso-app-0.9.4/src/django_sso_app/core/middleware/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/middleware/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      355 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/middleware/same_site.py
--rw-rw-r--   0 user      (1000) user      (1000)      317 2021-02-04 19:39:14.000000 django-sso-app-0.9.4/src/django_sso_app/core/middleware/x_forwarded_for.py
--rw-rw-r--   0 user      (1000) user      (1000)      795 2021-02-09 10:02:27.000000 django-sso-app-0.9.4/src/django_sso_app/core/mixins.py
--rw-rw-r--   0 user      (1000) user      (1000)     1516 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/models.py
--rw-rw-r--   0 user      (1000) user      (1000)     2760 2021-02-09 10:06:54.000000 django-sso-app-0.9.4/src/django_sso_app/core/permissions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1913 2021-02-03 16:28:13.000000 django-sso-app-0.9.4/src/django_sso_app/core/serializers.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.453590 django-sso-app-0.9.4/src/django_sso_app/core/settings/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/settings/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2038 2021-01-07 15:17:35.000000 django-sso-app-0.9.4/src/django_sso_app/core/settings/common.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.454589 django-sso-app-0.9.4/src/django_sso_app/core/solidity/
--rw-rw-r--   0 user      (1000) user      (1000)    10363 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/solidity/DjangoSsoAppProfileContract.sol
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.454589 django-sso-app-0.9.4/src/django_sso_app/core/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    11633 2021-02-08 14:51:04.000000 django-sso-app-0.9.4/src/django_sso_app/core/tests/factories.py
--rw-rw-r--   0 user      (1000) user      (1000)    10427 2021-02-08 16:58:44.000000 django-sso-app-0.9.4/src/django_sso_app/core/tests/test_views.py
--rw-rw-r--   0 user      (1000) user      (1000)      127 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/to_translate.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.454589 django-sso-app-0.9.4/src/django_sso_app/core/tokens/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/tokens/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3332 2020-12-14 14:28:35.000000 django-sso-app-0.9.4/src/django_sso_app/core/tokens/authentication.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.454589 django-sso-app-0.9.4/src/django_sso_app/core/tokens/tests/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/core/tokens/tests/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2387 2021-02-04 14:25:20.000000 django-sso-app-0.9.4/src/django_sso_app/core/tokens/tests/test_views.py
--rw-rw-r--   0 user      (1000) user      (1000)     4329 2021-02-08 15:14:13.000000 django-sso-app-0.9.4/src/django_sso_app/core/tokens/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)     3730 2020-12-14 14:26:09.000000 django-sso-app-0.9.4/src/django_sso_app/core/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     5243 2021-02-22 16:45:27.000000 django-sso-app-0.9.4/src/django_sso_app/core/utils.py
--rw-rw-r--   0 user      (1000) user      (1000)    13509 2021-02-22 14:36:11.000000 django-sso-app-0.9.4/src/django_sso_app/core/views.py
--rw-rw-r--   0 user      (1000) user      (1000)   466944 2021-01-07 14:45:21.000000 django-sso-app-0.9.4/src/django_sso_app/db.sqlite3
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.455590 django-sso-app-0.9.4/src/django_sso_app/fixtures/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/fixtures/.gitkeep
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.455590 django-sso-app-0.9.4/src/django_sso_app/locale/
--rw-rw-r--   0 user      (1000) user      (1000)      120 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/README.rst
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.415590 django-sso-app-0.9.4/src/django_sso_app/locale/de/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.455590 django-sso-app-0.9.4/src/django_sso_app/locale/de/LC_MESSAGES/
--rw-rw-r--   0 user      (1000) user      (1000)    24826 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 user      (1000) user      (1000)    27728 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.415590 django-sso-app-0.9.4/src/django_sso_app/locale/en/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.455590 django-sso-app-0.9.4/src/django_sso_app/locale/en/LC_MESSAGES/
--rw-rw-r--   0 user      (1000) user      (1000)    24826 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/en/LC_MESSAGES/django.po
--rw-rw-r--   0 user      (1000) user      (1000)    27728 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.415590 django-sso-app-0.9.4/src/django_sso_app/locale/es/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.455590 django-sso-app-0.9.4/src/django_sso_app/locale/es/LC_MESSAGES/
--rw-rw-r--   0 user      (1000) user      (1000)    24826 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/es/LC_MESSAGES/django.po
--rw-rw-r--   0 user      (1000) user      (1000)    27728 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.415590 django-sso-app-0.9.4/src/django_sso_app/locale/fr/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.456590 django-sso-app-0.9.4/src/django_sso_app/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 user      (1000) user      (1000)    24825 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 user      (1000) user      (1000)    27727 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.415590 django-sso-app-0.9.4/src/django_sso_app/locale/it/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.456590 django-sso-app-0.9.4/src/django_sso_app/locale/it/LC_MESSAGES/
--rw-rw-r--   0 user      (1000) user      (1000)    10733 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 user      (1000) user      (1000)    28829 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/it/LC_MESSAGES/django.po
--rw-rw-r--   0 user      (1000) user      (1000)     8559 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/it/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 user      (1000) user      (1000)    30620 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/it/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.415590 django-sso-app-0.9.4/src/django_sso_app/locale/nl/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.456590 django-sso-app-0.9.4/src/django_sso_app/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 user      (1000) user      (1000)    24826 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/nl/LC_MESSAGES/django.po
--rw-rw-r--   0 user      (1000) user      (1000)    27728 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/nl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.415590 django-sso-app-0.9.4/src/django_sso_app/locale/pt/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.457589 django-sso-app-0.9.4/src/django_sso_app/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 user      (1000) user      (1000)      421 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 user      (1000) user      (1000)    24826 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/pt/LC_MESSAGES/django.po
--rw-rw-r--   0 user      (1000) user      (1000)      486 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/pt/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 user      (1000) user      (1000)    27927 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/locale/pt/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.457589 django-sso-app-0.9.4/src/django_sso_app/logs/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/logs/.gitkeep
--rw-rw-r--   0 user      (1000) user      (1000)      852 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/manage.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.457589 django-sso-app-0.9.4/src/django_sso_app/management/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/management/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.458589 django-sso-app-0.9.4/src/django_sso_app/management/commands/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/management/commands/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1102 2021-02-09 12:25:19.000000 django-sso-app-0.9.4/src/django_sso_app/management/commands/clear_api_gateway_consumer_ids.py
--rw-rw-r--   0 user      (1000) user      (1000)     2126 2021-02-09 12:17:04.000000 django-sso-app-0.9.4/src/django_sso_app/management/commands/create_user_with_simple_profile.py
--rw-rw-r--   0 user      (1000) user      (1000)     1804 2021-02-09 12:17:04.000000 django-sso-app-0.9.4/src/django_sso_app/management/commands/delete_all_profiles_devices.py
--rw-rw-r--   0 user      (1000) user      (1000)     1971 2021-02-09 12:16:18.000000 django-sso-app-0.9.4/src/django_sso_app/management/commands/delete_all_users_devices_by_username.py
--rw-rw-r--   0 user      (1000) user      (1000)     1462 2021-02-09 12:11:42.000000 django-sso-app-0.9.4/src/django_sso_app/management/commands/restore_api_gateway_consumers.py
--rw-rw-r--   0 user      (1000) user      (1000)     1730 2021-02-09 12:11:42.000000 django-sso-app-0.9.4/src/django_sso_app/management/commands/restore_api_gateway_consumers_by_username.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.459590 django-sso-app-0.9.4/src/django_sso_app/migrations/
--rw-rw-r--   0 user      (1000) user      (1000)    10502 2020-12-14 13:46:34.000000 django-sso-app-0.9.4/src/django_sso_app/migrations/0001_initial.py
--rw-rw-r--   0 user      (1000) user      (1000)     1036 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/migrations/0002_auto_20200307_1035.py
--rw-rw-r--   0 user      (1000) user      (1000)      569 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/migrations/0003_emailaddress.py
--rw-rw-r--   0 user      (1000) user      (1000)     1481 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/migrations/0004_django_user_fields_in_profile__20200417_1757.py
--rw-rw-r--   0 user      (1000) user      (1000)     1069 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/migrations/0005_auto_20200519_1725.py
--rw-rw-r--   0 user      (1000) user      (1000)      309 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/migrations/0006_delete_emailaddress.py
--rw-r--r--   0 user      (1000) user      (1000)      482 2021-02-22 15:26:55.000000 django-sso-app-0.9.4/src/django_sso_app/migrations/0007_auto_20210222_1526.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/migrations/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      300 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/models.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.459590 django-sso-app-0.9.4/src/django_sso_app/private/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/private/.gitkeep
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.459590 django-sso-app-0.9.4/src/django_sso_app/private/users/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/private/users/.gitkeep
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.416590 django-sso-app-0.9.4/src/django_sso_app/public/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.459590 django-sso-app-0.9.4/src/django_sso_app/public/media/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/public/media/.gitkeep
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.459590 django-sso-app-0.9.4/src/django_sso_app/public/static/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/public/static/.gitkeep
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.459590 django-sso-app-0.9.4/src/django_sso_app/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)       43 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/scripts/compilemessages.sh
--rw-rw-r--   0 user      (1000) user      (1000)      311 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/scripts/makemessages.sh
--rw-rw-r--   0 user      (1000) user      (1000)      155 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/settings.py
--rw-rw-r--   0 user      (1000) user      (1000)     3643 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/skeleton.py
--rw-rw-r--   0 user      (1000) user      (1000)     1203 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/django_sso_app/urls.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-02-22 16:52:33.426590 django-sso-app-0.9.4/src/django_sso_app.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    10781 2021-02-22 16:52:33.000000 django-sso-app-0.9.4/src/django_sso_app.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)    18131 2021-02-22 16:52:33.000000 django-sso-app-0.9.4/src/django_sso_app.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2021-02-22 16:52:33.000000 django-sso-app-0.9.4/src/django_sso_app.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       64 2021-02-22 16:52:33.000000 django-sso-app-0.9.4/src/django_sso_app.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2021-02-22 16:52:33.000000 django-sso-app-0.9.4/src/django_sso_app.egg-info/not-zip-safe
--rw-r--r--   0 user      (1000) user      (1000)      410 2021-02-22 16:52:33.000000 django-sso-app-0.9.4/src/django_sso_app.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       15 2021-02-22 16:52:33.000000 django-sso-app-0.9.4/src/django_sso_app.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      243 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/makemessages.sh
--rw-rw-r--   0 user      (1000) user      (1000)      853 2020-08-24 11:58:21.000000 django-sso-app-0.9.4/src/manage.py
--rw-rw-r--   0 user      (1000) user      (1000)     1810 2020-12-16 13:23:58.000000 django-sso-app-0.9.4/src/server.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.956517 django-sso-app-0.9.6/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.907518 django-sso-app-0.9.6/.certs/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-09-15 12:15:30.000000 django-sso-app-0.9.6/.certs/.gitkeep
+-rw-rw-r--   0 user      (1000) user      (1000)      104 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/.coveragerc
+-rw-rw-r--   0 user      (1000) user      (1000)      138 2021-01-11 13:05:40.000000 django-sso-app-0.9.6/.dockerignore
+-rw-rw-r--   0 user      (1000) user      (1000)      631 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/.editorconfig
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.897518 django-sso-app-0.9.6/.envs/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.908518 django-sso-app-0.9.6/.envs/.local/
+-rw-rw-r--   0 user      (1000) user      (1000)      594 2021-01-25 18:54:32.000000 django-sso-app-0.9.6/.envs/.local/.django
+-rw-rw-r--   0 user      (1000) user      (1000)      225 2020-09-15 12:09:20.000000 django-sso-app-0.9.6/.envs/.local/.postgres
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.908518 django-sso-app-0.9.6/.envs/.production/
+-rw-r--r--   0 user      (1000) user      (1000)     1509 2021-01-25 18:59:11.000000 django-sso-app-0.9.6/.envs/.production/.django
+-rw-r--r--   0 user      (1000) user      (1000)      225 2021-01-25 18:59:11.000000 django-sso-app-0.9.6/.envs/.production/.postgres
+-rw-rw-r--   0 user      (1000) user      (1000)       12 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/.gitattributes
+-rw-rw-r--   0 user      (1000) user      (1000)     5306 2021-01-25 18:57:01.000000 django-sso-app-0.9.6/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)      437 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/.pre-commit-config.yaml
+-rw-rw-r--   0 user      (1000) user      (1000)      258 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/.pylintrc
+-rw-rw-r--   0 user      (1000) user      (1000)       13 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/CONTRIBUTORS.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1081 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      705 2021-03-09 15:15:54.000000 django-sso-app-0.9.6/Makefile
+-rw-r--r--   0 user      (1000) user      (1000)    10781 2021-03-09 15:17:01.956517 django-sso-app-0.9.6/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     8012 2021-02-22 16:41:44.000000 django-sso-app-0.9.6/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.898518 django-sso-app-0.9.6/compose/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.897518 django-sso-app-0.9.6/compose/local/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.908518 django-sso-app-0.9.6/compose/local/django/
+-rw-rw-r--   0 user      (1000) user      (1000)     1391 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/local/django/Dockerfile
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.898518 django-sso-app-0.9.6/compose/local/django/celery/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.908518 django-sso-app-0.9.6/compose/local/django/celery/beat/
+-rw-rw-r--   0 user      (1000) user      (1000)      111 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/local/django/celery/beat/start
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.908518 django-sso-app-0.9.6/compose/local/django/celery/flower/
+-rw-rw-r--   0 user      (1000) user      (1000)      196 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/local/django/celery/flower/start
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.908518 django-sso-app-0.9.6/compose/local/django/celery/worker/
+-rw-rw-r--   0 user      (1000) user      (1000)       88 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/local/django/celery/worker/start
+-rw-rw-r--   0 user      (1000) user      (1000)      131 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/local/django/start
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.898518 django-sso-app-0.9.6/compose/production/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.909518 django-sso-app-0.9.6/compose/production/django/
+-rw-rw-r--   0 user      (1000) user      (1000)     2597 2020-12-16 12:42:54.000000 django-sso-app-0.9.6/compose/production/django/Dockerfile
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.898518 django-sso-app-0.9.6/compose/production/django/celery/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.909518 django-sso-app-0.9.6/compose/production/django/celery/beat/
+-rw-rw-r--   0 user      (1000) user      (1000)      117 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/django/celery/beat/start
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.909518 django-sso-app-0.9.6/compose/production/django/celery/flower/
+-rw-rw-r--   0 user      (1000) user      (1000)      246 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/django/celery/flower/start
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.909518 django-sso-app-0.9.6/compose/production/django/celery/worker/
+-rw-rw-r--   0 user      (1000) user      (1000)      119 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/django/celery/worker/start
+-rw-rw-r--   0 user      (1000) user      (1000)      814 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/django/entrypoint
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.910518 django-sso-app-0.9.6/compose/production/django/maintenance/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.910518 django-sso-app-0.9.6/compose/production/django/maintenance/_sourced/
+-rw-rw-r--   0 user      (1000) user      (1000)       77 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/django/maintenance/_sourced/constants.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      322 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/django/maintenance/_sourced/countdown.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      458 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/django/maintenance/_sourced/messages.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      293 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/django/maintenance/_sourced/yes_no.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      994 2020-09-16 12:36:28.000000 django-sso-app-0.9.6/compose/production/django/maintenance/backup
+-rw-rw-r--   0 user      (1000) user      (1000)      392 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/django/maintenance/backups
+-rw-rw-r--   0 user      (1000) user      (1000)      995 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/django/maintenance/restore
+-rw-rw-r--   0 user      (1000) user      (1000)      131 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/django/start
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.910518 django-sso-app-0.9.6/compose/production/nginx/
+-rw-rw-r--   0 user      (1000) user      (1000)       68 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/nginx/Dockerfile
+-rw-rw-r--   0 user      (1000) user      (1000)     2127 2021-01-08 16:32:37.000000 django-sso-app-0.9.6/compose/production/nginx/nginx.conf
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.910518 django-sso-app-0.9.6/compose/production/postgres/
+-rw-rw-r--   0 user      (1000) user      (1000)      228 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/postgres/Dockerfile
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.911518 django-sso-app-0.9.6/compose/production/postgres/maintenance/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.911518 django-sso-app-0.9.6/compose/production/postgres/maintenance/_sourced/
+-rw-rw-r--   0 user      (1000) user      (1000)       77 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/postgres/maintenance/_sourced/constants.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      322 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/postgres/maintenance/_sourced/countdown.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      458 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/postgres/maintenance/_sourced/messages.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      293 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/postgres/maintenance/_sourced/yes_no.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1009 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/postgres/maintenance/backup
+-rw-rw-r--   0 user      (1000) user      (1000)      392 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/postgres/maintenance/backups
+-rw-rw-r--   0 user      (1000) user      (1000)     1635 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/postgres/maintenance/restore
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.911518 django-sso-app-0.9.6/compose/production/supervisor/
+-rw-rw-r--   0 user      (1000) user      (1000)      128 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/supervisor/start-supervisor
+-rw-rw-r--   0 user      (1000) user      (1000)      606 2020-09-15 14:16:37.000000 django-sso-app-0.9.6/compose/production/supervisor/supervisord.conf
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.912518 django-sso-app-0.9.6/compose/production/traefik/
+-rw-rw-r--   0 user      (1000) user      (1000)      188 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/traefik/Dockerfile
+-rw-rw-r--   0 user      (1000) user      (1000)     1809 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/compose/production/traefik/traefik.yml
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.912518 django-sso-app-0.9.6/docs/
+-rw-rw-r--   0 user      (1000) user      (1000)      634 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/docs/Makefile
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.912518 django-sso-app-0.9.6/docs/_static/
+-rw-rw-r--   0 user      (1000) user      (1000)       18 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/docs/_static/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)       41 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/docs/authors.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/docs/changelog.rst
+-rw-rw-r--   0 user      (1000) user      (1000)     9679 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/docs/conf.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2235 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/docs/index.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       67 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/docs/license.rst
+-rw-rw-r--   0 user      (1000) user      (1000)     1497 2020-09-15 12:14:00.000000 django-sso-app-0.9.6/local.yml
+-rw-rw-r--   0 user      (1000) user      (1000)     1887 2021-01-25 18:50:02.000000 django-sso-app-0.9.6/production.yml
+-rw-rw-r--   0 user      (1000) user      (1000)      105 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/pytest.ini
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.913518 django-sso-app-0.9.6/requirements/
+-rw-rw-r--   0 user      (1000) user      (1000)     1151 2021-01-09 17:32:51.000000 django-sso-app-0.9.6/requirements/base.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      469 2021-01-09 17:10:50.000000 django-sso-app-0.9.6/requirements/extra.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1556 2021-01-09 17:13:29.000000 django-sso-app-0.9.6/requirements/local.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      452 2021-01-09 17:12:46.000000 django-sso-app-0.9.6/requirements/production.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1867 2021-03-09 15:17:01.957517 django-sso-app-0.9.6/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      578 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.913518 django-sso-app-0.9.6/src/
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/compilemessages.sh
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.916518 django-sso-app-0.9.6/src/django_sso_app/
+-rw-rw-r--   0 user      (1000) user      (1000)     2675 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)      441 2021-03-09 15:10:55.000000 django-sso-app-0.9.6/src/django_sso_app/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.917518 django-sso-app-0.9.6/src/django_sso_app/app/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/app/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      288 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/app/settings.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.917518 django-sso-app-0.9.6/src/django_sso_app/app/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/app/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2245 2021-01-11 19:30:54.000000 django-sso-app-0.9.6/src/django_sso_app/app/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)      685 2021-03-09 15:08:14.000000 django-sso-app-0.9.6/src/django_sso_app/app/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)      122 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/app_settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)      874 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/apps.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.918517 django-sso-app-0.9.6/src/django_sso_app/backend/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.918517 django-sso-app-0.9.6/src/django_sso_app/backend/api/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/api/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2814 2020-11-16 13:37:01.000000 django-sso-app-0.9.6/src/django_sso_app/backend/api/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/conftest.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1521 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/context_processors.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.918517 django-sso-app-0.9.6/src/django_sso_app/backend/fixtures/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/fixtures/.gitkeep
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.919518 django-sso-app-0.9.6/src/django_sso_app/backend/pages/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/pages/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      758 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/pages/admin.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.919518 django-sso-app-0.9.6/src/django_sso_app/backend/pages/migrations/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/pages/migrations/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.899518 django-sso-app-0.9.6/src/django_sso_app/backend/pages/templates/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.919518 django-sso-app-0.9.6/src/django_sso_app/backend/pages/templates/flatpages/
+-rw-rw-r--   0 user      (1000) user      (1000)      243 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/pages/templates/flatpages/default.html
+-rw-rw-r--   0 user      (1000) user      (1000)      297 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/pages/views.py
+-rw-r--r--   0 user      (1000) user      (1000)     3106 2021-02-10 11:06:45.000000 django-sso-app-0.9.6/src/django_sso_app/backend/settings.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.900518 django-sso-app-0.9.6/src/django_sso_app/backend/static/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.919518 django-sso-app-0.9.6/src/django_sso_app/backend/static/css/
+-rw-rw-r--   0 user      (1000) user      (1000)     1330 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/static/css/accounts.css
+-rw-rw-r--   0 user      (1000) user      (1000)       52 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/static/css/project.css
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.919518 django-sso-app-0.9.6/src/django_sso_app/backend/static/fonts/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/static/fonts/.gitkeep
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.900518 django-sso-app-0.9.6/src/django_sso_app/backend/static/images/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.919518 django-sso-app-0.9.6/src/django_sso_app/backend/static/images/favicons/
+-rw-rw-r--   0 user      (1000) user      (1000)     8348 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/static/images/favicons/favicon.ico
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.920518 django-sso-app-0.9.6/src/django_sso_app/backend/static/js/
+-rw-rw-r--   0 user      (1000) user      (1000)       46 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/static/js/accounts.js
+-rw-rw-r--   0 user      (1000) user      (1000)       45 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/static/js/project.js
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.920518 django-sso-app-0.9.6/src/django_sso_app/backend/static/sass/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/static/sass/custom_bootstrap_vars.scss
+-rw-rw-r--   0 user      (1000) user      (1000)      610 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/static/sass/project.scss
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.921517 django-sso-app-0.9.6/src/django_sso_app/backend/templates/
+-rw-rw-r--   0 user      (1000) user      (1000)      194 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/403.html
+-rw-rw-r--   0 user      (1000) user      (1000)      192 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/404.html
+-rw-rw-r--   0 user      (1000) user      (1000)      313 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/500.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.924517 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/
+-rw-rw-r--   0 user      (1000) user      (1000)      252 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/account_inactive.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1304 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/base.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.924517 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/email/
+-rw-rw-r--   0 user      (1000) user      (1000)    14036 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/email/base_email.html
+-rw-rw-r--   0 user      (1000) user      (1000)      602 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/email/email_confirmation_message.html
+-rw-rw-r--   0 user      (1000) user      (1000)       62 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/email/email_confirmation_signup_message.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1100 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/email/password_reset_key_message.html
+-rw-rw-r--   0 user      (1000) user      (1000)     2639 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/email.html
+-rw-rw-r--   0 user      (1000) user      (1000)      968 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/email_confirm.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1529 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/login.html
+-rw-rw-r--   0 user      (1000) user      (1000)      558 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/logout.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.925517 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/partials/
+-rw-rw-r--   0 user      (1000) user      (1000)      882 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/partials/mapbox_initscript.html
+-rw-rw-r--   0 user      (1000) user      (1000)      501 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/password_change.html
+-rw-rw-r--   0 user      (1000) user      (1000)      870 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/password_reset.html
+-rw-rw-r--   0 user      (1000) user      (1000)      484 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/password_reset_done.html
+-rw-rw-r--   0 user      (1000) user      (1000)      992 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/password_reset_from_key.html
+-rw-rw-r--   0 user      (1000) user      (1000)      261 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/password_reset_from_key_done.html
+-rw-rw-r--   0 user      (1000) user      (1000)      486 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/password_set.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1425 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/profile.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1604 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/profile_complete.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1602 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/profile_update.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1030 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/signup.html
+-rw-rw-r--   0 user      (1000) user      (1000)      274 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/signup_closed.html
+-rw-rw-r--   0 user      (1000) user      (1000)      447 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/verification_sent.html
+-rw-rw-r--   0 user      (1000) user      (1000)      807 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/verified_email_required.html
+-rw-rw-r--   0 user      (1000) user      (1000)     2534 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/base.html
+-rw-rw-r--   0 user      (1000) user      (1000)      833 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/cookie_consent.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.925517 django-sso-app-0.9.6/src/django_sso_app/backend/templates/flatpages/
+-rw-rw-r--   0 user      (1000) user      (1000)      226 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/flatpages/default.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.925517 django-sso-app-0.9.6/src/django_sso_app/backend/templates/pages/
+-rw-rw-r--   0 user      (1000) user      (1000)      296 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/pages/home.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.925517 django-sso-app-0.9.6/src/django_sso_app/backend/templates/partials/
+-rw-rw-r--   0 user      (1000) user      (1000)      355 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/partials/google_analytics_site_tag.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1328 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/partials/nav_footer.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1895 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/partials/nav_pills.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.926517 django-sso-app-0.9.6/src/django_sso_app/backend/templates/polyfills/
+-rw-rw-r--   0 user      (1000) user      (1000)      850 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/polyfills/console_polyfill.html
+-rw-rw-r--   0 user      (1000) user      (1000)      575 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/polyfills/custom_event_polyfill.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.926517 django-sso-app-0.9.6/src/django_sso_app/backend/templates/users/
+-rw-rw-r--   0 user      (1000) user      (1000)      763 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/users/user_detail.html
+-rw-rw-r--   0 user      (1000) user      (1000)      615 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/templates/users/user_form.html
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.926517 django-sso-app-0.9.6/src/django_sso_app/backend/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2184 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/urls.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.927518 django-sso-app-0.9.6/src/django_sso_app/backend/users/
+-rw-rw-r--   0 user      (1000) user      (1000)       68 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      192 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/admin.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.927518 django-sso-app-0.9.6/src/django_sso_app/backend/users/api/
+-rw-rw-r--   0 user      (1000) user      (1000)       69 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/api/serializers.py
+-rw-rw-r--   0 user      (1000) user      (1000)       99 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/api/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)      320 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/apps.py
+-rw-rw-r--   0 user      (1000) user      (1000)      298 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/forms.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.927518 django-sso-app-0.9.6/src/django_sso_app/backend/users/migrations/
+-rw-rw-r--   0 user      (1000) user      (1000)     4722 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/migrations/0001_initial.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/migrations/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      536 2021-02-03 16:34:19.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)      238 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/tasks.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.928517 django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      838 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/factories.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1143 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/test_forms.py
+-rw-rw-r--   0 user      (1000) user      (1000)      215 2021-02-03 16:34:19.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/test_models.py
+-rw-rw-r--   0 user      (1000) user      (1000)      523 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/test_tasks.py
+-rw-rw-r--   0 user      (1000) user      (1000)      672 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/test_urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1353 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/test_views.py
+-rw-rw-r--   0 user      (1000) user      (1000)      380 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1296 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/users/views.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.928517 django-sso-app-0.9.6/src/django_sso_app/backend/utils/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/utils/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      372 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backend/utils/context_processors.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1269 2021-02-22 16:45:30.000000 django-sso-app-0.9.6/src/django_sso_app/backend/views.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.928517 django-sso-app-0.9.6/src/django_sso_app/backups/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/backups/.gitkeep
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.929517 django-sso-app-0.9.6/src/django_sso_app/config/
+-rw-rw-r--   0 user      (1000) user      (1000)      178 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/config/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      593 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/config/celery_app.py
+-rw-rw-r--   0 user      (1000) user      (1000)       60 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/config/extra_urls.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.930517 django-sso-app-0.9.6/src/django_sso_app/config/settings/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/config/settings/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19094 2021-02-26 13:55:06.000000 django-sso-app-0.9.6/src/django_sso_app/config/settings/base.py
+-rw-rw-r--   0 user      (1000) user      (1000)       34 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/config/settings/extra.py
+-rw-rw-r--   0 user      (1000) user      (1000)      241 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/config/settings/languages.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3286 2021-02-05 09:02:12.000000 django-sso-app-0.9.6/src/django_sso_app/config/settings/local.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7711 2021-02-10 13:08:31.000000 django-sso-app-0.9.6/src/django_sso_app/config/settings/production.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1773 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/config/settings/test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4944 2021-02-22 16:47:00.000000 django-sso-app-0.9.6/src/django_sso_app/config/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1708 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/config/wsgi.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.931517 django-sso-app-0.9.6/src/django_sso_app/core/
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5433 2021-02-08 20:23:44.000000 django-sso-app-0.9.6/src/django_sso_app/core/adapter.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.932517 django-sso-app-0.9.6/src/django_sso_app/core/api/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/api/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      480 2021-02-08 07:11:37.000000 django-sso-app-0.9.6/src/django_sso_app/core/api/authentication.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5399 2021-02-08 11:49:53.000000 django-sso-app-0.9.6/src/django_sso_app/core/api/serializers.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.932517 django-sso-app-0.9.6/src/django_sso_app/core/api/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/api/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9876 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/api/tests/test_views.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1096 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/api/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)      450 2021-02-05 16:56:38.000000 django-sso-app-0.9.6/src/django_sso_app/core/api/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16944 2021-02-09 11:51:11.000000 django-sso-app-0.9.6/src/django_sso_app/core/api/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11543 2021-02-09 15:06:14.000000 django-sso-app-0.9.6/src/django_sso_app/core/app_settings.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.933517 django-sso-app-0.9.6/src/django_sso_app/core/apps/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.933517 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)       72 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/functions.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.933517 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/kong/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/kong/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      366 2021-02-22 14:36:11.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/kong/functions.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10305 2021-02-22 14:36:11.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/kong/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.934517 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/signals/
+-rw-rw-r--   0 user      (1000) user      (1000)      366 2020-12-14 18:02:06.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/signals/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/signals/app.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5931 2021-02-24 11:46:34.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/signals/backend.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.934517 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      350 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/tests/test_views.py
+-rw-rw-r--   0 user      (1000) user      (1000)       26 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.935517 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      312 2021-02-22 13:57:45.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/admin.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1668 2021-02-03 16:22:56.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)      633 2021-02-03 16:22:56.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/serializers.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.935517 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/signals/
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2020-12-14 18:02:06.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/signals/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/signals/app.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4391 2021-02-09 12:09:42.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/signals/backend.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.935517 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      159 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/tests/test_models.py
+-rw-rw-r--   0 user      (1000) user      (1000)      433 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4597 2021-02-10 10:48:09.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1084 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/views.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.936517 django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)       48 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)      269 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/serializers.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.936517 django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/signals/
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2020-12-14 18:02:06.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/signals/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/signals/app.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1244 2020-12-14 11:54:57.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/signals/backend.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.936517 django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1445 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/tests/test_models.py
+-rw-r--r--   0 user      (1000) user      (1000)      280 2021-02-08 14:20:10.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.937517 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      476 2021-02-03 16:23:55.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)      244 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/serializers.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.937517 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/signals/
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2020-12-14 18:02:06.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/signals/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2021-02-05 10:00:47.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/signals/app.py
+-rw-r--r--   0 user      (1000) user      (1000)     3103 2021-02-09 10:05:31.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/signals/backend.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.938517 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1580 2021-02-08 15:26:47.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/tests/test_models.py
+-rw-r--r--   0 user      (1000) user      (1000)     1470 2021-02-08 17:06:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/tests/test_views.py
+-rw-rw-r--   0 user      (1000) user      (1000)      398 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2815 2021-02-10 12:48:31.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)      709 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/views.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.939517 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      385 2021-02-22 15:24:07.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/admin.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1839 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/functions.py
+-rw-r--r--   0 user      (1000) user      (1000)     1689 2021-02-22 15:26:02.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)      417 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/signals.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.939517 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)       79 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/tests/test_models.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2947 2021-02-22 15:25:28.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/tests/test_views.py
+-rw-rw-r--   0 user      (1000) user      (1000)      335 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2252 2021-02-09 10:27:30.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5755 2021-02-22 15:25:28.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/views.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.940517 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/
+-rw-rw-r--   0 user      (1000) user      (1000)      115 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      317 2021-02-22 14:25:29.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/admin.py
+-rw-rw-r--   0 user      (1000) user      (1000)      354 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/filters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3926 2021-02-22 14:37:16.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/forms.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9587 2021-02-22 14:37:16.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5109 2021-02-22 14:37:16.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/serializers.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.941517 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/signals/
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2020-12-14 18:02:06.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/signals/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      967 2021-02-08 12:09:04.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/signals/app.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2685 2021-02-09 12:05:29.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/signals/backend.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.941517 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1704 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/tests/test_models.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7522 2021-02-09 12:02:56.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/tests/test_views.py
+-rw-rw-r--   0 user      (1000) user      (1000)      796 2021-02-09 12:03:15.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/urls.py
+-rw-r--r--   0 user      (1000) user      (1000)     6609 2021-02-10 13:15:06.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5669 2021-02-09 12:02:56.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/views.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.942517 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1785 2021-02-22 14:37:16.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/admin.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4774 2021-02-08 19:29:16.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3370 2021-02-03 16:22:56.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/serializers.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.942517 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/signals/
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2020-12-14 18:02:06.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/signals/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/signals/app.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2021-02-08 19:32:35.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/signals/backend.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.942517 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9310 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/tests/test_views.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1256 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1907 2021-02-09 12:02:56.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5431 2021-02-09 12:16:18.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/services/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)      121 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/settings.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.943517 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      216 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/admin.py
+-rw-rw-r--   0 user      (1000) user      (1000)      613 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/models.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.943517 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/signals/
+-rw-r--r--   0 user      (1000) user      (1000)      310 2021-02-09 09:59:08.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/signals/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      445 2021-02-09 10:01:20.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/signals/app.py
+-rw-rw-r--   0 user      (1000) user      (1000)      445 2021-02-09 10:01:20.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/signals/backend.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.944517 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13414 2021-02-10 13:21:04.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/tests/test_app.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4950 2021-02-04 14:26:10.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/tests/test_backend.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5593 2021-02-05 16:31:31.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/status/tests/test_views.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1749 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/tests.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.945517 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/
+-rw-rw-r--   0 user      (1000) user      (1000)      425 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1156 2021-02-22 14:32:12.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/admin.py
+-rw-rw-r--   0 user      (1000) user      (1000)      482 2020-12-03 12:01:22.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/filters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1384 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/forms.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5334 2021-02-22 14:36:11.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14153 2021-02-09 12:16:18.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/serializers.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.946517 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/signals/
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2020-12-14 18:02:06.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/signals/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/signals/app.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-12-14 12:46:06.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/signals/backend.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.946517 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      712 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/tests/test_models.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16218 2021-02-05 17:22:26.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/tests/test_views.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1076 2020-10-14 14:57:25.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8801 2021-02-10 11:34:17.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7352 2021-02-09 12:16:18.000000 django-sso-app-0.9.6/src/django_sso_app/core/apps/users/views.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.946517 django-sso-app-0.9.6/src/django_sso_app/core/authentication/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/authentication/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.947517 django-sso-app-0.9.6/src/django_sso_app/core/authentication/backends/
+-rw-rw-r--   0 user      (1000) user      (1000)     2368 2021-02-05 17:15:23.000000 django-sso-app-0.9.6/src/django_sso_app/core/authentication/backends/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6389 2021-02-10 13:11:14.000000 django-sso-app-0.9.6/src/django_sso_app/core/authentication/backends/app.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2392 2021-02-08 14:06:49.000000 django-sso-app-0.9.6/src/django_sso_app/core/authentication/backends/backend.py
+-rw-r--r--   0 user      (1000) user      (1000)      731 2021-02-08 20:14:47.000000 django-sso-app-0.9.6/src/django_sso_app/core/authentication/backends/login.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.947517 django-sso-app-0.9.6/src/django_sso_app/core/authentication/middleware/
+-rw-rw-r--   0 user      (1000) user      (1000)    10065 2021-02-10 12:16:18.000000 django-sso-app-0.9.6/src/django_sso_app/core/authentication/middleware/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2306 2021-02-10 12:21:39.000000 django-sso-app-0.9.6/src/django_sso_app/core/authentication/middleware/app.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1864 2021-02-08 14:06:49.000000 django-sso-app-0.9.6/src/django_sso_app/core/authentication/middleware/backend.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3408 2021-02-10 12:20:01.000000 django-sso-app-0.9.6/src/django_sso_app/core/authentication/middleware/base.py
+-rw-rw-r--   0 user      (1000) user      (1000)      835 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/context_processors.py
+-rw-rw-r--   0 user      (1000) user      (1000)      810 2021-02-08 20:04:37.000000 django-sso-app-0.9.6/src/django_sso_app/core/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5798 2021-02-22 14:36:11.000000 django-sso-app-0.9.6/src/django_sso_app/core/forms.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1386 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/functions.py
+-rw-rw-r--   0 user      (1000) user      (1000)      720 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/loader.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.948517 django-sso-app-0.9.6/src/django_sso_app/core/middleware/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/middleware/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      355 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/middleware/same_site.py
+-rw-rw-r--   0 user      (1000) user      (1000)      317 2021-02-04 19:39:14.000000 django-sso-app-0.9.6/src/django_sso_app/core/middleware/x_forwarded_for.py
+-rw-rw-r--   0 user      (1000) user      (1000)      795 2021-02-09 10:02:27.000000 django-sso-app-0.9.6/src/django_sso_app/core/mixins.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1516 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2760 2021-02-09 10:06:54.000000 django-sso-app-0.9.6/src/django_sso_app/core/permissions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1913 2021-02-03 16:28:13.000000 django-sso-app-0.9.6/src/django_sso_app/core/serializers.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.948517 django-sso-app-0.9.6/src/django_sso_app/core/settings/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/settings/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2038 2021-01-07 15:17:35.000000 django-sso-app-0.9.6/src/django_sso_app/core/settings/common.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.948517 django-sso-app-0.9.6/src/django_sso_app/core/solidity/
+-rw-rw-r--   0 user      (1000) user      (1000)    10363 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/solidity/DjangoSsoAppProfileContract.sol
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.948517 django-sso-app-0.9.6/src/django_sso_app/core/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11633 2021-02-08 14:51:04.000000 django-sso-app-0.9.6/src/django_sso_app/core/tests/factories.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10427 2021-02-08 16:58:44.000000 django-sso-app-0.9.6/src/django_sso_app/core/tests/test_views.py
+-rw-rw-r--   0 user      (1000) user      (1000)      127 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/to_translate.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.949517 django-sso-app-0.9.6/src/django_sso_app/core/tokens/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/tokens/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3332 2020-12-14 14:28:35.000000 django-sso-app-0.9.6/src/django_sso_app/core/tokens/authentication.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.949517 django-sso-app-0.9.6/src/django_sso_app/core/tokens/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/core/tokens/tests/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2387 2021-02-04 14:25:20.000000 django-sso-app-0.9.6/src/django_sso_app/core/tokens/tests/test_views.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4329 2021-02-08 15:14:13.000000 django-sso-app-0.9.6/src/django_sso_app/core/tokens/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3730 2020-12-14 14:26:09.000000 django-sso-app-0.9.6/src/django_sso_app/core/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5243 2021-02-22 16:45:27.000000 django-sso-app-0.9.6/src/django_sso_app/core/utils.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13509 2021-02-22 14:36:11.000000 django-sso-app-0.9.6/src/django_sso_app/core/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)   466944 2021-01-07 14:45:21.000000 django-sso-app-0.9.6/src/django_sso_app/db.sqlite3
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.949517 django-sso-app-0.9.6/src/django_sso_app/fixtures/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/fixtures/.gitkeep
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.949517 django-sso-app-0.9.6/src/django_sso_app/locale/
+-rw-rw-r--   0 user      (1000) user      (1000)      120 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/README.rst
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.904518 django-sso-app-0.9.6/src/django_sso_app/locale/de/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.949517 django-sso-app-0.9.6/src/django_sso_app/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 user      (1000) user      (1000)    24826 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 user      (1000) user      (1000)    27728 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.904518 django-sso-app-0.9.6/src/django_sso_app/locale/en/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.950517 django-sso-app-0.9.6/src/django_sso_app/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 user      (1000) user      (1000)    24826 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/en/LC_MESSAGES/django.po
+-rw-rw-r--   0 user      (1000) user      (1000)    27728 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.905518 django-sso-app-0.9.6/src/django_sso_app/locale/es/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.950517 django-sso-app-0.9.6/src/django_sso_app/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 user      (1000) user      (1000)    24826 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/es/LC_MESSAGES/django.po
+-rw-rw-r--   0 user      (1000) user      (1000)    27728 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.905518 django-sso-app-0.9.6/src/django_sso_app/locale/fr/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.950517 django-sso-app-0.9.6/src/django_sso_app/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 user      (1000) user      (1000)    24825 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 user      (1000) user      (1000)    27727 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.905518 django-sso-app-0.9.6/src/django_sso_app/locale/it/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.951517 django-sso-app-0.9.6/src/django_sso_app/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 user      (1000) user      (1000)    10733 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 user      (1000) user      (1000)    28829 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/it/LC_MESSAGES/django.po
+-rw-rw-r--   0 user      (1000) user      (1000)     8559 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/it/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 user      (1000) user      (1000)    30620 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/it/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.905518 django-sso-app-0.9.6/src/django_sso_app/locale/nl/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.952517 django-sso-app-0.9.6/src/django_sso_app/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 user      (1000) user      (1000)    24826 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/nl/LC_MESSAGES/django.po
+-rw-rw-r--   0 user      (1000) user      (1000)    27728 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/nl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.905518 django-sso-app-0.9.6/src/django_sso_app/locale/pt/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.952517 django-sso-app-0.9.6/src/django_sso_app/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 user      (1000) user      (1000)      421 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 user      (1000) user      (1000)    24826 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/pt/LC_MESSAGES/django.po
+-rw-rw-r--   0 user      (1000) user      (1000)      486 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/pt/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 user      (1000) user      (1000)    27927 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/locale/pt/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.953517 django-sso-app-0.9.6/src/django_sso_app/logs/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/logs/.gitkeep
+-rw-rw-r--   0 user      (1000) user      (1000)      852 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/manage.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.953517 django-sso-app-0.9.6/src/django_sso_app/management/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/management/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.954517 django-sso-app-0.9.6/src/django_sso_app/management/commands/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/management/commands/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1102 2021-02-09 12:25:19.000000 django-sso-app-0.9.6/src/django_sso_app/management/commands/clear_api_gateway_consumer_ids.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2126 2021-02-09 12:17:04.000000 django-sso-app-0.9.6/src/django_sso_app/management/commands/create_user_with_simple_profile.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1804 2021-02-09 12:17:04.000000 django-sso-app-0.9.6/src/django_sso_app/management/commands/delete_all_profiles_devices.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1971 2021-02-09 12:16:18.000000 django-sso-app-0.9.6/src/django_sso_app/management/commands/delete_all_users_devices_by_username.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1462 2021-02-09 12:11:42.000000 django-sso-app-0.9.6/src/django_sso_app/management/commands/restore_api_gateway_consumers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1730 2021-02-09 12:11:42.000000 django-sso-app-0.9.6/src/django_sso_app/management/commands/restore_api_gateway_consumers_by_username.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.955517 django-sso-app-0.9.6/src/django_sso_app/migrations/
+-rw-rw-r--   0 user      (1000) user      (1000)    10502 2020-12-14 13:46:34.000000 django-sso-app-0.9.6/src/django_sso_app/migrations/0001_initial.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1036 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/migrations/0002_auto_20200307_1035.py
+-rw-rw-r--   0 user      (1000) user      (1000)      569 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/migrations/0003_emailaddress.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1481 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/migrations/0004_django_user_fields_in_profile__20200417_1757.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1069 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/migrations/0005_auto_20200519_1725.py
+-rw-rw-r--   0 user      (1000) user      (1000)      309 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/migrations/0006_delete_emailaddress.py
+-rw-r--r--   0 user      (1000) user      (1000)      482 2021-02-22 15:26:55.000000 django-sso-app-0.9.6/src/django_sso_app/migrations/0007_auto_20210222_1526.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/migrations/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      300 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/models.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.955517 django-sso-app-0.9.6/src/django_sso_app/private/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/private/.gitkeep
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.955517 django-sso-app-0.9.6/src/django_sso_app/private/users/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/private/users/.gitkeep
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.906518 django-sso-app-0.9.6/src/django_sso_app/public/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.955517 django-sso-app-0.9.6/src/django_sso_app/public/media/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/public/media/.gitkeep
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.955517 django-sso-app-0.9.6/src/django_sso_app/public/static/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/public/static/.gitkeep
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.955517 django-sso-app-0.9.6/src/django_sso_app/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/scripts/compilemessages.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      311 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/scripts/makemessages.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      155 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/settings.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3643 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/skeleton.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1203 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/django_sso_app/urls.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2021-03-09 15:17:01.917518 django-sso-app-0.9.6/src/django_sso_app.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    10781 2021-03-09 15:17:01.000000 django-sso-app-0.9.6/src/django_sso_app.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)    18131 2021-03-09 15:17:01.000000 django-sso-app-0.9.6/src/django_sso_app.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2021-03-09 15:17:01.000000 django-sso-app-0.9.6/src/django_sso_app.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       64 2021-03-09 15:17:01.000000 django-sso-app-0.9.6/src/django_sso_app.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2021-03-09 15:17:01.000000 django-sso-app-0.9.6/src/django_sso_app.egg-info/not-zip-safe
+-rw-r--r--   0 user      (1000) user      (1000)      410 2021-03-09 15:17:01.000000 django-sso-app-0.9.6/src/django_sso_app.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       15 2021-03-09 15:17:01.000000 django-sso-app-0.9.6/src/django_sso_app.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      243 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/makemessages.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      853 2020-08-24 11:58:21.000000 django-sso-app-0.9.6/src/manage.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1810 2020-12-16 13:23:58.000000 django-sso-app-0.9.6/src/server.py
```

### Comparing `django-sso-app-0.9.4/.editorconfig` & `django-sso-app-0.9.6/.editorconfig`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/.envs/.local/.django` & `django-sso-app-0.9.6/.envs/.local/.django`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/.envs/.production/.django` & `django-sso-app-0.9.6/.envs/.production/.django`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/.gitignore` & `django-sso-app-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/LICENSE` & `django-sso-app-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/Makefile` & `django-sso-app-0.9.6/Makefile`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 DOCKER=docker
 DPATH=${CURDIR}
 IMAGE_NAME=django-sso-app
-VERSION=$(shell python setup.py --version | sed 's/\.post.*//' | sed 's/\+g.*//')
-VERSION=0.9.4
+#VERSION=$(shell python setup.py --version | sed 's/\.post.*//' | sed 's/\+g.*//')
+VERSION=0.9.6
 
 export DPATH
 .PHONY:	clean build publish build-docker push-docker
 
 clean:
 	rm -rf ./dist/*
 	rm -rf ./build/*
```

### Comparing `django-sso-app-0.9.4/PKG-INFO` & `django-sso-app-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-app
-Version: 0.9.4
+Version: 0.9.6
 Summary: User profile management app
 Home-page: https://bitbucket.org/pai/django-sso-app
 Author: pai
 Author-email: paiuolo@gmail.com
 License: mit
 Project-URL: Documentation, https://pyscaffold.org/
 Description: # django-sso-app
```

### Comparing `django-sso-app-0.9.4/README.md` & `django-sso-app-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/compose/local/django/Dockerfile` & `django-sso-app-0.9.6/compose/local/django/Dockerfile`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/compose/production/django/Dockerfile` & `django-sso-app-0.9.6/compose/production/django/Dockerfile`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/compose/production/django/entrypoint` & `django-sso-app-0.9.6/compose/production/django/entrypoint`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/compose/production/django/maintenance/backup` & `django-sso-app-0.9.6/compose/production/django/maintenance/backup`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/compose/production/django/maintenance/restore` & `django-sso-app-0.9.6/compose/production/django/maintenance/restore`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/compose/production/nginx/nginx.conf` & `django-sso-app-0.9.6/compose/production/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/compose/production/postgres/maintenance/backup` & `django-sso-app-0.9.6/compose/production/postgres/maintenance/backup`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/compose/production/postgres/maintenance/restore` & `django-sso-app-0.9.6/compose/production/postgres/maintenance/restore`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/compose/production/supervisor/supervisord.conf` & `django-sso-app-0.9.6/compose/production/supervisor/supervisord.conf`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/compose/production/traefik/traefik.yml` & `django-sso-app-0.9.6/compose/production/traefik/traefik.yml`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/docs/Makefile` & `django-sso-app-0.9.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/docs/conf.py` & `django-sso-app-0.9.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/docs/index.rst` & `django-sso-app-0.9.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/local.yml` & `django-sso-app-0.9.6/local.yml`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/production.yml` & `django-sso-app-0.9.6/production.yml`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/requirements/base.txt` & `django-sso-app-0.9.6/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/requirements/local.txt` & `django-sso-app-0.9.6/requirements/local.txt`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/setup.cfg` & `django-sso-app-0.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/setup.py` & `django-sso-app-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/README.rst` & `django-sso-app-0.9.6/src/django_sso_app/README.rst`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/app/urls.py` & `django-sso-app-0.9.6/src/django_sso_app/app/urls.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/apps.py` & `django-sso-app-0.9.6/src/django_sso_app/apps.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/api/views.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/api/views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/context_processors.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/pages/admin.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/pages/admin.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/settings.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/settings.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/static/css/accounts.css` & `django-sso-app-0.9.6/src/django_sso_app/backend/static/css/accounts.css`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/static/images/favicons/favicon.ico` & `django-sso-app-0.9.6/src/django_sso_app/backend/static/images/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/static/sass/project.scss` & `django-sso-app-0.9.6/src/django_sso_app/backend/static/sass/project.scss`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/base.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/base.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/email/base_email.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/email/base_email.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/email/email_confirmation_message.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/email/email_confirmation_message.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/email/password_reset_key_message.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/email/password_reset_key_message.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/email.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/email.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/email_confirm.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/login.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/login.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/logout.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/logout.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/partials/mapbox_initscript.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/partials/mapbox_initscript.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/password_reset.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/password_reset_from_key.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/profile.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/profile.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/profile_complete.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/profile_complete.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/profile_update.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/profile_update.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/signup.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/account/verified_email_required.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/base.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/cookie_consent.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/cookie_consent.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/partials/nav_footer.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/partials/nav_footer.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/partials/nav_pills.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/partials/nav_pills.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/polyfills/console_polyfill.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/polyfills/console_polyfill.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/polyfills/custom_event_polyfill.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/polyfills/custom_event_polyfill.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/users/user_detail.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/users/user_detail.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/templates/users/user_form.html` & `django-sso-app-0.9.6/src/django_sso_app/backend/templates/users/user_form.html`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/urls.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/urls.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/users/migrations/0001_initial.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/users/models.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/users/models.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/factories.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/test_forms.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/test_tasks.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/test_urls.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/users/tests/test_views.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/users/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/users/views.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/users/views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/backend/views.py` & `django-sso-app-0.9.6/src/django_sso_app/backend/views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/config/celery_app.py` & `django-sso-app-0.9.6/src/django_sso_app/config/celery_app.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/config/settings/base.py` & `django-sso-app-0.9.6/src/django_sso_app/config/settings/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,17 +335,14 @@
 ENABLE_HTTPS = env.bool("ENABLE_HTTPS", default=not DEBUG)
 ACCOUNT_DEFAULT_HTTP_PROTOCOL = env("ACCOUNT_DEFAULT_HTTP_PROTOCOL", default="https" if ENABLE_HTTPS else "http")
 
 # CSRF
 if DEBUG:
     CSRF_COOKIE_DOMAIN = None
     CSRF_TRUSTED_ORIGINS = ['*']
-#else:  # defaults to APP_DOMAIN
-#    CSRF_COOKIE_DOMAIN = COOKIE_DOMAIN
-#    CSRF_TRUSTED_ORIGINS = ['.{0}'.format(COOKIE_DOMAIN)]
 
 # cors
 if DEBUG:
     CORS_ALLOW_ALL_ORIGINS = True
     CORS_ALLOW_CREDENTIALS = True
 else:
     # https://github.com/ottoyiu/django-cors-headers
```

### Comparing `django-sso-app-0.9.4/src/django_sso_app/config/settings/local.py` & `django-sso-app-0.9.6/src/django_sso_app/config/settings/local.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/config/settings/production.py` & `django-sso-app-0.9.6/src/django_sso_app/config/settings/production.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/config/settings/test.py` & `django-sso-app-0.9.6/src/django_sso_app/config/settings/test.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/config/urls.py` & `django-sso-app-0.9.6/src/django_sso_app/config/urls.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/config/wsgi.py` & `django-sso-app-0.9.6/src/django_sso_app/config/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/adapter.py` & `django-sso-app-0.9.6/src/django_sso_app/core/adapter.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/api/serializers.py` & `django-sso-app-0.9.6/src/django_sso_app/core/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/api/tests/test_views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/api/urls.py` & `django-sso-app-0.9.6/src/django_sso_app/core/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/api/views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/api/views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/app_settings.py` & `django-sso-app-0.9.6/src/django_sso_app/core/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/kong/utils.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/kong/utils.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/api_gateway/signals/backend.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/api_gateway/signals/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,14 +118,16 @@
                 status_code, resp = create_apigw_consumer_acl(apigateway_consumer_id, group.name)
 
                 if status_code < 400:
                     logger.debug('api gateway acl group created {}, {}'.format(status_code, resp))
 
                     if not is_loaddata:  # or is_apigateway_update):
                         profile.update_rev(True)
+                elif status_code == 409:
+                    logger.debug('acl group "{} already created'.format(group.name))
                 else:
                     logger.exception('error ({}) creating api gateway acl group'.format(status_code))
 
         elif action == 'pre_remove':
             for pk in pk_set:
                 group = Group.objects.get(id=pk)
                 logger.info('deleting apigw acl group "{}" for "{}"'.format(group, profile))
@@ -134,9 +136,11 @@
                 status_code, resp = delete_apigw_consumer_acl(apigateway_consumer_id, group.name)
 
                 if status_code < 400:
                     logger.debug('"{}" DELETED, updating profile sso_rev'.format(group))
 
                     if not is_loaddata:
                         profile.update_rev(True)
+                elif status_code == 404:
+                    logger.debug('acl group "{} already deleted'.format(group.name))
                 else:
                     logger.exception('error ({}) deleting api gateway acl group'.format(status_code))
```

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/models.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/models.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/serializers.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/signals/backend.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/signals/backend.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/utils.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/utils.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/devices/views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/devices/views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/signals/backend.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/signals/backend.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/emails/tests/test_models.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/emails/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/signals/backend.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/signals/backend.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/tests/test_models.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/tests/test_views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/utils.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/utils.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/groups/views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/groups/views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/functions.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/functions.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/models.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/models.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/tests/test_views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/utils.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/utils.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/passepartout/views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/passepartout/views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/forms.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/forms.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/models.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/models.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/serializers.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/signals/app.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/signals/app.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/signals/backend.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/signals/backend.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/tests/test_models.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/tests/test_views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/urls.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/urls.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/utils.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/utils.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/profiles/views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/profiles/views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/services/admin.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/services/admin.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/services/models.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/services/models.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/services/serializers.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/services/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/services/tests/test_views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/services/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/services/urls.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/services/urls.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/services/utils.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/services/utils.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/services/views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/services/views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/status/models.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/status/models.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/status/tests/test_app.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/status/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/status/tests/test_backend.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/status/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/status/tests/test_views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/status/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/tests.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/tests.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/users/admin.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/users/admin.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/users/forms.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/users/forms.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/users/models.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/users/models.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/users/serializers.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/users/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/users/tests/test_models.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/users/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/users/tests/test_views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/users/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/users/urls.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/users/urls.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/users/utils.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/users/utils.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/apps/users/views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/apps/users/views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/authentication/backends/__init__.py` & `django-sso-app-0.9.6/src/django_sso_app/core/authentication/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/authentication/backends/app.py` & `django-sso-app-0.9.6/src/django_sso_app/core/authentication/backends/app.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/authentication/backends/backend.py` & `django-sso-app-0.9.6/src/django_sso_app/core/authentication/backends/backend.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/authentication/backends/login.py` & `django-sso-app-0.9.6/src/django_sso_app/core/authentication/backends/login.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/authentication/middleware/__init__.py` & `django-sso-app-0.9.6/src/django_sso_app/core/authentication/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/authentication/middleware/app.py` & `django-sso-app-0.9.6/src/django_sso_app/core/authentication/middleware/app.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/authentication/middleware/backend.py` & `django-sso-app-0.9.6/src/django_sso_app/core/authentication/middleware/backend.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/authentication/middleware/base.py` & `django-sso-app-0.9.6/src/django_sso_app/core/authentication/middleware/base.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/context_processors.py` & `django-sso-app-0.9.6/src/django_sso_app/core/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/exceptions.py` & `django-sso-app-0.9.6/src/django_sso_app/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/forms.py` & `django-sso-app-0.9.6/src/django_sso_app/core/forms.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/functions.py` & `django-sso-app-0.9.6/src/django_sso_app/core/functions.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/loader.py` & `django-sso-app-0.9.6/src/django_sso_app/core/loader.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/mixins.py` & `django-sso-app-0.9.6/src/django_sso_app/core/mixins.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/models.py` & `django-sso-app-0.9.6/src/django_sso_app/core/models.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/permissions.py` & `django-sso-app-0.9.6/src/django_sso_app/core/permissions.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/serializers.py` & `django-sso-app-0.9.6/src/django_sso_app/core/serializers.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/settings/common.py` & `django-sso-app-0.9.6/src/django_sso_app/core/settings/common.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/solidity/DjangoSsoAppProfileContract.sol` & `django-sso-app-0.9.6/src/django_sso_app/core/solidity/DjangoSsoAppProfileContract.sol`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/tests/factories.py` & `django-sso-app-0.9.6/src/django_sso_app/core/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/tests/test_views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/tokens/authentication.py` & `django-sso-app-0.9.6/src/django_sso_app/core/tokens/authentication.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/tokens/tests/test_views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/tokens/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/tokens/utils.py` & `django-sso-app-0.9.6/src/django_sso_app/core/tokens/utils.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/urls.py` & `django-sso-app-0.9.6/src/django_sso_app/core/urls.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/utils.py` & `django-sso-app-0.9.6/src/django_sso_app/core/utils.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/core/views.py` & `django-sso-app-0.9.6/src/django_sso_app/core/views.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/db.sqlite3` & `django-sso-app-0.9.6/src/django_sso_app/db.sqlite3`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/de/LC_MESSAGES/django.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/de/LC_MESSAGES/djangojs.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/en/LC_MESSAGES/django.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/en/LC_MESSAGES/djangojs.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/es/LC_MESSAGES/django.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/es/LC_MESSAGES/djangojs.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/fr/LC_MESSAGES/django.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/fr/LC_MESSAGES/djangojs.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/it/LC_MESSAGES/django.mo` & `django-sso-app-0.9.6/src/django_sso_app/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/it/LC_MESSAGES/django.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/it/LC_MESSAGES/djangojs.mo` & `django-sso-app-0.9.6/src/django_sso_app/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/it/LC_MESSAGES/djangojs.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/nl/LC_MESSAGES/django.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/nl/LC_MESSAGES/djangojs.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/pt/LC_MESSAGES/django.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/locale/pt/LC_MESSAGES/djangojs.po` & `django-sso-app-0.9.6/src/django_sso_app/locale/pt/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/manage.py` & `django-sso-app-0.9.6/src/django_sso_app/manage.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/management/commands/clear_api_gateway_consumer_ids.py` & `django-sso-app-0.9.6/src/django_sso_app/management/commands/clear_api_gateway_consumer_ids.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/management/commands/create_user_with_simple_profile.py` & `django-sso-app-0.9.6/src/django_sso_app/management/commands/create_user_with_simple_profile.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/management/commands/delete_all_profiles_devices.py` & `django-sso-app-0.9.6/src/django_sso_app/management/commands/delete_all_profiles_devices.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/management/commands/delete_all_users_devices_by_username.py` & `django-sso-app-0.9.6/src/django_sso_app/management/commands/delete_all_users_devices_by_username.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/management/commands/restore_api_gateway_consumers.py` & `django-sso-app-0.9.6/src/django_sso_app/management/commands/restore_api_gateway_consumers.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/management/commands/restore_api_gateway_consumers_by_username.py` & `django-sso-app-0.9.6/src/django_sso_app/management/commands/restore_api_gateway_consumers_by_username.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/migrations/0001_initial.py` & `django-sso-app-0.9.6/src/django_sso_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/migrations/0002_auto_20200307_1035.py` & `django-sso-app-0.9.6/src/django_sso_app/migrations/0002_auto_20200307_1035.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/migrations/0003_emailaddress.py` & `django-sso-app-0.9.6/src/django_sso_app/migrations/0003_emailaddress.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/migrations/0004_django_user_fields_in_profile__20200417_1757.py` & `django-sso-app-0.9.6/src/django_sso_app/migrations/0004_django_user_fields_in_profile__20200417_1757.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/migrations/0005_auto_20200519_1725.py` & `django-sso-app-0.9.6/src/django_sso_app/migrations/0005_auto_20200519_1725.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/skeleton.py` & `django-sso-app-0.9.6/src/django_sso_app/skeleton.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app/urls.py` & `django-sso-app-0.9.6/src/django_sso_app/urls.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/django_sso_app.egg-info/PKG-INFO` & `django-sso-app-0.9.6/src/django_sso_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-app
-Version: 0.9.4
+Version: 0.9.6
 Summary: User profile management app
 Home-page: https://bitbucket.org/pai/django-sso-app
 Author: pai
 Author-email: paiuolo@gmail.com
 License: mit
 Project-URL: Documentation, https://pyscaffold.org/
 Description: # django-sso-app
```

### Comparing `django-sso-app-0.9.4/src/django_sso_app.egg-info/SOURCES.txt` & `django-sso-app-0.9.6/src/django_sso_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/manage.py` & `django-sso-app-0.9.6/src/manage.py`

 * *Files identical despite different names*

### Comparing `django-sso-app-0.9.4/src/server.py` & `django-sso-app-0.9.6/src/server.py`

 * *Files identical despite different names*

