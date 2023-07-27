# Comparing `tmp/dimtown_spider-0.0.3.tar.gz` & `tmp/dimtown_spider-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimtown_spider-0.0.3.tar", max compression
+gzip compressed data, was "dimtown_spider-0.0.4.tar", max compression
```

## Comparing `dimtown_spider-0.0.3.tar` & `dimtown_spider-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/LICENSE
--rw-r--r--   0        0        0     2028 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/README.md
--rw-r--r--   0        0        0     1611 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/AnimeAvatar.py
--rw-r--r--   0        0        0     1154 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/ArtAlbum.py
--rw-r--r--   0        0        0      926 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/CoupleAvatar.py
--rw-r--r--   0        0        0     1090 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/FemaleAvatar.py
--rw-r--r--   0        0        0     1019 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/Figure.py
--rw-r--r--   0        0        0     1099 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/MaleAvatar.py
--rw-r--r--   0        0        0     1386 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/SelectedIllustrations.py
--rw-r--r--   0        0        0     1330 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/SelectedPixiv.py
--rw-r--r--   0        0        0      922 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/__init__.py
--rw-r--r--   0        0        0     1276 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/cosplay.py
--rw-r--r--   0        0        0     1114 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/hanfu.py
--rw-r--r--   0        0        0     1123 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/jk.py
--rw-r--r--   0        0        0     1320 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/lolita.py
--rw-r--r--   0        0        0     1330 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/pcpic.py
--rw-r--r--   0        0        0     1478 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/phonepic.py
--rw-r--r--   0        0        0     4199 2023-07-27 07:46:42.948548 dimtown_spider-0.0.3/dimtown/utils.py
--rw-r--r--   0        0        0      399 2023-07-27 07:46:42.952548 dimtown_spider-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 dimtown_spider-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2028 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/README.md
+-rw-r--r--   0        0        0     1584 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/AnimeAvatar.py
+-rw-r--r--   0        0        0     1097 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/ArtAlbum.py
+-rw-r--r--   0        0        0      912 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/CoupleAvatar.py
+-rw-r--r--   0        0        0     1076 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/FemaleAvatar.py
+-rw-r--r--   0        0        0     1005 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/Figure.py
+-rw-r--r--   0        0        0     1085 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/MaleAvatar.py
+-rw-r--r--   0        0        0     1329 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/SelectedIllustrations.py
+-rw-r--r--   0        0        0     1273 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/SelectedPixiv.py
+-rw-r--r--   0        0        0      922 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/__init__.py
+-rw-r--r--   0        0        0     1125 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/cosplay.py
+-rw-r--r--   0        0        0     1101 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/hanfu.py
+-rw-r--r--   0        0        0     1066 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/jk.py
+-rw-r--r--   0        0        0     1263 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/lolita.py
+-rw-r--r--   0        0        0     1273 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/pcpic.py
+-rw-r--r--   0        0        0     1327 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/phonepic.py
+-rw-r--r--   0        0        0     4199 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/dimtown/utils.py
+-rw-r--r--   0        0        0      399 2023-07-27 07:55:00.707857 dimtown_spider-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 dimtown_spider-0.0.4/PKG-INFO
```

### Comparing `dimtown_spider-0.0.3/LICENSE` & `dimtown_spider-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.3/README.md` & `dimtown_spider-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.3/dimtown/AnimeAvatar.py` & `dimtown_spider-0.0.4/dimtown/AnimeAvatar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from utils import Spider
-import asyncio
-import httpx
+from .utils import Spider
 from bs4 import BeautifulSoup
 
 class AnimeAvatar(Spider):
     '''
     `漫画头像`获取
     '''
     def __init__(self) -> None:
```

### Comparing `dimtown_spider-0.0.3/dimtown/ArtAlbum.py` & `dimtown_spider-0.0.4/dimtown/ArtAlbum.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from utils import Spider
-from bs4 import BeautifulSoup
-import httpx
-import asyncio
+from .utils import Spider
 
 class ArtAlbum(Spider):
     '''
     `画册`获取
     '''
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `dimtown_spider-0.0.3/dimtown/CoupleAvatar.py` & `dimtown_spider-0.0.4/dimtown/CoupleAvatar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from AnimeAvatar import AnimeAvatar
-import asyncio
+from .AnimeAvatar import AnimeAvatar
 
 class CoupleAvatar(AnimeAvatar):
     '''
     `情侣头像`获取
     '''
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `dimtown_spider-0.0.3/dimtown/FemaleAvatar.py` & `dimtown_spider-0.0.4/dimtown/FemaleAvatar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from AnimeAvatar import AnimeAvatar
-import asyncio
+from .AnimeAvatar import AnimeAvatar
 
 class FemaleAvatar(AnimeAvatar):
     '''
     `女生头像`获取
     '''
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `dimtown_spider-0.0.3/dimtown/Figure.py` & `dimtown_spider-0.0.4/dimtown/Figure.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from utils import Spider
-import asyncio
+from .utils import Spider
 
 class Figure(Spider):
     '''
     `手办`图片获取
     '''
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `dimtown_spider-0.0.3/dimtown/MaleAvatar.py` & `dimtown_spider-0.0.4/dimtown/MaleAvatar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from AnimeAvatar import AnimeAvatar
-import asyncio
+from .AnimeAvatar import AnimeAvatar
 
 class MaleAvatar(AnimeAvatar):
     '''
     `男生头像`获取
     '''
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `dimtown_spider-0.0.3/dimtown/SelectedIllustrations.py` & `dimtown_spider-0.0.4/dimtown/SelectedIllustrations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from utils import Spider
-from bs4 import BeautifulSoup
-import httpx
-import asyncio
+from .utils import Spider
 
 class SelectedIllustrations(Spider):
     '''
     `精选插画`获取
     '''
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `dimtown_spider-0.0.3/dimtown/SelectedPixiv.py` & `dimtown_spider-0.0.4/dimtown/SelectedPixiv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from utils import Spider
-from bs4 import BeautifulSoup
-import httpx
-import asyncio
+from .utils import Spider
 
 class SelectedPixiv(Spider):
     '''
     `精选Pixiv`获取
     '''
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `dimtown_spider-0.0.3/dimtown/__init__.py` & `dimtown_spider-0.0.4/dimtown/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 
 __all__ = ['AnimeAvatar', 'ArtAlbum', 'CosPlay', 'CoupleAvatar', 'FemaleAvatar', 'Figure', 
             'HanFu', 'JK', 'Lolita', 'MaleAvatar', 'PcPic', 'PhonePic', 'SelectedIllustrations', 
             'SelectedPixiv']
 __title__ = 'dimtown'
 __description__ = 'A Spider for https://dimtown.com'
 __url__ = 'https://github.com/Cvandia/dimtown-spider'
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 __author__ = 'Cvandia'
 __author_email__ = '1141538825@qq.com'
 __license__ = 'MIT License'
```

### Comparing `dimtown_spider-0.0.3/dimtown/cosplay.py` & `dimtown_spider-0.0.4/dimtown/cosplay.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-from utils import Spider
-from bs4 import BeautifulSoup
-import httpx
-import asyncio
-try:
-    import ujson as json
-except ModuleNotFoundError:
-    import json
-import os
-import re
+from .utils import Spider
 
 class CosPlay(Spider):
     '''
     `CosPlay`获取
     '''
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `dimtown_spider-0.0.3/dimtown/hanfu.py` & `dimtown_spider-0.0.4/dimtown/hanfu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from utils import Spider
-import asyncio
+from .utils import Spider
+
 class HanFu(Spider):
     '''
     `汉服`图片获取
     '''
     def __init__(self) -> None:
         super().__init__()
         self.api_url = self.base_url + "hanfu"
```

### Comparing `dimtown_spider-0.0.3/dimtown/jk.py` & `dimtown_spider-0.0.4/dimtown/jk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from utils import Spider
-from bs4 import BeautifulSoup
-import httpx
-import asyncio
+from .utils import Spider
 
 class JK(Spider):
     '''
     `JK图片`获取
     '''
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `dimtown_spider-0.0.3/dimtown/lolita.py` & `dimtown_spider-0.0.4/dimtown/lolita.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from utils import Spider
-from bs4 import BeautifulSoup
-import httpx
-import asyncio
+from .utils import Spider
 
 class Lolita(Spider):
     '''
     `Lolita图片`获取
     '''
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `dimtown_spider-0.0.3/dimtown/pcpic.py` & `dimtown_spider-0.0.4/dimtown/pcpic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from utils import Spider
-from bs4 import BeautifulSoup
-import httpx
-import asyncio
+from .utils import Spider
 
 class PcPic(Spider):
     '''
     `pc壁纸`获取
     '''
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `dimtown_spider-0.0.3/dimtown/phonepic.py` & `dimtown_spider-0.0.4/dimtown/phonepic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-from utils import Spider
-from bs4 import BeautifulSoup
-import httpx
-import asyncio
-try:
-    import ujson as json
-except ModuleNotFoundError:
-    import json
-import os
-import re
+from .utils import Spider
 
 class PhonePic(Spider):
     '''
     `手机壁纸`获取
     '''
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `dimtown_spider-0.0.3/dimtown/utils.py` & `dimtown_spider-0.0.4/dimtown/utils.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.3/PKG-INFO` & `dimtown_spider-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimtown-spider
-Version: 0.0.3
+Version: 0.0.4
 Summary: A spider for https://dimtown.com
 Author: divandia
 Author-email: 106718176+Cvandia@users.noreply.github.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

