# Comparing `tmp/django_moses-0.8.8.tar.gz` & `tmp/django_moses-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_moses-0.8.8.tar", max compression
+gzip compressed data, was "django_moses-0.8.9.tar", max compression
```

## Comparing `django_moses-0.8.8.tar` & `django_moses-0.8.9.tar`

### file list

```diff
@@ -1,55 +1,16 @@
--rw-r--r--   0        0        0       21 2023-07-27 16:00:53.708476 django_moses-0.8.8/.git/HEAD
--rw-r--r--   0        0        0      307 2023-07-27 16:00:53.710019 django_moses-0.8.8/.git/config
--rw-r--r--   0        0        0       73 2023-07-27 16:00:51.120825 django_moses-0.8.8/.git/description
--rwxr-xr-x   0        0        0      478 2023-07-27 16:00:51.122325 django_moses-0.8.8/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      896 2023-07-27 16:00:51.121246 django_moses-0.8.8/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     4726 2023-07-27 16:00:51.122695 django_moses-0.8.8/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      189 2023-07-27 16:00:51.123527 django_moses-0.8.8/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      424 2023-07-27 16:00:51.123863 django_moses-0.8.8/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1643 2023-07-27 16:00:51.122127 django_moses-0.8.8/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      416 2023-07-27 16:00:51.123692 django_moses-0.8.8/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1374 2023-07-27 16:00:51.124019 django_moses-0.8.8/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4898 2023-07-27 16:00:51.121947 django_moses-0.8.8/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      544 2023-07-27 16:00:51.123082 django_moses-0.8.8/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1492 2023-07-27 16:00:51.123350 django_moses-0.8.8/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     2783 2023-07-27 16:00:51.124496 django_moses-0.8.8/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0        0        0     3650 2023-07-27 16:00:51.124252 django_moses-0.8.8/.git/hooks/update.sample
--rw-r--r--   0        0        0     2795 2023-07-27 16:01:43.950144 django_moses-0.8.8/.git/index
--rw-r--r--   0        0        0      240 2023-07-27 16:00:51.120499 django_moses-0.8.8/.git/info/exclude
--rw-r--r--   0        0        0      181 2023-07-27 16:00:53.709134 django_moses-0.8.8/.git/logs/HEAD
--rw-r--r--   0        0        0      181 2023-07-27 16:00:53.709312 django_moses-0.8.8/.git/logs/refs/heads/main
--rw-r--r--   0        0        0      181 2023-07-27 16:00:53.708110 django_moses-0.8.8/.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0        0        0    17340 2023-07-27 16:00:53.696308 django_moses-0.8.8/.git/objects/pack/pack-abdb98947593bcb20daa1b77c108b46a3c78a367.idx
--rw-r--r--   0        0        0   110698 2023-07-27 16:00:53.695858 django_moses-0.8.8/.git/objects/pack/pack-abdb98947593bcb20daa1b77c108b46a3c78a367.pack
--rw-r--r--   0        0        0      177 2023-07-27 16:00:53.706733 django_moses-0.8.8/.git/packed-refs
--rw-r--r--   0        0        0       41 2023-07-27 16:00:53.709035 django_moses-0.8.8/.git/refs/heads/main
--rw-r--r--   0        0        0       30 2023-07-27 16:00:53.708195 django_moses-0.8.8/.git/refs/remotes/origin/HEAD
--rw-r--r--   0        0        0      912 2023-07-27 16:00:53.711168 django_moses-0.8.8/.github/workflows/test-and-merge.yml
--rw-r--r--   0        0        0       55 2023-07-27 16:00:53.711287 django_moses-0.8.8/.gitignore
--rw-r--r--   0        0        0     1460 2023-07-27 16:00:53.711409 django_moses-0.8.8/LICENSE
--rw-r--r--   0        0        0      129 2023-07-27 16:00:53.711513 django_moses-0.8.8/MANIFEST.in
--rw-r--r--   0        0        0     1741 2023-07-27 16:00:53.711650 django_moses-0.8.8/README.md
--rw-r--r--   0        0        0        0 2023-07-27 16:00:53.711696 django_moses-0.8.8/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 16:00:53.711807 django_moses-0.8.8/moses/__init__.py
--rw-r--r--   0        0        0     2381 2023-07-27 16:00:53.711952 django_moses-0.8.8/moses/admin.py
--rw-r--r--   0        0        0       85 2023-07-27 16:00:53.712065 django_moses-0.8.8/moses/apps.py
--rw-r--r--   0        0        0     8696 2023-07-27 16:00:53.712223 django_moses-0.8.8/moses/authentication.py
--rw-r--r--   0        0        0     2830 2023-07-27 16:00:53.712347 django_moses-0.8.8/moses/conf.py
--rw-r--r--   0        0        0      933 2023-07-27 16:00:53.712450 django_moses-0.8.8/moses/decorators.py
--rw-r--r--   0        0        0     7588 2023-07-27 16:00:53.712635 django_moses-0.8.8/moses/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-27 16:00:53.712684 django_moses-0.8.8/moses/migrations/__init__.py
--rw-r--r--   0        0        0     9741 2023-07-27 16:00:53.712845 django_moses-0.8.8/moses/models.py
--rw-r--r--   0        0        0     9418 2023-07-27 16:00:53.712994 django_moses-0.8.8/moses/serializers.py
--rw-r--r--   0        0        0     2147 2023-07-27 16:00:53.713224 django_moses-0.8.8/moses/templates/admin/login.html
--rw-r--r--   0        0        0     1965 2023-07-27 16:00:53.713345 django_moses-0.8.8/moses/urls.py
--rw-r--r--   0        0        0    12102 2023-07-27 16:00:53.713490 django_moses-0.8.8/moses/views.py
--rw-r--r--   0        0        0      792 2023-07-27 16:16:16.138444 django_moses-0.8.8/pyproject.toml
--rw-r--r--   0        0        0      980 2023-07-27 16:00:53.713785 django_moses-0.8.8/runConfigurations/test moses.run.xml
--rw-r--r--   0        0        0        0 2023-07-27 16:00:53.713887 django_moses-0.8.8/test_project/__init__.py
--rwxr-xr-x   0        0        0      785 2023-07-27 16:00:53.713998 django_moses-0.8.8/test_project/manage.py
--rw-r--r--   0        0        0     2420 2023-07-27 16:00:53.714100 django_moses-0.8.8/test_project/settings.py
--rw-r--r--   0        0        0        0 2023-07-27 16:00:53.714187 django_moses-0.8.8/test_project/tests/__init__.py
--rw-r--r--   0        0        0     8768 2023-07-27 16:00:53.714321 django_moses-0.8.8/test_project/tests/accounts.py
--rw-r--r--   0        0        0      156 2023-07-27 16:00:53.714418 django_moses-0.8.8/test_project/tests/mocks.py
--rw-r--r--   0        0        0      202 2023-07-27 16:00:53.714506 django_moses-0.8.8/test_project/urls.py
--rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 django_moses-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1460 2023-07-27 16:00:53.711409 django_moses-0.8.9/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-27 16:00:53.711807 django_moses-0.8.9/moses/__init__.py
+-rw-r--r--   0        0        0     2381 2023-07-27 16:00:53.711952 django_moses-0.8.9/moses/admin.py
+-rw-r--r--   0        0        0       85 2023-07-27 16:00:53.712065 django_moses-0.8.9/moses/apps.py
+-rw-r--r--   0        0        0     8696 2023-07-27 16:00:53.712223 django_moses-0.8.9/moses/authentication.py
+-rw-r--r--   0        0        0     2830 2023-07-27 16:00:53.712347 django_moses-0.8.9/moses/conf.py
+-rw-r--r--   0        0        0      933 2023-07-27 16:00:53.712450 django_moses-0.8.9/moses/decorators.py
+-rw-r--r--   0        0        0     7588 2023-07-27 16:00:53.712635 django_moses-0.8.9/moses/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:00:53.712684 django_moses-0.8.9/moses/migrations/__init__.py
+-rw-r--r--   0        0        0     9741 2023-07-27 16:00:53.712845 django_moses-0.8.9/moses/models.py
+-rw-r--r--   0        0        0     9418 2023-07-27 16:00:53.712994 django_moses-0.8.9/moses/serializers.py
+-rw-r--r--   0        0        0     2147 2023-07-27 16:00:53.713224 django_moses-0.8.9/moses/templates/admin/login.html
+-rw-r--r--   0        0        0     1965 2023-07-27 16:00:53.713345 django_moses-0.8.9/moses/urls.py
+-rw-r--r--   0        0        0    12102 2023-07-27 16:00:53.713490 django_moses-0.8.9/moses/views.py
+-rw-r--r--   0        0        0      796 2023-07-27 16:19:11.198697 django_moses-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 django_moses-0.8.9/PKG-INFO
```

### Comparing `django_moses-0.8.8/LICENSE` & `django_moses-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_moses-0.8.8/moses/admin.py` & `django_moses-0.8.9/moses/admin.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.8.8/moses/authentication.py` & `django_moses-0.8.9/moses/authentication.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.8.8/moses/conf.py` & `django_moses-0.8.9/moses/conf.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.8.8/moses/decorators.py` & `django_moses-0.8.9/moses/decorators.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.8.8/moses/migrations/0001_initial.py` & `django_moses-0.8.9/moses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.8.8/moses/models.py` & `django_moses-0.8.9/moses/models.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.8.8/moses/serializers.py` & `django_moses-0.8.9/moses/serializers.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.8.8/moses/templates/admin/login.html` & `django_moses-0.8.9/moses/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django_moses-0.8.8/moses/urls.py` & `django_moses-0.8.9/moses/urls.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.8.8/moses/views.py` & `django_moses-0.8.9/moses/views.py`

 * *Files identical despite different names*

### Comparing `django_moses-0.8.8/PKG-INFO` & `django_moses-0.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-moses
-Version: 0.8.8
+Version: 0.8.9
 Summary: Advanced authentication with OTP and phone number verification
 Author: Vassily Vorobyov
 Author-email: vassily.v.v@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

