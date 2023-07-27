# Comparing `tmp/weboptout-0.2.1.tar.gz` & `tmp/weboptout-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weboptout-0.2.1.tar", max compression
+gzip compressed data, was "weboptout-0.2.2.tar", max compression
```

## Comparing `weboptout-0.2.1.tar` & `weboptout-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5003 2023-07-26 20:11:12.697787 weboptout-0.2.1/LICENSE
--rw-r--r--   0        0        0     7628 2023-07-26 20:11:13.265795 weboptout-0.2.1/data/tos.jsonl
--rw-r--r--   0        0        0      900 2023-07-26 20:11:13.285795 weboptout-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      183 2023-07-26 20:11:13.285795 weboptout-0.2.1/src/weboptout/__init__.py
--rw-r--r--   0        0        0     1228 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/client.py
--rw-r--r--   0        0        0     1421 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/config.py
--rw-r--r--   0        0        0     3418 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/html.py
--rw-r--r--   0        0        0     8030 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/http.py
--rw-r--r--   0        0        0     1537 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/types.py
--rw-r--r--   0        0        0     6987 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/utils.py
--rw-r--r--   0        0        0     1690 2023-07-26 20:11:12.697787 weboptout-0.2.1/src/weboptout/web.py
--rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 weboptout-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     5003 2023-07-27 10:15:30.579513 weboptout-0.2.2/LICENSE
+-rw-r--r--   0        0        0     7766 2023-07-27 10:15:31.339551 weboptout-0.2.2/data/tos.jsonl
+-rw-r--r--   0        0        0      900 2023-07-27 10:15:31.355552 weboptout-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      191 2023-07-27 10:15:31.355552 weboptout-0.2.2/src/weboptout/__init__.py
+-rw-r--r--   0        0        0     1228 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/client.py
+-rw-r--r--   0        0        0     1742 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/config.py
+-rw-r--r--   0        0        0     4092 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/html.py
+-rw-r--r--   0        0        0     8030 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/http.py
+-rw-r--r--   0        0        0     1637 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/types.py
+-rw-r--r--   0        0        0     7003 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/utils.py
+-rw-r--r--   0        0        0     1690 2023-07-27 10:15:30.579513 weboptout-0.2.2/src/weboptout/web.py
+-rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 weboptout-0.2.2/PKG-INFO
```

### Comparing `weboptout-0.2.1/LICENSE` & `weboptout-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `weboptout-0.2.1/data/tos.jsonl` & `weboptout-0.2.2/data/tos.jsonl`

 * *Files 0% similar despite different names*

```diff
@@ -28,21 +28,23 @@
 ["photos.smugmug.com", "https://www.smugmug.com/about/terms"]
 ["i?.cpcache.com", "https://www.cafepress.com/p/terms-conditions"]
 ["*aliexpress.*", "https://rulechannel.alibaba.com/icbu?spm=a1zaa.8161610.0.0.23eb61ecCCJxWd&type=detail&ruleId=2041&cId=1307#/rule/detail?cId=1307&ruleId=2041"]
 ["*.alicdn.com", "https://rulechannel.alibaba.com/icbu?spm=a1zaa.8161610.0.0.23eb61ecCCJxWd&type=detail&ruleId=2041&cId=1307#/rule/detail?cId=1307&ruleId=2041"]                
 ["*.i.aliimg.com", "https://rulechannel.alibaba.com/icbu?type=detail&ruleId=2041&cId=1307#/rule/detail?cId=1307&ruleId=2041"]
 ["*gettyimages.com", "https://www.gettyimages.com/company/terms?language=en-us"]
 ["cdn*.bigcommerce.com", "https://www.bigcommerce.com/terms/acceptable-use-policy/"]
-["*.gstatic.com", "https://policies.google.com/terms?hl=en"]
+["*.gstatic.com", "https://policies.google.com/terms?hl=en-us"]
+["*.googleusercontent.com", "https://policies.google.com/terms?hl=en"]
+["storage.googleapis.com", "https://policies.google.com/terms?hl=en"]
 ["media-cdn.tripadvisor.com", "https://tripadvisor.mediaroom.com/us-terms-of-use"]
 ["*.redbubble.net", "https://www.redbubble.com/agreement"]
 ["images.*.prom.st", "https://prom.ua/ua/terms-of-use"]
 ["cdn.xxl.thumbs.canstockphoto.com", "https://www.canstockphoto.com/terms_conditions/"]
 ["ssl.c.photoshelter.com", "https://company.photoshelter.com/terms/"]
-["?.bp.blogspot.com", "https://policies.google.com/u/0/terms?hl=en"]
+["?.bp.blogspot.com", "https://policies.google.com/u/0/terms"]
 ["*.scribdassets.com", "https://support.scribd.com/hc/en-us/articles/210129326-General-Terms-of-Use"]
 ["ctl.s6img.com", "https://society6.com/terms"]
 ["*.bing.net", "https://www.microsoft.com/en-us/legal/terms-of-use"]
 ["upload.wikimedia.org", "https://foundation.wikimedia.org/wiki/Policy:Terms_of_Use"]
 ["img.shopstyle-cdn.com", "https://www.shopstyle.com/tos"]
 ["cdn.webshopapp.com", "https://www.lightspeedhq.com/legal/lightspeed-service-agreement/"]
 ["?.keepcalms.com", "https://keepcalms.com/privacy/"]
```

### Comparing `weboptout-0.2.1/pyproject.toml` & `weboptout-0.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "weboptout"
 description = "Checks the Copyright information of online works and their conditions of use."
-version = "0.2.1"
+version = "0.2.2"
 authors = ["Alex J. Champandard <445208+alexjc@users.noreply.github.com>"]
 repository = "https://github.com/alexjc/weboptout"
 license = "MIT and UNLICENSED"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
 ]
@@ -17,15 +17,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 aiohttp = ">=3.8"
 langdetect = ">=1.0.9"
 beautifulsoup4 = ">=4.12"
-selenium = { version = "0.2.1", optional = true }
+selenium = { version = "0.2.2", optional = true }
 
 [tool.poetry.extras]
 webdriver = ["selenium"]
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.0.0"
 hypothesis = ">=6.0.0"
```

### Comparing `weboptout-0.2.1/src/weboptout/client.py` & `weboptout-0.2.2/src/weboptout/client.py`

 * *Files identical despite different names*

### Comparing `weboptout-0.2.1/src/weboptout/config.py` & `weboptout-0.2.2/src/weboptout/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,22 +15,32 @@
 terms|legal|conditions|guidelines\
 )""", re.I)
 
 # Parts of words that indicate a TDM activity, ordered by confidence.
 RE_TDM_CONCEPTS = [
     re.compile(p, re.I) for p in [
         "(scrap(e|er|ing)|data[\s-]min(e|ing))",
-        "(spider|robot|crawl(ing|er)?|index(ing|er))",
-        "automated (software|tool|mean|system|way|device)s?",
+        "(spider|robot|crawl(ing|er)?)",
+        "(automated|automatic) (software|tool|mean|system|way|device)s?",
         "(image library|machine learning|deep leaning|populate a database)",
         "(extract|compil(e|at)?|collect)(ing|ion)? (data|content|material|information)",
         "harvest(ing|er)?",
     ]
 ]
 
+# Parts of words that indicate non-commercial or personal use only.
+RE_NFP_CONCEPTS = [
+    re.compile(p, re.I) for p in [
+        "(non-commercial|non commercial) (use|purpose)",
+        "not\s*(meant|intended)?\s*for commercial (use|usage)",
+        "not-for-profit",
+        "(personal|private) (use|purpose)",
+    ]
+]
+
 # Bag-of-words that represent legal concepts to detect legal documents.
 RE_LEGAL_WORDS = re.compile("""\
 (effective|accept|entitle|dispute|providing|unable|reasonable|applicable|\
 precludes|enforcement|reserve|terminate|section|constitute|damages|liable|\
 obligations|information|processing|consent|privacy|limited|necessary|\
 purpose|decide|account|security|request|protection\
 )""", re.I)
```

### Comparing `weboptout-0.2.1/src/weboptout/html.py` & `weboptout-0.2.2/src/weboptout/html.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,101 @@
 ## Copyright © 2023, Alex J. Champandard.  Licensed under MIT; see LICENSE! ⚘
 
 import re
 import langdetect
 from bs4 import BeautifulSoup
 
 from .types import Status
-from .config import RE_TDM_CONCEPTS, RE_LEGAL_WORDS
+from .config import RE_TDM_CONCEPTS, RE_LEGAL_WORDS, RE_NFP_CONCEPTS
 
 
 __all__ = ["check_tos_reservation"]
 
 
-def check_tos_reservation(client, url: str, html: str) -> Status:
-    soup = BeautifulSoup(html, "html.parser")
-    text = "\n".join(_extract_paragraphs(soup))
-
-    para_count = text.count("\n") + 1
-
-    if len(text) > 1_000 and (lang := langdetect.detect(text)) != "en":
-        client.log(
-            Status.FAILURE,
-            f"Found a possible ToS page but language is '{lang.upper()}' at {url}.",
-        )
-        return Status.ABORT
-
+def _find_matching_paragraphs(patterns: list, text: str) -> list[tuple]:
+    """
+    For each paragraph in the text, apply all the patterns in order and stop when
+    there's a match.  The results are sorted by rank of the pattern to find which
+    is the most important.
+    """
     reasons = []
     for line in text.split("\n"):
-        for rank, regexp in enumerate(RE_TDM_CONCEPTS):
+        for rank, regexp in enumerate(patterns):
             match = regexp.search(line.rstrip("\n"))
             if not match:
                 continue
 
             i, j = match.start(), match.end() - 1
             while line[i] not in "().;" and i > 0:
                 i -= 1
             while line[j] not in "().;" and j + 1 < len(line):
                 j += 1
 
-            if len(line[i : j + 1]) < 512:
-                explain = line[i : j + 1].lstrip("().,; ").rstrip("() ")
-                reasons.append((rank, explain, line))
+            explain = line[i : j + 1].lstrip("().,; ").rstrip("() ")
+            reasons.append((rank, explain, line))
             break
 
-    if len(reasons):
-        reasons = sorted(reasons, key=lambda x: x[0] * 1000 - len(x[1]))
+    return sorted(reasons, key=lambda x: x[0] * 1000 - len(x[1]))
+
+
+def check_tos_reservation(client, url: str, html: str) -> Status:
+    soup = BeautifulSoup(html, "html.parser")
+    text = "\n".join(_extract_paragraphs(soup))
+
+    para_count = text.count("\n") + 1
+
+    # Only english language is currently supported.
+    if len(text) > 1_000 and (lang := langdetect.detect(text)) != "en":
+        client.log(
+            Status.FAILURE,
+            f"Found a possible ToS page but language is '{lang.upper()}' at {url}",
+        )
+        return Status.ABORT
+
+    # Words that match data-mining concepts.
+    if len(reasons := _find_matching_paragraphs(RE_TDM_CONCEPTS, text)):
         client.log(
             Status.SUCCESS,
             f"Found a total of {len(reasons)} matching paragraphs out of "
             f"{para_count} in Terms Of Service.",
             highlight=reasons[0][1],
             paragraph=reasons[0][2],
         )
         return Status.SUCCESS
 
-    elif len(text) < 2_000:
-        size = len(text)
+    # Words that match not-for-profit reservations.
+    if len(reasons := _find_matching_paragraphs(RE_NFP_CONCEPTS, text)):
+        client.log(
+            Status.SUCCESS,
+            f"Found total of {len(reasons)} paragraphs matching "
+            f"non-commercial activities in Terms Of Service.",
+            highlight=reasons[0][1],
+        )
+        return Status.SUCCESS
+
+    if (size := len(text)) < 2_000:
         client.log(
             Status.FAILURE,
             f"Too little information extracted, only {size:,} bytes from "
-            f"the ToS page at {url}.",
+            f"the ToS page at {url}",
         )
 
         # Suggest fetching page again via HTTP with Selenium.
         return Status.RETRY
 
-    else:
-        legal_words = len(RE_LEGAL_WORDS.findall(text))
-        if legal_words < 36:
-            client.log(
-                Status.FAILURE,
-                f"The ToS page does not appear to contain a legal text at {url}.",
-            )
-            return Status.FAILURE
+    if len(RE_LEGAL_WORDS.findall(text)) < 36:
+        client.log(
+            Status.FAILURE,
+            f"The ToS page does not appear to contain a legal text at {url}",
+        )
+        return Status.FAILURE
 
     client.log(
         Status.FAILURE,
-        f"No direct matches found in {para_count} paragraphs found at {url}.",
+        f"No direct matches found in {para_count} paragraphs found at {url}",
     )
     return Status.ABORT
 
 
 def _extract_paragraphs(soup):
     """
     Iterator that returns a cleaned up list of paragraphs, lists items, from
```

### Comparing `weboptout-0.2.1/src/weboptout/http.py` & `weboptout-0.2.2/src/weboptout/http.py`

 * *Files identical despite different names*

### Comparing `weboptout-0.2.1/src/weboptout/types.py` & `weboptout-0.2.2/src/weboptout/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,7 +47,11 @@
     Namespace with default Reservations that can be cloned and used for comparison.
     """
 
     YES = Reservation(2)
     MAYBE = Reservation(1)
     NO = Reservation(0)
     ERROR = Reservation(-1)
+
+    @staticmethod
+    def get_name(res):
+        return ['ERROR', 'NO', 'MAYBE', 'YES'][res._id+1]
```

### Comparing `weboptout-0.2.1/src/weboptout/utils.py` & `weboptout-0.2.2/src/weboptout/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,31 +54,31 @@
     return _decorator
 
 
 def cache_to_directory(directory, /, key: str, filter: callable = None):
     """
     Decorator to cache results of a function to individual pickle files on disk.
     """
-    directory = pkg_resources.resource_filename(__name__, directory)
-    directory = directory.replace('src/weboptout/', '')
-    os.makedirs(directory, exist_ok=True)
+    full_path = pkg_resources.resource_filename(__name__, directory)
+    full_path = full_path.replace('src/weboptout/', '')
+    os.makedirs(full_path, exist_ok=True)
 
     def _decorator(fn):        
         arg_names = list(inspect.signature(fn).parameters.keys())
         arg_idx = arg_names.index(key)
 
         assert inspect.iscoroutinefunction(fn), \
             "Synchronous functions not supported by cache_to_directory."
 
         async def _wrapper(*args, **kwargs):
             hex = hashlib.md5(args[arg_idx].encode()).hexdigest()
-            filename = f'{directory}/{hex}.pkl'
+            filename = f'{full_path}/{hex}.pkl'
             if os.path.isfile(filename):
                 result = pickle.load(open(filename, 'rb'))
-                if filter is None or not filter(*args, filename=filename, result=result):
+                if filter is None or not filter(*args, filename=f'{directory}/{hex}.pkl', result=result):
                     return result
 
             result = await fn(*args, **kwargs)
             pickle.dump(result, open(filename, 'wb'))
             return result
 
         _wrapper.__wrapped__ = fn
```

### Comparing `weboptout-0.2.1/src/weboptout/web.py` & `weboptout-0.2.2/src/weboptout/web.py`

 * *Files identical despite different names*

### Comparing `weboptout-0.2.1/PKG-INFO` & `weboptout-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weboptout
-Version: 0.2.1
+Version: 0.2.2
 Summary: Checks the Copyright information of online works and their conditions of use.
 Home-page: https://github.com/alexjc/weboptout
 License: MIT and UNLICENSED
 Author: Alex J. Champandard
 Author-email: 445208+alexjc@users.noreply.github.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,9 +14,9 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Provides-Extra: webdriver
 Requires-Dist: aiohttp (>=3.8)
 Requires-Dist: beautifulsoup4 (>=4.12)
 Requires-Dist: langdetect (>=1.0.9)
-Requires-Dist: selenium (==0.2.1) ; extra == "webdriver"
+Requires-Dist: selenium (==0.2.2) ; extra == "webdriver"
 Project-URL: Repository, https://github.com/alexjc/weboptout
```

