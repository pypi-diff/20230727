# Comparing `tmp/django-easy-notify-1.0.tar.gz` & `tmp/django-easy-notify-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-easy-notify-1.0.tar", last modified: Fri Jul 14 09:52:42 2023, max compression
+gzip compressed data, was "django-easy-notify-1.1.tar", last modified: Thu Jul 27 12:27:07 2023, max compression
```

## Comparing `django-easy-notify-1.0.tar` & `django-easy-notify-1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-14 09:52:42.944194 django-easy-notify-1.0/
--rw-rw-r--   0 manish    (1000) manish    (1000)     1093 2023-07-14 09:49:45.000000 django-easy-notify-1.0/LICENSE
--rw-rw-r--   0 manish    (1000) manish    (1000)     5271 2023-07-14 09:52:42.944194 django-easy-notify-1.0/PKG-INFO
--rw-rw-r--   0 manish    (1000) manish    (1000)     4365 2023-07-14 09:49:49.000000 django-easy-notify-1.0/README.md
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-14 09:52:42.944194 django-easy-notify-1.0/django_easy_notify.egg-info/
--rw-rw-r--   0 manish    (1000) manish    (1000)     5271 2023-07-14 09:52:42.000000 django-easy-notify-1.0/django_easy_notify.egg-info/PKG-INFO
--rw-rw-r--   0 manish    (1000) manish    (1000)      787 2023-07-14 09:52:42.000000 django-easy-notify-1.0/django_easy_notify.egg-info/SOURCES.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)        1 2023-07-14 09:52:42.000000 django-easy-notify-1.0/django_easy_notify.egg-info/dependency_links.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)       38 2023-07-14 09:52:42.000000 django-easy-notify-1.0/django_easy_notify.egg-info/requires.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)       35 2023-07-14 09:52:42.000000 django-easy-notify-1.0/django_easy_notify.egg-info/top_level.txt
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-14 09:52:42.944194 django-easy-notify-1.0/django_notifications/
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-07-14 09:49:45.000000 django-easy-notify-1.0/django_notifications/__init__.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      487 2023-07-14 09:49:45.000000 django-easy-notify-1.0/django_notifications/asgi.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     3798 2023-07-14 09:49:45.000000 django-easy-notify-1.0/django_notifications/settings.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      465 2023-07-14 09:49:45.000000 django-easy-notify-1.0/django_notifications/test_settings.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      970 2023-07-14 09:49:45.000000 django-easy-notify-1.0/django_notifications/urls.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      417 2023-07-14 09:49:45.000000 django-easy-notify-1.0/django_notifications/wsgi.py
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-14 09:52:42.944194 django-easy-notify-1.0/notifications/
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-07-14 09:49:45.000000 django-easy-notify-1.0/notifications/__init__.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      184 2023-07-14 09:49:45.000000 django-easy-notify-1.0/notifications/admin.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      158 2023-07-14 09:49:45.000000 django-easy-notify-1.0/notifications/apps.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     2237 2023-07-14 09:49:45.000000 django-easy-notify-1.0/notifications/consumers.py
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-14 09:52:42.944194 django-easy-notify-1.0/notifications/migrations/
--rw-rw-r--   0 manish    (1000) manish    (1000)     4481 2023-07-14 09:49:45.000000 django-easy-notify-1.0/notifications/migrations/0001_initial.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      620 2023-07-14 09:49:45.000000 django-easy-notify-1.0/notifications/migrations/0002_alter_notification_state.py
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-07-14 09:49:45.000000 django-easy-notify-1.0/notifications/migrations/__init__.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     2012 2023-07-14 09:49:45.000000 django-easy-notify-1.0/notifications/models.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      195 2023-07-14 09:49:45.000000 django-easy-notify-1.0/notifications/routing.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      109 2023-07-14 09:49:45.000000 django-easy-notify-1.0/notifications/urls.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     4225 2023-07-14 09:49:45.000000 django-easy-notify-1.0/notifications/utils.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      124 2023-07-14 09:49:45.000000 django-easy-notify-1.0/notifications/views.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     1298 2023-07-14 09:52:42.948254 django-easy-notify-1.0/setup.cfg
--rw-rw-r--   0 manish    (1000) manish    (1000)       38 2023-07-14 09:49:45.000000 django-easy-notify-1.0/setup.py
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-27 12:27:07.095489 django-easy-notify-1.1/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     1093 2023-07-14 09:49:45.000000 django-easy-notify-1.1/LICENSE
+-rw-rw-r--   0 manish    (1000) manish    (1000)     5276 2023-07-27 12:27:07.095489 django-easy-notify-1.1/PKG-INFO
+-rw-rw-r--   0 manish    (1000) manish    (1000)     4365 2023-07-14 09:49:49.000000 django-easy-notify-1.1/README.md
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-27 12:27:07.095489 django-easy-notify-1.1/django_easy_notify.egg-info/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     5276 2023-07-27 12:27:07.000000 django-easy-notify-1.1/django_easy_notify.egg-info/PKG-INFO
+-rw-rw-r--   0 manish    (1000) manish    (1000)      787 2023-07-27 12:27:07.000000 django-easy-notify-1.1/django_easy_notify.egg-info/SOURCES.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)        1 2023-07-27 12:27:07.000000 django-easy-notify-1.1/django_easy_notify.egg-info/dependency_links.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)       38 2023-07-27 12:27:07.000000 django-easy-notify-1.1/django_easy_notify.egg-info/requires.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)       35 2023-07-27 12:27:07.000000 django-easy-notify-1.1/django_easy_notify.egg-info/top_level.txt
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-27 12:27:07.095489 django-easy-notify-1.1/django_notifications/
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-07-14 09:49:45.000000 django-easy-notify-1.1/django_notifications/__init__.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      487 2023-07-14 09:49:45.000000 django-easy-notify-1.1/django_notifications/asgi.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     3798 2023-07-14 09:49:45.000000 django-easy-notify-1.1/django_notifications/settings.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      465 2023-07-14 09:49:45.000000 django-easy-notify-1.1/django_notifications/test_settings.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      970 2023-07-14 09:49:45.000000 django-easy-notify-1.1/django_notifications/urls.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      417 2023-07-14 09:49:45.000000 django-easy-notify-1.1/django_notifications/wsgi.py
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-27 12:27:07.095489 django-easy-notify-1.1/notifications/
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-07-14 09:49:45.000000 django-easy-notify-1.1/notifications/__init__.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      184 2023-07-14 09:49:45.000000 django-easy-notify-1.1/notifications/admin.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      158 2023-07-14 09:49:45.000000 django-easy-notify-1.1/notifications/apps.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2237 2023-07-14 09:49:45.000000 django-easy-notify-1.1/notifications/consumers.py
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-27 12:27:07.095489 django-easy-notify-1.1/notifications/migrations/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     4481 2023-07-14 09:49:45.000000 django-easy-notify-1.1/notifications/migrations/0001_initial.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      620 2023-07-14 09:49:45.000000 django-easy-notify-1.1/notifications/migrations/0002_alter_notification_state.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-07-14 09:49:45.000000 django-easy-notify-1.1/notifications/migrations/__init__.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2012 2023-07-14 09:49:45.000000 django-easy-notify-1.1/notifications/models.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      195 2023-07-14 09:49:45.000000 django-easy-notify-1.1/notifications/routing.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      109 2023-07-14 09:49:45.000000 django-easy-notify-1.1/notifications/urls.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     4229 2023-07-27 12:26:21.000000 django-easy-notify-1.1/notifications/utils.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      124 2023-07-14 09:49:45.000000 django-easy-notify-1.1/notifications/views.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     1303 2023-07-27 12:27:07.095489 django-easy-notify-1.1/setup.cfg
+-rw-rw-r--   0 manish    (1000) manish    (1000)       38 2023-07-14 09:49:45.000000 django-easy-notify-1.1/setup.py
```

### Comparing `django-easy-notify-1.0/LICENSE` & `django-easy-notify-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-easy-notify-1.0/PKG-INFO` & `django-easy-notify-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-easy-notify
-Version: 1.0
+Version: 1.1
 Summary: A Django Library to send notifications in easy way
-Home-page: https://github.com/Hashtrust-technology-private-limited/notifications
+Home-page: https://github.com/Hashtrust-technology-private-limited/django-easy-notify
 Author: Hashtrust Technologies Private Limited
 Author-email: support@hashtrust.in
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: django-easy-notify Version: 1.0 Summary: A Django
+Metadata-Version: 2.1 Name: django-easy-notify Version: 1.1 Summary: A Django
 Library to send notifications in easy way Home-page: https://github.com/
-Hashtrust-technology-private-limited/notifications Author: Hashtrust
+Hashtrust-technology-private-limited/django-easy-notify Author: Hashtrust
 Technologies Private Limited Author-email: support@hashtrust.in License: MIT
 License Classifier: Environment :: Web Environment Classifier: Framework ::
 Django :: 4.1 Classifier: Intended Audience :: Developers Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `django-easy-notify-1.0/README.md` & `django-easy-notify-1.1/README.md`

 * *Files identical despite different names*

### Comparing `django-easy-notify-1.0/django_easy_notify.egg-info/PKG-INFO` & `django-easy-notify-1.1/django_easy_notify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-easy-notify
-Version: 1.0
+Version: 1.1
 Summary: A Django Library to send notifications in easy way
-Home-page: https://github.com/Hashtrust-technology-private-limited/notifications
+Home-page: https://github.com/Hashtrust-technology-private-limited/django-easy-notify
 Author: Hashtrust Technologies Private Limited
 Author-email: support@hashtrust.in
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: django-easy-notify Version: 1.0 Summary: A Django
+Metadata-Version: 2.1 Name: django-easy-notify Version: 1.1 Summary: A Django
 Library to send notifications in easy way Home-page: https://github.com/
-Hashtrust-technology-private-limited/notifications Author: Hashtrust
+Hashtrust-technology-private-limited/django-easy-notify Author: Hashtrust
 Technologies Private Limited Author-email: support@hashtrust.in License: MIT
 License Classifier: Environment :: Web Environment Classifier: Framework ::
 Django :: 4.1 Classifier: Intended Audience :: Developers Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `django-easy-notify-1.0/django_easy_notify.egg-info/SOURCES.txt` & `django-easy-notify-1.1/django_easy_notify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-easy-notify-1.0/django_notifications/settings.py` & `django-easy-notify-1.1/django_notifications/settings.py`

 * *Files identical despite different names*

### Comparing `django-easy-notify-1.0/django_notifications/urls.py` & `django-easy-notify-1.1/django_notifications/urls.py`

 * *Files identical despite different names*

### Comparing `django-easy-notify-1.0/notifications/consumers.py` & `django-easy-notify-1.1/notifications/consumers.py`

 * *Files identical despite different names*

### Comparing `django-easy-notify-1.0/notifications/migrations/0001_initial.py` & `django-easy-notify-1.1/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-easy-notify-1.0/notifications/migrations/0002_alter_notification_state.py` & `django-easy-notify-1.1/notifications/migrations/0002_alter_notification_state.py`

 * *Files identical despite different names*

### Comparing `django-easy-notify-1.0/notifications/models.py` & `django-easy-notify-1.1/notifications/models.py`

 * *Files identical despite different names*

### Comparing `django-easy-notify-1.0/notifications/utils.py` & `django-easy-notify-1.1/notifications/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 def get_notifications(user, notification_type=None):
     if not notification_type:
         return (
             Notification.objects.prefetch_related("receivers")
             .filter(receivers=user)
             .annotate(
-                sender_name=F("sender__username"), category_type=F("category__title")
+                sender_name=F("sender__first_name"), category_type=F("category__title")
             )
             .values(
                 "title", "message", "notification_type", "sender_name", "category_type"
             )
         )
 
     if notification_type not in list(
@@ -95,15 +95,15 @@
     ):
         return f"Please provide valid notification type. It should be any of {list(dict(Notification.NotificationType.choices).keys())}."
     else:
         return (
             Notification.objects.prefetch_related("receivers")
             .filter(receivers=user, notification_type=notification_type)
             .annotate(
-                sender_name=F("sender__username"), category_type=F("category__title")
+                sender_name=F("sender__first_name"), category_type=F("category__title")
             )
             .values(
                 "title", "message", "notification_type", "sender_name", "category_type"
             )
         )
```

### Comparing `django-easy-notify-1.0/setup.cfg` & `django-easy-notify-1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = django-easy-notify
-version = 1.0
+version = 1.1
 description = A Django Library to send notifications in easy way
 readme = "README.md"
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/Hashtrust-technology-private-limited/notifications
+url = https://github.com/Hashtrust-technology-private-limited/django-easy-notify
 author = Hashtrust Technologies Private Limited
 author_email = support@hashtrust.in
 license = MIT License
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
```

