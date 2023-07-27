# Comparing `tmp/pydork-1.1.2.tar.gz` & `tmp/pydork-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydork-1.1.2.tar", last modified: Tue Jun 28 12:39:49 2022, max compression
+gzip compressed data, was "pydork-1.1.4.tar", last modified: Thu Jul 27 08:27:36 2023, max compression
```

## Comparing `pydork-1.1.2.tar` & `pydork-1.1.4.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2022-06-28 12:39:49.254720 pydork-1.1.2/
--rw-r--r--   0 uesugi     (501) staff       (20)     1065 2022-02-10 07:00:33.000000 pydork-1.1.2/LICENSE
--rw-r--r--   0 uesugi     (501) staff       (20)     8785 2022-06-28 12:39:49.254949 pydork-1.1.2/PKG-INFO
--rw-r--r--   0 uesugi     (501) staff       (20)     7954 2022-06-28 12:38:01.000000 pydork-1.1.2/README.md
--rw-r--r--   0 uesugi     (501) staff       (20)     8179 2022-02-13 15:58:36.000000 pydork-1.1.2/README.rst
-drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2022-06-28 12:39:49.227737 pydork-1.1.2/completion/
--rw-r--r--   0 uesugi     (501) staff       (20)     1808 2022-02-10 07:00:33.000000 pydork-1.1.2/completion/_pydork
--rwxr-xr-x   0 uesugi     (501) staff       (20)      301 2022-02-10 07:00:33.000000 pydork-1.1.2/completion/pydork-completion.bash
-drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2022-06-28 12:39:49.249085 pydork-1.1.2/pydork/
--rwxr-xr-x   0 uesugi     (501) staff       (20)     9581 2022-06-28 12:38:01.000000 pydork-1.1.2/pydork/__init__.py
--rw-r--r--   0 uesugi     (501) staff       (20)     5771 2022-06-22 14:02:46.000000 pydork-1.1.2/pydork/common.py
--rw-r--r--   0 uesugi     (501) staff       (20)    17407 2022-06-28 12:38:01.000000 pydork-1.1.2/pydork/engine.py
--rw-r--r--   0 uesugi     (501) staff       (20)    11229 2022-06-28 12:38:01.000000 pydork-1.1.2/pydork/engine_baidu.py
--rw-r--r--   0 uesugi     (501) staff       (20)    10180 2022-06-28 12:38:01.000000 pydork-1.1.2/pydork/engine_bing.py
--rw-r--r--   0 uesugi     (501) staff       (20)    28835 2022-06-28 12:38:01.000000 pydork-1.1.2/pydork/engine_common.py
--rw-r--r--   0 uesugi     (501) staff       (20)     8476 2022-05-04 10:46:27.000000 pydork-1.1.2/pydork/engine_duckduckgo.py
--rw-r--r--   0 uesugi     (501) staff       (20)    17557 2022-05-04 10:46:27.000000 pydork-1.1.2/pydork/engine_google.py
--rw-r--r--   0 uesugi     (501) staff       (20)     9951 2022-05-04 10:46:27.000000 pydork-1.1.2/pydork/engine_yahoo.py
--rw-r--r--   0 uesugi     (501) staff       (20)     9594 2022-02-13 11:13:20.000000 pydork-1.1.2/pydork/recaptcha.py
--rw-r--r--   0 uesugi     (501) staff       (20)    12105 2022-06-28 12:38:01.000000 pydork-1.1.2/pydork/subcommands.py
--rw-r--r--   0 uesugi     (501) staff       (20)    14642 2022-05-04 10:46:27.000000 pydork-1.1.2/pydork/test_engine.py
--rw-r--r--   0 uesugi     (501) staff       (20)    14744 2022-05-04 10:46:27.000000 pydork-1.1.2/pydork/test_engine_selenium.py
-drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2022-06-28 12:39:49.253816 pydork-1.1.2/pydork.egg-info/
--rw-r--r--   0 uesugi     (501) staff       (20)     8785 2022-06-28 12:39:47.000000 pydork-1.1.2/pydork.egg-info/PKG-INFO
--rw-r--r--   0 uesugi     (501) staff       (20)      574 2022-06-28 12:39:49.000000 pydork-1.1.2/pydork.egg-info/SOURCES.txt
--rw-r--r--   0 uesugi     (501) staff       (20)        1 2022-06-28 12:39:48.000000 pydork-1.1.2/pydork.egg-info/dependency_links.txt
--rw-r--r--   0 uesugi     (501) staff       (20)       39 2022-06-28 12:39:48.000000 pydork-1.1.2/pydork.egg-info/entry_points.txt
--rw-r--r--   0 uesugi     (501) staff       (20)      209 2022-06-28 12:39:48.000000 pydork-1.1.2/pydork.egg-info/requires.txt
--rw-r--r--   0 uesugi     (501) staff       (20)        7 2022-06-28 12:39:48.000000 pydork-1.1.2/pydork.egg-info/top_level.txt
--rw-r--r--   0 uesugi     (501) staff       (20)      111 2022-06-28 12:39:49.255774 pydork-1.1.2/setup.cfg
--rwxr-xr-x   0 uesugi     (501) staff       (20)     4091 2022-06-28 12:38:01.000000 pydork-1.1.2/setup.py
+drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-07-27 08:27:36.510560 pydork-1.1.4/
+-rw-r--r--   0 uesugi     (501) staff       (20)     1065 2022-02-10 07:00:33.000000 pydork-1.1.4/LICENSE
+-rw-r--r--   0 uesugi     (501) staff       (20)     8836 2023-07-27 08:27:36.510644 pydork-1.1.4/PKG-INFO
+-rw-r--r--   0 uesugi     (501) staff       (20)     7974 2023-07-10 10:10:56.000000 pydork-1.1.4/README.md
+-rw-r--r--   0 uesugi     (501) staff       (20)     8179 2022-02-13 15:58:36.000000 pydork-1.1.4/README.rst
+drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-07-27 08:27:36.503940 pydork-1.1.4/completion/
+-rw-r--r--   0 uesugi     (501) staff       (20)     1808 2022-02-10 07:00:33.000000 pydork-1.1.4/completion/_pydork
+-rwxr-xr-x   0 uesugi     (501) staff       (20)      301 2022-02-10 07:00:33.000000 pydork-1.1.4/completion/pydork-completion.bash
+drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-07-27 08:27:36.509430 pydork-1.1.4/pydork/
+-rwxr-xr-x   0 uesugi     (501) staff       (20)     9192 2023-07-17 07:42:24.000000 pydork-1.1.4/pydork/__init__.py
+-rw-r--r--   0 uesugi     (501) staff       (20)     7668 2023-02-17 02:51:20.000000 pydork-1.1.4/pydork/common.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    18957 2023-07-17 07:37:13.000000 pydork-1.1.4/pydork/engine.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    11393 2023-07-17 06:44:12.000000 pydork-1.1.4/pydork/engine_baidu.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    10344 2023-07-17 06:43:43.000000 pydork-1.1.4/pydork/engine_bing.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    31376 2023-07-17 08:01:31.000000 pydork-1.1.4/pydork/engine_common.py
+-rw-r--r--   0 uesugi     (501) staff       (20)     8749 2023-07-17 07:02:11.000000 pydork-1.1.4/pydork/engine_duckduckgo.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    19011 2023-07-17 08:01:34.000000 pydork-1.1.4/pydork/engine_google.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    10255 2023-07-17 07:37:47.000000 pydork-1.1.4/pydork/engine_yahoo.py
+-rw-r--r--   0 uesugi     (501) staff       (20)      556 2023-02-17 02:10:09.000000 pydork-1.1.4/pydork/engine_yandex.py
+-rw-r--r--   0 uesugi     (501) staff       (20)     5563 2023-07-10 14:22:02.000000 pydork-1.1.4/pydork/messages.py
+-rw-r--r--   0 uesugi     (501) staff       (20)     9743 2023-02-13 22:53:01.000000 pydork-1.1.4/pydork/recaptcha.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    12800 2023-07-17 06:45:42.000000 pydork-1.1.4/pydork/sub_commands.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    14791 2023-02-13 22:52:45.000000 pydork-1.1.4/pydork/test_engine.py
+-rw-r--r--   0 uesugi     (501) staff       (20)    14893 2023-02-13 22:52:49.000000 pydork-1.1.4/pydork/test_engine_selenium.py
+drwxr-xr-x   0 uesugi     (501) staff       (20)        0 2023-07-27 08:27:36.510424 pydork-1.1.4/pydork.egg-info/
+-rw-r--r--   0 uesugi     (501) staff       (20)     8836 2023-07-27 08:27:36.000000 pydork-1.1.4/pydork.egg-info/PKG-INFO
+-rw-r--r--   0 uesugi     (501) staff       (20)      618 2023-07-27 08:27:36.000000 pydork-1.1.4/pydork.egg-info/SOURCES.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)        1 2023-07-27 08:27:36.000000 pydork-1.1.4/pydork.egg-info/dependency_links.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)       39 2023-07-27 08:27:36.000000 pydork-1.1.4/pydork.egg-info/entry_points.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)      216 2023-07-27 08:27:36.000000 pydork-1.1.4/pydork.egg-info/requires.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)        7 2023-07-27 08:27:36.000000 pydork-1.1.4/pydork.egg-info/top_level.txt
+-rw-r--r--   0 uesugi     (501) staff       (20)      111 2023-07-27 08:27:36.510994 pydork-1.1.4/setup.cfg
+-rwxr-xr-x   0 uesugi     (501) staff       (20)     4301 2023-07-27 08:11:23.000000 pydork-1.1.4/setup.py
```

### Comparing `pydork-1.1.2/LICENSE` & `pydork-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydork-1.1.2/PKG-INFO` & `pydork-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pydork
-Version: 1.1.2
+Version: 1.1.4
 Summary: Scraping and listing text and image searches on Google, Bing, DuckDuckGo, Baidu, Yahoo japan.
 Home-page: https://github.com/blacknon/pydork
 Author: blacknon
 Author-email: blacknon@orebibou.com
 Maintainer: blacknon
 Maintainer-email: blacknon@orebibou.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 
 PyDork
 ======
 
 Description
```

### Comparing `pydork-1.1.2/README.md` & `pydork-1.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 PyDork
 ======
 
 ## Description
 
-Scraping and listing text and image searches on Google, Bing, DuckDuckGo, Baidu, Yahoo japan.
+Scraping and listing text and image searches on **Google**, **Bing**, **DuckDuckGo**, **Baidu**, **Yahoo japan**.
 
 ## Install
 
 ```bash
 pip install pydork
 ```
```

### Comparing `pydork-1.1.2/README.rst` & `pydork-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `pydork-1.1.2/completion/_pydork` & `pydork-1.1.4/completion/_pydork`

 * *Files identical despite different names*

### Comparing `pydork-1.1.2/pydork/common.py` & `pydork-1.1.4/pydork/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
 
 """common
     * 共通系や雑多な処理を詰め合わせたバルクモジュール.
-
 """
 
 import sys
 import datetime
 
 from string import Template
 
@@ -78,15 +80,15 @@
         return text
 
 
 # Message関連の制御用Class
 class Message:
     """Message
 
-    メッセージの出力を簡易化するためのClass(未完成...).
+    メッセージの出力を簡易化するためのClass.
 
     Examples:
 
     """
 
     def __init__(self):
         # command flag
@@ -152,41 +154,65 @@
 
         # 置換処理を実行
         result = template.safe_substitute(data)
 
         return result
 
     def print_line(self, *text, use_header=True, separator=' ', file=sys.stdout, header=None):
+        """print_line
+
+        メッセージを出力する(行)
+
+        Args:
+            text: メッセージとして出力するテキスト行
+            use_header: `header`で指定しているヘッダーを行頭に表示するかどうか
+            separator: printする際に使用する区切り文字
+            file: 出力先のファイル(デフォルトはstdout)
+            header: ヘッダーとして使用する文字列を指定
+        """
         # headerの生成
         if header is None:
             header = self.HEADER
 
         header = self.replace(header)
 
         # テキストを出力
         if use_header:
             print(header, *text, sep=separator, file=file)
         else:
             print(*text, sep=separator, file=file)
 
     def print_text(self, text, mode='message', use_header=True, separator=' ', file=sys.stdout, header=None):
+        """print_line
+
+        メッセージを出力する(テキスト)
+
+        Args:
+            text: メッセージとして出力するテキスト
+            mode: メッセージの出力モード(`message`, `error`, `warn`, `info`, `debug`)
+            use_header: `header`で指定しているヘッダーを行頭に表示するかどうか
+            separator: printする際に使用する区切り文字
+            file: 出力先のファイル(デフォルトはstdout)
+            header: ヘッダーとして使用する文字列を指定
+        """
         # is_commandが有効のときのみ出力させる
         if not self.IS_COMMAND:
             return
 
         # debug, infoのときは、self.is_debugが有効のときのみ出力
         if mode in ('info', 'debug'):
             # self.is_debugでない場合は出力しない
             if not self.IS_DEBUG:
                 return
 
         # 出力テキストの生成
         text = self.replace(text)
 
         # case
+        text_color: Color = Color(Color.END)
         if mode == 'message':  # modeが `message` のとき
             text_color = Color(Color.WHITE)
 
         elif mode == 'error':
             text_color = Color(Color.RED)
             file = sys.stderr
 
@@ -214,7 +240,30 @@
 
         # テキストの出力
         for line in text.splitlines():
             self.print_line(text_color.out(line),
                             separator=separator, use_header=use_header, file=file, header=header)
 
         return
+
+
+# 渡されたリスト内のdictに`num`を追加する関数
+def set_counter(links: list):
+    """set_counter
+
+    links(list)の要素に`num`キーを追加し、連続した数値を入れていく
+
+    Args:
+        links(list): リンクのリスト. ex) [{'link', 'http://...', 'title': 'hogehoge...'}, {'link': '...', 'title': '...'}, ... ]
+    Returns:
+        result(list):  [{'link', 'http://...', 'title': 'hogehoge...', num: 1}, {'link': '...', 'title': '...', num: 2}, ... ]
+    """
+    # result(list)の生成
+    result = list()
+
+    num = 1
+    for d in links:
+        d["num"] = num
+        num += 1
+        result.append(d)
+
+    return result
```

### Comparing `pydork-1.1.2/pydork/engine.py` & `pydork-1.1.4/pydork/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
+
+# TODO: json出力時にヒット番号を付与する(SEO対策が行えているかどうかのチェック用)
+
 """engine
     * Module for performing searches with SearchEngine
 """
 
 
 import os
 import pathlib
 import sys
 
 from time import sleep
 from string import ascii_lowercase, digits
 from datetime import datetime
 
-from .common import Color
-from .common import Message
+from .common import Color, Message
+from .common import set_counter
 from .engine_baidu import Baidu
 from .engine_bing import Bing
 from .engine_duckduckgo import DuckDuckGo
 from .engine_google import Google
 from .engine_yahoo import Yahoo
 
 
@@ -103,27 +109,27 @@
 
         set debug flag
 
         Args:
             debug (bool): debug flag(Enable debug with `True`).
         """
 
-        self.ENGINE.IS_DEBUG = is_debug
+        self.ENGINE.IS_DEBUG = is_debug  # type: ignore
 
     # commandフラグ(コマンドモードでの実行)を有効化する関数
     def set_is_command(self, is_command: bool):
         """set_is_command
 
         set command flag.
         When the command flag is enabled, the contents used in the command will be output to the console.
 
         Args:
             is_command (bool): command flag(Enable command mode with `True`).
         """
-        self.ENGINE.IS_COMMAND = is_command
+        self.ENGINE.IS_COMMAND = is_command  # type: ignore
 
     # color出力が有効か否か
     def set_is_color(self, is_color: bool = False):
         """set_is_color
 
         Specifies whether to display the output in color.
 
@@ -153,30 +159,30 @@
             >>> search_engine.set_disable_headless(True)
             >>>
             >>> # Open browser and search query
             >>> search_engine.search('mario')
 
         """
 
-        self.ENGINE.IS_DISABLE_HEADLESS = disable_headless
+        self.ENGINE.IS_DISABLE_HEADLESS = disable_headless  # type: ignore
 
     # cookieファイルを入れているディレクトリを渡して、使用するcookieファイルを取得する関数
     def set_cookie_files(self, cookie_dir: str):
         """set_cookie_files
 
         Function to specify and generate the cookie file name to be used by passing the directory to put the cookie file.
         Currently, cookie files are only used with Selenium.
 
         Args:
             cookie_dir (str): Directory path where cookie files are placed.
         """
 
         # フルパスに変換
-        cookie_dir = pathlib.Path(cookie_dir).expanduser()
-        cookie_dir = pathlib.Path(cookie_dir).resolve()
+        cookie_dir = pathlib.Path(cookie_dir).expanduser()  # type: ignore
+        cookie_dir = pathlib.Path(cookie_dir).resolve()  # type: ignore
 
         # 存在チェックをして、ディレクトリがない場合は新規作成
         if not os.path.exists(cookie_dir):
             # TODO: ディレクトリではなく、ファイルが存在していた場合はエラー処理をする
 
             # ディレクトリを作成
             os.mkdir(cookie_dir)
@@ -195,15 +201,28 @@
             cookie_dir, '.cookie_' + self.ENGINE.NAME.lower() + postfix)
 
         # 存在チェックをして、ファイルがない場合は新規作成
         if not os.path.exists(cookie_file):
             open(cookie_file, 'a').close()
 
         # ENGINEのself変数にセットする
-        self.ENGINE.COOKIE_FILE = cookie_file
+        self.ENGINE.COOKIE_FILE = cookie_file  # type: ignore
+
+    # クエリ実行ごとにCookieを削除して作り直しさせるかを指定する関数
+    def set_cookie_files_delete(self, is_delete_cookie: bool):
+        """set_cookie_files_delete
+
+        Function that specifies whether the cookie should be deleted and recreated each time the query is executed.
+
+        Args:
+            is_delete_cookie (bool): delete flag.
+        """
+
+        # ENGINEのself変数にセットする
+        self.ENGINE.COOKIE_FILE_DELETE = is_delete_cookie  # type: ignore
 
     # 検索エンジンにわたす言語・国の設定を受け付ける
     def set_lang(self, lang: str = "ja", locale: str = "JP"):
         """set_lang
 
         Function to set the language / country specified by the search engine.
 
@@ -234,15 +253,15 @@
 
         Args:
             proxy (str): proxy uri(ex. socks5://localhost:11080, http://hogehoge:8080)
         """
         self.ENGINE.set_proxy(proxy)
 
     # seleniumを有効にする
-    def set_selenium(self, uri: str = None, browser: str = None):
+    def set_selenium(self, uri: str = None, browser: str = None):  # type: ignore
         """set_selenium
 
         Use Selenium (priority over Splash).
 
         Args:
             uri (str, optional): Specify the `host:port` of Selenium  (used when Selenium is started by docker etc.). Defaults to None.
             browser (str, optional): Specify Browser to use with Selenium ([chrome, firefox]). Defaults to None.
@@ -259,15 +278,15 @@
         Args:
             splash_url (str): Splash uri(ex: `localhost:8050`)
         """
 
         self.ENGINE.set_splash(splash_url)
 
     # user_agentの設定値を受け付ける
-    def set_user_agent(self, useragent: str = None):
+    def set_user_agent(self, useragent: str = None):  # type: ignore
         """set_user_agent
 
         Specify the UserAgent.
         If not specified, FakeUA or hard-coded UserAgent will be used.
 
 
         Args:
@@ -281,25 +300,25 @@
         """set_ignore_ssl
 
         Ignore ssl verify.
 
         Args:
             verify (bool): bool.
         """
-        self.ENGINE.set_ignore_ssl = verify
+        self.ENGINE.set_ignore_ssl = verify  # type: ignore
 
     # 検索を行う
-    def search(self, keyword: str, type='text', maximum=100):
+    def search(self, keyword: str, search_type='text', maximum=100):
         """search
 
         Search with a search engine.
 
         Args:
             keyword (str): query.
-            type (str, optional): search type. text or image. Defaults to 'text'.
+            search_type (str, optional): search type. text or image. Defaults to 'text'.
             maximum (int, optional): Max count of searches. Defaults to 100.
 
         Returns:
             [list]: [{'link', 'http://...', 'title': 'hogehoge...'}, {'link': '...', 'title': '...'}, ... ]
         """
 
         # ENGINE.MESSAGEへis_command/is_debugを渡す
@@ -319,30 +338,30 @@
         if self.ENGINE.LANG != "" or self.ENGINE.LOCALE != "":
             self.set_lang()
 
         # メッセージ出力（コマンド実行時のみ）
         colored_keyword = self.ENGINE.MESSAGE.ENGINE_COLOR.out(keyword)
         self.ENGINE.MESSAGE.print_text(
             "$ENGINE: {} Search: {}".format(
-                type.capitalize(), colored_keyword),
+                search_type.capitalize(), colored_keyword),
             use_header=False,
             file=sys.stderr
 
         )
         result, total = [], 0
 
         # maximumが0の場合、返す値は0個になるのでこのままreturn
         if maximum == 0:
             return result
 
         # ENGINEのproxyやブラウザオプションを、各接続方式(Selenium, Splash, requests)に応じてセットし、ブラウザ(session)を作成する
         self.ENGINE.create_session()
 
         # 検索処理の開始
-        gen_url = self.ENGINE.gen_search_url(keyword, type)
+        gen_url = self.ENGINE.gen_search_url(keyword, search_type)
         while True:
             # リクエスト先のurlを取得
             try:
                 method, url, data = next(gen_url)
             except Exception:
                 break
 
@@ -361,25 +380,29 @@
                 mode='debug',
                 separator=": ",
                 header=self.ENGINE.MESSAGE.HEADER + ': ' +
                 Color.GRAY + '[DEBUG]: [UserAgent]' + Color.END
             )
 
             # 検索結果の取得
-            html = self.ENGINE.get_result(url, method=method, data=data)
+            html = self.ENGINE.get_result(
+                url, method=method, data=data)  # type: ignore
 
             # debug
             self.ENGINE.MESSAGE.print_text(
                 html,
                 mode='debug',
                 separator=": ",
                 header=self.ENGINE.MESSAGE.HEADER + ': ' +
                 Color.GRAY + '[DEBUG]: [Response]' + Color.END
             )
 
+            # 初期値
+            is_recaptcha = False
+
             while True:
                 # ReCaptchaページかどうかを識別
                 if html is not None:
                     is_recaptcha = self.ENGINE.check_recaptcha(html)
                 else:
                     break
 
@@ -391,15 +414,16 @@
                         header=self.ENGINE.MESSAGE.ENGINE,
                         separator=": "
                     )
 
                     # headless browserを使っている場合
                     if self.ENGINE.USE_SELENIUM or self.ENGINE.USE_SPLASH:
                         # byass用の関数にわたす
-                        html = self.ENGINE.bypass_recaptcha(url, html)
+                        html = self.ENGINE.bypass_recaptcha(
+                            url, html)  # type: ignore
 
                         if html is not None:
                             # debug
                             self.ENGINE.MESSAGE.print_text(
                                 html,
                                 mode='debug',
                                 header=self.ENGINE.MESSAGE.HEADER + ': ' + Color.GRAY +
@@ -424,28 +448,33 @@
                     separator=": "
                 )
 
                 break
 
             # TODO: resultも関数に渡して重複チェックを行わせる
             # 検索結果をパースしてurlリストを取得する
-            links = self.ENGINE.get_links(html, type)
+            links = self.ENGINE.get_links(
+                url, html, search_type)  # type: ignore
 
             # linksの件数に応じて処理を実施
             if not len(links):
                 # commandの場合の出力処理
                 self.ENGINE.MESSAGE.print_text(
                     'No more links.',
                     header=self.ENGINE.MESSAGE.ENGINE,
                     separator=": ",
                     file=sys.stderr,
                 )
 
                 # loopを抜ける
-                break
+                if self.ENGINE.NAME == "Google":
+                    if self.ENGINE.SEARCH_NEXT_URL is None:  # type: ignore
+                        break
+                else:
+                    break
 
             # maximumで指定した件数を超える場合、その件数までを追加してloopを抜ける
             elif len(links) > maximum - total:
                 result += links[:maximum - total]
                 break
 
             # TODO: bingのときだけ追加する処理として外だしする方法を考える
@@ -457,27 +486,34 @@
             else:
                 result += links
                 total += len(links)
 
             # 連続でアクセスすると問題があるため、3秒待機
             sleep(3)
 
+        # 検索番号を指定
+        result = set_counter(result)
+
         # commandの場合の出力処理
         self.ENGINE.MESSAGE.print_text(
             'Finally got ' + self.ENGINE.COLOR +
             str(len(result)) + Color.END + ' links.',
             header=self.ENGINE.MESSAGE.ENGINE,
             separator=": ",
             file=sys.stderr,
         )
 
         # save cookies
         if self.ENGINE.COOKIE_FILE != '':
             self.ENGINE.write_cookies()
 
+        # delete cookie file
+        if self.ENGINE.COOKIE_FILE_DELETE:
+            os.remove(self.ENGINE.COOKIE_FILE)
+
         # sessionを終了
         self.ENGINE.close_session()
 
         return result
 
     # suggestを取得する
     def suggest(self, keyword: str, jap=False, alph=False, num=False):
@@ -498,31 +534,32 @@
         # ENGINEのproxyやブラウザオプションを、各接続方式(Selenium, Splash, requests)に応じてセットし、ブラウザ(session)を作成する
         self.ENGINE.create_session()
 
         # 文字リスト作成
         chars = ['', ' ']
 
         # japフラグが有効な場合、キーワードに日本語を含めてサジェストを検索
-        chars += [' ' + chr(i) for i in range(12353, 12436)] if jap else[]
+        chars += [' ' + chr(i) for i in range(12353, 12436)] if jap else []
 
         # alphフラグが有効な場合、キーワードにアルファベットを含めてサジェストを検索
-        chars += [' ' + char for char in ascii_lowercase] if alph else[]
+        chars += [' ' + char for char in ascii_lowercase] if alph else []
 
         # numフラグが有効な場合、キーワードに数字を含めてサジェストを検索
         chars += [' ' + char for char in digits] if num else []
 
         # サジェスト取得
         suggests = {}
         for char in chars:
             word = keyword + char
             url = self.ENGINE.gen_suggest_url(word)
             html = self.ENGINE.get_result(url)
 
             # TODO: 各エンジンでjson/textの変換処理を別途実装する必要がある
-            suggests = self.ENGINE.get_suggest_list(suggests, char, html)
+            suggests = self.ENGINE.get_suggest_list(
+                suggests, char, html)  # type: ignore
 
             sleep(0.5)
 
         # sessionを終了
         self.ENGINE.close_session()
 
         return suggests
```

### Comparing `pydork-1.1.2/pydork/engine_baidu.py` & `pydork-1.1.4/pydork/engine_baidu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
 
 """engine_baidu
     * Baidu用の検索用Classを持つモジュール.
 """
 
@@ -132,15 +135,15 @@
         }
 
         params = parse.urlencode(url_param)
         url = self.SUGGEST_URL + '?' + params
 
         return url
 
-    def get_links(self, html: str, type: str):
+    def get_links(self, url: str, html: str, type: str):
         """get_links
 
         受け付けたhtmlを解析し、検索結果をlistに加工して返す関数.
 
         Args:
             html (str): 解析する検索結果のhtml.
             type (str): 検索タイプ([text, image]).現時点ではtextのみ対応.
@@ -154,15 +157,15 @@
         if type == 'text':
             # Splash経由で通信している場合
             self.SOUP_SELECT_URL = '.tts-title > a'
             self.SOUP_SELECT_TITLE = '.tts-title > a'
             self.SOUP_SELECT_TEXT = '.c-gap-top-small > span'
 
             # CommonEngineの処理を呼び出す
-            links = super().get_links(html, type)
+            links = super().get_links(url, html, type)
 
         elif type == 'image':
             # unicode escape
             # html = html.encode().decode("unicode-escape")
             html = html.replace("\\'", "'")
 
             # seleniumを使用している場合、htmlで返ってくるためjson要素のみを抽出する
```

### Comparing `pydork-1.1.2/pydork/engine_bing.py` & `pydork-1.1.4/pydork/engine_bing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
 
 """engine_bing
     * Bing用の検索用Classを持つモジュール.
 """
 
@@ -138,15 +141,15 @@
         }
 
         params = parse.urlencode(url_param)
         url = self.SUGGEST_URL + '?' + params
 
         return url
 
-    def get_links(self, html: str, type: str):
+    def get_links(self, url: str, html: str, type: str):
         """get_links
 
         受け付けたhtmlを解析し、検索結果をlistに加工して返す関数.
 
         Args:
             html (str): 解析する検索結果のhtml.
             type (str): 検索タイプ([text, image]).現時点ではtextのみ対応.
@@ -160,15 +163,15 @@
             self.SOUP_SELECT_TITLE = 'h2 > a'
             self.SOUP_SELECT_TEXT = 'li > div > p'
 
         elif type == 'image':
             self.SOUP_SELECT_URL = '.imgpt > .iusc'
 
         # CommonEngineの処理を呼び出す
-        links = super().get_links(html, type)
+        links = super().get_links(url, html, type)
 
         return links
 
     # 画像検索ページの検索結果(links(list()))を生成するfunction
     def get_image_links(self, soup: BeautifulSoup):
         """get_image_links
         BeautifulSoupから画像検索ページを解析して結果を返す関数.
```

### Comparing `pydork-1.1.2/pydork/engine_common.py` & `pydork-1.1.4/pydork/engine_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
 
 """engine_common
     * SearchEngine Classから呼び出す、各検索エンジンで共通の処理を保持させる継承用Classである `CommonEngine` を持つモジュール.
 """
 
@@ -46,23 +49,24 @@
         # headless browserの利用有無フラグ(デフォルト: False)
         self.USE_SELENIUM = False
         self.USE_SPLASH = False
 
         # 初期値の作成
         self.LOCK = None
         self.COOKIE_FILE = ''
+        self.COOKIE_FILE_DELETE = False
         self.SPLASH_URI = ''
         self.PROXY = ''
         self.USER_AGENT = ''
         self.LANG = ''
         self.LOCALE = ''
         self.IS_DEBUG = False
         self.IS_COMMAND = False
         self.IS_DISABLE_HEADLESS = False
-        self.MESSAGE = False
+        self.MESSAGE: Message
         self.IGNORE_SSL_VERIFY = False
 
         # ReCaptcha画面かどうかの識別用(初期値(ブランク))
         self.RECAPTCHA_SITEKEY = ''
         self.SOUP_RECAPTCHA_TAG = ''
         self.SOUP_RECAPTCHA_SITEKEY = ''
 
@@ -90,15 +94,15 @@
             start (datetime): 検索対象ページの対象範囲開始日時(datetime)
             end (datetime): 検索対象ページの対象範囲終了日時(datetime)
         """
         self.RANGE_START = start
         self.RANGE_END = end
 
     # user_agentの設定値を受け付ける(引数がない場合はランダム。Seleniumの際は自動的に使用したbrowserのagentを指定)
-    def set_user_agent(self, user_agent: str = None, browser: str = None):
+    def set_user_agent(self, user_agent: str = None, browser: str = None):  # type: ignore
         """set_user_agent
 
         user_agentの値を受け付ける.
         user_agentの指定がない場合、 Chromeを使用したものとする.
         また、もし`browser`が指定されている場合はそのブラウザのUser Agentを指定する.
 
         注) seleniumを利用する場合、事前に有効にする必要がある。
@@ -130,15 +134,15 @@
 
         self.USER_AGENT = user_agent
 
     # seleniumを有効にする
     #   - splashより優先
     #   - host, browserは、指定がない場合はそれぞれデフォルト設定(hostは指定なし、browserはchrome)での動作
     #   - browserは `chrome` or `firefox` のみ受け付ける
-    def set_selenium(self, uri: str = None, browser: str = None):
+    def set_selenium(self, uri: str = None, browser: str = None):  # type: ignore
         """set_selenium
 
         検索時にSelenium経由で通信を行う.
         他のHeadless Browserと比較して最優先(Splash等が有効でもこちらが優先される).
 
         Args:
             uri (str, optional): APIのURIを指定(localhost:4444). Defaults to None.
@@ -192,26 +196,33 @@
     def read_cookies(self):
         """read_cookies
 
         `self.COOKIE_FILE` からcookieを読み込む.
         現時点ではSeleniumでのみ動作.
         """
 
+        # cookieファイルが存在しない場合、空ファイルで作成する
+        exist_cookie_file = os.path.isfile(self.COOKIE_FILE)
+        if not exist_cookie_file:
+            cookie_file = open(self.COOKIE_FILE, 'w')
+            cookie_file.write('')
+            cookie_file.close()
+
         # cookieファイルのサイズを取得
         file_size = os.path.getsize(self.COOKIE_FILE)
 
         # cookieファイルのサイズが0以上の場合
         if file_size > 0:
             # cookie fileからcookieの取得
             cookies = pickle.load(open(self.COOKIE_FILE, "rb"))
 
             # seleniumを使う場合
             if self.USE_SELENIUM:
                 # 事前アクセスが必要になるため、検索対象ドメインのTOPページにアクセスしておく
-                self.driver.get(self.ENGINE_TOP_URL)
+                self.driver.get(self.ENGINE_TOP_URL)  # type: ignore
 
                 # cookieを設定していく
                 for cookie in cookies:
                     try:
                         self.driver.add_cookie(cookie)
                     except Exception:
                         pass
@@ -294,34 +305,67 @@
         Seleniumで使用するDriverを作成する関数.
         Optionsもこの関数で作成する.
         """
 
         # optionsを取得する
         options = self.create_selenium_options()
 
-        # proxyを追加
-        if self.PROXY != '':
-            options.add_argument('--proxy-server=%s' % self.PROXY)
-
         # browserに応じてdriverを作成していく
         if self.SELENIUM_BROWSER == 'chrome':
+            # proxyを追加
+            if self.PROXY != '':
+                options.add_argument('--proxy-server=%s' % self.PROXY)
+
             try:
                 chromedriver_autoinstaller.install()
             except Exception:
                 pass
 
             self.driver = Chrome(options=options)
 
         elif self.SELENIUM_BROWSER == 'firefox':
             # profileを作成する
             profile = webdriver.FirefoxProfile()
             profile.set_preference('devtools.jsonview.enabled', False)
             profile.set_preference('plain_text.wrap_long_lines', False)
             profile.set_preference('view_source.wrap_long_lines', False)
 
+            # proxyを追加
+            if self.PROXY != '':
+                # self.PROXYをパース処理する
+                parsed_uri = parse.urlparse(self.PROXY)
+
+                # socks5
+                if parsed_uri.scheme == "socks5":
+                    # Proxy設定を追加
+                    profile.set_preference(
+                        'network.proxy.type', 1)
+                    profile.set_preference('network.proxy.socks_version', 5)
+                    profile.set_preference(
+                        'network.proxy.socks', parsed_uri.hostname)
+                    profile.set_preference(
+                        'network.proxy.socks_port', parsed_uri.port)
+                    profile.set_preference('network.proxy.no_proxies_on', '')
+                    profile.set_preference(
+                        'network.proxy.socks_remote_dns', True)
+                    profile.update_preferences()
+                elif parsed_uri.scheme == "socks4":
+                    # Proxy設定を追加
+                    profile.set_preference(
+                        'network.proxy.type', 1)
+                    profile.set_preference('network.proxy.socks_version', 4)
+                    profile.set_preference(
+                        'network.proxy.socks', parsed_uri.hostname)
+                    profile.set_preference(
+                        'network.proxy.socks_port', parsed_uri.port)
+                    profile.set_preference('network.proxy.no_proxies_on', '')
+                    profile.set_preference(
+                        'network.proxy.socks_remote_dns', True)
+                    profile.update_preferences()
+
             # set ssl verify(firefoxの場合はprofileで処理するのでこちらに記述する)
             if not self.IGNORE_SSL_VERIFY:
                 profile.accept_untrusted_certs = True
 
             try:
                 geckodriver_autoinstaller.install()
             except Exception:
@@ -356,29 +400,29 @@
             response = self.driver.get(url)
 
             # wait all elements
             WebDriverWait(self.driver, 15).until(
                 EC.presence_of_all_elements_located)
 
             # wait 5 seconds(wait DOM)
-            if self.NAME in ('Bing', 'Baidu', 'DuckDuckGo'):
+            if self.NAME in ('Bing', 'Baidu', 'DuckDuckGo'):  # type: ignore
                 self.driver.implicitly_wait(20)
 
             # get result
             result = self.driver.page_source
 
         elif method == 'POST':
             response = self.driver.request('POST', url, data=data)
 
             # wait all elements
             WebDriverWait(self.driver, 15).until(
                 EC.presence_of_all_elements_located)
 
             # wait 5 seconds(wait DOM)
-            if self.NAME in ('Bing', 'Baidu', 'DuckDuckGo'):
+            if self.NAME in ('Bing', 'Baidu', 'DuckDuckGo'):  # type: ignore
                 self.driver.implicitly_wait(20)
 
             # get result
             result = response.text
 
         return result
 
@@ -411,15 +455,15 @@
 
         # リクエストを投げてレスポンスを取得する
         if method == 'GET':
             result = self.session.get(splash_url, params=params).text
 
         # NOTE: Googleの画像検索のPOSTがSplashではレンダリングできないので、特例対応でrequestsを使用する.
         # TODO: Splashでもレンダリングできるようになったら書き換える.
-        elif method == 'POST' and self.NAME == 'Google' and self.IMAGE_URL in url:
+        elif method == 'POST' and self.NAME == 'Google' and self.IMAGE_URL in url:  # type: ignore
             # create session
             session = requests.session()
 
             # proxyを設定
             if self.PROXY != '':
                 proxies = {
                     'http': self.PROXY,
@@ -437,15 +481,15 @@
                 )
 
             result = session.post(url, data=data).text
 
         elif method == 'POST':
             headers = {'Content-Type': 'application/json'}
             params['http_method'] = 'POST'
-            params['body'] = parse.urlencode(data)
+            params['body'] = parse.urlencode(data)  # type: ignore
 
             result = self.session.post(
                 splash_url,
                 headers=headers,
                 json=params
             ).text
 
@@ -567,20 +611,21 @@
             dict: data
         """
 
         result = {}
         return 'GET', result, None
 
     # テキスト、画像検索の結果からlinksを取得するための集約function
-    def get_links(self, html: str, type: str):
+    def get_links(self, source_url, html: str, type: str):
         """get_links
 
         受け付けたhtmlを解析し、検索結果をlistに加工して返す関数.
 
         Args:
+            url  (str): 解析する検索結果のurl.
             html (str): 解析する検索結果のhtml.
             type (str): 検索タイプ([text, image]).現時点ではtextのみ対応.
 
         Returns:
             list: 検索結果(`[{'title': 'title...', 'link': 'https://hogehoge....'}, {...}]`)
         """
 
@@ -589,15 +634,15 @@
 
         if type == 'text':
             # link, titleの組み合わせを取得する
             elinks, etitles, etexts = self.get_text_links(soup)
 
             # before processing elists
             self.MESSAGE.print_text(
-                ','.join(elinks),
+                ','.join(elinks),  # type: ignore
                 header=self.MESSAGE.HEADER + ': ' + Color.BLUE +
                 '[BeforeProcessing elinks]' + Color.END,
                 separator=" :",
                 mode="debug",
             )
 
             # before processing etitles
@@ -611,15 +656,15 @@
 
             # 加工処理を行う関数に渡す(各エンジンで独自対応)
             elinks, etitles, etexts = self.processings_elist(
                 elinks, etitles, etexts)
 
             # after processing elists
             self.MESSAGE.print_text(
-                ','.join(elinks),
+                ','.join(elinks),  # type: ignore
                 header=self.MESSAGE.HEADER + ': ' +
                 Color.GREEN + '[AfterProcessing elinks]' + Color.END,
                 separator=" :",
                 mode="debug",
             )
 
             # after processing etitles
@@ -629,15 +674,15 @@
                 Color.GREEN + '[AfterProcessing etitles]' + Color.END,
                 separator=" :",
                 mode="debug",
             )
 
             # dictに加工してリスト化する
             # [{'title': 'title...', 'link': 'https://hogehoge....'}, {...}]
-            links = self.create_text_links(elinks, etitles, etexts)
+            links = self.create_text_links(source_url, elinks, etitles, etexts)
 
             return links
 
         elif type == 'image':
             links = self.get_image_links(soup)
 
             return links
@@ -648,16 +693,17 @@
 
         BeautifulSoupからテキスト検索ページを解析して結果を返す関数.
 
         Args:
             soup (BeautifulSoup): 解析するBeautifulSoupオブジェクト.
 
         Returns:
-            list: linkの検索結果([xxx,xxx,xxx...)
-            list: titleの検索結果([xxx,xxx,xxx...)
+            list: linkの検索結果([xxx,xxx,xxx...])
+            list: titleの検索結果([xxx,xxx,xxx...])
+            list: textの検索結果([xxx,xxx,xxx...])
         """
         # linkのurlを取得する
         elements = soup.select(self.SOUP_SELECT_URL)
         elinks = [e['href'] for e in elements]
 
         # linkのtitleを取得する
         elements = soup.select(self.SOUP_SELECT_TITLE)
@@ -703,15 +749,15 @@
             etitles (list): etitles(検索結果のtitle)の配列
             etexts (list): etexts(検索結果のtext)の配列
         """
 
         return elinks, etitles, etexts
 
     # テキスト検索の1ページごとの検索結果から、links(links([{link: ..., title: ...},...]))を生成するfunction
-    def create_text_links(self, elinks, etitles, etext: list):
+    def create_text_links(self, source_url: str, elinks, etitles, etext: list):
         """create_text_links
 
         elinks, etitlesからlinks(get_linksのデータ)を返す関数.
 
         Args:
             elinks (list): elinks(検索結果のlink)の配列
             etitles (list): etitles(検索結果のtitle)の配列
@@ -732,19 +778,23 @@
             if len(etitles) > n:
                 d['title'] = etitles[n]
 
             # etext(urlに対応する検索結果のテキスト文)をdictに追加する
             if len(etext) > n:
                 d['text'] = etext[n]
 
+            # 検索元urlをdictに追加する
+            d['source_url'] = source_url
+
             if before_link != link:
                 links.append(d)
 
             before_link = link
             n += 1
+
         return links
 
     # サジェスト取得用のurlを生成
     def gen_suggest_url(self, keyword: str):
         """gen_suggest_url
 
         サジェスト取得用のurlを生成する.
```

### Comparing `pydork-1.1.2/pydork/engine_duckduckgo.py` & `pydork-1.1.4/pydork/engine_duckduckgo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
 
 """engine_duckduckgo
     * DuckDuckGo用の検索用Classを持つモジュール.
 """
 
@@ -174,20 +177,21 @@
         }
 
         params = parse.urlencode(url_param)
         url = self.SUGGEST_URL + '?' + params
 
         return url
 
-    def get_links(self, html: str, type: str):
+    def get_links(self, source_url: str, html: str, type: str):
         """get_links
 
         受け付けたhtmlを解析し、検索結果をlistに加工して返す関数.
 
         Args:
+            url  (str): 解析する検索結果のurl.
             html (str): 解析する検索結果のhtml.
             type (str): 検索タイプ([text, image]).現時点ではtextのみ対応.
 
         Returns:
             list: 検索結果(`[{'title': 'title...', 'url': 'https://hogehoge....'}, {...}]`)
         """
         links = list()
@@ -210,15 +214,16 @@
             for r_data in r_dict:
                 if "u" in r_data and "s" in r_data:
                     d = {
                         "link": r_data["u"],
                         "title": BeautifulSoup(
                             r_data["t"], "lxml").text,
                         "text": BeautifulSoup(
-                            r_data["a"], "lxml").text
+                            r_data["a"], "lxml").text,
+                        "source_url": source_url,
                     }
                     links.append(d)
 
                 elif "n" in r_data:
                     base_uri = '{uri.scheme}://{uri.netloc}'.format(
                         uri=parse.urlparse(self.SEARCH_URL)
                     )
```

### Comparing `pydork-1.1.2/pydork/engine_google.py` & `pydork-1.1.4/pydork/engine_google.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
 
 """engine_google
     * Google用の検索用Classを持つモジュール.
 """
 
@@ -11,14 +14,15 @@
 import json
 import os
 
 from time import sleep
 from json.decoder import JSONDecodeError
 from urllib import parse
 from lxml import etree
+from bs4 import BeautifulSoup
 
 from .common import Color
 from .recaptcha import TwoCaptcha
 from .engine_common import CommonEngine
 
 
 # Google画像検索で使用するパラメータID
@@ -41,14 +45,17 @@
 
         # リクエスト先のURLを指定
         self.ENGINE_TOP_URL = 'https://www.google.com/'
         self.SEARCH_URL = 'https://www.google.com/search'
         self.IMAGE_URL = 'https://www.google.com/_/VisualFrontendUi/data/batchexecute'
         self.SUGGEST_URL = 'http://www.google.com/complete/search'
 
+        # 次の検索ページのURL(`self.get_nextpage_url`の処理で取得する)
+        self.SEARCH_NEXT_URL = None
+
         # ReCaptcha画面かどうかの識別用
         self.SOUP_RECAPTCHA_TAG = '#captcha-form > #recaptcha'
 
     def gen_search_url(self, keyword: str, type: str):
         """gen_search_url
 
         検索用のurlを生成する.
@@ -67,15 +74,15 @@
             # 検索用urlを指定
             search_url = self.SEARCH_URL
 
             # 検索パラメータの設定
             url_param = {
                 'q': keyword,   # 検索キーワード
                 'oq': keyword,  # 検索キーワード
-                'num': '100',   # 1ページごとの表示件数
+                'num': '100',   # 1ページごとの表示件数.
                 'filter': '0',  # 類似ページのフィルタリング(0...無効, 1...有効)
                 'start': '',    # 開始位置
                 'tbs': '',      # 期間
                 'nfpr': '1'     # もしかして検索(Escape hatch)を無効化
             }
 
             # lang/localeが設定されている場合
@@ -96,22 +103,27 @@
                     cd_min, cd_max)
 
             except AttributeError:
                 None
 
             page = 0
             while True:
-                # parameterにページを開始する番号を指定
-                url_param['start'] = str(page * 100)
-                params = parse.urlencode(url_param)
-
-                target_url = search_url + '?' + params
+                if page == 0:
+                    # parameterにページを開始する番号を指定
+                    url_param['start'] = str(page * 100)
+                    params = parse.urlencode(url_param)
+
+                    target_url = search_url + '?' + params
+
+                else:
+                    target_url = self.SEARCH_NEXT_URL
+                    if self.SEARCH_NEXT_URL is None:
+                        break
 
                 yield 'GET', target_url, None
-
                 page += 1
 
         elif type == 'image':
             # 検索用urlを指定
             search_url = self.IMAGE_URL
 
             # Refererの設定
@@ -169,56 +181,62 @@
         }
 
         params = parse.urlencode(url_param)
         url = self.SUGGEST_URL + '?' + params
 
         return url
 
-    def get_links(self, html: str, type: str):
+    def get_links(self, url: str, html: str, type: str):
         """get_links
 
         受け付けたhtmlを解析し、検索結果をlistに加工して返す関数.
 
         Args:
+            url  (str): 解析する検索結果のurl.
             html (str): 解析する検索結果のhtml.
             type (str): 検索タイプ([text, image]).現時点ではtextのみ対応.
 
         Returns:
-            list: 検索結果(`[{'title': 'title...', 'url': 'https://hogehoge....'}, {...}]`)
+            list: 検索結果。変数名はlinks。(`[{'title': 'title...', 'url': 'https://hogehoge....'}, {...}]`)
         """
 
         # テキスト検索の場合
         if type == 'text':
             # request or seleniumの定義
             self.SOUP_SELECT_URL = '#main > div > div > .kCrYT > a'
             self.SOUP_SELECT_TITLE = '#main > div > div > .kCrYT > a > h3 > div'
             self.SOUP_SELECT_TEXT = '#main > div > div > .kCrYT > div > div > div > div > div'
+            self.SOUP_SELECT_NEXT_URL = ''
 
             # Selenium経由、かつFirefoxを使っている場合
-            if self.USE_SELENIUM and self.SELENIUM_BROWSER == 'firefox':
-                self.SOUP_SELECT_URL = '.jtfYYd > div > .yuRUbf > a'
-                self.SOUP_SELECT_TITLE = '.jtfYYd > div > .yuRUbf > a > .LC20lb'
-                self.SOUP_SELECT_TEXT = '.jtfYYd > div > div'
+            if self.USE_SELENIUM:
+                self.SOUP_SELECT_URL = '.yuRUbf > a'
+                self.SOUP_SELECT_TITLE = '.yuRUbf > a > .LC20lb'
+                self.SOUP_SELECT_TEXT = '.lEBKkf'
+                self.SOUP_SELECT_NEXT_URL = '.d6cvqb > a'
 
             # Splash経由で通信している場合
             elif self.USE_SPLASH:
                 self.SOUP_SELECT_URL = '.yuRUbf > a'
                 self.SOUP_SELECT_TITLE = '.yuRUbf > a > .LC20lb'
-                self.SOUP_SELECT_TEXT = '.jtfYYd > div > div'
+                self.SOUP_SELECT_TEXT = '.lEBKkf'
+                self.SOUP_SELECT_NEXT_URL = '.d6cvqb > a'
+
+            # TODO: SEARCH_NEXT_URLを書き換える
+            self.get_nextpage_url(html)
 
             # CommonEngineの処理を呼び出す
-            links = super().get_links(html, type)
+            links = super().get_links(url, html, type)
 
         # イメージ検索の場合
         elif type == 'image':
             links = self.get_image_links(html)
 
         return links
 
-    # 画像検索ページの検索結果(links(list()))を生成するfunction
     def get_image_links(self, html: str):
         """get_image_links
 
         BeautifulSoupから画像検索ページを解析して結果を返す関数.
         Seleniumを利用し、自動的にページ末尾まで移動して続きを取得する.
         クリック等が発生するため、抽出にかなり時間がかかる.
 
@@ -282,18 +300,41 @@
             dict: サジェスト配列
         """
 
         sug_root = etree.XML(html)
         sug_data = sug_root.xpath("//suggestion")
         data = [s.get("data") for s in sug_data]
 
-        suggests[char if char == '' else char[-1]] = data
+        suggests[char if char == '' else char[-1]] = data  # type: ignore
 
         return suggests
 
+    def get_nextpage_url(self, html: str):
+        # BeautifulSoupでの解析を実施
+        soup = BeautifulSoup(html, 'lxml')
+
+        # BeautifulSoupでnext urlの要素を確認する
+        elements = soup.select(self.SOUP_SELECT_NEXT_URL)
+
+        # next urlを取得する
+        elinks = [e['href'] for e in elements]
+
+        if len(elinks) == 0:
+            self.SEARCH_NEXT_URL = None
+
+        elif len(elinks) == 1:
+            next_url = parse.urljoin(
+                self.ENGINE_TOP_URL, elinks[0])  # type: ignore
+            self.SEARCH_NEXT_URL = next_url
+
+        elif len(elinks) > 1:
+            next_url = parse.urljoin(
+                self.ENGINE_TOP_URL, elinks[1])  # type: ignore
+            self.SEARCH_NEXT_URL = next_url
+
     def processings_elist(self, elinks, etitles, etexts: list):
         """processings_elist
 
         self.get_links 内で、取得直後のelinks, etitlesに加工を加えるための関数.
 
         Args:
             elinks (list): elinks(検索結果のlink)の配列
```

### Comparing `pydork-1.1.2/pydork/engine_yahoo.py` & `pydork-1.1.4/pydork/engine_yahoo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
 
 """engine_yahoo
     * Yahoo(yahoo.co.jp)用の検索用Classを持つモジュール.
 """
 
@@ -152,20 +155,21 @@
         }
 
         params = parse.urlencode(url_param)
         url = self.SUGGEST_URL + '?' + params
 
         return url
 
-    def get_links(self, html: str, type: str):
+    def get_links(self, url: str, html: str, type: str):
         """get_links
 
         受け付けたhtmlを解析し、検索結果をlistに加工して返す関数.
 
         Args:
+            url  (str): 解析する検索結果のurl.
             html (str): 解析する検索結果のhtml.
             type (str): 検索タイプ([text, image]).現時点ではtextのみ対応.
 
         Returns:
             list: 検索結果(`[{'title': 'title...', 'url': 'https://hogehoge....'}, {...}]`)
         """
 
@@ -180,44 +184,45 @@
                 elements = soup.select(self.SOUP_SELECT_JSON)
                 element = elements[0].string
 
                 # debug
                 if self.IS_DEBUG:
                     print(Color.PURPLE + '[JsonElement]' + Color.END,
                           file=sys.stderr)
-                    print(Color.PURPLE + element + Color.END, file=sys.stderr)
+                    print(Color.PURPLE + element + Color.END,
+                          file=sys.stderr)  # type: ignore
 
                 # jsonからデータを抽出　
-                j = json.loads(element)
+                j = json.loads(element)  # type: ignore
 
                 # debug
                 if self.IS_DEBUG:
                     print(Color.PURPLE + '[Json]' + Color.END, file=sys.stderr)
                     print(Color.PURPLE + json.dumps(j) + Color.END,
                           file=sys.stderr)
 
                 jd = j['props']['initialProps']['pageProps']['pageData']['algos']
 
                 elinks = [e['url'] for e in jd]
                 etitles = [e['title'] for e in jd]
                 etexts = [e['description'] for e in jd]
 
-                links = self.create_text_links(elinks, etitles, etexts)
+                links = self.create_text_links(url, elinks, etitles, etexts)
 
             else:
                 self.SOUP_SELECT_URL = '.sw-Card__headerSpace > .sw-Card__title > a'
                 self.SOUP_SELECT_TITLE = '.sw-Card__headerSpace > .sw-Card__title > a > h3'
                 self.SOUP_SELECT_TEXT = '.sw-Card__floatContainer > .sw-Card__summary'
 
                 # CommonEngineの処理を呼び出す
-                links = super().get_links(html, type)
+                links = super().get_links(url, html, type)
 
         elif type == 'image':
             # CommonEngineの処理を呼び出す
-            links = super().get_links(html, type)
+            links = super().get_links(url, html, type)
 
         return links
 
     # 画像検索ページの検索結果(links(list()))を生成するfunction
     def get_image_links(self, soup: BeautifulSoup):
         """get_image_links
         BeautifulSoupから画像検索ページを解析して結果を返す関数.
@@ -264,15 +269,15 @@
         Returns:
             dict: サジェスト配列
         """
         if self.USE_SELENIUM and self.SELENIUM_BROWSER == 'firefox':
             soup = BeautifulSoup(html, features="lxml")
             html = soup.find("pre").text
         data = json.loads(html)
-        suggests[char if char == '' else char[-1]] = [e['key']
+        suggests[char if char == '' else char[-1]] = [e['key']  # type: ignore
                                                       for e in data['gossip']['results']]
 
         return suggests
 
     def get_image_search_cr(self, keyword: str):
         """get_image_search_cr
```

### Comparing `pydork-1.1.2/pydork/recaptcha.py` & `pydork-1.1.4/pydork/recaptcha.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
 """engine
     * ReCaptcha関連のClassを集約するモジュールファイル
 """
 
 import json
```

### Comparing `pydork-1.1.2/pydork/subcommands.py` & `pydork-1.1.4/pydork/sub_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
-"""subcommand
+"""subcommands
     * pydorkをコマンドとして動作させる際の処理を記載しているモジュール
 """
 
 
 import sys
 import threading
 import json
 import os
 import pathlib
 
+from typing import List
+from argparse import Namespace
 from jinja2 import Template
 
 from .engine import SearchEngine, ENGINES
 from .common import Color
 from .common import Message
 
 
@@ -30,75 +35,62 @@
     """
 
     # template file用の変数セット(dict)
     template_variable = {}
 
     # query及びfileがともに指定なしの場合、エラーにして返す
     if args.query == "" and args.file == "" and args.template_file == "":
-        print("Error: クエリもしくはファイルを指定してください.")
+        print("Error: クエリもしくはファイルを指定してください.", file=sys.stderr)
         return
 
     # args.fileのチェック
     if args.file != "":
         if not os.path.exists(args.file):
-            print("Error: ファイルが存在しません.")
+            print("Error: ファイルが存在しません.", file=sys.stderr)
             return
 
-    # args.fileのチェック
+    # args.template_fileのチェック
     if args.template_file != "":
         if not os.path.exists(args.template_file):
-            print("Error: ファイルが存在しません.")
+            print("Error: ファイルが存在しません.", file=sys.stderr)
             return
 
         if args.template_variable == "":
-            print("Error: テンプレート変数が指定されていません.")
+            print("Error: テンプレート変数が指定されていません.", file=sys.stderr)
             return
 
         try:
             template_variable = json.loads(args.template_variable)
         except Exception:
-            print("Error: テンプレート変数の形式がまちがっています.")
+            print("Error: テンプレート変数の形式がまちがっています.", file=sys.stderr)
             return
 
+    # 各サブコマンドのチェック
     target = None
     search_mode = ''
     if subcommand == 'search':
         # チェック処理
         if ((args.start is None and args.end is not None) or (args.start is not None and args.end is None)):
             print(
                 Color.GRAY + "期間を指定する場合は--start, --endの両方を指定してください" + Color.END,
                 file=sys.stderr
             )
             return
-        target = search
+        target = run_search
         search_mode = 'text'
 
     elif subcommand == 'image':
-        target = search
+        target = run_search
         search_mode = 'image'
 
     elif subcommand == 'suggest':
-        target = suggest
+        target = run_suggest
 
     # create query_list
-    query_list = list()
-
-    # append query
-    if args.query != "":
-        query_list.append(args.query)
-
-    # append query in file
-    if args.file != "":
-        # fileのfull pathを取得
-        file = pathlib.Path(args.file).expanduser()
-
-        # ファイルを開いて1行ずつqueryに追加する
-        with open(file) as f:
-            file_querys = [s.strip() for s in f.readlines()]
-            query_list.extend(file_querys)
+    query_list = generate_query_list(args)
 
     # append query in template file
     if args.template_file != "":
         # template fileのfullpathを取得
         template_file = pathlib.Path(args.template_file).expanduser()
 
         # args.template_variableをjsonとして読み込む.
@@ -153,15 +145,15 @@
 
     # json出力が有効だった場合、json形式で出力
     if args.json:
         print(json.dumps(thread_result, ensure_ascii=False, indent=2))
 
 
 # SearchEngineのオプション設定用関数
-def set_se_options(se, args):
+def set_se_options(se: SearchEngine, args: Namespace):
     """set_se_options
 
     Args:
         se (SearchEngine): argsの情報を元に、オプションを設定するSearchEngine.
         args (Namespace): argparseで取得した引数(Namespace).
 
     Returns:
@@ -216,19 +208,22 @@
 
     # lang/country code
     se.set_lang(args.lang, args.country)
 
     # set cookie driver(last set)
     se.set_cookie_files(args.cookies)
 
+    # set cookie file delete
+    se.set_cookie_files_delete(args.delete_cookies)
+
     return se
 
 
 # 検索結果を出力する
-def print_search_result(result, args, message):
+def print_search_result(result, args: Namespace, message: Message):
     """print_search_result
 
 
     Args:
         result : SearchEngine.searchのresult.
         args (Namespace): argparseで取得した引数(Namespace).
         message (common.Message): 出力用Class.
@@ -275,29 +270,54 @@
                 title = Color.GRAY + title + Color.END
 
             data.insert(0, title)
 
         message.print_line(*data, separator=sep)
 
 
+# generate
+def generate_query_list(args: Namespace):
+    """generate_query_list
+
+    """
+    # create query_list
+    query_list: List[str] = list()
+
+    # append query
+    if args.query != "":
+        query_list.append(args.query)
+
+    # append query in file
+    if args.file != "":
+        # fileのfull pathを取得
+        file = pathlib.Path(args.file).expanduser()
+
+        # ファイルを開いて1行ずつqueryに追加する
+        with open(file) as f:
+            file_querys = [s.strip() for s in f.readlines()]
+            query_list.extend(file_querys)
+
+    return query_list
+
+
 # 検索
-def search(engine: str, query_list: list, args, thread_result: dict, cmd=False, lock=None, mode='text'):
+def run_search(engine: str, query_list: list, args, thread_result: dict, cmd=False, lock=None, mode='text'):
     """search
 
     Args:
         engine (str): 使用する検索エンジン(.engine.ENGINES).
         query_list(list): 検索クエリのリスト.
         args (Namespace): argparseで取得した引数(Namespace).
         thread_result(dict): 結果を1箇所に集約するためのresult dict. json出力するときのみ使用.
         cmd (bool, optional): commandで実行しているか否か. Defaults to False.
         lock (threading.Lock): threadingのマルチスレッドで使用するLock.現在は未使用. Defaults to None.
         type (str, optional): 検索タイプ. `text` or `image`.
     """
 
-    # start search engine class
+    # start SearchEngine class
     se = SearchEngine()
 
     # Set Engine
     se.set(engine)
 
     # Set SearchEngine options
     se = set_se_options(se, args)
@@ -320,15 +340,15 @@
     # json出力時の変数を宣言
     all_result_json = list()
 
     # query_listの内容を順番に処理
     for query in query_list:
         # 検索を実行
         result = se.search(
-            query, type=search_type,
+            query, search_type=search_type,
             maximum=args.num
         )
 
         # debug
         se.ENGINE.MESSAGE.print_text(
             json.dumps(result),
             separator=sep,
@@ -349,25 +369,25 @@
             print_search_result(result, args, se.ENGINE.MESSAGE)
 
     if args.json:
         thread_result[engine] = all_result_json
 
 
 # サジェスト
-def suggest(engine: str, query_list: list, args, thread_result: dict, cmd=False, lock=None, mode=''):
+def run_suggest(engine: str, query_list: list, args: Namespace, thread_result: dict, cmd=False, lock=None, mode=''):
     """suggest
 
     Args:
         engine (str): 使用する検索エンジン(.engine.ENGINES).
         query_list(list): 検索クエリのリスト.
         args (Namespace): argparseで取得した引数(Namespace).
         thread_result(dict): 結果を1箇所に集約するためのresult dict. json出力するときのみ使用.
         cmd (bool, optional): commandで実行しているか否か. Defaults to False.
         lock (threading.Lock): threadingのマルチスレッドで使用するLock.現在は未使用. Defaults to None.
-        mode (str, optional): マルチスレッドでsearchとある程度共用で使えるようにするための引数. 利用していない. Defaults to ''.
+        mode (str, optional): マルチスレッドでsearchある程度共用で使えるようにするための引数. 利用していない. Defaults to ''.
     """
 
     # start search engine class
     se = SearchEngine()
 
     # Set Engine
     se.set(engine)
```

### Comparing `pydork-1.1.2/pydork/test_engine.py` & `pydork-1.1.4/pydork/test_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
 
 """test_engine_google
     * SearchEngine Classのテストコード.
     * 各検索エンジンの動作テストを行う
 """
```

### Comparing `pydork-1.1.2/pydork/test_engine_selenium.py` & `pydork-1.1.4/pydork/test_engine_selenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
 
 """test_engine_google
     * SearchEngine Classのテストコード.
     * 各検索エンジンの動作テストを行う
 """
```

### Comparing `pydork-1.1.2/pydork.egg-info/PKG-INFO` & `pydork-1.1.4/pydork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pydork
-Version: 1.1.2
+Version: 1.1.4
 Summary: Scraping and listing text and image searches on Google, Bing, DuckDuckGo, Baidu, Yahoo japan.
 Home-page: https://github.com/blacknon/pydork
 Author: blacknon
 Author-email: blacknon@orebibou.com
 Maintainer: blacknon
 Maintainer-email: blacknon@orebibou.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 
 PyDork
 ======
 
 Description
```

### Comparing `pydork-1.1.2/pydork.egg-info/SOURCES.txt` & `pydork-1.1.4/pydork.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 pydork/engine.py
 pydork/engine_baidu.py
 pydork/engine_bing.py
 pydork/engine_common.py
 pydork/engine_duckduckgo.py
 pydork/engine_google.py
 pydork/engine_yahoo.py
+pydork/engine_yandex.py
+pydork/messages.py
 pydork/recaptcha.py
-pydork/subcommands.py
+pydork/sub_commands.py
 pydork/test_engine.py
 pydork/test_engine_selenium.py
 pydork.egg-info/PKG-INFO
 pydork.egg-info/SOURCES.txt
 pydork.egg-info/dependency_links.txt
 pydork.egg-info/entry_points.txt
 pydork.egg-info/requires.txt
```

### Comparing `pydork-1.1.2/setup.py` & `pydork-1.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+# Copyright (c) 2023 Blacknon. All rights reserved.
+# Use of this source code is governed by an MIT license
+# that can be found in the LICENSE file.
 # =======================================================
 
 
 import os
 import platform
 
 import setuptools
@@ -75,16 +78,16 @@
     data_files = []
     data_files.append((loc['bash'], files['bash']))
     data_files.append((loc['zsh'], files['zsh']))
     return data_files
 
 
 name = 'pydork'
-version = '1.1.2'
-release = '1.1.2'
+version = '1.1.4'
+release = '1.1.4'
 
 if __name__ == "__main__":
     setuptools.setup(
         name=name,
         version=version,
         author='blacknon',
         author_email='blacknon@orebibou.com',
@@ -98,15 +101,15 @@
             'get-chrome-driver',
             'get-gecko-driver',
             'chromedriver_autoinstaller',
             'geckodriver_autoinstaller',
             'fake_useragent',
             'lxml',
             'requests[socks]',
-            'selenium',
+            'selenium==4.7.2',
             'selenium_requests',
             'pickle-mixin',
             'sphinx',
             'sphinx-rtd-theme',
             'sphinx-autobuild'
         ],
         url='https://github.com/blacknon/pydork',
@@ -118,14 +121,15 @@
             ],
         },
         classifiers=[
             'Programming Language :: Python :: 3',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
             'License :: OSI Approved :: MIT License',
         ],
         data_files=get_data_files(),
         cmdclass=cmdclass,
         command_options={
             'build_sphinx': {
                 'project': ('setup.py', name),
```

