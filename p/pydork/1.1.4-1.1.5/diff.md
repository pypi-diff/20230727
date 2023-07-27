# Comparing `tmp/pydork-1.1.4.tar.gz` & `tmp/pydork-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydork-1.1.4.tar", last modified: Thu Jul 27 08:27:36 2023, max compression
+gzip compressed data, was "pydork-1.1.5.tar", last modified: Thu Jul 27 11:17:59 2023, max compression
```

## Comparing `pydork-1.1.4.tar` & `pydork-1.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-07-27 08:27:36.510560 pydork-1.1.4/
--rw-r--r--   0 uesugi     (501) staff       (20)     1065 2022-02-10 07:00:33.000000 pydork-1.1.4/LICENSE
--rw-r--r--   0 uesugi     (501) staff       (20)     8836 2023-07-27 08:27:36.510644 pydork-1.1.4/PKG-INFO
--rw-r--r--   0 uesugi     (501) staff       (20)     7974 2023-07-10 10:10:56.000000 pydork-1.1.4/README.md
--rw-r--r--   0 uesugi     (501) staff       (20)     8179 2022-02-13 15:58:36.000000 pydork-1.1.4/README.rst
-drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-07-27 08:27:36.503940 pydork-1.1.4/completion/
--rw-r--r--   0 uesugi     (501) staff       (20)     1808 2022-02-10 07:00:33.000000 pydork-1.1.4/completion/_pydork
--rwxr-xr-x   0 uesugi     (501) staff       (20)      301 2022-02-10 07:00:33.000000 pydork-1.1.4/completion/pydork-completion.bash
-drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-07-27 08:27:36.509430 pydork-1.1.4/pydork/
--rwxr-xr-x   0 uesugi     (501) staff       (20)     9192 2023-07-17 07:42:24.000000 pydork-1.1.4/pydork/__init__.py
--rw-r--r--   0 uesugi     (501) staff       (20)     7668 2023-02-17 02:51:20.000000 pydork-1.1.4/pydork/common.py
--rw-r--r--   0 uesugi     (501) staff       (20)    18957 2023-07-17 07:37:13.000000 pydork-1.1.4/pydork/engine.py
--rw-r--r--   0 uesugi     (501) staff       (20)    11393 2023-07-17 06:44:12.000000 pydork-1.1.4/pydork/engine_baidu.py
--rw-r--r--   0 uesugi     (501) staff       (20)    10344 2023-07-17 06:43:43.000000 pydork-1.1.4/pydork/engine_bing.py
--rw-r--r--   0 uesugi     (501) staff       (20)    31376 2023-07-17 08:01:31.000000 pydork-1.1.4/pydork/engine_common.py
--rw-r--r--   0 uesugi     (501) staff       (20)     8749 2023-07-17 07:02:11.000000 pydork-1.1.4/pydork/engine_duckduckgo.py
--rw-r--r--   0 uesugi     (501) staff       (20)    19011 2023-07-17 08:01:34.000000 pydork-1.1.4/pydork/engine_google.py
--rw-r--r--   0 uesugi     (501) staff       (20)    10255 2023-07-17 07:37:47.000000 pydork-1.1.4/pydork/engine_yahoo.py
--rw-r--r--   0 uesugi     (501) staff       (20)      556 2023-02-17 02:10:09.000000 pydork-1.1.4/pydork/engine_yandex.py
--rw-r--r--   0 uesugi     (501) staff       (20)     5563 2023-07-10 14:22:02.000000 pydork-1.1.4/pydork/messages.py
--rw-r--r--   0 uesugi     (501) staff       (20)     9743 2023-02-13 22:53:01.000000 pydork-1.1.4/pydork/recaptcha.py
--rw-r--r--   0 uesugi     (501) staff       (20)    12800 2023-07-17 06:45:42.000000 pydork-1.1.4/pydork/sub_commands.py
--rw-r--r--   0 uesugi     (501) staff       (20)    14791 2023-02-13 22:52:45.000000 pydork-1.1.4/pydork/test_engine.py
--rw-r--r--   0 uesugi     (501) staff       (20)    14893 2023-02-13 22:52:49.000000 pydork-1.1.4/pydork/test_engine_selenium.py
-drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-07-27 08:27:36.510424 pydork-1.1.4/pydork.egg-info/
--rw-r--r--   0 uesugi     (501) staff       (20)     8836 2023-07-27 08:27:36.000000 pydork-1.1.4/pydork.egg-info/PKG-INFO
--rw-r--r--   0 uesugi     (501) staff       (20)      618 2023-07-27 08:27:36.000000 pydork-1.1.4/pydork.egg-info/SOURCES.txt
--rw-r--r--   0 uesugi     (501) staff       (20)        1 2023-07-27 08:27:36.000000 pydork-1.1.4/pydork.egg-info/dependency_links.txt
--rw-r--r--   0 uesugi     (501) staff       (20)       39 2023-07-27 08:27:36.000000 pydork-1.1.4/pydork.egg-info/entry_points.txt
--rw-r--r--   0 uesugi     (501) staff       (20)      216 2023-07-27 08:27:36.000000 pydork-1.1.4/pydork.egg-info/requires.txt
--rw-r--r--   0 uesugi     (501) staff       (20)        7 2023-07-27 08:27:36.000000 pydork-1.1.4/pydork.egg-info/top_level.txt
--rw-r--r--   0 uesugi     (501) staff       (20)      111 2023-07-27 08:27:36.510994 pydork-1.1.4/setup.cfg
--rwxr-xr-x   0 uesugi     (501) staff       (20)     4301 2023-07-27 08:11:23.000000 pydork-1.1.4/setup.py
+drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-07-27 11:17:59.142310 pydork-1.1.5/
+-rw-r--r--   0 uesugi     (501) staff       (20)     1065 2022-02-10 07:00:33.000000 pydork-1.1.5/LICENSE
+-rw-r--r--   0 uesugi     (501) staff       (20)     8836 2023-07-27 11:17:59.142399 pydork-1.1.5/PKG-INFO
+-rw-r--r--   0 uesugi     (501) staff       (20)     7974 2023-07-10 10:10:56.000000 pydork-1.1.5/README.md
+-rw-r--r--   0 uesugi     (501) staff       (20)     8179 2022-02-13 15:58:36.000000 pydork-1.1.5/README.rst
+drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-07-27 11:17:59.136753 pydork-1.1.5/completion/
+-rw-r--r--   0 uesugi     (501) staff       (20)     1808 2022-02-10 07:00:33.000000 pydork-1.1.5/completion/_pydork
+-rwxr-xr-x   0 uesugi     (501) staff       (20)      301 2022-02-10 07:00:33.000000 pydork-1.1.5/completion/pydork-completion.bash
+drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-07-27 11:17:59.141322 pydork-1.1.5/pydork/
+-rwxr-xr-x   0 uesugi     (501) staff       (20)     9192 2023-07-17 07:42:24.000000 pydork-1.1.5/pydork/__init__.py
+-rw-r--r--   0 uesugi     (501) staff       (20)     7668 2023-02-17 02:51:20.000000 pydork-1.1.5/pydork/common.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    18958 2023-07-27 11:08:25.000000 pydork-1.1.5/pydork/engine.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    11393 2023-07-17 06:44:12.000000 pydork-1.1.5/pydork/engine_baidu.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    11282 2023-07-27 10:54:27.000000 pydork-1.1.5/pydork/engine_bing.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    31376 2023-07-17 08:01:31.000000 pydork-1.1.5/pydork/engine_common.py
+-rw-r--r--   0 uesugi     (501) staff       (20)     8749 2023-07-27 10:22:34.000000 pydork-1.1.5/pydork/engine_duckduckgo.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    19011 2023-07-17 08:01:34.000000 pydork-1.1.5/pydork/engine_google.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    10255 2023-07-17 07:37:47.000000 pydork-1.1.5/pydork/engine_yahoo.py
+-rw-r--r--   0 uesugi     (501) staff       (20)      556 2023-02-17 02:10:09.000000 pydork-1.1.5/pydork/engine_yandex.py
+-rw-r--r--   0 uesugi     (501) staff       (20)     5563 2023-07-10 14:22:02.000000 pydork-1.1.5/pydork/messages.py
+-rw-r--r--   0 uesugi     (501) staff       (20)     9743 2023-02-13 22:53:01.000000 pydork-1.1.5/pydork/recaptcha.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    12800 2023-07-27 10:58:20.000000 pydork-1.1.5/pydork/sub_commands.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    14791 2023-02-13 22:52:45.000000 pydork-1.1.5/pydork/test_engine.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    14893 2023-02-13 22:52:49.000000 pydork-1.1.5/pydork/test_engine_selenium.py
+drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-07-27 11:17:59.142186 pydork-1.1.5/pydork.egg-info/
+-rw-r--r--   0 uesugi     (501) staff       (20)     8836 2023-07-27 11:17:59.000000 pydork-1.1.5/pydork.egg-info/PKG-INFO
+-rw-r--r--   0 uesugi     (501) staff       (20)      618 2023-07-27 11:17:59.000000 pydork-1.1.5/pydork.egg-info/SOURCES.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)        1 2023-07-27 11:17:59.000000 pydork-1.1.5/pydork.egg-info/dependency_links.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)       39 2023-07-27 11:17:59.000000 pydork-1.1.5/pydork.egg-info/entry_points.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)      216 2023-07-27 11:17:59.000000 pydork-1.1.5/pydork.egg-info/requires.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)        7 2023-07-27 11:17:59.000000 pydork-1.1.5/pydork.egg-info/top_level.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)      111 2023-07-27 11:17:59.142733 pydork-1.1.5/setup.cfg
+-rwxr-xr-x   0 uesugi     (501) staff       (20)     4301 2023-07-27 09:57:42.000000 pydork-1.1.5/setup.py
```

### Comparing `pydork-1.1.4/LICENSE` & `pydork-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/PKG-INFO` & `pydork-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydork
-Version: 1.1.4
+Version: 1.1.5
 Summary: Scraping and listing text and image searches on Google, Bing, DuckDuckGo, Baidu, Yahoo japan.
 Home-page: https://github.com/blacknon/pydork
 Author: blacknon
 Author-email: blacknon@orebibou.com
 Maintainer: blacknon
 Maintainer-email: blacknon@orebibou.com
 License: MIT License
```

### Comparing `pydork-1.1.4/README.md` & `pydork-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/README.rst` & `pydork-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/completion/_pydork` & `pydork-1.1.5/completion/_pydork`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/__init__.py` & `pydork-1.1.5/pydork/__init__.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/common.py` & `pydork-1.1.5/pydork/common.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/engine.py` & `pydork-1.1.5/pydork/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,15 +331,15 @@
             sc = Color(self.ENGINE.COLOR)
             header = sc.out(header)
         self.MESSAGE.set_header(header)
 
         # ENGINEへMessage()を渡す
         self.ENGINE.set_messages(self.MESSAGE)
 
-        if self.ENGINE.LANG != "" or self.ENGINE.LOCALE != "":
+        if self.ENGINE.LANG == "" and self.ENGINE.LOCALE == "":
             self.set_lang()
 
         # メッセージ出力（コマンド実行時のみ）
         colored_keyword = self.ENGINE.MESSAGE.ENGINE_COLOR.out(keyword)
         self.ENGINE.MESSAGE.print_text(
             "$ENGINE: {} Search: {}".format(
                 search_type.capitalize(), colored_keyword),
```

### Comparing `pydork-1.1.4/pydork/engine_baidu.py` & `pydork-1.1.5/pydork/engine_baidu.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/engine_bing.py` & `pydork-1.1.5/pydork/engine_bing.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,33 +54,52 @@
 
         Returns:
             dict: 検索用url
         """
 
         search_url = ''
 
+        # NOTE:
+        #   2023/07/27にて、queryが以下のように切り替わったため修正
+        #     - `https://www.bing.com/search?q=site%3aorebibou.com&search=%e9%80%81%e4%bf%a1&rdr=1&rdrig=D4B6730A85514F25BAE1E9BDC04F1C28&cc=us&setlang=en`
+        #       ```json
+        #       {
+        #         'q': ['site:orebibou.com'],
+        #         'search': ['送信'],
+        #         'rdr': ['1'],
+        #         'rdrig': ['D4B6730A85514F25BAE1E9BDC04F1C28'],
+        #         'cc': ['us'],
+        #         'setlang': ['en']
+        #       }
+        #       ```
+        #     - `https://www.bing.com/search?q=site%3aorebibou.com&search=%E9%80%81%E4%BF%A1&rdr=1&rdrig=D4B6730A85514F25BAE1E9BDC04F1C28&cc=us&setlang=en&FPIG=B035C5DE50AE4A328CB93C767B02D08B&first=11&FORM=PERE&count=100`
+
         # 検索タイプがtextの場合
         if type == 'text':
             # 検索urlを指定
             search_url = self.SEARCH_URL
 
             # 検索パラメータの設定
             url_param = {
                 'q': keyword,    # 検索キーワード
                 'count': '100',  # 1ページごとの表示件数
-                'go': '検索',
-                'qs': 'ds',
-                'from': 'QBRE',
+                'search': '送信',
+                'rdr': '1',
+                'from': 'PERE',
+                'cc': 'us',
+                'setlang': 'en',
                 'filters': '',   # 期間含めフィルターとして指定するパラメータ
                 'first': ''      # 開始位置
             }
 
             # lang/localeが設定されている場合
-            if self.LANG != '' and self.LOCALE != '':
-                url_param['mkt'] = self.LANG + '-' + self.LOCALE
+            if self.LANG != '':
+                url_param['setlang'] = self.LANG.lower()
+            if self.LOCALE != '':
+                url_param['cc'] = self.LOCALE.lower()
 
             # rangeが設定されている場合
             try:
                 start = self.RANGE_START
                 end = self.RANGE_END
 
                 unix_day = datetime.strptime('1970-01-01', "%Y-%m-%d")
```

### Comparing `pydork-1.1.4/pydork/engine_common.py` & `pydork-1.1.5/pydork/engine_common.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/engine_duckduckgo.py` & `pydork-1.1.5/pydork/engine_duckduckgo.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/engine_google.py` & `pydork-1.1.5/pydork/engine_google.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/engine_yahoo.py` & `pydork-1.1.5/pydork/engine_yahoo.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/engine_yandex.py` & `pydork-1.1.5/pydork/engine_yandex.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/messages.py` & `pydork-1.1.5/pydork/messages.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/recaptcha.py` & `pydork-1.1.5/pydork/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/sub_commands.py` & `pydork-1.1.5/pydork/sub_commands.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/test_engine.py` & `pydork-1.1.5/pydork/test_engine.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork/test_engine_selenium.py` & `pydork-1.1.5/pydork/test_engine_selenium.py`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/pydork.egg-info/PKG-INFO` & `pydork-1.1.5/pydork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydork
-Version: 1.1.4
+Version: 1.1.5
 Summary: Scraping and listing text and image searches on Google, Bing, DuckDuckGo, Baidu, Yahoo japan.
 Home-page: https://github.com/blacknon/pydork
 Author: blacknon
 Author-email: blacknon@orebibou.com
 Maintainer: blacknon
 Maintainer-email: blacknon@orebibou.com
 License: MIT License
```

### Comparing `pydork-1.1.4/pydork.egg-info/SOURCES.txt` & `pydork-1.1.5/pydork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydork-1.1.4/setup.py` & `pydork-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,16 @@
     data_files = []
     data_files.append((loc['bash'], files['bash']))
     data_files.append((loc['zsh'], files['zsh']))
     return data_files
 
 
 name = 'pydork'
-version = '1.1.4'
-release = '1.1.4'
+version = '1.1.5'
+release = '1.1.5'
 
 if __name__ == "__main__":
     setuptools.setup(
         name=name,
         version=version,
         author='blacknon',
         author_email='blacknon@orebibou.com',
```

