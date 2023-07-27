# Comparing `tmp/pretix-mollie-1.6.0.tar.gz` & `tmp/pretix-mollie-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-mollie-1.6.0.tar", last modified: Tue Jun 27 12:58:20 2023, max compression
+gzip compressed data, was "pretix-mollie-1.6.1.tar", last modified: Thu Jul 27 12:52:53 2023, max compression
```

## Comparing `pretix-mollie-1.6.0.tar` & `pretix-mollie-1.6.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.494539 pretix-mollie-1.6.0/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1955 2023-06-27 12:58:20.494539 pretix-mollie-1.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      770 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/ca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/ca/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    12020 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15938 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15783 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    10733 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/el/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/el/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10708 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/fi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11506 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11325 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/lv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/lv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11735 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/nl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15802 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.462538 pretix-mollie-1.6.0/pretix_mollie/locale/nl_BE/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/nl_BE/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10711 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/nl_BE/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.478538 pretix-mollie-1.6.0/pretix_mollie/locale/nl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/nl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15845 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/nl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.478538 pretix-mollie-1.6.0/pretix_mollie/locale/pl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10969 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.478538 pretix-mollie-1.6.0/pretix_mollie/locale/pl_Informal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/pl_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10717 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/pl_Informal/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.478538 pretix-mollie-1.6.0/pretix_mollie/locale/pt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11325 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10708 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/locale/si/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/si/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11548 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/locale/sl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/sl/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10708 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/locale/sv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/sv/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10879 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11446 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)    27447 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     3365 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.490539 pretix-mollie-1.6.0/pretix_mollie/static/pretix_mollie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/static/pretix_mollie/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/static/pretix_mollie/logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.482539 pretix-mollie-1.6.0/pretix_mollie/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.494539 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/checkout_payment_form_banktransfer.html
--rw-rw-rw-   0 root         (0) root         (0)     2220 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/control.html
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/order_pending.txt
--rw-rw-rw-   0 root         (0) root         (0)     4832 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/pending.html
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/redirect.html
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2002 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14737 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pretix_mollie/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 12:58:20.486539 pretix-mollie-1.6.0/pretix_mollie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1955 2023-06-27 12:58:20.000000 pretix-mollie-1.6.0/pretix_mollie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1934 2023-06-27 12:58:20.000000 pretix-mollie-1.6.0/pretix_mollie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 12:58:20.000000 pretix-mollie-1.6.0/pretix_mollie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-27 12:58:20.000000 pretix-mollie-1.6.0/pretix_mollie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-27 12:58:20.000000 pretix-mollie-1.6.0/pretix_mollie.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-27 12:58:20.494539 pretix-mollie-1.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-27 12:57:54.000000 pretix-mollie-1.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/ca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie/locale/ca/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    12020 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15938 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15783 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    10733 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/el/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie/locale/el/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10708 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/fi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11506 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11325 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/lv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie/locale/lv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11735 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/nl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15802 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/nl_BE/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/locale/nl_BE/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10711 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/nl_BE/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/nl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/locale/nl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15845 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/nl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/pl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10969 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/pl_Informal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/locale/pl_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10717 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/pl_Informal/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/pt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11325 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10708 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/si/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/locale/si/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/sl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/locale/sl/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10708 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/sv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/locale/sv/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10879 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.201289 pretix-mollie-1.6.1/pretix_mollie/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    11446 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)    27719 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2670 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/static/pretix_mollie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/static/pretix_mollie/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/static/pretix_mollie/logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/pretix_mollie/templates/pretix_mollie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/templates/pretix_mollie/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/templates/pretix_mollie/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/templates/pretix_mollie/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/templates/pretix_mollie/checkout_payment_form_banktransfer.html
+-rw-rw-rw-   0 root         (0) root         (0)     2220 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/templates/pretix_mollie/control.html
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/templates/pretix_mollie/order_pending.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4832 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/templates/pretix_mollie/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/templates/pretix_mollie/redirect.html
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14793 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pretix_mollie/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:53.205289 pretix-mollie-1.6.1/pretix_mollie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-07-27 12:52:53.000000 pretix-mollie-1.6.1/pretix_mollie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-07-27 12:52:53.000000 pretix-mollie-1.6.1/pretix_mollie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 12:52:53.000000 pretix-mollie-1.6.1/pretix_mollie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-27 12:52:53.000000 pretix-mollie-1.6.1/pretix_mollie.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-27 12:52:53.000000 pretix-mollie-1.6.1/pretix_mollie.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-27 12:52:53.209289 pretix-mollie-1.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-27 12:52:28.000000 pretix-mollie-1.6.1/setup.py
```

### Comparing `pretix-mollie-1.6.0/LICENSE` & `pretix-mollie-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/PKG-INFO` & `pretix-mollie-1.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mollie
-Version: 1.6.0
+Version: 1.6.1
 Summary: Integration for the Mollie payment provider.
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: Copyright 2018 Raphael Michel
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `pretix-mollie-1.6.0/README.rst` & `pretix-mollie-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/apps.py` & `pretix-mollie-1.6.1/pretix_mollie/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/forms.py` & `pretix-mollie-1.6.1/pretix_mollie/forms.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/ca/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/de/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/django.pot` & `pretix-mollie-1.6.1/pretix_mollie/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/el/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/fi/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/ja/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/lv/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/nl/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/nl_BE/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/nl_BE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/nl_Informal/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/nl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/pl/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/pl_Informal/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/pl_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/pt/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/ru/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/si/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/sl/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/sv/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/locale/zh_Hans/LC_MESSAGES/django.po` & `pretix-mollie-1.6.1/pretix_mollie/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/payment.py` & `pretix-mollie-1.6.1/pretix_mollie/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,14 +405,15 @@
                 'currency': self.event.currency,
                 'value': str(refund.amount)
             },
         }
         if self.settings.connect_client_id and self.settings.access_token:
             body['testmode'] = refund.payment.info_data.get('mode', 'live') == 'test'
         try:
+            refresh_mollie_token(self.event, True)
             req = requests.post(
                 'https://api.mollie.com/v2/payments/{}/refunds'.format(payment),
                 json=body,
                 headers=self.request_headers
             )
             req.raise_for_status()
             refund.info_data = req.json()
@@ -501,14 +502,15 @@
                 if request:
                     return self.redirect(request, payment.info_data.get('_links').get('checkout').get('href'))
                 else:
                     return
         except:
             pass
         try:
+            refresh_mollie_token(self.event, True)
             req = requests.post(
                 'https://api.mollie.com/v2/payments',
                 json=self._get_payment_body(payment),
                 headers=self.request_headers
             )
             req.raise_for_status()
         except HTTPError:
@@ -585,20 +587,27 @@
     verbose_name = _('Bank transfer via Mollie')
     public_name = _('Bank transfer')
 
     @property
     def requires_invoice_immediately(self):
         return self.settings.get('method_banktransfer_invoice_immediately', False, as_type=bool)
 
-    @transaction.atomic()
     def execute_payment(self, request: HttpRequest, payment: OrderPayment, retry=True):
-        p_orig = payment
-        if retry:
-            payment = OrderPayment.objects.select_for_update(of=OF_SELF).get(pk=payment.pk)
-        super().execute_payment(request, payment, retry)
+        err = None
+        with transaction.atomic():
+            p_orig = payment
+            if retry:
+                payment = OrderPayment.objects.select_for_update(of=OF_SELF).get(pk=payment.pk)
+            try:
+                super().execute_payment(request, payment, retry)
+            except PaymentException as e:
+                err = e
+        if err:
+            raise err
+
         p_orig.refresh_from_db()
         return  # no redirect necessary for this method
 
     def _get_payment_body(self, payment):
         body = super()._get_payment_body(payment)
         body['dueDate'] = (payment.order.expires.date() + timedelta(days=1)).isoformat()
         return body
```

### Comparing `pretix-mollie-1.6.0/pretix_mollie/signals.py` & `pretix-mollie-1.6.1/pretix_mollie/signals.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 import logging
-import time
 from collections import OrderedDict
 
-import requests
 from django import forms
 from django.dispatch import receiver
 from django.utils.translation import gettext_lazy as _
-from django_scopes import scopes_disabled
 
 from pretix.base.forms import SecretKeySettingsField
-from pretix.base.models import Event_SettingsStore
-from pretix.base.settings import GlobalSettingsObject, settings_hierarkey
+from pretix.base.settings import settings_hierarkey
 from pretix.base.signals import (
-    logentry_display, periodic_task, register_global_settings,
-    register_payment_providers,
+    logentry_display, register_global_settings, register_payment_providers,
 )
-from pretix.helpers.urls import build_absolute_uri
 
 from .forms import MollieKeyValidator
-from .utils import refresh_mollie_token
 
 logger = logging.getLogger(__name__)
 
 
 @receiver(register_payment_providers, dispatch_uid="payment_mollie")
 def register_payment_provider(sender, **kwargs):
     from .payment import (
@@ -60,15 +53,15 @@
 
     plains = {
         'canceled': _('Payment canceled.'),
         'failed': _('Payment failed.'),
         'paid': _('Payment succeeded.'),
         'expired': _('Payment expired.'),
         'disabled': _('Payment method disabled since we were unable to refresh the access token. Please '
-                      'contact support.'),
+                      'contact support.'),  # for historical reasons, no longer occurs
     }
     text = plains.get(logentry.action_type[20:], None)
     if text:
         return _('Mollie reported an event: {}').format(text)
 
 
 settings_hierarkey.add_default('payment_mollie_method_cc', True, bool)
@@ -85,19 +78,7 @@
             ),
         )),
         ('payment_mollie_connect_client_secret', SecretKeySettingsField(
             label=_('Mollie Connect: Client secret'),
             required=False,
         )),
     ])
-
-
-@receiver(periodic_task, dispatch_uid='mollie_refresh_tokens')
-@scopes_disabled()
-def refresh_mollie_tokens(sender, **kwargs):
-    seen = set()
-    for es in Event_SettingsStore.objects.filter(key='payment_mollie_expires'):
-        if float(es.object.settings.payment_mollie_expires) - time.time() < 600:
-            rt = es.object.settings.payment_mollie_refresh_token
-            if rt not in seen:
-                refresh_mollie_token(es.object, True)
-                seen.add(rt)
```

### Comparing `pretix-mollie-1.6.0/pretix_mollie/static/pretix_mollie/logo.svg` & `pretix-mollie-1.6.1/pretix_mollie/static/pretix_mollie/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/control.html` & `pretix-mollie-1.6.1/pretix_mollie/templates/pretix_mollie/control.html`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/pending.html` & `pretix-mollie-1.6.1/pretix_mollie/templates/pretix_mollie/pending.html`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/templates/pretix_mollie/redirect.html` & `pretix-mollie-1.6.1/pretix_mollie/templates/pretix_mollie/redirect.html`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/urls.py` & `pretix-mollie-1.6.1/pretix_mollie/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pretix_mollie/utils.py` & `pretix-mollie-1.6.1/pretix_mollie/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 import hashlib
 import logging
 import time
 
 import requests
-from django.core.cache import cache
 
 from pretix.base.models import Event_SettingsStore
 from pretix.base.settings import GlobalSettingsObject
 from pretix.helpers.urls import build_absolute_uri
 
 logger = logging.getLogger(__name__)
 
 
-def refresh_mollie_token(event, disable=True):
-    # Rate limit
+def refresh_mollie_token(event, conditional=False):
     rt = event.settings.payment_mollie_refresh_token
     if not rt:
         return False
-    h = hashlib.sha1(rt.encode()).hexdigest()
-    if cache.get('mollie_refresh_{}'.format(h)):
-        return False
-    cache.set('mollie_refresh_{}'.format(h), 'started', 30)
+
+    if conditional:
+        # Only execute if refresh is near
+        if event.settings.payment_mollie_expires and float(event.settings.payment_mollie_expires) - time.time() > 60:
+            return False  # no refresh necessary
 
     gs = GlobalSettingsObject()
     try:
         resp = requests.post('https://api.mollie.com/oauth2/tokens', auth=(
             gs.settings.payment_mollie_connect_client_id,
             gs.settings.payment_mollie_connect_client_secret
         ), data={
             'grant_type': 'refresh_token',
             'refresh_token': event.settings.payment_mollie_refresh_token,
             'redirect_uri': build_absolute_uri('plugins:pretix_mollie:oauth.return')
         })
     except Exception as e:
         logger.exception('Unable to refresh mollie token')
-        if float(event.settings.payment_mollie_expires) > time.time() and not \
-                event.settings.payment_mollie_api_key and disable:
-            event.settings.payment_mollie__enabled = False
-            event.log_action('pretix_mollie.event.disabled', {
-                'reason': str(e)
-            })
         return False
     else:
         if resp.status_code == 200:
             data = resp.json()
             for ev in Event_SettingsStore.objects.filter(key='payment_mollie_refresh_token', value=rt):
                 ev.object.settings.payment_mollie_access_token = data['access_token']
                 ev.object.settings.payment_mollie_refresh_token = data['refresh_token']
                 ev.object.settings.payment_mollie_expires = time.time() + data['expires_in']
+            event.settings.flush()
             return True
     return False
```

### Comparing `pretix-mollie-1.6.0/pretix_mollie/views.py` & `pretix-mollie-1.6.1/pretix_mollie/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,14 +147,15 @@
     if pprov.settings.connect_client_id and payment.info_data and payment.info_data.get('mode', 'live') == 'test':
         qp = 'testmode=true'
     elif pprov.settings.connect_client_id and pprov.settings.access_token and pprov.settings.endpoint == "test":
         qp = 'testmode=true'
     else:
         qp = ''
     try:
+        refresh_mollie_token(payment.order.event, True)
         resp = requests.get(
             'https://api.mollie.com/v2/payments/' + mollie_id + '?' + qp,
             headers=pprov.request_headers
         )
         resp.raise_for_status()
         data = resp.json()
```

### Comparing `pretix-mollie-1.6.0/pretix_mollie.egg-info/PKG-INFO` & `pretix-mollie-1.6.1/pretix_mollie.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mollie
-Version: 1.6.0
+Version: 1.6.1
 Summary: Integration for the Mollie payment provider.
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: Copyright 2018 Raphael Michel
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

### Comparing `pretix-mollie-1.6.0/pretix_mollie.egg-info/SOURCES.txt` & `pretix-mollie-1.6.1/pretix_mollie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-mollie-1.6.0/pyproject.toml` & `pretix-mollie-1.6.1/pyproject.toml`

 * *Files identical despite different names*

