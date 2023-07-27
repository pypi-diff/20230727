# Comparing `tmp/sanic_useragent-0.1.3-py3-none-any.whl.zip` & `tmp/sanic_useragent-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3852 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     7291 b- defN 20-Aug-16 02:45 sanic_useragent/__init__.py
--rw-rw-rw-  2.0 fat      838 b- defN 20-Aug-16 02:58 sanic_useragent-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 20-Aug-16 02:58 sanic_useragent-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 20-Aug-16 02:58 sanic_useragent-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      413 b- defN 20-Aug-16 02:58 sanic_useragent-0.1.3.dist-info/RECORD
-5 files, 8655 bytes uncompressed, 3076 bytes compressed:  64.5%
+Zip file size: 3873 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     7293 b- defN 23-Jul-27 01:19 sanic_useragent/__init__.py
+-rw-rw-rw-  2.0 fat     1118 b- defN 23-Jul-27 01:25 sanic_useragent-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 01:25 sanic_useragent-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jul-27 01:25 sanic_useragent-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      414 b- defN 23-Jul-27 01:25 sanic_useragent-0.1.4.dist-info/RECORD
+5 files, 8933 bytes uncompressed, 3097 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: sanic_useragent/__init__.py
 Comment: 
 
-Filename: sanic_useragent-0.1.3.dist-info/METADATA
+Filename: sanic_useragent-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: sanic_useragent-0.1.3.dist-info/WHEEL
+Filename: sanic_useragent-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: sanic_useragent-0.1.3.dist-info/top_level.txt
+Filename: sanic_useragent-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: sanic_useragent-0.1.3.dist-info/RECORD
+Filename: sanic_useragent-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sanic_useragent/__init__.py

```diff
@@ -56,23 +56,23 @@
         ('netscape', 'netscape'),
         (r'msie|microsoft\s+internet\s+explorer|trident/.+? rv:', 'msie'),
         ('lynx', 'lynx'),
         ('links', 'links'),
         ('seamonkey|mozilla', 'seamonkey')
     )
 
-    _browser_version_re = r'(?:%s)[/\sa-z(]*(\d+[.\da-z]+)?(?i)'
+    _browser_version_re = r'(?:%s)[/\sa-z(]*(\d+[.\da-z]+)?'
     _language_re = re.compile(
         r'(?:;\s*|\s+)(\b\w{2}\b(?:-\b\w{2}\b)?)\s*;|'
         r'(?:\(|\[|;)\s*(\b\w{2}\b(?:-\b\w{2}\b)?)\s*(?:\]|\)|;)'
     )
 
     def __init__(self):
         self.platforms = [(b, re.compile(a, re.I)) for a, b in self.platforms]
-        self.browsers = [(b, re.compile(self._browser_version_re % a))
+        self.browsers = [(b, re.compile(self._browser_version_re % a, re.I))
                          for a, b in self.browsers]
 
     def __call__(self, headers):
         user_agent = headers.get('user-agent', '')
         if user_agent:
             for platform, regex in self.platforms:
                 match = regex.search(user_agent)
```

