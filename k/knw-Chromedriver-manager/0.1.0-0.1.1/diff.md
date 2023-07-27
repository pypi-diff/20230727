# Comparing `tmp/knw_Chromedriver_manager-0.1.0.tar.gz` & `tmp/knw_Chromedriver_manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knw_Chromedriver_manager-0.1.0.tar", last modified: Thu Jul 27 00:16:34 2023, max compression
+gzip compressed data, was "knw_Chromedriver_manager-0.1.1.tar", last modified: Thu Jul 27 14:40:30 2023, max compression
```

## Comparing `knw_Chromedriver_manager-0.1.0.tar` & `knw_Chromedriver_manager-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 00:16:34.847388 knw_Chromedriver_manager-0.1.0/
--rw-rw-rw-   0        0        0     1854 2023-07-27 00:16:34.847388 knw_Chromedriver_manager-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1409 2023-07-27 00:05:49.000000 knw_Chromedriver_manager-0.1.0/README
-drwxrwxrwx   0        0        0        0 2023-07-27 00:16:34.834385 knw_Chromedriver_manager-0.1.0/knw_Chromedriver_manager/
--rw-rw-rw-   0        0        0     6045 2023-07-27 00:07:43.000000 knw_Chromedriver_manager-0.1.0/knw_Chromedriver_manager/Chromedriver_manager.py
--rw-rw-rw-   0        0        0        0 2023-07-26 15:28:35.000000 knw_Chromedriver_manager-0.1.0/knw_Chromedriver_manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 00:16:34.846388 knw_Chromedriver_manager-0.1.0/knw_Chromedriver_manager.egg-info/
--rw-rw-rw-   0        0        0     1854 2023-07-27 00:16:34.000000 knw_Chromedriver_manager-0.1.0/knw_Chromedriver_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-07-27 00:16:34.000000 knw_Chromedriver_manager-0.1.0/knw_Chromedriver_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 00:16:34.000000 knw_Chromedriver_manager-0.1.0/knw_Chromedriver_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-27 00:16:34.000000 knw_Chromedriver_manager-0.1.0/knw_Chromedriver_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 00:16:34.847388 knw_Chromedriver_manager-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-07-27 00:06:20.000000 knw_Chromedriver_manager-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:40:30.685951 knw_Chromedriver_manager-0.1.1/
+-rw-rw-rw-   0        0        0     1793 2023-07-27 14:40:30.684950 knw_Chromedriver_manager-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1348 2023-07-27 14:35:45.000000 knw_Chromedriver_manager-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 14:40:30.668947 knw_Chromedriver_manager-0.1.1/knw_Chromedriver_manager/
+-rw-rw-rw-   0        0        0     8197 2023-07-27 14:36:43.000000 knw_Chromedriver_manager-0.1.1/knw_Chromedriver_manager/Chromedriver_manager.py
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:28:35.000000 knw_Chromedriver_manager-0.1.1/knw_Chromedriver_manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 14:40:30.683951 knw_Chromedriver_manager-0.1.1/knw_Chromedriver_manager.egg-info/
+-rw-rw-rw-   0        0        0     1793 2023-07-27 14:40:30.000000 knw_Chromedriver_manager-0.1.1/knw_Chromedriver_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-27 14:40:30.000000 knw_Chromedriver_manager-0.1.1/knw_Chromedriver_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 14:40:30.000000 knw_Chromedriver_manager-0.1.1/knw_Chromedriver_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-27 14:40:30.000000 knw_Chromedriver_manager-0.1.1/knw_Chromedriver_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-27 14:40:30.000000 knw_Chromedriver_manager-0.1.1/knw_Chromedriver_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 14:40:30.685951 knw_Chromedriver_manager-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      741 2023-07-27 14:40:01.000000 knw_Chromedriver_manager-0.1.1/setup.py
```

### Comparing `knw_Chromedriver_manager-0.1.0/PKG-INFO` & `knw_Chromedriver_manager-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 Metadata-Version: 2.1
 Name: knw_Chromedriver_manager
-Version: 0.1.0
+Version: 0.1.1
 Summary: Chromedriver_manager for knw
 Home-page: https://github.com/daumsong/knw_webdriver_manager
 Author: OH nam kyun
 Author-email: daumsong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Chromedriver_manager for knw / By archon.oh
 
 
-#####################################
-
-[install]
+############# [install] #############
 
 pip install knw-Chromedriver-manager
 
 #####################################
 
-#############################################################################################
 
-[window use sample code]
+################################# [window use sample code] ##################################
 
 from knw_Chromedriver_manager import Chromedriver_manager
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 options = Options()
-driver = webdriver.Chrome(service=Service(Chromedriver_manager.install()), options=options)
+driver = webdriver.Chrome(service= Service(Chromedriver_manager.install()), options=options)
 driver.get("https://www.daum.net/")
 
 #############################################################################################
 
 
-#############################################################################################
-
-[mac use sample code]
+###################################### [mac use sample code] ################################
 
 from knw_Chromedriver_manager import Chromedriver_manager
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 options = Options()
-options.binary_location=Chromedriver_manager.path_check() # add code
+options.binary_location = Chromedriver_manager.path_check() # add code
 driver = webdriver.Chrome(service=Service(Chromedriver_manager.install()), options=options)
 driver.get("https://www.daum.net/")
 
 #############################################################################################
```

### Comparing `knw_Chromedriver_manager-0.1.0/README` & `knw_Chromedriver_manager-0.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 Chromedriver_manager for knw / By archon.oh
 
 
-#####################################
-
-[install]
+############# [install] #############
 
 pip install knw-Chromedriver-manager
 
 #####################################
 
-#############################################################################################
 
-[window use sample code]
+################################# [window use sample code] ##################################
 
 from knw_Chromedriver_manager import Chromedriver_manager
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 options = Options()
-driver = webdriver.Chrome(service=Service(Chromedriver_manager.install()), options=options)
+driver = webdriver.Chrome(service= Service(Chromedriver_manager.install()), options=options)
 driver.get("https://www.daum.net/")
 
 #############################################################################################
 
 
-#############################################################################################
-
-[mac use sample code]
+###################################### [mac use sample code] ################################
 
 from knw_Chromedriver_manager import Chromedriver_manager
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 options = Options()
-options.binary_location=Chromedriver_manager.path_check() # add code
+options.binary_location = Chromedriver_manager.path_check() # add code
 driver = webdriver.Chrome(service=Service(Chromedriver_manager.install()), options=options)
 driver.get("https://www.daum.net/")
 
 #############################################################################################
```

### Comparing `knw_Chromedriver_manager-0.1.0/knw_Chromedriver_manager/Chromedriver_manager.py` & `knw_Chromedriver_manager-0.1.1/knw_Chromedriver_manager/Chromedriver_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -85,64 +85,91 @@
             if file_name == 'chromedriver.exe':
                 return os.path.join(chromedriver_folder, file_name)
 
     #크롬드라이버 목록 받아오기
     response = requests.get(
         'https://googlechromelabs.github.io/chrome-for-testing/latest-patch-versions-per-build-with-downloads.json')  # https://github.com/GoogleChromeLabs/chrome-for-testing#json-api-endpoints
     version_json_data = json.loads(response.text)
-    # json "builds"에서 버전 version[:4] 의 모든 버전 json추출 ex: 115.
-    main_versions = [key for key in version_json_data["builds"].keys() if key.startswith(version[:4])]
+    # json "builds"에서 버전 3째단까지의 숫자에 해당하는 모든 버전 리스트 추출 ex: ['115.0.1000','115.0.1000','115.0.1000'] 추후 뒷단 버전숫자까지 추가 됬을 경우 대비
+    main_versions = [key for key in version_json_data["builds"].keys() if key.startswith(version)]
 
-    # 버전 숫자를 기준으로 정렬하여 최신 버전을 얻음
-    latest_main_versions = sorted(main_versions, key=lambda x: list(map(int, x.split("."))))[-1]
+    first_version_value = re.search(r'^\d+', version).group(0)
+    if first_version_value == "114":
+        pass
+    else:
+        try:
+            # 버전 3째단까지의 숫자를 기준으로 정렬하여 해당앞단의 최신 버전값 추출 ex. 114.0.5735
+            latest_main_versions = sorted(main_versions, key=lambda x: list(map(int, x.split("."))))[-1]
+            # print("latest_main_versions",latest_main_versions)
+            # 해당버전의 최신 버전 chromedriver json 추출
+            latest_main_versions_json = version_json_data['builds'][latest_main_versions]['downloads']['chromedriver']
+        except:
+            #stable. 즉 현재 최신제공 버전의 드라이버 크롬드라이버 목록 받아오기
+            response = requests.get(
+                'https://googlechromelabs.github.io/chrome-for-testing/last-known-good-versions-with-downloads.json')  # https://github.com/GoogleChromeLabs/chrome-for-testing#json-api-endpoints
+            version_json_data = json.loads(response.text)
+            latest_main_versions_json = version_json_data["channels"]["Stable"]['downloads']['chromedriver']
 
-    # 최신 버전의 URL 추출
-    latest_main_versions_json = version_json_data['builds'][latest_main_versions]['downloads']['chromedriver']
 
     download_url = ''
-
-    if os_name == "Windows" and bit_value == "64bit": #윈도우 64비트
-        for kinds in latest_main_versions_json:
-            if kinds['platform'] == "win64":
-                download_url = kinds['url']
-    elif os_name == "Windows" and bit_value == "32bit": #윈도우 32비트
-        for kinds in latest_main_versions_json:
-            if kinds['platform'] == "win32":
-                download_url = kinds['url']
-    elif os_name == "Darwin" and processor == "x86_64": #인텔 맥
-        for kinds in latest_main_versions_json:
-            if kinds['platform'] == "mac-x64":#mac-x64
-                download_url = kinds['url']
-    elif os_name == "Darwin" and processor == "arm64": # 암 맥
-        for kinds in latest_main_versions_json:
-            if kinds['platform'] == "mac-arm64":
-                download_url = kinds['url']
-    else: # 리눅스
-        for kinds in latest_main_versions_json:
-            if kinds['platform'] == "linux64":
-                download_url = kinds['url']
+    if first_version_value == "114":
+        if os_name == "Windows" and bit_value == "64bit":  # 윈도우 64비트
+            download_url = "https://chromedriver.storage.googleapis.com/114.0.5735.90/chromedriver_win32.zip"
+        elif os_name == "Windows" and bit_value == "32bit":  # 윈도우 32비트
+            download_url = "https://chromedriver.storage.googleapis.com/114.0.5735.90/chromedriver_win32.zip"
+        elif os_name == "Darwin" and processor == "x86_64":  # 인텔 맥
+            download_url = "https://chromedriver.storage.googleapis.com/114.0.5735.90/chromedriver_mac64.zip"
+        elif os_name == "Darwin" and processor == "arm64":  # 암 맥
+            download_url = "https://chromedriver.storage.googleapis.com/114.0.5735.90/chromedriver_mac_arm64.zip"
+        else:  # 리눅스
+            download_url = "https://chromedriver.storage.googleapis.com/114.0.5735.90/chromedriver_linux64.zip"
+    else:
+        if os_name == "Windows" and bit_value == "64bit":  # 윈도우 64비트
+            for kinds in latest_main_versions_json:
+                if kinds['platform'] == "win64":
+                    download_url = kinds['url']
+        elif os_name == "Windows" and bit_value == "32bit":  # 윈도우 32비트
+            for kinds in latest_main_versions_json:
+                if kinds['platform'] == "win32":
+                    download_url = kinds['url']
+        elif os_name == "Darwin" and processor == "x86_64":  # 인텔 맥
+            for kinds in latest_main_versions_json:
+                if kinds['platform'] == "mac-x64":  # mac-x64
+                    download_url = kinds['url']
+        elif os_name == "Darwin" and processor == "arm64":  # 암 맥
+            for kinds in latest_main_versions_json:
+                if kinds['platform'] == "mac-arm64":
+                    download_url = kinds['url']
+        else:  # 리눅스
+            for kinds in latest_main_versions_json:
+                if kinds['platform'] == "linux64":
+                    download_url = kinds['url']
 
     #크롬드라이버 다운로드
     response = requests.get(download_url)
     file_path = os.path.join(chromedriver_folder, 'chromedriver.zip')
     # 압축파일 다운로드
     with open(file_path, 'wb') as f:
         f.write(response.content)
 
+    if first_version_value == "114":
+        file_reg = r'^chromedriver.*'
+    else:
+        file_reg = r'^chromedriver.*\/chromedriver'
+
     # 압축 풀기
     with zipfile.ZipFile(file_path, 'r') as zip_ref:
         for member in zip_ref.namelist():
-            if re.search(r'^chromedriver.*\/chromedriver', member):
+            if re.search(file_reg, member):
                 filename = os.path.basename(member)
                 source = zip_ref.open(member)
                 target = open(os.path.join(chromedriver_folder, filename), "wb")
                 with source, target:
                     shutil.copyfileobj(source, target)
                     if os_name == 'Darwin':
                         os.chmod(os.path.join(chromedriver_folder, filename), 0o700) #권한부여
                     return os.path.join(chromedriver_folder, filename)
 
 def install():
     version = get_chrome_version()
-    install_path = download(version[:-4])
-    return install_path
-
+    install_path = download(re.search(r'(\d+\.\d+\.\d+)', version).group(0))
+    return install_path
```

### Comparing `knw_Chromedriver_manager-0.1.0/knw_Chromedriver_manager.egg-info/PKG-INFO` & `knw_Chromedriver_manager-0.1.1/knw_Chromedriver_manager.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 Metadata-Version: 2.1
 Name: knw-Chromedriver-manager
-Version: 0.1.0
+Version: 0.1.1
 Summary: Chromedriver_manager for knw
 Home-page: https://github.com/daumsong/knw_webdriver_manager
 Author: OH nam kyun
 Author-email: daumsong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Chromedriver_manager for knw / By archon.oh
 
 
-#####################################
-
-[install]
+############# [install] #############
 
 pip install knw-Chromedriver-manager
 
 #####################################
 
-#############################################################################################
 
-[window use sample code]
+################################# [window use sample code] ##################################
 
 from knw_Chromedriver_manager import Chromedriver_manager
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 options = Options()
-driver = webdriver.Chrome(service=Service(Chromedriver_manager.install()), options=options)
+driver = webdriver.Chrome(service= Service(Chromedriver_manager.install()), options=options)
 driver.get("https://www.daum.net/")
 
 #############################################################################################
 
 
-#############################################################################################
-
-[mac use sample code]
+###################################### [mac use sample code] ################################
 
 from knw_Chromedriver_manager import Chromedriver_manager
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 options = Options()
-options.binary_location=Chromedriver_manager.path_check() # add code
+options.binary_location = Chromedriver_manager.path_check() # add code
 driver = webdriver.Chrome(service=Service(Chromedriver_manager.install()), options=options)
 driver.get("https://www.daum.net/")
 
 #############################################################################################
```

### Comparing `knw_Chromedriver_manager-0.1.0/setup.py` & `knw_Chromedriver_manager-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import setuptools
 
-with open("README", "r") as fh:
+with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="knw_Chromedriver_manager",
-    version="0.1.0",
+    version="0.1.1",
+    install_requires=[
+        "requests",
+    ],
     author="OH nam kyun",
     author_email="daumsong@gmail.com",
     description="Chromedriver_manager for knw",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/daumsong/knw_webdriver_manager",
     packages=setuptools.find_packages(),
```

