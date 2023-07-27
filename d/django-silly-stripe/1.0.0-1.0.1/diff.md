# Comparing `tmp/django-silly-stripe-1.0.0.tar.gz` & `tmp/django-silly-stripe-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-stripe-1.0.0.tar", last modified: Thu Jul 27 16:32:16 2023, max compression
+gzip compressed data, was "django-silly-stripe-1.0.1.tar", last modified: Thu Jul 27 19:16:04 2023, max compression
```

## Comparing `django-silly-stripe-1.0.0.tar` & `django-silly-stripe-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-27 16:32:16.561769 django-silly-stripe-1.0.0/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-stripe-1.0.0/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3241 2023-07-27 16:32:16.561769 django-silly-stripe-1.0.0/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2618 2023-07-27 13:44:35.000000 django-silly-stripe-1.0.0/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-27 16:32:16.557769 django-silly-stripe-1.0.0/django_silly_stripe/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       52 2023-07-27 16:30:23.000000 django-silly-stripe-1.0.0/django_silly_stripe/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1973 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.0/django_silly_stripe/admin.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1048 2023-07-27 14:11:12.000000 django-silly-stripe-1.0.0/django_silly_stripe/conf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      822 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.0/django_silly_stripe/helpers.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3428 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.0/django_silly_stripe/models.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2203 2023-07-27 13:47:01.000000 django-silly-stripe-1.0.0/django_silly_stripe/urls.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     9395 2023-07-27 16:31:45.000000 django-silly-stripe-1.0.0/django_silly_stripe/views.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-27 16:32:16.561769 django-silly-stripe-1.0.0/django_silly_stripe.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3241 2023-07-27 16:32:16.000000 django-silly-stripe-1.0.0/django_silly_stripe.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      450 2023-07-27 16:32:16.000000 django-silly-stripe-1.0.0/django_silly_stripe.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-07-27 16:32:16.000000 django-silly-stripe-1.0.0/django_silly_stripe.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       14 2023-07-27 16:32:16.000000 django-silly-stripe-1.0.0/django_silly_stripe.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       20 2023-07-27 16:32:16.000000 django-silly-stripe-1.0.0/django_silly_stripe.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-07-27 16:32:16.561769 django-silly-stripe-1.0.0/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1642 2023-07-12 12:08:15.000000 django-silly-stripe-1.0.0/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-27 19:16:04.859230 django-silly-stripe-1.0.1/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-stripe-1.0.1/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1727 2023-07-27 19:16:04.859230 django-silly-stripe-1.0.1/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1104 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.1/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-27 19:16:04.855230 django-silly-stripe-1.0.1/django_silly_stripe/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       52 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.1/django_silly_stripe/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1973 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.1/django_silly_stripe/admin.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1406 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.1/django_silly_stripe/conf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      942 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.1/django_silly_stripe/helpers.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3428 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.1/django_silly_stripe/models.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2203 2023-07-27 16:54:42.000000 django-silly-stripe-1.0.1/django_silly_stripe/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     8757 2023-07-27 19:14:42.000000 django-silly-stripe-1.0.1/django_silly_stripe/views.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-07-27 19:16:04.855230 django-silly-stripe-1.0.1/django_silly_stripe.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1727 2023-07-27 19:16:04.000000 django-silly-stripe-1.0.1/django_silly_stripe.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      450 2023-07-27 19:16:04.000000 django-silly-stripe-1.0.1/django_silly_stripe.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-07-27 19:16:04.000000 django-silly-stripe-1.0.1/django_silly_stripe.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       14 2023-07-27 19:16:04.000000 django-silly-stripe-1.0.1/django_silly_stripe.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       20 2023-07-27 19:16:04.000000 django-silly-stripe-1.0.1/django_silly_stripe.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-07-27 19:16:04.859230 django-silly-stripe-1.0.1/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1642 2023-07-12 12:08:15.000000 django-silly-stripe-1.0.1/setup.py
```

### Comparing `django-silly-stripe-1.0.0/LICENSE.md` & `django-silly-stripe-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.0/django_silly_stripe/admin.py` & `django-silly-stripe-1.0.1/django_silly_stripe/admin.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.0/django_silly_stripe/models.py` & `django-silly-stripe-1.0.1/django_silly_stripe/models.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.0/django_silly_stripe/urls.py` & `django-silly-stripe-1.0.1/django_silly_stripe/urls.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.0/django_silly_stripe/views.py` & `django-silly-stripe-1.0.1/django_silly_stripe/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,26 +25,16 @@
     if not request.user.is_authenticated or not request.user.is_active:
         return JsonResponse({"message": "Permission denied"}, status=403)
     if request.method != 'GET':
         return JsonResponse({"message": "Method not allowed"}, status=405)
     stripe.api_key = dss_conf["DSS_SECRET_KEY"]
     user = request.user
     if not hasattr(user, 'customer'):
-            new_customer_data = stripe.Customer.create(
-                email=request.user.email,
-                name=request.user.username,
-                metadata={
-                    'user_id': request.user.id,
-                }
-            )
-            # print("===new_customer_data: ", new_customer_data)
-            user_creates_new_customer(
-                user,
-                new_customer_data,
-            )
+        # print("===new_customer_data: ", new_customer_data)
+        user_creates_new_customer(user)
 
     stripe.billing_portal.Configuration.create(
             business_profile={
                 "headline": "Cactus Practice partners with Stripe for simplified billing.",
             },
             features={"invoice_history": {"enabled": True}},
         )
@@ -164,26 +154,16 @@
         data = json.loads(request.body)
         # print("===data: ", data)
         price_id = data["priceId"]
 
         stripe.api_key = dss_conf["DSS_SECRET_KEY"]
         user = request.user
         if not hasattr(user, 'customer'):
-            new_customer_data = stripe.Customer.create(
-                email=request.user.email,
-                name=request.user.username,
-                metadata={
-                    'user_id': request.user.id,
-                }
-            )
             # print("===new_customer_data: ", new_customer_data)
-            user_creates_new_customer(
-                user,
-                new_customer_data,
-            )
+            user_creates_new_customer(user)
 
         else:
             if dss_conf['SUBSCRIBE_ONLY_ONCE']:
                 product = Price.objects.get(id=price_id).product
                 if Subscription.objects.filter(
                         customer=user.customer,
                         product=product,
```

### Comparing `django-silly-stripe-1.0.0/setup.py` & `django-silly-stripe-1.0.1/setup.py`

 * *Files identical despite different names*

