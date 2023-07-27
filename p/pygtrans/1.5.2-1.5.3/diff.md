# Comparing `tmp/pygtrans-1.5.2.tar.gz` & `tmp/pygtrans-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygtrans-1.5.2.tar", last modified: Fri Apr 28 00:54:04 2023, max compression
+gzip compressed data, was "pygtrans-1.5.3.tar", last modified: Thu Jul 27 08:30:48 2023, max compression
```

## Comparing `pygtrans-1.5.2.tar` & `pygtrans-1.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:54:04.366644 pygtrans-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 00:53:56.000000 pygtrans-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 00:53:56.000000 pygtrans-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-28 00:54:04.366644 pygtrans-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-28 00:53:56.000000 pygtrans-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-28 00:53:56.000000 pygtrans-1.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 00:53:56.000000 pygtrans-1.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:54:04.370644 pygtrans-1.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:54:04.362645 pygtrans-1.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:54:04.366644 pygtrans-1.5.2/src/pygtrans/
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-28 00:53:56.000000 pygtrans-1.5.2/src/pygtrans/ApiKeyTranslate.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-28 00:53:56.000000 pygtrans-1.5.2/src/pygtrans/DetectResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-28 00:53:56.000000 pygtrans-1.5.2/src/pygtrans/LanguageResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-28 00:53:56.000000 pygtrans-1.5.2/src/pygtrans/Null.py
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-04-28 00:53:56.000000 pygtrans-1.5.2/src/pygtrans/Translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-28 00:53:56.000000 pygtrans-1.5.2/src/pygtrans/TranslateResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-28 00:54:03.000000 pygtrans-1.5.2/src/pygtrans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 00:53:56.000000 pygtrans-1.5.2/src/pygtrans/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:54:04.366644 pygtrans-1.5.2/src/pygtrans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-28 00:54:04.000000 pygtrans-1.5.2/src/pygtrans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-28 00:54:04.000000 pygtrans-1.5.2/src/pygtrans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:54:04.000000 pygtrans-1.5.2/src/pygtrans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 00:54:04.000000 pygtrans-1.5.2/src/pygtrans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 00:54:04.000000 pygtrans-1.5.2/src/pygtrans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 00:54:04.000000 pygtrans-1.5.2/src/pygtrans.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:30:48.758158 pygtrans-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-27 08:30:38.000000 pygtrans-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 08:30:38.000000 pygtrans-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-27 08:30:48.758158 pygtrans-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-27 08:30:38.000000 pygtrans-1.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-27 08:30:38.000000 pygtrans-1.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 08:30:38.000000 pygtrans-1.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 08:30:48.758158 pygtrans-1.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:30:48.754158 pygtrans-1.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:30:48.758158 pygtrans-1.5.3/src/pygtrans/
+-rw-r--r--   0 runner    (1001) docker     (123)     9883 2023-07-27 08:30:38.000000 pygtrans-1.5.3/src/pygtrans/ApiKeyTranslate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-27 08:30:38.000000 pygtrans-1.5.3/src/pygtrans/DetectResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-27 08:30:38.000000 pygtrans-1.5.3/src/pygtrans/LanguageResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-27 08:30:38.000000 pygtrans-1.5.3/src/pygtrans/Null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-07-27 08:30:38.000000 pygtrans-1.5.3/src/pygtrans/Translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-27 08:30:38.000000 pygtrans-1.5.3/src/pygtrans/TranslateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-27 08:30:47.000000 pygtrans-1.5.3/src/pygtrans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 08:30:38.000000 pygtrans-1.5.3/src/pygtrans/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:30:48.758158 pygtrans-1.5.3/src/pygtrans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-27 08:30:48.000000 pygtrans-1.5.3/src/pygtrans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-27 08:30:48.000000 pygtrans-1.5.3/src/pygtrans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:30:48.000000 pygtrans-1.5.3/src/pygtrans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 08:30:48.000000 pygtrans-1.5.3/src/pygtrans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 08:30:48.000000 pygtrans-1.5.3/src/pygtrans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 08:30:48.000000 pygtrans-1.5.3/src/pygtrans.egg-info/top_level.txt
```

### Comparing `pygtrans-1.5.2/LICENSE` & `pygtrans-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygtrans-1.5.2/PKG-INFO` & `pygtrans-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygtrans
-Version: 1.5.2
+Version: 1.5.3
 Summary: Google Translate, support APIKEY
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/pygtrans
 Project-URL: Homepage, https://github.com/foyoux/pygtrans
 Project-URL: Bug Tracker, https://github.com/foyoux/pygtrans/issues
 Project-URL: Documentation, https://pygtrans.readthedocs.io/zh_CN/latest/
 Keywords: pygtrans,google,translate,apikey,text,html,google.cn,google.com
```

### Comparing `pygtrans-1.5.2/README.md` & `pygtrans-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pygtrans-1.5.2/pyproject.toml` & `pygtrans-1.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygtrans-1.5.2/src/pygtrans/ApiKeyTranslate.py` & `pygtrans-1.5.3/src/pygtrans/ApiKeyTranslate.py`

 * *Files 12% similar despite different names*

```diff
@@ -85,110 +85,116 @@
 
     def __init__(
             self, api_key: str,
             target: str = 'zh-CN',
             source: str = None,
             fmt: str = 'html',
             model: str = 'nmt',
-            proxies: Dict = None
+            proxies: Dict = None,
+            timeout=None
     ):
         self.api_key = api_key
         self.target = target
+        self.timeout = timeout
         if source == 'auto':
             # '不提供' 替换 'auto'，'auto' 会导致 400，参数错误。
             source = None
         self.source = source
         self.fmt = fmt
         self.model = model
         self.session = requests.Session()
 
         if proxies is not None:
             self.session.trust_env = False
             self.session.proxies = proxies
 
-    def languages(self, target: str = None, model: str = None) -> Union[List[LanguageResponse], Null]:
+    def languages(self, target: str = None, model: str = None, timeout=...) -> Union[List[LanguageResponse], Null]:
         """语言支持列表"""
         if target is None:
             target = self.target
         if model is None:
             model = self.model
-        response = self.session.get(self._LANGUAGE_URL, params={'key': self.api_key, 'target': target, 'model': model})
+        if timeout is ...:
+            timeout = self.timeout
+        response = self.session.get(self._LANGUAGE_URL, params={'key': self.api_key, 'target': target, 'model': model},
+                                    timeout=timeout)
         if response.status_code == 200:
             return [LanguageResponse(**i) for i in response.json()['data']['languages']]
         return Null(response)
 
     @overload
-    def detect(self, q: str) -> DetectResponse:
+    def detect(self, q: str, timeout=...) -> DetectResponse:
         """..."""
 
     @overload
-    def detect(self, q: List[str]) -> List[DetectResponse]:
+    def detect(self, q: List[str], timeout=...) -> List[DetectResponse]:
         """..."""
 
-    def detect(self, q: Union[str, List[str]]) -> Union[DetectResponse, List[DetectResponse], Null]:
+    def detect(self, q: Union[str, List[str]], timeout=...) -> Union[DetectResponse, List[DetectResponse], Null]:
         """语言检测, 支持批量
 
         :param q: 字符串或字符串列表
+        :param timeout: 超时时间， int | None
         :return: 成功则返回: :class:`pygtrans.TranslateResponse.DetectResponse` 对象,
             或 :class:`pygtrans.TranslateResponse.DetectResponse` 对象列表, 这取决于 `参数: q` 是字符串还是字符串列表.
             失败则返回 :class:`pygtrans.Null.Null` 对象
 
         基本用法:
             >>> from pygtrans import ApiKeyTranslate
             >>> client = ApiKeyTranslate(api_key='<api_key>')
             >>> d1 = client.detect('Hello')
             >>> d1.language
             'en'
             >>> assert isinstance(client.detect(['Hello', 'Google']), list)
 
         """
+        if timeout is ...:
+            timeout = self.timeout
         ll = []
         for ql in split_list(q):
             for qli in split_list_by_content_size(ql):
                 for i in range(1, 4):
-                    response = self.session.post(self._DETECT_URL, params={
-                        'key': self.api_key
-                    }, data={
-                        'q': qli
-                    })
+                    response = self.session.post(self._DETECT_URL, params={'key': self.api_key}, data={'q': qli},
+                                                 timeout=timeout)
                     if response.status_code == 429:
                         time.sleep(5 * i)
                         continue
                     break
                 # noinspection PyUnboundLocalVariable
                 if response.status_code != 200:
                     return Null(response)
                 ll.extend([DetectResponse(**i[0]) for i in response.json()['data']['detections']])
         if isinstance(q, str):
             return ll[0]
         return ll
 
     @overload
     def translate(
-            self, q: str, target: str = None, source: str = None, fmt: str = None, model: str = None
+            self, q: str, target: str = None, source: str = None, fmt: str = None, model: str = None, timeout=...
     ) -> TranslateResponse:
         """..."""
 
     @overload
     def translate(
-            self, q: List[str], target: str = None, source: str = None, fmt: str = None, model: str = None
+            self, q: List[str], target: str = None, source: str = None, fmt: str = None, model: str = None, timeout=...
     ) -> List[TranslateResponse]:
         """..."""
 
     def translate(
             self, q: Union[str, List[str]], target: str = None, source: str = None, fmt: str = None,
-            model: str = None
+            model: str = None, timeout=...
     ) -> Union[TranslateResponse, List[TranslateResponse], Null]:
         """文本翻译, 支持批量
 
         :param q: str: 字符串或字符串列表
         :param target: str: (可选)  目标语言, 默认: ``self.target``, :doc:`查看支持列表 <target>`
         :param source: str: (可选)  源语言, 默认: ``self.source``, :doc:`查看支持列表 <source>`
         :param fmt: str: (可选) 文本格式, ``text`` | ``html``, 默认: ``self.format``
         :param model: str: (可选) 翻译模型, ``nmt`` | ``pbmt``, 默认: ``self.model``
+        :param timeout: 超时时间， int | None
         :return: 成功则返回: :class:`pygtrans.TranslateResponse.TranslateResponse` 对象,
             或 :class:`pygtrans.TranslateResponse.TranslateResponse` 对象列表, 这取决于 `参数: q` 是字符串还是字符串列表.
             失败则返回 :class:`pygtrans.Null.Null` 对象
 
         .. 谷歌API调用限制
             最大并发量: 128
             最大请求体大小: 102400 bytes
@@ -212,22 +218,23 @@
             source = None
         if source is None:
             source = self.source
         if fmt is None:
             fmt = self.fmt
         if model is None:
             model = self.model
-
+        if timeout is ...:
+            timeout = self.timeout
         ll = []
         for ql in split_list(q):
             for qli in split_list_by_content_size(ql):
                 for i in range(1, 4):
                     response = self.session.post(self._BASE_URL, params={
                         'key': self.api_key, 'target': target, 'source': source, 'format': fmt, 'model': model
-                    }, data={'q': qli})
+                    }, data={'q': qli}, timeout=timeout)
                     if response.status_code == 429:
                         time.sleep(5 * i)
                         continue
                     break
                 # noinspection PyUnboundLocalVariable
                 if response.status_code != 200:
                     return Null(response)
```

### Comparing `pygtrans-1.5.2/src/pygtrans/DetectResponse.py` & `pygtrans-1.5.3/src/pygtrans/DetectResponse.py`

 * *Files identical despite different names*

### Comparing `pygtrans-1.5.2/src/pygtrans/Translate.py` & `pygtrans-1.5.3/src/pygtrans/Translate.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,19 +46,21 @@
     def __init__(
             self,
             target: str = 'zh-CN',
             source: str = 'auto',
             fmt='html',
             user_agent: str = None,
             domain: str = 'com',
-            proxies: Dict = None
+            proxies: Dict = None,
+            timeout: int = None
     ):
         self.target = target
         self.source = source
         self.fmt = fmt
+        self.timeout = timeout
 
         if user_agent is None:
             user_agent = (
                 f'GoogleTranslate/6.{random.randint(10, 100)}.0.06.{random.randint(111111111, 999999999)}'
                 ' (Linux; U; Android {random.randint(5, 11)}; {base64.b64encode(str(random.random())['
                 '2:].encode()).decode()}) '
             )
@@ -73,62 +75,67 @@
         self.TRANSLATE_URL: str = f'{self.BASE_URL}/translate_a/t'
         self.TTS_URL: str = f'{self.BASE_URL}/translate_tts'
 
         if proxies is not None:
             self.session.trust_env = False
             self.session.proxies = proxies
 
-    def detect(self, q: str) -> Union[DetectResponse, Null]:
+    def detect(self, q: str, timeout=...) -> Union[DetectResponse, Null]:
         """语言检测
 
         :param q: 需要检测的内容, 不支持批量, 如需批量, 请参阅: :func:`translate_and_detect`.
+        :param timeout: 超时时间， int | None
         :return: 成功则返回 :class:`pygtrans.DetectResponse.DetectResponse` 对象,
             失败则返回 :class:`pygtrans.Null.Null` 对象
 
         基本用法:
             >>> from pygtrans import Translate
             >>> client = Translate(proxies={'http': 'http://localhost:10809', 'https': 'http://localhost:10809'})
             >>> d = client.detect('こんにちは')
             >>> assert d.language == 'ja'
         """
+        if timeout is ...:
+            timeout = self.timeout
         for i in range(1, 4):
             response = self.session.post(
                 self.DETECT_URL,
                 params={'dj': 1, 'sl': 'auto', 'ie': 'UTF-8', 'oe': 'UTF-8', 'client': 'at'},
-                data={'q': q}
+                data={'q': q}, timeout=timeout
             )
             if response.status_code == 429:
                 time.sleep(5 * i)
                 continue
             break
         # noinspection PyUnboundLocalVariable
         if response.status_code != 200:
             return Null(response)
         rt = response.json()
         return DetectResponse(language=rt['src'], confidence=rt['confidence'])
 
     @overload
-    def translate(self, q: str, target: str = None, source: str = None, fmt: str = None, ) -> TranslateResponse:
+    def translate(self, q: str, target: str = None, source: str = None, fmt: str = None,
+                  timeout=...) -> TranslateResponse:
         """..."""
 
     @overload
     def translate(
-            self, q: List[str], target: str = None, source: str = None, fmt: str = None
+            self, q: List[str], target: str = None, source: str = None, fmt: str = None, timeout=...
     ) -> List[TranslateResponse]:
         """..."""
 
     def translate(
-            self, q: Union[str, List[str]], target: str = None, source: str = None, fmt: str = None
+            self, q: Union[str, List[str]], target: str = None, source: str = None, fmt: str = None, timeout=...
     ) -> Union[TranslateResponse, List[TranslateResponse], Null]:
         """翻译文本, 支持批量, 支持 html
 
         :param q: str: 字符串或字符串列表
         :param target: str: (可选)  目标语言, 默认: ``self.target``, :doc:`查看支持列表 <target>`
         :param source: str: (可选)  源语言, 默认: ``self.source``, :doc:`查看支持列表 <source>`
         :param fmt: str: (可选) 文本格式, ``text`` | ``html``, 默认: ``self.format``
+        :param timeout: 超时时间， int | None
         :return: 成功则返回: :class:`pygtrans.TranslateResponse.TranslateResponse` 对象,
             或 :class:`pygtrans.TranslateResponse.TranslateResponse` 对象列表, 这取决于 `参数: q` 是字符串还是字符串列表.
             失败则返回 :class:`pygtrans.Null.Null` 对象
 
         基本用法:
             >>> from pygtrans import Translate
             >>> client = Translate(proxies={'http': 'http://localhost:10809', 'https': 'http://localhost:10809'})
@@ -141,75 +148,85 @@
             Batch test
             Batch translation
         """
 
         if not q:
             return []
 
+        if timeout is ...:
+            timeout = self.timeout
+
         if isinstance(q, str):
             if q == '':
                 return TranslateResponse('')
 
         for i in range(1, 4):
-            response = self.__translate(q=q, target=target, source=source, fmt=fmt, v='1.0')
+            response = self.__translate(q=q, target=target, source=source, fmt=fmt, v='1.0', timeout=timeout)
             if response.status_code == 429:
                 time.sleep(5 * i)
                 continue
             break
         # noinspection PyUnboundLocalVariable
         if response.status_code == 200:
             ll = [TranslateResponse(translatedText=i) for i in response.json()]
             if isinstance(q, str):
                 return ll[0]
             return ll
 
         return Null(response)
 
     def __translate(
-            self, q: Union[str, List[str]], target: str = None, source: str = None, fmt: str = None, v: str = None
+            self, q: Union[str, List[str]], target: str = None, source: str = None, fmt: str = None, v: str = None,
+            timeout=...
     ):
         if target is None:
             target = self.target
         if source is None:
             source = self.source
         if fmt is None:
             fmt = self.fmt
+        if timeout is ...:
+            timeout = self.timeout
         for i in range(1, 4):
             response = self.session.post(
                 self.TRANSLATE_URL,
                 params={'tl': target, 'sl': source, 'ie': 'UTF-8', 'oe': 'UTF-8', 'client': 'at', 'dj': '1',
                         'format': fmt, 'v': v},
-                data={'q': q}
+                data={'q': q}, timeout=timeout
             )
             if response.status_code == 429:
                 time.sleep(5 * i)
                 continue
             break
         # noinspection PyUnboundLocalVariable
         return response
 
-    def tts(self, q: str, target: str = None) -> Union[bytes, Null]:
+    def tts(self, q: str, target: str = None, timeout=...) -> Union[bytes, Null]:
         """语音: 实验性功能
 
         :param q: 只支持短语字符串
         :param target: 目标语言
+        :param timeout: 超时时间， int | None
         :return: 返回二进制数据, 需要自行写入文件, MP3
         """
         if target is None:
             target = self.target
 
+        if timeout is ...:
+            timeout = self.timeout
+
         for i in range(1, 4):
             response = self.session.get(
                 self.TTS_URL,
                 params={
                     'ie': 'UTF-8',
                     'client': 'at',
                     'tl': target,
                     'q': q
-                })
+                }, timeout=timeout)
             if response.status_code == 429:
                 time.sleep(5 * i)
                 continue
             break
         # noinspection PyUnboundLocalVariable
         if response.status_code == 200:
             return response.content
```

### Comparing `pygtrans-1.5.2/src/pygtrans/TranslateResponse.py` & `pygtrans-1.5.3/src/pygtrans/TranslateResponse.py`

 * *Files identical despite different names*

### Comparing `pygtrans-1.5.2/src/pygtrans/__init__.py` & `pygtrans-1.5.3/src/pygtrans/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .Null import Null
 from .Translate import Translate
 from .TranslateResponse import TranslateResponse
 
 __title__ = 'pygtrans'
 __description__ = 'Google Translate, support APIKEY'
 __url__ = 'https://github.com/foyoux/pygtrans'
-__version__ = '1.5.2'
+__version__ = '1.5.3'
 __author__ = 'foyoux'
 __author_email__ = 'yimi.0822@qq.com'
 __license__ = 'GPL-3.0'
 __copyright__ = f'Copyright 2021 {__author__}'
 __ide__ = 'PyCharm - https://www.jetbrains.com/pycharm/'
 
 __all__ = [
```

### Comparing `pygtrans-1.5.2/src/pygtrans.egg-info/PKG-INFO` & `pygtrans-1.5.3/src/pygtrans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygtrans
-Version: 1.5.2
+Version: 1.5.3
 Summary: Google Translate, support APIKEY
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/pygtrans
 Project-URL: Homepage, https://github.com/foyoux/pygtrans
 Project-URL: Bug Tracker, https://github.com/foyoux/pygtrans/issues
 Project-URL: Documentation, https://pygtrans.readthedocs.io/zh_CN/latest/
 Keywords: pygtrans,google,translate,apikey,text,html,google.cn,google.com
```

