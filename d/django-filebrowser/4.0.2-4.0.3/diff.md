# Comparing `tmp/django-filebrowser-4.0.2.tar.gz` & `tmp/django-filebrowser-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-filebrowser-4.0.2.tar", last modified: Tue Nov 22 14:38:01 2022, max compression
+gzip compressed data, was "django-filebrowser-4.0.3.tar", last modified: Thu Jul 27 13:46:20 2023, max compression
```

## Comparing `django-filebrowser-4.0.2.tar` & `django-filebrowser-4.0.3.tar`

### file list

```diff
@@ -1,377 +1,377 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.908460 django-filebrowser-4.0.2/
--rw-r--r--   0 patrick    (501) staff       (20)      204 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/AUTHORS
--rw-r--r--   0 patrick    (501) staff       (20)     1539 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/LICENSE
--rw-r--r--   0 patrick    (501) staff       (20)      238 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/MANIFEST.in
--rw-r--r--   0 patrick    (501) staff       (20)     2700 2022-11-22 14:38:01.907866 django-filebrowser-4.0.2/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     1509 2022-11-22 14:37:29.000000 django-filebrowser-4.0.2/README.rst
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.414019 django-filebrowser-4.0.2/django_filebrowser.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)     2700 2022-11-22 14:38:01.000000 django-filebrowser-4.0.2/django_filebrowser.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)    11464 2022-11-22 14:38:01.000000 django-filebrowser-4.0.2/django_filebrowser.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2022-11-22 14:38:01.000000 django-filebrowser-4.0.2/django_filebrowser.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2016-03-06 15:41:04.000000 django-filebrowser-4.0.2/django_filebrowser.egg-info/not-zip-safe
--rw-r--r--   0 patrick    (501) staff       (20)       38 2022-11-22 14:38:01.000000 django-filebrowser-4.0.2/django_filebrowser.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)       18 2022-11-22 14:38:01.000000 django-filebrowser-4.0.2/django_filebrowser.egg-info/top_level.txt
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.429785 django-filebrowser-4.0.2/docs/
--rw-r--r--   0 patrick    (501) staff       (20)     4626 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/Makefile
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.469504 django-filebrowser-4.0.2/docs/_build/
--rw-r--r--   0 patrick    (501) staff       (20)      230 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/.buildinfo
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.502649 django-filebrowser-4.0.2/docs/_build/.doctrees/
--rw-r--r--   0 patrick    (501) staff       (20)    72153 2020-11-24 15:56:42.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/admin.doctree
--rw-r--r--   0 patrick    (501) staff       (20)     2959 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/api.doctree
--rw-r--r--   0 patrick    (501) staff       (20)     5720 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/changelog.doctree
--rw-r--r--   0 patrick    (501) staff       (20)    73500 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/environment.pickle
--rw-r--r--   0 patrick    (501) staff       (20)    12663 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/faq.doctree
--rw-r--r--   0 patrick    (501) staff       (20)    23852 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/fieldswidgets.doctree
--rw-r--r--   0 patrick    (501) staff       (20)    28289 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/filelisting.doctree
--rw-r--r--   0 patrick    (501) staff       (20)    65375 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/fileobject.doctree
--rw-r--r--   0 patrick    (501) staff       (20)     3001 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/help.doctree
--rw-r--r--   0 patrick    (501) staff       (20)    14772 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/index.doctree
--rw-r--r--   0 patrick    (501) staff       (20)    12583 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/quickstart.doctree
--rw-r--r--   0 patrick    (501) staff       (20)     5382 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/releasenotes.doctree
--rw-r--r--   0 patrick    (501) staff       (20)    48026 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/settings.doctree
--rw-r--r--   0 patrick    (501) staff       (20)     4663 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/testing.doctree
--rw-r--r--   0 patrick    (501) staff       (20)     4831 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/translation.doctree
--rw-r--r--   0 patrick    (501) staff       (20)    13282 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/troubleshooting.doctree
--rw-r--r--   0 patrick    (501) staff       (20)    31089 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/.doctrees/versions.doctree
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.557202 django-filebrowser-4.0.2/docs/_build/_sources/
--rw-r--r--   0 patrick    (501) staff       (20)    10819 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/_build/_sources/admin.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)    10819 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/_build/_sources/admin.txt
--rw-r--r--   0 patrick    (501) staff       (20)      145 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/_build/_sources/api.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)      145 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/_build/_sources/api.txt
--rw-r--r--   0 patrick    (501) staff       (20)      427 2020-11-24 15:55:08.000000 django-filebrowser-4.0.2/docs/_build/_sources/changelog.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)      793 2016-06-20 10:31:59.000000 django-filebrowser-4.0.2/docs/_build/_sources/changelog.txt
--rw-r--r--   0 patrick    (501) staff       (20)     1834 2017-07-13 14:28:48.000000 django-filebrowser-4.0.2/docs/_build/_sources/faq.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)     1833 2016-03-07 17:20:27.000000 django-filebrowser-4.0.2/docs/_build/_sources/faq.txt
--rw-r--r--   0 patrick    (501) staff       (20)     4417 2019-11-12 16:19:42.000000 django-filebrowser-4.0.2/docs/_build/_sources/fieldswidgets.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)     4173 2018-03-21 14:23:17.000000 django-filebrowser-4.0.2/docs/_build/_sources/fieldswidgets.txt
--rw-r--r--   0 patrick    (501) staff       (20)     4439 2016-04-15 12:55:07.000000 django-filebrowser-4.0.2/docs/_build/_sources/filelisting.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)     4439 2016-04-15 12:55:07.000000 django-filebrowser-4.0.2/docs/_build/_sources/filelisting.txt
--rw-r--r--   0 patrick    (501) staff       (20)     9071 2019-11-13 11:17:43.000000 django-filebrowser-4.0.2/docs/_build/_sources/fileobject.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)     8942 2016-06-20 10:31:59.000000 django-filebrowser-4.0.2/docs/_build/_sources/fileobject.txt
--rw-r--r--   0 patrick    (501) staff       (20)      175 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/_build/_sources/help.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)      175 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/_build/_sources/help.txt
--rw-r--r--   0 patrick    (501) staff       (20)     2397 2020-11-24 15:55:41.000000 django-filebrowser-4.0.2/docs/_build/_sources/index.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)     2387 2016-04-15 13:22:14.000000 django-filebrowser-4.0.2/docs/_build/_sources/index.txt
--rw-r--r--   0 patrick    (501) staff       (20)     1806 2020-11-24 15:54:16.000000 django-filebrowser-4.0.2/docs/_build/_sources/quickstart.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)     1826 2016-03-07 17:20:27.000000 django-filebrowser-4.0.2/docs/_build/_sources/quickstart.txt
--rw-r--r--   0 patrick    (501) staff       (20)      519 2020-05-15 09:48:51.000000 django-filebrowser-4.0.2/docs/_build/_sources/releasenotes.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)     1016 2016-03-07 17:20:27.000000 django-filebrowser-4.0.2/docs/_build/_sources/releasenotes.txt
--rw-r--r--   0 patrick    (501) staff       (20)     9270 2019-11-12 16:15:31.000000 django-filebrowser-4.0.2/docs/_build/_sources/settings.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)     9245 2016-06-20 11:31:05.000000 django-filebrowser-4.0.2/docs/_build/_sources/settings.txt
--rw-r--r--   0 patrick    (501) staff       (20)      407 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/_build/_sources/testing.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)      407 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/_build/_sources/testing.txt
--rw-r--r--   0 patrick    (501) staff       (20)      345 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/_build/_sources/translation.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)      345 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/_build/_sources/translation.txt
--rw-r--r--   0 patrick    (501) staff       (20)     1698 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/_build/_sources/troubleshooting.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)     1698 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/_build/_sources/troubleshooting.txt
--rw-r--r--   0 patrick    (501) staff       (20)     6809 2018-03-21 15:27:11.000000 django-filebrowser-4.0.2/docs/_build/_sources/versions.rst.txt
--rw-r--r--   0 patrick    (501) staff       (20)     6795 2016-06-20 10:31:59.000000 django-filebrowser-4.0.2/docs/_build/_sources/versions.txt
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.602092 django-filebrowser-4.0.2/docs/_build/_static/
--rw-r--r--   0 patrick    (501) staff       (20)      673 2016-01-10 15:47:00.000000 django-filebrowser-4.0.2/docs/_build/_static/ajax-loader.gif
--rw-r--r--   0 patrick    (501) staff       (20)    12261 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/_static/basic.css
--rw-r--r--   0 patrick    (501) staff       (20)      756 2018-11-01 15:15:08.000000 django-filebrowser-4.0.2/docs/_build/_static/comment-bright.png
--rw-r--r--   0 patrick    (501) staff       (20)      829 2018-11-01 15:15:08.000000 django-filebrowser-4.0.2/docs/_build/_static/comment-close.png
--rw-r--r--   0 patrick    (501) staff       (20)      641 2018-11-01 15:15:08.000000 django-filebrowser-4.0.2/docs/_build/_static/comment.png
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.605557 django-filebrowser-4.0.2/docs/_build/_static/css/
--rw-r--r--   0 patrick    (501) staff       (20)     3391 2019-12-27 14:10:17.000000 django-filebrowser-4.0.2/docs/_build/_static/css/badge_only.css
--rw-r--r--   0 patrick    (501) staff       (20)   118340 2019-12-27 14:10:17.000000 django-filebrowser-4.0.2/docs/_build/_static/css/theme.css
--rw-r--r--   0 patrick    (501) staff       (20)     9270 2019-12-27 14:10:00.000000 django-filebrowser-4.0.2/docs/_build/_static/doctools.js
--rw-r--r--   0 patrick    (501) staff       (20)      330 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/_static/documentation_options.js
--rw-r--r--   0 patrick    (501) staff       (20)      222 2018-11-01 15:15:08.000000 django-filebrowser-4.0.2/docs/_build/_static/down-pressed.png
--rw-r--r--   0 patrick    (501) staff       (20)      202 2018-11-01 15:15:08.000000 django-filebrowser-4.0.2/docs/_build/_static/down.png
--rw-r--r--   0 patrick    (501) staff       (20)      286 2018-11-01 15:15:08.000000 django-filebrowser-4.0.2/docs/_build/_static/file.png
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.654586 django-filebrowser-4.0.2/docs/_build/_static/fonts/
--rw-r--r--   0 patrick    (501) staff       (20)   109948 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Inconsolata-Bold.ttf
--rw-r--r--   0 patrick    (501) staff       (20)    96964 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Inconsolata-Regular.ttf
--rw-r--r--   0 patrick    (501) staff       (20)    63184 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Inconsolata.ttf
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.729652 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/
--rw-r--r--   0 patrick    (501) staff       (20)   256056 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bold.eot
--rw-r--r--   0 patrick    (501) staff       (20)   600856 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bold.ttf
--rw-r--r--   0 patrick    (501) staff       (20)   309728 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bold.woff
--rw-r--r--   0 patrick    (501) staff       (20)   184912 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bold.woff2
--rw-r--r--   0 patrick    (501) staff       (20)   266158 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bolditalic.eot
--rw-r--r--   0 patrick    (501) staff       (20)   622572 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bolditalic.ttf
--rw-r--r--   0 patrick    (501) staff       (20)   323344 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bolditalic.woff
--rw-r--r--   0 patrick    (501) staff       (20)   193308 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bolditalic.woff2
--rw-r--r--   0 patrick    (501) staff       (20)   268604 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-italic.eot
--rw-r--r--   0 patrick    (501) staff       (20)   639388 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-italic.ttf
--rw-r--r--   0 patrick    (501) staff       (20)   328412 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-italic.woff
--rw-r--r--   0 patrick    (501) staff       (20)   195704 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-italic.woff2
--rw-r--r--   0 patrick    (501) staff       (20)   253461 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-regular.eot
--rw-r--r--   0 patrick    (501) staff       (20)   607720 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-regular.ttf
--rw-r--r--   0 patrick    (501) staff       (20)   309192 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-regular.woff
--rw-r--r--   0 patrick    (501) staff       (20)   182708 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-regular.woff2
--rw-r--r--   0 patrick    (501) staff       (20)   656544 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato-Bold.ttf
--rw-r--r--   0 patrick    (501) staff       (20)   656568 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato-Regular.ttf
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.752514 django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/
--rw-r--r--   0 patrick    (501) staff       (20)    79520 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot
--rw-r--r--   0 patrick    (501) staff       (20)   170616 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
--rw-r--r--   0 patrick    (501) staff       (20)    87624 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
--rw-r--r--   0 patrick    (501) staff       (20)    67312 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
--rw-r--r--   0 patrick    (501) staff       (20)    78331 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
--rw-r--r--   0 patrick    (501) staff       (20)   169064 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
--rw-r--r--   0 patrick    (501) staff       (20)    86288 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
--rw-r--r--   0 patrick    (501) staff       (20)    66444 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
--rw-r--r--   0 patrick    (501) staff       (20)   170616 2016-01-10 15:47:09.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab-Bold.ttf
--rw-r--r--   0 patrick    (501) staff       (20)   169064 2016-01-10 15:47:09.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab-Regular.ttf
--rw-r--r--   0 patrick    (501) staff       (20)   165742 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 patrick    (501) staff       (20)   444379 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 patrick    (501) staff       (20)   165548 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 patrick    (501) staff       (20)    98024 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 patrick    (501) staff       (20)    77160 2018-11-01 15:15:22.000000 django-filebrowser-4.0.2/docs/_build/_static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 patrick    (501) staff       (20)   282766 2016-01-10 15:47:00.000000 django-filebrowser-4.0.2/docs/_build/_static/jquery-1.11.1.js
--rw-r--r--   0 patrick    (501) staff       (20)   268039 2018-11-01 15:15:08.000000 django-filebrowser-4.0.2/docs/_build/_static/jquery-3.2.1.js
--rw-r--r--   0 patrick    (501) staff       (20)   280364 2019-12-27 14:10:00.000000 django-filebrowser-4.0.2/docs/_build/_static/jquery-3.4.1.js
--rw-r--r--   0 patrick    (501) staff       (20)    88145 2019-12-27 14:10:00.000000 django-filebrowser-4.0.2/docs/_build/_static/jquery.js
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.754492 django-filebrowser-4.0.2/docs/_build/_static/js/
--rw-r--r--   0 patrick    (501) staff       (20)    15414 2016-01-10 15:47:09.000000 django-filebrowser-4.0.2/docs/_build/_static/js/modernizr.min.js
--rw-r--r--   0 patrick    (501) staff       (20)     4414 2019-12-27 14:10:17.000000 django-filebrowser-4.0.2/docs/_build/_static/js/theme.js
--rw-r--r--   0 patrick    (501) staff       (20)    10847 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/_static/language_data.js
--rw-r--r--   0 patrick    (501) staff       (20)       90 2018-11-01 15:15:08.000000 django-filebrowser-4.0.2/docs/_build/_static/minus.png
--rw-r--r--   0 patrick    (501) staff       (20)       90 2018-11-01 15:15:08.000000 django-filebrowser-4.0.2/docs/_build/_static/plus.png
--rw-r--r--   0 patrick    (501) staff       (20)     4395 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/_static/pygments.css
--rw-r--r--   0 patrick    (501) staff       (20)    16029 2019-12-27 14:10:00.000000 django-filebrowser-4.0.2/docs/_build/_static/searchtools.js
--rw-r--r--   0 patrick    (501) staff       (20)    35168 2016-01-10 15:47:00.000000 django-filebrowser-4.0.2/docs/_build/_static/underscore-1.3.1.js
--rw-r--r--   0 patrick    (501) staff       (20)    12140 2016-01-10 15:47:00.000000 django-filebrowser-4.0.2/docs/_build/_static/underscore.js
--rw-r--r--   0 patrick    (501) staff       (20)      214 2018-11-01 15:15:08.000000 django-filebrowser-4.0.2/docs/_build/_static/up-pressed.png
--rw-r--r--   0 patrick    (501) staff       (20)      203 2018-11-01 15:15:08.000000 django-filebrowser-4.0.2/docs/_build/_static/up.png
--rw-r--r--   0 patrick    (501) staff       (20)    25355 2018-11-01 15:15:08.000000 django-filebrowser-4.0.2/docs/_build/_static/websupport.js
--rw-r--r--   0 patrick    (501) staff       (20)    32961 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/admin.html
--rw-r--r--   0 patrick    (501) staff       (20)     7336 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/api.html
--rw-r--r--   0 patrick    (501) staff       (20)     6226 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/changelog.html
--rw-r--r--   0 patrick    (501) staff       (20)    10533 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/faq.html
--rw-r--r--   0 patrick    (501) staff       (20)    18695 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/fieldswidgets.html
--rw-r--r--   0 patrick    (501) staff       (20)    21373 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/filelisting.html
--rw-r--r--   0 patrick    (501) staff       (20)    37586 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/fileobject.html
--rw-r--r--   0 patrick    (501) staff       (20)    13180 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/genindex.html
--rw-r--r--   0 patrick    (501) staff       (20)     6401 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/help.html
--rw-r--r--   0 patrick    (501) staff       (20)    15152 2020-11-24 15:56:43.000000 django-filebrowser-4.0.2/docs/_build/index.html
--rw-r--r--   0 patrick    (501) staff       (20)     1255 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/objects.inv
--rw-r--r--   0 patrick    (501) staff       (20)    10587 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/quickstart.html
--rw-r--r--   0 patrick    (501) staff       (20)     7270 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/releasenotes.html
--rw-r--r--   0 patrick    (501) staff       (20)     5190 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/search.html
--rw-r--r--   0 patrick    (501) staff       (20)    15308 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/searchindex.js
--rw-r--r--   0 patrick    (501) staff       (20)    37450 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/settings.html
--rw-r--r--   0 patrick    (501) staff       (20)     6327 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/testing.html
--rw-r--r--   0 patrick    (501) staff       (20)     6823 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/translation.html
--rw-r--r--   0 patrick    (501) staff       (20)     9354 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/troubleshooting.html
--rw-r--r--   0 patrick    (501) staff       (20)    25973 2020-11-24 15:56:44.000000 django-filebrowser-4.0.2/docs/_build/versions.html
--rw-r--r--   0 patrick    (501) staff       (20)    10819 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/admin.rst
--rw-r--r--   0 patrick    (501) staff       (20)      145 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/api.rst
--rw-r--r--   0 patrick    (501) staff       (20)      421 2022-11-22 14:30:52.000000 django-filebrowser-4.0.2/docs/changelog.rst
--rw-r--r--   0 patrick    (501) staff       (20)     7402 2022-11-22 14:33:10.000000 django-filebrowser-4.0.2/docs/conf.py
--rw-r--r--   0 patrick    (501) staff       (20)     1834 2017-07-13 14:28:48.000000 django-filebrowser-4.0.2/docs/faq.rst
--rw-r--r--   0 patrick    (501) staff       (20)     4410 2022-01-12 12:55:43.000000 django-filebrowser-4.0.2/docs/fieldswidgets.rst
--rw-r--r--   0 patrick    (501) staff       (20)     4439 2016-04-15 12:55:07.000000 django-filebrowser-4.0.2/docs/filelisting.rst
--rw-r--r--   0 patrick    (501) staff       (20)     9071 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/docs/fileobject.rst
--rw-r--r--   0 patrick    (501) staff       (20)      175 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/help.rst
--rw-r--r--   0 patrick    (501) staff       (20)     2142 2022-11-22 14:37:19.000000 django-filebrowser-4.0.2/docs/index.rst
--rw-r--r--   0 patrick    (501) staff       (20)     1809 2021-04-22 12:36:27.000000 django-filebrowser-4.0.2/docs/quickstart.rst
--rw-r--r--   0 patrick    (501) staff       (20)      512 2022-01-12 13:18:33.000000 django-filebrowser-4.0.2/docs/releasenotes.rst
--rw-r--r--   0 patrick    (501) staff       (20)     9270 2019-11-12 16:15:31.000000 django-filebrowser-4.0.2/docs/settings.rst
--rw-r--r--   0 patrick    (501) staff       (20)      407 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/testing.rst
--rw-r--r--   0 patrick    (501) staff       (20)      345 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/translation.rst
--rw-r--r--   0 patrick    (501) staff       (20)     1698 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/docs/troubleshooting.rst
--rw-r--r--   0 patrick    (501) staff       (20)     6809 2018-03-21 15:27:11.000000 django-filebrowser-4.0.2/docs/versions.rst
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.769163 django-filebrowser-4.0.2/filebrowser/
--rw-r--r--   0 patrick    (501) staff       (20)       18 2022-11-22 14:33:10.000000 django-filebrowser-4.0.2/filebrowser/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     2770 2020-11-25 15:00:38.000000 django-filebrowser-4.0.2/filebrowser/actions.py
--rw-r--r--   0 patrick    (501) staff       (20)    18468 2020-11-25 15:00:38.000000 django-filebrowser-4.0.2/filebrowser/base.py
--rw-r--r--   0 patrick    (501) staff       (20)     2498 2022-01-12 13:18:33.000000 django-filebrowser-4.0.2/filebrowser/decorators.py
--rw-r--r--   0 patrick    (501) staff       (20)    10445 2020-11-25 15:00:38.000000 django-filebrowser-4.0.2/filebrowser/fields.py
--rw-r--r--   0 patrick    (501) staff       (20)     3597 2020-11-25 15:00:38.000000 django-filebrowser-4.0.2/filebrowser/forms.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.402220 django-filebrowser-4.0.2/filebrowser/locale/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.388928 django-filebrowser-4.0.2/filebrowser/locale/az/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.772393 django-filebrowser-4.0.2/filebrowser/locale/az/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     5022 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/az/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11151 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/az/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.389203 django-filebrowser-4.0.2/filebrowser/locale/bg_BG/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.777279 django-filebrowser-4.0.2/filebrowser/locale/bg_BG/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     7808 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/bg_BG/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    13102 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/bg_BG/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.389515 django-filebrowser-4.0.2/filebrowser/locale/ca/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.779645 django-filebrowser-4.0.2/filebrowser/locale/ca/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6466 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11694 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.389913 django-filebrowser-4.0.2/filebrowser/locale/cs/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.782530 django-filebrowser-4.0.2/filebrowser/locale/cs/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6600 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11989 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.390259 django-filebrowser-4.0.2/filebrowser/locale/de/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.784870 django-filebrowser-4.0.2/filebrowser/locale/de/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6694 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11944 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.390632 django-filebrowser-4.0.2/filebrowser/locale/en/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.787342 django-filebrowser-4.0.2/filebrowser/locale/en/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     4353 2019-11-14 14:50:57.000000 django-filebrowser-4.0.2/filebrowser/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    10889 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.390993 django-filebrowser-4.0.2/filebrowser/locale/es/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.791588 django-filebrowser-4.0.2/filebrowser/locale/es/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6472 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11865 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.391306 django-filebrowser-4.0.2/filebrowser/locale/es_CO/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.793944 django-filebrowser-4.0.2/filebrowser/locale/es_CO/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     4042 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/es_CO/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    10840 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/es_CO/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.391717 django-filebrowser-4.0.2/filebrowser/locale/fa/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.795614 django-filebrowser-4.0.2/filebrowser/locale/fa/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     7426 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    12720 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.392488 django-filebrowser-4.0.2/filebrowser/locale/fr/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.796963 django-filebrowser-4.0.2/filebrowser/locale/fr/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6899 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    12181 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.393367 django-filebrowser-4.0.2/filebrowser/locale/hu/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.798557 django-filebrowser-4.0.2/filebrowser/locale/hu/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6771 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    12006 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.394049 django-filebrowser-4.0.2/filebrowser/locale/is/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.800721 django-filebrowser-4.0.2/filebrowser/locale/is/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6304 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/is/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11649 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.395018 django-filebrowser-4.0.2/filebrowser/locale/it/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.803220 django-filebrowser-4.0.2/filebrowser/locale/it/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6461 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11777 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.395796 django-filebrowser-4.0.2/filebrowser/locale/ja/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.805163 django-filebrowser-4.0.2/filebrowser/locale/ja/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     7425 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    12684 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.396328 django-filebrowser-4.0.2/filebrowser/locale/ja_JP/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.810022 django-filebrowser-4.0.2/filebrowser/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     7439 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    12626 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.396910 django-filebrowser-4.0.2/filebrowser/locale/mn/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.811963 django-filebrowser-4.0.2/filebrowser/locale/mn/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     7916 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    13166 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/mn/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.397549 django-filebrowser-4.0.2/filebrowser/locale/nb/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.813882 django-filebrowser-4.0.2/filebrowser/locale/nb/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6480 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11694 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.398080 django-filebrowser-4.0.2/filebrowser/locale/nl/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.816964 django-filebrowser-4.0.2/filebrowser/locale/nl/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)      496 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)     9649 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.398529 django-filebrowser-4.0.2/filebrowser/locale/pl_PL/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.818788 django-filebrowser-4.0.2/filebrowser/locale/pl_PL/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6484 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11887 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/pl_PL/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.399005 django-filebrowser-4.0.2/filebrowser/locale/pt_BR/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.820379 django-filebrowser-4.0.2/filebrowser/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6613 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11917 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.399420 django-filebrowser-4.0.2/filebrowser/locale/ru_RU/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.821783 django-filebrowser-4.0.2/filebrowser/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     8120 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/ru_RU/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    13540 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/ru_RU/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.399919 django-filebrowser-4.0.2/filebrowser/locale/sk/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.823230 django-filebrowser-4.0.2/filebrowser/locale/sk/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6760 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    12021 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.400406 django-filebrowser-4.0.2/filebrowser/locale/sl_SI/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.824651 django-filebrowser-4.0.2/filebrowser/locale/sl_SI/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6048 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/sl_SI/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11584 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/sl_SI/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.400878 django-filebrowser-4.0.2/filebrowser/locale/sv/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.826304 django-filebrowser-4.0.2/filebrowser/locale/sv/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6400 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11612 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.401417 django-filebrowser-4.0.2/filebrowser/locale/tr_TR/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.828105 django-filebrowser-4.0.2/filebrowser/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6468 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11917 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/tr_TR/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.401926 django-filebrowser-4.0.2/filebrowser/locale/vi/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.829620 django-filebrowser-4.0.2/filebrowser/locale/vi/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6683 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11900 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.402382 django-filebrowser-4.0.2/filebrowser/locale/zh_CN/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.831262 django-filebrowser-4.0.2/filebrowser/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 patrick    (501) staff       (20)     6235 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 patrick    (501) staff       (20)    11503 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.832695 django-filebrowser-4.0.2/filebrowser/management/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/management/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      161 2016-03-07 10:19:11.000000 django-filebrowser-4.0.2/filebrowser/management/__init__.pyc
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.835372 django-filebrowser-4.0.2/filebrowser/management/__pycache__/
--rw-r--r--   0 patrick    (501) staff       (20)      158 2018-03-21 13:34:13.000000 django-filebrowser-4.0.2/filebrowser/management/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 patrick    (501) staff       (20)      177 2022-01-07 15:34:04.000000 django-filebrowser-4.0.2/filebrowser/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.838877 django-filebrowser-4.0.2/filebrowser/management/commands/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/management/commands/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.843210 django-filebrowser-4.0.2/filebrowser/management/commands/__pycache__/
--rw-r--r--   0 patrick    (501) staff       (20)      167 2018-03-21 13:34:13.000000 django-filebrowser-4.0.2/filebrowser/management/commands/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 patrick    (501) staff       (20)      186 2022-01-07 15:34:04.000000 django-filebrowser-4.0.2/filebrowser/management/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 patrick    (501) staff       (20)     3833 2020-05-15 09:48:51.000000 django-filebrowser-4.0.2/filebrowser/management/commands/fb_version_generate.py
--rw-r--r--   0 patrick    (501) staff       (20)     5126 2020-05-15 09:48:51.000000 django-filebrowser-4.0.2/filebrowser/management/commands/fb_version_remove.py
--rw-r--r--   0 patrick    (501) staff       (20)       51 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/models.py
--rw-r--r--   0 patrick    (501) staff       (20)     3090 2020-05-15 09:48:51.000000 django-filebrowser-4.0.2/filebrowser/namers.py
--rw-r--r--   0 patrick    (501) staff       (20)     5605 2020-11-25 15:00:38.000000 django-filebrowser-4.0.2/filebrowser/settings.py
--rw-r--r--   0 patrick    (501) staff       (20)     1238 2022-01-12 12:55:43.000000 django-filebrowser-4.0.2/filebrowser/signals.py
--rw-r--r--   0 patrick    (501) staff       (20)    25187 2022-01-12 13:18:33.000000 django-filebrowser-4.0.2/filebrowser/sites.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.404030 django-filebrowser-4.0.2/filebrowser/static/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.404831 django-filebrowser-4.0.2/filebrowser/static/filebrowser/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.845459 django-filebrowser-4.0.2/filebrowser/static/filebrowser/css/
--rw-r--r--   0 patrick    (501) staff       (20)    11293 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/css/filebrowser.css
--rw-r--r--   0 patrick    (501) staff       (20)     4949 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/css/uploadfield.css
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.860082 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/
--rw-r--r--   0 patrick    (501) staff       (20)   870037 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/TEST_IMAGE_000.jpg
--rw-r--r--   0 patrick    (501) staff       (20)      236 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/cancel.png
--rw-r--r--   0 patrick    (501) staff       (20)      236 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/cancel_hover.png
--rw-r--r--   0 patrick    (501) staff       (20)     1122 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/completed.png
--rw-r--r--   0 patrick    (501) staff       (20)     3027 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/fb-upload-spinner.gif
--rw-r--r--   0 patrick    (501) staff       (20)     1090 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/fb-upload.png
--rw-r--r--   0 patrick    (501) staff       (20)     1091 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/fb-upload_hover.png
--rw-r--r--   0 patrick    (501) staff       (20)      165 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/icon-pulldown-versions-active.png
--rw-r--r--   0 patrick    (501) staff       (20)      165 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/icon-pulldown-versions-hover.png
--rw-r--r--   0 patrick    (501) staff       (20)      165 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/icon-pulldown-versions.png
--rw-r--r--   0 patrick    (501) staff       (20)      367 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/progress-bar-content.png
--rw-r--r--   0 patrick    (501) staff       (20)   870037 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/testimage.jpg
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.878253 django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/
--rw-r--r--   0 patrick    (501) staff       (20)     1474 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/AddFileBrowser.js
--rw-r--r--   0 patrick    (501) staff       (20)      622 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/FB_CKEditor.js
--rw-r--r--   0 patrick    (501) staff       (20)     1351 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/FB_FileBrowseField.js
--rw-r--r--   0 patrick    (501) staff       (20)      942 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/FB_TinyMCE.js
--rw-r--r--   0 patrick    (501) staff       (20)      649 2019-11-11 12:20:07.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/FB_TinyMCEv4.js
--rw-r--r--   0 patrick    (501) staff       (20)      198 2020-11-25 15:00:38.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/FB_TinyMCEv5.js
--rw-r--r--   0 patrick    (501) staff       (20)     5651 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/TinyMCEAdmin.js
--rw-r--r--   0 patrick    (501) staff       (20)     1288 2021-04-22 11:22:43.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/TinyMCEv5Admin.js
--rw-r--r--   0 patrick    (501) staff       (20)    40071 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/fileuploader.js
--rw-r--r--   0 patrick    (501) staff       (20)     3922 2020-05-15 09:48:51.000000 django-filebrowser-4.0.2/filebrowser/storage.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.405418 django-filebrowser-4.0.2/filebrowser/templates/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.887507 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/
--rw-r--r--   0 patrick    (501) staff       (20)     2522 2020-11-25 15:00:38.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/createdir.html
--rw-r--r--   0 patrick    (501) staff       (20)     1632 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/custom_field.html
--rw-r--r--   0 patrick    (501) staff       (20)     5151 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/custom_upload_field.html
--rw-r--r--   0 patrick    (501) staff       (20)     2222 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/delete_confirm.html
--rw-r--r--   0 patrick    (501) staff       (20)     8100 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/detail.html
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.892729 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/
--rw-r--r--   0 patrick    (501) staff       (20)       14 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/_response.html
--rw-r--r--   0 patrick    (501) staff       (20)     1078 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/breadcrumbs.html
--rw-r--r--   0 patrick    (501) staff       (20)     7038 2020-11-25 15:00:38.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/filelisting.html
--rw-r--r--   0 patrick    (501) staff       (20)     2540 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/filter.html
--rw-r--r--   0 patrick    (501) staff       (20)     1522 2022-01-12 12:55:43.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/paginator.html
--rw-r--r--   0 patrick    (501) staff       (20)     2837 2022-01-12 12:55:43.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/tableheader.html
--rw-r--r--   0 patrick    (501) staff       (20)     2078 2019-11-14 14:54:08.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/toolbar.html
--rw-r--r--   0 patrick    (501) staff       (20)     7529 2022-01-12 12:55:43.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/index.html
--rw-r--r--   0 patrick    (501) staff       (20)     7326 2022-01-12 13:18:27.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/upload.html
--rw-r--r--   0 patrick    (501) staff       (20)     2804 2022-01-12 12:55:43.000000 django-filebrowser-4.0.2/filebrowser/templates/filebrowser/version.html
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.895511 django-filebrowser-4.0.2/filebrowser/templatetags/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/templatetags/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     1041 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/templatetags/fb_csrf.py
--rw-r--r--   0 patrick    (501) staff       (20)     1740 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/filebrowser/templatetags/fb_pagination.py
--rw-r--r--   0 patrick    (501) staff       (20)     4668 2022-01-12 13:18:33.000000 django-filebrowser-4.0.2/filebrowser/templatetags/fb_tags.py
--rw-r--r--   0 patrick    (501) staff       (20)     4353 2018-09-24 14:10:49.000000 django-filebrowser-4.0.2/filebrowser/templatetags/fb_versions.py
--rw-r--r--   0 patrick    (501) staff       (20)     3054 2020-05-15 09:48:51.000000 django-filebrowser-4.0.2/filebrowser/utils.py
--rw-r--r--   0 patrick    (501) staff       (20)       38 2022-11-22 14:38:01.908668 django-filebrowser-4.0.2/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)     1215 2022-11-22 14:33:10.000000 django-filebrowser-4.0.2/setup.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2022-11-22 14:38:01.905940 django-filebrowser-4.0.2/tests/
--rw-r--r--   0 patrick    (501) staff       (20)     2305 2016-03-07 17:20:27.000000 django-filebrowser-4.0.2/tests/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     2881 2018-03-21 15:27:11.000000 django-filebrowser-4.0.2/tests/settings.py
--rw-r--r--   0 patrick    (501) staff       (20)    21436 2020-05-15 09:48:51.000000 django-filebrowser-4.0.2/tests/test_base.py
--rw-r--r--   0 patrick    (501) staff       (20)     1006 2020-05-15 09:48:51.000000 django-filebrowser-4.0.2/tests/test_commands.py
--rw-r--r--   0 patrick    (501) staff       (20)     1948 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/tests/test_decorators.py
--rw-r--r--   0 patrick    (501) staff       (20)     3478 2016-08-09 13:19:40.000000 django-filebrowser-4.0.2/tests/test_namers.py
--rw-r--r--   0 patrick    (501) staff       (20)     3451 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/tests/test_settings.py
--rw-r--r--   0 patrick    (501) staff       (20)    13850 2019-11-14 15:49:45.000000 django-filebrowser-4.0.2/tests/test_sites.py
--rw-r--r--   0 patrick    (501) staff       (20)      798 2016-03-06 14:43:09.000000 django-filebrowser-4.0.2/tests/test_templatetags.py
--rw-r--r--   0 patrick    (501) staff       (20)    22014 2016-08-09 13:19:40.000000 django-filebrowser-4.0.2/tests/test_versions.py
--rw-r--r--   0 patrick    (501) staff       (20)      279 2018-03-21 15:27:11.000000 django-filebrowser-4.0.2/tests/urls.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.064845 django-filebrowser-4.0.3/
+-rw-r--r--   0 patrick    (501) staff       (20)      204 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/AUTHORS
+-rw-r--r--   0 patrick    (501) staff       (20)     1539 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/LICENSE
+-rw-r--r--   0 patrick    (501) staff       (20)      238 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/MANIFEST.in
+-rw-r--r--   0 patrick    (501) staff       (20)     2784 2023-07-27 13:46:20.064627 django-filebrowser-4.0.3/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     1593 2023-07-27 13:45:03.000000 django-filebrowser-4.0.3/README.rst
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.958442 django-filebrowser-4.0.3/django_filebrowser.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)     2784 2023-07-27 13:46:19.000000 django-filebrowser-4.0.3/django_filebrowser.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)    11464 2023-07-27 13:46:19.000000 django-filebrowser-4.0.3/django_filebrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-07-27 13:46:19.000000 django-filebrowser-4.0.3/django_filebrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2016-03-06 15:41:04.000000 django-filebrowser-4.0.3/django_filebrowser.egg-info/not-zip-safe
+-rw-r--r--   0 patrick    (501) staff       (20)       38 2023-07-27 13:46:19.000000 django-filebrowser-4.0.3/django_filebrowser.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       18 2023-07-27 13:46:19.000000 django-filebrowser-4.0.3/django_filebrowser.egg-info/top_level.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.961949 django-filebrowser-4.0.3/docs/
+-rw-r--r--   0 patrick    (501) staff       (20)     4626 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/Makefile
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.967098 django-filebrowser-4.0.3/docs/_build/
+-rw-r--r--   0 patrick    (501) staff       (20)      230 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/.buildinfo
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.970648 django-filebrowser-4.0.3/docs/_build/.doctrees/
+-rw-r--r--   0 patrick    (501) staff       (20)    72153 2020-11-24 15:56:42.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/admin.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)     2959 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/api.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)     5720 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/changelog.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)    73500 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/environment.pickle
+-rw-r--r--   0 patrick    (501) staff       (20)    12663 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/faq.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)    23852 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/fieldswidgets.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)    28289 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/filelisting.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)    65375 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/fileobject.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)     3001 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/help.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)    14772 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/index.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)    12583 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/quickstart.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)     5382 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/releasenotes.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)    48026 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/settings.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)     4663 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/testing.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)     4831 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/translation.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)    13282 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/troubleshooting.doctree
+-rw-r--r--   0 patrick    (501) staff       (20)    31089 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/.doctrees/versions.doctree
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.976299 django-filebrowser-4.0.3/docs/_build/_sources/
+-rw-r--r--   0 patrick    (501) staff       (20)    10819 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/_build/_sources/admin.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)    10819 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/_build/_sources/admin.txt
+-rw-r--r--   0 patrick    (501) staff       (20)      145 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/_build/_sources/api.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)      145 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/_build/_sources/api.txt
+-rw-r--r--   0 patrick    (501) staff       (20)      427 2020-11-24 15:55:08.000000 django-filebrowser-4.0.3/docs/_build/_sources/changelog.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)      793 2016-06-20 10:31:59.000000 django-filebrowser-4.0.3/docs/_build/_sources/changelog.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     1834 2017-07-13 14:28:48.000000 django-filebrowser-4.0.3/docs/_build/_sources/faq.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     1833 2016-03-07 17:20:27.000000 django-filebrowser-4.0.3/docs/_build/_sources/faq.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     4417 2019-11-12 16:19:42.000000 django-filebrowser-4.0.3/docs/_build/_sources/fieldswidgets.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     4173 2018-03-21 14:23:17.000000 django-filebrowser-4.0.3/docs/_build/_sources/fieldswidgets.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     4439 2016-04-15 12:55:07.000000 django-filebrowser-4.0.3/docs/_build/_sources/filelisting.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     4439 2016-04-15 12:55:07.000000 django-filebrowser-4.0.3/docs/_build/_sources/filelisting.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     9071 2019-11-13 11:17:43.000000 django-filebrowser-4.0.3/docs/_build/_sources/fileobject.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     8942 2016-06-20 10:31:59.000000 django-filebrowser-4.0.3/docs/_build/_sources/fileobject.txt
+-rw-r--r--   0 patrick    (501) staff       (20)      175 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/_build/_sources/help.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)      175 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/_build/_sources/help.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     2397 2020-11-24 15:55:41.000000 django-filebrowser-4.0.3/docs/_build/_sources/index.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     2387 2016-04-15 13:22:14.000000 django-filebrowser-4.0.3/docs/_build/_sources/index.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     1806 2020-11-24 15:54:16.000000 django-filebrowser-4.0.3/docs/_build/_sources/quickstart.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     1826 2016-03-07 17:20:27.000000 django-filebrowser-4.0.3/docs/_build/_sources/quickstart.txt
+-rw-r--r--   0 patrick    (501) staff       (20)      519 2020-05-15 09:48:51.000000 django-filebrowser-4.0.3/docs/_build/_sources/releasenotes.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     1016 2016-03-07 17:20:27.000000 django-filebrowser-4.0.3/docs/_build/_sources/releasenotes.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     9270 2019-11-12 16:15:31.000000 django-filebrowser-4.0.3/docs/_build/_sources/settings.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     9245 2016-06-20 11:31:05.000000 django-filebrowser-4.0.3/docs/_build/_sources/settings.txt
+-rw-r--r--   0 patrick    (501) staff       (20)      407 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/_build/_sources/testing.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)      407 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/_build/_sources/testing.txt
+-rw-r--r--   0 patrick    (501) staff       (20)      345 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/_build/_sources/translation.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)      345 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/_build/_sources/translation.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     1698 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/_build/_sources/troubleshooting.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     1698 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/_build/_sources/troubleshooting.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     6809 2018-03-21 15:27:11.000000 django-filebrowser-4.0.3/docs/_build/_sources/versions.rst.txt
+-rw-r--r--   0 patrick    (501) staff       (20)     6795 2016-06-20 10:31:59.000000 django-filebrowser-4.0.3/docs/_build/_sources/versions.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.982430 django-filebrowser-4.0.3/docs/_build/_static/
+-rw-r--r--   0 patrick    (501) staff       (20)      673 2016-01-10 15:47:00.000000 django-filebrowser-4.0.3/docs/_build/_static/ajax-loader.gif
+-rw-r--r--   0 patrick    (501) staff       (20)    12261 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/_static/basic.css
+-rw-r--r--   0 patrick    (501) staff       (20)      756 2018-11-01 15:15:08.000000 django-filebrowser-4.0.3/docs/_build/_static/comment-bright.png
+-rw-r--r--   0 patrick    (501) staff       (20)      829 2018-11-01 15:15:08.000000 django-filebrowser-4.0.3/docs/_build/_static/comment-close.png
+-rw-r--r--   0 patrick    (501) staff       (20)      641 2018-11-01 15:15:08.000000 django-filebrowser-4.0.3/docs/_build/_static/comment.png
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.983446 django-filebrowser-4.0.3/docs/_build/_static/css/
+-rw-r--r--   0 patrick    (501) staff       (20)     3391 2019-12-27 14:10:17.000000 django-filebrowser-4.0.3/docs/_build/_static/css/badge_only.css
+-rw-r--r--   0 patrick    (501) staff       (20)   118340 2019-12-27 14:10:17.000000 django-filebrowser-4.0.3/docs/_build/_static/css/theme.css
+-rw-r--r--   0 patrick    (501) staff       (20)     9270 2019-12-27 14:10:00.000000 django-filebrowser-4.0.3/docs/_build/_static/doctools.js
+-rw-r--r--   0 patrick    (501) staff       (20)      330 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/_static/documentation_options.js
+-rw-r--r--   0 patrick    (501) staff       (20)      222 2018-11-01 15:15:08.000000 django-filebrowser-4.0.3/docs/_build/_static/down-pressed.png
+-rw-r--r--   0 patrick    (501) staff       (20)      202 2018-11-01 15:15:08.000000 django-filebrowser-4.0.3/docs/_build/_static/down.png
+-rw-r--r--   0 patrick    (501) staff       (20)      286 2018-11-01 15:15:08.000000 django-filebrowser-4.0.3/docs/_build/_static/file.png
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.991681 django-filebrowser-4.0.3/docs/_build/_static/fonts/
+-rw-r--r--   0 patrick    (501) staff       (20)   109948 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Inconsolata-Bold.ttf
+-rw-r--r--   0 patrick    (501) staff       (20)    96964 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Inconsolata-Regular.ttf
+-rw-r--r--   0 patrick    (501) staff       (20)    63184 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Inconsolata.ttf
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.009430 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/
+-rw-r--r--   0 patrick    (501) staff       (20)   256056 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bold.eot
+-rw-r--r--   0 patrick    (501) staff       (20)   600856 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bold.ttf
+-rw-r--r--   0 patrick    (501) staff       (20)   309728 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bold.woff
+-rw-r--r--   0 patrick    (501) staff       (20)   184912 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bold.woff2
+-rw-r--r--   0 patrick    (501) staff       (20)   266158 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bolditalic.eot
+-rw-r--r--   0 patrick    (501) staff       (20)   622572 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bolditalic.ttf
+-rw-r--r--   0 patrick    (501) staff       (20)   323344 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bolditalic.woff
+-rw-r--r--   0 patrick    (501) staff       (20)   193308 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bolditalic.woff2
+-rw-r--r--   0 patrick    (501) staff       (20)   268604 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-italic.eot
+-rw-r--r--   0 patrick    (501) staff       (20)   639388 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-italic.ttf
+-rw-r--r--   0 patrick    (501) staff       (20)   328412 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-italic.woff
+-rw-r--r--   0 patrick    (501) staff       (20)   195704 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-italic.woff2
+-rw-r--r--   0 patrick    (501) staff       (20)   253461 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-regular.eot
+-rw-r--r--   0 patrick    (501) staff       (20)   607720 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-regular.ttf
+-rw-r--r--   0 patrick    (501) staff       (20)   309192 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-regular.woff
+-rw-r--r--   0 patrick    (501) staff       (20)   182708 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-regular.woff2
+-rw-r--r--   0 patrick    (501) staff       (20)   656544 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato-Bold.ttf
+-rw-r--r--   0 patrick    (501) staff       (20)   656568 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato-Regular.ttf
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.013949 django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/
+-rw-r--r--   0 patrick    (501) staff       (20)    79520 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot
+-rw-r--r--   0 patrick    (501) staff       (20)   170616 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
+-rw-r--r--   0 patrick    (501) staff       (20)    87624 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
+-rw-r--r--   0 patrick    (501) staff       (20)    67312 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
+-rw-r--r--   0 patrick    (501) staff       (20)    78331 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
+-rw-r--r--   0 patrick    (501) staff       (20)   169064 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
+-rw-r--r--   0 patrick    (501) staff       (20)    86288 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
+-rw-r--r--   0 patrick    (501) staff       (20)    66444 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
+-rw-r--r--   0 patrick    (501) staff       (20)   170616 2016-01-10 15:47:09.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab-Bold.ttf
+-rw-r--r--   0 patrick    (501) staff       (20)   169064 2016-01-10 15:47:09.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab-Regular.ttf
+-rw-r--r--   0 patrick    (501) staff       (20)   165742 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 patrick    (501) staff       (20)   444379 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 patrick    (501) staff       (20)   165548 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 patrick    (501) staff       (20)    98024 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 patrick    (501) staff       (20)    77160 2018-11-01 15:15:22.000000 django-filebrowser-4.0.3/docs/_build/_static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 patrick    (501) staff       (20)   282766 2016-01-10 15:47:00.000000 django-filebrowser-4.0.3/docs/_build/_static/jquery-1.11.1.js
+-rw-r--r--   0 patrick    (501) staff       (20)   268039 2018-11-01 15:15:08.000000 django-filebrowser-4.0.3/docs/_build/_static/jquery-3.2.1.js
+-rw-r--r--   0 patrick    (501) staff       (20)   280364 2019-12-27 14:10:00.000000 django-filebrowser-4.0.3/docs/_build/_static/jquery-3.4.1.js
+-rw-r--r--   0 patrick    (501) staff       (20)    88145 2019-12-27 14:10:00.000000 django-filebrowser-4.0.3/docs/_build/_static/jquery.js
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.014842 django-filebrowser-4.0.3/docs/_build/_static/js/
+-rw-r--r--   0 patrick    (501) staff       (20)    15414 2016-01-10 15:47:09.000000 django-filebrowser-4.0.3/docs/_build/_static/js/modernizr.min.js
+-rw-r--r--   0 patrick    (501) staff       (20)     4414 2019-12-27 14:10:17.000000 django-filebrowser-4.0.3/docs/_build/_static/js/theme.js
+-rw-r--r--   0 patrick    (501) staff       (20)    10847 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/_static/language_data.js
+-rw-r--r--   0 patrick    (501) staff       (20)       90 2018-11-01 15:15:08.000000 django-filebrowser-4.0.3/docs/_build/_static/minus.png
+-rw-r--r--   0 patrick    (501) staff       (20)       90 2018-11-01 15:15:08.000000 django-filebrowser-4.0.3/docs/_build/_static/plus.png
+-rw-r--r--   0 patrick    (501) staff       (20)     4395 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/_static/pygments.css
+-rw-r--r--   0 patrick    (501) staff       (20)    16029 2019-12-27 14:10:00.000000 django-filebrowser-4.0.3/docs/_build/_static/searchtools.js
+-rw-r--r--   0 patrick    (501) staff       (20)    35168 2016-01-10 15:47:00.000000 django-filebrowser-4.0.3/docs/_build/_static/underscore-1.3.1.js
+-rw-r--r--   0 patrick    (501) staff       (20)    12140 2016-01-10 15:47:00.000000 django-filebrowser-4.0.3/docs/_build/_static/underscore.js
+-rw-r--r--   0 patrick    (501) staff       (20)      214 2018-11-01 15:15:08.000000 django-filebrowser-4.0.3/docs/_build/_static/up-pressed.png
+-rw-r--r--   0 patrick    (501) staff       (20)      203 2018-11-01 15:15:08.000000 django-filebrowser-4.0.3/docs/_build/_static/up.png
+-rw-r--r--   0 patrick    (501) staff       (20)    25355 2018-11-01 15:15:08.000000 django-filebrowser-4.0.3/docs/_build/_static/websupport.js
+-rw-r--r--   0 patrick    (501) staff       (20)    32961 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/admin.html
+-rw-r--r--   0 patrick    (501) staff       (20)     7336 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/api.html
+-rw-r--r--   0 patrick    (501) staff       (20)     6226 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/changelog.html
+-rw-r--r--   0 patrick    (501) staff       (20)    10533 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/faq.html
+-rw-r--r--   0 patrick    (501) staff       (20)    18695 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/fieldswidgets.html
+-rw-r--r--   0 patrick    (501) staff       (20)    21373 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/filelisting.html
+-rw-r--r--   0 patrick    (501) staff       (20)    37586 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/fileobject.html
+-rw-r--r--   0 patrick    (501) staff       (20)    13180 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/genindex.html
+-rw-r--r--   0 patrick    (501) staff       (20)     6401 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/help.html
+-rw-r--r--   0 patrick    (501) staff       (20)    15152 2020-11-24 15:56:43.000000 django-filebrowser-4.0.3/docs/_build/index.html
+-rw-r--r--   0 patrick    (501) staff       (20)     1255 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/objects.inv
+-rw-r--r--   0 patrick    (501) staff       (20)    10587 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/quickstart.html
+-rw-r--r--   0 patrick    (501) staff       (20)     7270 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/releasenotes.html
+-rw-r--r--   0 patrick    (501) staff       (20)     5190 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/search.html
+-rw-r--r--   0 patrick    (501) staff       (20)    15308 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/searchindex.js
+-rw-r--r--   0 patrick    (501) staff       (20)    37450 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/settings.html
+-rw-r--r--   0 patrick    (501) staff       (20)     6327 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/testing.html
+-rw-r--r--   0 patrick    (501) staff       (20)     6823 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/translation.html
+-rw-r--r--   0 patrick    (501) staff       (20)     9354 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/troubleshooting.html
+-rw-r--r--   0 patrick    (501) staff       (20)    25973 2020-11-24 15:56:44.000000 django-filebrowser-4.0.3/docs/_build/versions.html
+-rw-r--r--   0 patrick    (501) staff       (20)    10819 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/admin.rst
+-rw-r--r--   0 patrick    (501) staff       (20)      145 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/api.rst
+-rw-r--r--   0 patrick    (501) staff       (20)      616 2023-07-27 13:45:03.000000 django-filebrowser-4.0.3/docs/changelog.rst
+-rw-r--r--   0 patrick    (501) staff       (20)     7402 2023-07-27 13:45:03.000000 django-filebrowser-4.0.3/docs/conf.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1834 2017-07-13 14:28:48.000000 django-filebrowser-4.0.3/docs/faq.rst
+-rw-r--r--   0 patrick    (501) staff       (20)     4410 2022-01-12 12:55:43.000000 django-filebrowser-4.0.3/docs/fieldswidgets.rst
+-rw-r--r--   0 patrick    (501) staff       (20)     4439 2016-04-15 12:55:07.000000 django-filebrowser-4.0.3/docs/filelisting.rst
+-rw-r--r--   0 patrick    (501) staff       (20)     9071 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/docs/fileobject.rst
+-rw-r--r--   0 patrick    (501) staff       (20)      175 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/help.rst
+-rw-r--r--   0 patrick    (501) staff       (20)     2101 2023-07-27 13:45:03.000000 django-filebrowser-4.0.3/docs/index.rst
+-rw-r--r--   0 patrick    (501) staff       (20)     1809 2021-04-22 12:36:27.000000 django-filebrowser-4.0.3/docs/quickstart.rst
+-rw-r--r--   0 patrick    (501) staff       (20)      512 2022-01-12 13:18:33.000000 django-filebrowser-4.0.3/docs/releasenotes.rst
+-rw-r--r--   0 patrick    (501) staff       (20)     9270 2019-11-12 16:15:31.000000 django-filebrowser-4.0.3/docs/settings.rst
+-rw-r--r--   0 patrick    (501) staff       (20)      407 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/testing.rst
+-rw-r--r--   0 patrick    (501) staff       (20)      345 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/translation.rst
+-rw-r--r--   0 patrick    (501) staff       (20)     1698 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/docs/troubleshooting.rst
+-rw-r--r--   0 patrick    (501) staff       (20)     6809 2018-03-21 15:27:11.000000 django-filebrowser-4.0.3/docs/versions.rst
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.019597 django-filebrowser-4.0.3/filebrowser/
+-rw-r--r--   0 patrick    (501) staff       (20)       18 2023-07-27 13:45:03.000000 django-filebrowser-4.0.3/filebrowser/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2770 2020-11-25 15:00:38.000000 django-filebrowser-4.0.3/filebrowser/actions.py
+-rw-r--r--   0 patrick    (501) staff       (20)    18468 2020-11-25 15:00:38.000000 django-filebrowser-4.0.3/filebrowser/base.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2498 2022-01-12 13:18:33.000000 django-filebrowser-4.0.3/filebrowser/decorators.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10445 2020-11-25 15:00:38.000000 django-filebrowser-4.0.3/filebrowser/fields.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3597 2020-11-25 15:00:38.000000 django-filebrowser-4.0.3/filebrowser/forms.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.955949 django-filebrowser-4.0.3/filebrowser/locale/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.953201 django-filebrowser-4.0.3/filebrowser/locale/az/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.020316 django-filebrowser-4.0.3/filebrowser/locale/az/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     5022 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/az/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11151 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/az/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.953315 django-filebrowser-4.0.3/filebrowser/locale/bg_BG/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.021144 django-filebrowser-4.0.3/filebrowser/locale/bg_BG/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     7808 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/bg_BG/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    13102 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/bg_BG/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.953425 django-filebrowser-4.0.3/filebrowser/locale/ca/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.021978 django-filebrowser-4.0.3/filebrowser/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6466 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11694 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.953539 django-filebrowser-4.0.3/filebrowser/locale/cs/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.022647 django-filebrowser-4.0.3/filebrowser/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6600 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11989 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.953649 django-filebrowser-4.0.3/filebrowser/locale/de/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.023344 django-filebrowser-4.0.3/filebrowser/locale/de/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6694 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11944 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.953759 django-filebrowser-4.0.3/filebrowser/locale/en/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.023991 django-filebrowser-4.0.3/filebrowser/locale/en/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     4353 2019-11-14 14:50:57.000000 django-filebrowser-4.0.3/filebrowser/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    10889 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.953864 django-filebrowser-4.0.3/filebrowser/locale/es/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.024529 django-filebrowser-4.0.3/filebrowser/locale/es/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6472 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11865 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.953975 django-filebrowser-4.0.3/filebrowser/locale/es_CO/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.025094 django-filebrowser-4.0.3/filebrowser/locale/es_CO/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     4042 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/es_CO/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    10840 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/es_CO/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.954083 django-filebrowser-4.0.3/filebrowser/locale/fa/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.032125 django-filebrowser-4.0.3/filebrowser/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     7426 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    12720 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.954191 django-filebrowser-4.0.3/filebrowser/locale/fr/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.033246 django-filebrowser-4.0.3/filebrowser/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6899 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    12181 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.954307 django-filebrowser-4.0.3/filebrowser/locale/hu/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.034049 django-filebrowser-4.0.3/filebrowser/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6771 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    12006 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.954413 django-filebrowser-4.0.3/filebrowser/locale/is/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.034841 django-filebrowser-4.0.3/filebrowser/locale/is/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6304 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/is/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11649 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.954519 django-filebrowser-4.0.3/filebrowser/locale/it/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.035402 django-filebrowser-4.0.3/filebrowser/locale/it/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6461 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11777 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.954620 django-filebrowser-4.0.3/filebrowser/locale/ja/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.036021 django-filebrowser-4.0.3/filebrowser/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     7425 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    12684 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.954722 django-filebrowser-4.0.3/filebrowser/locale/ja_JP/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.036790 django-filebrowser-4.0.3/filebrowser/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     7439 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    12626 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.954833 django-filebrowser-4.0.3/filebrowser/locale/mn/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.037446 django-filebrowser-4.0.3/filebrowser/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     7916 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    13166 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/mn/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.954937 django-filebrowser-4.0.3/filebrowser/locale/nb/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.038027 django-filebrowser-4.0.3/filebrowser/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6480 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11694 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.955040 django-filebrowser-4.0.3/filebrowser/locale/nl/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.038613 django-filebrowser-4.0.3/filebrowser/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)      496 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)     9649 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.955143 django-filebrowser-4.0.3/filebrowser/locale/pl_PL/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.039159 django-filebrowser-4.0.3/filebrowser/locale/pl_PL/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6484 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11887 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/pl_PL/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.955246 django-filebrowser-4.0.3/filebrowser/locale/pt_BR/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.039669 django-filebrowser-4.0.3/filebrowser/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6613 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11917 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.955355 django-filebrowser-4.0.3/filebrowser/locale/ru_RU/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.040228 django-filebrowser-4.0.3/filebrowser/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     8120 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    13540 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/ru_RU/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.955457 django-filebrowser-4.0.3/filebrowser/locale/sk/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.040971 django-filebrowser-4.0.3/filebrowser/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6760 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    12021 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.955562 django-filebrowser-4.0.3/filebrowser/locale/sl_SI/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.041473 django-filebrowser-4.0.3/filebrowser/locale/sl_SI/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6048 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/sl_SI/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11584 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/sl_SI/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.955671 django-filebrowser-4.0.3/filebrowser/locale/sv/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.041911 django-filebrowser-4.0.3/filebrowser/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6400 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11612 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.955779 django-filebrowser-4.0.3/filebrowser/locale/tr_TR/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.042450 django-filebrowser-4.0.3/filebrowser/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6468 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11917 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/tr_TR/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.955885 django-filebrowser-4.0.3/filebrowser/locale/vi/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.043093 django-filebrowser-4.0.3/filebrowser/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6683 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11900 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.955992 django-filebrowser-4.0.3/filebrowser/locale/zh_CN/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.043576 django-filebrowser-4.0.3/filebrowser/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 patrick    (501) staff       (20)     6235 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 patrick    (501) staff       (20)    11503 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.043962 django-filebrowser-4.0.3/filebrowser/management/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/management/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      161 2016-03-07 10:19:11.000000 django-filebrowser-4.0.3/filebrowser/management/__init__.pyc
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.044465 django-filebrowser-4.0.3/filebrowser/management/__pycache__/
+-rw-r--r--   0 patrick    (501) staff       (20)      158 2018-03-21 13:34:13.000000 django-filebrowser-4.0.3/filebrowser/management/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 patrick    (501) staff       (20)      177 2022-01-07 15:34:04.000000 django-filebrowser-4.0.3/filebrowser/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.045176 django-filebrowser-4.0.3/filebrowser/management/commands/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/management/commands/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.047048 django-filebrowser-4.0.3/filebrowser/management/commands/__pycache__/
+-rw-r--r--   0 patrick    (501) staff       (20)      167 2018-03-21 13:34:13.000000 django-filebrowser-4.0.3/filebrowser/management/commands/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 patrick    (501) staff       (20)      186 2022-01-07 15:34:04.000000 django-filebrowser-4.0.3/filebrowser/management/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 patrick    (501) staff       (20)     3833 2020-05-15 09:48:51.000000 django-filebrowser-4.0.3/filebrowser/management/commands/fb_version_generate.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5126 2020-05-15 09:48:51.000000 django-filebrowser-4.0.3/filebrowser/management/commands/fb_version_remove.py
+-rw-r--r--   0 patrick    (501) staff       (20)       51 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/models.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3090 2020-05-15 09:48:51.000000 django-filebrowser-4.0.3/filebrowser/namers.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5605 2023-07-27 12:20:11.000000 django-filebrowser-4.0.3/filebrowser/settings.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1238 2022-01-12 12:55:43.000000 django-filebrowser-4.0.3/filebrowser/signals.py
+-rw-r--r--   0 patrick    (501) staff       (20)    25187 2022-01-12 13:18:33.000000 django-filebrowser-4.0.3/filebrowser/sites.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.956362 django-filebrowser-4.0.3/filebrowser/static/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.956519 django-filebrowser-4.0.3/filebrowser/static/filebrowser/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.047564 django-filebrowser-4.0.3/filebrowser/static/filebrowser/css/
+-rw-r--r--   0 patrick    (501) staff       (20)    11293 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/css/filebrowser.css
+-rw-r--r--   0 patrick    (501) staff       (20)     4949 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/css/uploadfield.css
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.052832 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/
+-rw-r--r--   0 patrick    (501) staff       (20)   870037 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/TEST_IMAGE_000.jpg
+-rw-r--r--   0 patrick    (501) staff       (20)      236 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/cancel.png
+-rw-r--r--   0 patrick    (501) staff       (20)      236 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/cancel_hover.png
+-rw-r--r--   0 patrick    (501) staff       (20)     1122 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/completed.png
+-rw-r--r--   0 patrick    (501) staff       (20)     3027 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/fb-upload-spinner.gif
+-rw-r--r--   0 patrick    (501) staff       (20)     1090 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/fb-upload.png
+-rw-r--r--   0 patrick    (501) staff       (20)     1091 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/fb-upload_hover.png
+-rw-r--r--   0 patrick    (501) staff       (20)      165 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/icon-pulldown-versions-active.png
+-rw-r--r--   0 patrick    (501) staff       (20)      165 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/icon-pulldown-versions-hover.png
+-rw-r--r--   0 patrick    (501) staff       (20)      165 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/icon-pulldown-versions.png
+-rw-r--r--   0 patrick    (501) staff       (20)      367 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/progress-bar-content.png
+-rw-r--r--   0 patrick    (501) staff       (20)   870037 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/testimage.jpg
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.056296 django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/
+-rw-r--r--   0 patrick    (501) staff       (20)     1474 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/AddFileBrowser.js
+-rw-r--r--   0 patrick    (501) staff       (20)      622 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/FB_CKEditor.js
+-rw-r--r--   0 patrick    (501) staff       (20)     1351 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/FB_FileBrowseField.js
+-rw-r--r--   0 patrick    (501) staff       (20)      942 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/FB_TinyMCE.js
+-rw-r--r--   0 patrick    (501) staff       (20)      649 2019-11-11 12:20:07.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/FB_TinyMCEv4.js
+-rw-r--r--   0 patrick    (501) staff       (20)      198 2020-11-25 15:00:38.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/FB_TinyMCEv5.js
+-rw-r--r--   0 patrick    (501) staff       (20)     5651 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/TinyMCEAdmin.js
+-rw-r--r--   0 patrick    (501) staff       (20)     1288 2021-04-22 11:22:43.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/TinyMCEv5Admin.js
+-rw-r--r--   0 patrick    (501) staff       (20)    40022 2023-07-27 13:45:03.000000 django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/fileuploader.js
+-rw-r--r--   0 patrick    (501) staff       (20)     3922 2020-05-15 09:48:51.000000 django-filebrowser-4.0.3/filebrowser/storage.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:19.956627 django-filebrowser-4.0.3/filebrowser/templates/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.058582 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/
+-rw-r--r--   0 patrick    (501) staff       (20)     2522 2020-11-25 15:00:38.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/createdir.html
+-rw-r--r--   0 patrick    (501) staff       (20)     1632 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/custom_field.html
+-rw-r--r--   0 patrick    (501) staff       (20)     5151 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/custom_upload_field.html
+-rw-r--r--   0 patrick    (501) staff       (20)     2222 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/delete_confirm.html
+-rw-r--r--   0 patrick    (501) staff       (20)     8100 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/detail.html
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.059855 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/
+-rw-r--r--   0 patrick    (501) staff       (20)       14 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/_response.html
+-rw-r--r--   0 patrick    (501) staff       (20)     1078 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/breadcrumbs.html
+-rw-r--r--   0 patrick    (501) staff       (20)     7038 2020-11-25 15:00:38.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/filelisting.html
+-rw-r--r--   0 patrick    (501) staff       (20)     2540 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/filter.html
+-rw-r--r--   0 patrick    (501) staff       (20)     1522 2022-01-12 12:55:43.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/paginator.html
+-rw-r--r--   0 patrick    (501) staff       (20)     2837 2022-01-12 12:55:43.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/tableheader.html
+-rw-r--r--   0 patrick    (501) staff       (20)     2078 2019-11-14 14:54:08.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/toolbar.html
+-rw-r--r--   0 patrick    (501) staff       (20)     7529 2022-01-12 12:55:43.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/index.html
+-rw-r--r--   0 patrick    (501) staff       (20)     7326 2022-01-12 13:18:27.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/upload.html
+-rw-r--r--   0 patrick    (501) staff       (20)     2804 2022-01-12 12:55:43.000000 django-filebrowser-4.0.3/filebrowser/templates/filebrowser/version.html
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.061299 django-filebrowser-4.0.3/filebrowser/templatetags/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/templatetags/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1041 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/templatetags/fb_csrf.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1740 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/filebrowser/templatetags/fb_pagination.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4668 2022-01-12 13:18:33.000000 django-filebrowser-4.0.3/filebrowser/templatetags/fb_tags.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4353 2018-09-24 14:10:49.000000 django-filebrowser-4.0.3/filebrowser/templatetags/fb_versions.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3063 2023-07-27 13:45:03.000000 django-filebrowser-4.0.3/filebrowser/utils.py
+-rw-r--r--   0 patrick    (501) staff       (20)       38 2023-07-27 13:46:20.064962 django-filebrowser-4.0.3/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)     1215 2023-07-27 13:45:03.000000 django-filebrowser-4.0.3/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-27 13:46:20.064220 django-filebrowser-4.0.3/tests/
+-rw-r--r--   0 patrick    (501) staff       (20)     2305 2016-03-07 17:20:27.000000 django-filebrowser-4.0.3/tests/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2881 2018-03-21 15:27:11.000000 django-filebrowser-4.0.3/tests/settings.py
+-rw-r--r--   0 patrick    (501) staff       (20)    21436 2020-05-15 09:48:51.000000 django-filebrowser-4.0.3/tests/test_base.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1006 2020-05-15 09:48:51.000000 django-filebrowser-4.0.3/tests/test_commands.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1948 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/tests/test_decorators.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3478 2016-08-09 13:19:40.000000 django-filebrowser-4.0.3/tests/test_namers.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3451 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/tests/test_settings.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13850 2019-11-14 15:49:45.000000 django-filebrowser-4.0.3/tests/test_sites.py
+-rw-r--r--   0 patrick    (501) staff       (20)      798 2016-03-06 14:43:09.000000 django-filebrowser-4.0.3/tests/test_templatetags.py
+-rw-r--r--   0 patrick    (501) staff       (20)    22014 2016-08-09 13:19:40.000000 django-filebrowser-4.0.3/tests/test_versions.py
+-rw-r--r--   0 patrick    (501) staff       (20)      279 2018-03-21 15:27:11.000000 django-filebrowser-4.0.3/tests/urls.py
```

### Comparing `django-filebrowser-4.0.2/LICENSE` & `django-filebrowser-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/PKG-INFO` & `django-filebrowser-4.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: django-filebrowser
-Version: 4.0.2
+Version: 4.0.3
 Summary: Media-Management with Grappelli
 Home-page: http://django-filebrowser.readthedocs.org
 Author: Patrick Kranzlmueller, Axel Swoboda (vonautomatisch)
 Author-email: office@vonautomatisch.at
 License: BSD
 Description: Django FileBrowser
         ==================
-        .. image:: https://api.travis-ci.org/sehmaschine/django-filebrowser.svg
-            :target: https://travis-ci.org/sehmaschine/django-filebrowser
+        .. image:: https://github.com/sehmaschine/django-filebrowser/actions/workflows/tests.yml/badge.svg?branch=master
+            :target: https://github.com/sehmaschine/django-filebrowser/actions/workflows/tests.yml?query=branch%3Amaster
         
         .. image:: https://readthedocs.org/projects/django-filebrowser/badge/?version=latest
             :target: http://django-filebrowser.readthedocs.org/en/latest/?badge=latest
         
         **Media-Management with Grappelli**.
         
         The FileBrowser is an extension to the `Django <http://www.djangoproject.com>`_ administration interface in order to:
@@ -21,15 +21,15 @@
         * browse directories on your server and upload/delete/edit/rename files.
         * include images/documents to your models/database using the ``FileBrowseField``.
         * select images/documents with TinyMCE.
         
         Requirements
         ------------
         
-        FileBrowser 4.0.2 requires
+        FileBrowser 4.0.3 requires
         
         * Django 4.0 (http://www.djangoproject.com)
         * Grappelli 3.0 (https://github.com/sehmaschine/django-grappelli)
         * Pillow (https://github.com/python-imaging/Pillow)
         
         Documentation
         -------------
@@ -40,20 +40,20 @@
         -----------
         
         https://www.transifex.com/projects/p/django-filebrowser/
         
         Releases
         --------
         
-        * FileBrowser 4.0.2 (November 22nd, 2022): Compatible with Django 4.0
+        * FileBrowser 4.0.3 (July 27th, 2023): Compatible with Django 4.0
         * FileBrowser 3.14.3 (January 12th, 2022): Compatible with Django 3.2 (LTS)
         
         Current development branches:
         
-        * FileBrowser 4.0.3 (Development Version for Django 4.0, see Branch Stable/4.0.x)
+        * FileBrowser 4.0.4 (Development Version for Django 4.0, see Branch Stable/4.0.x)
         * FileBrowser 3.14.4 (Development Version for Django 3.2, see Branch Stable/3.14.x)
         
         Older versions are available at GitHub, but are not supported anymore.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-filebrowser-4.0.2/README.rst` & `django-filebrowser-4.0.3/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Django FileBrowser
 ==================
-.. image:: https://api.travis-ci.org/sehmaschine/django-filebrowser.svg
-    :target: https://travis-ci.org/sehmaschine/django-filebrowser
+.. image:: https://github.com/sehmaschine/django-filebrowser/actions/workflows/tests.yml/badge.svg?branch=master
+    :target: https://github.com/sehmaschine/django-filebrowser/actions/workflows/tests.yml?query=branch%3Amaster
 
 .. image:: https://readthedocs.org/projects/django-filebrowser/badge/?version=latest
     :target: http://django-filebrowser.readthedocs.org/en/latest/?badge=latest
 
 **Media-Management with Grappelli**.
 
 The FileBrowser is an extension to the `Django <http://www.djangoproject.com>`_ administration interface in order to:
@@ -13,15 +13,15 @@
 * browse directories on your server and upload/delete/edit/rename files.
 * include images/documents to your models/database using the ``FileBrowseField``.
 * select images/documents with TinyMCE.
 
 Requirements
 ------------
 
-FileBrowser 4.0.2 requires
+FileBrowser 4.0.3 requires
 
 * Django 4.0 (http://www.djangoproject.com)
 * Grappelli 3.0 (https://github.com/sehmaschine/django-grappelli)
 * Pillow (https://github.com/python-imaging/Pillow)
 
 Documentation
 -------------
@@ -32,16 +32,16 @@
 -----------
 
 https://www.transifex.com/projects/p/django-filebrowser/
 
 Releases
 --------
 
-* FileBrowser 4.0.2 (November 22nd, 2022): Compatible with Django 4.0
+* FileBrowser 4.0.3 (July 27th, 2023): Compatible with Django 4.0
 * FileBrowser 3.14.3 (January 12th, 2022): Compatible with Django 3.2 (LTS)
 
 Current development branches:
 
-* FileBrowser 4.0.3 (Development Version for Django 4.0, see Branch Stable/4.0.x)
+* FileBrowser 4.0.4 (Development Version for Django 4.0, see Branch Stable/4.0.x)
 * FileBrowser 3.14.4 (Development Version for Django 3.2, see Branch Stable/3.14.x)
 
 Older versions are available at GitHub, but are not supported anymore.
```

### Comparing `django-filebrowser-4.0.2/django_filebrowser.egg-info/PKG-INFO` & `django-filebrowser-4.0.3/django_filebrowser.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: django-filebrowser
-Version: 4.0.2
+Version: 4.0.3
 Summary: Media-Management with Grappelli
 Home-page: http://django-filebrowser.readthedocs.org
 Author: Patrick Kranzlmueller, Axel Swoboda (vonautomatisch)
 Author-email: office@vonautomatisch.at
 License: BSD
 Description: Django FileBrowser
         ==================
-        .. image:: https://api.travis-ci.org/sehmaschine/django-filebrowser.svg
-            :target: https://travis-ci.org/sehmaschine/django-filebrowser
+        .. image:: https://github.com/sehmaschine/django-filebrowser/actions/workflows/tests.yml/badge.svg?branch=master
+            :target: https://github.com/sehmaschine/django-filebrowser/actions/workflows/tests.yml?query=branch%3Amaster
         
         .. image:: https://readthedocs.org/projects/django-filebrowser/badge/?version=latest
             :target: http://django-filebrowser.readthedocs.org/en/latest/?badge=latest
         
         **Media-Management with Grappelli**.
         
         The FileBrowser is an extension to the `Django <http://www.djangoproject.com>`_ administration interface in order to:
@@ -21,15 +21,15 @@
         * browse directories on your server and upload/delete/edit/rename files.
         * include images/documents to your models/database using the ``FileBrowseField``.
         * select images/documents with TinyMCE.
         
         Requirements
         ------------
         
-        FileBrowser 4.0.2 requires
+        FileBrowser 4.0.3 requires
         
         * Django 4.0 (http://www.djangoproject.com)
         * Grappelli 3.0 (https://github.com/sehmaschine/django-grappelli)
         * Pillow (https://github.com/python-imaging/Pillow)
         
         Documentation
         -------------
@@ -40,20 +40,20 @@
         -----------
         
         https://www.transifex.com/projects/p/django-filebrowser/
         
         Releases
         --------
         
-        * FileBrowser 4.0.2 (November 22nd, 2022): Compatible with Django 4.0
+        * FileBrowser 4.0.3 (July 27th, 2023): Compatible with Django 4.0
         * FileBrowser 3.14.3 (January 12th, 2022): Compatible with Django 3.2 (LTS)
         
         Current development branches:
         
-        * FileBrowser 4.0.3 (Development Version for Django 4.0, see Branch Stable/4.0.x)
+        * FileBrowser 4.0.4 (Development Version for Django 4.0, see Branch Stable/4.0.x)
         * FileBrowser 3.14.4 (Development Version for Django 3.2, see Branch Stable/3.14.x)
         
         Older versions are available at GitHub, but are not supported anymore.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-filebrowser-4.0.2/django_filebrowser.egg-info/SOURCES.txt` & `django-filebrowser-4.0.3/django_filebrowser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/Makefile` & `django-filebrowser-4.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/admin.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/admin.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/api.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/changelog.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/environment.pickle` & `django-filebrowser-4.0.3/docs/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/faq.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/faq.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/fieldswidgets.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/fieldswidgets.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/filelisting.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/filelisting.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/fileobject.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/fileobject.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/help.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/help.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/index.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/quickstart.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/quickstart.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/releasenotes.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/releasenotes.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/settings.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/settings.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/testing.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/testing.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/translation.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/translation.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/troubleshooting.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/troubleshooting.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/.doctrees/versions.doctree` & `django-filebrowser-4.0.3/docs/_build/.doctrees/versions.doctree`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/admin.rst.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/admin.rst.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/admin.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/admin.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/changelog.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/changelog.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/faq.rst.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/faq.rst.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/faq.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/faq.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/fieldswidgets.rst.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/fieldswidgets.rst.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/fieldswidgets.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/fieldswidgets.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/filelisting.rst.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/filelisting.rst.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/filelisting.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/filelisting.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/fileobject.rst.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/fileobject.rst.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/fileobject.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/fileobject.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/index.rst.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/index.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/index.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/quickstart.rst.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/quickstart.rst.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/quickstart.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/quickstart.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/releasenotes.rst.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/releasenotes.rst.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/releasenotes.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/releasenotes.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/settings.rst.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/settings.rst.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/settings.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/settings.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/troubleshooting.rst.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/troubleshooting.rst.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/troubleshooting.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/troubleshooting.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/versions.rst.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/versions.rst.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_sources/versions.txt` & `django-filebrowser-4.0.3/docs/_build/_sources/versions.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/ajax-loader.gif` & `django-filebrowser-4.0.3/docs/_build/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/basic.css` & `django-filebrowser-4.0.3/docs/_build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/comment-bright.png` & `django-filebrowser-4.0.3/docs/_build/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/comment-close.png` & `django-filebrowser-4.0.3/docs/_build/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/comment.png` & `django-filebrowser-4.0.3/docs/_build/_static/comment.png`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/css/badge_only.css` & `django-filebrowser-4.0.3/docs/_build/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/css/theme.css` & `django-filebrowser-4.0.3/docs/_build/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/doctools.js` & `django-filebrowser-4.0.3/docs/_build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Inconsolata-Bold.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Inconsolata-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Inconsolata-Regular.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Inconsolata-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Inconsolata.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Inconsolata.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bold.eot` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bold.eot`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bold.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bold.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bold.woff` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bold.woff2` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bolditalic.eot` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bolditalic.eot`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bolditalic.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bolditalic.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bolditalic.woff` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bolditalic.woff`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-bolditalic.woff2` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-bolditalic.woff2`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-italic.eot` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-italic.eot`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-italic.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-italic.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-italic.woff` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-italic.woff`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-italic.woff2` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-italic.woff2`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-regular.eot` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-regular.eot`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-regular.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-regular.woff` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-regular.woff`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato/lato-regular.woff2` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato/lato-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato-Bold.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/Lato-Regular.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab-Bold.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/RobotoSlab-Regular.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/RobotoSlab-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/fontawesome-webfont.eot` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/fontawesome-webfont.svg` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/fontawesome-webfont.ttf` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/fontawesome-webfont.woff` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/fonts/fontawesome-webfont.woff2` & `django-filebrowser-4.0.3/docs/_build/_static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/jquery-1.11.1.js` & `django-filebrowser-4.0.3/docs/_build/_static/jquery-1.11.1.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/jquery-3.2.1.js` & `django-filebrowser-4.0.3/docs/_build/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/jquery-3.4.1.js` & `django-filebrowser-4.0.3/docs/_build/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/jquery.js` & `django-filebrowser-4.0.3/docs/_build/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/js/modernizr.min.js` & `django-filebrowser-4.0.3/docs/_build/_static/js/modernizr.min.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/js/theme.js` & `django-filebrowser-4.0.3/docs/_build/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/language_data.js` & `django-filebrowser-4.0.3/docs/_build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/pygments.css` & `django-filebrowser-4.0.3/docs/_build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/searchtools.js` & `django-filebrowser-4.0.3/docs/_build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/underscore-1.3.1.js` & `django-filebrowser-4.0.3/docs/_build/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/underscore.js` & `django-filebrowser-4.0.3/docs/_build/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/_static/websupport.js` & `django-filebrowser-4.0.3/docs/_build/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/admin.html` & `django-filebrowser-4.0.3/docs/_build/admin.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/api.html` & `django-filebrowser-4.0.3/docs/_build/api.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/changelog.html` & `django-filebrowser-4.0.3/docs/_build/changelog.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/faq.html` & `django-filebrowser-4.0.3/docs/_build/faq.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/fieldswidgets.html` & `django-filebrowser-4.0.3/docs/_build/fieldswidgets.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/filelisting.html` & `django-filebrowser-4.0.3/docs/_build/filelisting.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/fileobject.html` & `django-filebrowser-4.0.3/docs/_build/fileobject.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/genindex.html` & `django-filebrowser-4.0.3/docs/_build/genindex.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/help.html` & `django-filebrowser-4.0.3/docs/_build/help.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/index.html` & `django-filebrowser-4.0.3/docs/_build/index.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/objects.inv` & `django-filebrowser-4.0.3/docs/_build/objects.inv`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/quickstart.html` & `django-filebrowser-4.0.3/docs/_build/quickstart.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/releasenotes.html` & `django-filebrowser-4.0.3/docs/_build/releasenotes.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/search.html` & `django-filebrowser-4.0.3/docs/_build/search.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/searchindex.js` & `django-filebrowser-4.0.3/docs/_build/searchindex.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/settings.html` & `django-filebrowser-4.0.3/docs/_build/settings.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/testing.html` & `django-filebrowser-4.0.3/docs/_build/testing.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/translation.html` & `django-filebrowser-4.0.3/docs/_build/translation.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/troubleshooting.html` & `django-filebrowser-4.0.3/docs/_build/troubleshooting.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/_build/versions.html` & `django-filebrowser-4.0.3/docs/_build/versions.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/admin.rst` & `django-filebrowser-4.0.3/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/conf.py` & `django-filebrowser-4.0.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,17 +47,17 @@
 copyright = u'2022, Patrick Kranzlmueller'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '4.0.2'
+version = '4.0.3'
 # The full version, including alpha/beta/rc tags.
-release = '4.0.2'
+release = '4.0.3'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `django-filebrowser-4.0.2/docs/faq.rst` & `django-filebrowser-4.0.3/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/fieldswidgets.rst` & `django-filebrowser-4.0.3/docs/fieldswidgets.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/filelisting.rst` & `django-filebrowser-4.0.3/docs/filelisting.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/fileobject.rst` & `django-filebrowser-4.0.3/docs/fileobject.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/index.rst` & `django-filebrowser-4.0.3/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -86,18 +86,18 @@
 ----------
 
 Use the `FileBrowser Google Group <http://groups.google.com/group/django-filebrowser>`_ to ask questions or discuss features.
 
 Versions and Compatibility
 --------------------------
 
-**FileBrowser is always developed against the latest stable Django release and is NOT tested with Djangos trunk.**
+**FileBrowser is always developed against the latest stable Django release.**
 
-* FileBrowser 4.0.2 (November 22nd, 2022): Compatible with Django 4.0
+* FileBrowser 4.0.3 (July 27th, 2023): Compatible with Django 4.0
 * FileBrowser 3.14.3 (January 12th, 2022): Compatible with Django 3.2 (LTS)
 
 Current development branches:
 
-* FileBrowser 4.0.3 (Development Version for Django 4.0, see Branch Stable/4.0.x)
+* FileBrowser 4.0.4 (Development Version for Django 4.0, see Branch Stable/4.0.x)
 * FileBrowser 3.14.4 (Development Version for Django 3.2, see Branch Stable/3.14.x)
 
 Older versions are available at GitHub, but are not supported anymore.
```

### Comparing `django-filebrowser-4.0.2/docs/quickstart.rst` & `django-filebrowser-4.0.3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/releasenotes.rst` & `django-filebrowser-4.0.3/docs/releasenotes.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/settings.rst` & `django-filebrowser-4.0.3/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/troubleshooting.rst` & `django-filebrowser-4.0.3/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/docs/versions.rst` & `django-filebrowser-4.0.3/docs/versions.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/actions.py` & `django-filebrowser-4.0.3/filebrowser/actions.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/base.py` & `django-filebrowser-4.0.3/filebrowser/base.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/decorators.py` & `django-filebrowser-4.0.3/filebrowser/decorators.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/fields.py` & `django-filebrowser-4.0.3/filebrowser/fields.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/forms.py` & `django-filebrowser-4.0.3/filebrowser/forms.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/az/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/az/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/az/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/az/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/bg_BG/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/bg_BG/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/bg_BG/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/bg_BG/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/ca/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/ca/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/cs/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/cs/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/de/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/de/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/en/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/en/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/es/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/es/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/es_CO/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/es_CO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/es_CO/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/es_CO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/fa/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/fa/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/fr/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/fr/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/hu/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/hu/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/is/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/is/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/is/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/it/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/it/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/ja/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/ja/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/ja_JP/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/ja_JP/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/ja_JP/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/mn/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/mn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/mn/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/mn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/nb/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/nb/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/nl/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/pl_PL/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/pl_PL/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/pt_BR/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/pt_BR/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/ru_RU/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/ru_RU/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/sk/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/sk/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/sl_SI/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/sl_SI/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/sl_SI/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/sl_SI/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/sv/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/sv/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/tr_TR/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/tr_TR/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/vi/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/vi/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/zh_CN/LC_MESSAGES/django.mo` & `django-filebrowser-4.0.3/filebrowser/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/locale/zh_CN/LC_MESSAGES/django.po` & `django-filebrowser-4.0.3/filebrowser/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/management/commands/fb_version_generate.py` & `django-filebrowser-4.0.3/filebrowser/management/commands/fb_version_generate.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/management/commands/fb_version_remove.py` & `django-filebrowser-4.0.3/filebrowser/management/commands/fb_version_remove.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/namers.py` & `django-filebrowser-4.0.3/filebrowser/namers.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/settings.py` & `django-filebrowser-4.0.3/filebrowser/settings.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/signals.py` & `django-filebrowser-4.0.3/filebrowser/signals.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/sites.py` & `django-filebrowser-4.0.3/filebrowser/sites.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/css/filebrowser.css` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/css/filebrowser.css`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/css/uploadfield.css` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/css/uploadfield.css`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/TEST_IMAGE_000.jpg` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/TEST_IMAGE_000.jpg`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/completed.png` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/completed.png`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/fb-upload-spinner.gif` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/fb-upload-spinner.gif`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/fb-upload.png` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/fb-upload.png`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/fb-upload_hover.png` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/fb-upload_hover.png`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/img/testimage.jpg` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/img/testimage.jpg`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/AddFileBrowser.js` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/AddFileBrowser.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/FB_CKEditor.js` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/FB_CKEditor.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/FB_FileBrowseField.js` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/FB_FileBrowseField.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/FB_TinyMCE.js` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/FB_TinyMCE.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/FB_TinyMCEv4.js` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/FB_TinyMCEv4.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/TinyMCEAdmin.js` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/TinyMCEAdmin.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/TinyMCEv5Admin.js` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/TinyMCEv5Admin.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/static/filebrowser/js/fileuploader.js` & `django-filebrowser-4.0.3/filebrowser/static/filebrowser/js/fileuploader.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -450,23 +450,23 @@
     _formatFileName: function(name) {
         if (name.length > 33) {
             name = name.slice(0, 19) + '...' + name.slice(-13);
         }
         return name;
     },
     _isAllowedExtension: function(fileName) {
-        var ext = (-1 !== fileName.indexOf('.')) ? fileName.substr(fileName.lastIndexOf('.')).toLowerCase() : '';
+        var fileNameLower = fileName.toLowerCase();
         var allowed = this._options.allowedExtensions;
 
         if (!allowed.length) {
             return true;
         }
 
         for (var i = 0; i < allowed.length; i++) {
-            if (allowed[i].toLowerCase() == ext) {
+            if (fileNameLower.endsWith(allowed[i].toLowerCase())) {
                 return true;
             }
         }
 
         return false;
     },
     _formatSize: function(bytes) {
```

### Comparing `django-filebrowser-4.0.2/filebrowser/storage.py` & `django-filebrowser-4.0.3/filebrowser/storage.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/createdir.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/createdir.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/custom_field.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/custom_field.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/custom_upload_field.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/custom_upload_field.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/delete_confirm.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/delete_confirm.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/detail.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/detail.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/breadcrumbs.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/filelisting.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/filelisting.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/filter.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/filter.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/paginator.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/paginator.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/tableheader.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/tableheader.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/include/toolbar.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/include/toolbar.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/index.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/index.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/upload.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/upload.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templates/filebrowser/version.html` & `django-filebrowser-4.0.3/filebrowser/templates/filebrowser/version.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templatetags/fb_csrf.py` & `django-filebrowser-4.0.3/filebrowser/templatetags/fb_csrf.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templatetags/fb_pagination.py` & `django-filebrowser-4.0.3/filebrowser/templatetags/fb_pagination.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templatetags/fb_tags.py` & `django-filebrowser-4.0.3/filebrowser/templatetags/fb_tags.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/templatetags/fb_versions.py` & `django-filebrowser-4.0.3/filebrowser/templatetags/fb_versions.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/filebrowser/utils.py` & `django-filebrowser-4.0.3/filebrowser/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
     if 'crop' in opts:
         r = max(xr / x, yr / y)
     else:
         r = min(xr / x, yr / y)
 
     if r < 1.0 or (r > 1.0 and 'upscale' in opts):
-        im = im.resize((int(math.ceil(x * r)), int(math.ceil(y * r))), resample=Image.ANTIALIAS)
+        im = im.resize((int(math.ceil(x * r)), int(math.ceil(y * r))), resample=Image.Resampling.LANCZOS)
 
     if 'crop' in opts:
         x, y = [float(v) for v in im.size]
         ex, ey = (x - min(x, xr)) / 2, (y - min(y, yr)) / 2
         if ex or ey:
             im = im.crop((int(ex), int(ey), int(ex + xr), int(ey + yr)))
     return im
```

### Comparing `django-filebrowser-4.0.2/setup.py` & `django-filebrowser-4.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='django-filebrowser',
-    version='4.0.2',
+    version='4.0.3',
     description='Media-Management with Grappelli',
     long_description=read('README.rst'),
     url='http://django-filebrowser.readthedocs.org',
     download_url='',
     author='Patrick Kranzlmueller, Axel Swoboda (vonautomatisch)',
     author_email='office@vonautomatisch.at',
     license='BSD',
```

### Comparing `django-filebrowser-4.0.2/tests/__init__.py` & `django-filebrowser-4.0.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/tests/settings.py` & `django-filebrowser-4.0.3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/tests/test_base.py` & `django-filebrowser-4.0.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/tests/test_commands.py` & `django-filebrowser-4.0.3/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/tests/test_decorators.py` & `django-filebrowser-4.0.3/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/tests/test_namers.py` & `django-filebrowser-4.0.3/tests/test_namers.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/tests/test_settings.py` & `django-filebrowser-4.0.3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/tests/test_sites.py` & `django-filebrowser-4.0.3/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/tests/test_templatetags.py` & `django-filebrowser-4.0.3/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-4.0.2/tests/test_versions.py` & `django-filebrowser-4.0.3/tests/test_versions.py`

 * *Files identical despite different names*

