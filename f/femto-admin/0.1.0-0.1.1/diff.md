# Comparing `tmp/femto-admin-0.1.0.tar.gz` & `tmp/femto-admin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femto-admin-0.1.0.tar", last modified: Thu Jul 20 23:53:22 2023, max compression
+gzip compressed data, was "femto-admin-0.1.1.tar", last modified: Thu Jul 27 11:14:36 2023, max compression
```

## Comparing `femto-admin-0.1.0.tar` & `femto-admin-0.1.1.tar`

### file list

```diff
@@ -1,56 +1,76 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.167400 femto-admin-0.1.0/
--rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 femto-admin-0.1.0/LICENSE
--rw-r--r--   0 sol        (501) staff       (20)       17 2023-07-20 14:49:50.000000 femto-admin-0.1.0/MANIFEST.in
--rw-r--r--   0 sol        (501) staff       (20)     2062 2023-07-20 23:53:22.167163 femto-admin-0.1.0/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1499 2023-07-20 23:49:02.000000 femto-admin-0.1.0/README.md
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.139828 femto-admin-0.1.0/femto_admin/
--rw-r--r--   0 sol        (501) staff       (20)       36 2023-07-20 11:43:08.000000 femto-admin-0.1.0/femto_admin/__init__.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.142997 femto-admin-0.1.0/femto_admin/__pycache__/
--rw-r--r--   0 sol        (501) staff       (20)      220 2023-07-20 14:50:39.000000 femto-admin-0.1.0/femto_admin/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)     7092 2023-07-20 23:07:29.000000 femto-admin-0.1.0/femto_admin/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)     1314 2023-07-13 11:06:49.000000 femto-admin-0.1.0/femto_admin/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 sol        (501) staff       (20)     3335 2023-07-20 23:06:46.000000 femto-admin-0.1.0/femto_admin/admin.py
--rw-r--r--   0 sol        (501) staff       (20)      193 2023-07-19 16:49:12.000000 femto-admin-0.1.0/femto_admin/consts.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.135776 femto-admin-0.1.0/femto_admin/statics/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.143571 femto-admin-0.1.0/femto_admin/statics/placeholders/
--rw-r--r--   0 sol        (501) staff       (20)    16958 2023-06-23 13:05:44.000000 femto-admin-0.1.0/femto_admin/statics/placeholders/favicon.ico
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.144709 femto-admin-0.1.0/femto_admin/statics/placeholders/logo/
--rw-r--r--   0 sol        (501) staff       (20)      418 2023-06-23 17:08:58.000000 femto-admin-0.1.0/femto_admin/statics/placeholders/logo/logo-white.svg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.145305 femto-admin-0.1.0/femto_admin/statics/placeholders/users/
--rw-r--r--   0 sol        (501) staff       (20)     2094 2023-05-04 14:33:48.000000 femto-admin-0.1.0/femto_admin/statics/placeholders/users/admin.jpg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.136268 femto-admin-0.1.0/femto_admin/statics/vendor/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.136045 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.146448 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/css/
--rw-r--r--   0 sol        (501) staff       (20)    13550 2023-07-04 13:18:30.000000 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css
--rw-r--r--   0 sol        (501) staff       (20)    11981 2023-07-04 13:18:30.000000 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.150565 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/
--rw-r--r--   0 sol        (501) staff       (20)     5265 2023-07-04 13:18:32.000000 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js
--rw-r--r--   0 sol        (501) staff       (20)     2353 2023-07-04 13:18:32.000000 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js
--rw-r--r--   0 sol        (501) staff       (20)   457166 2023-07-04 13:18:32.000000 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js
--rw-r--r--   0 sol        (501) staff       (20)    87093 2023-07-04 13:18:32.000000 femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.154156 femto-admin-0.1.0/femto_admin/statics/vendor/jQuery/
--rw-r--r--   0 sol        (501) staff       (20)   284996 2023-07-04 13:23:04.000000 femto-admin-0.1.0/femto_admin/statics/vendor/jQuery/jquery.js
--rw-r--r--   0 sol        (501) staff       (20)    87462 2023-07-04 13:23:04.000000 femto-admin-0.1.0/femto_admin/statics/vendor/jQuery/jquery.min.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.136463 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.158036 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/css/
--rw-r--r--   0 sol        (501) staff       (20)   642443 2023-05-16 21:47:00.000000 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/css/tabler.css
--rw-r--r--   0 sol        (501) staff       (20)   542559 2023-05-16 21:47:00.000000 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/css/tabler.min.css
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.163921 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/
--rw-r--r--   0 sol        (501) staff       (20)     1053 2023-07-19 10:42:04.000000 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/dark-theme.js
--rw-r--r--   0 sol        (501) staff       (20)      679 2023-05-16 21:47:00.000000 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/dark-theme.min.js
--rw-r--r--   0 sol        (501) staff       (20)   265501 2023-05-16 21:47:00.000000 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/tabler.js
--rw-r--r--   0 sol        (501) staff       (20)   136567 2023-05-16 21:47:00.000000 femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/tabler.min.js
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.166876 femto-admin-0.1.0/femto_admin/templates/
--rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-20 15:06:51.000000 femto-admin-0.1.0/femto_admin/templates/dashboard.html
--rw-r--r--   0 sol        (501) staff       (20)    26017 2023-07-20 14:57:19.000000 femto-admin-0.1.0/femto_admin/templates/layout.html
--rw-r--r--   0 sol        (501) staff       (20)        0 2023-07-18 09:39:11.000000 femto-admin-0.1.0/femto_admin/templates/modal.html
--rw-r--r--   0 sol        (501) staff       (20)      816 2023-07-20 20:27:40.000000 femto-admin-0.1.0/femto_admin/templates/table.html
--rw-r--r--   0 sol        (501) staff       (20)     2183 2023-07-20 21:10:39.000000 femto-admin-0.1.0/femto_admin/utils.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 23:53:22.140989 femto-admin-0.1.0/femto_admin.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)     2062 2023-07-20 23:53:22.000000 femto-admin-0.1.0/femto_admin.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1533 2023-07-20 23:53:22.000000 femto-admin-0.1.0/femto_admin.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 23:53:22.000000 femto-admin-0.1.0/femto_admin.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-20 23:53:22.000000 femto-admin-0.1.0/femto_admin.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       12 2023-07-20 23:53:22.000000 femto-admin-0.1.0/femto_admin.egg-info/top_level.txt
--rw-r--r--   0 sol        (501) staff       (20)      691 2023-07-20 23:40:54.000000 femto-admin-0.1.0/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 23:53:22.167472 femto-admin-0.1.0/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.375717 femto-admin-0.1.1/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 femto-admin-0.1.1/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)       17 2023-07-20 14:49:50.000000 femto-admin-0.1.1/MANIFEST.in
+-rw-r--r--   0 sol        (501) staff       (20)     2062 2023-07-27 11:14:36.375496 femto-admin-0.1.1/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1499 2023-07-20 23:49:02.000000 femto-admin-0.1.1/README.md
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.352861 femto-admin-0.1.1/femto_admin/
+-rw-r--r--   0 sol        (501) staff       (20)       58 2023-07-27 11:06:02.000000 femto-admin-0.1.1/femto_admin/__init__.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.354968 femto-admin-0.1.1/femto_admin/__pycache__/
+-rw-r--r--   0 sol        (501) staff       (20)      247 2023-07-27 11:07:52.000000 femto-admin-0.1.1/femto_admin/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)     7386 2023-07-27 11:12:47.000000 femto-admin-0.1.1/femto_admin/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)      672 2023-07-25 15:42:13.000000 femto-admin-0.1.1/femto_admin/__pycache__/consts.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)     4345 2023-07-26 11:21:07.000000 femto-admin-0.1.1/femto_admin/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 sol        (501) staff       (20)     3691 2023-07-27 11:12:33.000000 femto-admin-0.1.1/femto_admin/admin.py
+-rw-r--r--   0 sol        (501) staff       (20)      208 2023-07-25 15:41:09.000000 femto-admin-0.1.1/femto_admin/consts.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.349391 femto-admin-0.1.1/femto_admin/statics/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.355205 femto-admin-0.1.1/femto_admin/statics/placeholders/
+-rw-r--r--   0 sol        (501) staff       (20)    16958 2023-06-23 13:05:44.000000 femto-admin-0.1.1/femto_admin/statics/placeholders/favicon.ico
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.355483 femto-admin-0.1.1/femto_admin/statics/placeholders/logo/
+-rw-r--r--   0 sol        (501) staff       (20)      418 2023-06-23 17:08:58.000000 femto-admin-0.1.1/femto_admin/statics/placeholders/logo/logo-white.svg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.355708 femto-admin-0.1.1/femto_admin/statics/placeholders/users/
+-rw-r--r--   0 sol        (501) staff       (20)     2094 2023-05-04 14:33:48.000000 femto-admin-0.1.1/femto_admin/statics/placeholders/users/admin.jpg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.349903 femto-admin-0.1.1/femto_admin/statics/vendor/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.349673 femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.356178 femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/css/
+-rw-r--r--   0 sol        (501) staff       (20)    13550 2023-07-04 13:18:30.000000 femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css
+-rw-r--r--   0 sol        (501) staff       (20)    11981 2023-07-04 13:18:30.000000 femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.358476 femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/js/
+-rw-r--r--   0 sol        (501) staff       (20)     5265 2023-07-04 13:18:32.000000 femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js
+-rw-r--r--   0 sol        (501) staff       (20)     2353 2023-07-04 13:18:32.000000 femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js
+-rw-r--r--   0 sol        (501) staff       (20)   457166 2023-07-04 13:18:32.000000 femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js
+-rw-r--r--   0 sol        (501) staff       (20)    87093 2023-07-04 13:18:32.000000 femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.360535 femto-admin-0.1.1/femto_admin/statics/vendor/jQuery/
+-rw-r--r--   0 sol        (501) staff       (20)   284996 2023-07-04 13:23:04.000000 femto-admin-0.1.1/femto_admin/statics/vendor/jQuery/jquery.js
+-rw-r--r--   0 sol        (501) staff       (20)    87462 2023-07-04 13:23:04.000000 femto-admin-0.1.1/femto_admin/statics/vendor/jQuery/jquery.min.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.350098 femto-admin-0.1.1/femto_admin/statics/vendor/tabler/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.362797 femto-admin-0.1.1/femto_admin/statics/vendor/tabler/css/
+-rw-r--r--   0 sol        (501) staff       (20)   642443 2023-05-16 21:47:00.000000 femto-admin-0.1.1/femto_admin/statics/vendor/tabler/css/tabler.css
+-rw-r--r--   0 sol        (501) staff       (20)   542559 2023-05-16 21:47:00.000000 femto-admin-0.1.1/femto_admin/statics/vendor/tabler/css/tabler.min.css
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.366738 femto-admin-0.1.1/femto_admin/statics/vendor/tabler/js/
+-rw-r--r--   0 sol        (501) staff       (20)     1053 2023-07-19 10:42:04.000000 femto-admin-0.1.1/femto_admin/statics/vendor/tabler/js/dark-theme.js
+-rw-r--r--   0 sol        (501) staff       (20)      679 2023-05-16 21:47:00.000000 femto-admin-0.1.1/femto_admin/statics/vendor/tabler/js/dark-theme.min.js
+-rw-r--r--   0 sol        (501) staff       (20)   265501 2023-05-16 21:47:00.000000 femto-admin-0.1.1/femto_admin/statics/vendor/tabler/js/tabler.js
+-rw-r--r--   0 sol        (501) staff       (20)   136567 2023-05-16 21:47:00.000000 femto-admin-0.1.1/femto_admin/statics/vendor/tabler/js/tabler.min.js
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.368960 femto-admin-0.1.1/femto_admin/templates/
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.369907 femto-admin-0.1.1/femto_admin/templates/components/
+-rw-r--r--   0 sol        (501) staff       (20)      940 2023-07-27 11:12:41.000000 femto-admin-0.1.1/femto_admin/templates/components/footer.html
+-rw-r--r--   0 sol        (501) staff       (20)     1421 2023-07-24 10:32:54.000000 femto-admin-0.1.1/femto_admin/templates/components/global_actions.html
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.374996 femto-admin-0.1.1/femto_admin/templates/components/inputs/
+-rw-r--r--   0 sol        (501) staff       (20)       83 2023-07-23 20:17:52.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/_help.html
+-rw-r--r--   0 sol        (501) staff       (20)      424 2023-07-03 09:15:48.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/color.html
+-rw-r--r--   0 sol        (501) staff       (20)      380 2023-07-03 09:15:48.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/date.html
+-rw-r--r--   0 sol        (501) staff       (20)     1019 2023-07-03 09:15:48.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/datetime.html
+-rw-r--r--   0 sol        (501) staff       (20)     1794 2023-07-03 09:15:48.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/editor.html
+-rw-r--r--   0 sol        (501) staff       (20)      489 2023-07-03 09:15:48.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/image.html
+-rw-r--r--   0 sol        (501) staff       (20)      253 2023-07-23 20:19:51.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/input.html
+-rw-r--r--   0 sol        (501) staff       (20)     1333 2023-07-03 09:15:48.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/json.html
+-rw-r--r--   0 sol        (501) staff       (20)      857 2023-07-03 09:15:48.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/many_to_many.html
+-rw-r--r--   0 sol        (501) staff       (20)      731 2023-07-26 11:30:32.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/point.html
+-rw-r--r--   0 sol        (501) staff       (20)      607 2023-07-03 09:15:48.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/radio.html
+-rw-r--r--   0 sol        (501) staff       (20)      459 2023-07-23 20:17:52.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/select.html
+-rw-r--r--   0 sol        (501) staff       (20)      473 2023-07-03 09:15:48.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/switch.html
+-rw-r--r--   0 sol        (501) staff       (20)      415 2023-07-03 09:15:48.000000 femto-admin-0.1.1/femto_admin/templates/components/inputs/textarea.html
+-rw-r--r--   0 sol        (501) staff       (20)     2195 2023-07-25 16:59:54.000000 femto-admin-0.1.1/femto_admin/templates/components/modal.html
+-rw-r--r--   0 sol        (501) staff       (20)     7353 2023-07-23 19:34:25.000000 femto-admin-0.1.1/femto_admin/templates/components/notofications.html
+-rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-20 15:06:51.000000 femto-admin-0.1.1/femto_admin/templates/dashboard.html
+-rw-r--r--   0 sol        (501) staff       (20)    11468 2023-07-24 10:30:44.000000 femto-admin-0.1.1/femto_admin/templates/layout.html
+-rw-r--r--   0 sol        (501) staff       (20)      899 2023-07-23 20:48:59.000000 femto-admin-0.1.1/femto_admin/templates/table.html
+-rw-r--r--   0 sol        (501) staff       (20)     3793 2023-07-26 11:20:58.000000 femto-admin-0.1.1/femto_admin/utils.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 11:14:36.354029 femto-admin-0.1.1/femto_admin.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     2062 2023-07-27 11:14:36.000000 femto-admin-0.1.1/femto_admin.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     2469 2023-07-27 11:14:36.000000 femto-admin-0.1.1/femto_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-27 11:14:36.000000 femto-admin-0.1.1/femto_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       27 2023-07-27 11:14:36.000000 femto-admin-0.1.1/femto_admin.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       12 2023-07-27 11:14:36.000000 femto-admin-0.1.1/femto_admin.egg-info/top_level.txt
+-rw-r--r--   0 sol        (501) staff       (20)      766 2023-07-27 11:04:53.000000 femto-admin-0.1.1/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-27 11:14:36.375773 femto-admin-0.1.1/setup.cfg
```

### Comparing `femto-admin-0.1.0/LICENSE` & `femto-admin-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/PKG-INFO` & `femto-admin-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femto-admin
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simplest fastest minimal ASGI CRUD Admin panel for Tortoise ORM models. It's generating fully native async auto  zero config one line app
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/femto-admin
 Project-URL: Repository, https://github.com/mixartemev/femto-admin
 Keywords: starlette,fastapi,admin,dashboard,datatables,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

### Comparing `femto-admin-0.1.0/README.md` & `femto-admin-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/__pycache__/admin.cpython-311.pyc` & `femto-admin-0.1.1/femto_admin/__pycache__/admin.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,348 +1,428 @@
 magic:    0xa70d0d0a
-moddate:  0x06beb964 (Thu Jul 20 23:06:46 2023 UTC)
-files sz: 3335
+moddate:  0x2151c264 (Thu Jul 27 11:12:33 2023 UTC)
+files sz: 3691
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a026d035a030100640064026c046d
-      055a050100640064036c066d075a076d085a080100640064046c096d0a5a
-      0a6d0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d0f5a0f01
-      00640064076c106d115a116d125a120100640064086c136d145a14010002
-      00470064098400640a6511a6030000ab0300000000000000005a15640b53
-      00
+      0x9700640064016c006d005a000100640064026c016d025a026d035a036d
+      045a040100640064036c056d065a060100640064046c076d085a086d095a
+      090100640064056c0a6d0b5a0b6d0c5a0c0100640064066c0d6d0e5a0e01
+      00640064076c0f6d105a100100640064086c116d125a126d135a13010064
+      0064096c146d155a1501006400640a6c165a166400640b6c176d185a1801
+      0002004700640c8400640d6512a6030000ab0300000000000000005a1964
+      0a5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('ChoiceLoader', 'FileSystemLoader', 'PackageLoader'))
-                 6 IMPORT_NAME              0 (jinja2)
-                 8 IMPORT_FROM              1 (ChoiceLoader)
-                10 STORE_NAME               1 (ChoiceLoader)
-                12 IMPORT_FROM              2 (FileSystemLoader)
-                14 STORE_NAME               2 (FileSystemLoader)
-                16 IMPORT_FROM              3 (PackageLoader)
-                18 STORE_NAME               3 (PackageLoader)
-                20 POP_TOP
-   
-     2          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               2 (('Request',))
-                26 IMPORT_NAME              4 (starlette.requests)
-                28 IMPORT_FROM              5 (Request)
-                30 STORE_NAME               5 (Request)
+                 4 LOAD_CONST               1 (('datetime',))
+                 6 IMPORT_NAME              0 (datetime)
+                 8 IMPORT_FROM              0 (datetime)
+                10 STORE_NAME               0 (datetime)
+                12 POP_TOP
+   
+     3          14 LOAD_CONST               0 (0)
+                16 LOAD_CONST               2 (('ChoiceLoader', 'FileSystemLoader', 'PackageLoader'))
+                18 IMPORT_NAME              1 (jinja2)
+                20 IMPORT_FROM              2 (ChoiceLoader)
+                22 STORE_NAME               2 (ChoiceLoader)
+                24 IMPORT_FROM              3 (FileSystemLoader)
+                26 STORE_NAME               3 (FileSystemLoader)
+                28 IMPORT_FROM              4 (PackageLoader)
+                30 STORE_NAME               4 (PackageLoader)
                 32 POP_TOP
    
-     3          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               3 (('RedirectResponse', 'JSONResponse'))
-                38 IMPORT_NAME              6 (starlette.responses)
-                40 IMPORT_FROM              7 (RedirectResponse)
-                42 STORE_NAME               7 (RedirectResponse)
-                44 IMPORT_FROM              8 (JSONResponse)
-                46 STORE_NAME               8 (JSONResponse)
-                48 POP_TOP
-   
-     4          50 LOAD_CONST               0 (0)
-                52 LOAD_CONST               4 (('Mount', 'Route'))
-                54 IMPORT_NAME              9 (starlette.routing)
-                56 IMPORT_FROM             10 (Mount)
-                58 STORE_NAME              10 (Mount)
-                60 IMPORT_FROM             11 (Route)
-                62 STORE_NAME              11 (Route)
-                64 POP_TOP
-   
-     5          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               5 (('StaticFiles',))
-                70 IMPORT_NAME             12 (starlette.staticfiles)
-                72 IMPORT_FROM             13 (StaticFiles)
-                74 STORE_NAME              13 (StaticFiles)
+     4          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               3 (('Request',))
+                38 IMPORT_NAME              5 (starlette.requests)
+                40 IMPORT_FROM              6 (Request)
+                42 STORE_NAME               6 (Request)
+                44 POP_TOP
+   
+     5          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('RedirectResponse', 'JSONResponse'))
+                50 IMPORT_NAME              7 (starlette.responses)
+                52 IMPORT_FROM              8 (RedirectResponse)
+                54 STORE_NAME               8 (RedirectResponse)
+                56 IMPORT_FROM              9 (JSONResponse)
+                58 STORE_NAME               9 (JSONResponse)
+                60 POP_TOP
+   
+     6          62 LOAD_CONST               0 (0)
+                64 LOAD_CONST               5 (('Mount', 'Route'))
+                66 IMPORT_NAME             10 (starlette.routing)
+                68 IMPORT_FROM             11 (Mount)
+                70 STORE_NAME              11 (Mount)
+                72 IMPORT_FROM             12 (Route)
+                74 STORE_NAME              12 (Route)
                 76 POP_TOP
    
-     6          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               6 (('Jinja2Templates',))
-                82 IMPORT_NAME             14 (starlette.templating)
-                84 IMPORT_FROM             15 (Jinja2Templates)
-                86 STORE_NAME              15 (Jinja2Templates)
+     7          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               6 (('StaticFiles',))
+                82 IMPORT_NAME             13 (starlette.staticfiles)
+                84 IMPORT_FROM             14 (StaticFiles)
+                86 STORE_NAME              14 (StaticFiles)
                 88 POP_TOP
    
-     7          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               7 (('Api', 'Model'))
-                94 IMPORT_NAME             16 (tortoise_api.api)
-                96 IMPORT_FROM             17 (Api)
-                98 STORE_NAME              17 (Api)
-               100 IMPORT_FROM             18 (Model)
-               102 STORE_NAME              18 (Model)
-               104 POP_TOP
-   
-     8         106 LOAD_CONST               0 (0)
-               108 LOAD_CONST               8 (('jsonify',))
-               110 IMPORT_NAME             19 (tortoise_api.util)
-               112 IMPORT_FROM             20 (jsonify)
-               114 STORE_NAME              20 (jsonify)
+     8          90 LOAD_CONST               0 (0)
+                92 LOAD_CONST               7 (('Jinja2Templates',))
+                94 IMPORT_NAME             15 (starlette.templating)
+                96 IMPORT_FROM             16 (Jinja2Templates)
+                98 STORE_NAME              16 (Jinja2Templates)
+               100 POP_TOP
+   
+     9         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               8 (('Api', 'Model'))
+               106 IMPORT_NAME             17 (tortoise_api.api)
+               108 IMPORT_FROM             18 (Api)
+               110 STORE_NAME              18 (Api)
+               112 IMPORT_FROM             19 (Model)
+               114 STORE_NAME              19 (Model)
                116 POP_TOP
    
-    11         118 PUSH_NULL
-               120 LOAD_BUILD_CLASS
-               122 LOAD_CONST               9 (<code object Admin, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 11>)
-               124 MAKE_FUNCTION            0
-               126 LOAD_CONST              10 ('Admin')
-               128 LOAD_NAME               17 (Api)
-               130 PRECALL                  3
-               134 CALL                     3
-               144 STORE_NAME              21 (Admin)
-               146 LOAD_CONST              11 (None)
-               148 RETURN_VALUE
+    10         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST               9 (('jsonify',))
+               122 IMPORT_NAME             20 (tortoise_api.util)
+               124 IMPORT_FROM             21 (jsonify)
+               126 STORE_NAME              21 (jsonify)
+               128 POP_TOP
+   
+    12         130 LOAD_CONST               0 (0)
+               132 LOAD_CONST              10 (None)
+               134 IMPORT_NAME             22 (femto_admin)
+               136 STORE_NAME              22 (femto_admin)
+   
+    13         138 LOAD_CONST               0 (0)
+               140 LOAD_CONST              11 (('_fields',))
+               142 IMPORT_NAME             23 (femto_admin.utils)
+               144 IMPORT_FROM             24 (_fields)
+               146 STORE_NAME              24 (_fields)
+               148 POP_TOP
+   
+    16         150 PUSH_NULL
+               152 LOAD_BUILD_CLASS
+               154 LOAD_CONST              12 (<code object Admin, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 16>)
+               156 MAKE_FUNCTION            0
+               158 LOAD_CONST              13 ('Admin')
+               160 LOAD_NAME               18 (Api)
+               162 PRECALL                  3
+               166 CALL                     3
+               176 STORE_NAME              25 (Admin)
+               178 LOAD_CONST              10 (None)
+               180 RETURN_VALUE
    consts
       0
+      ('datetime',)
       ('ChoiceLoader', 'FileSystemLoader', 'PackageLoader')
       ('Request',)
       ('RedirectResponse', 'JSONResponse')
       ('Mount', 'Route')
       ('StaticFiles',)
       ('Jinja2Templates',)
       ('Api', 'Model')
       ('jsonify',)
+      None
+      ('_fields',)
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 5
+         stacksize : 10
          flags     : 0
          code
-            0x8700970065005a0164005a02640a640265036403650466048800660164
-            04840d5a0588006601640584085a06640665076602640784045a08640665
-            076602640884045a09640665076602640984045a0a880078015a0b5300
+            0x8700970065005a0164005a02640d640365036404650464056504640665
+            0465037a0700006608880066016407840d5a0588006601640884085a0664
+            0965076602640a84045a08640965076602640b84045a0964096507660264
+            0c84045a0a880078015a0b5300
                        0 MAKE_CELL                0 (__class__)
          
-          11           2 RESUME                   0
+          16           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Admin')
                       10 STORE_NAME               2 (__qualname__)
          
-          12          12 LOAD_CONST              10 ((False, 'Admin'))
-                      14 LOAD_CONST               2 ('debug')
+          17          12 LOAD_CONST              13 ((False, 'Admin', None, None))
+                      14 LOAD_CONST               3 ('debug')
                       16 LOAD_NAME                3 (bool)
-                      18 LOAD_CONST               3 ('title')
+                      18 LOAD_CONST               4 ('title')
                       20 LOAD_NAME                4 (str)
-                      22 BUILD_TUPLE              4
-                      24 LOAD_CLOSURE             0 (__class__)
-                      26 BUILD_TUPLE              1
-                      28 LOAD_CONST               4 (<code object __init__, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 12>)
-                      30 MAKE_FUNCTION           13 (defaults, annotations, closure)
-                      32 STORE_NAME               5 (__init__)
+                      22 LOAD_CONST               5 ('static_dir')
+                      24 LOAD_NAME                4 (str)
+                      26 LOAD_CONST               6 ('logo')
+                      28 LOAD_NAME                4 (str)
+                      30 LOAD_NAME                3 (bool)
+                      32 BINARY_OP                7 (|)
+                      36 BUILD_TUPLE              8
+                      38 LOAD_CLOSURE             0 (__class__)
+                      40 BUILD_TUPLE              1
+                      42 LOAD_CONST               7 (<code object __init__, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 17>)
+                      44 MAKE_FUNCTION           13 (defaults, annotations, closure)
+                      46 STORE_NAME               5 (__init__)
          
-          42          34 LOAD_CLOSURE             0 (__class__)
-                      36 BUILD_TUPLE              1
-                      38 LOAD_CONST               5 (<code object start, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 42>)
-                      40 MAKE_FUNCTION            8 (closure)
-                      42 STORE_NAME               6 (start)
+          52          48 LOAD_CLOSURE             0 (__class__)
+                      50 BUILD_TUPLE              1
+                      52 LOAD_CONST               8 (<code object start, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 52>)
+                      54 MAKE_FUNCTION            8 (closure)
+                      56 STORE_NAME               6 (start)
          
-          48          44 LOAD_CONST               6 ('request')
-                      46 LOAD_NAME                7 (Request)
-                      48 BUILD_TUPLE              2
-                      50 LOAD_CONST               7 (<code object dash, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 48>)
-                      52 MAKE_FUNCTION            4 (annotations)
-                      54 STORE_NAME               8 (dash)
+          58          58 LOAD_CONST               9 ('request')
+                      60 LOAD_NAME                7 (Request)
+                      62 BUILD_TUPLE              2
+                      64 LOAD_CONST              10 (<code object dash, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 58>)
+                      66 MAKE_FUNCTION            4 (annotations)
+                      68 STORE_NAME               8 (dash)
          
-          55          56 LOAD_CONST               6 ('request')
-                      58 LOAD_NAME                7 (Request)
-                      60 BUILD_TUPLE              2
-                      62 LOAD_CONST               8 (<code object index, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 55>)
-                      64 MAKE_FUNCTION            4 (annotations)
-                      66 STORE_NAME               9 (index)
+          65          70 LOAD_CONST               9 ('request')
+                      72 LOAD_NAME                7 (Request)
+                      74 BUILD_TUPLE              2
+                      76 LOAD_CONST              11 (<code object index, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 65>)
+                      78 MAKE_FUNCTION            4 (annotations)
+                      80 STORE_NAME               9 (index)
          
-          64          68 LOAD_CONST               6 ('request')
-                      70 LOAD_NAME                7 (Request)
-                      72 BUILD_TUPLE              2
-                      74 LOAD_CONST               9 (<code object dt, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 64>)
-                      76 MAKE_FUNCTION            4 (annotations)
-                      78 STORE_NAME              10 (dt)
-                      80 LOAD_CLOSURE             0 (__class__)
-                      82 COPY                     1
-                      84 STORE_NAME              11 (__classcell__)
-                      86 RETURN_VALUE
+          74          82 LOAD_CONST               9 ('request')
+                      84 LOAD_NAME                7 (Request)
+                      86 BUILD_TUPLE              2
+                      88 LOAD_CONST              12 (<code object dt, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 74>)
+                      90 MAKE_FUNCTION            4 (annotations)
+                      92 STORE_NAME              10 (dt)
+                      94 LOAD_CLOSURE             0 (__class__)
+                      96 COPY                     1
+                      98 STORE_NAME              11 (__classcell__)
+                     100 RETURN_VALUE
          consts
             'Admin'
             False
+            None
             'debug'
             'title'
+            'static_dir'
+            'logo'
             code
-               argcount  : 3
-               nlocals   : 4
-               stacksize : 10
+               argcount  : 5
+               nlocals   : 6
+               stacksize : 9
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a00100000000000000000000000000000000000000007c01a6010000ab
                   01000000000000000001007c027c005f0200000000000000007407000000
                   00000000000000640174090000000000000000000064026701ac03a60100
                   00ab0100000000000000006404ac05a6030000ab03000000000000000074
                   070000000000000000000064067c006a050000000000000000ac07a60200
                   00ab020000000000000000740d0000000000000000000064086409840064
                   0a6701ac0ba6030000ab030000000000000000740d000000000000000000
-                  00640c7c006a070000000000000000640a6701ac0ba6030000ab03000000
-                  0000000000740d00000000000000000000640d7c006a0800000000000000
-                  00640a6701ac0ba6030000ab030000000000000000740d00000000000000
-                  000000640e7c006a090000000000000000640a6701ac0ba6030000ab0300
-                  0000000000000067067c005f0500000000000000007c006a050000000000
-                  000000640f190000000000000000006a050000000000000000a00a000000
-                  0000000000000000000000000000000000640fa6010000ab010000000000
-                  00000001007417000000000000000000006410a6010000ab010000000000
-                  0000007d03741900000000000000000000741b0000000000000000000064
-                  10a6010000ab010000000000000000741d00000000000000000000640264
-                  10a6020000ab0200000000000000006702a6010000ab0100000000000000
-                  007c036a0f00000000000000005f1000000000000000007c006a02000000
-                  00000000007c036a0f00000000000000006a11000000000000000064113c
-                  0000007c01720264126e0164137c036a0f00000000000000006a11000000
-                  000000000064143c0000007c037c005f12000000000000000064155300
+                  00640c7c006a070000000000000000a6020000ab02000000000000000074
+                  0d00000000000000000000640d7c006a080000000000000000a6020000ab
+                  020000000000000000740d00000000000000000000640e7c006a09000000
+                  0000000000a6020000ab02000000000000000067067c005f050000000000
+                  0000007c006a050000000000000000640f190000000000000000006a0500
+                  00000000000000a00a000000000000000000000000000000000000000064
+                  0fa6010000ab010000000000000000010074170000000000000000000064
+                  10a6010000ab0100000000000000007d057c03724c7c006a050000000000
+                  000000a00c00000000000000000000000000000000000000007407000000
+                  00000000000000640e7c037a0000007409000000000000000000007c03ac
+                  11a6010000ab0100000000000000006412ac05a6030000ab030000000000
+                  000000a6010000ab01000000000000000001007c04810f7c047c056a0d00
+                  000000000000006a0e000000000000000064143c000000741f0000000000
+                  00000000007421000000000000000000006410a6010000ab010000000000
+                  00000074230000000000000000000064026410a6020000ab020000000000
+                  0000006702a6010000ab0100000000000000007c056a0d00000000000000
+                  005f1200000000000000007c006a0200000000000000007c056a0d000000
+                  00000000006a0e000000000000000064153c000000742700000000000000
+                  0000006a140000000000000000a6000000ab0000000000000000006a1500
+                  00000000000000742c000000000000000000006a17000000000000000064
+                  169c027c056a0d00000000000000006a0e000000000000000064173c0000
+                  007c01720264186e0164197c056a0d00000000000000006a0e0000000000
+                  000000641a3c0000007c057c005f18000000000000000064135300
                              0 COPY_FREE_VARS           1
                
-                12           2 RESUME                   0
+                17           2 RESUME                   0
                
-                18           4 LOAD_GLOBAL              1 (NULL + super)
+                23           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (__init__)
                             52 LOAD_FAST                1 (debug)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 POP_TOP
                
-                19          70 LOAD_FAST                2 (title)
+                24          70 LOAD_FAST                2 (title)
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               2 (title)
                
-                22          84 LOAD_GLOBAL              7 (NULL + Mount)
+                27          84 LOAD_GLOBAL              7 (NULL + Mount)
                             96 LOAD_CONST               1 ('/static')
                             98 LOAD_GLOBAL              9 (NULL + StaticFiles)
                            110 LOAD_CONST               2 ('femto_admin')
                            112 BUILD_LIST               1
                            114 KW_NAMES                 3
                            116 PRECALL                  1
                            120 CALL                     1
                            130 LOAD_CONST               4 ('public')
                            132 KW_NAMES                 5
                            134 PRECALL                  3
                            138 CALL                     3
                
-                23         148 LOAD_GLOBAL              7 (NULL + Mount)
+                28         148 LOAD_GLOBAL              7 (NULL + Mount)
                            160 LOAD_CONST               6 ('/api')
                            162 LOAD_FAST                0 (self)
                            164 LOAD_ATTR                5 (routes)
                            174 KW_NAMES                 7
                            176 PRECALL                  2
                            180 CALL                     2
                
-                24         190 LOAD_GLOBAL             13 (NULL + Route)
+                29         190 LOAD_GLOBAL             13 (NULL + Route)
                            202 LOAD_CONST               8 ('/favicon.ico')
-                           204 LOAD_CONST               9 (<code object <lambda>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 24>)
+                           204 LOAD_CONST               9 (<code object <lambda>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 29>)
                            206 MAKE_FUNCTION            0
                            208 LOAD_CONST              10 ('GET')
                            210 BUILD_LIST               1
                            212 KW_NAMES                11
                            214 PRECALL                  3
                            218 CALL                     3
                
-                25         228 LOAD_GLOBAL             13 (NULL + Route)
+                30         228 LOAD_GLOBAL             13 (NULL + Route)
                            240 LOAD_CONST              12 ('/{model}')
                            242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                7 (index)
-                           254 LOAD_CONST              10 ('GET')
-                           256 BUILD_LIST               1
-                           258 KW_NAMES                11
-                           260 PRECALL                  3
-                           264 CALL                     3
-               
-                26         274 LOAD_GLOBAL             13 (NULL + Route)
-                           286 LOAD_CONST              13 ('/dt/{model}')
-                           288 LOAD_FAST                0 (self)
-                           290 LOAD_ATTR                8 (dt)
-                           300 LOAD_CONST              10 ('GET')
-                           302 BUILD_LIST               1
-                           304 KW_NAMES                11
-                           306 PRECALL                  3
-                           310 CALL                     3
-               
-                27         320 LOAD_GLOBAL             13 (NULL + Route)
-                           332 LOAD_CONST              14 ('/')
-                           334 LOAD_FAST                0 (self)
-                           336 LOAD_ATTR                9 (dash)
-                           346 LOAD_CONST              10 ('GET')
-                           348 BUILD_LIST               1
-                           350 KW_NAMES                11
-                           352 PRECALL                  3
-                           356 CALL                     3
-               
-                21         366 BUILD_LIST               6
-                           368 LOAD_FAST                0 (self)
-                           370 STORE_ATTR               5 (routes)
-               
-                29         380 LOAD_FAST                0 (self)
-                           382 LOAD_ATTR                5 (routes)
-                           392 LOAD_CONST              15 (1)
-                           394 BINARY_SUBSCR
-                           404 LOAD_ATTR                5 (routes)
-                           414 LOAD_METHOD             10 (pop)
-                           436 LOAD_CONST              15 (1)
-                           438 PRECALL                  1
-                           442 CALL                     1
-                           452 POP_TOP
-               
-                31         454 LOAD_GLOBAL             23 (NULL + Jinja2Templates)
-                           466 LOAD_CONST              16 ('templates')
-                           468 PRECALL                  1
-                           472 CALL                     1
-                           482 STORE_FAST               3 (templates)
-               
-                32         484 LOAD_GLOBAL             25 (NULL + ChoiceLoader)
-               
-                34         496 LOAD_GLOBAL             27 (NULL + FileSystemLoader)
-                           508 LOAD_CONST              16 ('templates')
-                           510 PRECALL                  1
-                           514 CALL                     1
-               
-                35         524 LOAD_GLOBAL             29 (NULL + PackageLoader)
-                           536 LOAD_CONST               2 ('femto_admin')
-                           538 LOAD_CONST              16 ('templates')
-                           540 PRECALL                  2
-                           544 CALL                     2
-               
-                33         554 BUILD_LIST               2
-               
-                32         556 PRECALL                  1
-                           560 CALL                     1
-                           570 LOAD_FAST                3 (templates)
-                           572 LOAD_ATTR               15 (env)
-                           582 STORE_ATTR              16 (loader)
-               
-                38         592 LOAD_FAST                0 (self)
-                           594 LOAD_ATTR                2 (title)
-                           604 LOAD_FAST                3 (templates)
-                           606 LOAD_ATTR               15 (env)
-                           616 LOAD_ATTR               17 (globals)
-                           626 LOAD_CONST              17 ('title')
-                           628 STORE_SUBSCR
-               
-                39         632 LOAD_FAST                1 (debug)
-                           634 POP_JUMP_FORWARD_IF_FALSE     2 (to 640)
-                           636 LOAD_CONST              18 ('')
-                           638 JUMP_FORWARD             1 (to 642)
-                       >>  640 LOAD_CONST              19 ('min.')
-                       >>  642 LOAD_FAST                3 (templates)
-                           644 LOAD_ATTR               15 (env)
-                           654 LOAD_ATTR               17 (globals)
-                           664 LOAD_CONST              20 ('minify')
-                           666 STORE_SUBSCR
-               
-                40         670 LOAD_FAST                3 (templates)
-                           672 LOAD_FAST                0 (self)
-                           674 STORE_ATTR              18 (templates)
-                           684 LOAD_CONST              21 (None)
-                           686 RETURN_VALUE
+                           254 PRECALL                  2
+                           258 CALL                     2
+               
+                31         268 LOAD_GLOBAL             13 (NULL + Route)
+                           280 LOAD_CONST              13 ('/dt/{model}')
+                           282 LOAD_FAST                0 (self)
+                           284 LOAD_ATTR                8 (dt)
+                           294 PRECALL                  2
+                           298 CALL                     2
+               
+                32         308 LOAD_GLOBAL             13 (NULL + Route)
+                           320 LOAD_CONST              14 ('/')
+                           322 LOAD_FAST                0 (self)
+                           324 LOAD_ATTR                9 (dash)
+                           334 PRECALL                  2
+                           338 CALL                     2
+               
+                26         348 BUILD_LIST               6
+                           350 LOAD_FAST                0 (self)
+                           352 STORE_ATTR               5 (routes)
+               
+                34         362 LOAD_FAST                0 (self)
+                           364 LOAD_ATTR                5 (routes)
+                           374 LOAD_CONST              15 (1)
+                           376 BINARY_SUBSCR
+                           386 LOAD_ATTR                5 (routes)
+                           396 LOAD_METHOD             10 (pop)
+                           418 LOAD_CONST              15 (1)
+                           420 PRECALL                  1
+                           424 CALL                     1
+                           434 POP_TOP
+               
+                36         436 LOAD_GLOBAL             23 (NULL + Jinja2Templates)
+                           448 LOAD_CONST              16 ('templates')
+                           450 PRECALL                  1
+                           454 CALL                     1
+                           464 STORE_FAST               5 (templates)
+               
+                37         466 LOAD_FAST                3 (static_dir)
+                           468 POP_JUMP_FORWARD_IF_FALSE    76 (to 622)
+               
+                38         470 LOAD_FAST                0 (self)
+                           472 LOAD_ATTR                5 (routes)
+                           482 LOAD_METHOD             12 (append)
+                           504 LOAD_GLOBAL              7 (NULL + Mount)
+                           516 LOAD_CONST              14 ('/')
+                           518 LOAD_FAST                3 (static_dir)
+                           520 BINARY_OP                0 (+)
+                           524 LOAD_GLOBAL              9 (NULL + StaticFiles)
+                           536 LOAD_FAST                3 (static_dir)
+                           538 KW_NAMES                17
+                           540 PRECALL                  1
+                           544 CALL                     1
+                           554 LOAD_CONST              18 ('my-public')
+                           556 KW_NAMES                 5
+                           558 PRECALL                  3
+                           562 CALL                     3
+                           572 PRECALL                  1
+                           576 CALL                     1
+                           586 POP_TOP
+               
+                39         588 LOAD_FAST                4 (logo)
+                           590 POP_JUMP_FORWARD_IF_NONE    15 (to 622)
+               
+                40         592 LOAD_FAST                4 (logo)
+                           594 LOAD_FAST                5 (templates)
+                           596 LOAD_ATTR               13 (env)
+                           606 LOAD_ATTR               14 (globals)
+                           616 LOAD_CONST              20 ('logo')
+                           618 STORE_SUBSCR
+               
+                41     >>  622 LOAD_GLOBAL             31 (NULL + ChoiceLoader)
+               
+                43         634 LOAD_GLOBAL             33 (NULL + FileSystemLoader)
+                           646 LOAD_CONST              16 ('templates')
+                           648 PRECALL                  1
+                           652 CALL                     1
+               
+                44         662 LOAD_GLOBAL             35 (NULL + PackageLoader)
+                           674 LOAD_CONST               2 ('femto_admin')
+                           676 LOAD_CONST              16 ('templates')
+                           678 PRECALL                  2
+                           682 CALL                     2
+               
+                42         692 BUILD_LIST               2
+               
+                41         694 PRECALL                  1
+                           698 CALL                     1
+                           708 LOAD_FAST                5 (templates)
+                           710 LOAD_ATTR               13 (env)
+                           720 STORE_ATTR              18 (loader)
+               
+                47         730 LOAD_FAST                0 (self)
+                           732 LOAD_ATTR                2 (title)
+                           742 LOAD_FAST                5 (templates)
+                           744 LOAD_ATTR               13 (env)
+                           754 LOAD_ATTR               14 (globals)
+                           764 LOAD_CONST              21 ('title')
+                           766 STORE_SUBSCR
+               
+                48         770 LOAD_GLOBAL             39 (NULL + datetime)
+                           782 LOAD_ATTR               20 (now)
+                           792 PRECALL                  0
+                           796 CALL                     0
+                           806 LOAD_ATTR               21 (year)
+                           816 LOAD_GLOBAL             44 (femto_admin)
+                           828 LOAD_ATTR               23 (__version__)
+                           838 LOAD_CONST              22 (('year', 'ver'))
+                           840 BUILD_CONST_KEY_MAP      2
+                           842 LOAD_FAST                5 (templates)
+                           844 LOAD_ATTR               13 (env)
+                           854 LOAD_ATTR               14 (globals)
+                           864 LOAD_CONST              23 ('meta')
+                           866 STORE_SUBSCR
+               
+                49         870 LOAD_FAST                1 (debug)
+                           872 POP_JUMP_FORWARD_IF_FALSE     2 (to 878)
+                           874 LOAD_CONST              24 ('')
+                           876 JUMP_FORWARD             1 (to 880)
+                       >>  878 LOAD_CONST              25 ('min.')
+                       >>  880 LOAD_FAST                5 (templates)
+                           882 LOAD_ATTR               13 (env)
+                           892 LOAD_ATTR               14 (globals)
+                           902 LOAD_CONST              26 ('minify')
+                           904 STORE_SUBSCR
+               
+                50         908 LOAD_FAST                5 (templates)
+                           910 LOAD_FAST                0 (self)
+                           912 STORE_ATTR              24 (templates)
+                           922 LOAD_CONST              19 (None)
+                           924 RETURN_VALUE
                consts
                   '\n        Parameters:\n            title: Admin title.\n            # auth_provider: Authentication Provider\n        '
                   '/static'
                   'femto_admin'
                   ('packages',)
                   'public'
                   ('name',)
@@ -353,15 +433,15 @@
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 4
                      flags     : 19
                      code
                         0x970074010000000000000000000064016402ac03a6020000ab02000000
                         00000000005300
-                      24           0 RESUME                   0
+                      29           0 RESUME                   0
                                    2 LOAD_GLOBAL              1 (NULL + RedirectResponse)
                                   14 LOAD_CONST               1 ('./static/placeholders/favicon.ico')
                                   16 LOAD_CONST               2 (301)
                                   18 KW_NAMES                 3
                                   20 PRECALL                  2
                                   24 CALL                     2
                                   34 RETURN_VALUE
@@ -372,233 +452,192 @@
                         ('status_code',)
                      names      ('RedirectResponse',)
                      varnames   ('r',)
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                      name       '<lambda>'
-                     firstlineno 24
+                     firstlineno 29
                      lnotab 0x
                   'GET'
                   ('methods',)
                   '/{model}'
                   '/dt/{model}'
                   '/'
                   1
                   'templates'
+                  ('directory',)
+                  'my-public'
+                  None
+                  'logo'
                   'title'
+                  ('year', 'ver')
+                  'meta'
                   ''
                   'min.'
                   'minify'
-                  None
-               names      ('super', '__init__', 'title', 'Mount', 'StaticFiles', 'routes', 'Route', 'index', 'dt', 'dash', 'pop', 'Jinja2Templates', 'ChoiceLoader', 'FileSystemLoader', 'PackageLoader', 'env', 'loader', 'globals', 'templates')
-               varnames   ('self', 'debug', 'title', 'templates')
+               names      ('super', '__init__', 'title', 'Mount', 'StaticFiles', 'routes', 'Route', 'index', 'dt', 'dash', 'pop', 'Jinja2Templates', 'append', 'env', 'globals', 'ChoiceLoader', 'FileSystemLoader', 'PackageLoader', 'loader', 'datetime', 'now', 'year', 'femto_admin', '__version__', 'templates')
+               varnames   ('self', 'debug', 'title', 'static_dir', 'logo', 'templates')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       '__init__'
-               firstlineno 12
+               firstlineno 17
                lnotab
-                  0x040642010e0340012a0126012e012e012efa0e084a021e010c021c011e
-                  fe02ff240628012601
+                  0x040642010e0340012a0126012801280128fa0e084a021e010401760104
+                  011e010c021c011efe02ff2406280164012601
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a00100000000000000000000000000000000000000007c01a6010000ab
                   0100000000000000007d027c006a0200000000000000007c006a03000000
                   00000000006a0400000000000000006a05000000000000000064013c0000
                   007c025300
                              0 COPY_FREE_VARS           1
                
-                42           2 RESUME                   0
+                52           2 RESUME                   0
                
-                43           4 LOAD_GLOBAL              1 (NULL + super)
+                53           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (start)
                             52 LOAD_FAST                1 (models_module)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 STORE_FAST               2 (app)
                
-                44          70 LOAD_FAST                0 (self)
+                54          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                2 (models)
                             82 LOAD_FAST                0 (self)
                             84 LOAD_ATTR                3 (templates)
                             94 LOAD_ATTR                4 (env)
                            104 LOAD_ATTR                5 (globals)
                            114 LOAD_CONST               1 ('models')
                            116 STORE_SUBSCR
                
-                45         120 LOAD_FAST                2 (app)
+                55         120 LOAD_FAST                2 (app)
                            122 RETURN_VALUE
                consts
                   None
                   'models'
                names      ('super', 'start', 'models', 'templates', 'env', 'globals')
                varnames   ('self', 'models_module', 'app')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       'start'
-               firstlineno 42
+               firstlineno 52
                lnotab 0x040142013201
             'request'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 7
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000006401640264037c0164049c03a6020000ab0200
                   000000000000005300
-                48           0 RETURN_GENERATOR
+                58           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                49           6 LOAD_FAST                0 (self)
+                59           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (templates)
                             18 LOAD_METHOD              1 (TemplateResponse)
                             40 LOAD_CONST               1 ('dashboard.html')
                
-                50          42 LOAD_CONST               2 ('Home')
+                60          42 LOAD_CONST               2 ('Home')
                
-                51          44 LOAD_CONST               3 ('Dashboard')
+                61          44 LOAD_CONST               3 ('Dashboard')
                
-                52          46 LOAD_FAST                1 (request)
+                62          46 LOAD_FAST                1 (request)
                
-                49          48 LOAD_CONST               4 (('title', 'subtitle', 'request'))
+                59          48 LOAD_CONST               4 (('model', 'subtitle', 'request'))
                             50 BUILD_CONST_KEY_MAP      3
                             52 PRECALL                  2
                             56 CALL                     2
                             66 RETURN_VALUE
                consts
                   None
                   'dashboard.html'
                   'Home'
                   'Dashboard'
-                  ('title', 'subtitle', 'request')
+                  ('model', 'subtitle', 'request')
                names      ('templates', 'TemplateResponse')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       'dash'
-               firstlineno 48
+               firstlineno 58
                lnotab 0x060124010201020102fd
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 9
                flags     : 131
                code
                   0x4b00010097007c00a00000000000000000000000000000000000000000
                   007c01a6010000ab0100000000000000007d027c006a0100000000000000
                   00a002000000000000000000000000000000000000000064017c026a0300
                   000000000000007c026a0400000000000000006a0500000000000000007c
-                  01640284007c026a0400000000000000006a060000000000000000a00700
-                  00000000000000000000000000000000000000a6000000ab000000000000
-                  0000004400a6000000ab00000000000000000064039c04a6020000ab0200
-                  000000000000005300
-                55           0 RETURN_GENERATOR
+                  01740d000000000000000000007c02a6010000ab01000000000000000064
+                  029c04a6020000ab0200000000000000005300
+                65           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                56           6 LOAD_FAST                0 (self)
+                66           6 LOAD_FAST                0 (self)
                              8 LOAD_METHOD              0 (_get_model)
                             30 LOAD_FAST                1 (request)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 STORE_FAST               2 (model)
                
-                57          48 LOAD_FAST                0 (self)
+                67          48 LOAD_FAST                0 (self)
                             50 LOAD_ATTR                1 (templates)
                             60 LOAD_METHOD              2 (TemplateResponse)
                             82 LOAD_CONST               1 ('table.html')
                
-                58          84 LOAD_FAST                2 (model)
+                68          84 LOAD_FAST                2 (model)
                             86 LOAD_ATTR                3 (__name__)
                
-                59          96 LOAD_FAST                2 (model)
+                69          96 LOAD_FAST                2 (model)
                             98 LOAD_ATTR                4 (_meta)
                            108 LOAD_ATTR                5 (table_description)
                
-                60         118 LOAD_FAST                1 (request)
+                70         118 LOAD_FAST                1 (request)
                
-                61         120 LOAD_CONST               2 (<code object <dictcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 61>)
-                           122 MAKE_FUNCTION            0
-                           124 LOAD_FAST                2 (model)
-                           126 LOAD_ATTR                4 (_meta)
-                           136 LOAD_ATTR                6 (fields_map)
-                           146 LOAD_METHOD              7 (items)
-                           168 PRECALL                  0
-                           172 CALL                     0
-                           182 GET_ITER
-                           184 PRECALL                  0
-                           188 CALL                     0
-               
-                57         198 LOAD_CONST               3 (('title', 'subtitle', 'request', 'fields'))
-                           200 BUILD_CONST_KEY_MAP      4
-                           202 PRECALL                  2
-                           206 CALL                     2
-                           216 RETURN_VALUE
+                71         120 LOAD_GLOBAL             13 (NULL + _fields)
+                           132 LOAD_FAST                2 (model)
+                           134 PRECALL                  1
+                           138 CALL                     1
+               
+                67         148 LOAD_CONST               2 (('model', 'subtitle', 'request', 'fields'))
+                           150 BUILD_CONST_KEY_MAP      4
+                           152 PRECALL                  2
+                           156 CALL                     2
+                           166 RETURN_VALUE
                consts
                   None
                   'table.html'
-                  code
-                     argcount  : 1
-                     nlocals   : 3
-                     stacksize : 5
-                     flags     : 19
-                     code
-                        0x970069007c005d1d5c0200007d017d027c01a000000000000000000000
-                        00000000000000000000006400a6010000ab010000000000000000b01a7c
-                        017c0293028c1e5300
-                      61           0 RESUME                   0
-                                   2 BUILD_MAP                0
-                                   4 LOAD_FAST                0 (.0)
-                             >>    6 FOR_ITER                29 (to 66)
-                                   8 UNPACK_SEQUENCE          2
-                                  12 STORE_FAST               1 (k)
-                                  14 STORE_FAST               2 (v)
-                                  16 LOAD_FAST                1 (k)
-                                  18 LOAD_METHOD              0 (endswith)
-                                  40 LOAD_CONST               0 ('_id')
-                                  42 PRECALL                  1
-                                  46 CALL                     1
-                                  56 POP_JUMP_BACKWARD_IF_TRUE    26 (to 6)
-                                  58 LOAD_FAST                1 (k)
-                                  60 LOAD_FAST                2 (v)
-                                  62 MAP_ADD                  2
-                                  64 JUMP_BACKWARD           30 (to 6)
-                             >>   66 RETURN_VALUE
-                     consts
-                        '_id'
-                     names      ('endswith',)
-                     varnames   ('.0', 'k', 'v')
-                     freevars   ()
-                     cellvars   ()
-                     filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
-                     name       '<dictcomp>'
-                     firstlineno 61
-                     lnotab 0x
-                  ('title', 'subtitle', 'request', 'fields')
-               names      ('_get_model', 'templates', 'TemplateResponse', '__name__', '_meta', 'table_description', 'fields_map', 'items')
+                  ('model', 'subtitle', 'request', 'fields')
+               names      ('_get_model', 'templates', 'TemplateResponse', '__name__', '_meta', 'table_description', '_fields')
                varnames   ('self', 'request', 'model')
                freevars   ()
                cellvars   ()
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       'index'
-               firstlineno 55
-               lnotab 0x06012a0124010c01160102014efc
+               firstlineno 65
+               lnotab 0x06012a0124010c01160102011cfc
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 4
                flags     : 131
                code
                   0x87054b000100970064017400000000000000000000006602640284048a
@@ -607,33 +646,33 @@
                   000000000000000000a6000000ab0000000000000000006a030000000000
                   0000007c026a0400000000000000006a0500000000000000008e00830064
                   007b035600970386047d0388056601640384087c034400a6000000ab0000
                   000000000000007d04740d0000000000000000000064047c046901a60100
                   00ab0100000000000000005300
                              0 MAKE_CELL                5 (render)
                
-                64           2 RETURN_GENERATOR
+                74           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-                65           8 LOAD_CONST               1 ('dct')
+                75           8 LOAD_CONST               1 ('dct')
                             10 LOAD_GLOBAL              0 (dict)
                             22 BUILD_TUPLE              2
-                            24 LOAD_CONST               2 (<code object render, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 65>)
+                            24 LOAD_CONST               2 (<code object render, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 75>)
                             26 MAKE_FUNCTION            4 (annotations)
                             28 STORE_DEREF              5 (render)
                
-                77          30 LOAD_FAST                0 (self)
+                87          30 LOAD_FAST                0 (self)
                             32 LOAD_METHOD              1 (_get_model)
                             54 LOAD_FAST                1 (request)
                             56 PRECALL                  1
                             60 CALL                     1
                             70 STORE_FAST               2 (model)
                
-                78          72 PUSH_NULL
+                88          72 PUSH_NULL
                             74 LOAD_FAST                2 (model)
                             76 LOAD_METHOD              2 (all)
                             98 PRECALL                  0
                            102 CALL                     0
                            112 LOAD_ATTR                3 (prefetch_related)
                            122 LOAD_FAST                2 (model)
                            124 LOAD_ATTR                4 (_meta)
@@ -643,25 +682,25 @@
                            148 LOAD_CONST               0 (None)
                        >>  150 SEND                     3 (to 158)
                            152 YIELD_VALUE
                            154 RESUME                   3
                            156 JUMP_BACKWARD_NO_INTERRUPT     4 (to 150)
                        >>  158 STORE_FAST               3 (objects)
                
-                79         160 LOAD_CLOSURE             5 (render)
+                89         160 LOAD_CLOSURE             5 (render)
                            162 BUILD_TUPLE              1
-                           164 LOAD_CONST               3 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 79>)
+                           164 LOAD_CONST               3 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 89>)
                            166 MAKE_FUNCTION            8 (closure)
                            168 LOAD_FAST                3 (objects)
                            170 GET_ITER
                            172 PRECALL                  0
                            176 CALL                     0
                            186 STORE_FAST               4 (data)
                
-                80         188 LOAD_GLOBAL             13 (NULL + JSONResponse)
+                90         188 LOAD_GLOBAL             13 (NULL + JSONResponse)
                            200 LOAD_CONST               4 ('data')
                            202 LOAD_FAST                4 (data)
                            204 BUILD_MAP                1
                            206 PRECALL                  1
                            210 CALL                     1
                            220 RETURN_VALUE
                consts
@@ -676,32 +715,32 @@
                         0x87018702970064017400000000000000000000006602640284048a0288
                         026601640384088a0188016601640484087c00a001000000000000000000
                         0000000000000000000000a6000000ab0000000000000000004400a60000
                         00ab0000000000000000005300
                                    0 MAKE_CELL                1 (check)
                                    2 MAKE_CELL                2 (rel)
                      
-                      65           4 RESUME                   0
+                      75           4 RESUME                   0
                      
-                      66           6 LOAD_CONST               1 ('val')
+                      76           6 LOAD_CONST               1 ('val')
                                    8 LOAD_GLOBAL              0 (dict)
                                   20 BUILD_TUPLE              2
-                                  22 LOAD_CONST               2 (<code object rel, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 66>)
+                                  22 LOAD_CONST               2 (<code object rel, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 76>)
                                   24 MAKE_FUNCTION            4 (annotations)
                                   26 STORE_DEREF              2 (rel)
                      
-                      68          28 LOAD_CLOSURE             2 (rel)
+                      78          28 LOAD_CLOSURE             2 (rel)
                                   30 BUILD_TUPLE              1
-                                  32 LOAD_CONST               3 (<code object check, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 68>)
+                                  32 LOAD_CONST               3 (<code object check, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 78>)
                                   34 MAKE_FUNCTION            8 (closure)
                                   36 STORE_DEREF              1 (check)
                      
-                      75          38 LOAD_CLOSURE             1 (check)
+                      85          38 LOAD_CLOSURE             1 (check)
                                   40 BUILD_TUPLE              1
-                                  42 LOAD_CONST               4 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 75>)
+                                  42 LOAD_CONST               4 (<code object <listcomp>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 85>)
                                   44 MAKE_FUNCTION            8 (closure)
                                   46 LOAD_FAST                0 (dct)
                                   48 LOAD_METHOD              1 (items)
                                   70 PRECALL                  0
                                   74 CALL                     0
                                   84 GET_ITER
                                   86 PRECALL                  0
@@ -715,17 +754,17 @@
                            nlocals   : 1
                            stacksize : 7
                            flags     : 19
                            code
                               0x970064017c006402190000000000000000009b0064037c006404190000
                               000000000000009b0064057c006406190000000000000000009b0064079d
                               075300
-                            66           0 RESUME                   0
+                            76           0 RESUME                   0
                            
-                            67           2 LOAD_CONST               1 ('<a class="m-1 py-1 px-2 badge bg-blue-lt lead" href="/')
+                            77           2 LOAD_CONST               1 ('<a class="m-1 py-1 px-2 badge bg-blue-lt lead" href="/')
                                          4 LOAD_FAST                0 (val)
                                          6 LOAD_CONST               2 ('type')
                                          8 BINARY_SUBSCR
                                         18 FORMAT_VALUE             0
                                         20 LOAD_CONST               3 ('/')
                                         22 LOAD_FAST                0 (val)
                                         24 LOAD_CONST               4 ('id')
@@ -750,15 +789,15 @@
                               '</a>'
                            names      ()
                            varnames   ('val',)
                            freevars   ()
                            cellvars   ()
                            filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                            name       'rel'
-                           firstlineno 66
+                           firstlineno 76
                            lnotab 0x0201
                         code
                            argcount  : 1
                            nlocals   : 1
                            stacksize : 4
                            flags     : 19
                            code
@@ -772,38 +811,38 @@
                               00723d64017c00640219000000000000000000a002000000000000000000
                               0000000000000000000000a6000000ab0000000000000000007600722164
                               03a004000000000000000000000000000000000000000088016601640484
                               087c004400a6000000ab000000000000000000a6010000ab010000000000
                               00000053007c005300
                                          0 COPY_FREE_VARS           1
                            
-                            68           2 RESUME                   0
+                            78           2 RESUME                   0
                            
-                            69           4 LOAD_GLOBAL              1 (NULL + isinstance)
+                            79           4 LOAD_GLOBAL              1 (NULL + isinstance)
                                         16 LOAD_FAST                0 (val)
                                         18 LOAD_GLOBAL              2 (dict)
                                         30 PRECALL                  2
                                         34 CALL                     2
                                         44 POP_JUMP_FORWARD_IF_FALSE    33 (to 112)
                                         46 LOAD_CONST               1 ('repr')
                                         48 LOAD_FAST                0 (val)
                                         50 LOAD_METHOD              2 (keys)
                                         72 PRECALL                  0
                                         76 CALL                     0
                                         86 CONTAINS_OP              0
                                         88 POP_JUMP_FORWARD_IF_FALSE    11 (to 112)
                            
-                            70          90 PUSH_NULL
+                            80          90 PUSH_NULL
                                         92 LOAD_DEREF               1 (rel)
                                         94 LOAD_FAST                0 (val)
                                         96 PRECALL                  1
                                        100 CALL                     1
                                        110 RETURN_VALUE
                            
-                            71     >>  112 LOAD_GLOBAL              1 (NULL + isinstance)
+                            81     >>  112 LOAD_GLOBAL              1 (NULL + isinstance)
                                        124 LOAD_FAST                0 (val)
                                        126 LOAD_GLOBAL              6 (list)
                                        138 PRECALL                  2
                                        142 CALL                     2
                                        152 POP_JUMP_FORWARD_IF_FALSE    90 (to 334)
                                        154 LOAD_FAST                0 (val)
                                        156 POP_JUMP_FORWARD_IF_FALSE    88 (to 334)
@@ -821,29 +860,29 @@
                                        218 BINARY_SUBSCR
                                        228 LOAD_METHOD              2 (keys)
                                        250 PRECALL                  0
                                        254 CALL                     0
                                        264 CONTAINS_OP              0
                                        266 POP_JUMP_FORWARD_IF_FALSE    33 (to 334)
                            
-                            72         268 LOAD_CONST               3 (' ')
+                            82         268 LOAD_CONST               3 (' ')
                                        270 LOAD_METHOD              4 (join)
                                        292 LOAD_CLOSURE             1 (rel)
                                        294 BUILD_TUPLE              1
-                                       296 LOAD_CONST               4 (<code object <genexpr>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 72>)
+                                       296 LOAD_CONST               4 (<code object <genexpr>, file "/Users/sol/www/femto-admin/femto_admin/admin.py", line 82>)
                                        298 MAKE_FUNCTION            8 (closure)
                                        300 LOAD_FAST                0 (val)
                                        302 GET_ITER
                                        304 PRECALL                  0
                                        308 CALL                     0
                                        318 PRECALL                  1
                                        322 CALL                     1
                                        332 RETURN_VALUE
                            
-                            73     >>  334 LOAD_FAST                0 (val)
+                            83     >>  334 LOAD_FAST                0 (val)
                                        336 RETURN_VALUE
                            consts
                               None
                               'repr'
                               0
                               ' '
                               code
@@ -852,15 +891,15 @@
                                  stacksize : 4
                                  flags     : 51
                                  code
                                     0x95014b00010097007c005d0f7d01020089027c01a6010000ab01000000
                                     00000000005600970101008c1064005300
                                                0 COPY_FREE_VARS           1
                                  
-                                  72           2 RETURN_GENERATOR
+                                  82           2 RETURN_GENERATOR
                                                4 POP_TOP
                                                6 RESUME                   0
                                                8 LOAD_FAST                0 (.0)
                                          >>   10 FOR_ITER                15 (to 42)
                                               12 STORE_FAST               1 (v)
                                               14 PUSH_NULL
                                               16 LOAD_DEREF               2 (rel)
@@ -877,35 +916,35 @@
                                     None
                                  names      ()
                                  varnames   ('.0', 'v')
                                  freevars   ('rel',)
                                  cellvars   ()
                                  filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                                  name       '<genexpr>'
-                                 firstlineno 72
+                                 firstlineno 82
                                  lnotab 0x
                            names      ('isinstance', 'dict', 'keys', 'list', 'join')
                            varnames   ('val',)
                            freevars   ('rel',)
                            cellvars   ()
                            filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                            name       'check'
-                           firstlineno 68
+                           firstlineno 78
                            lnotab 0x0401560116019c014201
                         code
                            argcount  : 1
                            nlocals   : 3
                            stacksize : 5
                            flags     : 19
                            code
                               0x9501970067007c005d105c0200007d017d02020089037c02a6010000ab
                               01000000000000000091028c115300
                                          0 COPY_FREE_VARS           1
                            
-                            75           2 RESUME                   0
+                            85           2 RESUME                   0
                                          4 BUILD_LIST               0
                                          6 LOAD_FAST                0 (.0)
                                    >>    8 FOR_ITER                16 (to 42)
                                         10 UNPACK_SEQUENCE          2
                                         14 STORE_FAST               1 (key)
                                         16 STORE_FAST               2 (val)
                                         18 PUSH_NULL
@@ -919,36 +958,36 @@
                            consts
                            names      ()
                            varnames   ('.0', 'key', 'val')
                            freevars   ('check',)
                            cellvars   ()
                            filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                            name       '<listcomp>'
-                           firstlineno 75
+                           firstlineno 85
                            lnotab 0x
                      names      ('dict', 'items')
                      varnames   ('dct',)
                      freevars   ()
                      cellvars   ('check', 'rel')
                      filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                      name       'render'
-                     firstlineno 65
+                     firstlineno 75
                      lnotab 0x060116020a07
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 7
                      flags     : 19
                      code
                         0x9501970067007c005d1a7d01020089027401000000000000000000007c
                         01a6010000ab010000000000000000a6010000ab01000000000000000091
                         028c1b5300
                                    0 COPY_FREE_VARS           1
                      
-                      79           2 RESUME                   0
+                      89           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                26 (to 62)
                                   10 STORE_FAST               1 (obj)
                                   12 PUSH_NULL
                                   14 LOAD_DEREF               2 (render)
                                   16 LOAD_GLOBAL              1 (NULL + jsonify)
@@ -963,37 +1002,36 @@
                      consts
                      names      ('jsonify',)
                      varnames   ('.0', 'obj')
                      freevars   ('render',)
                      cellvars   ()
                      filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                      name       '<listcomp>'
-                     firstlineno 79
+                     firstlineno 89
                      lnotab 0x
                   'data'
                names      ('dict', '_get_model', 'all', 'prefetch_related', '_meta', 'fetch_fields', 'JSONResponse')
                varnames   ('self', 'request', 'model', 'objects', 'data')
                freevars   ()
                cellvars   ('render',)
                filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
                name       'dt'
-               firstlineno 64
+               firstlineno 74
                lnotab 0x0801160c2a0158011c01
-            (False, 'Admin')
+            (False, 'Admin', None, None)
          names      ('__name__', '__module__', '__qualname__', 'bool', 'str', '__init__', 'start', 'Request', 'dash', 'index', 'dt', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
          name       'Admin'
-         firstlineno 11
-         lnotab 0x0c01161e0a060c070c09
+         firstlineno 16
+         lnotab 0x0c0124230a060c070c09
       'Admin'
-      None
-   names      ('jinja2', 'ChoiceLoader', 'FileSystemLoader', 'PackageLoader', 'starlette.requests', 'Request', 'starlette.responses', 'RedirectResponse', 'JSONResponse', 'starlette.routing', 'Mount', 'Route', 'starlette.staticfiles', 'StaticFiles', 'starlette.templating', 'Jinja2Templates', 'tortoise_api.api', 'Api', 'Model', 'tortoise_api.util', 'jsonify', 'Admin')
+   names      ('datetime', 'jinja2', 'ChoiceLoader', 'FileSystemLoader', 'PackageLoader', 'starlette.requests', 'Request', 'starlette.responses', 'RedirectResponse', 'JSONResponse', 'starlette.routing', 'Mount', 'Route', 'starlette.staticfiles', 'StaticFiles', 'starlette.templating', 'Jinja2Templates', 'tortoise_api.api', 'Api', 'Model', 'tortoise_api.util', 'jsonify', 'femto_admin', 'femto_admin.utils', '_fields', 'Admin')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/sol/www/femto-admin/femto_admin/admin.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020114010c01100110010c010c0110010c03
+   lnotab 0x00ff02010c0214010c01100110010c010c0110010c0208010c03
```

### Comparing `femto-admin-0.1.0/femto_admin/admin.py` & `femto-admin-0.1.1/femto_admin/admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,78 @@
+from datetime import datetime
+
 from jinja2 import ChoiceLoader, FileSystemLoader, PackageLoader
 from starlette.requests import Request
 from starlette.responses import RedirectResponse, JSONResponse
 from starlette.routing import Mount, Route
 from starlette.staticfiles import StaticFiles
 from starlette.templating import Jinja2Templates
 from tortoise_api.api import Api, Model
 from tortoise_api.util import jsonify
 
+import femto_admin
+from femto_admin.utils import _fields
+
 
 class Admin(Api):
-    def __init__(self, debug: bool = False, title: str = "Admin"):
+    def __init__(self, debug: bool = False, title: str = "Admin", static_dir: str = None, logo: str|bool = None):
         """
         Parameters:
             title: Admin title.
             # auth_provider: Authentication Provider
         """
         super().__init__(debug)
         self.title = title
         # self._views: List[BaseView] = []
         self.routes: [Route | Mount] = [
             Mount('/static', StaticFiles(packages=["femto_admin"]), name='public'),
             Mount('/api', routes=self.routes), # mount api routes to /api/*
             Route("/favicon.ico", lambda r: RedirectResponse('./static/placeholders/favicon.ico', status_code=301), methods=['GET']),
-            Route('/{model}', self.index, methods=['GET']),
-            Route('/dt/{model}', self.dt, methods=['GET']),
-            Route('/', self.dash, methods=['GET']),
+            Route('/{model}', self.index),
+            Route('/dt/{model}', self.dt),
+            Route('/', self.dash),
         ]
         self.routes[1].routes.pop(1)  # remove apt/favicon.ico route
         # globals
         templates = Jinja2Templates("templates")
+        if static_dir:
+            self.routes.append(Mount('/'+static_dir, StaticFiles(directory=static_dir), name='my-public'))
+            if logo is not None:
+                templates.env.globals["logo"] = logo
         templates.env.loader = ChoiceLoader(
             [
                 FileSystemLoader("templates"),
                 PackageLoader("femto_admin", "templates"),
             ]
         )
         templates.env.globals["title"] = self.title
+        templates.env.globals["meta"] = {'year': datetime.now().year, 'ver': femto_admin.__version__}
         templates.env.globals["minify"] = '' if debug else 'min.'
         self.templates = templates
 
     def start(self, models_module):
         app = super().start(models_module)
         self.templates.env.globals["models"] = self.models
         return app
 
     # INTERFACE
     async def dash(self, request: Request):
         return self.templates.TemplateResponse("dashboard.html", {
-            'title': 'Home',
+            'model': 'Home',
             'subtitle': 'Dashboard',
             'request': request,
         })
 
     async def index(self, request: Request):
-        model: Model = self._get_model(request)
+        model: type[Model] = self._get_model(request)
         return self.templates.TemplateResponse("table.html", {
-            'title': model.__name__,
+            'model': model.__name__,
             'subtitle': model._meta.table_description,
             'request': request,
-            'fields': {k: v for k, v in model._meta.fields_map.items() if not k.endswith('_id')}
+            'fields': _fields(model),
         })
 
     async def dt(self, request: Request):
         def render(dct: dict):
             def rel(val: dict):
                 return f'<a class="m-1 py-1 px-2 badge bg-blue-lt lead" href="/{val["type"]}/{val["id"]}">{val["repr"]}</a>'
             def check(val):
@@ -70,11 +80,11 @@
                     return rel(val)
                 elif isinstance(val, list) and val and isinstance(val[0], dict) and 'repr' in val[0].keys():
                     return ' '.join(rel(v) for v in val)
                 return val
 
             return [check(val) for key, val in dct.items()]
 
-        model: Model = self._get_model(request)
+        model: type[Model] = self._get_model(request)
         objects: [Model] = await model.all().prefetch_related(*model._meta.fetch_fields)
         data = [render(jsonify(obj)) for obj in objects]
         return JSONResponse({'data': data})
```

### Comparing `femto-admin-0.1.0/femto_admin/statics/placeholders/favicon.ico` & `femto-admin-0.1.1/femto_admin/statics/placeholders/favicon.ico`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/placeholders/users/admin.jpg` & `femto-admin-0.1.1/femto_admin/statics/placeholders/users/admin.jpg`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css` & `femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css` & `femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/css/dataTables.bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js` & `femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js` & `femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/js/dataTables.bootstrap5.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js` & `femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js` & `femto-admin-0.1.1/femto_admin/statics/vendor/DataTables/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/jQuery/jquery.js` & `femto-admin-0.1.1/femto_admin/statics/vendor/jQuery/jquery.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/jQuery/jquery.min.js` & `femto-admin-0.1.1/femto_admin/statics/vendor/jQuery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/tabler/css/tabler.css` & `femto-admin-0.1.1/femto_admin/statics/vendor/tabler/css/tabler.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/tabler/css/tabler.min.css` & `femto-admin-0.1.1/femto_admin/statics/vendor/tabler/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/dark-theme.js` & `femto-admin-0.1.1/femto_admin/statics/vendor/tabler/js/dark-theme.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/dark-theme.min.js` & `femto-admin-0.1.1/femto_admin/statics/vendor/tabler/js/dark-theme.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/tabler.js` & `femto-admin-0.1.1/femto_admin/statics/vendor/tabler/js/tabler.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/statics/vendor/tabler/js/tabler.min.js` & `femto-admin-0.1.1/femto_admin/statics/vendor/tabler/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `femto-admin-0.1.0/femto_admin/templates/table.html` & `femto-admin-0.1.1/femto_admin/templates/table.html`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 {% endblock %}
 
 {% block body %}
     <table id="dt" class="table table-striped" style="width:100%">
         <thead>
         <tr>
             {% for field in fields %}
-                <th>{{ field }}</th>
+                {% if not field.endswith('_id') %}
+                    <th>{{ field }}</th>
+                {% endif %}
             {% endfor %}
         </tr>
         </thead>
     </table>
 {% endblock %}
 
 {% block scripts %}
```

### Comparing `femto-admin-0.1.0/femto_admin.egg-info/PKG-INFO` & `femto-admin-0.1.1/femto_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femto-admin
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simplest fastest minimal ASGI CRUD Admin panel for Tortoise ORM models. It's generating fully native async auto  zero config one line app
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/femto-admin
 Project-URL: Repository, https://github.com/mixartemev/femto-admin
 Keywords: starlette,fastapi,admin,dashboard,datatables,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

