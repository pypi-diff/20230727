# Comparing `tmp/wiretap-5.0.0-py3-none-any.whl.zip` & `tmp/wiretap-5.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5380 bytes, number of entries: 7
+Zip file size: 5209 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      140 b- defN 23-Jul-20 17:54 wiretap/__init__.py
 -rw-rw-rw-  2.0 fat      620 b- defN 23-Feb-08 09:16 wiretap/layers.py
--rw-rw-rw-  2.0 fat    14455 b- defN 23-Jul-20 20:20 wiretap/wiretap.py
--rw-rw-rw-  2.0 fat      244 b- defN 23-Jul-21 12:34 wiretap-5.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 12:34 wiretap-5.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-21 12:34 wiretap-5.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      520 b- defN 23-Jul-21 12:34 wiretap-5.0.0.dist-info/RECORD
-7 files, 16079 bytes uncompressed, 4462 bytes compressed:  72.2%
+-rw-rw-rw-  2.0 fat    13934 b- defN 23-Jul-27 07:55 wiretap/wiretap.py
+-rw-rw-rw-  2.0 fat      244 b- defN 23-Jul-27 08:10 wiretap-5.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-27 08:10 wiretap-5.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-27 08:10 wiretap-5.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      520 b- defN 23-Jul-27 08:11 wiretap-5.0.1.dist-info/RECORD
+7 files, 15558 bytes uncompressed, 4291 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: wiretap/layers.py
 Comment: 
 
 Filename: wiretap/wiretap.py
 Comment: 
 
-Filename: wiretap-5.0.0.dist-info/METADATA
+Filename: wiretap-5.0.1.dist-info/METADATA
 Comment: 
 
-Filename: wiretap-5.0.0.dist-info/WHEEL
+Filename: wiretap-5.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: wiretap-5.0.0.dist-info/top_level.txt
+Filename: wiretap-5.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: wiretap-5.0.0.dist-info/RECORD
+Filename: wiretap-5.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wiretap/wiretap.py

```diff
@@ -167,15 +167,15 @@
             self,
             message: Optional[str] = None,
             details: Optional[dict[str, Any]] = None,
             attachment: Optional[Any] = None,
             result: Optional[TValue] = None,
             result_format: FormatOptions | dict[str, FormatOptions] = None
     ) -> Optional[TValue]:
-        self._logger.setLevel(logging.ERROR if sys.exc_info()[0] is Failure else logging.WARNING)
+        self._logger.setLevel(logging.ERROR)
         self._log(message, details, attachment, result, result_format)
         return result
 
     def failed(
             self,
             message: Optional[str] = None,
             details: Optional[dict[str, Any]] = None,
@@ -183,22 +183,18 @@
             result: Optional[TValue] = None,
             result_format: FormatOptions | dict[str, FormatOptions] = None
     ) -> Optional[TValue]:
         self._logger.setLevel(logging.ERROR)
 
         # process the exception only if it's not Failure
         exc_cls, exc, exc_tb = sys.exc_info()
-        if exc and exc_cls is not Failure:
+        if all((exc_cls, exc, exc_tb)):
             # the first 3 frames are the decorator traces; let's get rid of them
-            for _ in range(3):
-                # in case there aren't that many frames
-                if exc_tb.tb_next:
-                    exc_tb = exc_tb.tb_next
-                else:
-                    break
+            while exc_tb.tb_next:
+                exc_tb = exc_tb.tb_next
             self._log(message, details, attachment, result, result_format, (exc_cls, exc, exc_tb))
         else:
             self._log(message, details, attachment, result, result_format)
 
         return result
 
     def _log(
@@ -240,19 +236,14 @@
     def __iter__(self):
         current = self
         while current:
             yield current
             current = current.parent
 
 
-# Helps to prevent logging the same exception multiple times.
-class Failure(Exception):
-    pass
-
-
 @contextlib.contextmanager
 def telemetry_scope(
         module: Optional[str],
         name: str,
         message: Optional[str] = None,
         details: Optional[dict[str, Any]] = None,
         attachment: Optional[Any] = None
@@ -260,20 +251,17 @@
     """Begins a new telemetry scope."""
     logger = Logger(module, name, _scope.get())
     token = _scope.set(logger)
     try:
         logger.started(message, details, attachment)
         yield logger
         logger.completed()
-    except Failure:
-        logger.canceled(message="Unhandled exception has occurred.")
-        raise
     except Exception as e:  # noqa
         logger.failed(message="Unhandled exception has occurred.")
-        raise Failure from e  # wrap the original exception in Failure to keep failing and prevent logging it multiple times
+        raise
     finally:
         _scope.reset(token)
 
 
 class Cancellation(Exception):
     def __init__(self, message: str, result: Any | None = None, result_format: FormatOptions | dict[str, FormatOptions] = None):
         super().__init__(message)
```

## Comparing `wiretap-5.0.0.dist-info/RECORD` & `wiretap-5.0.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 wiretap/__init__.py,sha256=k7Ug6yarTCPvPv1NKjoHrC-Cw4cFZ25FGxBG88Ra7pM,140
 wiretap/layers.py,sha256=KUAcHoCD4DsiBqd85OndrxZpxl0YVYfr2UKm8Co0004,620
-wiretap/wiretap.py,sha256=UP7BLF0HoYJV5wamEihu-TNIq3znm6_7cpcgDpqn6yM,14455
-wiretap-5.0.0.dist-info/METADATA,sha256=yQ3aB3czjM2OUtoXdEA_5V_3LQy_r8-NhDwbADNbBCQ,244
-wiretap-5.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-wiretap-5.0.0.dist-info/top_level.txt,sha256=qmBPPxbsuDq57r7kh5q29WKFFyvB8j8Mzgx5RKHnwAw,8
-wiretap-5.0.0.dist-info/RECORD,,
+wiretap/wiretap.py,sha256=-S4Rlx_LKc6uXWWUYC5JKq_4GZpkHjmKtmz-hCw1UYM,13934
+wiretap-5.0.1.dist-info/METADATA,sha256=wEVVnLENz0GEopNRacAB1pQtcrzSKFFbTWYjHf5Wp3o,244
+wiretap-5.0.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wiretap-5.0.1.dist-info/top_level.txt,sha256=qmBPPxbsuDq57r7kh5q29WKFFyvB8j8Mzgx5RKHnwAw,8
+wiretap-5.0.1.dist-info/RECORD,,
```

