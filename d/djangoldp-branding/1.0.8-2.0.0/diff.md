# Comparing `tmp/djangoldp_branding-1.0.8.tar.gz` & `tmp/djangoldp_branding-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_branding-1.0.8.tar", last modified: Wed Jul 20 09:38:46 2022, max compression
+gzip compressed data, was "djangoldp_branding-2.0.0.tar", last modified: Thu Jul 27 15:06:19 2023, max compression
```

## Comparing `djangoldp_branding-1.0.8.tar` & `djangoldp_branding-2.0.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     2358 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      569 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding.egg-info/
--rw-r--r--   0 root         (0) root         (0)      313 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2964 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      313 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/
--rw-rw-rw-   0 root         (0) root         (0)     2954 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/views.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/accessrequests/
--rw-rw-rw-   0 root         (0) root         (0)     2071 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/accessrequests/access_requested.html
--rw-rw-rw-   0 root         (0) root         (0)     2067 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/accessrequests/access_resolved.html
--rw-rw-rw-   0 root         (0) root         (0)     6040 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/base_email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      353 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)     2088 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_change_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2094 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)     1970 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      525 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1288 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      538 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      497 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/lost_user.html
--rw-rw-rw-   0 root         (0) root         (0)      263 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/activate.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      489 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/logged_out.html
--rw-rw-rw-   0 root         (0) root         (0)      545 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      482 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/logout.html
--rw-rw-rw-   0 root         (0) root         (0)     4159 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/login.html
--rw-rw-rw-   0 root         (0) root         (0)      500 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_change_done.html
--rw-rw-rw-   0 root         (0) root         (0)      297 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2103 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/joboffer/
--rw-rw-rw-   0 root         (0) root         (0)     2557 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/joboffer/email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/admin/
--rw-rw-rw-   0 root         (0) root         (0)     4686 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/admin/base.html
--rw-rw-rw-   0 root         (0) root         (0)     2458 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/admin/login.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)     2381 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/oidc_provider/authorize.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/password/
--rw-rw-rw-   0 root         (0) root         (0)     1791 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/password/email.html
--rw-rw-rw-   0 root         (0) root         (0)     2279 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)      551 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     2052 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      275 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      266 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      380 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/activation_failed.html
--rw-rw-rw-   0 root         (0) root         (0)      567 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)       50 2022-07-20 09:38:44.000000 djangoldp_branding-1.0.8/djangoldp_branding/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15362 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/es/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     7249 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/es/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15233 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     7176 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/fr/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    14897 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/en/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     6840 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)      110 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/static/css/
--rw-rw-rw-   0 root         (0) root         (0)    19356 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/static/css/admin.css
--rw-rw-rw-   0 root         (0) root         (0)      432 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/static/css/main.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/static/images/
--rw-rw-rw-   0 root         (0) root         (0)      832 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/static/images/favicon.webp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templatetags/orbit.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/djangoldp_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.570899 djangoldp_branding-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      285 2023-07-27 15:06:19.570899 djangoldp_branding-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2358 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.554898 djangoldp_branding-2.0.0/djangoldp_branding/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-27 15:06:17.000000 djangoldp_branding-2.0.0/djangoldp_branding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/djangoldp_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.550898 djangoldp_branding-2.0.0/djangoldp_branding/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.550898 djangoldp_branding-2.0.0/djangoldp_branding/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.558898 djangoldp_branding-2.0.0/djangoldp_branding/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     6840 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    14897 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.550898 djangoldp_branding-2.0.0/djangoldp_branding/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.562898 djangoldp_branding-2.0.0/djangoldp_branding/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7249 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    15362 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.550898 djangoldp_branding-2.0.0/djangoldp_branding/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.562898 djangoldp_branding-2.0.0/djangoldp_branding/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7176 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    15233 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.550898 djangoldp_branding-2.0.0/djangoldp_branding/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.562898 djangoldp_branding-2.0.0/djangoldp_branding/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)    19356 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/static/css/admin.css
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/static/css/main.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.562898 djangoldp_branding-2.0.0/djangoldp_branding/static/images/
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/static/images/favicon.webp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.562898 djangoldp_branding-2.0.0/djangoldp_branding/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.562898 djangoldp_branding-2.0.0/djangoldp_branding/templates/accessrequests/
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/accessrequests/access_requested.html
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/accessrequests/access_resolved.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.562898 djangoldp_branding-2.0.0/djangoldp_branding/templates/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     4669 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/admin/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     2458 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/admin/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     2287 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     6023 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/base_email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.566898 djangoldp_branding-2.0.0/djangoldp_branding/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/django_registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/django_registration/activation_failed.html
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/django_registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/django_registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     2052 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/django_registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.566898 djangoldp_branding-2.0.0/djangoldp_branding/templates/joboffer/
+-rw-rw-rw-   0 root         (0) root         (0)     2557 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/joboffer/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.566898 djangoldp_branding-2.0.0/djangoldp_branding/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2381 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/oidc_provider/authorize.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.566898 djangoldp_branding-2.0.0/djangoldp_branding/templates/password/
+-rw-rw-rw-   0 root         (0) root         (0)     1791 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/password/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.570899 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/activate.html
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/logged_out.html
+-rw-rw-rw-   0 root         (0) root         (0)     4159 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/login.html
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/logout.html
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/lost_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_change_done.html
+-rw-rw-rw-   0 root         (0) root         (0)     2088 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1288 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      297 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/registration_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.570899 djangoldp_branding-2.0.0/djangoldp_branding/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/templatetags/orbit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2954 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/djangoldp_branding/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:19.558898 djangoldp_branding-2.0.0/djangoldp_branding.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-07-27 15:06:19.000000 djangoldp_branding-2.0.0/djangoldp_branding.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-07-27 15:06:19.000000 djangoldp_branding-2.0.0/djangoldp_branding.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 15:06:19.000000 djangoldp_branding-2.0.0/djangoldp_branding.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-27 15:06:19.000000 djangoldp_branding-2.0.0/djangoldp_branding.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-27 15:06:19.000000 djangoldp_branding-2.0.0/djangoldp_branding.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-27 15:06:19.570899 djangoldp_branding-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-07-27 15:06:00.000000 djangoldp_branding-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_branding-1.0.8/README.md` & `djangoldp_branding-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/setup.cfg` & `djangoldp_branding-2.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 author_email = jbaptiste@startinblox.com
 description = djangoldp package for GBS
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp~=2.1
+	djangoldp~=3.0
 
 [options.extras_require]
 include_package_data = True
 
 [semantic_release]
 version_source = tag
 version_variable = djangoldp_branding/__init__.py:__version__
```

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding.egg-info/SOURCES.txt` & `djangoldp_branding-2.0.0/djangoldp_branding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/views.py` & `djangoldp_branding-2.0.0/djangoldp_branding/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/processor.py` & `djangoldp_branding-2.0.0/djangoldp_branding/processor.py`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/accessrequests/access_requested.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/accessrequests/access_requested.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/accessrequests/access_resolved.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/accessrequests/access_resolved.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/base_email.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/base_email.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% load i18n %}
 {% load orbit %}
-{% load static from staticfiles %}
+{% load static %}
 {% get_current_language as LANGUAGE_CODE %}{% get_current_language_bidi as LANGUAGE_BIDI %}
 <!DOCTYPE html>
 <html lang="{{ LANGUAGE_CODE|default:"en-us" }}"{% if LANGUAGE_BIDI %} dir="rtl"{% endif %}>
   <head>
     <meta charset="UTF-8" />
     <title>{% orbit 'client.name' %} - {% block title %}{% endblock %}</title>
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-{% load i18n %} {% load orbit %} {% load static from staticfiles %} {%
-get_current_language as LANGUAGE_CODE %}{% get_current_language_bidi as
-LANGUAGE_BIDI %}
+{% load i18n %} {% load orbit %} {% load static %} {% get_current_language as
+LANGUAGE_CODE %}{% get_current_language_bidi as LANGUAGE_BIDI %}
 
  }}"{% if LANGUAGE_BIDI %} dir="rtl"{% endif %}>
 
 
  [{% orbit 'client.name' %}]                                                            
   {% block content %}{% endblock %}
                                                  {% orbit "client.name" %}
```

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_change_form.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_email.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_confirm.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/activation_complete.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_form.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_complete.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/registration_closed.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/registration_closed.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/login.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/email.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/joboffer/email.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/joboffer/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/admin/base.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/admin/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% load i18n %}
 {% load orbit %}
-{% load static from staticfiles %}
+{% load static %}
 {% get_current_language as LANGUAGE_CODE %}{% get_current_language_bidi as LANGUAGE_BIDI %}
 <!DOCTYPE html>
 <html lang="{{ LANGUAGE_CODE|default:"en-us" }}"{% if LANGUAGE_BIDI %} dir="rtl"{% endif %}>
   <head>
     <meta charset="UTF-8" />
     <title>{% orbit 'client.name' %} - {% block title %}{% endblock %}</title>
     <meta http-equiv="X-UA-Compatible" content="ie=edge" />
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-{% load i18n %} {% load orbit %} {% load static from staticfiles %} {%
-get_current_language as LANGUAGE_CODE %}{% get_current_language_bidi as
-LANGUAGE_BIDI %}
+{% load i18n %} {% load orbit %} {% load static %} {% get_current_language as
+LANGUAGE_CODE %}{% get_current_language_bidi as LANGUAGE_BIDI %}
 
  }}"{% if LANGUAGE_BIDI %} dir="rtl"{% endif %}>
 
 ss/base.css" %}{% endblock %}"> {% block extrastyle %}{% endblock %} {% if
 LANGUAGE_BIDI %}
 ss/rtl.css" %}{% endblock %}">{% endif %}
```

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/admin/login.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/oidc_provider/authorize.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/password/email.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/password/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/base.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   <head>
     <meta charset="UTF-8" />
     <title>{% orbit 'client_settings.name' %} - {% block title %}{{ title }}{% endblock %}</title>
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <meta http-equiv="X-UA-Compatible" content="ie=edge" />
     <link rel="preconnect" href="https://fonts.gstatic.com" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&amp;display=swap" />
-    <link rel="stylesheet" href="https://unpkg.com/@startinblox/orbit-styling-framework" />
+    <link rel="stylesheet" href="https://cdn.startinblox.com/orbit-styling-framework/index.css" />
     <link rel="stylesheet" href="{% static 'css/main.css' %}{% if debug_flag %}?{% now 'U' %}{% endif %}" />
     {% block extrastyle %}{% endblock %}
     {% if "css" in client_settings %}
     <link rel="stylesheet" href="{% orbit 'client.css' %}" />
     {% endif %}
     {% if "favicon" in client_settings %}
     <link rel="icon" type="image/webp" href="{% orbit 'client.favicon' %}">
@@ -38,8 +38,9 @@
           <div class="segment full sm-full whitespace-normal">
             {% block content %}{% autoescape off %}{{ content }}{% endautoescape %}{% endblock %}
           </div>
         </div>
       </div>
     </div>
   </body>
+
 </html>
```

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/activation_complete.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/django_registration/activation_complete.html`

 * *Files 19% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 
 {% block content %}
 
 <p class="text-semibold text-color-heading">
   {% trans "Merci, l'activation est terminée" %}.
 </p>
 
-{% url 'login' as auth_login_url %}
 <div class="segment full margin-top-xsmall">
-  <a class="button reversed button-icon text-xsmall text-bold text-uppercase color-secondary bordered icon-rocket icon-small icon-margin-right-xsmall" href="{% auth_login_url %}">{% trans "Se connecter" %}</a>
+  <a class="button reversed button-icon text-xsmall text-bold text-uppercase color-secondary bordered icon-rocket icon-small icon-margin-right-xsmall" 
+  href="{% url 'login' %}">{% trans "Se connecter" %}</a>
 </div>
 
 {% endblock %}
```

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/registration_form.html` & `djangoldp_branding-2.0.0/djangoldp_branding/templates/django_registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/djangoldp_urls.py` & `djangoldp_branding-2.0.0/djangoldp_branding/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/locale/es/LC_MESSAGES/django.po` & `djangoldp_branding-2.0.0/djangoldp_branding/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/locale/es/LC_MESSAGES/django.mo` & `djangoldp_branding-2.0.0/djangoldp_branding/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/locale/fr/LC_MESSAGES/django.po` & `djangoldp_branding-2.0.0/djangoldp_branding/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/locale/fr/LC_MESSAGES/django.mo` & `djangoldp_branding-2.0.0/djangoldp_branding/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/locale/en/LC_MESSAGES/django.po` & `djangoldp_branding-2.0.0/djangoldp_branding/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/locale/en/LC_MESSAGES/django.mo` & `djangoldp_branding-2.0.0/djangoldp_branding/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/static/css/admin.css` & `djangoldp_branding-2.0.0/djangoldp_branding/static/css/admin.css`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/static/images/favicon.webp` & `djangoldp_branding-2.0.0/djangoldp_branding/static/images/favicon.webp`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/templatetags/orbit.py` & `djangoldp_branding-2.0.0/djangoldp_branding/templatetags/orbit.py`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.8/djangoldp_branding/djangoldp_settings.py` & `djangoldp_branding-2.0.0/djangoldp_branding/djangoldp_settings.py`

 * *Files identical despite different names*

