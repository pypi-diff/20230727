# Comparing `tmp/cubicweb-preview-1.5.0.tar.gz` & `tmp/cubicweb-preview-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-preview-1.5.0.tar", last modified: Tue Oct 15 16:25:34 2019, max compression
+gzip compressed data, was "cubicweb-preview-2.0.0.tar", last modified: Thu Jul 27 12:52:16 2023, max compression
```

## Comparing `cubicweb-preview-1.5.0.tar` & `cubicweb-preview-2.0.0.tar`

### file list

```diff
@@ -1,43 +1,51 @@
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      306 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/MANIFEST.in
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     2624 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/setup.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview.egg-info/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       45 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview.egg-info/entry_points.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       17 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview.egg-info/top_level.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview.egg-info/not-zip-safe
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     1014 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview.egg-info/SOURCES.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       26 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview.egg-info/requires.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)        1 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview.egg-info/dependency_links.txt
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     4083 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview.egg-info/PKG-INFO
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       38 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/setup.cfg
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     3000 2019-03-14 14:19:43.000000 cubicweb-preview-1.5.0/README
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     4083 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/PKG-INFO
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1816 2019-03-14 14:19:43.000000 cubicweb-preview-1.5.0/cubicweb_preview/hooks.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      681 2019-10-15 16:24:46.000000 cubicweb-preview-1.5.0/cubicweb_preview/__pkginfo__.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview/i18n/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      493 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/cubicweb_preview/i18n/fr.po
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      391 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/cubicweb_preview/i18n/es.po
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      480 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/cubicweb_preview/i18n/en.po
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview/entities/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1948 2019-01-29 10:23:32.000000 cubicweb-preview-1.5.0/cubicweb_preview/entities/adapters.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       19 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/cubicweb_preview/entities/__init__.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)       49 2019-01-29 10:23:32.000000 cubicweb-preview-1.5.0/cubicweb_preview/uiprops.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview/wdoc/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      136 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/cubicweb_preview/wdoc/ChangeLog_en
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     2839 2019-03-14 14:19:43.000000 cubicweb-preview-1.5.0/cubicweb_preview/wdoc/preview_en.rst
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      206 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/cubicweb_preview/wdoc/toc.xml
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)      125 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/cubicweb_preview/wdoc/todo_en.rst
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1087 2019-01-29 10:23:32.000000 cubicweb-preview-1.5.0/cubicweb_preview/site_cubicweb.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      821 2019-01-29 10:23:32.000000 cubicweb-preview-1.5.0/cubicweb_preview/utils.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview/views/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1984 2019-01-29 10:23:32.000000 cubicweb-preview-1.5.0/cubicweb_preview/views/forms.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     1435 2019-01-29 10:23:32.000000 cubicweb-preview-1.5.0/cubicweb_preview/views/templates.py
--rw-------   0 ppepiot   (1000) ppepiot   (1000)     6794 2019-03-14 14:19:43.000000 cubicweb-preview-1.5.0/cubicweb_preview/views/controllers.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       16 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/cubicweb_preview/views/__init__.py
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)       80 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/cubicweb_preview/__init__.py
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/cubicweb_preview/data/
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     3382 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/cubicweb_preview/data/preview.png
--rw-r--r--   0 ppepiot   (1000) ppepiot   (1000)     1145 2019-01-29 10:22:18.000000 cubicweb-preview-1.5.0/cubicweb_preview/data/cubes.preview.js
-drwxr-xr-x   0 ppepiot   (1000) ppepiot   (1000)        0 2019-10-15 16:25:34.000000 cubicweb-preview-1.5.0/test/
--rw-------   0 ppepiot   (1000) ppepiot   (1000)      454 2019-03-14 14:19:43.000000 cubicweb-preview-1.5.0/test/test_preview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:16.587199 cubicweb-preview-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-07-27 12:52:16.587199 cubicweb-preview-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3000 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:16.563198 cubicweb-preview-2.0.0/cubicweb_preview/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:16.571199 cubicweb-preview-2.0.0/cubicweb_preview/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/data/cubes.preview.js
+-rw-rw-rw-   0 root         (0) root         (0)     3382 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/data/preview.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:16.571199 cubicweb-preview-2.0.0/cubicweb_preview/entities/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/entities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1915 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/entities/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:16.575199 cubicweb-preview-2.0.0/cubicweb_preview/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      493 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/uiprops.py
+-rw-rw-rw-   0 root         (0) root         (0)      821 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:16.579199 cubicweb-preview-2.0.0/cubicweb_preview/views/
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6835 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/views/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/views/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/views/templates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:16.579199 cubicweb-preview-2.0.0/cubicweb_preview/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/wdoc/ChangeLog_en
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/wdoc/preview_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/wdoc/toc.xml
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/cubicweb_preview/wdoc/todo_en.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:16.567199 cubicweb-preview-2.0.0/cubicweb_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-07-27 12:52:16.000000 cubicweb-preview-2.0.0/cubicweb_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-07-27 12:52:16.000000 cubicweb-preview-2.0.0/cubicweb_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 12:52:16.000000 cubicweb-preview-2.0.0/cubicweb_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-27 12:52:16.000000 cubicweb-preview-2.0.0/cubicweb_preview.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 12:52:16.000000 cubicweb-preview-2.0.0/cubicweb_preview.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 12:52:16.000000 cubicweb-preview-2.0.0/cubicweb_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-27 12:52:16.000000 cubicweb-preview-2.0.0/cubicweb_preview.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 12:52:16.587199 cubicweb-preview-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2614 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:16.583199 cubicweb-preview-2.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 12:52:16.587199 cubicweb-preview-2.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/test/data/schema.py
+-rwxrwxrwx   0 root         (0) root         (0)     3424 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/test/data/small.png
+-rw-rw-rw-   0 root         (0) root         (0)      399 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/test/data/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/test/test_preview.py
+-rw-rw-rw-   0 root         (0) root         (0)     8504 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/test/unittest_preview.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-07-27 12:51:37.000000 cubicweb-preview-2.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-preview-1.5.0/setup.py` & `cubicweb-preview-2.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,56 +27,57 @@
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
 
 # load metadata from the __pkginfo__.py file so there is no risk of conflict
 # see https://packaging.python.org/en/latest/single_source_version.html
-pkginfo = join(here, 'cubicweb_preview', '__pkginfo__.py')
+pkginfo = join(here, "cubicweb_preview", "__pkginfo__.py")
 __pkginfo__ = {}
 with open(pkginfo) as f:
     exec(f.read(), __pkginfo__)
 
 # get required metadatas
-distname = __pkginfo__['distname']
-version = __pkginfo__['version']
-license = __pkginfo__['license']
-description = __pkginfo__['description']
-web = __pkginfo__['web']
-author = __pkginfo__['author']
-author_email = __pkginfo__['author_email']
-classifiers = __pkginfo__['classifiers']
+distname = __pkginfo__["distname"]
+version = __pkginfo__["version"]
+license = __pkginfo__["license"]
+description = __pkginfo__["description"]
+web = __pkginfo__["web"]
+author = __pkginfo__["author"]
+author_email = __pkginfo__["author_email"]
+classifiers = __pkginfo__["classifiers"]
 
-with open(join(here, 'README')) as f:
+with open(join(here, "README.rst")) as f:
     long_description = f.read()
 
 # get optional metadatas
-data_files = __pkginfo__.get('data_files', None)
-dependency_links = __pkginfo__.get('dependency_links', ())
+data_files = __pkginfo__.get("data_files", None)
+dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = ["{0} {1}".format(d, v and v or "").strip()
-                    for d, v in requires.items()]
+install_requires = [
+    "{0} {1}".format(d, v and v or "").strip() for d, v in requires.items()
+]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
     long_description=long_description,
     author=author,
     author_email=author_email,
     url=web,
     classifiers=classifiers,
-    packages=find_packages(exclude=['test']),
+    packages=find_packages(exclude=["test"]),
     install_requires=install_requires,
     include_package_data=True,
     entry_points={
-        'cubicweb.cubes': [
-            'preview=cubicweb_preview',
+        "cubicweb.cubes": [
+            "preview=cubicweb_preview",
         ],
     },
     zip_safe=False,
 )
```

### Comparing `cubicweb-preview-1.5.0/cubicweb_preview.egg-info/PKG-INFO` & `cubicweb-preview-2.0.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,78 @@
-Metadata-Version: 1.1
-Name: cubicweb-preview
-Version: 1.5.0
-Summary: Enables adding a preview button in your forms
-Home-page: https://www.cubicweb.org/project/cubicweb-preview
-Author: LOGILAB S.A. (Paris, FRANCE)
-Author-email: contact@logilab.fr
-License: LGPL
-Description: General description
-        ===================
-        
-        Preview cube adds the ability to preview the effect of a form submission.
-        
-        The main idea is:
-        
-        * submit the form data to a special controller, that will
-          insert / update data in the database transaction, as normal
-        
-        * generate the preview
-        
-        * rollback the database changes to leave the database unchanged
-        
-        The only exceptions to this rules are downloadable entities, like images : when
-        an html page (as a preview example view) that contains newly created / updated
-        images is rendered, the actual image content is queried by users' browser a
-        while after the above-mentionned database rollback was performed. The solution
-        adopted in this cube is to save such contents on the disk, and keep it for some
-        time (that can be set using the preview-time option) so that it can be previewed
-        and clean it up afterwards.
-        
-        Usage
-        =====
-        
-        Simplest usage concerns automatic entity forms, where you generally want to
-        preview the just created or updated entity : in this case, import
-        PreviewFormMixin from cubicweb_preview.utils and make your form inherit it :
-        you're done. For example, to apply it to all AutomaticEntityForm forms, use::
-        
-         from cubicweb.selectors import yes
-         from cubicweb.web.views.autoform import AutomaticEntityForm
-         from cubicweb_preview.views.forms import PreviewFormMixin
-        
-         class PreviewAutomaticEntityForm(PreviewFormMixin, AutomaticEntityForm):
-             __select__ = AutomaticEntityForm.__select__ & yes()
-        
-        You can of course customize the preview, using PreviewFormMixin preview_vid
-        and preview_rql attributes, that will be used by the controller to create a
-        result set (using preview_rql, if not None) and apply a view (which name is
-        preview_vid value, default to "index") to it.
-        
-        Below is an example for a CubicWeb instance using the file and preview cubes,
-        that can be used to preview the list of all images when you add or edit one :
-        we request all images through the preview_rql setting and display them using
-        the primary view ::
-        
-          from cubicweb.selectors import is_instance
-          from cubicweb.web.views.autoform import AutomaticEntityForm
-          from cubicweb_preview.views.forms import PreviewFormMixin
-        
-          class ImageForm(PreviewFormMixin, AutomaticEntityForm):
-             __select__ = AutomaticEntityForm.__select__ & is_instance('Image')
-             preview_vid = 'primary'
-             preview_rql = 'Any X WHERE X is Image'
-             preview_mode = 'inline'
-        
-        Note that the previously created images are stored in the database while the
-        previewed one is temporarily stored on disk. By default, the previewed image
-        will be kept for one hour on disk, which can be set using the preview-store-time
-        option.
-        
-        The `preview_mode` attribute accepts `newtab` (the default, opening
-        the preview in a new browser windows/tab within a custom template), or
-        `inline` (will show the preview below the form).
-        
-        
-        
-        Authors
-        =======
-        
-        This cube has been written by SecondWeb S.A.S. and is now maintained
-        and developped by Logilab S.A.
-        
-        License
-        =======
-        
-        This cube is distributed under the LGPL-2 license.
-        
-Platform: UNKNOWN
-Classifier: Environment :: Web Environment
-Classifier: Framework :: CubicWeb
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: JavaScript
+General description
+===================
+
+Preview cube adds the ability to preview the effect of a form submission.
+
+The main idea is:
+
+* submit the form data to a special controller, that will
+  insert / update data in the database transaction, as normal
+
+* generate the preview
+
+* rollback the database changes to leave the database unchanged
+
+The only exceptions to this rules are downloadable entities, like images : when
+an html page (as a preview example view) that contains newly created / updated
+images is rendered, the actual image content is queried by users' browser a
+while after the above-mentionned database rollback was performed. The solution
+adopted in this cube is to save such contents on the disk, and keep it for some
+time (that can be set using the preview-time option) so that it can be previewed
+and clean it up afterwards.
+
+Usage
+=====
+
+Simplest usage concerns automatic entity forms, where you generally want to
+preview the just created or updated entity : in this case, import
+PreviewFormMixin from cubicweb_preview.utils and make your form inherit it :
+you're done. For example, to apply it to all AutomaticEntityForm forms, use::
+
+ from cubicweb.selectors import yes
+ from cubicweb_web.views.autoform import AutomaticEntityForm
+ from cubicweb_preview.views.forms import PreviewFormMixin
+
+ class PreviewAutomaticEntityForm(PreviewFormMixin, AutomaticEntityForm):
+     __select__ = AutomaticEntityForm.__select__ & yes()
+
+You can of course customize the preview, using PreviewFormMixin preview_vid
+and preview_rql attributes, that will be used by the controller to create a
+result set (using preview_rql, if not None) and apply a view (which name is
+preview_vid value, default to "index") to it.
+
+Below is an example for a CubicWeb instance using the file and preview cubes,
+that can be used to preview the list of all images when you add or edit one :
+we request all images through the preview_rql setting and display them using
+the primary view ::
+
+  from cubicweb.selectors import is_instance
+  from cubicweb_web.views.autoform import AutomaticEntityForm
+  from cubicweb_preview.views.forms import PreviewFormMixin
+
+  class ImageForm(PreviewFormMixin, AutomaticEntityForm):
+     __select__ = AutomaticEntityForm.__select__ & is_instance('Image')
+     preview_vid = 'primary'
+     preview_rql = 'Any X WHERE X is Image'
+     preview_mode = 'inline'
+
+Note that the previously created images are stored in the database while the
+previewed one is temporarily stored on disk. By default, the previewed image
+will be kept for one hour on disk, which can be set using the preview-store-time
+option.
+
+The `preview_mode` attribute accepts `newtab` (the default, opening
+the preview in a new browser windows/tab within a custom template), or
+`inline` (will show the preview below the form).
+
+
+
+Authors
+=======
+
+This cube has been written by SecondWeb S.A.S. and is now maintained
+and developped by Logilab S.A.
+
+License
+=======
+
+This cube is distributed under the LGPL-2 license.
```

### Comparing `cubicweb-preview-1.5.0/README` & `cubicweb-preview-2.0.0/cubicweb_preview/wdoc/preview_en.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+===================
 General description
 ===================
 
 Preview cube adds the ability to preview the effect of a form submission.
 
-The main idea is:
+The main idea is :
 
 * submit the form data to a special controller, that will
   insert / update data in the database transaction, as normal
 
 * generate the preview
 
 * rollback the database changes to leave the database unchanged
@@ -16,24 +17,25 @@
 an html page (as a preview example view) that contains newly created / updated
 images is rendered, the actual image content is queried by users' browser a
 while after the above-mentionned database rollback was performed. The solution
 adopted in this cube is to save such contents on the disk, and keep it for some
 time (that can be set using the preview-time option) so that it can be previewed
 and clean it up afterwards.
 
+=====
 Usage
 =====
 
 Simplest usage concerns automatic entity forms, where you generally want to
 preview the just created or updated entity : in this case, import
 PreviewFormMixin from cubicweb_preview.utils and make your form inherit it :
 you're done. For example, to apply it to all AutomaticEntityForm forms, use::
 
  from cubicweb.selectors import yes
- from cubicweb.web.views.autoform import AutomaticEntityForm
+ from cubicweb_web.views.autoform import AutomaticEntityForm
  from cubicweb_preview.views.forms import PreviewFormMixin
 
  class PreviewAutomaticEntityForm(PreviewFormMixin, AutomaticEntityForm):
      __select__ = AutomaticEntityForm.__select__ & yes()
 
 You can of course customize the preview, using PreviewFormMixin preview_vid
 and preview_rql attributes, that will be used by the controller to create a
@@ -42,15 +44,15 @@
 
 Below is an example for a CubicWeb instance using the file and preview cubes,
 that can be used to preview the list of all images when you add or edit one :
 we request all images through the preview_rql setting and display them using
 the primary view ::
 
   from cubicweb.selectors import is_instance
-  from cubicweb.web.views.autoform import AutomaticEntityForm
+  from cubicweb_web.views.autoform import AutomaticEntityForm
   from cubicweb_preview.views.forms import PreviewFormMixin
 
   class ImageForm(PreviewFormMixin, AutomaticEntityForm):
      __select__ = AutomaticEntityForm.__select__ & is_instance('Image')
      preview_vid = 'primary'
      preview_rql = 'Any X WHERE X is Image'
      preview_mode = 'inline'
@@ -60,19 +62,7 @@
 will be kept for one hour on disk, which can be set using the preview-store-time
 option.
 
 The `preview_mode` attribute accepts `newtab` (the default, opening
 the preview in a new browser windows/tab within a custom template), or
 `inline` (will show the preview below the form).
 
-
-
-Authors
-=======
-
-This cube has been written by SecondWeb S.A.S. and is now maintained
-and developped by Logilab S.A.
-
-License
-=======
-
-This cube is distributed under the LGPL-2 license.
```

### Comparing `cubicweb-preview-1.5.0/PKG-INFO` & `cubicweb-preview-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,91 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cubicweb-preview
-Version: 1.5.0
+Version: 2.0.0
 Summary: Enables adding a preview button in your forms
 Home-page: https://www.cubicweb.org/project/cubicweb-preview
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Description: General description
-        ===================
-        
-        Preview cube adds the ability to preview the effect of a form submission.
-        
-        The main idea is:
-        
-        * submit the form data to a special controller, that will
-          insert / update data in the database transaction, as normal
-        
-        * generate the preview
-        
-        * rollback the database changes to leave the database unchanged
-        
-        The only exceptions to this rules are downloadable entities, like images : when
-        an html page (as a preview example view) that contains newly created / updated
-        images is rendered, the actual image content is queried by users' browser a
-        while after the above-mentionned database rollback was performed. The solution
-        adopted in this cube is to save such contents on the disk, and keep it for some
-        time (that can be set using the preview-time option) so that it can be previewed
-        and clean it up afterwards.
-        
-        Usage
-        =====
-        
-        Simplest usage concerns automatic entity forms, where you generally want to
-        preview the just created or updated entity : in this case, import
-        PreviewFormMixin from cubicweb_preview.utils and make your form inherit it :
-        you're done. For example, to apply it to all AutomaticEntityForm forms, use::
-        
-         from cubicweb.selectors import yes
-         from cubicweb.web.views.autoform import AutomaticEntityForm
-         from cubicweb_preview.views.forms import PreviewFormMixin
-        
-         class PreviewAutomaticEntityForm(PreviewFormMixin, AutomaticEntityForm):
-             __select__ = AutomaticEntityForm.__select__ & yes()
-        
-        You can of course customize the preview, using PreviewFormMixin preview_vid
-        and preview_rql attributes, that will be used by the controller to create a
-        result set (using preview_rql, if not None) and apply a view (which name is
-        preview_vid value, default to "index") to it.
-        
-        Below is an example for a CubicWeb instance using the file and preview cubes,
-        that can be used to preview the list of all images when you add or edit one :
-        we request all images through the preview_rql setting and display them using
-        the primary view ::
-        
-          from cubicweb.selectors import is_instance
-          from cubicweb.web.views.autoform import AutomaticEntityForm
-          from cubicweb_preview.views.forms import PreviewFormMixin
-        
-          class ImageForm(PreviewFormMixin, AutomaticEntityForm):
-             __select__ = AutomaticEntityForm.__select__ & is_instance('Image')
-             preview_vid = 'primary'
-             preview_rql = 'Any X WHERE X is Image'
-             preview_mode = 'inline'
-        
-        Note that the previously created images are stored in the database while the
-        previewed one is temporarily stored on disk. By default, the previewed image
-        will be kept for one hour on disk, which can be set using the preview-store-time
-        option.
-        
-        The `preview_mode` attribute accepts `newtab` (the default, opening
-        the preview in a new browser windows/tab within a custom template), or
-        `inline` (will show the preview below the form).
-        
-        
-        
-        Authors
-        =======
-        
-        This cube has been written by SecondWeb S.A.S. and is now maintained
-        and developped by Logilab S.A.
-        
-        License
-        =======
-        
-        This cube is distributed under the LGPL-2 license.
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
+
+General description
+===================
+
+Preview cube adds the ability to preview the effect of a form submission.
+
+The main idea is:
+
+* submit the form data to a special controller, that will
+  insert / update data in the database transaction, as normal
+
+* generate the preview
+
+* rollback the database changes to leave the database unchanged
+
+The only exceptions to this rules are downloadable entities, like images : when
+an html page (as a preview example view) that contains newly created / updated
+images is rendered, the actual image content is queried by users' browser a
+while after the above-mentionned database rollback was performed. The solution
+adopted in this cube is to save such contents on the disk, and keep it for some
+time (that can be set using the preview-time option) so that it can be previewed
+and clean it up afterwards.
+
+Usage
+=====
+
+Simplest usage concerns automatic entity forms, where you generally want to
+preview the just created or updated entity : in this case, import
+PreviewFormMixin from cubicweb_preview.utils and make your form inherit it :
+you're done. For example, to apply it to all AutomaticEntityForm forms, use::
+
+ from cubicweb.selectors import yes
+ from cubicweb_web.views.autoform import AutomaticEntityForm
+ from cubicweb_preview.views.forms import PreviewFormMixin
+
+ class PreviewAutomaticEntityForm(PreviewFormMixin, AutomaticEntityForm):
+     __select__ = AutomaticEntityForm.__select__ & yes()
+
+You can of course customize the preview, using PreviewFormMixin preview_vid
+and preview_rql attributes, that will be used by the controller to create a
+result set (using preview_rql, if not None) and apply a view (which name is
+preview_vid value, default to "index") to it.
+
+Below is an example for a CubicWeb instance using the file and preview cubes,
+that can be used to preview the list of all images when you add or edit one :
+we request all images through the preview_rql setting and display them using
+the primary view ::
+
+  from cubicweb.selectors import is_instance
+  from cubicweb_web.views.autoform import AutomaticEntityForm
+  from cubicweb_preview.views.forms import PreviewFormMixin
+
+  class ImageForm(PreviewFormMixin, AutomaticEntityForm):
+     __select__ = AutomaticEntityForm.__select__ & is_instance('Image')
+     preview_vid = 'primary'
+     preview_rql = 'Any X WHERE X is Image'
+     preview_mode = 'inline'
+
+Note that the previously created images are stored in the database while the
+previewed one is temporarily stored on disk. By default, the previewed image
+will be kept for one hour on disk, which can be set using the preview-store-time
+option.
+
+The `preview_mode` attribute accepts `newtab` (the default, opening
+the preview in a new browser windows/tab within a custom template), or
+`inline` (will show the preview below the form).
+
+
+
+Authors
+=======
+
+This cube has been written by SecondWeb S.A.S. and is now maintained
+and developped by Logilab S.A.
+
+License
+=======
+
+This cube is distributed under the LGPL-2 license.
```

### Comparing `cubicweb-preview-1.5.0/cubicweb_preview/hooks.py` & `cubicweb-preview-2.0.0/cubicweb_preview/hooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,39 +10,43 @@
 
 from cubicweb_preview.utils import preview_dir, preview_dir_cleanup
 
 from cubicweb.server.hook import Hook
 
 
 class PreviewDirCheckHook(Hook):
-    __regid__ = 'preview_dir_check'
-    events = ('server_startup',)
+    __regid__ = "preview_dir_check"
+    events = ("server_startup",)
 
     def __call__(self):
-        if self.repo.config.name != 'all-in-one':
+        if self.repo.config.name != "all-in-one":
             return
         directory = preview_dir(self.repo.config)
         if not os.path.isdir(directory):
             try:
                 os.makedirs(directory)
             except Exception:
-                self.critical('could not find preview directory '
-                              '(check preview-dir option which present value is %r)',
-                              self.config['preview-dir'])
+                self.critical(
+                    "could not find preview directory "
+                    "(check preview-dir option which present value is %r)",
+                    self.config["preview-dir"],
+                )
                 raise
         if not os.access(directory, os.W_OK):
-            raise ValueError('directory %r is not writable '
-                             '(check preview-dir option)' % directory)
+            raise ValueError(
+                "directory %r is not writable " "(check preview-dir option)" % directory
+            )
         # XXX hack to work around 1193301
         pdcfunc = preview_dir_cleanup
 
         def regular_preview_dir_cleanup(config):
             try:
-                self.info('starting preview directory cleanup...')
+                self.info("starting preview directory cleanup...")
                 pdcfunc(config)
             except Exception as ex:
-                self.error('preview directory cleanup error occured : %s', ex)
-        cleanup_time = self.repo.config['preview-dir-cleanup-time']
+                self.error("preview directory cleanup error occured : %s", ex)
+
+        cleanup_time = self.repo.config["preview-dir-cleanup-time"]
         if cleanup_time:
-            self.repo.looping_task(cleanup_time,
-                                   regular_preview_dir_cleanup,
-                                   self.repo.config)
+            self.repo.looping_task(
+                cleanup_time, regular_preview_dir_cleanup, self.repo.config
+            )
```

### Comparing `cubicweb-preview-1.5.0/cubicweb_preview/entities/adapters.py` & `cubicweb-preview-2.0.0/cubicweb_preview/entities/adapters.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,43 +7,46 @@
 """
 import os.path as osp
 from cubicweb.predicates import objectify_predicate
 from cubicweb.entities.adapters import IDownloadableAdapter
 
 
 @objectify_predicate
-def previewable_downloadable_adapter(cls, req, rset=None, row=0, col=0, entity=None,
-                                     do_not_select_me=False, **kwargs):
+def previewable_downloadable_adapter(
+    cls, req, rset=None, row=0, col=0, entity=None, do_not_select_me=False, **kwargs
+):
     if do_not_select_me:
         return 0
     eid = None
     if entity is not None:
         eid = entity.eid
     elif rset:
         eid = rset[row][col]
-    if eid in req.data.get('preview_entities', ()):
+    if hasattr(req, "data") and eid in req.data.get("preview_entities", ()):
         return 999
     return 0
 
 
 class PreviewIDownloadable(IDownloadableAdapter):
     __select__ = previewable_downloadable_adapter()
 
     def __init__(self, *args, **kwargs):
         super(PreviewIDownloadable, self).__init__(*args, **kwargs)
-        adapter = self._cw.vreg['adapters'].select(self.__regid__, self._cw,
-                                                   entity=self.entity, do_not_select_me=True)
-        self.entity._cw_adapters_cache['IDownloadable'] = self
+        adapter = self._cw.vreg["adapters"].select(
+            self.__regid__, self._cw, entity=self.entity, do_not_select_me=True
+        )
+        self.entity._cw_adapters_cache["IDownloadable"] = self
         self._wrapped_adapter = adapter
         self.download_content_type = adapter.download_content_type
         self.download_file_name = adapter.download_file_name
         self.download_data = adapter.download_data
         self.download_encoding = adapter.download_encoding
 
     def download_url(self, **kwargs):
-        prev_ents = self._cw.data.get('preview_entities', {})
+        prev_ents = self._cw.data.get("preview_entities", {})
         eid = int(self.entity.eid)
         if eid in prev_ents:
-            return osp.join(self._cw.vreg.config['preview-urlpath'],
-                            osp.basename(prev_ents[eid]))
+            return osp.join(
+                self._cw.vreg.config["preview-urlpath"], osp.basename(prev_ents[eid])
+            )
         else:
             return self._wrapped_adapter.download_url(**kwargs)
```

### Comparing `cubicweb-preview-1.5.0/cubicweb_preview/wdoc/preview_en.rst` & `cubicweb-preview-2.0.0/cubicweb_preview.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,26 @@
-===================
+Metadata-Version: 2.1
+Name: cubicweb-preview
+Version: 2.0.0
+Summary: Enables adding a preview button in your forms
+Home-page: https://www.cubicweb.org/project/cubicweb-preview
+Author: LOGILAB S.A. (Paris, FRANCE)
+Author-email: contact@logilab.fr
+License: LGPL
+Classifier: Environment :: Web Environment
+Classifier: Framework :: CubicWeb
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: JavaScript
+
 General description
 ===================
 
 Preview cube adds the ability to preview the effect of a form submission.
 
-The main idea is :
+The main idea is:
 
 * submit the form data to a special controller, that will
   insert / update data in the database transaction, as normal
 
 * generate the preview
 
 * rollback the database changes to leave the database unchanged
@@ -17,25 +29,24 @@
 an html page (as a preview example view) that contains newly created / updated
 images is rendered, the actual image content is queried by users' browser a
 while after the above-mentionned database rollback was performed. The solution
 adopted in this cube is to save such contents on the disk, and keep it for some
 time (that can be set using the preview-time option) so that it can be previewed
 and clean it up afterwards.
 
-=====
 Usage
 =====
 
 Simplest usage concerns automatic entity forms, where you generally want to
 preview the just created or updated entity : in this case, import
 PreviewFormMixin from cubicweb_preview.utils and make your form inherit it :
 you're done. For example, to apply it to all AutomaticEntityForm forms, use::
 
  from cubicweb.selectors import yes
- from cubicweb.web.views.autoform import AutomaticEntityForm
+ from cubicweb_web.views.autoform import AutomaticEntityForm
  from cubicweb_preview.views.forms import PreviewFormMixin
 
  class PreviewAutomaticEntityForm(PreviewFormMixin, AutomaticEntityForm):
      __select__ = AutomaticEntityForm.__select__ & yes()
 
 You can of course customize the preview, using PreviewFormMixin preview_vid
 and preview_rql attributes, that will be used by the controller to create a
@@ -44,15 +55,15 @@
 
 Below is an example for a CubicWeb instance using the file and preview cubes,
 that can be used to preview the list of all images when you add or edit one :
 we request all images through the preview_rql setting and display them using
 the primary view ::
 
   from cubicweb.selectors import is_instance
-  from cubicweb.web.views.autoform import AutomaticEntityForm
+  from cubicweb_web.views.autoform import AutomaticEntityForm
   from cubicweb_preview.views.forms import PreviewFormMixin
 
   class ImageForm(PreviewFormMixin, AutomaticEntityForm):
      __select__ = AutomaticEntityForm.__select__ & is_instance('Image')
      preview_vid = 'primary'
      preview_rql = 'Any X WHERE X is Image'
      preview_mode = 'inline'
@@ -62,7 +73,19 @@
 will be kept for one hour on disk, which can be set using the preview-store-time
 option.
 
 The `preview_mode` attribute accepts `newtab` (the default, opening
 the preview in a new browser windows/tab within a custom template), or
 `inline` (will show the preview below the form).
 
+
+
+Authors
+=======
+
+This cube has been written by SecondWeb S.A.S. and is now maintained
+and developped by Logilab S.A.
+
+License
+=======
+
+This cube is distributed under the LGPL-2 license.
```

### Comparing `cubicweb-preview-1.5.0/cubicweb_preview/utils.py` & `cubicweb-preview-2.0.0/cubicweb_preview/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 import os
 import os.path as osp
 from time import time
 
 
 def preview_dir(config):
-    directory = config['preview-dir']
+    directory = config["preview-dir"]
     if not osp.isabs(directory):
         directory = osp.join(config.static_directory, directory)
     return directory
 
 
 def preview_dir_cleanup(config):
-    cleanup_time = config['preview-dir-cleanup-time']
+    cleanup_time = config["preview-dir-cleanup-time"]
     directory = preview_dir(config)
     for fname in os.listdir(directory):
         fullname = osp.join(directory, fname)
         if time() - os.stat(fullname).st_mtime > cleanup_time:
             os.unlink(fullname)
```

### Comparing `cubicweb-preview-1.5.0/cubicweb_preview/views/forms.py` & `cubicweb-preview-2.0.0/cubicweb_preview/views/forms.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,47 +4,52 @@
 :copyright: 2007-2010 SECOND WEB S.A.S. (Paris, FRANCE), license is LGPL v2.
 :contact: http://www.secondweb.fr/ -- mailto:contact@secondweb.fr
 :license: GNU Lesser General Public License, v2.1 - http://www.gnu.org/licenses
 """
 
 from cubicweb import _
 
-from cubicweb.web.formwidgets import Button
+from cubicweb_web.formwidgets import Button
 
 
-PreviewButton = Button((_('button_preview'), 'PREVIEW_ICON'),
-                       attrs={'klass': 'validateButton preview_button btn btn-default'},
-                       onclick=("postForm('__action_preview', 'button_preview', "
-                                "$(this).closest('form').attr('id'))"))
+PreviewButton = Button(
+    (_("button_preview"), "PREVIEW_ICON"),
+    attrs={"klass": "validateButton preview_button btn btn-default"},
+    onclick=(
+        "postForm('__action_preview', 'button_preview', "
+        "$(this).closest('form').attr('id'))"
+    ),
+)
 
 
 class PreviewFormMixin(object):
-    """ mix this with all forms you want to have a preview with """
+    """mix this with all forms you want to have a preview with"""
+
     preview_vid = None
     preview_rql = None
-    preview_mode = 'newtab'  # 'inline'/'newtab'
-    cwtarget = 'eformframe'
+    preview_mode = "newtab"  # 'inline'/'newtab'
+    cwtarget = "eformframe"
 
     def __init__(self, *args, **kwargs):
         super(PreviewFormMixin, self).__init__(*args, **kwargs)
         if PreviewButton not in self.form_buttons:
             # XXX handle reledit ... (we do not want preview button there)
-            fname = self._cw.form.get('fname')
-            if fname != 'reledit_form':
+            fname = self._cw.form.get("fname")
+            if fname != "reledit_form":
                 self.form_buttons = self.form_buttons[:]
                 self.form_buttons.append(PreviewButton)
         if self.preview_vid is not None:
-            self.add_hidden('__preview_vid', self.preview_vid)
+            self.add_hidden("__preview_vid", self.preview_vid)
         if self.preview_rql is not None:
-            self.add_hidden('__preview_rql', self.preview_rql)
-        if self.formtype == 'main':
-            self.add_hidden('__preview_mode', self.preview_mode)
+            self.add_hidden("__preview_rql", self.preview_rql)
+        if self.formtype == "main":
+            self.add_hidden("__preview_mode", self.preview_mode)
 
     def render(self, *args, **kwargs):
-        self._cw.add_js('cubes.preview.js')
+        self._cw.add_js("cubes.preview.js")
         return super(PreviewFormMixin, self).render(*args, **kwargs)
 
 
 def registration_callback(vreg):
-    if 'bootstrap' in vreg.config.cubes():
-        PreviewButton.icon = 'glyphicon glyphicon-search'
+    if "bootstrap" in vreg.config.cubes():
+        PreviewButton.icon = "glyphicon glyphicon-search"
     vreg.register_all(globals().values(), __name__)
```

### Comparing `cubicweb-preview-1.5.0/cubicweb_preview/views/templates.py` & `cubicweb-preview-2.0.0/cubicweb_preview/views/templates.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,41 +5,44 @@
 :contact: http://www.secondweb.fr/ -- mailto:contact@secondweb.fr
 :license: GNU Lesser General Public License, v2.1 - http://www.gnu.org/licenses
 """
 
 from cubicweb import _
 
 from cubicweb.predicates import objectify_predicate
-from cubicweb.web.views.basetemplates import TheMainTemplate
+from cubicweb_web.views.basetemplates import TheMainTemplate
 
 
 @objectify_predicate
 def preview_form(cls, req, rset=None, **kwargs):
-    if req.form.get('__preview_mode') == 'newtab':
+    if req.form.get("__preview_mode") == "newtab":
         return 1
     return 0
 
 
 class PreviewTemplate(TheMainTemplate):
-    """ a very lightweight main template showing only
+    """a very lightweight main template showing only
     the previewed entity, for the 'newtab' mode
     """
+
     __select__ = TheMainTemplate.__select__ & preview_form()
-    preview_msg = _('This is a preview. Do not try to follow links or trigger actions as both may fail.')
+    preview_msg = _(
+        "This is a preview. Do not try to follow links or trigger actions as both may fail."
+    )
 
     def call(self, view):
         self.set_request_content_type()
         self.template_header(self.content_type, view)
-        self._cw.add_js('cubicweb.edition.js')
+        self._cw.add_js("cubicweb.edition.js")
         w = self.w
-        w(u'<div id="pageContent">')
-        w(u'<p>%s</p>' % self._cw._(self.preview_msg))
-        w(u'<div id="contentmain">\n')
+        w('<div id="pageContent">')
+        w("<p>%s</p>" % self._cw._(self.preview_msg))
+        w('<div id="contentmain">\n')
         view.render(w=w)
-        w(u'</div></div>\n')
+        w("</div></div>\n")
         self.template_footer(view)
 
     def template_body_header(self, view=None):
         pass
 
     def template_footer(self, view=None):
         pass
```

### Comparing `cubicweb-preview-1.5.0/cubicweb_preview/views/controllers.py` & `cubicweb-preview-2.0.0/cubicweb_preview/views/controllers.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,79 +5,87 @@
 :contact: http://www.secondweb.fr/ -- mailto:contact@secondweb.fr
 :license: GNU Lesser General Public License, v2.1 - http://www.gnu.org/licenses
 """
 
 from os import path as osp
 from tempfile import NamedTemporaryFile
 
-from six import text_type, string_types
-
 from logilab.common.registry import yes
 
 from cubicweb import NoSelectableObject, ValidationError
 from cubicweb.utils import json
-from cubicweb.web import Redirect
-from cubicweb.web.views.basecontrollers import FormValidatorController, _validation_error
+from cubicweb_web import Redirect
+from cubicweb_web.views.basecontrollers import (
+    FormValidatorController,
+    _validation_error,
+)
 
 from cubicweb_preview.utils import preview_dir
 
 
 class PreviewControllerMixin(object):
-
     def _preview_trampoline(self, domid, stream, preview_mode):
-        self._cw.set_content_type('text/html')
-        jsfunction = 'rePostFormForPreview' if preview_mode == 'newtab' else 'handleInlinePreview'
+        self._cw.set_content_type("text/html")
+        jsfunction = (
+            "rePostFormForPreview"
+            if preview_mode == "newtab"
+            else "handleInlinePreview"
+        )
         stream = stream.decode(self._cw.encoding)
-        return u"""<script type="text/javascript">
+        return """<script type="text/javascript">
 var html = %s;
 window.parent.%s('%s', html);
-</script>""" % (json.dumps(stream).replace('/', r'\/'), jsfunction, domid)
+</script>""" % (
+            json.dumps(stream).replace("/", r"\/"),
+            jsfunction,
+            domid,
+        )
 
 
 class PreviewController(PreviewControllerMixin, FormValidatorController):
     __select__ = FormValidatorController.__select__ & yes()
 
     def _extract_typed_edited_eids(self):
-        eids = self._cw.form.get('eid')
-        if isinstance(eids, string_types):
+        eids = self._cw.form.get("eid")
+        if isinstance(eids, str):
             eids = [eids]
-        eidmap = self._cw.data.get('eidmap', {})
+        eidmap = self._cw.data.get("eidmap", {})
         out = []
         for eid in eids:
             try:
                 out.append(int(eidmap.get(eid, eid)))
             except Exception:
                 continue
         return out
 
     def _validate_form(self):
-        """ commit-less _validate_form """
+        """commit-less _validate_form"""
         # XXX make the version in cw accept an opt. param
         #     to tell it not to commit ?
         req = self._cw
         try:
-            ctrl = req.vreg['controllers'].select('edit', req=req)
+            ctrl = req.vreg["controllers"].select("edit", req=req)
         except NoSelectableObject:
-            return (False, {None: req._('not authorized')}, None)
+            return (False, {None: req._("not authorized")}, None)
         try:
             ctrl.publish(None)
         except ValidationError as ex:
             return (False, _validation_error(req, ex), ctrl._edited_entity)
         except Redirect as ex:
             if ctrl._edited_entity:
                 ctrl._edited_entity.complete()
             return (True, ex.location, ctrl._edited_entity)
         except Exception as ex:
             req.cnx.rollback()
-            req.exception('unexpected error while validating form')
-            return (False, req._(str(ex).decode('utf-8')), ctrl._edited_entity)
-        return (False, '???', None)
+            req.exception("unexpected error while validating form")
+            return (False, req._(str(ex)), ctrl._edited_entity)
+        return (False, "???", None)
 
     def publish(self, rset=None):
-        """ sketch of the control flow for both modes (python & js)
+        """sketch of the control flow for both modes (python & js)
         newtab:
         * preview button clicked
         * postForm (invokes controller)
         * PreviewController.publish
         * if not ok: standard trampoline (handleFormValidationResponse)
         * preview_trampoline -> passes html stream
         * rePostFormForPreview -> stores stream into form, form.target = '_blank'
@@ -89,73 +97,76 @@
         * PreviewController.publish
         * if not ok:  standard trampoline (handleFormValidationResponse)
         * preview_trampoline -> passes html fragment
         * handleInlinePreview: appends html fragment
         """
         form = self._cw.form
         # handle cancel action
-        if '__redirect_path' not in form:
+        if "__redirect_path" not in form:
             eids = self._extract_typed_edited_eids()
             if eids:
-                form['__redirectpath'] = text_type(eids[0])
-        if '__action_preview' in form:
-            form['__action_apply'] = form.pop('__action_preview', 'button_preview')
+                form["__redirectpath"] = str(eids[0])
+        if "__action_preview" in form:
+            form["__action_apply"] = form.pop("__action_preview", "button_preview")
             self._cw.ajax_request = True
             try:
                 status, args, entity = self._validate_form()
-                domid = str(form.get('__domid', 'entityForm'))
+                domid = str(form.get("__domid", "entityForm"))
                 if not status:  # error, do the standard thing
                     return self.response(domid, status, args, entity)
-                preview_mode = form.get('__preview_mode')
-                if preview_mode == 'newtab':
-                    preview_html = form.get('__preview_html')
+                preview_mode = form.get("__preview_mode")
+                if preview_mode == "newtab":
+                    preview_html = form.get("__preview_html")
                     if preview_html:
-                        self._cw.set_content_type('text/html')
+                        self._cw.set_content_type("text/html")
                         self._cw.ajax_request = False
                         return preview_html.encode(self._cw.encoding)
                 stream = self._build_preview_stream(entity, preview_mode)
                 ret = self._preview_trampoline(domid, stream, preview_mode)
                 ret = ret.encode(self._cw.encoding)
                 return ret
             finally:
                 self._cw.cnx.rollback()
         else:
             return super(PreviewController, self).publish(rset)
 
     def _get_local_file(self, idwnl_adapter):
         directory = preview_dir(self._cw.vreg.config)
         ext = osp.splitext(idwnl_adapter.download_file_name())[1]
-        prefix = '%s_%s_' % (self._cw.user.eid, idwnl_adapter.entity.eid)
-        return NamedTemporaryFile(suffix=ext, prefix=prefix, dir=directory,
-                                  delete=False)
+        prefix = "%s_%s_" % (self._cw.user.eid, idwnl_adapter.entity.eid)
+        return NamedTemporaryFile(
+            suffix=ext, prefix=prefix, dir=directory, delete=False
+        )
 
     def _handle_downloadables(self):
         # handle downloadable entities created within hooks
         # XXX we need precommit() for operations, too
         eids = self._extract_typed_edited_eids()
         prev_ents = {}
-        self._cw.data['preview_entities'] = prev_ents
+        self._cw.data["preview_entities"] = prev_ents
         for eid in eids:
             entity = self._cw.entity_from_eid(eid)
-            adapter = entity.cw_adapt_to('IDownloadable')
+            adapter = entity.cw_adapt_to("IDownloadable")
             if adapter:
                 with self._get_local_file(adapter) as f:
-                    self.info('PreviewController: saving file %s', f.name)
+                    self.info("PreviewController: saving file %s", f.name)
                     f.write(adapter.download_data())
                 prev_ents[adapter.entity.eid] = f.name
 
-    def _build_preview_stream(self, entity=None, preview_mode='inline'):
+    def _build_preview_stream(self, entity=None, preview_mode="inline"):
         self._handle_downloadables()
-        rql = self._cw.form.get('__preview_rql')
+        rql = self._cw.form.get("__preview_rql")
         if rql:
             rset = self._cw.execute(rql)
         else:
             rset = entity.as_rset()
-        self._cw.form['vid'] = vid = self._cw.form.get('__preview_vid', 'primary')
-        self.info('previewing rset %s with vid %s', rset, vid)
-        if preview_mode == 'inline':
-            view = self._cw.vreg['views'].select(vid, self._cw, rset=rset)
+        self._cw.form["vid"] = vid = self._cw.form.get("__preview_vid", "primary")
+        self.info("previewing rset %s with vid %s", rset, vid)
+        if preview_mode == "inline":
+            view = self._cw.vreg["views"].select(vid, self._cw, rset=rset)
             # assume to work with HTML/text views only
             return view.render().encode(self._cw.encoding)
         # template: delegate construction to view controller
-        ctrl = self._cw.vreg['controllers'].select('view', req=self._cw, appli=self.appli)
+        ctrl = self._cw.vreg["controllers"].select(
+            "view", req=self._cw, appli=self.appli
+        )
         return ctrl.publish(rset)
```

### Comparing `cubicweb-preview-1.5.0/cubicweb_preview/data/preview.png` & `cubicweb-preview-2.0.0/cubicweb_preview/data/preview.png`

 * *Files identical despite different names*

### Comparing `cubicweb-preview-1.5.0/cubicweb_preview/data/cubes.preview.js` & `cubicweb-preview-2.0.0/cubicweb_preview/data/cubes.preview.js`

 * *Files identical despite different names*

