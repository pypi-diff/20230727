# Comparing `tmp/VNPT-0.3.tar.gz` & `tmp/VNPT-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VNPT-0.3.tar", last modified: Thu Jul 27 02:22:33 2023, max compression
+gzip compressed data, was "VNPT-0.4.tar", last modified: Thu Jul 27 02:44:18 2023, max compression
```

## Comparing `VNPT-0.3.tar` & `VNPT-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 02:22:33.979395 VNPT-0.3/
--rw-rw-rw-   0        0        0     1083 2023-07-27 01:43:43.000000 VNPT-0.3/LICENSE
--rw-rw-rw-   0        0        0      228 2023-07-27 02:22:33.978391 VNPT-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       49 2023-07-27 01:43:43.000000 VNPT-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 02:22:33.971396 VNPT-0.3/VNPT.egg-info/
--rw-rw-rw-   0        0        0      228 2023-07-27 02:22:33.000000 VNPT-0.3/VNPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-07-27 02:22:33.000000 VNPT-0.3/VNPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 02:22:33.000000 VNPT-0.3/VNPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-27 01:50:41.000000 VNPT-0.3/VNPT.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-07-27 02:22:33.000000 VNPT-0.3/VNPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-27 02:22:33.000000 VNPT-0.3/VNPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 02:22:33.980395 VNPT-0.3/setup.cfg
--rw-rw-rw-   0        0        0      435 2023-07-27 02:22:23.000000 VNPT-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 02:22:33.975393 VNPT-0.3/vnpt/
--rw-rw-rw-   0        0        0        0 2023-07-27 02:12:21.000000 VNPT-0.3/vnpt/__init__.py
--rw-rw-rw-   0        0        0     1405 2023-07-26 06:06:56.000000 VNPT-0.3/vnpt/sql_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:44:18.077353 VNPT-0.4/
+-rw-rw-rw-   0        0        0     1083 2023-07-27 01:43:43.000000 VNPT-0.4/LICENSE
+-rw-rw-rw-   0        0        0      228 2023-07-27 02:44:18.076353 VNPT-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2023-07-27 01:43:43.000000 VNPT-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 02:44:18.067362 VNPT-0.4/VNPT.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-07-27 02:44:17.000000 VNPT-0.4/VNPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-07-27 02:44:17.000000 VNPT-0.4/VNPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 02:44:17.000000 VNPT-0.4/VNPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-27 01:50:41.000000 VNPT-0.4/VNPT.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-07-27 02:44:17.000000 VNPT-0.4/VNPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-27 02:44:17.000000 VNPT-0.4/VNPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 02:44:18.078353 VNPT-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      435 2023-07-27 02:44:13.000000 VNPT-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 02:44:18.072356 VNPT-0.4/vnpt/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:12:21.000000 VNPT-0.4/vnpt/__init__.py
+-rw-rw-rw-   0        0        0     1938 2023-07-27 02:43:50.000000 VNPT-0.4/vnpt/sql_helper.py
```

### Comparing `VNPT-0.3/LICENSE` & `VNPT-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `VNPT-0.3/vnpt/sql_helper.py` & `VNPT-0.4/vnpt/sql_helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -47,9 +47,28 @@
             del cursor
             gc.collect()
             
             return df
         except Exception as e:
             traceback.print_exc()
 
-    
-        
+    def execute(self, sql_str, params)->int:
+        count = -1
+        try:
+            conn = self.conn
+            cursor = conn.cursor()
+            cursor.execute(sql_str, params)
+            count = cursor.rowcount
+            conn.commit()
+            
+            # clear cache
+            cursor.close()
+            conn.close()
+            del conn
+            del cursor
+            gc.collect()
+        except Exception as e:
+            traceback.print_exc()
+        finally:
+            return count
+        
+
```

