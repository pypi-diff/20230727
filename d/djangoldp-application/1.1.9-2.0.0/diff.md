# Comparing `tmp/djangoldp_application-1.1.9.tar.gz` & `tmp/djangoldp_application-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_application-1.1.9.tar", last modified: Wed May 24 08:53:26 2023, max compression
+gzip compressed data, was "djangoldp_application-2.0.0.tar", last modified: Thu Jul 27 15:06:37 2023, max compression
```

## Comparing `djangoldp_application-1.1.9.tar` & `djangoldp_application-2.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:53:26.000000 djangoldp_application-1.1.9/
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2023-05-24 08:53:26.000000 djangoldp_application-1.1.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-24 08:53:26.000000 djangoldp_application-1.1.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:53:26.000000 djangoldp_application-1.1.9/djangoldp_application.egg-info/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-24 08:53:26.000000 djangoldp_application-1.1.9/djangoldp_application.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 08:53:26.000000 djangoldp_application-1.1.9/djangoldp_application.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1348 2023-05-24 08:53:26.000000 djangoldp_application-1.1.9/djangoldp_application.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-24 08:53:26.000000 djangoldp_application-1.1.9/djangoldp_application.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-24 08:53:26.000000 djangoldp_application-1.1.9/djangoldp_application.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:53:26.000000 djangoldp_application-1.1.9/djangoldp_application/
--rw-rw-rw-   0 root         (0) root         (0)    17495 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/views.py
--rw-rw-rw-   0 root         (0) root         (0)    19328 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5488 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-24 08:53:24.000000 djangoldp_application-1.1.9/djangoldp_application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 08:53:26.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0009_applicationgraphics.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0014_auto_20230512_1613.py
--rw-rw-rw-   0 root         (0) root         (0)    22281 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0011_auto_20230512_1555.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0010_auto_20230331_0921.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0013_auto_20230512_1608.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0012_auto_20230512_1556.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0003_application_api_url.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0005_auto_20230331_0850.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0007_auto_20230331_0857.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0008_applicationnpm.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0004_auto_20230328_1657.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0002_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-05-24 08:53:08.000000 djangoldp_application-1.1.9/djangoldp_application/migrations/0006_applicationservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:37.531599 djangoldp_application-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-27 15:06:37.531599 djangoldp_application-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:37.527599 djangoldp_application-2.0.0/djangoldp_application/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-07-27 15:06:35.000000 djangoldp_application-2.0.0/djangoldp_application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5227 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:37.531599 djangoldp_application-2.0.0/djangoldp_application/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    22281 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0002_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0003_application_api_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0004_auto_20230328_1657.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0005_auto_20230331_0850.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0006_applicationservice.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0007_auto_20230331_0857.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0008_applicationnpm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0009_applicationgraphics.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0010_auto_20230331_0921.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0011_auto_20230512_1555.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0012_auto_20230512_1556.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0013_auto_20230512_1608.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/0014_auto_20230512_1613.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19843 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    26614 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/djangoldp_application/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:06:37.527599 djangoldp_application-2.0.0/djangoldp_application.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-07-27 15:06:37.000000 djangoldp_application-2.0.0/djangoldp_application.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-07-27 15:06:37.000000 djangoldp_application-2.0.0/djangoldp_application.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 15:06:37.000000 djangoldp_application-2.0.0/djangoldp_application.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-27 15:06:37.000000 djangoldp_application-2.0.0/djangoldp_application.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-27 15:06:37.000000 djangoldp_application-2.0.0/djangoldp_application.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-27 15:06:37.531599 djangoldp_application-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-07-27 15:06:18.000000 djangoldp_application-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangoldp_application-1.1.9/README.md` & `djangoldp_application-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/setup.cfg` & `djangoldp_application-2.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 author_email = jbaptiste@startinblox.com
 description = djangoldp application management package
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
-	djangoldp~=2.1
+	djangoldp~=3.0
 	djangoldp_branding
-	djangoldp_account~=2.3
+	djangoldp_account~=3.0
 	djangoldp_component
 	djangorestframework-yaml~=2.0
 
 [semantic_release]
 version_source = tag
 version_variable = djangoldp_application/__init__.py:__version__
 commit_parser = commit_parser.parse
```

### Comparing `djangoldp_application-1.1.9/djangoldp_application.egg-info/SOURCES.txt` & `djangoldp_application-2.0.0/djangoldp_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/djangoldp_application/views.py` & `djangoldp_application-2.0.0/djangoldp_application/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,45 @@
-from .models import Application, Federation
 from django.conf import settings
 from django.core.mail import send_mail
 from django.http import JsonResponse
 from django.template import loader
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
+from djangoldp.filters import LocalObjectOnContainerPathBackend
+from djangoldp.models import Model
+from djangoldp.views import LDPViewSet
+from djangoldp_application.models import (
+    Application,
+    ApplicationComponent,
+    ApplicationComponentParameter,
+    ApplicationGraphics,
+    ApplicationNPM,
+    ApplicationPackage,
+    ApplicationPackageParameter,
+    ApplicationService,
+    ComponentExtension,
+    ComponentExtensionParameter,
+    Federation,
+)
 from djangoldp_component.models import Component, Package
-from rest_framework import serializers, viewsets
+from rest_framework import response, serializers, status, viewsets
 from rest_framework_yaml.parsers import YAMLParser
 from rest_framework_yaml.renderers import YAMLRenderer
 
-
-EMAIL_FROM = (getattr(settings, 'DEFAULT_FROM_EMAIL', False) or getattr(settings, 'EMAIL_HOST_USER', False))
+EMAIL_FROM = getattr(settings, "DEFAULT_FROM_EMAIL", False) or getattr(
+    settings, "EMAIL_HOST_USER", False
+)
 ANSIBLE_SERVERS = set({"127.0.0.1"})
 
 
 if hasattr(settings, "ANSIBLE_SERVERS"):
     ANSIBLE_SERVERS = ANSIBLE_SERVERS.union(getattr(settings, "ANSIBLE_SERVERS"))
 
 
 def get_client_ip(request):
-    x_forwarded_for = request.META.get("HTTP_X_FORWARDED_FOR")
+    x_forwarded_for = request.headers.get("x-forwarded-for")
     if x_forwarded_for:
         ip = x_forwarded_for.split(",")[0]
     else:
         ip = request.META.get("REMOTE_ADDR")
     return ip
 
 
@@ -156,36 +172,60 @@
                 if parameter.key == "route":
                     insertComponent["route"] = format(parameter.value)
                     keys.append(parameter.key)
                 elif parameter.key == "defaultRoute":
                     insertComponent["defaultRoute"] = format(parameter.value)
                     keys.append(parameter.key)
                 elif not parameter.key in keys:
-                    insertComponent["parameters"][parameter.key] = format(parameter.value)
+                    insertComponent["parameters"][parameter.key] = format(
+                        parameter.value
+                    )
                     keys.append(parameter.key)
-                elif hasattr(insertComponent["parameters"][parameter.key], "__len__") and (not isinstance(insertComponent["parameters"][parameter.key], str)):
-                    insertComponent["parameters"][parameter.key].append(format(parameter.value))
+                elif hasattr(
+                    insertComponent["parameters"][parameter.key], "__len__"
+                ) and (
+                    not isinstance(insertComponent["parameters"][parameter.key], str)
+                ):
+                    insertComponent["parameters"][parameter.key].append(
+                        format(parameter.value)
+                    )
                 else:
-                    insertComponent["parameters"][parameter.key] = [insertComponent["parameters"][parameter.key], format(parameter.value)]
+                    insertComponent["parameters"][parameter.key] = [
+                        insertComponent["parameters"][parameter.key],
+                        format(parameter.value),
+                    ]
             missingKeys = []
             for parameter in component.parameters.all():
                 if not parameter.key in keys:
                     if parameter.key == "route":
                         insertComponent["route"] = format(parameter.default)
                         missingKeys.append(parameter.key)
                     elif parameter.key == "defaultRoute":
                         insertComponent["defaultRoute"] = format(parameter.default)
                         keys.append(parameter.key)
                     elif not parameter.key in missingKeys:
-                        insertComponent["parameters"][parameter.key] = format(parameter.default)
+                        insertComponent["parameters"][parameter.key] = format(
+                            parameter.default
+                        )
                         missingKeys.append(parameter.key)
-                    elif hasattr(insertComponent["parameters"][parameter.key], "__len__") and (not isinstance(insertComponent["parameters"][parameter.key], str)):
-                        insertComponent["parameters"][parameter.key].append(format(parameter.default))
+                    elif hasattr(
+                        insertComponent["parameters"][parameter.key], "__len__"
+                    ) and (
+                        not isinstance(
+                            insertComponent["parameters"][parameter.key], str
+                        )
+                    ):
+                        insertComponent["parameters"][parameter.key].append(
+                            format(parameter.default)
+                        )
                     else:
-                        insertComponent["parameters"][parameter.key] = [insertComponent["parameters"][parameter.key], format(parameter.default)]
+                        insertComponent["parameters"][parameter.key] = [
+                            insertComponent["parameters"][parameter.key],
+                            format(parameter.default),
+                        ]
             for extensionComponent in applicationComponent.obj.extensions.all():
                 extension = Component.objects.get(id=extensionComponent.component_id)
                 componentExtension = {
                     "type": extension.name,
                     "route": format(component.preferred_route),
                     "parameters": {},
                     "experimental": [],
@@ -199,36 +239,64 @@
                     if parameter.key == "route":
                         componentExtension["route"] = format(parameter.value)
                         keys.append(parameter.key)
                     elif parameter.key == "defaultRoute":
                         componentExtension["defaultRoute"] = format(parameter.value)
                         keys.append(parameter.key)
                     elif not parameter.key in keys:
-                        componentExtension["parameters"][parameter.key] = format(parameter.value)
+                        componentExtension["parameters"][parameter.key] = format(
+                            parameter.value
+                        )
                         keys.append(parameter.key)
-                    elif hasattr(insertComponent["parameters"][parameter.key], "__len__") and (not isinstance(componentExtension["parameters"][parameter.key], str)):
-                        componentExtension["parameters"][parameter.key].append(format(parameter.value))
+                    elif hasattr(
+                        insertComponent["parameters"][parameter.key], "__len__"
+                    ) and (
+                        not isinstance(
+                            componentExtension["parameters"][parameter.key], str
+                        )
+                    ):
+                        componentExtension["parameters"][parameter.key].append(
+                            format(parameter.value)
+                        )
                     else:
-                        componentExtension["parameters"][parameter.key] = [componentExtension["parameters"][parameter.key], format(parameter.value)]
+                        componentExtension["parameters"][parameter.key] = [
+                            componentExtension["parameters"][parameter.key],
+                            format(parameter.value),
+                        ]
                 missingKeys = []
                 for parameter in extension.parameters.all():
                     if not parameter.key in keys:
                         if parameter.key == "route":
                             componentExtension["route"] = format(parameter.default)
                             missingKeys.append(parameter.key)
                         elif parameter.key == "defaultRoute":
-                            componentExtension["defaultRoute"] = format(parameter.default)
+                            componentExtension["defaultRoute"] = format(
+                                parameter.default
+                            )
                             missingKeys.append(parameter.key)
                         elif not parameter.key in missingKeys:
-                            componentExtension["parameters"][parameter.key] = format(parameter.default)
+                            componentExtension["parameters"][parameter.key] = format(
+                                parameter.default
+                            )
                             missingKeys.append(parameter.key)
-                        elif hasattr(componentExtension["parameters"][parameter.key], "__len__") and (not isinstance(componentExtension["parameters"][parameter.key], str)):
-                            componentExtension["parameters"][parameter.key].append(format(parameter.default))
+                        elif hasattr(
+                            componentExtension["parameters"][parameter.key], "__len__"
+                        ) and (
+                            not isinstance(
+                                componentExtension["parameters"][parameter.key], str
+                            )
+                        ):
+                            componentExtension["parameters"][parameter.key].append(
+                                format(parameter.default)
+                            )
                         else:
-                            componentExtension["parameters"][parameter.key] = [componentExtension["parameters"][parameter.key], format(parameter.default)]
+                            componentExtension["parameters"][parameter.key] = [
+                                componentExtension["parameters"][parameter.key],
+                                format(parameter.default),
+                            ]
                 insertComponent["extensions"].append(componentExtension)
             serialized["apps"]["hosts"][application["slug"]]["components"].append(
                 insertComponent
             )
 
         insertDependencies = []
         for applicationPackage in application["packages"]:
@@ -237,30 +305,54 @@
                 "distribution": package.distribution,
                 "module": package.module,
                 "parameters": {},
             }
             keys = []
             for parameter in applicationPackage.obj.parameters.all():
                 if not parameter.key in keys:
-                    insertDependency["parameters"][parameter.key] = format(parameter.value)
+                    insertDependency["parameters"][parameter.key] = format(
+                        parameter.value
+                    )
                     keys.append(parameter.key)
-                elif hasattr(insertDependency["parameters"][parameter.key], "__len__") and (not isinstance(insertDependency["parameters"][parameter.key], str)):
-                    insertDependency["parameters"][parameter.key].append(format(parameter.value))
+                elif hasattr(
+                    insertDependency["parameters"][parameter.key], "__len__"
+                ) and (
+                    not isinstance(insertDependency["parameters"][parameter.key], str)
+                ):
+                    insertDependency["parameters"][parameter.key].append(
+                        format(parameter.value)
+                    )
                 else:
-                    insertDependency["parameters"][parameter.key] = [insertDependency["parameters"][parameter.key], format(parameter.value)]
+                    insertDependency["parameters"][parameter.key] = [
+                        insertDependency["parameters"][parameter.key],
+                        format(parameter.value),
+                    ]
             missingKeys = []
             for parameter in package.parameters.all():
                 if not parameter.key in keys:
                     if not parameter.key in missingKeys:
-                        insertDependency["parameters"][parameter.key] = format(parameter.default)
+                        insertDependency["parameters"][parameter.key] = format(
+                            parameter.default
+                        )
                         missingKeys.append(parameter.key)
-                    elif hasattr(insertDependency["parameters"][parameter.key], "__len__") and (not isinstance(insertDependency["parameters"][parameter.key], str)):
-                        insertDependency["parameters"][parameter.key].append(format(parameter.default))
+                    elif hasattr(
+                        insertDependency["parameters"][parameter.key], "__len__"
+                    ) and (
+                        not isinstance(
+                            insertDependency["parameters"][parameter.key], str
+                        )
+                    ):
+                        insertDependency["parameters"][parameter.key].append(
+                            format(parameter.default)
+                        )
                     else:
-                        insertDependency["parameters"][parameter.key] = [insertDependency["parameters"][parameter.key], format(parameter.default)]
+                        insertDependency["parameters"][parameter.key] = [
+                            insertDependency["parameters"][parameter.key],
+                            format(parameter.default),
+                        ]
             insertDependencies.append(insertDependency)
         serialized["apps"]["hosts"][application["slug"]][
             "packages"
         ] = insertDependencies
 
         return serialized
 
@@ -296,77 +388,242 @@
     queryset = Application.objects.all()
     serializer_class = ApplicationDetailSerializer
     lookup_field = "slug"
     parser_classes = (YAMLParser,)
     renderer_classes = (YAMLRenderer,)
 
 
+class CreateApplicationViewSet(LDPViewSet):
+    model = Application
+    depth = 0
+
+    def __init__(self, **kwargs):
+        viewsets.ModelViewSet.__init__(self, **kwargs)
+        if self.permission_classes:
+            filtered_classes = [
+                p
+                for p in self.permission_classes
+                if hasattr(p, "filter_backends") and p.filter_backends is not None
+            ]
+            for p in filtered_classes:
+                self.filter_backends = list(
+                    set(self.filter_backends).union(set(p.filter_backends))
+                )
+
+        if getattr(settings, "DISABLE_LOCAL_OBJECT_FILTER", False):
+            if LocalObjectOnContainerPathBackend in self.filter_backends:
+                self.filter_backends.remove(LocalObjectOnContainerPathBackend)
+
+        self.serializer_class = self.build_read_serializer()
+        self.write_serializer_class = self.build_write_serializer()
+
+    def create(self, request, *args, **kwargs):
+        self.check_model_permissions(request)
+        serializer = self.get_write_serializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
+        if not self.is_safe_create(request.user, serializer.validated_data):
+            return response.Response(
+                {"detail": "You do not have permission to perform this action"},
+                status=status.HTTP_403_FORBIDDEN,
+            )
+
+        entry = self.perform_create(serializer)
+
+        if serializer.initial_data["source"]:
+            container, source_application = Model.resolve(
+                serializer.initial_data["source"]["@id"]
+            )
+
+            try:
+                for component_relation in source_application.components.all():
+                    (
+                        new_component_relation,
+                        created,
+                    ) = ApplicationComponent.objects.get_or_create(
+                        component=component_relation.component, application=entry
+                    )
+                    for parameter in component_relation.parameters.all():
+                        ApplicationComponentParameter.objects.create(
+                            component=new_component_relation,
+                            key=parameter.key,
+                            value=parameter.value,
+                        )
+                    for extension in component_relation.extensions.all():
+                        (
+                            new_extension_relation,
+                            created,
+                        ) = ComponentExtension.objects.get_or_create(
+                            base_component=new_component_relation,
+                            component=extension.component,
+                        )
+                        for parameter in new_extension_relation.parameters.all():
+                            ComponentExtensionParameter.objects.create(
+                                component=new_extension_relation,
+                                key=parameter.key,
+                                value=parameter.value,
+                            )
+            except:
+                pass
+
+            try:
+                for package_relation in source_application.packages.all():
+                    (
+                        new_package_relation,
+                        created,
+                    ) = ApplicationPackage.objects.get_or_create(
+                        package=package_relation.package, application=entry
+                    )
+                    for parameter in package_relation.parameters.all():
+                        ApplicationPackageParameter.objects.create(
+                            package=new_package_relation,
+                            key=parameter.key,
+                            value=parameter.value,
+                        )
+            except:
+                pass
+
+            try:
+                for application_npm in source_application.npms.all():
+                    ApplicationNPM.objects.get_or_create(
+                        application=entry,
+                        package=application_npm.package,
+                        version=application_npm.version,
+                    )
+            except:
+                pass
+
+            try:
+                for application_service in source_application.services.all():
+                    ApplicationService.objects.get_or_create(
+                        application=entry,
+                        primary_key=application_service.primary_key,
+                        key=application_service.key,
+                        value=application_service.value,
+                    )
+            except:
+                pass
+
+            try:
+                for application_graphic in source_application.graphics.all():
+                    ApplicationGraphics.objects.get_or_create(
+                        application=entry,
+                        primary_key=application_graphic.primary_key,
+                        key=application_graphic.key,
+                        value=application_graphic.value,
+                    )
+            except:
+                pass
+
+            try:
+                for application_federation in source_application.federation.all():
+                    Federation.objects.get_or_create(
+                        application=entry, target=application_federation.target
+                    )
+            except:
+                pass
+
+        response_serializer = self.get_serializer()
+        container, updated_entry = Model.resolve(serializer.instance.urlid)
+        data = response_serializer.to_representation(updated_entry)
+        headers = self.get_success_headers(data)
+        return response.Response(data, status=status.HTTP_201_CREATED, headers=headers)
+
+
 def mark_as_doing(request, slug):
     if request.method == "GET" and get_client_ip(request) in ANSIBLE_SERVERS:
         application = Application.objects.get(slug=slug)
         for deploy in application.deployments.filter(status="Todo"):
             deploy.status = "Doing"
             deploy.save()
         return JsonResponse({"status": "success"}, status=200)
     else:
         return JsonResponse({"status": "invalid request"}, status=400)
 
+
 def mark_as_done(request, slug):
     if request.method == "GET" and get_client_ip(request) in ANSIBLE_SERVERS:
         application = Application.objects.get(slug=slug)
         for deploy in application.deployments.filter(status="Doing"):
             deploy.status = "Done"
             deploy.save()
+
             if deploy.requester:
+                requester = deploy.requester
+            else:
+                requester = application.creator
+
+            if application.deployments.count() == 1:
                 html_message = loader.render_to_string(
-                    'email.html',
+                    "email.html",
                     {
-                        'on': application.client_url,
-                        'instance': {"summary": "Deployment done"},
-                        'author': deploy.requester.get_full_name(),
-                        'object': _("about your deployment of") + " https://{}".format(application.client_url)
-                    }
+                        "on": application.client_url,
+                        "instance": {"summary": _("Deployment done. You can use the default account: admin/admin. Don't forget to create your own account.")},
+                        "author": requester.get_full_name(),
+                        "object": "{} https://{}".format(
+                            _("About your deployment of"), application.client_url
+                        ),
+                    },
                 )
-
-                send_mail(
-                    _('Déploiement de ') + application.application_title + " (https://{})".format(application.client_url),
-                    "Deployment done",
-                    EMAIL_FROM,
-                    [deploy.requester.email],
-                    fail_silently=True,
-                    html_message=html_message
+            else :
+                html_message = loader.render_to_string(
+                    "email.html",
+                    {
+                        "on": application.client_url,
+                        "instance": {"summary": _("Deployment done.")},
+                        "author": requester.get_full_name(),
+                        "object": "{} https://{}".format(
+                            _("About your deployment of"), application.client_url
+                        ),
+                    },
                 )
 
+            send_mail(
+                "{} (https://{})".format(
+                    _("Déploiement de ") + application.application_title,
+                    application.client_url,
+                ),
+                _("Deployment done"),
+                EMAIL_FROM,
+                [requester.email],
+                fail_silently=True,
+                html_message=html_message,
+            )
+
         return JsonResponse({"status": "success"}, status=200)
     else:
         return JsonResponse({"status": "invalid request"}, status=400)
 
 
 def mark_as_failed(request, slug):
     if request.method == "GET" and get_client_ip(request) in ANSIBLE_SERVERS:
         application = Application.objects.get(slug=slug)
         for deploy in application.deployments.filter(status="Doing"):
             deploy.status = "Failed"
             deploy.save()
             if deploy.requester:
                 html_message = loader.render_to_string(
-                    'email.html',
+                    "email.html",
                     {
-                        'on': application.client_url,
-                        'instance': {"summary": "Deployment failed"},
-                        'author': deploy.requester.get_full_name(),
-                        'object': _("about your deployment of") + " https://{}".format(application.client_url)
-                    }
+                        "on": application.client_url,
+                        "instance": {"summary": _("Deployment failed")},
+                        "author": deploy.requester.get_full_name(),
+                        "object": "{} https://{}".format(
+                            _("About your deployment of"), application.client_url
+                        ),
+                    },
                 )
 
                 send_mail(
-                    _('Déploiement de ') + application.application_title + " (https://{})".format(application.client_url),
-                    "Deployment failed",
+                    "{} (https://{})".format(
+                        _("Déploiement de ") + application.application_title,
+                        application.client_url,
+                    ),
+                    _("Deployment failed"),
                     EMAIL_FROM,
                     [deploy.requester.email],
                     fail_silently=True,
-                    html_message=html_message
+                    html_message=html_message,
                 )
 
         return JsonResponse({"status": "success"}, status=200)
     else:
         return JsonResponse({"status": "invalid request"}, status=400)
```

### Comparing `djangoldp_application-1.1.9/djangoldp_application/models.py` & `djangoldp_application-2.0.0/djangoldp_application/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import uuid
+
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.db import models
-from django.db.models.signals import pre_save, post_save
+from django.db.models.signals import post_save, pre_save
 from django.dispatch import receiver
 from django.utils.text import slugify
-from django.utils.translation import ugettext_lazy as _
-from djangoldp_component.models import Component, Package
+from django.utils.translation import gettext_lazy as _
 from djangoldp.models import Model
+from djangoldp_component.models import Component, Package
 from rest_framework.exceptions import ValidationError
-import uuid
 
 
 class Application(Model):
     repository = models.CharField(max_length=255, blank=True, null=True)
     friendly_name = models.CharField(max_length=255, blank=True, null=True)
     short_description = models.CharField(max_length=255, blank=True, null=True)
     creator = models.ForeignKey(
@@ -40,29 +41,29 @@
     def __str__(self):
         try:
             return "{} ({})".format(self.friendly_name, self.urlid)
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        anonymous_perms = ["view"]
-        authenticated_perms = ["inherit", "add"]
+        anonymous_perms = []
+        authenticated_perms = ["add"]
         auto_author = "creator"
         container_path = "/applications/"
         depth = 2  # Do not serialize user
         lookup_field = "slug"
         nested_fields = ["components", "packages"]
         ordering = ["slug"]
         owner_field = "creator"
-        owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "friendly_name": "sib:friendlyName",
-            "short_description": "sib:shortDescription",
-            "creator": "foaf:user",
-        }
+        owner_perms = ["view", "add", "change", "delete"]
+        # rdf_context = {
+        #     "friendly_name": "sib:friendlyName",
+        #     "short_description": "sib:shortDescription",
+        #     "creator": "foaf:user",
+        # }
         rdf_type = "sib:application"
         serializer_fields = [
             "@id",
             "repository",
             "friendly_name",
             "short_description",
             "creator",
@@ -70,18 +71,19 @@
             "client_url",
             "application_title",
             "application_logo",
             "components",
             "packages",
             "graphics",
             "services",
+            "npms",
             "federation",
             "deployments",
         ]
-        superuser_perms = ["view"]
+        superuser_perms = ["view", "add", "change", "delete"]
         verbose_name = _("application")
         verbose_name_plural = _("applications")
 
 
 STATUS_CHOICES = [
     ("Todo", _("Todo")),
     ("Doing", _("Doing")),
@@ -116,36 +118,39 @@
             return "{} - {} ({})".format(
                 self.date, self.application.friendly_name, self.application.urlid
             )
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        anonymous_perms = ["view"]
-        authenticated_perms = ["inherit", "add"]
+        anonymous_perms = []
+        authenticated_perms = [
+            "view",
+            "add",
+        ]  # workaround "view" permission, otherwise creator see other requester with only a "add" permission
         container_path = "/deployments/"
         depth = 0
         auto_author = "requester"
         owner_field = "requester"
-        owner_perms = ["inherit", "change", "delete"]
+        owner_perms = ["view", "add", "change", "delete"]
         ordering = ["application__urlid", "date"]
-        rdf_context = {
-            "application": "sib:application",
-            "date": "sib:deploymentDate",
-            "resolutionDate": "sib:deploymentDate",
-            "status": "sib:deploymentStatus",
-        }
+        # rdf_context = {
+        #     "application": "sib:application",
+        #     "date": "sib:deploymentDate",
+        #     "resolutionDate": "sib:deploymentDate",
+        #     "status": "sib:deploymentStatus",
+        # }
         rdf_type = "sib:federation"
         serializer_fields = [
             "@id",
             "date",
             "resolutionDate",
             "status",
         ]
-        superuser_perms = ["view"]
+        superuser_perms = ["view", "add", "change", "delete"]
         verbose_name = _("deployment")
         verbose_name_plural = _("deployments")
 
 
 class Federation(Model):
     application = models.ForeignKey(
         Application,
@@ -165,32 +170,32 @@
     def __str__(self):
         try:
             return "{} ({})".format(self.friendly_name, self.urlid)
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        anonymous_perms = ["view"]
-        authenticated_perms = ["inherit", "add"]
+        anonymous_perms = []
+        authenticated_perms = ["add"]
         container_path = "/federations/"
         depth = 0
         # nested_fields = []
         ordering = ["application__urlid", "target__urlid"]
         owner_field = "application__creator"
-        owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "application": "sib:application",
-            "target": "sib:application",
-        }
+        owner_perms = ["view", "add", "change", "delete"]
+        # rdf_context = {
+        #     "application": "sib:application",
+        #     "target": "sib:application",
+        # }
         rdf_type = "sib:federation"
         serializer_fields = [
             "@id",
             "target",
         ]
-        superuser_perms = ["view"]
+        superuser_perms = ["view", "add", "change", "delete"]
         verbose_name = _("federation")
         verbose_name_plural = _("federations")
 
 
 class ApplicationGraphics(Model):
     application = models.ForeignKey(
         Application,
@@ -208,28 +213,28 @@
             return "{} + {}.{} ({})".format(
                 self.application.friendly_name, self.primary_key, self.key, self.urlid
             )
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        anonymous_perms = ["view"]
-        authenticated_perms = ["inherit"]
+        anonymous_perms = []
+        authenticated_perms = ["add"]
         container_path = "application-graphics/"
         owner_field = "application__creator"
-        owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "application": "sib:application",
-            "primary_key": "sib:key",
-            "key": "sib:key",
-            "value": "sib:value",
-        }
+        owner_perms = ["view", "add", "change", "delete"]
+        # rdf_context = {
+        #     "application": "sib:application",
+        #     "primary_key": "sib:key",
+        #     "key": "sib:key",
+        #     "value": "sib:value",
+        # }
         rdf_type = "sib:graphic"
         serializer_fields = ["@id", "primary_key", "key", "value"]
-        superuser_perms = ["inherit"]
+        superuser_perms = ["view", "add", "change", "delete"]
         verbose_name = _("application graphic")
         verbose_name_plural = _("application graphics")
 
 
 class ApplicationService(Model):
     application = models.ForeignKey(
         Application,
@@ -247,28 +252,28 @@
             return "{} + {}.{} ({})".format(
                 self.application.friendly_name, self.primary_key, self.key, self.urlid
             )
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        anonymous_perms = ["view"]
-        authenticated_perms = ["inherit"]
+        anonymous_perms = []
+        authenticated_perms = ["add"]
         container_path = "application-services/"
         owner_field = "application__creator"
-        owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "application": "sib:application",
-            "primary_key": "sib:key",
-            "key": "sib:key",
-            "value": "sib:value",
-        }
+        owner_perms = ["view", "add", "change", "delete"]
+        # rdf_context = {
+        #     "application": "sib:application",
+        #     "primary_key": "sib:key",
+        #     "key": "sib:key",
+        #     "value": "sib:value",
+        # }
         rdf_type = "sib:service"
         serializer_fields = ["@id", "primary_key", "key", "value"]
-        superuser_perms = ["inherit"]
+        superuser_perms = ["view", "add", "change", "delete"]
         verbose_name = _("application service")
         verbose_name_plural = _("application services")
 
 
 class ApplicationNPM(Model):
     application = models.ForeignKey(
         Application,
@@ -285,27 +290,27 @@
             return "{} + {}@{} ({})".format(
                 self.application.friendly_name, self.package, self.version, self.urlid
             )
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        anonymous_perms = ["view"]
-        authenticated_perms = ["inherit"]
+        anonymous_perms = []
+        authenticated_perms = ["add"]
         container_path = "application-npms/"
         owner_field = "application__creator"
-        owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "application": "sib:application",
-            "package": "sib:npmpackage",
-            "version": "sib:npmversion",
-        }
+        owner_perms = ["view", "add", "change", "delete"]
+        # rdf_context = {
+        #     "application": "sib:application",
+        #     "package": "sib:npmpackage",
+        #     "version": "sib:npmversion",
+        # }
         rdf_type = "sib:npm"
         serializer_fields = ["@id", "package", "version"]
-        superuser_perms = ["inherit"]
+        superuser_perms = ["view", "add", "change", "delete"]
         verbose_name = _("application npm")
         verbose_name_plural = _("application npms")
 
 
 class ApplicationComponent(Model):
     application = models.ForeignKey(
         Application,
@@ -327,27 +332,27 @@
             return "{} + {} ({})".format(
                 self.application.friendly_name, self.component.friendly_name, self.urlid
             )
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        anonymous_perms = ["view"]
-        authenticated_perms = ["inherit"]
+        anonymous_perms = []
+        authenticated_perms = ["add"]
         container_path = "application-components/"
         nested_fields = ["component", "parameters"]
         owner_field = "application__creator"
-        owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "application": "sib:application",
-            "component": "sib:component",
-        }
+        owner_perms = ["view", "add", "change", "delete"]
+        # rdf_context = {
+        #     "application": "sib:application",
+        #     "component": "sib:component",
+        # }
         rdf_type = "sib:dependency"
-        serializer_fields = ["@id", "component", "parameters"]
-        superuser_perms = ["inherit"]
+        serializer_fields = ["@id", "application", "component", "parameters"]
+        superuser_perms = ["view", "add", "change", "delete"]
         verbose_name = _("application component")
         verbose_name_plural = _("application components")
 
     def save(self, *args, **kwargs):
         if (
             not self.pk
             and ApplicationComponent.objects.filter(
@@ -377,27 +382,27 @@
                 self.component.component.friendly_name,
                 self.urlid,
             )
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        anonymous_perms = ["view"]
-        authenticated_perms = ["inherit"]
+        anonymous_perms = []
+        authenticated_perms = ["add"]
         container_path = "application-component-parameters/"
         owner_field = "component__application__creator"
-        owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "component": "sib:dependency",
-            "key": "sib:key",
-            "value": "sib:value",
-        }
+        owner_perms = ["view", "add", "change", "delete"]
+        # rdf_context = {
+        #     "component": "sib:dependency",
+        #     "key": "sib:key",
+        #     "value": "sib:value",
+        # }
         rdf_type = "sib:parameter"
         serializer_fields = ["@id", "key", "value"]
-        superuser_perms = ["inherit"]
+        superuser_perms = ["view", "add", "change", "delete"]
         verbose_name = _("component parameter")
         verbose_name_plural = _("component parameters")
 
 
 class ApplicationPackage(Model):
     application = models.ForeignKey(
         Application,
@@ -419,27 +424,27 @@
             return "{} + {} ({})".format(
                 self.application.friendly_name, self.package.friendly_name, self.urlid
             )
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        anonymous_perms = ["view"]
-        authenticated_perms = ["inherit"]
+        anonymous_perms = []
+        authenticated_perms = ["add"]
         container_path = "application-packages/"
         nested_fields = ["package", "parameters"]
         owner_field = "application__creator"
-        owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "application": "sib:application",
-            "package": "sib:package",
-        }
+        owner_perms = ["view", "add", "change", "delete"]
+        # rdf_context = {
+        #     "application": "sib:application",
+        #     "package": "sib:package",
+        # }
         rdf_type = "sib:dependency"
-        serializer_fields = ["@id", "package", "parameters"]
-        superuser_perms = ["inherit"]
+        serializer_fields = ["@id", "application", "package", "parameters"]
+        superuser_perms = ["view", "add", "change", "delete"]
         verbose_name = _("application package")
         verbose_name_plural = _("application packages")
 
     def save(self, *args, **kwargs):
         if (
             not self.pk
             and ApplicationPackage.objects.filter(
@@ -469,27 +474,27 @@
                 self.package.package.friendly_name,
                 self.urlid,
             )
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        anonymous_perms = ["view"]
-        authenticated_perms = ["inherit"]
+        anonymous_perms = []
+        authenticated_perms = ["add"]
         container_path = "application-package-parameters/"
         owner_field = "package__application__creator"
-        owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "package": "sib:dependency",
-            "key": "sib:key",
-            "value": "sib:value",
-        }
+        owner_perms = ["view", "add", "change", "delete"]
+        # rdf_context = {
+        #     "package": "sib:dependency",
+        #     "key": "sib:key",
+        #     "value": "sib:value",
+        # }
         rdf_type = "sib:parameter"
         serializer_fields = ["@id", "key", "value"]
-        superuser_perms = ["inherit"]
+        superuser_perms = ["view", "add", "change", "delete"]
         verbose_name = _("package parameter")
         verbose_name_plural = _("package parameters")
 
 
 class ComponentExtension(Model):
     base_component = models.ForeignKey(
         ApplicationComponent,
@@ -513,27 +518,27 @@
                 self.component.friendly_name,
                 self.urlid,
             )
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        anonymous_perms = ["view"]
-        authenticated_perms = ["inherit"]
+        anonymous_perms = []
+        authenticated_perms = ["add"]
         container_path = "component-extensions/"
         nested_fields = ["component", "base_component"]
         owner_field = "base_component__application__creator"
-        owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "base_component": "sib:dependency",
-            "component": "sib:component",
-        }
+        owner_perms = ["view", "add", "change", "delete"]
+        # rdf_context = {
+        #     "base_component": "sib:dependency",
+        #     "component": "sib:component",
+        # }
         rdf_type = "sib:dependency"
         serializer_fields = ["@id", "component"]
-        superuser_perms = ["inherit"]
+        superuser_perms = ["view", "add", "change", "delete"]
         verbose_name = _("component extension")
         verbose_name_plural = _("component extensions")
 
     def save(self, *args, **kwargs):
         if (
             not self.pk
             and ComponentExtension.objects.filter(
@@ -563,27 +568,27 @@
                 self.component.component.friendly_name,
                 self.urlid,
             )
         except:
             return self.urlid
 
     class Meta(Model.Meta):
-        anonymous_perms = ["view"]
-        authenticated_perms = ["inherit"]
+        anonymous_perms = []
+        authenticated_perms = ["add"]
         container_path = "component-extension-parameters/"
         owner_field = "component__base_component__application__creator"
-        owner_perms = ["inherit", "change", "delete"]
-        rdf_context = {
-            "component": "sib:dependency",
-            "key": "sib:key",
-            "value": "sib:value",
-        }
+        owner_perms = ["view", "add", "change", "delete"]
+        # rdf_context = {
+        #     "component": "sib:dependency",
+        #     "key": "sib:key",
+        #     "value": "sib:value",
+        # }
         rdf_type = "sib:parameter"
         serializer_fields = ["@id", "key", "value"]
-        superuser_perms = ["inherit"]
+        superuser_perms = ["view", "add", "change", "delete"]
         verbose_name = _("component extension parameter")
         verbose_name_plural = _("component extension parameters")
 
 
 @receiver(pre_save, sender=Application)
 def pre_save_slugify(sender, instance, **kwargs):
     if not instance.urlid or instance.urlid.startswith(settings.SITE_URL):
```

### Comparing `djangoldp_application-1.1.9/djangoldp_application/admin.py` & `djangoldp_application-2.0.0/djangoldp_application/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from django import forms
 from django.contrib import admin
 from django.core.exceptions import ValidationError
 from djangoldp.admin import DjangoLDPAdmin
+
 from .models import (
     Application,
-    Federation,
-    ApplicationService,
-    ApplicationNPM,
-    ApplicationGraphics,
     ApplicationComponent,
-    ApplicationPackage,
     ApplicationComponentParameter,
+    ApplicationGraphics,
+    ApplicationNPM,
+    ApplicationPackage,
     ApplicationPackageParameter,
+    ApplicationService,
     ComponentExtension,
     ComponentExtensionParameter,
     Deployment,
+    Federation,
 )
 
 
+@admin.register(ApplicationComponentParameter, ApplicationGraphics, ApplicationNPM, ApplicationPackageParameter, ApplicationService, ComponentExtensionParameter, Federation)
 class EmptyAdmin(admin.ModelAdmin):
     def get_model_perms(self, request):
         return {}
 
 
 class ApplicationComponentInline(admin.TabularInline):
     model = ApplicationComponent
@@ -63,17 +65,23 @@
 class FederationInline(admin.TabularInline):
     model = Federation
     fk_name = "application"
     exclude = ("urlid", "is_backlink", "allow_create_backlink")
     extra = 0
 
 
+@admin.register(Application)
 class ApplicationAdmin(DjangoLDPAdmin):
     list_display = ("urlid", "friendly_name", "short_description")
-    exclude = ("urlid", "slug", "is_backlink", "allow_create_backlink")
+    exclude = (
+        "urlid",
+        "slug",
+        "is_backlink",
+        "allow_create_backlink",
+    )
     inlines = [
         ApplicationGraphicsInline,
         ApplicationServiceInline,
         ApplicationNPMInline,
         ApplicationComponentInline,
         ApplicationPackageInline,
         FederationInline,
@@ -84,14 +92,15 @@
 
 class ApplicationPackageParameterInline(admin.TabularInline):
     model = ApplicationPackageParameter
     exclude = ("urlid", "is_backlink", "allow_create_backlink")
     extra = 0
 
 
+@admin.register(ApplicationPackage)
 class ApplicationPackageAdmin(DjangoLDPAdmin):
     list_display = ("urlid", "application", "package")
     exclude = ("urlid", "slug", "is_backlink", "allow_create_backlink")
     inlines = [ApplicationPackageParameterInline]
     search_fields = [
         "urlid",
         "package__friendly_name",
@@ -104,14 +113,15 @@
 
 class ApplicationComponentParameterInline(admin.TabularInline):
     model = ApplicationComponentParameter
     exclude = ("urlid", "is_backlink", "allow_create_backlink")
     extra = 0
 
 
+@admin.register(ApplicationComponent)
 class ApplicationComponentAdmin(DjangoLDPAdmin):
     list_display = ("urlid", "application", "component")
     exclude = ("urlid", "slug", "is_backlink", "allow_create_backlink")
     inlines = [ApplicationComponentParameterInline]
     search_fields = [
         "urlid",
         "component__friendly_name",
@@ -124,14 +134,15 @@
 
 class ComponentExtensionParameterInline(admin.TabularInline):
     model = ComponentExtensionParameter
     exclude = ("urlid", "is_backlink", "allow_create_backlink")
     extra = 0
 
 
+@admin.register(ComponentExtension)
 class ComponentExtensionAdmin(DjangoLDPAdmin):
     list_display = ("urlid", "base_component", "component")
     exclude = ("urlid", "slug", "is_backlink", "allow_create_backlink")
     inlines = [ComponentExtensionParameterInline]
     search_fields = [
         "urlid",
         "component__friendly_name",
@@ -140,26 +151,20 @@
         "base_component__component__short_description",
         "base_component__application__friendly_name",
         "base_component__application__short_description",
     ]
     ordering = ["base_component__application__slug", "component__slug"]
 
 
+@admin.register(Deployment)
 class DeploymentAdmin(DjangoLDPAdmin):
     list_display = ("application", "requester", "date", "status", "resolutionDate")
     exclude = ("urlid", "slug", "is_backlink", "allow_create_backlink")
-    search_fields = ["urlid", "application__slug", "requester__name", "application__friendly_name"]
+    search_fields = [
+        "urlid",
+        "application__slug",
+        "requester__name",
+        "application__friendly_name",
+    ]
     ordering = ["application__slug", "date", "resolutionDate"]
 
 
-admin.site.register(Application, ApplicationAdmin)
-admin.site.register(Federation, EmptyAdmin)
-admin.site.register(ApplicationGraphics, EmptyAdmin)
-admin.site.register(ApplicationService, EmptyAdmin)
-admin.site.register(ApplicationNPM, EmptyAdmin)
-admin.site.register(ApplicationComponent, ApplicationComponentAdmin)
-admin.site.register(ApplicationPackage, ApplicationPackageAdmin)
-admin.site.register(ApplicationComponentParameter, EmptyAdmin)
-admin.site.register(ApplicationPackageParameter, EmptyAdmin)
-admin.site.register(ComponentExtension, ComponentExtensionAdmin)
-admin.site.register(ComponentExtensionParameter, EmptyAdmin)
-admin.site.register(Deployment, DeploymentAdmin)
```

### Comparing `djangoldp_application-1.1.9/djangoldp_application/djangoldp_urls.py` & `djangoldp_application-2.0.0/djangoldp_application/djangoldp_urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from django.urls import path
+
 from .views import (
-    ApplicationViewSet,
     ApplicationDetailViewSet,
+    ApplicationViewSet,
+    CreateApplicationViewSet,
     mark_as_doing,
     mark_as_done,
     mark_as_failed,
 )
 
 urlpatterns = [
     path(
+        "create-application/",
+        CreateApplicationViewSet.as_view({"get": "list", "post": "create"}),
+        name="create_application",
+    ),
+    path(
         "ansible/inventory/",
         ApplicationViewSet.as_view({"get": "list"}),
         name="ansible_inventory",
     ),
     path(
         "ansible/<slug:slug>/",
         ApplicationDetailViewSet.as_view({"get": "retrieve"}, lookup_field="slug"),
```

### Comparing `djangoldp_application-1.1.9/djangoldp_application/migrations/0009_applicationgraphics.py` & `djangoldp_application-2.0.0/djangoldp_application/migrations/0009_applicationgraphics.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/djangoldp_application/migrations/0014_auto_20230512_1613.py` & `djangoldp_application-2.0.0/djangoldp_application/migrations/0014_auto_20230512_1613.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/djangoldp_application/migrations/0001_initial.py` & `djangoldp_application-2.0.0/djangoldp_application/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/djangoldp_application/migrations/0011_auto_20230512_1555.py` & `djangoldp_application-2.0.0/djangoldp_application/migrations/0011_auto_20230512_1555.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/djangoldp_application/migrations/0010_auto_20230331_0921.py` & `djangoldp_application-2.0.0/djangoldp_application/migrations/0010_auto_20230331_0921.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/djangoldp_application/migrations/0013_auto_20230512_1608.py` & `djangoldp_application-2.0.0/djangoldp_application/migrations/0013_auto_20230512_1608.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/djangoldp_application/migrations/0012_auto_20230512_1556.py` & `djangoldp_application-2.0.0/djangoldp_application/migrations/0012_auto_20230512_1556.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/djangoldp_application/migrations/0005_auto_20230331_0850.py` & `djangoldp_application-2.0.0/djangoldp_application/migrations/0005_auto_20230331_0850.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/djangoldp_application/migrations/0008_applicationnpm.py` & `djangoldp_application-2.0.0/djangoldp_application/migrations/0008_applicationnpm.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/djangoldp_application/migrations/0004_auto_20230328_1657.py` & `djangoldp_application-2.0.0/djangoldp_application/migrations/0004_auto_20230328_1657.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/djangoldp_application/migrations/0002_deployment.py` & `djangoldp_application-2.0.0/djangoldp_application/migrations/0002_deployment.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.1.9/djangoldp_application/migrations/0006_applicationservice.py` & `djangoldp_application-2.0.0/djangoldp_application/migrations/0006_applicationservice.py`

 * *Files identical despite different names*

