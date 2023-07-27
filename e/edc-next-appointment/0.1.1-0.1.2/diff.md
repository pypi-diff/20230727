# Comparing `tmp/edc-next-appointment-0.1.1.tar.gz` & `tmp/edc-next-appointment-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-next-appointment-0.1.1.tar", last modified: Thu Jul 27 01:53:10 2023, max compression
+gzip compressed data, was "edc-next-appointment-0.1.2.tar", last modified: Thu Jul 27 12:18:35 2023, max compression
```

## Comparing `edc-next-appointment-0.1.1.tar` & `edc-next-appointment-0.1.2.tar`

### file list

```diff
@@ -1,60 +1,59 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 01:53:10.490350 edc-next-appointment-0.1.1/
--rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 01:53:10.481877 edc-next-appointment-0.1.1/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 01:53:10.485640 edc-next-appointment-0.1.1/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     3090 2023-07-27 01:53:02.000000 edc-next-appointment-0.1.1/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       23 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2023-07-24 19:09:02.000000 edc-next-appointment-0.1.1/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      126 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2531 2023-07-27 01:53:10.490460 edc-next-appointment-0.1.1/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1600 2023-07-27 01:53:02.000000 edc-next-appointment-0.1.1/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 01:53:10.487068 edc-next-appointment-0.1.1/edc_next_appointment/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      250 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      184 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/choices.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 01:53:10.488251 edc-next-appointment-0.1.1/edc_next_appointment/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      143 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1578 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/form_validators/form_validator_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      309 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/form_validators/next_appointment_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1928 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/form_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)      550 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 01:53:10.488536 edc-next-appointment-0.1.1/edc_next_appointment/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     2898 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1789 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/model_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1771 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/modeladmin_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4541 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/modelform_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 01:53:10.488779 edc-next-appointment-0.1.1/edc_next_appointment/models/
--rw-r--r--   0 erikvw     (501) staff       (20)       37 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      224 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/models/list_models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 01:53:10.488913 edc-next-appointment-0.1.1/edc_next_appointment/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 01:53:10.490123 edc-next-appointment-0.1.1/edc_next_appointment/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      127 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/tests/etc/django_crypto_fields
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 01:53:10.490261 edc-next-appointment-0.1.1/edc_next_appointment/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      214 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      760 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/edc_next_appointment/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 01:53:10.487807 edc-next-appointment-0.1.1/edc_next_appointment.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2531 2023-07-27 01:53:10.000000 edc-next-appointment-0.1.1/edc_next_appointment.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1706 2023-07-27 01:53:10.000000 edc-next-appointment-0.1.1/edc_next_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-27 01:53:10.000000 edc-next-appointment-0.1.1/edc_next_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-25 13:58:46.000000 edc-next-appointment-0.1.1/edc_next_appointment.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2023-07-27 01:53:10.000000 edc-next-appointment-0.1.1/edc_next_appointment.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1786 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1860 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.1/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1238 2023-07-27 01:53:10.490811 edc-next-appointment-0.1.1/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.162643 edc-next-appointment-0.1.2/
+-rw-r--r--   0 erikvw     (501) staff       (20)      253 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.154609 edc-next-appointment-0.1.2/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.157835 edc-next-appointment-0.1.2/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     3121 2023-07-27 12:18:27.000000 edc-next-appointment-0.1.2/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       23 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2023-07-24 19:09:02.000000 edc-next-appointment-0.1.2/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      126 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2531 2023-07-27 12:18:35.162732 edc-next-appointment-0.1.2/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1600 2023-07-27 01:53:02.000000 edc-next-appointment-0.1.2/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.159547 edc-next-appointment-0.1.2/edc_next_appointment/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      250 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      184 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/choices.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.160722 edc-next-appointment-0.1.2/edc_next_appointment/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      143 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1578 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/form_validators/form_validator_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      309 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/form_validators/next_appointment_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1928 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/form_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      550 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.160993 edc-next-appointment-0.1.2/edc_next_appointment/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2898 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1789 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/model_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1771 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/modeladmin_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4541 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/modelform_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.161235 edc-next-appointment-0.1.2/edc_next_appointment/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)       37 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      224 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/models/list_models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.161378 edc-next-appointment-0.1.2/edc_next_appointment/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.162425 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.162553 edc-next-appointment-0.1.2/edc_next_appointment/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      214 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      760 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/edc_next_appointment/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-27 12:18:35.160301 edc-next-appointment-0.1.2/edc_next_appointment.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2531 2023-07-27 12:18:35.000000 edc-next-appointment-0.1.2/edc_next_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1654 2023-07-27 12:18:35.000000 edc-next-appointment-0.1.2/edc_next_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-27 12:18:35.000000 edc-next-appointment-0.1.2/edc_next_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-25 13:58:46.000000 edc-next-appointment-0.1.2/edc_next_appointment.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2023-07-27 12:18:35.000000 edc-next-appointment-0.1.2/edc_next_appointment.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1786 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1860 2023-07-27 01:48:13.000000 edc-next-appointment-0.1.2/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1238 2023-07-27 12:18:35.163022 edc-next-appointment-0.1.2/setup.cfg
```

### Comparing `edc-next-appointment-0.1.1/.github/workflows/build.yml` & `edc-next-appointment-0.1.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/.gitignore` & `edc-next-appointment-0.1.2/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 _version.py
+django_crypto_fields
+.env
+.etc
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `edc-next-appointment-0.1.1/.pre-commit-config.yaml` & `edc-next-appointment-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/LICENSE` & `edc-next-appointment-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/PKG-INFO` & `edc-next-appointment-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-next-appointment
-Version: 0.1.1
+Version: 0.1.2
 Summary: Base classes for managing next appointment CRF at each timepoint in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-next-appointment
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc appointment,scheduling,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-next-appointment-0.1.1/README.rst` & `edc-next-appointment-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/edc_next_appointment/form_validators/form_validator_mixins.py` & `edc-next-appointment-0.1.2/edc_next_appointment/form_validators/form_validator_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/edc_next_appointment/form_validators.py` & `edc-next-appointment-0.1.2/edc_next_appointment/form_validators.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/edc_next_appointment/list_data.py` & `edc-next-appointment-0.1.2/edc_next_appointment/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/edc_next_appointment/migrations/0001_initial.py` & `edc-next-appointment-0.1.2/edc_next_appointment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/edc_next_appointment/model_mixins.py` & `edc-next-appointment-0.1.2/edc_next_appointment/model_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/edc_next_appointment/modeladmin_mixins.py` & `edc-next-appointment-0.1.2/edc_next_appointment/modeladmin_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/edc_next_appointment/modelform_mixins.py` & `edc-next-appointment-0.1.2/edc_next_appointment/modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/edc_next_appointment/tests/etc/user-rsa-local-private.pem` & `edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem` & `edc-next-appointment-0.1.2/edc_next_appointment/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/edc_next_appointment/utils.py` & `edc-next-appointment-0.1.2/edc_next_appointment/utils.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/edc_next_appointment.egg-info/PKG-INFO` & `edc-next-appointment-0.1.2/edc_next_appointment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-next-appointment
-Version: 0.1.1
+Version: 0.1.2
 Summary: Base classes for managing next appointment CRF at each timepoint in clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-next-appointment
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc appointment,scheduling,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-next-appointment-0.1.1/edc_next_appointment.egg-info/SOURCES.txt` & `edc-next-appointment-0.1.2/edc_next_appointment.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 edc_next_appointment/form_validators/form_validator_mixins.py
 edc_next_appointment/form_validators/next_appointment_form_validator.py
 edc_next_appointment/migrations/0001_initial.py
 edc_next_appointment/migrations/__init__.py
 edc_next_appointment/models/__init__.py
 edc_next_appointment/models/list_models.py
 edc_next_appointment/tests/__init__.py
-edc_next_appointment/tests/etc/django_crypto_fields
 edc_next_appointment/tests/etc/user-aes-local.key
 edc_next_appointment/tests/etc/user-aes-restricted.key
 edc_next_appointment/tests/etc/user-rsa-local-private.pem
 edc_next_appointment/tests/etc/user-rsa-local-public.pem
 edc_next_appointment/tests/etc/user-rsa-restricted-private.pem
 edc_next_appointment/tests/etc/user-rsa-restricted-public.pem
 edc_next_appointment/tests/etc/user-salt-local.key
```

### Comparing `edc-next-appointment-0.1.1/pyproject.toml` & `edc-next-appointment-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/runtests.py` & `edc-next-appointment-0.1.2/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-next-appointment-0.1.1/setup.cfg` & `edc-next-appointment-0.1.2/setup.cfg`

 * *Files identical despite different names*

