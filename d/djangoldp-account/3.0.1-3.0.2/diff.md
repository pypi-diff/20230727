# Comparing `tmp/djangoldp_account-3.0.1.tar.gz` & `tmp/djangoldp_account-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_account-3.0.1.tar", last modified: Mon Jul 24 19:59:25 2023, max compression
+gzip compressed data, was "djangoldp_account-3.0.2.tar", last modified: Thu Jul 27 14:42:02 2023, max compression
```

## Comparing `djangoldp_account-3.0.1.tar` & `djangoldp_account-3.0.2.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.802680 djangoldp_account-3.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      275 2023-07-24 19:59:25.802680 djangoldp_account-3.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8962 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.786680 djangoldp_account-3.0.1/djangoldp_account/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-24 19:59:22.000000 djangoldp_account-3.0.1/djangoldp_account/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/auth/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6745 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/auth/backends.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/auth/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     3141 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/auth/solid.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/djangoldp_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9594 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/endpoints/rp_login.py
--rw-rw-rw-   0 root         (0) root         (0)     1296 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/endpoints/webfinger.py
--rw-rw-rw-   0 root         (0) root         (0)     1142 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/errors.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.786680 djangoldp_account-3.0.1/djangoldp_account/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.782680 djangoldp_account-3.0.1/djangoldp_account/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)     9063 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.786680 djangoldp_account-3.0.1/djangoldp_account/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7687 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    12366 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.786680 djangoldp_account-3.0.1/djangoldp_account/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     8046 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    13008 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.786680 djangoldp_account-3.0.1/djangoldp_account/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     7801 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    12899 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1837 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/management/commands/create_distant_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/management/commands/fill_user_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     2919 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/management/commands/import_csv.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/management/commands/mock_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.794680 djangoldp_account-3.0.1/djangoldp_account/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     4931 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0002_auto_20190917_1141.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0003_auto_20191024_0854.py
--rw-rw-rw-   0 root         (0) root         (0)      606 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0004_auto_20191203_0921.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0005_ldpuser_default_redirect_uri.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0006_auto_20200121_1321.py
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0007_auto_20200130_1242.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0008_auto_20200130_1251.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0009_auto_20200429_1346.py
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0010_auto_20200501_1207.py
--rw-rw-rw-   0 root         (0) root         (0)      602 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0011_auto_20200501_1420.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0012_auto_20200501_1433.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0013_auto_20200505_1733.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0014_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0015_auto_20200617_1817.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0016_auto_20200903_1049.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0017_auto_20200910_1606.py
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0018_auto_20210223_2254.py
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/0019_auto_20221031_1426.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9600 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.794680 djangoldp_account-3.0.1/djangoldp_account/static/
--rw-rw-rw-   0 root         (0) root         (0)     2675 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/static/base.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.794680 djangoldp_account-3.0.1/djangoldp_account/static/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/static/django_registration/registration_form.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.794680 djangoldp_account-3.0.1/djangoldp_account/static/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/static/oidc_provider/authorize.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.794680 djangoldp_account-3.0.1/djangoldp_account/static/registration/
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/static/registration/login.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.794680 djangoldp_account-3.0.1/djangoldp_account/templates/
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.798680 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/activation_email_body.txt
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/activation_failed.html
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/registration_base.html
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/registration_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.798680 djangoldp_account-3.0.1/djangoldp_account/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/oidc_provider/authorize.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.798680 djangoldp_account-3.0.1/djangoldp_account/templates/password/
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/password/email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.802680 djangoldp_account-3.0.1/djangoldp_account/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/activate.html
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/activation_email.txt
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)     2969 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/login.html
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/logout.html
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/lost_user.html
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_change_done.html
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_change_form.html
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      374 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/templates/registration/registration_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.802680 djangoldp_account-3.0.1/djangoldp_account/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)      814 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     7461 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/tests/tests_auth_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     2201 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/tests/tests_update.py
--rw-rw-rw-   0 root         (0) root         (0)     9436 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/djangoldp_account/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 19:59:25.790680 djangoldp_account-3.0.1/djangoldp_account.egg-info/
--rw-r--r--   0 root         (0) root         (0)      275 2023-07-24 19:59:25.000000 djangoldp_account-3.0.1/djangoldp_account.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5027 2023-07-24 19:59:25.000000 djangoldp_account-3.0.1/djangoldp_account.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 19:59:25.000000 djangoldp_account-3.0.1/djangoldp_account.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-07-24 19:59:25.000000 djangoldp_account-3.0.1/djangoldp_account.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-24 19:59:25.000000 djangoldp_account-3.0.1/djangoldp_account.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-07-24 19:59:25.802680 djangoldp_account-3.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 19:59:05.000000 djangoldp_account-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.086003 djangoldp_account-3.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      275 2023-07-27 14:42:02.086003 djangoldp_account-3.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8962 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.070003 djangoldp_account-3.0.2/djangoldp_account/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-27 14:41:59.000000 djangoldp_account-3.0.2/djangoldp_account/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.070003 djangoldp_account-3.0.2/djangoldp_account/auth/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6745 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/auth/backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/auth/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     3141 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/auth/solid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/djangoldp_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.074003 djangoldp_account-3.0.2/djangoldp_account/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9594 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/endpoints/rp_login.py
+-rw-rw-rw-   0 root         (0) root         (0)     1296 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/endpoints/webfinger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.066003 djangoldp_account-3.0.2/djangoldp_account/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.066003 djangoldp_account-3.0.2/djangoldp_account/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.074003 djangoldp_account-3.0.2/djangoldp_account/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     9063 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.066003 djangoldp_account-3.0.2/djangoldp_account/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.074003 djangoldp_account-3.0.2/djangoldp_account/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7687 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    12366 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.066003 djangoldp_account-3.0.2/djangoldp_account/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.074003 djangoldp_account-3.0.2/djangoldp_account/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     8046 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    13008 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.066003 djangoldp_account-3.0.2/djangoldp_account/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.074003 djangoldp_account-3.0.2/djangoldp_account/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     7801 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)    12899 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.074003 djangoldp_account-3.0.2/djangoldp_account/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.074003 djangoldp_account-3.0.2/djangoldp_account/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/management/commands/create_distant_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/management/commands/fill_user_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/management/commands/import_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/management/commands/mock_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.078003 djangoldp_account-3.0.2/djangoldp_account/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     4931 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0002_auto_20190917_1141.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0003_auto_20191024_0854.py
+-rw-rw-rw-   0 root         (0) root         (0)      606 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0004_auto_20191203_0921.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0005_ldpuser_default_redirect_uri.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0006_auto_20200121_1321.py
+-rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0007_auto_20200130_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0008_auto_20200130_1251.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0009_auto_20200429_1346.py
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0010_auto_20200501_1207.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0011_auto_20200501_1420.py
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0012_auto_20200501_1433.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0013_auto_20200505_1733.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0014_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0015_auto_20200617_1817.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0016_auto_20200903_1049.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0017_auto_20200910_1606.py
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0018_auto_20210223_2254.py
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/0019_auto_20221031_1426.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9600 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.078003 djangoldp_account-3.0.2/djangoldp_account/static/
+-rw-rw-rw-   0 root         (0) root         (0)     2675 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/static/base.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.078003 djangoldp_account-3.0.2/djangoldp_account/static/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/static/django_registration/registration_form.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.078003 djangoldp_account-3.0.2/djangoldp_account/static/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/static/oidc_provider/authorize.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.078003 djangoldp_account-3.0.2/djangoldp_account/static/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/static/registration/login.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.078003 djangoldp_account-3.0.2/djangoldp_account/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.078003 djangoldp_account-3.0.2/djangoldp_account/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/django_registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/django_registration/activation_email_body.txt
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/django_registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/django_registration/activation_failed.html
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/django_registration/registration_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/django_registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/django_registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/django_registration/registration_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.078003 djangoldp_account-3.0.2/djangoldp_account/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/oidc_provider/authorize.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.078003 djangoldp_account-3.0.2/djangoldp_account/templates/password/
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/password/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.082003 djangoldp_account-3.0.2/djangoldp_account/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/activate.html
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/activation_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/login.html
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/logout.html
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/lost_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/password_change_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/password_change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      374 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:41:42.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/password_reset_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/templates/registration/registration_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.086003 djangoldp_account-3.0.2/djangoldp_account/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:41:42.000000 djangoldp_account-3.0.2/djangoldp_account/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      814 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     7461 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/tests/tests_auth_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     2201 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/tests/tests_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     9993 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/djangoldp_account/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:42:02.070003 djangoldp_account-3.0.2/djangoldp_account.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-07-27 14:42:01.000000 djangoldp_account-3.0.2/djangoldp_account.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5027 2023-07-27 14:42:02.000000 djangoldp_account-3.0.2/djangoldp_account.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 14:42:01.000000 djangoldp_account-3.0.2/djangoldp_account.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-07-27 14:42:01.000000 djangoldp_account-3.0.2/djangoldp_account.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-27 14:42:01.000000 djangoldp_account-3.0.2/djangoldp_account.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-07-27 14:42:02.086003 djangoldp_account-3.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-27 14:41:41.000000 djangoldp_account-3.0.2/setup.py
```

### Comparing `djangoldp_account-3.0.1/README.md` & `djangoldp_account-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/admin.py` & `djangoldp_account-3.0.2/djangoldp_account/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/auth/backends.py` & `djangoldp_account-3.0.2/djangoldp_account/auth/backends.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/auth/middleware.py` & `djangoldp_account-3.0.2/djangoldp_account/auth/middleware.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/auth/solid.py` & `djangoldp_account-3.0.2/djangoldp_account/auth/solid.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/djangoldp_settings.py` & `djangoldp_account-3.0.2/djangoldp_account/djangoldp_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/djangoldp_urls.py` & `djangoldp_account-3.0.2/djangoldp_account/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/endpoints/rp_login.py` & `djangoldp_account-3.0.2/djangoldp_account/endpoints/rp_login.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/endpoints/webfinger.py` & `djangoldp_account-3.0.2/djangoldp_account/endpoints/webfinger.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/errors.py` & `djangoldp_account-3.0.2/djangoldp_account/errors.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/factories.py` & `djangoldp_account-3.0.2/djangoldp_account/factories.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/forms.py` & `djangoldp_account-3.0.2/djangoldp_account/forms.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/locale/de/LC_MESSAGES/django.po` & `djangoldp_account-3.0.2/djangoldp_account/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/locale/en/LC_MESSAGES/django.mo` & `djangoldp_account-3.0.2/djangoldp_account/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/locale/en/LC_MESSAGES/django.po` & `djangoldp_account-3.0.2/djangoldp_account/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/locale/es/LC_MESSAGES/django.mo` & `djangoldp_account-3.0.2/djangoldp_account/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/locale/es/LC_MESSAGES/django.po` & `djangoldp_account-3.0.2/djangoldp_account/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/locale/fr/LC_MESSAGES/django.mo` & `djangoldp_account-3.0.2/djangoldp_account/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/locale/fr/LC_MESSAGES/django.po` & `djangoldp_account-3.0.2/djangoldp_account/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/management/commands/create_distant_admin.py` & `djangoldp_account-3.0.2/djangoldp_account/management/commands/create_distant_admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/management/commands/fill_user_fields.py` & `djangoldp_account-3.0.2/djangoldp_account/management/commands/fill_user_fields.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/management/commands/import_csv.py` & `djangoldp_account-3.0.2/djangoldp_account/management/commands/import_csv.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/management/commands/mock_account.py` & `djangoldp_account-3.0.2/djangoldp_account/management/commands/mock_account.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0001_initial.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0002_auto_20190917_1141.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0002_auto_20190917_1141.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0003_auto_20191024_0854.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0003_auto_20191024_0854.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0004_auto_20191203_0921.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0004_auto_20191203_0921.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0006_auto_20200121_1321.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0006_auto_20200121_1321.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0007_auto_20200130_1242.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0007_auto_20200130_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0008_auto_20200130_1251.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0008_auto_20200130_1251.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0009_auto_20200429_1346.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0009_auto_20200429_1346.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0010_auto_20200501_1207.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0010_auto_20200501_1207.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0011_auto_20200501_1420.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0011_auto_20200501_1420.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0012_auto_20200501_1433.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0012_auto_20200501_1433.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0013_auto_20200505_1733.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0013_auto_20200505_1733.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0014_auto_20200610_1323.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0014_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0015_auto_20200617_1817.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0015_auto_20200617_1817.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0016_auto_20200903_1049.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0016_auto_20200903_1049.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0017_auto_20200910_1606.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0017_auto_20200910_1606.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/migrations/0019_auto_20221031_1426.py` & `djangoldp_account-3.0.2/djangoldp_account/migrations/0019_auto_20221031_1426.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/models.py` & `djangoldp_account-3.0.2/djangoldp_account/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/permissions.py` & `djangoldp_account-3.0.2/djangoldp_account/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/static/base.css` & `djangoldp_account-3.0.2/djangoldp_account/static/base.css`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/static/registration/login.css` & `djangoldp_account-3.0.2/djangoldp_account/static/registration/login.css`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/templates/base.html` & `djangoldp_account-3.0.2/djangoldp_account/templates/base.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/activation_complete.html` & `djangoldp_account-3.0.2/djangoldp_account/templates/django_registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/activation_email_body.txt` & `djangoldp_account-3.0.2/djangoldp_account/templates/django_registration/activation_email_body.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/templates/django_registration/registration_form.html` & `djangoldp_account-3.0.2/djangoldp_account/templates/django_registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/templates/oidc_provider/authorize.html` & `djangoldp_account-3.0.2/djangoldp_account/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/templates/password/email.html` & `djangoldp_account-3.0.2/djangoldp_account/templates/password/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/templates/registration/login.html` & `djangoldp_account-3.0.2/djangoldp_account/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/templates/registration/lost_user.html` & `djangoldp_account-3.0.2/djangoldp_account/templates/registration/lost_user.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/templates/registration/password_reset_form.html` & `djangoldp_account-3.0.2/djangoldp_account/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/tests/models.py` & `djangoldp_account-3.0.2/djangoldp_account/tests/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/tests/runner.py` & `djangoldp_account-3.0.2/djangoldp_account/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/tests/tests_auth_backends.py` & `djangoldp_account-3.0.2/djangoldp_account/tests/tests_auth_backends.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/tests/tests_update.py` & `djangoldp_account-3.0.2/djangoldp_account/tests/tests_update.py`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/djangoldp_account/views.py` & `djangoldp_account-3.0.2/djangoldp_account/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,20 +145,34 @@
 
 class LDPAccountRegistrationView(RedirectURLMixin, RegistrationView):
     """
     Extension of django-registration's RegistrationView for managing user's default_redirect_uri
     """
     template_name = getattr(django_settings, 'REGISTRATION_TEMPLATE_PATH', 'django_registration/registration_form.html')
 
-    def get_redirect_url(self):
+    def get_success_url(self, user=None):  # pylint: disable=unused-argument
+        """
+        Return the URL to redirect to after successful redirection.
+
+        """
+        # This is overridden solely to allow django-registration to
+        # support passing the user account as an argument; otherwise,
+        # the base FormMixin implementation, which accepts no
+        # arguments, could be called and end up raising a TypeError.
+        self.success_url = reverse_lazy("django_registration_complete")
+
+        return self.success_url
+
+    def get_redirect_url(self, user=None):
         """Return the user-originating redirect URL if it's safe."""
         redirect_to = self.request.POST.get(
             'next',
             self.request.GET.get('next', '')
         )
+
         url_is_safe = url_has_allowed_host_and_scheme(
             url=redirect_to,
             allowed_hosts=self.get_success_url_allowed_hosts(),
             require_https=self.request.is_secure(),
         )
         return redirect_to if url_is_safe else ''
```

### Comparing `djangoldp_account-3.0.1/djangoldp_account.egg-info/SOURCES.txt` & `djangoldp_account-3.0.2/djangoldp_account.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_account-3.0.1/setup.cfg` & `djangoldp_account-3.0.2/setup.cfg`

 * *Files identical despite different names*

