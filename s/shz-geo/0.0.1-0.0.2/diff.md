# Comparing `tmp/shz_geo-0.0.1.tar.gz` & `tmp/shz_geo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shz_geo-0.0.1.tar", last modified: Thu Jul 27 16:39:08 2023, max compression
+gzip compressed data, was "shz_geo-0.0.2.tar", last modified: Thu Jul 27 16:47:28 2023, max compression
```

## Comparing `shz_geo-0.0.1.tar` & `shz_geo-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:39:08.589950 shz_geo-0.0.1/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)     1078 2023-07-25 13:56:48.000000 shz_geo-0.0.1/LICENSE
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      301 2023-07-27 16:39:08.589691 shz_geo-0.0.1/PKG-INFO
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-25 13:57:15.000000 shz_geo-0.0.1/README.md
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       38 2023-07-27 16:39:08.590053 shz_geo-0.0.1/setup.cfg
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      537 2023-07-27 16:39:06.000000 shz_geo-0.0.1/setup.py
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:39:08.586336 shz_geo-0.0.1/shz_geo/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 15:10:49.000000 shz_geo-0.0.1/shz_geo/__init__.py
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:39:08.589095 shz_geo-0.0.1/shz_geo.egg-info/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      301 2023-07-27 16:39:08.000000 shz_geo-0.0.1/shz_geo.egg-info/PKG-INFO
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      200 2023-07-27 16:39:08.000000 shz_geo-0.0.1/shz_geo.egg-info/SOURCES.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        1 2023-07-27 16:39:08.000000 shz_geo-0.0.1/shz_geo.egg-info/dependency_links.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       19 2023-07-27 16:39:08.000000 shz_geo-0.0.1/shz_geo.egg-info/requires.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        8 2023-07-27 16:39:08.000000 shz_geo-0.0.1/shz_geo.egg-info/top_level.txt
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:47:28.301629 shz_geo-0.0.2/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)     1078 2023-07-25 13:56:48.000000 shz_geo-0.0.2/LICENSE
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      301 2023-07-27 16:47:28.301301 shz_geo-0.0.2/PKG-INFO
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-25 13:57:15.000000 shz_geo-0.0.2/README.md
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       38 2023-07-27 16:47:28.301734 shz_geo-0.0.2/setup.cfg
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      537 2023-07-27 16:47:24.000000 shz_geo-0.0.2/setup.py
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:47:28.297480 shz_geo-0.0.2/shz_geo/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       25 2023-07-27 16:47:10.000000 shz_geo-0.0.2/shz_geo/__init__.py
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:47:28.300538 shz_geo-0.0.2/shz_geo.egg-info/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      301 2023-07-27 16:47:28.000000 shz_geo-0.0.2/shz_geo.egg-info/PKG-INFO
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      200 2023-07-27 16:47:28.000000 shz_geo-0.0.2/shz_geo.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        1 2023-07-27 16:47:28.000000 shz_geo-0.0.2/shz_geo.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       19 2023-07-27 16:47:28.000000 shz_geo-0.0.2/shz_geo.egg-info/requires.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        8 2023-07-27 16:47:28.000000 shz_geo-0.0.2/shz_geo.egg-info/top_level.txt
```

### Comparing `shz_geo-0.0.1/LICENSE` & `shz_geo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shz_geo-0.0.1/setup.py` & `shz_geo-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 project_name = 'shz_geo'
 
 setup(name=project_name,
-    version='0.0.1',
+    version='0.0.2',
     license='MIT License',
     author='Eliseu Brito',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='eliseubrito776@gmail.com',
     keywords='shz geo shz_geo shzgeo',
     description=u'Personal support tools in the development of geospatial projects',
```

