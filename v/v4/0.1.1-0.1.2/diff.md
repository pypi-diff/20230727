# Comparing `tmp/v4-0.1.1.tar.gz` & `tmp/v4-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v4-0.1.1.tar", last modified: Thu Jul 27 01:07:12 2023, max compression
+gzip compressed data, was "v4-0.1.2.tar", last modified: Thu Jul 27 01:19:49 2023, max compression
```

## Comparing `v4-0.1.1.tar` & `v4-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 reeves     (501) staff       (20)        0 2023-07-27 01:07:12.628681 v4-0.1.1/
--rwxrwxrwx   0 reeves     (501) staff       (20)    35148 2014-09-08 17:52:36.000000 v4-0.1.1/LICENSE.txt
--rw-r--r--   0 reeves     (501) staff       (20)      288 2023-07-27 01:07:12.628508 v4-0.1.1/PKG-INFO
--rwxrwxrwx   0 reeves     (501) staff       (20)      838 2018-04-12 20:31:22.000000 v4-0.1.1/README.md
--rw-r--r--   0 reeves     (501) staff       (20)       38 2023-07-27 01:07:12.628731 v4-0.1.1/setup.cfg
--rwxrwxrwx   0 reeves     (501) staff       (20)      384 2023-07-27 01:05:40.000000 v4-0.1.1/setup.py
-drwxr-xr-x   0 reeves     (501) staff       (20)        0 2023-07-27 01:07:12.627583 v4-0.1.1/v4/
--rwxrwxrwx   0 reeves     (501) staff       (20)        2 2017-12-29 23:35:19.000000 v4-0.1.1/v4/__init__.py
--rw-r--r--   0 reeves     (501) staff       (20)    12327 2023-07-27 00:50:11.000000 v4-0.1.1/v4/vd.py
--rwxr-xr-x   0 reeves     (501) staff       (20)    28090 2023-07-27 00:50:03.000000 v4-0.1.1/v4/vx.py
-drwxr-xr-x   0 reeves     (501) staff       (20)        0 2023-07-27 01:07:12.628311 v4-0.1.1/v4.egg-info/
--rwxrwxrwx   0 reeves     (501) staff       (20)      288 2023-07-27 01:07:12.000000 v4-0.1.1/v4.egg-info/PKG-INFO
--rwxrwxrwx   0 reeves     (501) staff       (20)      167 2023-07-27 01:07:12.000000 v4-0.1.1/v4.egg-info/SOURCES.txt
--rwxrwxrwx   0 reeves     (501) staff       (20)        1 2023-07-27 01:07:12.000000 v4-0.1.1/v4.egg-info/dependency_links.txt
--rwxrwxrwx   0 reeves     (501) staff       (20)        3 2023-07-27 01:07:12.000000 v4-0.1.1/v4.egg-info/top_level.txt
+drwxr-xr-x   0 reeves     (501) staff       (20)        0 2023-07-27 01:19:49.516219 v4-0.1.2/
+-rwxrwxrwx   0 reeves     (501) staff       (20)    35148 2014-09-08 17:52:36.000000 v4-0.1.2/LICENSE.txt
+-rw-r--r--   0 reeves     (501) staff       (20)      288 2023-07-27 01:19:49.516006 v4-0.1.2/PKG-INFO
+-rwxrwxrwx   0 reeves     (501) staff       (20)      838 2018-04-12 20:31:22.000000 v4-0.1.2/README.md
+-rw-r--r--   0 reeves     (501) staff       (20)       38 2023-07-27 01:19:49.516265 v4-0.1.2/setup.cfg
+-rwxrwxrwx   0 reeves     (501) staff       (20)      384 2023-07-27 01:18:04.000000 v4-0.1.2/setup.py
+drwxr-xr-x   0 reeves     (501) staff       (20)        0 2023-07-27 01:19:49.513381 v4-0.1.2/v4/
+-rwxrwxrwx   0 reeves     (501) staff       (20)        2 2017-12-29 23:35:19.000000 v4-0.1.2/v4/__init__.py
+-rw-r--r--   0 reeves     (501) staff       (20)    12327 2023-07-27 00:50:11.000000 v4-0.1.2/v4/vd.py
+-rwxr-xr-x   0 reeves     (501) staff       (20)    28084 2023-07-27 01:17:15.000000 v4-0.1.2/v4/vx.py
+drwxr-xr-x   0 reeves     (501) staff       (20)        0 2023-07-27 01:19:49.515769 v4-0.1.2/v4.egg-info/
+-rwxrwxrwx   0 reeves     (501) staff       (20)      288 2023-07-27 01:19:49.000000 v4-0.1.2/v4.egg-info/PKG-INFO
+-rwxrwxrwx   0 reeves     (501) staff       (20)      167 2023-07-27 01:19:49.000000 v4-0.1.2/v4.egg-info/SOURCES.txt
+-rwxrwxrwx   0 reeves     (501) staff       (20)        1 2023-07-27 01:19:49.000000 v4-0.1.2/v4.egg-info/dependency_links.txt
+-rwxrwxrwx   0 reeves     (501) staff       (20)        3 2023-07-27 01:19:49.000000 v4-0.1.2/v4.egg-info/top_level.txt
```

### Comparing `v4-0.1.1/LICENSE.txt` & `v4-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `v4-0.1.1/README.md` & `v4-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `v4-0.1.1/v4/vd.py` & `v4-0.1.2/v4/vd.py`

 * *Files identical despite different names*

### Comparing `v4-0.1.1/v4/vx.py` & `v4-0.1.2/v4/vx.py`

 * *Files 0% similar despite different names*

```diff
@@ -806,24 +806,24 @@
         else:
             dolist += ' ' + i
             #print i
     return plist + dolist + polist;
 def vxinfo( vxarg):
     #if type(vxim)  == np.ndarray:
     res = {}
-    vxim = vx.vximp(vxarg)
+    vxim = vximp(vxarg)
     res['shape'] = np.shape(vxim.i)
     res['dtype'] = vxim.i.dtype
     #res[bbox'] = vxim.bbx
     res['color'] = vxim.c == 3
     return res
 
 def vxstats( vxarg):
     res = {}
-    vxim = vx.vximp(vxarg)
+    vxim = vximp(vxarg)
     res['mean'] = round(np.mean(vxim.i), 5)
     res['median'] = round(np.median(vxim.i), 5)
     res['min'] = round(np.min(vxim.i), 5)
     res['max'] = round(np.max(vxim.i), 5)
     res['std'] = round(np.std(vxim.i), 5)
     vq = vxim.i.astype(float)
     #vq = np.where(vxim.i == 0, 'NaN',vq)
```

