# Comparing `tmp/djangoldp-3.0.6.tar.gz` & `tmp/djangoldp-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp-3.0.6.tar", last modified: Mon Jul 24 20:29:58 2023, max compression
+gzip compressed data, was "djangoldp-3.0.7.tar", last modified: Thu Jul 27 14:58:59 2023, max compression
```

## Comparing `djangoldp-3.0.6.tar` & `djangoldp-3.0.7.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-24 20:29:34.000000 djangoldp-3.0.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-24 20:29:34.000000 djangoldp-3.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-24 20:29:58.734598 djangoldp-3.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3694 2023-07-24 20:29:34.000000 djangoldp-3.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.722597 djangoldp-3.0.6/djangoldp/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-24 20:29:51.000000 djangoldp-3.0.6/djangoldp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/activities/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/activities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/activities/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     5050 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/activities/objects.py
--rw-rw-rw-   0 root         (0) root         (0)    30916 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/activities/services.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/activities/verbs.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2075 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     5144 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     4621 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/conf/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5269 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/ldpsettings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/conf/package_template/
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/__init__.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/admin.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/apps.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/djangoldp_settings.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/djangoldp_urls.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/models.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/tests.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/app_name/views.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      374 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/package_template/setup.py-tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/conf/server_template/
--rwxrwxrwx   0 root         (0) root         (0)      816 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/server_template/manage.py-tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/conf/server_template/server/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/server_template/server/__init__.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/server_template/server/urls.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/server_template/server/wsgi.py-tpl
--rw-rw-rw-   0 root         (0) root         (0)      367 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/conf/server_template/settings.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3043 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/endpoints/webfinger.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/fields.py
--rw-rw-rw-   0 root         (0) root         (0)     6264 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/management/commands/check_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/management/commands/configure.py
--rw-rw-rw-   0 root         (0) root         (0)     2524 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/management/commands/federate.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/management/commands/mock_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.730598 djangoldp-3.0.6/djangoldp/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0002_auto_20190906_0642.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0003_auto_20190911_0931.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0004_auto_20200221_1118.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0005_auto_20200221_1127.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0006_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0007_auto_20200429_1346.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0008_auto_20200501_1207.py
--rw-rw-rw-   0 root         (0) root         (0)      601 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0009_auto_20200505_1733.py
--rw-rw-rw-   0 root         (0) root         (0)     1176 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0010_follower.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0011_auto_20200610_1323.py
--rw-rw-rw-   0 root         (0) root         (0)      992 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0012_auto_20200617_1817.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0013_auto_20200624_1709.py
--rw-rw-rw-   0 root         (0) root         (0)     3177 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0014_auto_20200909_2206.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/0015_auto_20210125_1847.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21294 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1188 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     7718 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2594 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/related.py
--rw-rw-rw-   0 root         (0) root         (0)    43569 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.730598 djangoldp-3.0.6/djangoldp/templates/
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/templates/swagger-ui.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/djangoldp_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1160 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp/tests/dummy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/dummy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/dummy/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/dummy/middleware.py
--rw-rw-rw-   0 root         (0) root         (0)    13968 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/performance_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     1179 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp/tests/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2209 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/scripts/prod_data_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     1324 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/scripts/test_data_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     5102 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/scripts/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      770 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/server_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1528 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_anonymous_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_auto_author.py
--rw-rw-rw-   0 root         (0) root         (0)    18371 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_backlinks_service.py
--rw-rw-rw-   0 root         (0) root         (0)    14619 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_cache.py
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_delete.py
--rw-rw-rw-   0 root         (0) root         (0)    12402 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_get.py
--rw-rw-rw-   0 root         (0) root         (0)     7640 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_guardian.py
--rw-rw-rw-   0 root         (0) root         (0)    28857 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_inbox.py
--rw-rw-rw-   0 root         (0) root         (0)     2811 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_ldp_model.py
--rw-rw-rw-   0 root         (0) root         (0)     6134 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_ldp_viewset.py
--rw-rw-rw-   0 root         (0) root         (0)    36663 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_model_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     6074 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_perf_get.py
--rw-rw-rw-   0 root         (0) root         (0)     1625 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_performance.py
--rw-rw-rw-   0 root         (0) root         (0)    12660 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_post.py
--rw-rw-rw-   0 root         (0) root         (0)     2031 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_sources.py
--rw-rw-rw-   0 root         (0) root         (0)    28385 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_update.py
--rw-rw-rw-   0 root         (0) root         (0)    23475 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/tests/tests_user_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    31406 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.726597 djangoldp-3.0.6/djangoldp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4271 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      283 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-24 20:29:58.000000 djangoldp-3.0.6/djangoldp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp_crypto/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp_crypto/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp_crypto/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/management/commands/creatersakey.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 20:29:58.734598 djangoldp-3.0.6/djangoldp_crypto/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-24 20:29:34.000000 djangoldp-3.0.6/djangoldp_crypto/models.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-07-24 20:29:58.734598 djangoldp-3.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-24 20:29:34.000000 djangoldp-3.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.377733 djangoldp-3.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-27 14:58:36.000000 djangoldp-3.0.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-27 14:58:36.000000 djangoldp-3.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-27 14:58:59.377733 djangoldp-3.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3694 2023-07-27 14:58:36.000000 djangoldp-3.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.365732 djangoldp-3.0.7/djangoldp/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-27 14:58:52.000000 djangoldp-3.0.7/djangoldp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.365732 djangoldp-3.0.7/djangoldp/activities/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/activities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/activities/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5050 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/activities/objects.py
+-rw-rw-rw-   0 root         (0) root         (0)    30916 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/activities/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/activities/verbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2631 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     5144 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     4621 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.365732 djangoldp-3.0.7/djangoldp/conf/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5300 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/default_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/ldpsettings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.365732 djangoldp-3.0.7/djangoldp/conf/package_template/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/package_template/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.369732 djangoldp-3.0.7/djangoldp/conf/package_template/app_name/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/package_template/app_name/__init__.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/package_template/app_name/admin.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/package_template/app_name/apps.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/package_template/app_name/djangoldp_settings.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/package_template/app_name/djangoldp_urls.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/package_template/app_name/models.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/package_template/app_name/tests.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/package_template/app_name/views.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      374 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/package_template/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/package_template/setup.py-tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.369732 djangoldp-3.0.7/djangoldp/conf/server_template/
+-rwxrwxrwx   0 root         (0) root         (0)      816 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/server_template/manage.py-tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.369732 djangoldp-3.0.7/djangoldp/conf/server_template/server/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/server_template/server/__init__.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/server_template/server/urls.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/server_template/server/wsgi.py-tpl
+-rw-rw-rw-   0 root         (0) root         (0)      367 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/conf/server_template/settings.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.369732 djangoldp-3.0.7/djangoldp/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3043 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/endpoints/webfinger.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     6264 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.369732 djangoldp-3.0.7/djangoldp/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.369732 djangoldp-3.0.7/djangoldp/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/management/commands/check_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/management/commands/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     2524 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/management/commands/federate.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/management/commands/mock_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.373732 djangoldp-3.0.7/djangoldp/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0002_auto_20190906_0642.py
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0003_auto_20190911_0931.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0004_auto_20200221_1118.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0005_auto_20200221_1127.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0006_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0007_auto_20200429_1346.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0008_auto_20200501_1207.py
+-rw-rw-rw-   0 root         (0) root         (0)      601 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0009_auto_20200505_1733.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0010_follower.py
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0011_auto_20200610_1323.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0012_auto_20200617_1817.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0013_auto_20200624_1709.py
+-rw-rw-rw-   0 root         (0) root         (0)     3177 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0014_auto_20200909_2206.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/0015_auto_20210125_1847.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21294 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     7718 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2594 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/related.py
+-rw-rw-rw-   0 root         (0) root         (0)    43569 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.373732 djangoldp-3.0.7/djangoldp/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/templates/swagger-ui.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.377733 djangoldp-3.0.7/djangoldp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/djangoldp_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.377733 djangoldp-3.0.7/djangoldp/tests/dummy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/dummy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/dummy/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/dummy/middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)    13968 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/performance_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.377733 djangoldp-3.0.7/djangoldp/tests/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2209 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/scripts/prod_data_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1324 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/scripts/test_data_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5102 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/scripts/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/server_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_anonymous_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_auto_author.py
+-rw-rw-rw-   0 root         (0) root         (0)    18371 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_backlinks_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    14619 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)    12402 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     7640 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_guardian.py
+-rw-rw-rw-   0 root         (0) root         (0)    28857 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_inbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     2811 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_ldp_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     6134 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_ldp_viewset.py
+-rw-rw-rw-   0 root         (0) root         (0)    36663 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_model_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     6074 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_perf_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_performance.py
+-rw-rw-rw-   0 root         (0) root         (0)    12660 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_post.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_sources.py
+-rw-rw-rw-   0 root         (0) root         (0)    28385 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_update.py
+-rw-rw-rw-   0 root         (0) root         (0)    23475 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/tests/tests_user_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31406 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.365732 djangoldp-3.0.7/djangoldp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-27 14:58:59.000000 djangoldp-3.0.7/djangoldp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-07-27 14:58:59.000000 djangoldp-3.0.7/djangoldp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 14:58:59.000000 djangoldp-3.0.7/djangoldp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-27 14:58:59.000000 djangoldp-3.0.7/djangoldp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 14:58:59.000000 djangoldp-3.0.7/djangoldp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      283 2023-07-27 14:58:59.000000 djangoldp-3.0.7/djangoldp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-27 14:58:59.000000 djangoldp-3.0.7/djangoldp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.377733 djangoldp-3.0.7/djangoldp_crypto/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp_crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp_crypto/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.377733 djangoldp-3.0.7/djangoldp_crypto/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp_crypto/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.377733 djangoldp-3.0.7/djangoldp_crypto/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp_crypto/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp_crypto/management/commands/creatersakey.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 14:58:59.377733 djangoldp-3.0.7/djangoldp_crypto/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp_crypto/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp_crypto/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-27 14:58:36.000000 djangoldp-3.0.7/djangoldp_crypto/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-07-27 14:58:59.377733 djangoldp-3.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-27 14:58:36.000000 djangoldp-3.0.7/setup.py
```

### Comparing `djangoldp-3.0.6/LICENSE` & `djangoldp-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/README.md` & `djangoldp-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/activities/objects.py` & `djangoldp-3.0.7/djangoldp/activities/objects.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/activities/services.py` & `djangoldp-3.0.7/djangoldp/activities/services.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/activities/verbs.py` & `djangoldp-3.0.7/djangoldp/activities/verbs.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/admin.py` & `djangoldp-3.0.7/djangoldp/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/apps.py` & `djangoldp-3.0.7/djangoldp/apps.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/check_integrity.py` & `djangoldp-3.0.7/djangoldp/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/cli.py` & `djangoldp-3.0.7/djangoldp/cli.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/conf/default_settings.py` & `djangoldp-3.0.7/djangoldp/conf/default_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
 ##################
 # AUTHENTICATION #
 ##################
 
 AUTHENTICATION_BACKENDS = ['django.contrib.auth.backends.ModelBackend', 'guardian.backends.ObjectPermissionBackend']
 
-OIDC_ACCESS_CONTROL_ALLOW_HEADERS = 'Content-Type, if-match, accept, authorization, DPoP'
+OIDC_ACCESS_CONTROL_ALLOW_HEADERS = 'Content-Type, if-match, accept, authorization, DPoP, cache-control, pragma, prefer'
 
 # The minimum number of seconds a password reset link is valid for
 PASSWORD_RESET_TIMEOUT = 60 * 60 * 24 * 3
 
 DISABLE_LOCAL_OBJECT_FILTER = False
 
 GUARDIAN_AUTO_PREFETCH = True
```

### Comparing `djangoldp-3.0.6/djangoldp/conf/ldpsettings.py` & `djangoldp-3.0.7/djangoldp/conf/ldpsettings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/conf/server_template/manage.py-tpl` & `djangoldp-3.0.7/djangoldp/conf/server_template/manage.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/conf/server_template/server/urls.py-tpl` & `djangoldp-3.0.7/djangoldp/conf/server_template/server/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/conf/server_template/server/wsgi.py-tpl` & `djangoldp-3.0.7/djangoldp/conf/server_template/server/wsgi.py-tpl`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/endpoints/webfinger.py` & `djangoldp-3.0.7/djangoldp/endpoints/webfinger.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/filters.py` & `djangoldp-3.0.7/djangoldp/filters.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/management/commands/check_integrity.py` & `djangoldp-3.0.7/djangoldp/management/commands/check_integrity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/management/commands/configure.py` & `djangoldp-3.0.7/djangoldp/management/commands/configure.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/management/commands/federate.py` & `djangoldp-3.0.7/djangoldp/management/commands/federate.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/middleware.py` & `djangoldp-3.0.7/djangoldp/middleware.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/migrations/0001_initial.py` & `djangoldp-3.0.7/djangoldp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/migrations/0002_auto_20190906_0642.py` & `djangoldp-3.0.7/djangoldp/migrations/0002_auto_20190906_0642.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/migrations/0006_activity.py` & `djangoldp-3.0.7/djangoldp/migrations/0006_activity.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/migrations/0007_auto_20200429_1346.py` & `djangoldp-3.0.7/djangoldp/migrations/0007_auto_20200429_1346.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/migrations/0008_auto_20200501_1207.py` & `djangoldp-3.0.7/djangoldp/migrations/0008_auto_20200501_1207.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/migrations/0009_auto_20200505_1733.py` & `djangoldp-3.0.7/djangoldp/migrations/0009_auto_20200505_1733.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/migrations/0010_follower.py` & `djangoldp-3.0.7/djangoldp/migrations/0010_follower.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/migrations/0011_auto_20200610_1323.py` & `djangoldp-3.0.7/djangoldp/migrations/0011_auto_20200610_1323.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/migrations/0012_auto_20200617_1817.py` & `djangoldp-3.0.7/djangoldp/migrations/0012_auto_20200617_1817.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/migrations/0013_auto_20200624_1709.py` & `djangoldp-3.0.7/djangoldp/migrations/0013_auto_20200624_1709.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/migrations/0014_auto_20200909_2206.py` & `djangoldp-3.0.7/djangoldp/migrations/0014_auto_20200909_2206.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/migrations/0015_auto_20210125_1847.py` & `djangoldp-3.0.7/djangoldp/migrations/0015_auto_20210125_1847.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/models.py` & `djangoldp-3.0.7/djangoldp/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/pagination.py` & `djangoldp-3.0.7/djangoldp/pagination.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/permissions.py` & `djangoldp-3.0.7/djangoldp/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/related.py` & `djangoldp-3.0.7/djangoldp/related.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/serializers.py` & `djangoldp-3.0.7/djangoldp/serializers.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/templates/swagger-ui.html` & `djangoldp-3.0.7/djangoldp/templates/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/djangoldp_urls.py` & `djangoldp-3.0.7/djangoldp/tests/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/models.py` & `djangoldp-3.0.7/djangoldp/tests/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/performance_runner.py` & `djangoldp-3.0.7/djangoldp/tests/performance_runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/runner.py` & `djangoldp-3.0.7/djangoldp/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/scripts/prod_data_generator.py` & `djangoldp-3.0.7/djangoldp/tests/scripts/prod_data_generator.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/scripts/test_data_generator.py` & `djangoldp-3.0.7/djangoldp/tests/scripts/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/scripts/utils.py` & `djangoldp-3.0.7/djangoldp/tests/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/server_settings.py` & `djangoldp-3.0.7/djangoldp/tests/server_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_anonymous_permissions.py` & `djangoldp-3.0.7/djangoldp/tests/tests_anonymous_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_auto_author.py` & `djangoldp-3.0.7/djangoldp/tests/tests_auto_author.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_backlinks_service.py` & `djangoldp-3.0.7/djangoldp/tests/tests_backlinks_service.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_cache.py` & `djangoldp-3.0.7/djangoldp/tests/tests_cache.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_delete.py` & `djangoldp-3.0.7/djangoldp/tests/tests_delete.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_get.py` & `djangoldp-3.0.7/djangoldp/tests/tests_get.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_guardian.py` & `djangoldp-3.0.7/djangoldp/tests/tests_guardian.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_inbox.py` & `djangoldp-3.0.7/djangoldp/tests/tests_inbox.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_ldp_model.py` & `djangoldp-3.0.7/djangoldp/tests/tests_ldp_model.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_ldp_viewset.py` & `djangoldp-3.0.7/djangoldp/tests/tests_ldp_viewset.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_model_serializer.py` & `djangoldp-3.0.7/djangoldp/tests/tests_model_serializer.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_pagination.py` & `djangoldp-3.0.7/djangoldp/tests/tests_pagination.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_perf_get.py` & `djangoldp-3.0.7/djangoldp/tests/tests_perf_get.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_performance.py` & `djangoldp-3.0.7/djangoldp/tests/tests_performance.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_post.py` & `djangoldp-3.0.7/djangoldp/tests/tests_post.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_settings.py` & `djangoldp-3.0.7/djangoldp/tests/tests_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_sources.py` & `djangoldp-3.0.7/djangoldp/tests/tests_sources.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_update.py` & `djangoldp-3.0.7/djangoldp/tests/tests_update.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/tests/tests_user_permissions.py` & `djangoldp-3.0.7/djangoldp/tests/tests_user_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/urls.py` & `djangoldp-3.0.7/djangoldp/urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/utils.py` & `djangoldp-3.0.7/djangoldp/utils.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp/views.py` & `djangoldp-3.0.7/djangoldp/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp.egg-info/SOURCES.txt` & `djangoldp-3.0.7/djangoldp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp_crypto/management/commands/creatersakey.py` & `djangoldp-3.0.7/djangoldp_crypto/management/commands/creatersakey.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp_crypto/migrations/0001_initial.py` & `djangoldp-3.0.7/djangoldp_crypto/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/djangoldp_crypto/models.py` & `djangoldp-3.0.7/djangoldp_crypto/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp-3.0.6/setup.cfg` & `djangoldp-3.0.7/setup.cfg`

 * *Files identical despite different names*

