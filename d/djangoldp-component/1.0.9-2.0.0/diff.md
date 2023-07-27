# Comparing `tmp/djangoldp_component-1.0.9.tar.gz` & `tmp/djangoldp_component-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_component-1.0.9.tar", last modified: Tue Jun 20 16:28:41 2023, max compression
+gzip compressed data, was "djangoldp_component-2.0.0.tar", last modified: Thu Jul 27 15:06:58 2023, max compression
```

## Comparing `djangoldp_component-1.0.9.tar` & `djangoldp_component-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:28:41.000000 djangoldp_component-1.0.9/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-06-20 16:28:22.000000 djangoldp_component-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:28:41.000000 djangoldp_component-1.0.9/djangoldp_component.egg-info/
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-20 16:28:41.000000 djangoldp_component-1.0.9/djangoldp_component.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 16:28:41.000000 djangoldp_component-1.0.9/djangoldp_component.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      599 2023-06-20 16:28:41.000000 djangoldp_component-1.0.9/djangoldp_component.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-20 16:28:41.000000 djangoldp_component-1.0.9/djangoldp_component.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 16:28:41.000000 djangoldp_component-1.0.9/djangoldp_component.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-06-20 16:28:22.000000 djangoldp_component-1.0.9/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-20 16:28:41.000000 djangoldp_component-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-20 16:28:41.000000 djangoldp_component-1.0.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:28:41.000000 djangoldp_component-1.0.9/djangoldp_component/
--rw-rw-rw-   0 root         (0) root         (0)     9713 2023-06-20 16:28:22.000000 djangoldp_component-1.0.9/djangoldp_component/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1630 2023-06-20 16:28:22.000000 djangoldp_component-1.0.9/djangoldp_component/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-20 16:28:39.000000 djangoldp_component-1.0.9/djangoldp_component/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-20 16:28:22.000000 djangoldp_component-1.0.9/djangoldp_component/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-20 16:28:22.000000 djangoldp_component-1.0.9/djangoldp_component/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 16:28:41.000000 djangoldp_component-1.0.9/djangoldp_component/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    12897 2023-06-20 16:28:22.000000 djangoldp_component-1.0.9/djangoldp_component/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-06-20 16:28:22.000000 djangoldp_component-1.0.9/djangoldp_component/migrations/0003_component_auto_menu.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:28:22.000000 djangoldp_component-1.0.9/djangoldp_component/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-20 16:28:22.000000 djangoldp_component-1.0.9/djangoldp_component/migrations/0002_delete_dependency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:58.480415 djangoldp_component-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-27 15:06:58.480415 djangoldp_component-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:58.476415 djangoldp_component-2.0.0/djangoldp_component/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-27 15:06:55.000000 djangoldp_component-2.0.0/djangoldp_component/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:58.480415 djangoldp_component-2.0.0/djangoldp_component/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    12897 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/migrations/0002_delete_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/migrations/0003_component_auto_menu.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9712 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/djangoldp_component/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:58.476415 djangoldp_component-2.0.0/djangoldp_component.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-27 15:06:58.000000 djangoldp_component-2.0.0/djangoldp_component.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-27 15:06:58.000000 djangoldp_component-2.0.0/djangoldp_component.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 15:06:58.000000 djangoldp_component-2.0.0/djangoldp_component.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 15:06:58.000000 djangoldp_component-2.0.0/djangoldp_component.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-27 15:06:58.000000 djangoldp_component-2.0.0/djangoldp_component.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-27 15:06:58.480415 djangoldp_component-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-27 15:06:39.000000 djangoldp_component-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_component-1.0.9/README.md` & `djangoldp_component-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.9/djangoldp_component.egg-info/SOURCES.txt` & `djangoldp_component-2.0.0/djangoldp_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.9/setup.cfg` & `djangoldp_component-2.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 author_email = jbaptiste@startinblox.com
 description = djangoldp component management package
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp~=2.1
-	djangoldp_account~=2.3
+	djangoldp~=3.0
+	djangoldp_account~=3.0
 
 [semantic_release]
 version_source = tag
 version_variable = djangoldp_component/__init__.py:__version__
 commit_parser = commit_parser.parse
 
 [egg_info]
```

### Comparing `djangoldp_component-1.0.9/djangoldp_component/models.py` & `djangoldp_component-2.0.0/djangoldp_component/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.db import models
 from django.db.models.signals import pre_save
 from django.dispatch import receiver
 from django.utils.text import slugify
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from djangoldp.models import Model
 from rest_framework.exceptions import ValidationError
 
 
 class Component(Model):
     friendly_name = models.CharField(max_length=255, blank=True, null=True)
     name = models.CharField(
```

### Comparing `djangoldp_component-1.0.9/djangoldp_component/admin.py` & `djangoldp_component-2.0.0/djangoldp_component/admin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.contrib import admin
 from djangoldp.admin import DjangoLDPAdmin
 
 from .models import Component, ComponentScriptTag, Package, Parameter, ServerParameter
 
 
+@admin.register(ComponentScriptTag, Parameter, ServerParameter)
 class EmptyAdmin(admin.ModelAdmin):
     def get_model_perms(self, request):
         return {}
 
 
 class ParameterInline(admin.TabularInline):
     model = Parameter
@@ -23,28 +24,25 @@
 
 class ServerParameterInline(admin.TabularInline):
     model = ServerParameter
     exclude = ("urlid", "is_backlink", "allow_create_backlink")
     extra = 0
 
 
+@admin.register(Component)
 class ComponentAdmin(DjangoLDPAdmin):
     list_display = ("urlid", "friendly_name", "short_description")
     exclude = ("urlid", "slug", "is_backlink", "allow_create_backlink")
     inlines = [ComponentScriptTagInline, ParameterInline]
     search_fields = ["urlid", "friendly_name", "name", "parameters__parameter__name"]
     ordering = ["urlid"]
 
 
+@admin.register(Package)
 class PackageAdmin(DjangoLDPAdmin):
     list_display = ("urlid", "friendly_name", "short_description")
     exclude = ("urlid", "slug", "is_backlink", "allow_create_backlink")
     inlines = [ServerParameterInline]
     search_fields = ["urlid", "friendly_name", "parameters__parameter__name"]
     ordering = ["urlid"]
 
 
-admin.site.register(Component, ComponentAdmin)
-admin.site.register(Parameter, EmptyAdmin)
-admin.site.register(ComponentScriptTag, EmptyAdmin)
-admin.site.register(ServerParameter, EmptyAdmin)
-admin.site.register(Package, PackageAdmin)
```

### Comparing `djangoldp_component-1.0.9/djangoldp_component/migrations/0001_initial.py` & `djangoldp_component-2.0.0/djangoldp_component/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.9/djangoldp_component/migrations/0003_component_auto_menu.py` & `djangoldp_component-2.0.0/djangoldp_component/migrations/0003_component_auto_menu.py`

 * *Files identical despite different names*

