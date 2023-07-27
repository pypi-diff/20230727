# Comparing `tmp/shz_geo-0.0.3.tar.gz` & `tmp/shz_geo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shz_geo-0.0.3.tar", last modified: Thu Jul 27 16:50:59 2023, max compression
+gzip compressed data, was "shz_geo-0.0.4.tar", last modified: Thu Jul 27 16:52:23 2023, max compression
```

## Comparing `shz_geo-0.0.3.tar` & `shz_geo-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:50:59.548343 shz_geo-0.0.3/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)     1078 2023-07-25 13:56:48.000000 shz_geo-0.0.3/LICENSE
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      301 2023-07-27 16:50:59.539238 shz_geo-0.0.3/PKG-INFO
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-25 13:57:15.000000 shz_geo-0.0.3/README.md
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       38 2023-07-27 16:50:59.548618 shz_geo-0.0.3/setup.cfg
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      537 2023-07-27 16:50:56.000000 shz_geo-0.0.3/setup.py
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:50:59.532132 shz_geo-0.0.3/shz_geo/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       25 2023-07-27 16:47:10.000000 shz_geo-0.0.3/shz_geo/__init__.py
-drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:50:59.537113 shz_geo-0.0.3/shz_geo.egg-info/
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      301 2023-07-27 16:50:59.000000 shz_geo-0.0.3/shz_geo.egg-info/PKG-INFO
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      200 2023-07-27 16:50:59.000000 shz_geo-0.0.3/shz_geo.egg-info/SOURCES.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        1 2023-07-27 16:50:59.000000 shz_geo-0.0.3/shz_geo.egg-info/dependency_links.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       19 2023-07-27 16:50:59.000000 shz_geo-0.0.3/shz_geo.egg-info/requires.txt
--rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        8 2023-07-27 16:50:59.000000 shz_geo-0.0.3/shz_geo.egg-info/top_level.txt
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:52:23.345669 shz_geo-0.0.4/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)     1078 2023-07-25 13:56:48.000000 shz_geo-0.0.4/LICENSE
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      301 2023-07-27 16:52:23.345351 shz_geo-0.0.4/PKG-INFO
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-25 13:57:15.000000 shz_geo-0.0.4/README.md
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       38 2023-07-27 16:52:23.345774 shz_geo-0.0.4/setup.cfg
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      537 2023-07-27 16:52:19.000000 shz_geo-0.0.4/setup.py
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:52:23.342578 shz_geo-0.0.4/shz_geo/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       39 2023-07-27 16:52:15.000000 shz_geo-0.0.4/shz_geo/__init__.py
+drwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        0 2023-07-27 16:52:23.344855 shz_geo-0.0.4/shz_geo.egg-info/
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      301 2023-07-27 16:52:23.000000 shz_geo-0.0.4/shz_geo.egg-info/PKG-INFO
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)      200 2023-07-27 16:52:23.000000 shz_geo-0.0.4/shz_geo.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        1 2023-07-27 16:52:23.000000 shz_geo-0.0.4/shz_geo.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)       19 2023-07-27 16:52:23.000000 shz_geo-0.0.4/shz_geo.egg-info/requires.txt
+-rwxrwxrwx   0 shz-pop   (1000) shz-pop   (1000)        8 2023-07-27 16:52:23.000000 shz_geo-0.0.4/shz_geo.egg-info/top_level.txt
```

### Comparing `shz_geo-0.0.3/LICENSE` & `shz_geo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shz_geo-0.0.3/setup.py` & `shz_geo-0.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 project_name = 'shz_geo'
 
 setup(name=project_name,
-    version='0.0.3',
+    version='0.0.4',
     license='MIT License',
     author='Eliseu Brito',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='eliseubrito776@gmail.com',
     keywords='shz geo shz_geo shzgeo',
     description=u'Personal support tools in the development of geospatial projects',
```

