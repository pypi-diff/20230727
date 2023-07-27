# Comparing `tmp/django-sphinx-hosting-1.1.5.tar.gz` & `tmp/django-sphinx-hosting-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sphinx-hosting-1.1.5.tar", last modified: Thu May  4 21:06:49 2023, max compression
+gzip compressed data, was "django-sphinx-hosting-1.2.0.tar", last modified: Thu Jul 27 20:15:34 2023, max compression
```

## Comparing `django-sphinx-hosting-1.1.5.tar` & `django-sphinx-hosting-1.2.0.tar`

### file list

```diff
@@ -1,91 +1,94 @@
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.083254 django-sphinx-hosting-1.1.5/
--rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.1.5/LICENSE.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.1.5/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-04 21:06:49.083448 django-sphinx-hosting-1.1.5/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.1.5/README.md
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.027914 django-sphinx-hosting-1.1.5/django_sphinx_hosting.egg-info/
--rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-05-04 21:06:48.000000 django-sphinx-hosting-1.1.5/django_sphinx_hosting.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) admin       (80)     2739 2023-05-04 21:06:48.000000 django-sphinx-hosting-1.1.5/django_sphinx_hosting.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-05-04 21:06:48.000000 django-sphinx-hosting-1.1.5/django_sphinx_hosting.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-05-04 21:06:48.000000 django-sphinx-hosting-1.1.5/django_sphinx_hosting.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-05-04 21:06:48.000000 django-sphinx-hosting-1.1.5/django_sphinx_hosting.egg-info/top_level.txt
--rw-rw-r--   0 cmalek     (501) admin       (80)     1256 2023-05-04 21:06:49.084358 django-sphinx-hosting-1.1.5/setup.cfg
--rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-05-04 21:06:38.000000 django-sphinx-hosting-1.1.5/setup.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.039768 django-sphinx-hosting-1.1.5/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-05-04 21:06:38.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.043068 django-sphinx-hosting-1.1.5/sphinx_hosting/api/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/api/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/api/apps.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4896 2023-03-28 15:50:00.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/api/serializers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1274 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/api/urls.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     8676 2023-04-06 17:29:54.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/api/views.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/apps.py
--rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/exc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/fields.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.043914 django-sphinx-hosting-1.1.5/sphinx_hosting/fixtures/
--rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/fixtures/classifiers.json
--rw-r--r--   0 cmalek     (501) admin       (80)      312 2023-05-03 16:48:22.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/form_fields.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     6919 2023-05-03 23:30:39.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/forms.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    22276 2023-05-04 16:31:15.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/importers.py
--rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/logging.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.044815 django-sphinx-hosting-1.1.5/sphinx_hosting/management/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/management/__init__.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.049070 django-sphinx-hosting-1.1.5/sphinx_hosting/management/commands/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/management/commands/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     2568 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/management/commands/import_docs.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1626 2023-02-01 17:53:25.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/management/commands/parse_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/management/commands/print_classifier_tree.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2288 2023-02-01 17:06:33.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/management/commands/print_doctree.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.062575 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/
--rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0001_initial.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0002_original_html.py
--rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0003_globaltoc.py
--rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0004_next_page_FK.py
--rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0005_orig_global_toc.py
--rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0007_load_classifiers.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0008_Version_archived.py
--rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
--rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0010_add_groups.py
--rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0011_machinenamefield.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/__init__.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    32525 2023-05-04 20:34:24.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/models.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/py.typed
--rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/search_indexes.py
--rw-r--r--   0 cmalek     (501) admin       (80)      566 2023-03-24 21:26:47.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/settings.py
--rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/signals.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.022497 django-sphinx-hosting-1.1.5/sphinx_hosting/static/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.022805 django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.068987 django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/css/
--rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
--rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
--rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
--rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.070013 django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/images/
--rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.023551 django-sphinx-hosting-1.1.5/sphinx_hosting/templates/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.023233 django-sphinx-hosting-1.1.5/sphinx_hosting/templates/search/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.023354 django-sphinx-hosting-1.1.5/sphinx_hosting/templates/search/indexes/
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.071641 django-sphinx-hosting-1.1.5/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
--rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.072661 django-sphinx-hosting-1.1.5/sphinx_hosting/templates/sphinx_hosting/
--rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/templates/sphinx_hosting/base.html
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.074411 django-sphinx-hosting-1.1.5/sphinx_hosting/templatetags/
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-05-03 20:48:17.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/templatetags/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)      444 2023-05-03 20:52:11.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/templatetags/sphinx_hosting.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/types.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     1656 2023-05-03 17:07:06.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/urls.py
--rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-05-03 16:45:18.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/validators.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    20844 2023-04-28 17:09:25.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/views.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.081054 django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/
--rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)     6630 2023-05-03 23:24:52.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/classifier.py
-drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-05-04 21:06:49.082909 django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/core/
--rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/core/__init__.py
--rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/core/basic.py
--rw-rw-r--   0 cmalek     (501) admin       (80)     4701 2023-05-04 19:20:06.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/navigation.py
--rw-r--r--   0 cmalek     (501) admin       (80)    14426 2023-05-04 20:40:19.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/project.py
--rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/search.py
--rw-r--r--   0 cmalek     (501) admin       (80)     7375 2023-05-03 22:49:20.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/sphinx_page.py
--rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/version.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.233319 django-sphinx-hosting-1.2.0/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1459 2023-04-28 16:31:54.000000 django-sphinx-hosting-1.2.0/LICENSE.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      221 2023-05-01 22:07:11.000000 django-sphinx-hosting-1.2.0/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-07-27 20:15:34.233528 django-sphinx-hosting-1.2.0/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1188 2023-04-28 17:53:11.000000 django-sphinx-hosting-1.2.0/README.md
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.181705 django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2207 2023-07-27 20:15:34.000000 django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2913 2023-07-27 20:15:34.000000 django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)        1 2023-07-27 20:15:34.000000 django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)      324 2023-07-27 20:15:34.000000 django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)       15 2023-07-27 20:15:34.000000 django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/top_level.txt
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1281 2023-07-27 20:15:34.234727 django-sphinx-hosting-1.2.0/setup.cfg
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1821 2023-07-27 20:15:11.000000 django-sphinx-hosting-1.2.0/setup.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.195402 django-sphinx-hosting-1.2.0/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)       21 2023-07-27 20:15:11.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.199204 django-sphinx-hosting-1.2.0/sphinx_hosting/api/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 23:25:25.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/api/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      331 2023-03-28 15:43:43.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/api/apps.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     5706 2023-07-27 18:03:47.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/api/serializers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1357 2023-07-27 20:06:34.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/api/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    13616 2023-07-27 17:25:04.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/api/views.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      305 2023-02-22 19:04:46.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/apps.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       49 2022-11-03 21:55:52.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/exc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-05-03 16:51:15.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/fields.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.200055 django-sphinx-hosting-1.2.0/sphinx_hosting/fixtures/
+-rw-r--r--   0 cmalek     (501) admin       (80)    12034 2023-04-07 22:07:37.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/fixtures/classifiers.json
+-rw-rw-r--   0 cmalek     (501) admin       (80)      445 2023-07-26 17:59:23.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/form_fields.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     8372 2023-07-27 17:56:55.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/forms.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    23812 2023-07-26 23:12:09.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/importers.py
+-rw-r--r--   0 cmalek     (501) admin       (80)       62 2022-11-17 22:11:14.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/logging.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.200855 django-sphinx-hosting-1.2.0/sphinx_hosting/management/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:32.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/__init__.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.205343 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-03 21:42:44.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2649 2023-07-26 23:13:05.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/fix_broken_hrefs.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2566 2023-07-26 17:58:46.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/import_docs.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1624 2023-07-26 17:58:54.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/parse_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1421 2023-02-01 17:06:59.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/print_classifier_tree.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2286 2023-07-26 17:59:35.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/print_doctree.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.216013 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/
+-rw-r--r--   0 cmalek     (501) admin       (80)     6366 2022-11-22 19:27:09.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0001_initial.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1592 2022-11-22 23:23:38.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0002_original_html.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      659 2022-12-08 23:32:00.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0003_globaltoc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      586 2022-12-09 00:04:04.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0004_next_page_FK.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      683 2023-01-06 00:23:12.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0005_orig_global_toc.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     3829 2023-03-24 22:50:14.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      658 2023-01-19 19:26:47.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0007_load_classifiers.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      497 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0008_Version_archived.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      857 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0009_SphinxPage_searchable.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     2858 2023-03-28 21:23:19.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0010_add_groups.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      935 2023-05-03 17:01:21.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0011_machinenamefield.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     1838 2023-07-26 18:06:51.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0012_project_relatedlinks.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      521 2023-07-27 17:59:47.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-04 18:37:19.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/__init__.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    33617 2023-07-27 17:55:22.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/models.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-11-18 23:13:36.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/py.typed
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1663 2023-04-27 18:08:13.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/search_indexes.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)      776 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/settings.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      625 2023-05-02 23:35:34.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/signals.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.175937 django-sphinx-hosting-1.2.0/sphinx_hosting/static/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.176285 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.220132 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/
+-rw-r--r--   0 cmalek     (501) admin       (80)     1075 2023-02-02 18:58:20.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)     4819 2022-11-22 19:08:46.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    18183 2023-01-10 17:44:02.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
+-rw-r--r--   0 cmalek     (501) admin       (80)    34945 2023-02-02 18:58:21.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
+-rw-r--r--   0 cmalek     (501) admin       (80)     2896 2023-02-01 21:52:48.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.221139 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/images/
+-rw-r--r--   0 cmalek     (501) admin       (80)    37933 2022-11-17 21:25:05.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/images/logo.jpg
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.177017 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.176716 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/search/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.176833 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/search/indexes/
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.222505 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/search/indexes/sphinxhostingcore/
+-rw-rw-r--   0 cmalek     (501) admin       (80)       36 2023-02-11 00:37:43.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/search/indexes/sphinxhostingcore/sphinxpage_text.txt
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.223152 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/sphinx_hosting/
+-rw-r--r--   0 cmalek     (501) admin       (80)      523 2023-01-18 19:41:49.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/templates/sphinx_hosting/base.html
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.224383 django-sphinx-hosting-1.2.0/sphinx_hosting/templatetags/
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-05-03 20:48:17.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/templatetags/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)      444 2023-05-03 20:52:11.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/templatetags/sphinx_hosting.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2022-10-21 21:37:03.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/types.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     2205 2023-07-26 17:16:32.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/urls.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     1103 2023-07-26 00:01:34.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/validators.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    26588 2023-07-27 17:58:45.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/views.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.230891 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/
+-rw-rw-r--   0 cmalek     (501) admin       (80)      255 2023-04-28 16:10:38.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     6630 2023-05-03 23:24:52.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/classifier.py
+drwxrwxr-x   0 cmalek     (501) admin       (80)        0 2023-07-27 20:15:34.232936 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/core/
+-rw-r--r--   0 cmalek     (501) admin       (80)       39 2023-01-18 23:39:43.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/core/__init__.py
+-rw-r--r--   0 cmalek     (501) admin       (80)        0 2023-01-18 23:39:52.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/core/basic.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)     4701 2023-05-04 19:20:06.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/navigation.py
+-rw-r--r--   0 cmalek     (501) admin       (80)    18051 2023-07-27 20:11:32.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/project.py
+-rw-rw-r--   0 cmalek     (501) admin       (80)    11411 2023-04-27 20:32:48.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/search.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     8924 2023-07-27 18:29:50.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/sphinx_page.py
+-rw-r--r--   0 cmalek     (501) admin       (80)     8438 2023-04-27 23:13:13.000000 django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/version.py
```

### Comparing `django-sphinx-hosting-1.1.5/LICENSE.txt` & `django-sphinx-hosting-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/PKG-INFO` & `django-sphinx-hosting-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.1.5
+Version: 1.2.0
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.1.5/README.md` & `django-sphinx-hosting-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/django_sphinx_hosting.egg-info/PKG-INFO` & `django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sphinx-hosting
-Version: 1.1.5
+Version: 1.2.0
 Summary: Reusable Django app for hosting Sphinx documentation privately.
 Home-page: https://github.com/caltechads/django-sphinx-hosting
 Author: Caltech IMSS ADS
 Author-email: imss-ads-staff@caltech.edu
 Keywords: documentation,sphinx,django
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `django-sphinx-hosting-1.1.5/django_sphinx_hosting.egg-info/SOURCES.txt` & `django-sphinx-hosting-1.2.0/django_sphinx_hosting.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 sphinx_hosting/api/apps.py
 sphinx_hosting/api/serializers.py
 sphinx_hosting/api/urls.py
 sphinx_hosting/api/views.py
 sphinx_hosting/fixtures/classifiers.json
 sphinx_hosting/management/__init__.py
 sphinx_hosting/management/commands/__init__.py
+sphinx_hosting/management/commands/fix_broken_hrefs.py
 sphinx_hosting/management/commands/import_docs.py
 sphinx_hosting/management/commands/parse_globaltoc.py
 sphinx_hosting/management/commands/print_classifier_tree.py
 sphinx_hosting/management/commands/print_doctree.py
 sphinx_hosting/migrations/0001_initial.py
 sphinx_hosting/migrations/0002_original_html.py
 sphinx_hosting/migrations/0003_globaltoc.py
@@ -44,14 +45,16 @@
 sphinx_hosting/migrations/0005_orig_global_toc.py
 sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py
 sphinx_hosting/migrations/0007_load_classifiers.py
 sphinx_hosting/migrations/0008_Version_archived.py
 sphinx_hosting/migrations/0009_SphinxPage_searchable.py
 sphinx_hosting/migrations/0010_add_groups.py
 sphinx_hosting/migrations/0011_machinenamefield.py
+sphinx_hosting/migrations/0012_project_relatedlinks.py
+sphinx_hosting/migrations/0013_projectrelatedlink_url_to_uri.py
 sphinx_hosting/migrations/__init__.py
 sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss
 sphinx_hosting/static/sphinx_hosting/css/_pygments.scss
 sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss
 sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css
 sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss
 sphinx_hosting/static/sphinx_hosting/images/logo.jpg
```

### Comparing `django-sphinx-hosting-1.1.5/setup.cfg` & `django-sphinx-hosting-1.2.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 disable = 
 	missing-docstring,
 	protected-access,
 	unused-argument,
 	invalid-name,
 	too-few-public-methods,
 	attribute-defined-outside-init,
+	consider-using-f-string,
 	too-many-lines,
 	no-member
 
 [mypy]
 python_executable = ~/.pyenv/shims/python
 implicit_optional = True
 exclude = (?x)(
-	^build$
+	^build
 	| sandbox\/setup\.py$
 	| migrations\/.*.py$
 	)
 
 [mypy-haystack.*]
 ignore_missing_imports = True
```

### Comparing `django-sphinx-hosting-1.1.5/setup.py` & `django-sphinx-hosting-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="django-sphinx-hosting",
-    version="1.1.5",
+    version="1.2.0",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "django-braces >= 1.15.0",
         "django-crispy-forms>=1.14.0",
         "django-extensions >= 3.2.1",
         "django-filter >= 22.1",
         "django-haystack >= 3.2.1",
         "django-rest-framework-helpers >= 8.5.0",
-        "django-theme-academy >= 0.3.0",
+        "django-theme-academy >= 0.3.5",
         "django-wildewidgets >= 0.16.7",
         "djangorestframework >= 3.14.0",
         "drf-spectacular >= 0.25.1",
         "crispy-bootstrap5",
         "humanize",
         "lxml >= 4.9.1",
         "cssselect >= 1.2.0",
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/api/serializers.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/api/serializers.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from django.db.models import Model
 from rest_framework import serializers
 from rest_framework.relations import RelatedField
 
 from sphinx_hosting.models import (
     Classifier,
     Project,
+    ProjectRelatedLink,
     SphinxImage,
     SphinxPage,
     Version,
 )
 
 
 class ClassifierSerializer(serializers.HyperlinkedModelSerializer):
@@ -31,32 +32,59 @@
 
     versions: RelatedField = serializers.HyperlinkedRelatedField(
         many=True,
         read_only=True,
         view_name='sphinx_hosting_api:version-detail'
     )
     classifiers: serializers.Serializer = ClassifierSerializer(many=True)
+    related_links: RelatedField = serializers.HyperlinkedRelatedField(
+        many=True,
+        read_only=True,
+        view_name='sphinx_hosting_api:projectrelatedlink-detail'
+    )
 
     class Meta:
         model: Type[Model] = Project
         read_only_fields: Tuple[str, ...] = ('machine_name', )
         fields: Tuple[str, ...] = (
             'url',
             'id',
             'title',
             'machine_name',
             'description',
+            'related_links',
             'classifiers',
             'versions',
         )
         extra_kwargs = {
             'url': {'view_name': 'sphinx_hosting_api:project-detail'},
         }
 
 
+class ProjectRelatedLinkSerializer(serializers.HyperlinkedModelSerializer):
+
+    project: RelatedField = serializers.HyperlinkedRelatedField(
+        queryset=Project.objects.all(),
+        view_name='sphinx_hosting_api:project-detail'
+    )
+
+    class Meta:
+        model: Type[Model] = ProjectRelatedLink
+        fields: Tuple[str, ...] = (
+            'url',
+            'id',
+            'title',
+            'uri',
+            'project',
+        )
+        extra_kwargs = {
+            'url': {'view_name': 'sphinx_hosting_api:projectrelatedlink-detail'},
+        }
+
+
 class VersionSerializer(serializers.HyperlinkedModelSerializer):
 
     project: RelatedField = serializers.HyperlinkedRelatedField(
         read_only=True,
         view_name='sphinx_hosting_api:project-detail'
     )
     head: RelatedField = serializers.HyperlinkedRelatedField(
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/api/urls.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/api/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import List, Union
 
-from django.urls import include, path, re_path, URLPattern, URLResolver
+from django.urls import include, path, URLPattern, URLResolver
 
 from drf_spectacular.views import (
     SpectacularAPIView,
     SpectacularRedocView,
     SpectacularSwaggerView
 )
 from rest_framework import routers
 
 from .views import (
     ClassifierViewSet,
     ProjectViewSet,
+    ProjectRelatedLinkViewSet,
     VersionViewSet,
     SphinxPageViewSet,
     SphinxImageViewSet,
     VersionUploadView
 )
 
 app_name: str = "sphinx_hosting_api"
@@ -23,14 +24,15 @@
 
 # Users
 router.register(r'classifiers', ClassifierViewSet)
 router.register(r'projects', ProjectViewSet)
 router.register(r'versions', VersionViewSet)
 router.register(r'pages', SphinxPageViewSet)
 router.register(r'images', SphinxImageViewSet)
+router.register(r'related-links', ProjectRelatedLinkViewSet)
 
 urlpatterns: List[Union[URLPattern, URLResolver]] = [
     path('', include(router.urls)),
     path('version/import/', VersionUploadView.as_view(), name='version-import'),
     path('schema/', SpectacularAPIView.as_view(), name='schema'),
     path(
         'schema/swagger-ui/',
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/fields.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/fields.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/fixtures/classifiers.json` & `django-sphinx-hosting-1.2.0/sphinx_hosting/fixtures/classifiers.json`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/forms.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/forms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Type
+from typing import Type, cast
 
 from crispy_forms.helper import FormHelper
 from crispy_forms.layout import Submit, Layout, Field, Fieldset, HTML, ButtonHolder
 
 from crispy_forms.bootstrap import FieldWithButtons
 from django import forms
 from django.db.models import Model
 from django.urls import reverse, reverse_lazy
 from haystack.forms import SearchForm
 
-from .models import Project
+from .models import Project, ProjectRelatedLink
 
 
 class GlobalSearchForm(SearchForm):
     """
     This is the search form at the top of the sidebar, underneath the logo.  It is
     a subclass of :py:class:`haystack.forms.SearchForm`, and does a search of our
     haystack backend.
@@ -164,14 +164,60 @@
                     'rows': 3,
                     'readonly': 'readonly',
                 }
             ),
         }
 
 
+class ProjectRelatedLinkBaseForm(forms.ModelForm):
+
+    def __init__(self, *args, project_machine_name: str = None, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.helper = FormHelper()
+        self.helper.form_class = 'form-horizontal'
+        self.helper.label_class = 'col-lg-3'
+        self.helper.field_class = 'col'
+        self.helper.form_method = 'post'
+        self.helper.layout = Layout(
+            Fieldset(
+                '',
+                Field('title'),
+                Field('uri'),
+            ),
+            ButtonHolder(
+                Submit('submit', 'Save', css_class='btn btn-primary'),
+                css_class='d-flex flex-row justify-content-end button-holder'
+            )
+        )
+
+    class Meta:
+        model: Type[Model] = ProjectRelatedLink
+        fields = (
+            'title',
+            'uri',
+        )
+
+
+class ProjectRelatedLinkCreateForm(ProjectRelatedLinkBaseForm):
+
+    def __init__(self, *args, project: Project = None, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.helper.form_action = reverse(
+            'sphinx_hosting:projectrelatedlink--create',
+            args=[cast(Project, project).machine_name]
+        )
+
+
+class ProjectRelatedLinkUpdateForm(ProjectRelatedLinkBaseForm):
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.helper.form_action = self.instance.get_update_url()
+
+
 class VersionUploadForm(forms.Form):
     """
     This is the form on :py:class:`sphinx_hosting.views.ProjectDetailView` that
     allows the user to upload a new documentation set.
 
     Keyword Args:
         project: the project to which this documentation set should be
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/importers.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/importers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from dataclasses import dataclass
 import io
 import json
 from pathlib import Path
 import re
 import tarfile
 from typing import Any, Dict, IO, List, Optional, cast
+import urllib.parse
+
 
 from django.utils.text import slugify
 import lxml.html
 from lxml.etree import XML  #: pylint: disable=no-name-in-module
 
 from .exc import VersionAlreadyExists
 from .logging import logger
@@ -275,14 +277,48 @@
         if 'title' not in data:
             # Some of the special pages don't have 'title' keys
             if 'indextitle' in data:
                 data['title'] = data['indextitle']
             else:
                 data['title'] = SphinxPage.SPECIAL_PAGES[path]
 
+    def _fix_link_hrefs(self, body: str) -> str:
+        """
+        Given an HTML body of a Sphinx page, update the ``<a href="path">``
+        references to be absolute.  If we don't do this, any links on the
+        index page the version will be relative to the index page, instead of
+        being relative to the root of the docs, and won't work.
+
+        Args:
+            body: the HTML body of a Sphinx document
+
+        Returns:
+            ``body`` with its ``<a>`` urls and updated
+        """
+        if not body:
+            return ''
+        html = lxml.html.fromstring(body)
+        links = html.cssselect('a.reference.internal')
+        for link in links:
+            href = link.attrib['href']
+            anchor = None
+            if '#' in href:
+                href, anchor = href.split('#')
+            if href.endswith('/'):
+                href = href[:-1]
+            href = re.sub('^(../)*', '', href)
+            link.attrib['href'] = "{{% url 'sphinx_hosting:sphinxpage--detail' project_slug='{}' version='{}' path='{}' %}}".format(
+                self.config['project'],
+                self.config['release'],
+                href
+            )
+            if anchor:
+                link.attrib['href'] += f'#{anchor}'
+        return lxml.html.tostring(html).decode('utf-8')
+
     def _fix_page_body(self, path: str, data: Dict[str, Any]) -> None:
         """
         Do any work needed to prepare the page body before inserting into the
         database.  This means
 
         * Ensure the ``body`` key exists in ``data``
         * Update the ``img`` sources to point to our Django storage location.
@@ -297,14 +333,18 @@
             # we create the SphinxPage, below
             data['body'] = ''
         data['orig_body'] = data['body']
         if data['body']:
             # Update the img src for any images in data['body'] for to point to our
             # Django storage locations
             data['body'] = self._update_image_src(data['body'])
+            # Update the hrefs for any <a> links to be absolute.  The relative
+            # paths we get from Sphinx end up being relative to the Sphinx index
+            # document instead of to the root of the docs
+            data['body'] = self._fix_link_hrefs(data['body'])
             html = lxml.html.fromstring(data['body'])
             # remove the first <h1> -- we'll display the page title another way
             first_h1 = html.cssselect('h1')
             if first_h1:
                 first_h1[0].getparent().remove(first_h1[0])
             # Fix our tables to look better
             tables = html.cssselect('table')
@@ -328,20 +368,18 @@
                 for div in table.cssselect('tbody > tr div.line'):
                     div.classes.discard('line')
                     div.classes.add('text-start')
                 for div in table.cssselect('tbody > tr p'):
                     div.classes.add('text-start')
             data['body'] = lxml.html.tostring(html).decode('utf-8')
             # Unescape our template tags after lxml has converted our {% %}
-            # to entities.  The pattern we're looking for looks something
-            # like this::
-            #
-            #     %7B%%20sphinximage_url%2026%20%%7D
-            html = re.sub(r'%7B%%20', r'{% ', data['body'])
-            data['body'] = re.sub(r'%20([0-9]+)%20%%7D', r' \1 %}', html)
+            # to entities.
+            tags = [m.group() for m in re.finditer(r'%7B%%20.*?%20%%7D', data['body'])]
+            for tag in tags:
+                data['body'] = data['body'].replace(tag, urllib.parse.unquote(tag))
             # Convert the weird paragraph symbols to actual paragraph symbols
             data['body'] = re.sub(r'#61633;', r'para;', data['body'])
 
     def _fix_toc(self, data: Dict[str, Any]) -> None:
         """
         Update our page's local table of contents (``data['toc']`) to have the CSS
         classes we need in order for it to display properly.
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/management/commands/import_docs.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/import_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         json/environment.pickle
         json/searchindex.json
         json/objects.inv
         ...
 
     """
     args = '<tarfile>'
-    help = ('Imports a tarfile of Sphinx documentation into a pre-existing project.')
+    help = 'Imports a tarfile of Sphinx documentation into a pre-existing project.'
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument(
             'tarfile',
             metavar='tarfile',
             type=str,
             help='The filename of the tarfile to import.'
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/management/commands/parse_globaltoc.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/parse_globaltoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class Command(BaseCommand):
     """
     **Usage**: ``./manage.py print_globaltoc <project_machine_name> <version number>``
 
     Print the global table of contents for a :py:class:`Version`.
     """
     args = '<project_machine_name> <version_number>'
-    help = ('Print the deduced page hierarchy for a version of a project.')
+    help = 'Print the deduced page hierarchy for a version of a project.'
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument(
             'project',
             metavar='project_machine_name',
             type=str,
             help='The machine_name of the project.'
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/management/commands/print_classifier_tree.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/print_classifier_tree.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/management/commands/print_doctree.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/management/commands/print_doctree.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 class Command(BaseCommand):
     """
     **Usage**: ``./manage.py print_doctree <project_machine_name> <version number>``
 
     Print the page tree for a :py:class:`Version`
     """
     args = '<tarfile>'
-    help = ('Print the deduced page hierarchy for a version of a project.')
+    help = 'Print the deduced page hierarchy for a version of a project.'
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument(
             'project',
             metavar='project_machine_name',
             type=str,
             help='The machine_name of the project.'
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0001_initial.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0002_original_html.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0002_original_html.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0003_globaltoc.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0003_globaltoc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0004_next_page_FK.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0004_next_page_FK.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0005_orig_global_toc.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0005_orig_global_toc.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0006_classifiers_and_permissiongroups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0007_load_classifiers.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0007_load_classifiers.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0009_SphinxPage_searchable.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0009_SphinxPage_searchable.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0010_add_groups.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0010_add_groups.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/migrations/0011_machinenamefield.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/migrations/0011_machinenamefield.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/models.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         if node.children:
             for child in node.children:
                 self.build(item['items'], child)
         items.append(item)
 
     def run(self, version: "Version") -> List[Dict[str, Any]]:
         """
-        Parse the :py:func:`Version.page_tree` and return a struct that looks like:
+        Parse the :py:func:`Version.page_tree` and return a struct that works
         with
         :py:class:`sphinx_hosting.wildewidgets.SphinxPageGlobalTableOfContentsMenu.parse_obj`
 
         The returned struct should look something like this::
 
             [
                 {'text': 'foo'},
@@ -398,20 +398,20 @@
             # This is really only necessary to get the pretty printer below to
             # work properly.  If the \n chars are not removed, lxml won't indent
             # properly
             global_toc_html = re.sub(r'\n', '', self.version.head.orig_global_toc)
             html = lxml.html.fromstring(global_toc_html)
             if verbose:
                 print(
-                    etree.tostring(
+                    etree.tostring(  # pylint: disable=c-extension-no-member
                         html,
                         method='xml',
                         encoding='unicode',
                         pretty_print=True
-                    )  # pylint: disable=c-extension-no-member
+                    )
                 )
             return self.parse_globaltoc(html)
         else:
             return []
 
 # --------------------------
 # FileField upload functions
@@ -961,7 +961,43 @@
         help_text=_('The actual image file')
     )
 
     class Meta:
         verbose_name = _('sphinx image')
         verbose_name_plural = _('sphinx images')
         unique_together = ('version', 'orig_path')
+
+
+class ProjectRelatedLink(TimeStampedModel, models.Model):
+    """
+    A ``ProjectRelatedLink`` is a link to an external resource that is related
+    to a :py:class:`Project`.
+    """
+
+    title: F = models.CharField(
+        'Link Title',
+        max_length=100,
+        help_text=_('The title for this link')
+    )
+    uri: F = models.URLField(
+        'Link URL',
+        max_length=256,
+        help_text=_('The URL for this link')
+    )
+    project: FK = models.ForeignKey(
+        Project,
+        on_delete=models.CASCADE,
+        related_name='related_links',
+        help_text=_('The project to which this link is related')
+    )
+
+    def get_update_url(self) -> str:
+        return reverse("sphinx_hosting:projectrelatedlink--update", kwargs={'pk': self.pk})
+
+    def get_delete_url(self) -> str:
+        return reverse("sphinx_hosting:projectrelatedlink--delete", kwargs={'pk': self.pk})
+
+    class Meta:
+        verbose_name = _('project related link')
+        verbose_name_plural = _('project related links')
+        unique_together = ('project', 'uri')
+        ordering = ('title',)
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/search_indexes.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/signals.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/signals.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss` & `django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/_classifierfilterblock.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss` & `django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/_pygments.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss` & `django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/_sphinx_layout.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css` & `django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.css`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss` & `django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/css/sphinx_hosting.scss`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/static/sphinx_hosting/images/logo.jpg` & `django-sphinx-hosting-1.2.0/sphinx_hosting/static/sphinx_hosting/images/logo.jpg`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/templates/sphinx_hosting/base.html` & `django-sphinx-hosting-1.2.0/sphinx_hosting/templates/sphinx_hosting/base.html`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/urls.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/urls.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     ClassifierViewSet,
     GlobalSphinxPageSearchView,
     ProjectCreateView,
     ProjectDeleteView,
     ProjectDetailView,
     ProjectListView,
     ProjectUpdateView,
+    ProjectRelatedLinkCreateView,
+    ProjectRelatedLinkUpdateView,
+    ProjectRelatedLinkDeleteView,
     SphinxPageDetailView,
     VersionDeleteView,
     VersionDetailView,
     VersionUploadView
 )
 from .wildewidgets import ProjectClassifierSelectorWidget
 
@@ -23,14 +26,29 @@
 urlpatterns: List[URLPattern] = [
     path('', ProjectListView.as_view(), name='project--list'),
     path('project/', ProjectCreateView.as_view(), name='project--create'),
     path('project/<str:slug>/', ProjectDetailView.as_view(), name='project--detail'),
     path('project/<str:slug>/update/', ProjectUpdateView.as_view(), name='project--update'),
     path('project/<str:slug>/upload/', VersionUploadView.as_view(), name='version--upload'),
     path('project/<str:slug>/delete/', ProjectDeleteView.as_view(), name='project--delete'),
+    path(
+        'project/<str:project_slug>/link/',
+        ProjectRelatedLinkCreateView.as_view(),
+        name='projectrelatedlink--create'
+    ),
+    path(
+        'project/link/<int:pk>/update/',
+        ProjectRelatedLinkUpdateView.as_view(),
+        name='projectrelatedlink--update'
+    ),
+    path(
+        'project/link/<int:pk>/delete/',
+        ProjectRelatedLinkDeleteView.as_view(),
+        name='projectrelatedlink--delete'
+    ),
     path('project/<str:project_slug>/<str:version>/', VersionDetailView.as_view(), name='version--detail'),
     path('project/<str:project_slug>/<str:version>/delete/', VersionDeleteView.as_view(), name='version--delete'),
     re_path(
         r'project/(?P<project_slug>[-a-zA-Z0-9_.]+)/(?P<version>[^/]+)/(?P<path>.*)/',
         SphinxPageDetailView.as_view(),
         name='sphinxpage--detail'
     ),
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/validators.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/validators.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.utils.regex_helper import _lazy_re_compile
 from django.utils.translation import gettext_lazy as _
 
 
 @deconstructible
 class NoHTMLValidator:
     """
-    Verify that field contains no HTML
+    Raises a ValidationError if the given value contains any HTML.
     """
     message: str = 'Cannot contain any HTML'
     code: str = 'invalid'
 
     def __call__(self, value: str) -> None:
         if not value == strip_tags(value):
             raise ValidationError(self.message, code=self.code)
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/views.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,19 +10,23 @@
     PermissionRequiredMixin,
 )
 from django.contrib import messages
 from django.contrib.auth.models import AbstractUser
 from django.core.files.storage import FileSystemStorage
 from django.db.models import Model, QuerySet
 from django.forms import ModelForm, Form
-from django.http import HttpResponse, HttpRequest
-from django.shortcuts import redirect
+from django.http import HttpResponse, HttpRequest, Http404
+from django.shortcuts import redirect, get_object_or_404
 from django.utils.translation import gettext as _
 from django.urls import reverse, reverse_lazy
-from django.views.generic.edit import BaseFormView
+from django.views.generic.edit import (
+    BaseFormView,
+    BaseCreateView,
+    BaseUpdateView
+)
 from django.views.generic import (
     CreateView,
     DeleteView,
     DetailView,
     TemplateView,
     UpdateView
 )
@@ -39,31 +43,37 @@
 )
 from wildewidgets.viewsets import ModelViewSet
 
 from .forms import (
     ProjectCreateForm,
     ProjectUpdateForm,
     ProjectReadonlyUpdateForm,
+    ProjectRelatedLinkCreateForm,
+    ProjectRelatedLinkUpdateForm,
     VersionUploadForm
 )
 from .importers import SphinxPackageImporter
 from .logging import logger
 from .models import (
     Classifier,
     Project,
+    ProjectRelatedLink,
     Version,
     SphinxPage
 )
 
 from .wildewidgets import (
     ProjectClassifierListWidget,
     ProjectClassifierSelectorWidget,
     ProjectCreateModalWidget,
     ProjectDetailWidget,
     ProjectInfoWidget,
+    ProjectRelatedLinkCreateModalWidget,
+    ProjectRelatedLinksWidget,
+    ProjectRelatedLinksListWidget,
     ProjectVersionsTableWidget,
     ProjectTableWidget,
     PagedSearchLayout,
     SphinxPageGlobalTableOfContentsMenu,
     SphinxHostingBreadcrumbs,
     SphinxHostingSidebar,
     SphinxPageLayout,
@@ -155,14 +165,15 @@
         layout.add_widget(ProjectInfoWidget(self.object))
         layout.add_widget(
             ProjectDetailWidget(
                 self.object,
                 form=ProjectReadonlyUpdateForm(instance=self.object)
             )
         )
+        layout.add_widget(ProjectRelatedLinksListWidget(queryset=self.object.related_links.all()))
         layout.add_widget(ProjectClassifierListWidget(queryset=self.object.classifiers.all()))
         layout.add_widget(ProjectVersionsTableWidget(project_id=self.object.pk))
         user = cast(AbstractUser, self.request.user)
         version = self.object.latest_version
         if version and version.head:
             layout.add_sidebar_link_button(
                 'Read Docs',
@@ -208,14 +219,24 @@
     form_class: Type[ModelForm] = ProjectCreateForm
 
     def get_form_valid_message(self) -> str:
         obj = cast(Project, self.object)
         return f'Added Project "{obj.title}"'
 
     def form_invalid(self, form: ModelForm) -> HttpResponse:
+        """
+        If the form is invalid, we want to display the errors to the user and
+        redirect them back to the project list page.
+
+        Args:
+            form: The form that was submitted
+
+        Returns:
+            The redirect response
+        """
         for k, errors in form.errors.as_data().items():
             for error in errors:
                 messages.error(self.request, f"{k}: {error.message}")
         return redirect('sphinx_hosting:project--list')
 
     def get_success_url(self) -> str:
         obj = cast(Project, self.object)
@@ -248,16 +269,18 @@
     form_class: Type[ModelForm] = ProjectUpdateForm
     slug_field: str = 'machine_name'
 
     def get_content(self) -> Widget:
         layout = WidgetListLayout(self.object.title)
         layout.add_widget(ProjectInfoWidget(self.object))
         layout.add_widget(ProjectDetailWidget(self.object))
+        layout.add_widget(ProjectRelatedLinksWidget(self.object))
         layout.add_widget(ProjectClassifierSelectorWidget(self.object))
         layout.add_widget(ProjectVersionsTableWidget(project_id=self.object.pk))
+        layout.add_widget(ProjectRelatedLinkCreateModalWidget(self.object))
         version = self.object.latest_version
         user = cast(AbstractUser, self.request.user)
         if version and version.head:
             layout.add_sidebar_link_button(
                 'Read Docs',
                 reverse(
                     'sphinx_hosting:sphinxpage--detail',
@@ -313,14 +336,106 @@
             self.object.machine_name,
             self.object.pk
         )
         return response
 
 
 # ===========================
+# ProjectRelatedLinks
+# ===========================
+
+class ProjectRelatedLinkCreateView(
+    LoginRequiredMixin,
+    PermissionRequiredMixin,
+    FormValidMessageMixin,
+    BaseCreateView
+):
+    form_class = ProjectRelatedLinkCreateForm
+    model: Type[Model] = ProjectRelatedLink
+    permission_required: str = 'sphinxhostingcore.change_project'
+
+    def get_form_kwargs(self) -> Dict[str, str]:
+        self.project: Project = get_object_or_404(Project, machine_name=self.kwargs['project_slug'])
+        kwargs = super().get_form_kwargs()
+        kwargs['project'] = self.project
+        return kwargs
+
+    def form_valid(self, form: Form) -> HttpResponse:
+        form.instance.project = self.project  # type: ignore
+        return super().form_valid(form)
+
+    def get_form_valid_message(self) -> str:
+        link = cast(ProjectRelatedLink, self.object)
+        return f'Created Related Link "{link.title}" for project "{link.project.machine_name}"'
+
+    def get_success_url(self) -> str:
+        link = cast(ProjectRelatedLink, self.object)
+        logger.info(
+            'project.relatedlink.create.success project=%s link_id=%s link_title=%s link_url=%s',
+            link.project.machine_name,
+            link.id,
+            link.title,
+            link.uri
+        )
+        return reverse('sphinx_hosting:project--update', args=[link.project.machine_name])
+
+
+class ProjectRelatedLinkUpdateView(
+    LoginRequiredMixin,
+    PermissionRequiredMixin,
+    FormValidMessageMixin,
+    BaseUpdateView
+):
+    form_class = ProjectRelatedLinkUpdateForm
+    model: Type[Model] = ProjectRelatedLink
+    permission_required: str = 'sphinxhostingcore.change_project'
+
+    def get_form_kwargs(self) -> Dict[str, str]:
+        kwargs = super().get_form_kwargs()
+        kwargs['project_machine_name'] = self.object.project.machine_name
+        return kwargs
+
+    def get_form_valid_message(self) -> str:
+        return f'Updated Related Link "{self.object.title}" for project "{self.object.project.machine_name}"'
+
+    def get_success_url(self) -> str:
+        logger.info(
+            'project.relatedlink.update.success project=%s link_id=%s link_title=%s link_url=%s',
+            self.object.project.machine_name,
+            self.object.id,
+            self.object.title,
+            self.object.uri
+        )
+        return reverse('sphinx_hosting:project--update', args=[self.object.project.machine_name])
+
+
+class ProjectRelatedLinkDeleteView(
+    LoginRequiredMixin,
+    PermissionRequiredMixin,
+    DeleteView
+):
+    model: Type[Model] = ProjectRelatedLink
+    permission_required: str = 'sphinxhostingcore.change_project'
+
+    def delete(self, request: HttpRequest, *args, **kwargs) -> HttpResponse:
+        response = super().delete(request, *args, **kwargs)
+        logger.info(
+            'project.relatedlink.delete.success project=%s link_id=%s link_title=%s link_url=%s',
+            self.object.project.machine_name,
+            self.object.id,
+            self.object.title,
+            self.object.uri
+        )
+        return response
+
+    def get_success_url(self) -> str:
+        return reverse('sphinx_hosting:project--update', args=[self.object.project.machine_name])
+
+
+# ===========================
 # Versions
 # ===========================
 
 
 class VersionDetailView(
     LoginRequiredMixin,
     WildewidgetsMixin,
@@ -335,14 +450,39 @@
 
     menu_item: str = "Projects"
 
     model: Type[Model] = Version
     slug_field: str = 'version'
     slug_url_kwarg: str = 'version'
 
+    def get_object(self, queryset: QuerySet = None) -> Version:
+        """
+        If ``version`` is ``latest``, return the latest version of the
+        :py:class:`sphinx_hosting.models.Project` whose ``machine_name`` is
+        ``project_slug``.  Otherwise, return the version identified by
+        ``version``.
+
+        Raises:
+            Http404: if the project has no versions, or the ``project_slug`` does
+                not match any :py:class:`sphinx_hosting.models.Project` objects.
+
+        Returns:
+            The latest version of the project identified by ``project_slug``
+        """
+        if queryset is None:
+            queryset = self.get_queryset()
+        if self.kwargs['version'] == 'latest':
+            project_slug = self.kwargs.get('project_slug', None)
+            project = get_object_or_404(Project, machine_name=project_slug)
+            version = project.latest_version
+            if not version:
+                raise Http404(f'Project "{project_slug}" has no versions')
+            return version
+        return super().get_object(queryset=queryset)
+
     def get_queryset(self) -> QuerySet[Version]:
         """
         Pre-filter our default queryset so that we only are able to get
         :py:class:`sphinx_hosting.models.Version` objects associated with the
         :py:class:`sphinx_hosting.models.Project` identified by our
         ``project_slug`` URLPath kwarg.
 
@@ -498,41 +638,55 @@
 
     model: Type[Model] = SphinxPage
     slug_field: str = 'relative_path'
     slug_url_kwarg: str = 'path'
 
     def get_navbar(self) -> Navbar:
         navbar = super().get_navbar()
-        globaltoc = SphinxPageGlobalTableOfContentsMenu.parse_obj(self.object.version.globaltoc)
+        globaltoc = SphinxPageGlobalTableOfContentsMenu.parse_obj(self.object.version)
         globaltoc.title = self.object.version.project.title
         navbar.add_to_menu_section(globaltoc)
         return navbar
 
     def get_menu_item(self) -> str:
         return self.request.path
 
     def get_queryset(self) -> QuerySet[SphinxPage]:
         """
         Pre-filter our default queryset so that we only are able to get
         :py:class:`sphinx_hosting.models.SphinxPage` objects associated with the
         :py:class:`sphinx_hosting.models.Version` identified by our ``project_slug``
-        and ``version`` URLPath kwargs:
+        and ``version`` URLPath kwargs.
+
+        If ``version`` is ``latest``, return the latest version of the
+        :py:class:`sphinx_hosting.models.Project`.
 
         Parameters:
             project_slug: the :py:attr:`sphinx_hosting.models.Project.machine_name`
                 of our project
             version: the :py:attr:`sphinx_hosting.models.Version.version` string
                 of our version
 
+        Raises:
+            Http404: if ``version`` is ``latest`` and the project has no
+                versions, or the ``project_slug`` does not match any
+                :py:class:`sphinx_hosting.models.Project` objects.
+
         Returns:
             A queryset of ``SphinxPage`` objects filtered to a particular version of
             a particular project.
         """
         project_slug = self.kwargs.get('project_slug', None)
         version = self.kwargs.get('version', None)
+        if version == 'latest':
+            project = get_object_or_404(Project, machine_name=project_slug)
+            version_obj = project.latest_version
+            if not version_obj:
+                raise Http404(f'Project "{project_slug}" has no versions')
+            version = version_obj.version
         return super().get_queryset().filter(
             version__version=version,
             version__project__machine_name=project_slug
         )
 
     def get_content(self) -> Widget:
         return SphinxPageLayout(self.object)
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/classifier.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/classifier.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/navigation.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/navigation.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/project.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/project.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,38 @@
 
 from django.contrib.auth.models import AbstractUser
 from django.db.models import Model, QuerySet
 from wildewidgets import (
     ActionButtonModelTable,
     BasicModelTable,
     Block,
+    CardWidget,
     CrispyFormModalWidget,
     CrispyFormWidget,
-    CardWidget,
     Datagrid,
+    HorizontalLayoutBlock,
+    Link,
+    FormButton,
     ListModelWidget,
+    ModalButton,
     RowActionButton,
     RowEditButton,
     RowModelUrlButton,
     ToggleableManyToManyFieldBlock,
     TwoColumnLayout,
     Widget,
     WidgetListLayoutHeader,
 )
 
-from ..forms import ProjectCreateForm
-from ..models import Classifier, Project, Version
+from ..forms import (
+    ProjectCreateForm,
+    ProjectRelatedLinkCreateForm,
+    ProjectRelatedLinkUpdateForm,
+)
+from ..models import Classifier, Project, Version, ProjectRelatedLink
 
 from .classifier import ClassifierFilterBlock
 
 
 #------------------------------------------------------
 # Modals
 #------------------------------------------------------
@@ -40,14 +48,47 @@
     modal_title: str = "Add Project"
 
     def __init__(self, *args, **kwargs):
         form = ProjectCreateForm()
         super().__init__(form=form, *args, **kwargs)
 
 
+class ProjectRelatedLinkCreateModalWidget(CrispyFormModalWidget):
+    """
+    This is a modal dialog that holds the
+    :py:class:`sphinx_hosting.forms.ProjectRelatedLinkForm` for
+    creating links.
+    """
+
+    modal_id: str = "projectrelatedlink__create"
+    modal_title: str = "Add Related Link"
+
+    def __init__(self, project: Project, *args, **kwargs):
+        form = ProjectRelatedLinkCreateForm(project=project)
+        super().__init__(form=form, *args, **kwargs)
+
+
+class ProjectRelatedLinkUpdateModalWidget(CrispyFormModalWidget):
+    """
+    This is a modal dialog that holds the
+    :py:class:`sphinx_hosting.forms.ProjectRelatedLinkForm` for
+    updating links.
+
+    One of these is created for each
+    :py:class:`sphinx_hosting.models.ProjectRelatedLink` object, and lives in
+    the :py:class:`sphinx_hosting.widgets.ProjectRelatedLinksWidget`.
+    """
+
+    modal_title: str = "Update Related Link"
+
+    def __init__(self, link: ProjectRelatedLink, *args, **kwargs):
+        form = ProjectRelatedLinkUpdateForm(instance=link)
+        super().__init__(form=form, *args, **kwargs)
+
+
 #------------------------------------------------------
 # Project related widgets
 #------------------------------------------------------
 
 class ProjectInfoWidget(CardWidget):
     """
     This is a :py:class:`wildewidgets.CardWidget` containing a Tabler datagrid
@@ -83,15 +124,15 @@
             ClassifierFilterBlock(
                 table_name=table.table_name,
                 column_number=table.get_column_number('classifiers')
             )
         )
         self.add_block(layout)
 
-    def get_title(self, user: AbstractUser) -> WidgetListLayoutHeader:
+    def get_title(self, user: AbstractUser) -> WidgetListLayoutHeader:  # pylint: disable=arguments-differ
         header = WidgetListLayoutHeader(
             header_text="Projects",
             badge_text=Project.objects.count(),
         )
         if user.has_perm('sphinxhostingcore.add_project'):
             header.add_modal_button(
                 text="New Project",
@@ -167,14 +208,82 @@
     name: str = 'project-detail__section'
     modifier: str = 'general'
     icon: str = "card-checklist"
     css_class: str = CrispyFormWidget.css_class + " p-4"
 
 
 #------------------------------------------------------
+# ProjectRelatedLink related widgets
+#------------------------------------------------------
+
+class ProjectRelatedLinkListItemWidget(HorizontalLayoutBlock):
+
+    def __init__(self, object: ProjectRelatedLink):  # pylint: disable=redefined-builtin
+        modal_id = f"projectrelatedlink__update__{object.pk}"
+        super().__init__(
+            Link(object.title, url=object.uri, title=object.title),
+            Block(
+                ModalButton(text='Edit', color="azure", target=f'#{modal_id}'),
+                FormButton(
+                    text='Delete',
+                    color="outline-secondary",
+                    css_class="d-inline",
+                    action=object.get_delete_url(),
+                    confirm_text="Are you sure you want to delete this link?",
+                ),
+            ),
+            ProjectRelatedLinkUpdateModalWidget(object, modal_id=modal_id),
+        )
+
+
+class ProjectRelatedLinksWidget(CardWidget):
+    """
+    This is a :py:class:`wildewidgets.CardWidget` that allows us to
+    manage the :py:class:`sphinx_hosting.models.ProjectRelatedLink` objects
+    for this :py:class:`sphinx_hosting.models.Project`.
+    """
+
+    title: str = "Related Links"
+    icon: str = "box-arrow-up-right"
+
+    def __init__(self, project: Project, **kwargs):
+        self.project = project
+        super().__init__(
+            widget=ListModelWidget(
+                queryset=self.project.related_links,
+                model_widget=ProjectRelatedLinkListItemWidget,
+            ),
+            **kwargs,
+        )
+
+    def get_title(self) -> WidgetListLayoutHeader:
+        header = WidgetListLayoutHeader(
+            header_text="Related Links",
+            badge_text=self.project.related_links.count(),
+        )
+        header.add_modal_button(
+            text="Add Related Link",
+            color="primary",
+            target=f'#{ProjectRelatedLinkCreateModalWidget.modal_id}'
+        )
+        return header
+
+
+class ProjectRelatedLinksListWidget(ListModelWidget):
+
+    paginate_by: int = 100
+    item_label: str = 'Related Link'
+    title: str = 'Related Links'
+    icon: str = "external-link"
+
+    def get_model_subblock(self, instance: ProjectRelatedLink) -> Block:
+        return Link(instance.title, url=instance.uri)
+
+
+#------------------------------------------------------
 # Datatables
 #------------------------------------------------------
 
 class LatestVersionButton(RowModelUrlButton):
 
     attribute: str = 'get_latest_version_url'
     text: str = 'Read Docs'
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/search.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/search.py`

 * *Files identical despite different names*

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/sphinx_page.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/sphinx_page.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     HTMLWidget,
     LinkButton,
     Menu,
     MenuItem,
     Row,
     TwoColumnLayout
 )
-from ..models import SphinxPage
+from ..models import SphinxPage, Version
 
 
 #------------------------------------------------------
 # SphinxPage related widgets
 #------------------------------------------------------
 
 class SphinxPagePagination(Row):
@@ -115,34 +115,65 @@
     that version.
     """
 
     css_class: str = 'mt-4'
     title_css_classes: str = 'mt-3'
 
     @classmethod
-    def parse_obj(cls, data: Dict[str, Any]) -> "SphinxPageGlobalTableOfContentsMenu":
+    def parse_obj(cls, version: Version) -> "SphinxPageGlobalTableOfContentsMenu":
         """
-        Given a dict like this::
+        Parse the globaltoc of a :py:class:`sphinx_hosting.models.Version` into
+        a :py:class:`wildewidgets.Menu` suitable for insertion into a
+        :py:class:`wildewidgets.Navbar`
+
+        The :py:attr:`sphinx_hosting.models.Version.globaltoc` is a dict that
+        looks like this::
 
             {
                 items: [
                     {'text': 'foo'},
                     {'text': 'bar', 'url': '/foo', 'icon': 'blah'}
                     {'text': 'bar', 'url': '/foo', 'icon': 'blah', items: [{'text': 'blah' ...} ...]}
                     ...
                 ]
             }
 
-        Return a fully configured :py:class:`SphinxPageGlobalTableOfContentsMenu` suitable
-        for insertion into a :py:class:`wildewidgets.Navbar`.
+        Args:
+            version: the ``Version`` for which we are building the menu
 
         Returns:
             A configured  ``SphinxPageGlobalTableOfContentsMenu``.
         """
+        data = version.globaltoc
         menu_items = cls._load_menuitems(data['items'])
+        if version.project.related_links.exists():
+            link_items: List[MenuItem] = [MenuItem(text="Related Links")]
+            for link in version.project.related_links.all():
+                link_items.append(MenuItem(text=link.title, url=link.uri, icon="link"))
+            if len(menu_items) == 1:
+                # There's only a single page in this version, so we can
+                # just extend the list of menu items with the link items
+                menu_items.extend(link_items)
+            else:
+                if (
+                    menu_items[1].url is not None and
+                    menu_items[1].items is not None
+                ):
+                    # Insert a "Content" heading after the "Home" link
+                    # to separate it from the links
+                    menu_items.insert(1, MenuItem(text="Content"))
+                link_items.reverse()
+                for item in link_items:
+                    menu_items.insert(1, item)
+        if menu_items[0].text != 'Home':
+            # Let's be consistent about naming the top page of the
+            # version "Home".  The globaltoc adds a Home link if there
+            # isn't one, but those without globaltoc will have their
+            # top page named after the project.
+            menu_items[0].text = 'Home'
         return cls(*menu_items)
 
     @classmethod
     def _load_menuitems(cls, items: List[Dict[str, Any]]) -> List[MenuItem]:
         """
         Given a list like this::
```

### Comparing `django-sphinx-hosting-1.1.5/sphinx_hosting/wildewidgets/version.py` & `django-sphinx-hosting-1.2.0/sphinx_hosting/wildewidgets/version.py`

 * *Files identical despite different names*

