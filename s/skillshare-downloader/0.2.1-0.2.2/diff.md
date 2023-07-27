# Comparing `tmp/skillshare_downloader-0.2.1.tar.gz` & `tmp/skillshare_downloader-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillshare_downloader-0.2.1.tar", max compression
+gzip compressed data, was "skillshare_downloader-0.2.2.tar", max compression
```

## Comparing `skillshare_downloader-0.2.1.tar` & `skillshare_downloader-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-07-21 06:55:00.000000 skillshare_downloader-0.2.1/LICENSE
--rw-r--r--   0        0        0     3240 2023-07-22 06:03:14.000000 skillshare_downloader-0.2.1/README.md
--rw-r--r--   0        0        0      637 2023-07-23 07:01:43.000000 skillshare_downloader-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-22 02:39:12.000000 skillshare_downloader-0.2.1/skillshare_downloader/__init__.py
--rw-r--r--   0        0        0       62 2023-07-22 04:58:55.000000 skillshare_downloader-0.2.1/skillshare_downloader/__main__.py
--rw-r--r--   0        0        0     6061 2023-07-23 07:11:13.000000 skillshare_downloader-0.2.1/skillshare_downloader/main.py
--rw-r--r--   0        0        0     2529 2023-07-19 05:02:18.000000 skillshare_downloader-0.2.1/skillshare_downloader/progress.py
--rw-r--r--   0        0        0    16425 2023-07-23 07:31:17.000000 skillshare_downloader-0.2.1/skillshare_downloader/skillshare.py
--rw-r--r--   0        0        0     4122 1970-01-01 00:00:00.000000 skillshare_downloader-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-21 06:55:00.000000 skillshare_downloader-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3519 2023-07-27 01:31:30.000000 skillshare_downloader-0.2.2/README.md
+-rw-r--r--   0        0        0      637 2023-07-27 01:33:03.000000 skillshare_downloader-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-22 02:39:12.000000 skillshare_downloader-0.2.2/skillshare_downloader/__init__.py
+-rw-r--r--   0        0        0       62 2023-07-22 04:58:55.000000 skillshare_downloader-0.2.2/skillshare_downloader/__main__.py
+-rw-r--r--   0        0        0     5756 2023-07-27 01:32:54.000000 skillshare_downloader-0.2.2/skillshare_downloader/main.py
+-rw-r--r--   0        0        0     2529 2023-07-19 05:02:18.000000 skillshare_downloader-0.2.2/skillshare_downloader/progress.py
+-rw-r--r--   0        0        0    16623 2023-07-27 01:21:59.000000 skillshare_downloader-0.2.2/skillshare_downloader/skillshare.py
+-rw-r--r--   0        0        0     4401 1970-01-01 00:00:00.000000 skillshare_downloader-0.2.2/PKG-INFO
```

### Comparing `skillshare_downloader-0.2.1/LICENSE` & `skillshare_downloader-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skillshare_downloader-0.2.1/README.md` & `skillshare_downloader-0.2.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -59,19 +59,23 @@
 
 ```
 The files are going to be downloaded locally and uploaded to Telegram after each file it's downloaded, but if you want to remove the file after upload, you can use [-e]
 ```bash
   $ down -r 1920x1080 1749908541 -t -e @yourgroup
 
 ```
-### UPDATE ---------
+### UPDATES ---------
 - Added automatic resume download
 - Added automatic resume uploads to Telegram on the same Topic
 - If the choosed resolution doesn't exist the script look for the next lower resolution
 - If the subtitles doesn't exist, now download the default en-US subtitles to avoid error
+## 0.2.1 -
+- Fixed an error related with missing video resolutions
+## 0.2.2 -
+- If the video doesn't exist (404) or the content it's Manifest not found (similar to 404 error) The video it's going to be skipped since doesn't exist, on the V 0.2.1 this just was causing an error.
 
 ## License
 This project is licensed under the MIT License.
 
 ## Acknowledgments
 This project was inspired by the need to download Skillshare videos for offline viewing.
```

### Comparing `skillshare_downloader-0.2.1/pyproject.toml` & `skillshare_downloader-0.2.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=1.1.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "skillshare_downloader"
-version = "0.2.1"
+version = "0.2.2"
 description = "A Python package to download Skillshare classes."
 readme = "README.md"  # Make sure you have a valid README.md file in the root of your project.
 license = "MIT"
 authors = ["Uriel Albarran Oropeza <hello@ozonostudio.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `skillshare_downloader-0.2.1/skillshare_downloader/main.py` & `skillshare_downloader-0.2.2/skillshare_downloader/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,41 +75,37 @@
 
         def format_help(self):
             instructions = """
     \033[1;35m=========== Instructions ===========\033[0m
 
     \033[91m YOU REQUIRE A SUBSCRIPTION, THIS CODE DOESN'T DOWNLOAD VIDEOS FOR PEOPLE WITHOUT AN ACTIVE SUBSCRIPTION ON SKILLSHARE \033[0m
 
-    \033[1mFollow these steps to make the code work:\033[0m
+    \033[1mFollow these steps to make the code work with Telegram if your don't already have it configurated:\033[0m
 
-    \033[33m1 - Open skillshare.com on Chrome and using the inspection window.\033[0m
-    \033[33m    1.1 - Go to network and select the \033[1mDoc filter\033[0m \033[0m
-    \033[33m    1.2 - Press the first document and inside the headers copy all the Cookies from the Request Headers\033[0m
-    \033[33m    1.3 - Paste the cookies into the file config.py\033[0m
-    \033[33m2 - If you have plans of backup your tutorials on Telegram you need to create an app:\033[0m
-    \033[33m    2.1 - Go to \033[1mhttps://my.telegram.org/auth\033[0m\033[0m
-    \033[33m    2.2 - Enter your phone number wtih the international prefix code\033[0m
-    \033[33m    2.3 - Click on \033[1mAPI development tools\033[0m\033[0m
-    \033[33m    2.5 - Create you App\033[0m
-    \033[33m    2.6 - use down -config to open the initial configuration\033[0m
-    \033[33m    2.7 - Copy and paste your App api_id, api_hash and your phone number when it's asked\033[0m
-    \033[33m3 - Run the script following the next template:\033[0m
+    \033[33m1 - If you have plans of backup your tutorials on Telegram you need to create an app:\033[0m
+    \033[33m    1.1 - Go to \033[1mhttps://my.telegram.org/auth\033[0m\033[0m
+    \033[33m    1.2 - Enter your phone number wtih the international prefix code\033[0m
+    \033[33m    1.3 - Click on \033[1mAPI development tools\033[0m\033[0m
+    \033[33m    1.5 - Create you App\033[0m
+    \033[33m    1.6 - use down -config to open the initial configuration\033[0m
+    \033[33m    1.7 - Copy and paste your App api_id, api_hash and your phone number when it's asked\033[0m
+    \033[33m2 - Run the script following the next template:\033[0m
 
     """
             help_text = super().format_help()
             help_text = help_text.replace("[-h] ", "").replace("[-config] ", "").strip()
             return instructions + help_text
         
     # parser = CustomArgumentParser()
     parser = CustomArgumentParser(prog='skillshare-download')  # Add "python" before the script name
     parser.add_argument('-h', '--help', action='help', help='show the current help')
     parser.add_argument('id', nargs='?', type=str, default=None, help='your class id, ex: 1749908541')
     parser.add_argument("-config", action="store_true", help="Configure the Skillshare Downloader")
     parser.add_argument('-s', type=str, default='en-US', choices=['es-MX', 'de', 'en-US', 'pt', 'fr'], help='Subtitles language (if nothing found subtitles are going to be downloaded as en-US)')
-    parser.add_argument('-r', type=str, default='854x480', choices=['1920x1080', '1280x720', '854x480', '640x360', '426x240'], help='Video resolution (if not found, the code it\'s going to search for the next lower resolution)')
+    parser.add_argument('-r', type=str, default='1920x1080', choices=['1920x1080', '1280x720', '854x480', '640x360', '426x240'], help='Video resolution (if not found, the code it\'s going to search for the next lower resolution)')
     parser.add_argument('-t', type=str, default=None, help='Your telegram group to save the files in format .mp4')
     parser.add_argument("-e", action="store_true", help="Erase the files after upload (only if there\'s a valid telegram group or id)")
 
     args = parser.parse_args()
     if args.config:
         configure()
         exit(0)
```

### Comparing `skillshare_downloader-0.2.1/skillshare_downloader/progress.py` & `skillshare_downloader-0.2.2/skillshare_downloader/progress.py`

 * *Files identical despite different names*

### Comparing `skillshare_downloader-0.2.1/skillshare_downloader/skillshare.py` & `skillshare_downloader-0.2.2/skillshare_downloader/skillshare.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,14 +227,18 @@
         response = requests.get(url)
         m3u8_content = response.text
         # print(m3u8_content)
         lines = m3u8_content.split("\n")
         output_file = os.path.join(base_path, file_name + '.' + format)
         base_url = os.path.dirname(url)
 
+        if m3u8_content == 'Manifest not found':
+            print(f'\033[91mThe stream content of {file_name} looks missing, and it\'s not possible to download it.\033[0m')
+            return
+
         if os.path.exists(output_file):
             print('File already exists. Skipping download:', file_name + '.' + format)
             if telegram is None:
                 return
             else:
                 try:
                     self.upload_to_telegram_group(output_file, telegram,file_name,topic_id)
```

### Comparing `skillshare_downloader-0.2.1/PKG-INFO` & `skillshare_downloader-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skillshare-downloader
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python package to download Skillshare classes.
 License: MIT
 Author: Uriel Albarran Oropeza
 Author-email: hello@ozonostudio.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -82,19 +82,23 @@
 
 ```
 The files are going to be downloaded locally and uploaded to Telegram after each file it's downloaded, but if you want to remove the file after upload, you can use [-e]
 ```bash
   $ down -r 1920x1080 1749908541 -t -e @yourgroup
 
 ```
-### UPDATE ---------
+### UPDATES ---------
 - Added automatic resume download
 - Added automatic resume uploads to Telegram on the same Topic
 - If the choosed resolution doesn't exist the script look for the next lower resolution
 - If the subtitles doesn't exist, now download the default en-US subtitles to avoid error
+## 0.2.1 -
+- Fixed an error related with missing video resolutions
+## 0.2.2 -
+- If the video doesn't exist (404) or the content it's Manifest not found (similar to 404 error) The video it's going to be skipped since doesn't exist, on the V 0.2.1 this just was causing an error.
 
 ## License
 This project is licensed under the MIT License.
 
 ## Acknowledgments
 This project was inspired by the need to download Skillshare videos for offline viewing.
```

