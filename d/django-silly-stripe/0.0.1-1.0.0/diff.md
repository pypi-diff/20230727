# Comparing `tmp/django-silly-stripe-0.0.1.tar.gz` & `tmp/django-silly-stripe-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-stripe-0.0.1.tar", last modified: Wed Jul 12 15:47:59 2023, max compression
+gzip compressed data, was "django-silly-stripe-1.0.0.tar", last modified: Thu Jul 27 16:32:16 2023, max compression
```

## Comparing `django-silly-stripe-0.0.1.tar` & `django-silly-stripe-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-12 15:47:59.062058 django-silly-stripe-0.0.1/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-stripe-0.0.1/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1091 2023-07-12 15:47:59.062058 django-silly-stripe-0.0.1/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      468 2023-07-12 13:44:46.000000 django-silly-stripe-0.0.1/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-12 15:47:59.058058 django-silly-stripe-0.0.1/django_silly_stripe/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       22 2023-07-12 12:00:42.000000 django-silly-stripe-0.0.1/django_silly_stripe/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      230 2023-07-12 13:56:19.000000 django-silly-stripe-0.0.1/django_silly_stripe/admin.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      877 2023-07-12 14:48:03.000000 django-silly-stripe-0.0.1/django_silly_stripe/conf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      221 2023-07-12 13:32:57.000000 django-silly-stripe-0.0.1/django_silly_stripe/helpers.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-12 12:25:30.000000 django-silly-stripe-0.0.1/django_silly_stripe/mixins.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      673 2023-07-12 13:58:07.000000 django-silly-stripe-0.0.1/django_silly_stripe/models.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-07-12 13:41:39.000000 django-silly-stripe-0.0.1/django_silly_stripe/urls.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-12 15:47:59.062058 django-silly-stripe-0.0.1/django_silly_stripe.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1091 2023-07-12 15:47:59.000000 django-silly-stripe-0.0.1/django_silly_stripe.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      451 2023-07-12 15:47:59.000000 django-silly-stripe-0.0.1/django_silly_stripe.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-07-12 15:47:59.000000 django-silly-stripe-0.0.1/django_silly_stripe.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       14 2023-07-12 15:47:59.000000 django-silly-stripe-0.0.1/django_silly_stripe.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       20 2023-07-12 15:47:59.000000 django-silly-stripe-0.0.1/django_silly_stripe.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-07-12 15:47:59.062058 django-silly-stripe-0.0.1/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1642 2023-07-12 12:08:15.000000 django-silly-stripe-0.0.1/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-27 16:32:16.561769 django-silly-stripe-1.0.0/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-stripe-1.0.0/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3241 2023-07-27 16:32:16.561769 django-silly-stripe-1.0.0/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2618 2023-07-27 13:44:35.000000 django-silly-stripe-1.0.0/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-27 16:32:16.557769 django-silly-stripe-1.0.0/django_silly_stripe/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       52 2023-07-27 16:30:23.000000 django-silly-stripe-1.0.0/django_silly_stripe/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1973 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.0/django_silly_stripe/admin.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1048 2023-07-27 14:11:12.000000 django-silly-stripe-1.0.0/django_silly_stripe/conf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      822 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.0/django_silly_stripe/helpers.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3428 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.0/django_silly_stripe/models.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2203 2023-07-27 13:47:01.000000 django-silly-stripe-1.0.0/django_silly_stripe/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     9395 2023-07-27 16:31:45.000000 django-silly-stripe-1.0.0/django_silly_stripe/views.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-27 16:32:16.561769 django-silly-stripe-1.0.0/django_silly_stripe.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3241 2023-07-27 16:32:16.000000 django-silly-stripe-1.0.0/django_silly_stripe.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      450 2023-07-27 16:32:16.000000 django-silly-stripe-1.0.0/django_silly_stripe.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-07-27 16:32:16.000000 django-silly-stripe-1.0.0/django_silly_stripe.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       14 2023-07-27 16:32:16.000000 django-silly-stripe-1.0.0/django_silly_stripe.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       20 2023-07-27 16:32:16.000000 django-silly-stripe-1.0.0/django_silly_stripe.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-07-27 16:32:16.561769 django-silly-stripe-1.0.0/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1642 2023-07-12 12:08:15.000000 django-silly-stripe-1.0.0/setup.py
```

### Comparing `django-silly-stripe-0.0.1/LICENSE.md` & `django-silly-stripe-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-0.0.1/setup.py` & `django-silly-stripe-1.0.0/setup.py`

 * *Files identical despite different names*

