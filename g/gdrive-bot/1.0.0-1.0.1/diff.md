# Comparing `tmp/gdrive_bot-1.0.0-py3-none-any.whl.zip` & `tmp/gdrive_bot-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6924 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 22-Aug-22 15:35 g_bot/__inti__.py
--rw-r--r--  2.0 unx     2114 b- defN 23-Jul-27 03:38 g_bot/cli.py
--rw-r--r--  2.0 unx       68 b- defN 23-Jul-27 03:14 g_bot/config.ini
--rw-r--r--  2.0 unx     7695 b- defN 23-Jul-27 03:38 g_bot/main.py
--rwxrwxrwx  2.0 unx     1064 b- defN 23-Jul-27 03:43 gdrive_bot-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2416 b- defN 23-Jul-27 03:43 gdrive_bot-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 03:43 gdrive_bot-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 23-Jul-27 03:43 gdrive_bot-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-27 03:43 gdrive_bot-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      779 b- defN 23-Jul-27 03:43 gdrive_bot-1.0.0.dist-info/RECORD
-10 files, 14275 bytes uncompressed, 5592 bytes compressed:  60.8%
+Zip file size: 6214 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-27 10:13 g_bot/__init__.py
+-rw-r--r--  2.0 unx     1925 b- defN 23-Jul-27 10:13 g_bot/cli.py
+-rw-r--r--  2.0 unx       68 b- defN 23-Jul-27 10:13 g_bot/config.ini
+-rw-r--r--  2.0 unx     6439 b- defN 23-Jul-27 10:13 g_bot/main.py
+-rwxr-xr-x  2.0 unx     1064 b- defN 23-Jul-27 10:13 gdrive_bot-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1449 b- defN 23-Jul-27 10:13 gdrive_bot-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 10:13 gdrive_bot-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-27 10:13 gdrive_bot-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-27 10:13 gdrive_bot-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      780 b- defN 23-Jul-27 10:13 gdrive_bot-1.0.1.dist-info/RECORD
+10 files, 11886 bytes uncompressed, 4882 bytes compressed:  58.9%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
-Filename: g_bot/__inti__.py
+Filename: g_bot/__init__.py
 Comment: 
 
 Filename: g_bot/cli.py
 Comment: 
 
 Filename: g_bot/config.ini
 Comment: 
 
 Filename: g_bot/main.py
 Comment: 
 
-Filename: gdrive_bot-1.0.0.dist-info/LICENSE
+Filename: gdrive_bot-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: gdrive_bot-1.0.0.dist-info/METADATA
+Filename: gdrive_bot-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: gdrive_bot-1.0.0.dist-info/WHEEL
+Filename: gdrive_bot-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: gdrive_bot-1.0.0.dist-info/entry_points.txt
+Filename: gdrive_bot-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: gdrive_bot-1.0.0.dist-info/top_level.txt
+Filename: gdrive_bot-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: gdrive_bot-1.0.0.dist-info/RECORD
+Filename: gdrive_bot-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## g_bot/cli.py

```diff
@@ -1,14 +1,14 @@
 import os
 import argparse
 import configparser
 
+from g_bot import __version__
 from g_bot.main import setup, reset, upload_file, download, config_file
 
-__version__ = "1.0.0"
 package_name = "g-bot"
 
 config = configparser.ConfigParser()
 config.read(config_file)
 access_token = config['GDRIVE']['access_token']
 folder_id = config["GDRIVE"]['folder_id']
 if folder_id == 'xxxxxxxxxxxxx':
@@ -30,18 +30,14 @@
 
 	upload_parser = subparsers.add_parser("up", help="upload file to your group or channel")
 	upload_parser.add_argument("filename", type=str, help="one or more files to upload")
 
 	download_parser = subparsers.add_parser("d", help="download and upload file to your group or channel")
 	download_parser.add_argument("url", type=str, help="url")
 
-	files_parser = subparsers.add_parser("files", help="Show all available files 'downloads' folder")
-
-	delete_parser = subparsers.add_parser("del", help="delete available files 'downloads' folder")
-
 	parser.add_argument('-v',"--version",
 							action="store_true",
 							dest="version",
 							help="check version of g-bot")
 
 	args = parser.parse_args(argv)
```

## g_bot/main.py

```diff
@@ -9,14 +9,15 @@
 from pathlib import Path
 from shutil import copy2
 import requests_toolbelt
 import urllib.parse as urlparse
 from requests.exceptions import JSONDecodeError
 from requests.exceptions import MissingSchema
 from requests import get, ConnectionError, head
+
 urllib3.disable_warnings()
 
 base_dir = os.path.dirname(os.path.realpath(__file__))
 config = os.path.join(base_dir, 'config.ini')
 
 home_path = Path.home()
 if os.path.isfile(os.path.join(home_path, ".config/g-bot/config.ini")):
@@ -190,48 +191,7 @@
         filename = input("Enter new filename : ")
         file_path = os.path.join(download_path, filename)
         downloader(url, file_path)
     
     print("\nUploading file......")
     filedirectory = f"downloads/{filename}"
     upload_file(access_token, filename, filedirectory, folder_id)
-
-def files():
-    try:
-        files = os.listdir('downloads')
-    except FileNotFoundError:
-        sys.exit('Directory "downloads" not found !')
-    if files != []:
-        print("id -> File Name")
-        i = 0
-        for file in files:
-            i += 1
-            print(f"{i} -> {file[0:55]}")
-
-def delete():
-    try:
-        files = os.listdir('downloads')
-    except FileNotFoundError:
-        sys.exit('Directory "downloads" not found !')
-    if files != []:
-        print("\nId ->  File Name")
-        i = 0
-        for file in files:
-            i += 1
-            print(f"{i}  ->  {file[0:55]}")
-
-        num_of_files = len(files)
-        inputs = list(map(str, input(f"\nSelect file number [1-{num_of_files}] seprated by commasm, or 'all':").split(sep=",")))
-        print(inputs)
-        if inputs == ['all']:
-            print("all")
-        try:
-            isdigits = all(isinstance(int(x), int) for x in inputs)
-        except ValueError:
-            sys.exit("Invalid input !")
-        if isdigits:
-            for x in inputs:
-                try:
-                    print(files[int(x)-1])
-                    os.remove(f"downloads/{files[int(x)-1]}")
-                except IndexError:
-                    print(f"Id {x} not found")
```

## Comparing `gdrive_bot-1.0.0.dist-info/LICENSE` & `gdrive_bot-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gdrive_bot-1.0.0.dist-info/METADATA` & `gdrive_bot-1.0.1.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,47 @@
 Metadata-Version: 2.1
 Name: gdrive-bot
-Version: 1.0.0
+Version: 1.0.1
 Summary: upload files to gdrive with access token
 Home-page: https://github.com/jakbin/g-bot
 Author: Jak Bin
 Author-email: jakbin4747@gmail.com
 Project-URL: Bug Tracker, https://github.com/jakbin/g-bot/issues
 Keywords: gdrive,g-bot,gdrive-api,gdrive-api-bot,gdrive-file-upload,gdrive-upload
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: tqdm
 Requires-Dist: requests
 Requires-Dist: requests-toolbelt
-Requires-Dist: tqdm
 
-# g-bot
+# gdrive-bot
 
-Upload files to your Telegram channel or group with your telegram bot
+Upload files to your gdrive with your gdrive bot
 
- ![GitHub Contributors](https://img.shields.io/github/contributors/jakbin/g-bot)
- ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/jakbin/g-bot)
- ![GitHub last commit](https://img.shields.io/github/last-commit/jakbin/g-bot)
+ ![GitHub Contributors](https://img.shields.io/github/contributors/jakbin/gdrive-bot)
+ ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/jakbin/gdrive-bot)
+ ![GitHub last commit](https://img.shields.io/github/last-commit/jakbin/gdrive-bot)
  ![Python 3.6](https://img.shields.io/badge/python-3.6-yellow.svg)
 
 
 ## Features
 - Progress bar
-- You can change file name before upload on telegram
-
-Note : Bot can upload only 50 MB file (with default telegram bot api server url)
 
 
 ## Installation
 
 ```sh
-pip3 install -U https://github.com/jakbin/g-bot/archive/main.zip
+pip3 install -U gdrive-bot
 ```
 
 ## Usage 
 ```sh
-g-bot setup               # setup your telegram credentials
-g-bot reset               # reset to default your telegram credentials
-g-bot test                # test telegram bot token
-g-bot getid               # get chat id of your connected group or channel
-g-bot up {file_name} -c file_caption       # upload Telegram channel or group
-g-bot d {url} -c caption                   # download and file to your server
-```
-
-# API
-
-The anonfile-upload client is also usable through an API (for test integration, automation, etc)
-
-### g_bot.main.test_token(bot_token)
-
-```py
-from g_bot.main import test_token
-
-test_token(bot_token)   # bot_token type str
-```
-
-### g_bot.main.uploadd_file(bot_token, chat_id, file_name, caption)
-
-```py
-from g_bot.main import uploadd_file
-
-uploadd_file(bot_token, chat_id, file_name, caption)    # all arguments must be str
-```
-
-### g_bot.main.download(url:str, bot_token:str, chat_id:str, caption:str=None)
-
-```py
-from g_bot.main import download
-
-download(url, bot_token, chat_id, caption)    # all arguments must be str
+g-bot setup               # setup your gdrive credentials
+g-bot reset               # reset to default your gdrive credentials
+g-bot up {file_name}      # upload gdrive channel or group
+g-bot d {url}             # download and upload file to your gdrive
 ```
```

