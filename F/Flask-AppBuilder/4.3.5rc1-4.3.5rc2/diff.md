# Comparing `tmp/Flask-AppBuilder-4.3.5rc1.tar.gz` & `tmp/Flask-AppBuilder-4.3.5rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-AppBuilder-4.3.5rc1.tar", last modified: Thu Jul 27 10:48:05 2023, max compression
+gzip compressed data, was "Flask-AppBuilder-4.3.5rc2.tar", last modified: Thu Jul 27 11:08:06 2023, max compression
```

## Comparing `Flask-AppBuilder-4.3.5rc1.tar` & `Flask-AppBuilder-4.3.5rc2.tar`

### file list

```diff
@@ -1,1182 +1,1182 @@
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.923703 Flask-AppBuilder-4.3.5rc1/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       97 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/.coveragerc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      113 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/.env
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.903297 Flask-AppBuilder-4.3.5rc1/.github/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      642 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)      681 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)      202 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/.github/prlint.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)      709 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/.github/stale.yml
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.905388 Flask-AppBuilder-4.3.5rc1/.github/workflows/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8119 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/.github/workflows/ci.yml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      137 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/.github/workflows/odbcinst.ini
--rw-r--r--   0 dpgaspar   (501) staff       (20)      951 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/.github/workflows/ptlint.yml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      147 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)    64876 2023-07-27 10:40:19.000000 Flask-AppBuilder-4.3.5rc1/CHANGELOG.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1894 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/CONTRIBUTING.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.909886 Flask-AppBuilder-4.3.5rc1/Flask_AppBuilder.egg-info/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9315 2023-07-27 10:48:04.000000 Flask-AppBuilder-4.3.5rc1/Flask_AppBuilder.egg-info/PKG-INFO
--rw-r--r--   0 dpgaspar   (501) staff       (20)    36154 2023-07-27 10:48:04.000000 Flask-AppBuilder-4.3.5rc1/Flask_AppBuilder.egg-info/SOURCES.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2023-07-27 10:48:04.000000 Flask-AppBuilder-4.3.5rc1/Flask_AppBuilder.egg-info/dependency_links.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)      110 2023-07-27 10:48:04.000000 Flask-AppBuilder-4.3.5rc1/Flask_AppBuilder.egg-info/entry_points.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-12 08:40:39.000000 Flask-AppBuilder-4.3.5rc1/Flask_AppBuilder.egg-info/not-zip-safe
--rw-r--r--   0 dpgaspar   (501) staff       (20)      559 2023-07-27 10:48:04.000000 Flask-AppBuilder-4.3.5rc1/Flask_AppBuilder.egg-info/requires.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)       17 2023-07-27 10:48:04.000000 Flask-AppBuilder-4.3.5rc1/Flask_AppBuilder.egg-info/top_level.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1493 2023-04-05 15:10:33.000000 Flask-AppBuilder-4.3.5rc1/LICENSE
--rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/MANIFEST.in
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9315 2023-07-27 10:48:05.923855 Flask-AppBuilder-4.3.5rc1/PKG-INFO
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6684 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/README.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/RELEASE.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.911130 Flask-AppBuilder-4.3.5rc1/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    36590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/babel/messages.pot
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.900539 Flask-AppBuilder-4.3.5rc1/bin/
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      176 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/bin/babel_extract.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/bin/babel_init.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      422 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/bin/bootswatch_update.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1632 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/bin/config.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/bin/db_create.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      840 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/bin/db_migrate.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/bin/db_upgrade.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1419 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/bin/hash_db_password.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/bin/migrate_db_0.7.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     4001 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/bin/migrate_db_1.3.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1917 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/bin/sqlite_upgrade_1.3.sql
--rw-r--r--   0 dpgaspar   (501) staff       (20)      999 2023-05-24 14:03:04.000000 Flask-AppBuilder-4.3.5rc1/docker-compose.yml
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.933151 Flask-AppBuilder-4.3.5rc1/docs/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6802 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/Makefile
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.933778 Flask-AppBuilder-4.3.5rc1/docs/_static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_static/Flask-AppBuilder.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.934663 Flask-AppBuilder-4.3.5rc1/docs/_templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_templates/layout.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.936494 Flask-AppBuilder-4.3.5rc1/docs/_themes/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_themes/LICENSE
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1093 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_themes/README
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.938492 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      954 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask/layout.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask/relations.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.939880 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask/static/Flask-AppBuilder.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9062 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask/static/flasky.css_t
--rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask/theme.conf
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.941146 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask_small/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      683 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask_small/layout.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.941747 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask_small/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask_small/static/flasky.css_t
--rw-r--r--   0 dpgaspar   (501) staff       (20)      184 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask_small/theme.conf
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4875 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/_themes/flask_theme_support.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2277 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/actions.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3828 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/addons.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10881 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.5rc1/docs/advanced.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/api.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/cli.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8834 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/conf.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    33485 2023-06-19 07:52:15.000000 Flask-AppBuilder-4.3.5rc1/docs/config.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10806 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/customizing.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4109 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/diagrams.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/generic_datasource.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3817 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/docs/i18n.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.962115 Flask-AppBuilder-4.3.5rc1/docs/images/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/ListThumbnail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/chart_time1.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/chart_time2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/charts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/contact_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/contacts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/direct_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/fab.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/group_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/grouped_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/groups.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/images_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/list_cascade.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/list_cascade_block.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/list_compact_inline.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/list_master_detail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/login_db.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/login_oid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    82437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/oauth_login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    48690 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/oauth_login_one_provider.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    42827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/security.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/simpleview2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/swagger001.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26185 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/images/swagger002.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1389 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/docs/index.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4377 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.5rc1/docs/installation.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2634 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/intro.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6721 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/make.bat
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/multipledbs.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/quickcharts.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/quickfiles.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/quickhowto.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4829 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/quickhowto_mongo.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1676 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/quickminimal.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8990 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/relations.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    47345 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.5rc1/docs/rest_api.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    36706 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/docs/security.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17032 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/templates.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4335 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/user_registration.rst
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    12302 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/versionmigration.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/docs/views.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.962779 Flask-AppBuilder-4.3.5rc1/examples/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.964015 Flask-AppBuilder-4.3.5rc1/examples/base_api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/base_api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.965219 Flask-AppBuilder-4.3.5rc1/examples/base_api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      380 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/base_api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/base_api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1809 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/base_api/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.968348 Flask-AppBuilder-4.3.5rc1/examples/basefilter/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/basefilter/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      429 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/basefilter/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.970254 Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1458 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.842288 Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.842341 Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.971505 Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1413 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.973358 Flask-AppBuilder-4.3.5rc1/examples/basefilter/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/basefilter/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/basefilter/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/basefilter/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/basefilter/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2423 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/basefilter/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.975353 Flask-AppBuilder-4.3.5rc1/examples/composite_keys/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      254 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/composite_keys/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.977317 Flask-AppBuilder-4.3.5rc1/examples/composite_keys/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/composite_keys/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/composite_keys/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/composite_keys/app/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2182 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/composite_keys/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1477 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/composite_keys/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.980439 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.982649 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2061 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1804 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.842873 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.842919 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.984174 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.985699 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2460 2023-07-10 13:44:00.000000 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.987649 Flask-AppBuilder-4.3.5rc1/examples/dash/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      291 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/dash/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.988964 Flask-AppBuilder-4.3.5rc1/examples/dash/app/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.991506 Flask-AppBuilder-4.3.5rc1/examples/dash/app/Dashboard/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      797 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/dash/app/Dashboard/Dash_App1.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/dash/app/Dashboard/Dash_App2.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1568 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/dash/app/Dashboard/Dash_fun.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/dash/app/Dashboard/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/dash/app/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.992079 Flask-AppBuilder-4.3.5rc1/examples/dash/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      701 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/dash/app/templates/dash.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1031 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/dash/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.993357 Flask-AppBuilder-4.3.5rc1/examples/dash/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/dash/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/dash/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/dash/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/dash/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.994580 Flask-AppBuilder-4.3.5rc1/examples/employees/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      276 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/employees/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.997072 Flask-AppBuilder-4.3.5rc1/examples/employees/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/employees/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/employees/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/employees/app/security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1972 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.5rc1/examples/employees/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.997814 Flask-AppBuilder-4.3.5rc1/examples/employees/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/employees/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/employees/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.000539 Flask-AppBuilder-4.3.5rc1/examples/enums/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/enums/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/enums/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.002395 Flask-AppBuilder-4.3.5rc1/examples/enums/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/enums/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1158 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/enums/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.843857 Flask-AppBuilder-4.3.5rc1/examples/enums/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.843904 Flask-AppBuilder-4.3.5rc1/examples/enums/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.003717 Flask-AppBuilder-4.3.5rc1/examples/enums/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3436 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/enums/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.005004 Flask-AppBuilder-4.3.5rc1/examples/enums/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/enums/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/enums/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/enums/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1841 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/enums/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.008139 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.012175 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2607 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/sec_forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1923 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.844251 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.844308 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.013412 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1589 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.015266 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1961 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2977 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.018011 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      560 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.021772 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2831 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/sec_forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1929 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.844639 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.844686 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.023002 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2133 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.024204 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.028372 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      432 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.031269 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.845032 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.845077 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.033512 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2121 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.036682 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1904 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/config2.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1867 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/examples/factoryapp/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.038980 Flask-AppBuilder-4.3.5rc1/examples/issue_789/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1610 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/issue_789/README.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4740 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/issue_789/app.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.042686 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/NAMES.DIC
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.046555 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1164 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.845495 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.845543 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.048778 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.052005 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/masterdetail/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.056678 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.060964 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/mysecurity.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.845873 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.845920 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.064836 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2988 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.069863 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.076011 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.079186 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.846251 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.846299 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.081294 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2623 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.084464 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoengine/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.089994 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      296 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.093352 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2732 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.846621 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.846665 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.095689 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4050 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.098924 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/mongoimages/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.103328 Flask-AppBuilder-4.3.5rc1/examples/oauth/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/oauth/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)      531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/oauth/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.108782 Flask-AppBuilder-4.3.5rc1/examples/oauth/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      743 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/oauth/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      399 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/oauth/app/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/oauth/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/examples/oauth/app/security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2395 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/examples/oauth/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.110925 Flask-AppBuilder-4.3.5rc1/examples/oauth/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/oauth/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/oauth/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8905 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/examples/oauth/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/oauth/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.114197 Flask-AppBuilder-4.3.5rc1/examples/productsale/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      192 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/productsale/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.117324 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1755 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.847476 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.847398 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.119485 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.847526 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.121717 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1304 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/productsale/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.122849 Flask-AppBuilder-4.3.5rc1/examples/productsale/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/productsale/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/productsale/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/productsale/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.126246 Flask-AppBuilder-4.3.5rc1/examples/quickactions/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.129392 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      554 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      263 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.847978 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.847907 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.131428 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.848025 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.133499 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1067 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.134555 Flask-AppBuilder-4.3.5rc1/examples/quickactions/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickactions/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1945 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickactions/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickactions/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      279 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickactions/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.136602 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.140985 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1646 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/data.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.848349 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.848401 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.143098 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2928 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.146870 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1775 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.150766 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.156597 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      352 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.848875 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.848953 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.160730 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5034 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.166734 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/babel/messages.pot~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.849467 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.849315 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/bdist.linux-i686/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.849371 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/bdist.linux-i686/egg/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.173246 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.849528 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/lib/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.179353 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/lib/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/lib/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/lib/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/lib/app/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1726 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.185323 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      225 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.191204 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1188 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.193142 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.849906 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.199314 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16804 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.850032 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.205622 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16794 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1395 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.209664 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1795 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickfiles/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.219249 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.230711 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-07-29 16:17:15.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.850396 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.850444 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.238444 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3166 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.249666 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2758 2023-07-10 14:06:44.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.264922 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/NAMES.DIC
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.294669 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      556 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      105 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/indexview.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3024 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      300 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/sec_models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2047 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.851017 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.335636 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abBtnAdd.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      171 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abBtnDelete.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abBtnEdit.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      179 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abBtnShow.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abDate.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abMenuPageSize.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      548 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1633 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abModelSearch.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2033 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abModelTable.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abPagination.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abSelect.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.343214 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7059 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/css/clean-blog.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1446 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/css/scrolling-nav.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.350602 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/img/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      783 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/img/brand.jpg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3208 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/img/loading.gif
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.365874 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.376922 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Controllers/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1781 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      240 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Controllers/searchCtrl.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.384409 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Directives/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3764 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Directives/bigDirectives.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9587 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Directives/btnDirectives.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.388141 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Services/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2825 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Services/apiService.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)   125321 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/angular.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/app.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17294 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/clean-blog.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      612 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/scrolling-nav.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.423389 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.430519 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/appbuilder/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/list_angulajs.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      332 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/list_contacts.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/list_json.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      199 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/mylist.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/new_base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      371 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/show_contacts.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.444884 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2549 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/widgets/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      280 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/widgets/list_override.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.851673 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.851731 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.459261 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2511 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.480787 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2387 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2327 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1533 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.531662 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    92965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/.coverage
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      220 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.553418 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      753 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.852139 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.852199 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.567687 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.589240 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1942 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/migrate_db_0.7.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1397 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.603896 Flask-AppBuilder-4.3.5rc1/examples/quickimages/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickimages/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.626532 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2636 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.852753 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.852655 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.641848 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.852810 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.657002 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4155 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.664471 Flask-AppBuilder-4.3.5rc1/examples/quickimages/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickimages/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1704 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickimages/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.677669 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.678639 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      418 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.853183 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.853229 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.679282 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3627 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.679966 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.680213 Flask-AppBuilder-4.3.5rc1/examples/quickminimal/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      430 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quickminimal/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.682832 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.683987 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/.idea/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      159 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/.idea/encodings.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      679 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/.idea/misc.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      278 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/.idea/modules.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/.idea/quicksqlviews.iml
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1846 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/.idea/workspace.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.685337 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.853716 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.853768 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.685877 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.686324 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.687713 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.690793 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      386 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.854126 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.691048 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/static/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2891 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/static/css/landing-page.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.691255 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3347 2023-07-27 10:30:58.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/templates/mybase.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.854319 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.854366 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.691798 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3658 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.694949 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.696649 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.697744 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1553 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.705206 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       66 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/.babelrc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      398 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/README.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)   838924 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/package-lock.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3522 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/package.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)      746 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/package.json.react-original
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.706069 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/public/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/public/favicon.ico
--rw-r--r--   0 dpgaspar   (501) staff       (20)      283 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/public/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/public/manifest.json
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.706566 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      375 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/App.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.706822 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      959 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/api/Api.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.707497 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/components/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3602 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/components/CRUDButtons.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4478 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/components/Forms.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15937 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/components/Table.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      349 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/index.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      285 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/webpack.config.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.707932 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      856 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/templates/base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/templates/react.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.855141 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.855186 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.708327 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.708719 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2462 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.710524 Flask-AppBuilder-4.3.5rc1/examples/related_fields/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/related_fields/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      221 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/related_fields/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.711194 Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.855535 Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.855595 Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.711692 Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5713 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.712122 Flask-AppBuilder-4.3.5rc1/examples/related_fields/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/related_fields/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/related_fields/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/related_fields/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/related_fields/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2739 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/related_fields/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.712842 Flask-AppBuilder-4.3.5rc1/examples/simpleform/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleform/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)      286 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleform/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.713367 Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      507 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/forms.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.713569 Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/templates/404.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.856007 Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.856056 Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.714061 Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)      940 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.714553 Flask-AppBuilder-4.3.5rc1/examples/simpleform/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleform/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      662 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleform/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3697 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleform/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleform/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.715248 Flask-AppBuilder-4.3.5rc1/examples/simpleview1/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      173 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview1/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.715639 Flask-AppBuilder-4.3.5rc1/examples/simpleview1/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview1/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      601 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview1/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.716062 Flask-AppBuilder-4.3.5rc1/examples/simpleview1/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview1/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview1/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview1/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview1/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.716511 Flask-AppBuilder-4.3.5rc1/examples/simpleview2/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.716922 Flask-AppBuilder-4.3.5rc1/examples/simpleview2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      381 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview2/app/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.721764 Flask-AppBuilder-4.3.5rc1/examples/simpleview2/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      108 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview2/app/templates/method3.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1198 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.722232 Flask-AppBuilder-4.3.5rc1/examples/simpleview2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/simpleview2/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.723917 Flask-AppBuilder-4.3.5rc1/examples/user_registration/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      267 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.726738 Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1639 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.856902 Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.856949 Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.727555 Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3965 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.728339 Flask-AppBuilder-4.3.5rc1/examples/user_registration/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/user_registration/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.731933 Flask-AppBuilder-4.3.5rc1/examples/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      229 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.732459 Flask-AppBuilder-4.3.5rc1/examples/widgets/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.857383 Flask-AppBuilder-4.3.5rc1/examples/widgets/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.857458 Flask-AppBuilder-4.3.5rc1/examples/widgets/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.732880 Flask-AppBuilder-4.3.5rc1/examples/widgets/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4839 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.735862 Flask-AppBuilder-4.3.5rc1/examples/widgets/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1491 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/examples/widgets/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.745421 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2023-07-27 10:39:18.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1970 2023-06-30 15:17:51.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/_compat.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1233 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/actions.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.746599 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    76068 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/api/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9871 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/api/convert.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3368 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/api/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/api/schemas.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.747315 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/babel/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2311 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/babel/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/babel/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26023 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      346 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/basemanager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    48967 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/baseviews.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.752834 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/charts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/charts/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/charts/jsontools.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17665 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/charts/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/charts/widgets.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14981 2023-05-05 08:39:47.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/cli.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14159 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/console.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8403 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/const.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1138 2022-09-30 13:30:31.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/exceptions.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8785 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/fields.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5984 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/fieldwidgets.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8534 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/filemanager.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     6206 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11129 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3131 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/hooks.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7648 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/menu.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      290 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/messages.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.754214 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9580 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      846 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/decorators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10374 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/filters.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.754771 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/generic/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13059 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/generic/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/generic/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/generic/interface.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10970 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/group.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2633 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/mixins.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.755523 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1765 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/mongoengine/fields.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4184 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/mongoengine/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9982 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/mongoengine/interface.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.756239 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4145 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/sqla/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11046 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/sqla/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39115 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/sqla/interface.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.758616 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5220 2023-05-08 09:55:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10558 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/decorators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4162 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    76822 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/manager.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.759087 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15303 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/mongoengine/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3219 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/mongoengine/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10630 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/registerviews.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1359 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/schemas.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.759561 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.759739 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.760327 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/permission/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       45 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/permission/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      624 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/permission/api.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.760732 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       53 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      647 2023-07-10 13:48:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.761595 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/role/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/role/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5053 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/role/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      390 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/role/schema.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.762427 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/user/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/user/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6695 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/user/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2481 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/user/schema.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1100 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/user/validator.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.762826 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/view_menu/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       43 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/view_menu/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      569 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/view_menu/api.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    26664 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/manager.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     5260 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/utils.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    25706 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.859967 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.861034 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.763348 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/ab.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121457 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/bootstrap.min.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.764245 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/flags/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/flags/flags16.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.765834 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18600 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    80761 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)      586 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)      578 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1760 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    27593 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.783190 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   105250 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/amelia.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120090 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/cerulean.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   119768 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/cosmo.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   119799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/cyborg.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121625 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/darkly.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121354 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/flatly.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118666 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/journal.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   124431 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/lumen.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   132318 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/paper.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118678 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/readable.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/sandstone.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/simplex.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   129014 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/slate.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   125030 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/solar.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/spacelab.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120731 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/superhero.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   117016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/united.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121865 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/yeti.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.783734 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/datepicker/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.785265 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/fonts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20127 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 dpgaspar   (501) staff       (20)   108738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    45404 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)    23424 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18028 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.789174 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/aol.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/fab.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.789393 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/flags/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/flags/flags16.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/flickr.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8777 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    12799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2558 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/google.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2882 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/myopenid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/yahoo.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.797080 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3321 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/ab.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4228 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/ab_actions.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5176 2023-07-10 14:06:29.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/ab_filters.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1526 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39680 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/bootstrap.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    46151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/google_charts.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    89501 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/jquery-latest.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    27347 2023-01-10 15:34:59.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/v4-shims.min.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.801790 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16792 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1849 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17358 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/select2.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    79212 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/select2.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/select2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)      845 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/select2x2.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.811124 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   186124 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)   107656 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)    62320 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)    25236 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)   397420 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)   150516 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10140 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4568 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.861163 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.818706 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/_formhelpers.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)       28 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      874 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/baselayout.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4588 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/baselib.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      486 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/flash.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      143 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/footer.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.819252 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/alert.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.824426 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/charts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      778 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/charts/chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      890 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      717 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/confirm.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14587 2023-07-27 10:30:58.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/lib.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.830708 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/add.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1181 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/edit.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      813 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      653 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      496 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      517 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      501 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/search.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1207 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      784 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.836953 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/activation.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2949 2023-01-10 15:41:47.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/login_db.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1996 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6568 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/login_oid.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      230 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/register_mail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1057 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.845564 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1153 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2981 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2613 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/form.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1326 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1328 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/group_form_list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2745 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1331 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2038 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2843 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      572 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1167 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1631 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.845844 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1087 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/search.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1833 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1544 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      145 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2997 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/init.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1299 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/navbar.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1247 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/navbar_menu.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1564 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/navbar_right.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.845990 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/swagger/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      884 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/swagger/swagger.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.846133 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.846238 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/__pycache__/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2023-07-05 19:34:38.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.862630 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/de/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.851318 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/de/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9681 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26578 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.863595 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/el/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.852230 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/el/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11017 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    22936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.864526 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.853120 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8468 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20079 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.865451 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/fr/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.858139 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/fr/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8504 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20065 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.866409 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/it/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.858535 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/it/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9121 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    24545 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.867331 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ja_JP/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.863813 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9412 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20790 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.868250 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ko/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.864242 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ko/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9513 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.869150 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/nl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.864641 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/nl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8252 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19648 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.870030 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.864979 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8136 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.870979 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.867760 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8441 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20002 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.871943 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt_BR/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.868260 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8336 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20517 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.872874 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ru/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.868844 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ru/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10674 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    22035 2023-03-13 10:27:18.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.873806 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/sl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.869505 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/sl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9682 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20841 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.874755 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/zh/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.870184 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/zh/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7528 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:04.875651 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/zh_HK/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.870593 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7576 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/upload.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3226 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/urltools.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.871105 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/utils/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/utils/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2284 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/utils/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      734 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/utils/limit.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3360 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/validators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31361 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4997 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc1/flask_appbuilder/widgets.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.903104 Flask-AppBuilder-4.3.5rc1/images/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/ListThumbnail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/chart_time1.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/chart_time2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/charts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/contact_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/contacts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/direct_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/fab.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/group_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/grouped_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/groups.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/images_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/list_cascade.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/list_cascade_block.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/list_compact_inline.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/list_master_detail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/login_db.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    84309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/login_oauth.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/login_oid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   417827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/security.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/images/simpleview2.png
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      181 2023-07-10 15:46:46.000000 Flask-AppBuilder-4.3.5rc1/release.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)      218 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.5rc1/requirements-dev.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)      157 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.5rc1/requirements-extra.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2905 2023-07-27 10:30:58.000000 Flask-AppBuilder-4.3.5rc1/requirements.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2320 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.5rc1/rtd_requirements.txt
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.903555 Flask-AppBuilder-4.3.5rc1/scripts/
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      217 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/scripts/babel_extract.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/scripts/babel_init.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2023-07-27 10:48:05.924366 Flask-AppBuilder-4.3.5rc1/setup.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2866 2023-07-27 10:30:58.000000 Flask-AppBuilder-4.3.5rc1/setup.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.916706 Flask-AppBuilder-4.3.5rc1/tests/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5390 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      463 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/config_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1029 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/config_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      479 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/config_security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      515 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/config_security_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      250 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/const.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.917309 Flask-AppBuilder-4.3.5rc1/tests/fixtures/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/fixtures/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      370 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/fixtures/addon_manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9430 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/fixtures/data_models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1113 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/fixtures/users.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.917607 Flask-AppBuilder-4.3.5rc1/tests/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1006 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/mongoengine/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.918764 Flask-AppBuilder-4.3.5rc1/tests/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/security/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35649 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/security/test_auth_ldap.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14748 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/security/test_auth_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2434 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/security/test_base_security_manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18479 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/security/test_mvc_security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1715 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/security/test_password_complexity.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2956 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/security/test_rate_limiter.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 10:48:05.919026 Flask-AppBuilder-4.3.5rc1/tests/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/sqla/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5815 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/sqla/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1264 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/test_addon.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)   129520 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/test_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1211 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/test_custom_indexview.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8787 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/test_fab_cli.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6470 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/test_menu.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    24059 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/test_mongoengine.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    72094 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/test_mvc.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5016 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/test_mvc_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    44610 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/test_security_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6022 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/test_security_permissions.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/test_sqlalchemy.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2506 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc1/tests/test_urltools.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1766 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc1/tox.ini
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.474969 Flask-AppBuilder-4.3.5rc2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       97 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/.coveragerc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      113 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/.env
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.562483 Flask-AppBuilder-4.3.5rc2/.github/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      642 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      681 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      202 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/.github/prlint.json
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      709 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/.github/stale.yml
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.564648 Flask-AppBuilder-4.3.5rc2/.github/workflows/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8119 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/.github/workflows/ci.yml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      137 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/.github/workflows/odbcinst.ini
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      951 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/.github/workflows/ptlint.yml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      147 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/.gitignore
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    64935 2023-07-27 11:05:18.000000 Flask-AppBuilder-4.3.5rc2/CHANGELOG.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1894 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/CONTRIBUTING.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.569012 Flask-AppBuilder-4.3.5rc2/Flask_AppBuilder.egg-info/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9315 2023-07-27 11:08:05.000000 Flask-AppBuilder-4.3.5rc2/Flask_AppBuilder.egg-info/PKG-INFO
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    36154 2023-07-27 11:08:05.000000 Flask-AppBuilder-4.3.5rc2/Flask_AppBuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2023-07-27 11:08:05.000000 Flask-AppBuilder-4.3.5rc2/Flask_AppBuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      110 2023-07-27 11:08:05.000000 Flask-AppBuilder-4.3.5rc2/Flask_AppBuilder.egg-info/entry_points.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-12 08:40:39.000000 Flask-AppBuilder-4.3.5rc2/Flask_AppBuilder.egg-info/not-zip-safe
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      559 2023-07-27 11:08:05.000000 Flask-AppBuilder-4.3.5rc2/Flask_AppBuilder.egg-info/requires.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       17 2023-07-27 11:08:05.000000 Flask-AppBuilder-4.3.5rc2/Flask_AppBuilder.egg-info/top_level.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1493 2023-04-05 15:10:33.000000 Flask-AppBuilder-4.3.5rc2/LICENSE
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2023-07-27 11:04:15.000000 Flask-AppBuilder-4.3.5rc2/MANIFEST.in
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9315 2023-07-27 11:08:06.475308 Flask-AppBuilder-4.3.5rc2/PKG-INFO
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6684 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/README.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/RELEASE.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.570206 Flask-AppBuilder-4.3.5rc2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    36590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/babel/messages.pot
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.559860 Flask-AppBuilder-4.3.5rc2/bin/
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      176 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/bin/babel_extract.sh
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/bin/babel_init.sh
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      422 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/bin/bootswatch_update.sh
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1632 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/bin/config.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/bin/db_create.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      840 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/bin/db_migrate.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/bin/db_upgrade.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1419 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/bin/hash_db_password.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/bin/migrate_db_0.7.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)     4001 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/bin/migrate_db_1.3.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1917 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/bin/sqlite_upgrade_1.3.sql
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      999 2023-05-24 14:03:04.000000 Flask-AppBuilder-4.3.5rc2/docker-compose.yml
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.592123 Flask-AppBuilder-4.3.5rc2/docs/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6802 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/Makefile
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.592778 Flask-AppBuilder-4.3.5rc2/docs/_static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_static/Flask-AppBuilder.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.593660 Flask-AppBuilder-4.3.5rc2/docs/_templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_templates/layout.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.595729 Flask-AppBuilder-4.3.5rc2/docs/_themes/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_themes/LICENSE
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1093 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_themes/README
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.597769 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      954 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask/layout.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask/relations.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.599201 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask/static/Flask-AppBuilder.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9062 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask/static/flasky.css_t
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask/theme.conf
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.600486 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask_small/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      683 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask_small/layout.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.601136 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask_small/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask_small/static/flasky.css_t
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      184 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask_small/theme.conf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4875 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/_themes/flask_theme_support.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2277 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/actions.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3828 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/addons.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10881 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.5rc2/docs/advanced.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/api.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/cli.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8834 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/conf.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)    33485 2023-06-19 07:52:15.000000 Flask-AppBuilder-4.3.5rc2/docs/config.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10806 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/customizing.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4109 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/diagrams.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/generic_datasource.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3817 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/docs/i18n.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.624245 Flask-AppBuilder-4.3.5rc2/docs/images/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/ListThumbnail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/chart_time1.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/chart_time2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/charts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/contact_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/contacts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/direct_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/fab.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/group_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/grouped_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/groups.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/images_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/list_cascade.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/list_cascade_block.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/list_compact_inline.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/list_master_detail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/login.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/login_db.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/login_oid.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    82437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/oauth_login.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    48690 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/oauth_login_one_provider.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    42827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/security.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/simpleview2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    41274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/swagger001.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26185 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/images/swagger002.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1389 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/docs/index.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4377 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.5rc2/docs/installation.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2634 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/intro.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6721 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/make.bat
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/multipledbs.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/quickcharts.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/quickfiles.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/quickhowto.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4829 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/quickhowto_mongo.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1676 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/quickminimal.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8990 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/relations.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    47345 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.5rc2/docs/rest_api.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    36706 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/docs/security.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17032 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/templates.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4335 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/user_registration.rst
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)    12302 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/versionmigration.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/docs/views.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.625333 Flask-AppBuilder-4.3.5rc2/examples/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.627429 Flask-AppBuilder-4.3.5rc2/examples/base_api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/base_api/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.629573 Flask-AppBuilder-4.3.5rc2/examples/base_api/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      380 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/base_api/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/base_api/app/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1809 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/base_api/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.634520 Flask-AppBuilder-4.3.5rc2/examples/basefilter/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/basefilter/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      429 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/basefilter/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.637775 Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1458 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.448403 Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.448452 Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.639960 Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1413 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.643180 Flask-AppBuilder-4.3.5rc2/examples/basefilter/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/basefilter/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/basefilter/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/basefilter/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/basefilter/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2423 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/basefilter/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.646480 Flask-AppBuilder-4.3.5rc2/examples/composite_keys/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      254 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/composite_keys/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.649669 Flask-AppBuilder-4.3.5rc2/examples/composite_keys/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/composite_keys/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/composite_keys/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/composite_keys/app/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2182 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/composite_keys/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1477 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/composite_keys/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.654553 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.658180 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2061 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1804 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.448970 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.449019 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.660721 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.663177 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2460 2023-07-10 13:44:00.000000 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.666708 Flask-AppBuilder-4.3.5rc2/examples/dash/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      291 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/dash/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.670264 Flask-AppBuilder-4.3.5rc2/examples/dash/app/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.675063 Flask-AppBuilder-4.3.5rc2/examples/dash/app/Dashboard/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      797 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/dash/app/Dashboard/Dash_App1.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/dash/app/Dashboard/Dash_App2.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1568 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/dash/app/Dashboard/Dash_fun.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/dash/app/Dashboard/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/dash/app/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.676062 Flask-AppBuilder-4.3.5rc2/examples/dash/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      701 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/dash/app/templates/dash.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1031 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/dash/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.678233 Flask-AppBuilder-4.3.5rc2/examples/dash/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/dash/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/dash/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/dash/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/dash/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.680597 Flask-AppBuilder-4.3.5rc2/examples/employees/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      276 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/employees/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.684983 Flask-AppBuilder-4.3.5rc2/examples/employees/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/employees/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/employees/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/employees/app/security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1972 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.5rc2/examples/employees/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.686201 Flask-AppBuilder-4.3.5rc2/examples/employees/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/employees/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/employees/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.691222 Flask-AppBuilder-4.3.5rc2/examples/enums/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/enums/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/enums/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.694435 Flask-AppBuilder-4.3.5rc2/examples/enums/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/enums/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1158 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/enums/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.449945 Flask-AppBuilder-4.3.5rc2/examples/enums/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.449992 Flask-AppBuilder-4.3.5rc2/examples/enums/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.696753 Flask-AppBuilder-4.3.5rc2/examples/enums/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3436 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/enums/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.698875 Flask-AppBuilder-4.3.5rc2/examples/enums/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/enums/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/enums/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/enums/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1841 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/enums/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.703711 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.710207 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2607 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/sec.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/sec_forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1923 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/sec_views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.450322 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.450369 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.712329 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1589 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.715575 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1961 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2977 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.720053 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      560 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.726493 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2831 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/sec.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/sec_forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1929 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/sec_views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.450770 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.450827 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.728611 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2133 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.730827 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.737192 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      432 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.740444 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.451202 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.451248 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.742545 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2121 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.745690 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1904 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/config2.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1867 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/examples/factoryapp/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.747859 Flask-AppBuilder-4.3.5rc2/examples/issue_789/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1610 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/issue_789/README.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4740 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/issue_789/app.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.751434 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/NAMES.DIC
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.754884 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1164 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.453573 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.453971 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.757120 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.761541 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/masterdetail/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.766284 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.770581 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/mysecurity.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.456392 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.456761 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.772786 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2988 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.774891 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.780914 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.784625 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.459348 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.459706 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.788495 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2623 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.794201 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoengine/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.804258 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      296 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.810020 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2732 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.462292 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.462661 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.813932 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4050 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.819746 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/mongoimages/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.828533 Flask-AppBuilder-4.3.5rc2/examples/oauth/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/oauth/.gitignore
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/oauth/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.846834 Flask-AppBuilder-4.3.5rc2/examples/oauth/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      743 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/oauth/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      399 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/oauth/app/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/oauth/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/examples/oauth/app/security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2395 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/examples/oauth/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.854032 Flask-AppBuilder-4.3.5rc2/examples/oauth/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/oauth/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/oauth/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8905 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/examples/oauth/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/oauth/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.865027 Flask-AppBuilder-4.3.5rc2/examples/productsale/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      192 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/productsale/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.875936 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1755 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.467786 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.467252 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.883493 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.468145 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.891049 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1304 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/productsale/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.894826 Flask-AppBuilder-4.3.5rc2/examples/productsale/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/productsale/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/productsale/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/productsale/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.906623 Flask-AppBuilder-4.3.5rc2/examples/quickactions/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.918080 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      554 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      263 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.471608 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.471068 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.925583 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.471964 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.933297 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1067 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.937112 Flask-AppBuilder-4.3.5rc2/examples/quickactions/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickactions/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1945 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickactions/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickactions/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      279 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickactions/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.944682 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.959849 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1646 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/data.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.474478 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.474833 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.967222 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2928 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.978228 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1775 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.985542 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.996794 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      352 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.477509 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.477904 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.004331 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5034 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.024541 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/babel/messages.pot~
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.480720 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.479769 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/bdist.linux-i686/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.480168 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/bdist.linux-i686/egg/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.045688 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.481081 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/lib/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.067330 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/lib/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/lib/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/lib/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/lib/app/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1726 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.091607 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      225 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.113097 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1188 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.120298 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.483624 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.141647 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16804 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.484507 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.162935 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16794 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1395 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.177509 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1795 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickfiles/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.206795 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.228344 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-07-29 16:17:15.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.487083 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.487439 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.242801 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3166 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.257239 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2758 2023-07-10 14:06:44.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.258767 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/NAMES.DIC
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.260733 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      556 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      105 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/indexview.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3024 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      300 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/sec.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/sec_models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2047 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/sec_views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.491590 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.263477 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abBtnAdd.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      171 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abBtnDelete.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abBtnEdit.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      179 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abBtnShow.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abDate.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abMenuPageSize.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      548 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1633 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abModelSearch.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2033 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abModelTable.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abPagination.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abSelect.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.263957 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/css/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7059 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/css/clean-blog.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1446 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/css/scrolling-nav.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.264414 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/img/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      783 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/img/brand.jpg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3208 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/img/loading.gif
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.265681 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.266293 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Controllers/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1781 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      240 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Controllers/searchCtrl.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.266721 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Directives/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3764 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Directives/bigDirectives.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9587 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Directives/btnDirectives.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.266950 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Services/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2825 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Services/apiService.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   125321 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/angular.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/app.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17294 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/clean-blog.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      612 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/scrolling-nav.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.268595 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.268813 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/appbuilder/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/list_angulajs.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      332 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/list_contacts.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/list_json.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      199 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/mylist.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/new_base.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      371 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/show_contacts.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.269284 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/widgets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2549 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/widgets/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      280 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/widgets/list_override.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.492595 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.492655 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.269781 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2511 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.270479 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2387 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2327 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1533 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.272739 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    92965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/.coverage
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      220 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.273380 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      753 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.493044 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.493092 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.273833 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.274458 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1942 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/migrate_db_0.7.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1397 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.274903 Flask-AppBuilder-4.3.5rc2/examples/quickimages/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickimages/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.275588 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2636 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.493596 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.493489 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.276061 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.493668 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.276578 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4155 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.276836 Flask-AppBuilder-4.3.5rc2/examples/quickimages/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickimages/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1704 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickimages/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.277831 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.282971 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      418 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.494221 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.494286 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.283443 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3627 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.283818 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.284021 Flask-AppBuilder-4.3.5rc2/examples/quickminimal/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      430 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quickminimal/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.285527 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.286604 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/.idea/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      159 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/.idea/encodings.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      679 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/.idea/misc.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      278 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/.idea/modules.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/.idea/quicksqlviews.iml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1846 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/.idea/workspace.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.287265 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.494999 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.495069 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.287747 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.288270 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.289980 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.290566 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      386 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.495697 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/static/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.290777 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/static/css/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2891 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/static/css/landing-page.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.290962 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3347 2023-07-27 10:30:58.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/templates/mybase.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.496187 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.496265 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.291398 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3658 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.292048 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.293383 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.294245 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1553 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.302952 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       66 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/.babelrc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      398 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/README.md
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   838924 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/package-lock.json
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3522 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/package.json
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      746 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/package.json.react-original
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.303774 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/public/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/public/favicon.ico
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      283 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/public/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/public/manifest.json
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.309009 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      375 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/App.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.309286 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      959 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/api/Api.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.310334 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/components/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3602 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/components/CRUDButtons.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4478 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/components/Forms.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15937 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/components/Table.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      349 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/index.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      285 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/webpack.config.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.310813 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      856 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/templates/base.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/templates/react.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.497293 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.497356 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.311369 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.311865 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2462 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.313560 Flask-AppBuilder-4.3.5rc2/examples/related_fields/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/related_fields/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      221 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/related_fields/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.314102 Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.497731 Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.497779 Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.314551 Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5713 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.315006 Flask-AppBuilder-4.3.5rc2/examples/related_fields/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/related_fields/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/related_fields/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/related_fields/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/related_fields/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2739 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/related_fields/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.315955 Flask-AppBuilder-4.3.5rc2/examples/simpleform/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleform/.gitignore
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      286 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleform/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.316567 Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      507 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/forms.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.316733 Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/templates/404.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.498195 Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.498268 Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.317080 Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      940 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.317450 Flask-AppBuilder-4.3.5rc2/examples/simpleform/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleform/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      662 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleform/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3697 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleform/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleform/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.317933 Flask-AppBuilder-4.3.5rc2/examples/simpleview1/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      173 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview1/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.318247 Flask-AppBuilder-4.3.5rc2/examples/simpleview1/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview1/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      601 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview1/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.318542 Flask-AppBuilder-4.3.5rc2/examples/simpleview1/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview1/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview1/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview1/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview1/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.318848 Flask-AppBuilder-4.3.5rc2/examples/simpleview2/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.319151 Flask-AppBuilder-4.3.5rc2/examples/simpleview2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      381 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview2/app/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.319548 Flask-AppBuilder-4.3.5rc2/examples/simpleview2/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      108 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview2/app/templates/method3.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1198 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.319860 Flask-AppBuilder-4.3.5rc2/examples/simpleview2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/simpleview2/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.321682 Flask-AppBuilder-4.3.5rc2/examples/user_registration/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      267 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.322166 Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1639 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.499378 Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.499426 Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.322594 Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3965 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.323062 Flask-AppBuilder-4.3.5rc2/examples/user_registration/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/user_registration/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.324115 Flask-AppBuilder-4.3.5rc2/examples/widgets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      229 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.326995 Flask-AppBuilder-4.3.5rc2/examples/widgets/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.499825 Flask-AppBuilder-4.3.5rc2/examples/widgets/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.499889 Flask-AppBuilder-4.3.5rc2/examples/widgets/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.327378 Flask-AppBuilder-4.3.5rc2/examples/widgets/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4839 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.327918 Flask-AppBuilder-4.3.5rc2/examples/widgets/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1491 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/examples/widgets/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.342892 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2023-07-27 11:04:35.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1970 2023-06-30 15:17:51.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/_compat.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1233 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/actions.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.343856 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    76068 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/api/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9871 2023-06-21 12:37:29.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/api/convert.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3368 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/api/manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/api/schemas.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.345028 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/babel/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2311 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/babel/manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/babel/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26023 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      346 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/basemanager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    48967 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/baseviews.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.345770 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/charts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/charts/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/charts/jsontools.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17665 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/charts/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/charts/widgets.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14981 2023-05-05 08:39:47.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/cli.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14159 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/console.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8403 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/const.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1138 2022-09-30 13:30:31.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/exceptions.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8785 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/fields.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5984 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/fieldwidgets.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8534 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/filemanager.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)     6206 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11129 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3131 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/hooks.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7648 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/menu.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      290 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/messages.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.347218 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9580 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      846 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/decorators.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10374 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/filters.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.347821 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/generic/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    13059 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/generic/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/generic/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/generic/interface.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10970 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/group.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2633 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/mixins.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.348516 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/mongoengine/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1765 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/mongoengine/fields.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4184 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/mongoengine/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9982 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/mongoengine/interface.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.349153 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/sqla/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4145 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/sqla/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11046 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/sqla/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39115 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/sqla/interface.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.351227 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5220 2023-05-08 09:55:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10558 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/decorators.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4162 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    76822 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/manager.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.351724 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/mongoengine/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15303 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/mongoengine/manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3219 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/mongoengine/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10630 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/registerviews.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1359 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/schemas.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.356916 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.357082 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.357631 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/permission/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       45 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/permission/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      624 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/permission/api.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.358037 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       53 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      647 2023-07-10 13:48:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.358625 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/role/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/role/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5053 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/role/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      390 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/role/schema.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.362075 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/user/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/user/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6695 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/user/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2481 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/user/schema.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1100 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/user/validator.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.362556 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/view_menu/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       43 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/view_menu/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      569 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/view_menu/api.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)    26664 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/manager.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)     5260 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/utils.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    25706 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.507806 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.514203 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.363016 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/ab.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121457 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/bootstrap.min.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.363862 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/flags/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/flags/flags16.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.365109 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18600 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    80761 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      586 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      578 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1760 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    27593 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.391091 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   105250 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/amelia.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   120090 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/cerulean.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   119768 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/cosmo.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   119799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/cyborg.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121625 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/darkly.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121354 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/flatly.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118666 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/journal.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   124431 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/lumen.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   132318 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/paper.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118678 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/readable.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/sandstone.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   120186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/simplex.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   129014 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/slate.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   125030 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/solar.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/spacelab.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   120731 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/superhero.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   117016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/united.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121865 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/yeti.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.391559 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/datepicker/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.402027 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/fonts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20127 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   108738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    45404 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    23424 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18028 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.403324 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/aol.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/fab.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.403502 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/flags/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    63284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/flags/flags16.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/flickr.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8777 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    12799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2558 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/google.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2882 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/myopenid.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/yahoo.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.411055 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3321 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/ab.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4228 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/ab_actions.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5176 2023-07-10 14:06:29.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/ab_filters.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1526 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39680 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/bootstrap.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    46151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/google_charts.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    89501 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/jquery-latest.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    27347 2023-01-10 15:34:59.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/v4-shims.min.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.412856 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16792 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1849 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17358 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/select2.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    79212 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/select2.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/select2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      845 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/select2x2.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.421070 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   186124 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   107656 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    62320 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    25236 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   397420 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   150516 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10140 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4568 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.515107 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.423303 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/_formhelpers.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       28 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/base.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      874 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/baselayout.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4588 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/baselib.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      486 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/flash.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      143 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/footer.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.423747 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/alert.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.424260 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/charts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      778 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/charts/chart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      890 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      717 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/confirm.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14587 2023-07-27 10:30:58.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/lib.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.425824 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/add.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1181 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/edit.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      813 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      653 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      496 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      517 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      501 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/search.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1207 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/show.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      784 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.427178 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/activation.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2949 2023-01-10 15:41:47.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/login_db.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1996 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6568 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/login_oid.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      230 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/register_mail.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1057 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.430268 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1153 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2981 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/chart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2613 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/form.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1326 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1328 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/group_form_list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2745 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1331 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2038 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2843 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      572 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1167 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1631 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.430559 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1087 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/search.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/show.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1833 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1544 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      145 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2997 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/init.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1299 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/navbar.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1247 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/navbar_menu.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1564 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/navbar_right.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.430717 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/swagger/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      884 2023-07-10 14:05:21.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/swagger/swagger.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.430893 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.431007 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/__pycache__/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2023-07-05 19:34:38.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.521112 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/de/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.431516 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/de/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9681 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26578 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.522061 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/el/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.432229 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/el/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11017 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    22936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.523005 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.433092 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8468 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20079 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.523932 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/fr/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.433443 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8504 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20065 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.524889 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/it/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.433807 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/it/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9121 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    24545 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.525865 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ja_JP/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.434642 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9412 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20790 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.526797 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ko/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.434999 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ko/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9513 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.527694 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/nl/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.435338 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8252 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19648 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.528619 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pl/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.435673 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8136 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.529614 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.440902 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8441 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20002 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.530579 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt_BR/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.441377 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8336 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20517 2023-06-20 13:15:53.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.531528 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ru/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.441987 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10674 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    22035 2023-03-13 10:27:18.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.532460 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/sl/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.442715 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/sl/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9682 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20841 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.533398 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/zh/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.448151 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/zh/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7528 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:05.534318 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/zh_HK/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.448614 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7576 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/upload.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3226 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/urltools.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.449123 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/utils/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/utils/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2284 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/utils/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      734 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/utils/limit.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3360 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/validators.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    31361 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4997 2023-06-30 15:50:04.000000 Flask-AppBuilder-4.3.5rc2/flask_appbuilder/widgets.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.464761 Flask-AppBuilder-4.3.5rc2/images/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/ListThumbnail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/chart_time1.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/chart_time2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/charts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/contact_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/contacts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/direct_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/fab.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/group_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/grouped_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/groups.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/images_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/list_cascade.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/list_cascade_block.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/list_compact_inline.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/list_master_detail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/login.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/login_db.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    84309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/login_oauth.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/login_oid.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   417827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/security.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/images/simpleview2.png
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      193 2023-07-27 11:04:15.000000 Flask-AppBuilder-4.3.5rc2/release.sh
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      218 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.5rc2/requirements-dev.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      157 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.5rc2/requirements-extra.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2905 2023-07-27 10:30:58.000000 Flask-AppBuilder-4.3.5rc2/requirements.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2320 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.5rc2/rtd_requirements.txt
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.465164 Flask-AppBuilder-4.3.5rc2/scripts/
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      217 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/scripts/babel_extract.sh
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/scripts/babel_init.sh
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2023-07-27 11:08:06.475769 Flask-AppBuilder-4.3.5rc2/setup.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2866 2023-07-27 10:56:32.000000 Flask-AppBuilder-4.3.5rc2/setup.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.472452 Flask-AppBuilder-4.3.5rc2/tests/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5390 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      463 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/config_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1029 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/config_oauth.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      479 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/config_security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      515 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/config_security_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      250 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/const.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.473072 Flask-AppBuilder-4.3.5rc2/tests/fixtures/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/fixtures/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      370 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/fixtures/addon_manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9430 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/fixtures/data_models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1113 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/fixtures/users.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.473326 Flask-AppBuilder-4.3.5rc2/tests/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/mongoengine/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1006 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/mongoengine/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.474534 Flask-AppBuilder-4.3.5rc2/tests/security/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/security/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    35649 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/security/test_auth_ldap.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14748 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/security/test_auth_oauth.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2434 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/security/test_base_security_manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18479 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/security/test_mvc_security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1715 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/security/test_password_complexity.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2956 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/security/test_rate_limiter.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-07-27 11:08:06.474816 Flask-AppBuilder-4.3.5rc2/tests/sqla/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/sqla/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5815 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/sqla/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1264 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/test_addon.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   129520 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/test_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1211 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/test_custom_indexview.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8787 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/test_fab_cli.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6470 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/test_menu.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    24059 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/test_mongoengine.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    72094 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/test_mvc.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5016 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/test_mvc_oauth.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    44610 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/test_security_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6022 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/test_security_permissions.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/test_sqlalchemy.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2506 2023-07-06 09:54:12.000000 Flask-AppBuilder-4.3.5rc2/tests/test_urltools.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1766 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.5rc2/tox.ini
```

### Comparing `Flask-AppBuilder-4.3.5rc1/.github/ISSUE_TEMPLATE.md` & `Flask-AppBuilder-4.3.5rc2/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/.github/PULL_REQUEST_TEMPLATE.md` & `Flask-AppBuilder-4.3.5rc2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/.github/stale.yml` & `Flask-AppBuilder-4.3.5rc2/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/.github/workflows/ci.yml` & `Flask-AppBuilder-4.3.5rc2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/.github/workflows/ptlint.yml` & `Flask-AppBuilder-4.3.5rc2/.github/workflows/ptlint.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/CHANGELOG.rst` & `Flask-AppBuilder-4.3.5rc2/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Flask-AppBuilder ChangeLog
 ==========================
 
 Improvements and Bug fixes on 4.3.5
 -----------------------------------
 
+- fix: release tests exclusion (#2093) [Daniel Vaz Gaspar]
 - fix: make deletion in quicktemplates example work again (#2088) [Fabian Halkivaha]
 - fix: MVC form action, broken reset my password (#2091) [Daniel Vaz Gaspar]
 - chore: dont add 'tests' package to wheel (#2087) [cwegener]
 - chore(deps): bump pygments from 2.13.0 to 2.15.0 (#2089) [dependabot[bot]]
 
 Improvements and Bug fixes on 4.3.4
 -----------------------------------
```

### Comparing `Flask-AppBuilder-4.3.5rc1/CONTRIBUTING.rst` & `Flask-AppBuilder-4.3.5rc2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/Flask_AppBuilder.egg-info/PKG-INFO` & `Flask-AppBuilder-4.3.5rc2/Flask_AppBuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-AppBuilder
-Version: 4.3.5rc1
+Version: 4.3.5rc2
 Summary: Simple and rapid application development framework, built on top of Flask. includes detailed security, auto CRUD generation for your models, google charts and much more.
 Home-page: https://github.com/dpgaspar/flask-appbuilder/
 Author: Daniel Vaz Gaspar
 Author-email: danielvazgaspar@gmail.com
 License: BSD
 Description: Flask App Builder
         =================
```

### Comparing `Flask-AppBuilder-4.3.5rc1/Flask_AppBuilder.egg-info/SOURCES.txt` & `Flask-AppBuilder-4.3.5rc2/Flask_AppBuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/Flask_AppBuilder.egg-info/requires.txt` & `Flask-AppBuilder-4.3.5rc2/Flask_AppBuilder.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/LICENSE` & `Flask-AppBuilder-4.3.5rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/PKG-INFO` & `Flask-AppBuilder-4.3.5rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-AppBuilder
-Version: 4.3.5rc1
+Version: 4.3.5rc2
 Summary: Simple and rapid application development framework, built on top of Flask. includes detailed security, auto CRUD generation for your models, google charts and much more.
 Home-page: https://github.com/dpgaspar/flask-appbuilder/
 Author: Daniel Vaz Gaspar
 Author-email: danielvazgaspar@gmail.com
 License: BSD
 Description: Flask App Builder
         =================
```

### Comparing `Flask-AppBuilder-4.3.5rc1/README.rst` & `Flask-AppBuilder-4.3.5rc2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/bin/config.py` & `Flask-AppBuilder-4.3.5rc2/bin/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/bin/db_migrate.py` & `Flask-AppBuilder-4.3.5rc2/bin/db_migrate.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/bin/hash_db_password.py` & `Flask-AppBuilder-4.3.5rc2/bin/hash_db_password.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/bin/migrate_db_0.7.py` & `Flask-AppBuilder-4.3.5rc2/bin/migrate_db_0.7.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/bin/migrate_db_1.3.py` & `Flask-AppBuilder-4.3.5rc2/bin/migrate_db_1.3.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/bin/sqlite_upgrade_1.3.sql` & `Flask-AppBuilder-4.3.5rc2/bin/sqlite_upgrade_1.3.sql`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docker-compose.yml` & `Flask-AppBuilder-4.3.5rc2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/Makefile` & `Flask-AppBuilder-4.3.5rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/_static/Flask-AppBuilder.png` & `Flask-AppBuilder-4.3.5rc2/docs/_static/Flask-AppBuilder.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/_templates/layout.html` & `Flask-AppBuilder-4.3.5rc2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/_themes/LICENSE` & `Flask-AppBuilder-4.3.5rc2/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/_themes/README` & `Flask-AppBuilder-4.3.5rc2/docs/_themes/README`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/_themes/flask/layout.html` & `Flask-AppBuilder-4.3.5rc2/docs/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/_themes/flask/relations.html` & `Flask-AppBuilder-4.3.5rc2/docs/_themes/flask/relations.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/_themes/flask/static/Flask-AppBuilder.png` & `Flask-AppBuilder-4.3.5rc2/docs/_themes/flask/static/Flask-AppBuilder.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/_themes/flask/static/flasky.css_t` & `Flask-AppBuilder-4.3.5rc2/docs/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/_themes/flask_small/layout.html` & `Flask-AppBuilder-4.3.5rc2/docs/_themes/flask_small/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/_themes/flask_small/static/flasky.css_t` & `Flask-AppBuilder-4.3.5rc2/docs/_themes/flask_small/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/_themes/flask_theme_support.py` & `Flask-AppBuilder-4.3.5rc2/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/actions.rst` & `Flask-AppBuilder-4.3.5rc2/docs/actions.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/addons.rst` & `Flask-AppBuilder-4.3.5rc2/docs/addons.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/advanced.rst` & `Flask-AppBuilder-4.3.5rc2/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/api.rst` & `Flask-AppBuilder-4.3.5rc2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/cli.rst` & `Flask-AppBuilder-4.3.5rc2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/conf.py` & `Flask-AppBuilder-4.3.5rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/config.rst` & `Flask-AppBuilder-4.3.5rc2/docs/config.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/customizing.rst` & `Flask-AppBuilder-4.3.5rc2/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/diagrams.rst` & `Flask-AppBuilder-4.3.5rc2/docs/diagrams.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/generic_datasource.rst` & `Flask-AppBuilder-4.3.5rc2/docs/generic_datasource.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/i18n.rst` & `Flask-AppBuilder-4.3.5rc2/docs/i18n.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/ListThumbnail.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/ListThumbnail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/chart.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/chart_time1.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/chart_time1.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/chart_time2.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/chart_time2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/charts.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/charts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/contact_list.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/contact_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/contacts.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/contacts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/direct_chart.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/direct_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/fab.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/group_list.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/group_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/grouped_chart.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/grouped_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/groups.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/groups.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/images_list.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/images_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/list_cascade.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/list_cascade.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/list_cascade_block.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/list_cascade_block.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/list_compact_inline.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/list_compact_inline.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/list_master_detail.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/list_master_detail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/login.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/login_db.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/login_db.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/login_oid.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/login_oid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/oauth_login.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/oauth_login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/oauth_login_one_provider.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/oauth_login_one_provider.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/security.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/security.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/simpleview2.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/simpleview2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/swagger001.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/swagger001.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/images/swagger002.png` & `Flask-AppBuilder-4.3.5rc2/docs/images/swagger002.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/index.rst` & `Flask-AppBuilder-4.3.5rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/installation.rst` & `Flask-AppBuilder-4.3.5rc2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/intro.rst` & `Flask-AppBuilder-4.3.5rc2/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/make.bat` & `Flask-AppBuilder-4.3.5rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/multipledbs.rst` & `Flask-AppBuilder-4.3.5rc2/docs/multipledbs.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/quickcharts.rst` & `Flask-AppBuilder-4.3.5rc2/docs/quickcharts.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/quickfiles.rst` & `Flask-AppBuilder-4.3.5rc2/docs/quickfiles.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/quickhowto.rst` & `Flask-AppBuilder-4.3.5rc2/docs/quickhowto.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/quickhowto_mongo.rst` & `Flask-AppBuilder-4.3.5rc2/docs/quickhowto_mongo.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/quickminimal.rst` & `Flask-AppBuilder-4.3.5rc2/docs/quickminimal.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/relations.rst` & `Flask-AppBuilder-4.3.5rc2/docs/relations.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/rest_api.rst` & `Flask-AppBuilder-4.3.5rc2/docs/rest_api.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/security.rst` & `Flask-AppBuilder-4.3.5rc2/docs/security.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/templates.rst` & `Flask-AppBuilder-4.3.5rc2/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/user_registration.rst` & `Flask-AppBuilder-4.3.5rc2/docs/user_registration.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/versionmigration.rst` & `Flask-AppBuilder-4.3.5rc2/docs/versionmigration.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/docs/views.rst` & `Flask-AppBuilder-4.3.5rc2/docs/views.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/README.rst` & `Flask-AppBuilder-4.3.5rc2/examples/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/base_api/app/api.py` & `Flask-AppBuilder-4.3.5rc2/examples/base_api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/base_api/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/base_api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/basefilter/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/basefilter/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/basefilter/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/basefilter/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/basefilter/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/basefilter/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/basefilter/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/basefilter/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/basefilter/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/basefilter/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/basefilter/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/basefilter/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/composite_keys/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/composite_keys/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/composite_keys/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/composite_keys/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/composite_keys/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/composite_keys/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/composite_keys/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/composite_keys/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/api.py` & `Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/crud_rest_api/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/crud_rest_api/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/dash/app/Dashboard/Dash_App1.py` & `Flask-AppBuilder-4.3.5rc2/examples/dash/app/Dashboard/Dash_App1.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/dash/app/Dashboard/Dash_App2.py` & `Flask-AppBuilder-4.3.5rc2/examples/dash/app/Dashboard/Dash_App2.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/dash/app/Dashboard/Dash_fun.py` & `Flask-AppBuilder-4.3.5rc2/examples/dash/app/Dashboard/Dash_fun.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/dash/app/templates/dash.html` & `Flask-AppBuilder-4.3.5rc2/examples/dash/app/templates/dash.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/dash/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/dash/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/dash/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/dash/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/employees/app/__init__.py` & `Flask-AppBuilder-4.3.5rc2/examples/employees/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/employees/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/employees/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/employees/app/security.py` & `Flask-AppBuilder-4.3.5rc2/examples/employees/app/security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/employees/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/employees/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/employees/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/employees/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/enums/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/enums/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/enums/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/enums/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/enums/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/enums/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/enums/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/enums/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/enums/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/enums/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/enums/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/enums/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/README.rst` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/__init__.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/sec_forms.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/sec_forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/sec_views.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/README.rst` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/sec_forms.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/sec_forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/sec_views.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/extendsecurity2/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/extendsecurity2/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/factoryapp/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/factoryapp/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/factoryapp/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/factoryapp/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/factoryapp/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/factoryapp/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/factoryapp/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/factoryapp/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/factoryapp/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/factoryapp/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/factoryapp/config2.py` & `Flask-AppBuilder-4.3.5rc2/examples/factoryapp/config2.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/factoryapp/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/factoryapp/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/issue_789/README.rst` & `Flask-AppBuilder-4.3.5rc2/examples/issue_789/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/issue_789/app.py` & `Flask-AppBuilder-4.3.5rc2/examples/issue_789/app.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/masterdetail/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/masterdetail/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/masterdetail/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/masterdetail/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/masterdetail/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/masterdetail/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/masterdetail/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/masterdetail/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/masterdetail/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/masterdetail/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/masterdetail/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/masterdetail/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/__init__.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/mysecurity.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/mysecurity.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongo_extendedsecurity/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongo_extendedsecurity/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoengine/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/mongoengine/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoengine/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongoengine/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoengine/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/mongoengine/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoengine/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/mongoengine/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoengine/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongoengine/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoengine/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongoengine/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoimages/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/mongoimages/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoimages/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongoimages/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoimages/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/mongoimages/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoimages/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/mongoimages/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoimages/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongoimages/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/mongoimages/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/mongoimages/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/oauth/README.rst` & `Flask-AppBuilder-4.3.5rc2/examples/oauth/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/oauth/app/__init__.py` & `Flask-AppBuilder-4.3.5rc2/examples/oauth/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/oauth/app/security.py` & `Flask-AppBuilder-4.3.5rc2/examples/oauth/app/security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/oauth/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/oauth/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/oauth/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/oauth/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/productsale/app/__init__.py` & `Flask-AppBuilder-4.3.5rc2/examples/productsale/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/productsale/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/productsale/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/productsale/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/productsale/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/productsale/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/productsale/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/__init__.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickactions/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickactions/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickactions/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickactions/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/data.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/data.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/lib/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/lib/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/build/lib/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/build/lib/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickcharts2/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickcharts2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickfiles/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickfiles/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickfiles/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/quickfiles/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickfiles/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickfiles/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/__init__.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/forms.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/sec_views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abModelSearch.html` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abModelSearch.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abModelTable.html` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abModelTable.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/angularAssets/abPagination.html` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/angularAssets/abPagination.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/css/clean-blog.min.css` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/css/clean-blog.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/css/scrolling-nav.css` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/css/scrolling-nav.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/img/brand.jpg` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/img/brand.jpg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/img/loading.gif` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Directives/bigDirectives.js` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Directives/bigDirectives.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Directives/btnDirectives.js` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Directives/btnDirectives.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/Services/apiService.js` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/Services/apiService.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/angular.min.js` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/angular.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/app.js` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/app.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/clean-blog.min.js` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/clean-blog.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/static/js/scrolling-nav.js` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/static/js/scrolling-nav.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/list_angulajs.html` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/list_angulajs.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/list_json.html` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/list_json.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/templates/widgets/list.html` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/templates/widgets/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto2/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto2/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/.coverage` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/.coverage`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/__init__.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/migrate_db_0.7.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/migrate_db_0.7.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickhowto3/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickhowto3/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/__init__.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickimages/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickimages/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickimages/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickimages/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quickmigrate/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/quickmigrate/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/.idea/misc.xml` & `Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/.idea/misc.xml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/.idea/workspace.xml` & `Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicksqlviews/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/quicksqlviews/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/static/css/landing-page.css` & `Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/static/css/landing-page.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/templates/mybase.html` & `Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/templates/mybase.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/quicktemplates/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/quicktemplates/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/api.py` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/package-lock.json` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/package.json` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/package.json`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/package.json.react-original` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/package.json.react-original`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/public/favicon.ico` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/api/Api.js` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/api/Api.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/components/CRUDButtons.js` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/components/CRUDButtons.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/components/Forms.js` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/components/Forms.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/static/src/components/Table.js` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/static/src/components/Table.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/templates/base.html` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/react-rest-api/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/react-rest-api/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/related_fields/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/related_fields/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/related_fields/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/related_fields/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/related_fields/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/related_fields/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/related_fields/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/related_fields/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/related_fields/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/related_fields/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/simpleform/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/simpleform/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/simpleform/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/simpleform/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/simpleform/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/simpleform/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/simpleview1/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/simpleview1/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/simpleview1/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/simpleview1/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/simpleview2/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/simpleview2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/simpleview2/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/simpleview2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/user_registration/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/user_registration/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/user_registration/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/user_registration/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/user_registration/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/user_registration/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/user_registration/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/user_registration/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/user_registration/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/user_registration/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/user_registration/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/user_registration/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/widgets/NAMES.DIC` & `Flask-AppBuilder-4.3.5rc2/examples/widgets/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/widgets/app/models.py` & `Flask-AppBuilder-4.3.5rc2/examples/widgets/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/widgets/app/views.py` & `Flask-AppBuilder-4.3.5rc2/examples/widgets/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/widgets/babel/messages.pot` & `Flask-AppBuilder-4.3.5rc2/examples/widgets/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/widgets/babel/messages.pot~` & `Flask-AppBuilder-4.3.5rc2/examples/widgets/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/widgets/config.py` & `Flask-AppBuilder-4.3.5rc2/examples/widgets/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/examples/widgets/testdata.py` & `Flask-AppBuilder-4.3.5rc2/examples/widgets/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/__init__.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Daniel Vaz Gaspar"
-__version__ = "4.3.5rc1"
+__version__ = "4.3.5rc2"
 
 from .actions import action  # noqa: F401
 from .api import ModelRestApi  # noqa: F401
 from .base import AppBuilder  # noqa: F401
 from .baseviews import BaseView, expose  # noqa: F401
 from .charts.views import DirectByChartView, GroupByChartView  # noqa: F401
 from .models.group import aggregate_avg, aggregate_count, aggregate_sum  # noqa: F401
```

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/_compat.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/_compat.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/actions.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/actions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/api/__init__.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/api/convert.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/api/convert.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/api/manager.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/api/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/api/schemas.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/api/schemas.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/babel/manager.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/babel/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/base.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/baseviews.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/baseviews.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/charts/jsontools.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/charts/jsontools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/charts/views.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/charts/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/cli.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/console.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/console.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/const.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/const.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/exceptions.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/fields.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/fields.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/fieldwidgets.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/fieldwidgets.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/filemanager.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/filemanager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/filters.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/forms.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/hooks.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/hooks.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/menu.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/menu.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/base.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/decorators.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/filters.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/generic/__init__.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/generic/filters.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/generic/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/generic/interface.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/generic/interface.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/group.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/group.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/mixins.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/mixins.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/mongoengine/fields.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/mongoengine/fields.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/mongoengine/filters.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/mongoengine/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/mongoengine/interface.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/mongoengine/interface.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/sqla/__init__.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/sqla/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/sqla/filters.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/sqla/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/models/sqla/interface.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/models/sqla/interface.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/api.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/decorators.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/forms.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/manager.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/mongoengine/manager.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/mongoengine/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/mongoengine/models.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/mongoengine/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/registerviews.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/registerviews.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/schemas.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/schemas.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/permission/api.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/permission/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/role/api.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/role/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/user/api.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/user/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/user/schema.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/user/schema.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/user/validator.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/user/validator.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/apis/view_menu/api.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/apis/view_menu/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/manager.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/sqla/models.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/sqla/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/security/views.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/security/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/ab.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/ab.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/bootstrap.min.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/flags/flags16.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/flags/flags16.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/amelia.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/amelia.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/cerulean.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/cerulean.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/cosmo.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/cosmo.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/cyborg.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/cyborg.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/darkly.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/darkly.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/flatly.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/flatly.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/journal.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/journal.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/lumen.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/lumen.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/paper.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/paper.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/readable.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/readable.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/sandstone.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/sandstone.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/simplex.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/simplex.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/slate.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/slate.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/solar.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/solar.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/spacelab.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/spacelab.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/superhero.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/superhero.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/united.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/united.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/css/themes/yeti.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/css/themes/yeti.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/aol.png` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/aol.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/fab.png` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/flags/flags16.png` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/flags/flags16.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/flickr.png` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/flickr.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/google.png` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/google.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/myopenid.png` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/myopenid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/img/yahoo.png` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/img/yahoo.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/ab.js` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/ab.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/ab_actions.js` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/ab_actions.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/ab_filters.js` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/ab_filters.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/bootstrap.min.js` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/google_charts.js` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/google_charts.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/jquery-latest.js` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/jquery-latest.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/js/v4-shims.min.js` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/js/v4-shims.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/select2.css` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/select2.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/select2.js` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/select2.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/select2.png` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/select2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/select2/select2x2.png` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/select2/select2x2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/baselayout.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/baselayout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/baselib.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/baselib.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/charts/chart.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/charts/chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/confirm.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/confirm.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/lib.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/lib.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/edit.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/edit.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/show.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/login_db.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/login_db.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/login_oid.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/login_oid.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/chart.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/form.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/form.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/search.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/search.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/show.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/init.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/init.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/navbar.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/navbar.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/navbar_menu.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/navbar_menu.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/navbar_right.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/navbar_right.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/templates/appbuilder/swagger/swagger.html` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/templates/appbuilder/swagger/swagger.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/upload.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/upload.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/urltools.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/urltools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/utils/base.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/utils/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/utils/limit.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/utils/limit.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/validators.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/validators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/views.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/flask_appbuilder/widgets.py` & `Flask-AppBuilder-4.3.5rc2/flask_appbuilder/widgets.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/ListThumbnail.png` & `Flask-AppBuilder-4.3.5rc2/images/ListThumbnail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/chart.png` & `Flask-AppBuilder-4.3.5rc2/images/chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/chart_time1.png` & `Flask-AppBuilder-4.3.5rc2/images/chart_time1.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/chart_time2.png` & `Flask-AppBuilder-4.3.5rc2/images/chart_time2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/charts.png` & `Flask-AppBuilder-4.3.5rc2/images/charts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/contact_list.png` & `Flask-AppBuilder-4.3.5rc2/images/contact_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/contacts.png` & `Flask-AppBuilder-4.3.5rc2/images/contacts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/direct_chart.png` & `Flask-AppBuilder-4.3.5rc2/images/direct_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/fab.png` & `Flask-AppBuilder-4.3.5rc2/images/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/group_list.png` & `Flask-AppBuilder-4.3.5rc2/images/group_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/grouped_chart.png` & `Flask-AppBuilder-4.3.5rc2/images/grouped_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/groups.png` & `Flask-AppBuilder-4.3.5rc2/images/groups.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/images_list.png` & `Flask-AppBuilder-4.3.5rc2/images/images_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/list_cascade.png` & `Flask-AppBuilder-4.3.5rc2/images/list_cascade.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/list_cascade_block.png` & `Flask-AppBuilder-4.3.5rc2/images/list_cascade_block.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/list_compact_inline.png` & `Flask-AppBuilder-4.3.5rc2/images/list_compact_inline.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/list_master_detail.png` & `Flask-AppBuilder-4.3.5rc2/images/list_master_detail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/login.png` & `Flask-AppBuilder-4.3.5rc2/images/login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/login_db.png` & `Flask-AppBuilder-4.3.5rc2/images/login_db.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/login_oauth.png` & `Flask-AppBuilder-4.3.5rc2/images/login_oauth.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/login_oid.png` & `Flask-AppBuilder-4.3.5rc2/images/login_oid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/security.png` & `Flask-AppBuilder-4.3.5rc2/images/security.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/images/simpleview2.png` & `Flask-AppBuilder-4.3.5rc2/images/simpleview2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/requirements.txt` & `Flask-AppBuilder-4.3.5rc2/requirements.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/rtd_requirements.txt` & `Flask-AppBuilder-4.3.5rc2/rtd_requirements.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/setup.cfg` & `Flask-AppBuilder-4.3.5rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/setup.py` & `Flask-AppBuilder-4.3.5rc2/setup.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/base.py` & `Flask-AppBuilder-4.3.5rc2/tests/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/config_oauth.py` & `Flask-AppBuilder-4.3.5rc2/tests/config_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/config_security_api.py` & `Flask-AppBuilder-4.3.5rc2/tests/config_security_api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/fixtures/data_models.py` & `Flask-AppBuilder-4.3.5rc2/tests/fixtures/data_models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/fixtures/users.py` & `Flask-AppBuilder-4.3.5rc2/tests/fixtures/users.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/mongoengine/models.py` & `Flask-AppBuilder-4.3.5rc2/tests/mongoengine/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/security/test_auth_ldap.py` & `Flask-AppBuilder-4.3.5rc2/tests/security/test_auth_ldap.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/security/test_auth_oauth.py` & `Flask-AppBuilder-4.3.5rc2/tests/security/test_auth_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/security/test_base_security_manager.py` & `Flask-AppBuilder-4.3.5rc2/tests/security/test_base_security_manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/security/test_mvc_security.py` & `Flask-AppBuilder-4.3.5rc2/tests/security/test_mvc_security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/security/test_password_complexity.py` & `Flask-AppBuilder-4.3.5rc2/tests/security/test_password_complexity.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/security/test_rate_limiter.py` & `Flask-AppBuilder-4.3.5rc2/tests/security/test_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/sqla/models.py` & `Flask-AppBuilder-4.3.5rc2/tests/sqla/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/test_addon.py` & `Flask-AppBuilder-4.3.5rc2/tests/test_addon.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/test_api.py` & `Flask-AppBuilder-4.3.5rc2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/test_custom_indexview.py` & `Flask-AppBuilder-4.3.5rc2/tests/test_custom_indexview.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/test_fab_cli.py` & `Flask-AppBuilder-4.3.5rc2/tests/test_fab_cli.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/test_menu.py` & `Flask-AppBuilder-4.3.5rc2/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/test_mongoengine.py` & `Flask-AppBuilder-4.3.5rc2/tests/test_mongoengine.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/test_mvc.py` & `Flask-AppBuilder-4.3.5rc2/tests/test_mvc.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/test_mvc_oauth.py` & `Flask-AppBuilder-4.3.5rc2/tests/test_mvc_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/test_security_api.py` & `Flask-AppBuilder-4.3.5rc2/tests/test_security_api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/test_security_permissions.py` & `Flask-AppBuilder-4.3.5rc2/tests/test_security_permissions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/test_sqlalchemy.py` & `Flask-AppBuilder-4.3.5rc2/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tests/test_urltools.py` & `Flask-AppBuilder-4.3.5rc2/tests/test_urltools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.5rc1/tox.ini` & `Flask-AppBuilder-4.3.5rc2/tox.ini`

 * *Files identical despite different names*

