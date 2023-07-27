# Comparing `tmp/webdriver_manager-3.9.1.tar.gz` & `tmp/webdriver_manager-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/webdriver_manager-3.9.1.tar", last modified: Sun Jul 23 15:07:42 2023, max compression
+gzip compressed data, was "dist/webdriver_manager-4.0.0.tar", last modified: Thu Jul 27 12:18:08 2023, max compression
```

## Comparing `webdriver_manager-3.9.1.tar` & `webdriver_manager-4.0.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/tests/test_brave_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/tests/test_chrome_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/tests/test_chromium_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/tests/test_custom_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/tests/test_custom_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/tests/test_edge_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/tests/test_firefox_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/tests/test_ie_driver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2974 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/tests/test_opera_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/tests/test_silent_global_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/webdriver_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/chrome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/webdriver_manager/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/driver_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/os_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/webdriver_manager/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/drivers/chrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/drivers/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/drivers/firefox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/drivers/ie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/drivers/opera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/firefox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/microsoft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/opera.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 15:07:13.000000 webdriver_manager-3.9.1/webdriver_manager/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/webdriver_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/webdriver_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/webdriver_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/webdriver_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/webdriver_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-23 15:07:42.000000 webdriver_manager-3.9.1/webdriver_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/tests/test_brave_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/tests/test_chrome_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/tests/test_chromium_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/tests/test_custom_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/tests/test_custom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/tests/test_edge_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/tests/test_firefox_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/tests/test_ie_driver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2974 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/tests/test_opera_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/tests/test_silent_global_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/webdriver_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/chrome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/webdriver_manager/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/driver_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/os_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/webdriver_manager/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/drivers/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/drivers/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/drivers/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/drivers/ie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/drivers/opera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/firefox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/microsoft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/opera.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:17:40.000000 webdriver_manager-4.0.0/webdriver_manager/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/webdriver_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/webdriver_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/webdriver_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/webdriver_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/webdriver_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 12:18:08.000000 webdriver_manager-4.0.0/webdriver_manager.egg-info/top_level.txt
```

### Comparing `webdriver_manager-3.9.1/LICENSE` & `webdriver_manager-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/PKG-INFO` & `webdriver_manager-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver_manager
-Version: 3.9.1
+Version: 4.0.0
 Summary: Library provides the way to automatically manage drivers for different browsers
 Home-page: https://github.com/SergeyPirogov/webdriver_manager
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Keywords: testing,selenium,driver,test automation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Information Technology
```

### Comparing `webdriver_manager-3.9.1/README.md` & `webdriver_manager-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/setup.py` & `webdriver_manager-4.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 setuptools.setup(
     name='webdriver_manager',
     python_requires=">=3.7",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(include=['webdriver_manager*']),
     include_package_data=True,
-    version='3.9.1',
+    version='4.0.0',
     description='Library provides the way to automatically manage drivers for different browsers',
     author='Sergey Pirogov',
     author_email='automationremarks@gmail.com',
     url='https://github.com/SergeyPirogov/webdriver_manager',
     keywords=['testing', 'selenium', 'driver', 'test automation'],
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `webdriver_manager-3.9.1/tests/test_brave_driver.py` & `webdriver_manager-4.0.0/tests/test_brave_driver.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/tests/test_chrome_driver.py` & `webdriver_manager-4.0.0/tests/test_chrome_driver.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 
 import pytest
+import browsers
 from selenium import webdriver
 
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.constants import ROOT_FOLDER_NAME
 from selenium.webdriver.chrome.service import Service
 
 from webdriver_manager.core.driver_cache import DriverCacheManager
@@ -47,16 +48,18 @@
 def test_chrome_manager_with_wrong_version():
     with pytest.raises(ValueError) as ex:
         ChromeDriverManager("0.2").install()
     assert "There is no such driver by url" in ex.value.args[0]
 
 
 def test_chrome_manager_with_selenium():
+    options = webdriver.ChromeOptions()
+    options.binary_location = browsers.get("chrome")["path"]
     driver_path = ChromeDriverManager().install()
-    driver = webdriver.Chrome(service=Service(driver_path))
+    driver = webdriver.Chrome(service=Service(driver_path), options=options)
     driver.get("http://automation-remarks.com")
     driver.close()
 
 
 def test_driver_with_ssl_verify_disabled_can_be_downloaded(ssl_verify_enable):
     os.environ['WDM_SSL_VERIFY'] = '0'
     custom_path = os.path.join(os.path.dirname(
@@ -65,17 +68,19 @@
     )
     driver_path = ChromeDriverManager(cache_manager=DriverCacheManager(custom_path)).install()
     os.environ['WDM_SSL_VERIFY'] = '1'
     assert os.path.exists(driver_path)
 
 
 def test_chrome_manager_cached_driver_with_selenium():
+    options = webdriver.ChromeOptions()
+    options.binary_location = browsers.get("chrome")["path"]
     custom_path = os.path.join(os.path.dirname(os.path.dirname(__file__)), "custom-cache")
     manager = ChromeDriverManager(cache_manager=DriverCacheManager(custom_path))
-    driver = webdriver.Chrome(service=Service(manager.install()))
+    driver = webdriver.Chrome(service=Service(manager.install()), options=options)
     driver.get("http://automation-remarks.com")
 
     metadata_file = os.path.join(custom_path, ROOT_FOLDER_NAME, 'drivers.json')
 
     with open(metadata_file) as json_file:
         data = json.load(json_file)
```

### Comparing `webdriver_manager-3.9.1/tests/test_chromium_driver.py` & `webdriver_manager-4.0.0/tests/test_chromium_driver.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/tests/test_custom_http_client.py` & `webdriver_manager-4.0.0/tests/test_custom_http_client.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/tests/test_custom_logger.py` & `webdriver_manager-4.0.0/tests/test_custom_logger.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/tests/test_downloader.py` & `webdriver_manager-4.0.0/tests/test_downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from webdriver_manager.core.constants import DEFAULT_PROJECT_ROOT_CACHE_PATH
 from webdriver_manager.core.download_manager import WDMDownloadManager
 from webdriver_manager.core.file_manager import FileManager
 from webdriver_manager.core.http import WDMHttpClient
 from webdriver_manager.core.os_manager import OperationSystemManager, ChromeType
 from webdriver_manager.drivers.chrome import ChromeDriver
 
+os_manager = OperationSystemManager()
 download_manager = WDMDownloadManager()
-file_manager = FileManager(OperationSystemManager())
+file_manager = FileManager(os_manager)
 
 
 def test_can_download_driver_as_zip_file(delete_drivers_dir):
     file = download_manager.download_file("http://chromedriver.storage.googleapis.com/2.26/chromedriver_win32.zip")
     assert file.filename == "chromedriver_win32.zip"
     archive = file_manager.save_archive_file(file, DEFAULT_PROJECT_ROOT_CACHE_PATH)
     assert archive.file_path == f"{DEFAULT_PROJECT_ROOT_CACHE_PATH}{os.sep}{file.filename}"
@@ -28,18 +29,19 @@
     archive = file_manager.save_archive_file(file, DEFAULT_PROJECT_ROOT_CACHE_PATH)
     assert archive.file_path == f"{DEFAULT_PROJECT_ROOT_CACHE_PATH}{os.sep}{file.filename}"
     assert file_manager.unpack_archive(archive, DEFAULT_PROJECT_ROOT_CACHE_PATH) == ["geckodriver"]
 
 
 @pytest.mark.parametrize('version', ["2.26"])
 def test_can_download_chrome_driver(delete_drivers_dir, version):
+    os_sys_manager = OperationSystemManager("win32")
     driver = ChromeDriver(name="chromedriver",
                           driver_version=version,
-                          os_system_manager=OperationSystemManager("win32"),
+                          os_system_manager=os_sys_manager,
                           url="http://chromedriver.storage.googleapis.com",
                           latest_release_url="http://chromedriver.storage.googleapis.com/LATEST_RELEASE",
                           chrome_type=ChromeType.GOOGLE, http_client=WDMHttpClient())
 
-    file = download_manager.download_file(driver.get_driver_download_url())
+    file = download_manager.download_file(driver.get_driver_download_url(os_sys_manager.get_os_type()))
     assert file.filename == "chromedriver_win32.zip"
     archive = file_manager.save_archive_file(file, DEFAULT_PROJECT_ROOT_CACHE_PATH)
     assert "chromedriver.exe" in file_manager.unpack_archive(archive, DEFAULT_PROJECT_ROOT_CACHE_PATH)
```

### Comparing `webdriver_manager-3.9.1/tests/test_edge_driver.py` & `webdriver_manager-4.0.0/tests/test_edge_driver.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/tests/test_firefox_manager.py` & `webdriver_manager-4.0.0/tests/test_firefox_manager.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/tests/test_ie_driver.py` & `webdriver_manager-4.0.0/tests/test_ie_driver.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/tests/test_opera_manager.py` & `webdriver_manager-4.0.0/tests/test_opera_manager.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/tests/test_utils.py` & `webdriver_manager-4.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/webdriver_manager/chrome.py` & `webdriver_manager-4.0.0/webdriver_manager/firefox.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 import os
 from typing import Optional
 
 from webdriver_manager.core.download_manager import DownloadManager
 from webdriver_manager.core.driver_cache import DriverCacheManager
 from webdriver_manager.core.manager import DriverManager
-from webdriver_manager.core.os_manager import OperationSystemManager, ChromeType
-from webdriver_manager.drivers.chrome import ChromeDriver
+from webdriver_manager.core.os_manager import OperationSystemManager
+from webdriver_manager.drivers.firefox import GeckoDriver
 
 
-class ChromeDriverManager(DriverManager):
+class GeckoDriverManager(DriverManager):
     def __init__(
             self,
-            driver_version: Optional[str] = None,
-            name: str = "chromedriver",
-            url: str = "https://chromedriver.storage.googleapis.com",
-            latest_release_url: str = "https://chromedriver.storage.googleapis.com/LATEST_RELEASE",
-            chrome_type: str = ChromeType.GOOGLE,
+            version: Optional[str] = None,
+            name: str = "geckodriver",
+            url: str = "https://github.com/mozilla/geckodriver/releases/download",
+            latest_release_url: str = "https://api.github.com/repos/mozilla/geckodriver/releases/latest",
+            mozila_release_tag: str = "https://api.github.com/repos/mozilla/geckodriver/releases/tags/{0}",
             download_manager: Optional[DownloadManager] = None,
             cache_manager: Optional[DriverCacheManager] = None,
             os_system_manager: Optional[OperationSystemManager] = None
     ):
-        super().__init__(
+        super(GeckoDriverManager, self).__init__(
             download_manager=download_manager,
             cache_manager=cache_manager
         )
 
-        self.driver = ChromeDriver(
+        self.driver = GeckoDriver(
+            driver_version=version,
             name=name,
-            driver_version=driver_version,
             url=url,
             latest_release_url=latest_release_url,
-            chrome_type=chrome_type,
+            mozila_release_tag=mozila_release_tag,
             http_client=self.http_client,
             os_system_manager=os_system_manager
         )
 
     def install(self) -> str:
         driver_path = self._get_driver_binary_path(self.driver)
-        if all(test_os not in driver_path for test_os in ["mac_arm64", "mac_x64"]):
-            os.chmod(driver_path, 0o755)
+        os.chmod(driver_path, 0o755)
         return driver_path
+
+    def get_os_type(self):
+        os_type = super().get_os_type()
+        if not self._os_system_manager.is_mac_os(os_type):
+            return os_type
+
+        macos = 'macos'
+        if self._os_system_manager.is_arch(os_type):
+            return f"{macos}-aarch64"
+        return macos
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/core/archive.py` & `webdriver_manager-4.0.0/webdriver_manager/core/archive.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import os
-import tarfile
 import zipfile
-import typing
 
 
 class LinuxZipFileWithPermissions(zipfile.ZipFile):
     """Class for extract files in linux with right permissions"""
 
     def extract(self, member, path=None, pwd=None):
         if not isinstance(member, zipfile.ZipInfo):
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/core/config.py` & `webdriver_manager-4.0.0/webdriver_manager/core/config.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/webdriver_manager/core/download_manager.py` & `webdriver_manager-4.0.0/webdriver_manager/core/download_manager.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/webdriver_manager/core/driver.py` & `webdriver_manager-4.0.0/webdriver_manager/core/driver.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 from webdriver_manager.core.os_manager import OperationSystemManager
 
 
 class Driver(object):
     def __init__(
             self,
             name,
-            driver_version,
+            driver_version_to_download,
             url,
             latest_release_url,
             http_client,
             os_system_manager):
         self._name = name
         self._url = url
-        self._driver_version = driver_version
         self._latest_release_url = latest_release_url
         self._http_client = http_client
         self._browser_version = None
-        self._driver_to_download_version = None
+        self._driver_version_to_download = driver_version_to_download
         self._os_system_manager = os_system_manager
         if not self._os_system_manager:
             self._os_system_manager = OperationSystemManager()
 
     @property
     def auth_header(self):
         token = gh_token()
@@ -30,30 +29,27 @@
             log("GH_TOKEN will be used to perform requests")
             return {"Authorization": f"token {token}"}
         return None
 
     def get_name(self):
         return self._name
 
-    def get_os_type(self):
-        return self._os_system_manager.get_os_type()
-
-    def get_driver_download_url(self):
-        return f"{self._url}/{self.get_driver_version_to_download()}/{self._name}_{self.get_os_type()}.zip"
+    def get_driver_download_url(self, os_type):
+        return f"{self._url}/{self.get_driver_version_to_download()}/{self._name}_{os_type}.zip"
 
     def get_driver_version_to_download(self):
         """
         Downloads version from parameter if version not None or "latest".
         Downloads latest, if version is "latest" or browser could not been determined.
         Downloads determined browser version driver in all other ways as a bonus fallback for lazy users.
         """
-        if not self._driver_to_download_version:
-            self._driver_to_download_version = self._driver_version if self._driver_version not in (None, "latest") \
-                else self.get_latest_release_version()
-        return self._driver_to_download_version
+        if self._driver_version_to_download:
+            return self._driver_version_to_download
+
+        return self.get_latest_release_version()
 
     def get_latest_release_version(self):
         # type: () -> str
         raise NotImplementedError("Please implement this method")
 
     def get_browser_version_from_os(self):
         """
@@ -66,16 +62,16 @@
         if self._browser_version is None:
             self._browser_version = self._os_system_manager.get_browser_version_from_os(self.get_browser_type())
         return self._browser_version
 
     def get_browser_type(self):
         raise NotImplementedError("Please implement this method")
 
-    def get_binary_name(self):
+    def get_binary_name(self, os_type):
         driver_name = self.get_name()
         driver_binary_name = (
             "msedgedriver" if driver_name == "edgedriver" else driver_name
         )
         driver_binary_name = (
-            f"{driver_binary_name}.exe" if "win" in self.get_os_type() else driver_binary_name
+            f"{driver_binary_name}.exe" if "win" in os_type else driver_binary_name
         )
         return driver_binary_name
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/core/driver_cache.py` & `webdriver_manager-4.0.0/webdriver_manager/core/driver_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,17 @@
 
     def find_driver(self, driver: Driver):
         """Find driver by '{os_type}_{driver_name}_{driver_version}_{browser_version}'."""
         os_type = self.get_os_type()
         driver_name = driver.get_name()
         browser_type = driver.get_browser_type()
         browser_version = self._os_system_manager.get_browser_version_from_os(browser_type)
+        if not browser_version:
+            return None
+
         driver_version = self.get_cache_key_driver_version(driver)
         metadata = self.load_metadata_content()
 
         key = self.__get_metadata_key(driver)
         if key not in metadata:
             log(f'There is no [{os_type}] {driver_name} "{driver_version}" for browser {browser_type} '
                 f'"{browser_version}" in cache')
@@ -129,29 +132,30 @@
     def load_metadata_content(self):
         if os.path.exists(self._drivers_json_path):
             with open(self._drivers_json_path, "r") as outfile:
                 return json.load(outfile)
         return {}
 
     def __get_metadata_key(self, driver: Driver):
-        if self._metadata_key is None:
-            driver_version = self.get_cache_key_driver_version(driver)
-            browser_version = driver.get_browser_version_from_os()
-            browser_version = browser_version if browser_version else ""
-            self._metadata_key = f"{driver.get_os_type()}_{driver.get_name()}_{driver_version}_for_{browser_version}"
-        return self._metadata_key
+        if self._metadata_key:
+            return self._metadata_key
+
+        driver_version = self.get_cache_key_driver_version(driver)
+        browser_version = driver.get_browser_version_from_os()
+        browser_version = browser_version if browser_version else ""
+        self._metadata_key = f"{self.get_os_type()}_{driver.get_name()}_{driver_version}" \
+                             f"_for_{browser_version}"
 
     def get_cache_key_driver_version(self, driver: Driver):
-        if self._cache_key_driver_version is None:
-            self._cache_key_driver_version = "latest" if driver._driver_version in (
-            None, "latest") else driver._driver_version
-        return self._cache_key_driver_version
+        if self._cache_key_driver_version:
+            return self._cache_key_driver_version
+        return driver.get_driver_version_to_download()
 
     def __get_path(self, driver: Driver):
         if self._driver_binary_path is None:
             self._driver_binary_path = os.path.join(
                 self._drivers_directory,
                 driver.get_name(),
-                driver.get_os_type(),
+                self.get_os_type(),
                 driver.get_driver_version_to_download(),
             )
         return self._driver_binary_path
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/core/file_manager.py` & `webdriver_manager-4.0.0/webdriver_manager/core/file_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 if "/" not in n:
                     file_names.append(n)
                 else:
                     file_path, file_name = n.split("/")
                     full_file_path = os.path.join(to_directory, file_path)
                     source = os.path.join(full_file_path, file_name)
                     destination = os.path.join(to_directory, file_name)
-                    os.rename(source, destination)
+                    os.replace(source, destination)
                     file_names.append(file_name)
             return sorted(file_names, key=lambda x: x.lower())
         return archive.namelist()
 
     def __extract_tar_file(self, archive_file, to_directory):
         try:
             tar = tarfile.open(archive_file.file_path, mode="r:gz")
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/core/http.py` & `webdriver_manager-4.0.0/webdriver_manager/core/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,11 +28,11 @@
         self._ssl_verify = ssl_verify()
 
     def get(self, url, **kwargs) -> Response:
         try:
             resp = requests.get(
                 url=url, verify=self._ssl_verify, stream=True, **kwargs)
         except exceptions.ConnectionError:
-            raise ConnectionError(f"Could not reach host. Are you offline?")
+            raise exceptions.ConnectionError(f"Could not reach host. Are you offline?")
         self.validate_response(resp)
         return resp
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/core/logger.py` & `webdriver_manager-4.0.0/webdriver_manager/core/logger.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/webdriver_manager/core/os_manager.py` & `webdriver_manager-4.0.0/webdriver_manager/core/os_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,7 +156,8 @@
         try:
             cmd_mapping = cmd_mapping[browser_type][OperationSystemManager.get_os_name()]
             pattern = PATTERN[browser_type]
             version = read_version_from_cmd(cmd_mapping, pattern)
             return version
         except Exception:
             return None
+            # raise Exception("Can not get browser version from OS")
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/core/utils.py` & `webdriver_manager-4.0.0/webdriver_manager/core/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import datetime
 import os
 import re
 import subprocess
 
 
-
-
-
 def get_date_diff(date1, date2, date_format):
     a = datetime.datetime.strptime(date1, date_format)
     b = datetime.datetime.strptime(
         str(date2.strftime(date_format)), date_format)
 
     return (b - a).days
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/drivers/chrome.py` & `webdriver_manager-4.0.0/webdriver_manager/drivers/chrome.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from packaging import version
 
 from webdriver_manager.core.driver import Driver
 from webdriver_manager.core.logger import log
-from webdriver_manager.core.os_manager import OperationSystemManager, ChromeType
+from webdriver_manager.core.os_manager import ChromeType
 
 
 class ChromeDriver(Driver):
 
     def __init__(
             self,
             name,
@@ -22,32 +22,17 @@
             driver_version,
             url,
             latest_release_url,
             http_client,
             os_system_manager
         )
         self._browser_type = chrome_type
-        self._os_type = self.get_os_type()
 
-    def get_os_type(self):
-        os_type = super().get_os_type()
-        if "win" in os_type:
-            return "win32"
-
-        if not OperationSystemManager.is_mac_os(os_type):
-            return os_type
-
-        if OperationSystemManager.is_arch(os_type):
-            return "mac_arm64"
-
-        return os_type
-
-    def get_driver_download_url(self):
+    def get_driver_download_url(self, os_type):
         driver_version_to_download = self.get_driver_version_to_download()
-        os_type = self._os_type
         # For Mac ARM CPUs after version 106.0.5249.61 the format of OS type changed
         # to more unified "mac_arm64". For newer versions, it'll be "mac_arm64"
         # by default, for lower versions we replace "mac_arm64" to old format - "mac64_m1".
         if version.parse(driver_version_to_download) < version.parse("106.0.5249.61"):
             os_type = os_type.replace("mac_arm64", "mac64_m1")
 
         if version.parse(driver_version_to_download) >= version.parse("115"):
@@ -64,31 +49,43 @@
 
     def get_browser_type(self):
         return self._browser_type
 
     def get_latest_release_version(self):
         determined_browser_version = self.get_browser_version_from_os()
         log(f"Get LATEST {self._name} version for {self._browser_type}")
-        if version.parse(determined_browser_version) >= version.parse("113"):
+        if determined_browser_version is not None and version.parse(determined_browser_version) >= version.parse("113"):
             return determined_browser_version
 
         latest_release_url = (
             self._latest_release_url
-            if (self._driver_version == "latest" or determined_browser_version is None)
+            if (determined_browser_version is None)
             else f"{self._latest_release_url}_{determined_browser_version}"
         )
         resp = self._http_client.get(url=latest_release_url)
         return resp.text.rstrip()
 
     def get_url_for_version_and_platform(self, browser_version, platform):
         url = "https://googlechromelabs.github.io/chrome-for-testing/known-good-versions-with-downloads.json"
         response = self._http_client.get(url)
         data = response.json()
         versions = data["versions"]
-        for v in versions:
-            if v["version"] == browser_version:
-                downloads = v["downloads"]["chromedriver"]
+
+        if version.parse(browser_version) >= version.parse("115"):
+            short_version = ".".join(browser_version.split(".")[:3])
+            compatible_versions = [v for v in versions if short_version in v["version"]]
+            if compatible_versions:
+                latest_version = compatible_versions[-1]
+                log(f"WebDriver version {latest_version['version']} selected")
+                downloads = latest_version["downloads"]["chromedriver"]
                 for d in downloads:
                     if d["platform"] == platform:
                         return d["url"]
+        else:
+            for v in versions:
+                if v["version"] == browser_version:
+                    downloads = v["downloads"]["chromedriver"]
+                    for d in downloads:
+                        if d["platform"] == platform:
+                            return d["url"]
 
         raise Exception(f"No such driver version {browser_version} for {platform}")
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/drivers/edge.py` & `webdriver_manager-4.0.0/webdriver_manager/drivers/edge.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,38 +18,38 @@
             name,
             driver_version,
             url,
             latest_release_url,
             http_client,
             os_system_manager
         )
-        self._os_type = self.get_os_type()
 
     def get_stable_release_version(self):
         """Stable driver version when browser version was not determined."""
         stable_url = self._latest_release_url.replace("LATEST_RELEASE", "LATEST_STABLE")
         resp = self._http_client.get(url=stable_url)
         return resp.text.rstrip()
 
     def get_latest_release_version(self) -> str:
         determined_browser_version = self.get_browser_version_from_os()
         log(f"Get LATEST {self._name} version for Edge {determined_browser_version}")
 
         edge_driver_version_to_download = (
             self.get_stable_release_version()
-            if (self._driver_version == "latest" or determined_browser_version is None)
+            if (determined_browser_version is None)
             else determined_browser_version
         )
         major_edge_version = edge_driver_version_to_download.split(".")[0]
+        os_type = self._os_system_manager.get_os_type()
         latest_release_url = {
             OSType.WIN
-            in self._os_type: f"{self._latest_release_url}_{major_edge_version}_WINDOWS",
+            in os_type: f"{self._latest_release_url}_{major_edge_version}_WINDOWS",
             OSType.MAC
-            in self._os_type: f"{self._latest_release_url}_{major_edge_version}_MACOS",
+            in os_type: f"{self._latest_release_url}_{major_edge_version}_MACOS",
             OSType.LINUX
-            in self._os_type: f"{self._latest_release_url}_{major_edge_version}_LINUX",
+            in os_type: f"{self._latest_release_url}_{major_edge_version}_LINUX",
         }[True]
         resp = self._http_client.get(url=latest_release_url)
         return resp.text.rstrip()
 
     def get_browser_type(self):
         return ChromeType.MSEDGE
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/drivers/firefox.py` & `webdriver_manager-4.0.0/webdriver_manager/drivers/firefox.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,49 +18,38 @@
             driver_version,
             url,
             latest_release_url,
             http_client,
             os_system_manager,
         )
         self._mozila_release_tag = mozila_release_tag
-        self._os_type = self.get_os_type()
 
     def get_latest_release_version(self) -> str:
         determined_browser_version = self.get_browser_version_from_os()
         log(f"Get LATEST {self._name} version for {determined_browser_version} firefox")
         resp = self._http_client.get(
             url=self.latest_release_url,
             headers=self.auth_header
         )
         return resp.json()["tag_name"]
 
-    def get_driver_download_url(self):
+    def get_driver_download_url(self, os_type):
         """Like https://github.com/mozilla/geckodriver/releases/download/v0.11.1/geckodriver-v0.11.1-linux64.tar.gz"""
         driver_version_to_download = self.get_driver_version_to_download()
         log(f"Getting latest mozilla release info for {driver_version_to_download}")
         resp = self._http_client.get(
             url=self.tagged_release_url(driver_version_to_download),
             headers=self.auth_header
         )
         assets = resp.json()["assets"]
-        name = f"{self.get_name()}-{driver_version_to_download}-{self._os_type}."
+        name = f"{self.get_name()}-{driver_version_to_download}-{os_type}."
         output_dict = [
             asset for asset in assets if asset["name"].startswith(name)]
         return output_dict[0]["browser_download_url"]
 
-    def get_os_type(self):
-        os_type = super().get_os_type()
-        if not self._os_system_manager.is_mac_os(os_type):
-            return os_type
-
-        macos = 'macos'
-        if self._os_system_manager.is_arch(os_type):
-            return f"{macos}-aarch64"
-        return macos
-
     @property
     def latest_release_url(self):
         return self._latest_release_url
 
     def tagged_release_url(self, version):
         return self._mozila_release_tag.format(version)
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/drivers/ie.py` & `webdriver_manager-4.0.0/webdriver_manager/drivers/ie.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
             name,
             driver_version,
             url,
             latest_release_url,
             http_client,
             os_system_manager
         )
-        self.os_type = "x64" if self._os_system_manager.get_os_type() == "win64" else "Win32"
         self._ie_release_tag = ie_release_tag
         # todo: for 'browser_version' implement installed IE version detection
         #       like chrome or firefox
 
     def get_latest_release_version(self) -> str:
         log(f"Get LATEST driver version for Internet Explorer")
         resp = self._http_client.get(
@@ -39,26 +38,26 @@
             release
             for release in releases
             for asset in release["assets"]
             if asset["name"].startswith(self.get_name())
         )
         return release["tag_name"].replace("selenium-", "")
 
-    def get_driver_download_url(self):
+    def get_driver_download_url(self, os_type):
         """Like https://github.com/seleniumhq/selenium/releases/download/3.141.59/IEDriverServer_Win32_3.141.59.zip"""
         driver_version_to_download = self.get_driver_version_to_download()
         log(f"Getting latest ie release info for {driver_version_to_download}")
         resp = self._http_client.get(
             url=self.tagged_release_url(driver_version_to_download),
             headers=self.auth_header
         )
 
         assets = resp.json()["assets"]
 
-        name = f"{self._name}_{self.os_type}_{driver_version_to_download}" + "."
+        name = f"{self._name}_{os_type}_{driver_version_to_download}" + "."
         output_dict = [
             asset for asset in assets if asset["name"].startswith(name)]
         return output_dict[0]["browser_download_url"]
 
     @property
     def latest_release_url(self):
         return self._latest_release_url
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/drivers/opera.py` & `webdriver_manager-4.0.0/webdriver_manager/drivers/opera.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,24 +26,24 @@
     def get_latest_release_version(self) -> str:
         resp = self._http_client.get(
             url=self.latest_release_url,
             headers=self.auth_header
         )
         return resp.json()["tag_name"]
 
-    def get_driver_download_url(self) -> str:
+    def get_driver_download_url(self, os_type) -> str:
         """Like https://github.com/operasoftware/operachromiumdriver/releases/download/v.2.45/operadriver_linux64.zip"""
         driver_version_to_download = self.get_driver_version_to_download()
         log(f"Getting latest opera release info for {driver_version_to_download}")
         resp = self._http_client.get(
             url=self.tagged_release_url(driver_version_to_download),
             headers=self.auth_header
         )
         assets = resp.json()["assets"]
-        name = "{0}_{1}".format(self.get_name(), self.get_os_type())
+        name = "{0}_{1}".format(self.get_name(), os_type)
         output_dict = [
             asset for asset in assets if asset["name"].startswith(name)]
         return output_dict[0]["browser_download_url"]
 
     @property
     def latest_release_url(self):
         return self._latest_release_url
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/firefox.py` & `webdriver_manager-4.0.0/webdriver_manager/microsoft.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,74 @@
 import os
 from typing import Optional
 
 from webdriver_manager.core.download_manager import DownloadManager
 from webdriver_manager.core.driver_cache import DriverCacheManager
-from webdriver_manager.core.manager import DriverManager
 from webdriver_manager.core.os_manager import OperationSystemManager
-from webdriver_manager.drivers.firefox import GeckoDriver
+from webdriver_manager.drivers.edge import EdgeChromiumDriver
+from webdriver_manager.drivers.ie import IEDriver
+from webdriver_manager.core.manager import DriverManager
 
 
-class GeckoDriverManager(DriverManager):
+class IEDriverManager(DriverManager):
     def __init__(
             self,
             version: Optional[str] = None,
-            name: str = "geckodriver",
-            url: str = "https://github.com/mozilla/geckodriver/releases/download",
-            latest_release_url: str = "https://api.github.com/repos/mozilla/geckodriver/releases/latest",
-            mozila_release_tag: str = "https://api.github.com/repos/mozilla/geckodriver/releases/tags/{0}",
+            name: str = "IEDriverServer",
+            url: str = "https://github.com/seleniumhq/selenium/releases/download",
+            latest_release_url: str = "https://api.github.com/repos/seleniumhq/selenium/releases",
+            ie_release_tag: str = "https://api.github.com/repos/seleniumhq/selenium/releases/tags/selenium-{0}",
             download_manager: Optional[DownloadManager] = None,
             cache_manager: Optional[DriverCacheManager] = None,
             os_system_manager: Optional[OperationSystemManager] = None
     ):
-        super(GeckoDriverManager, self).__init__(
+        super().__init__(
             download_manager=download_manager,
             cache_manager=cache_manager
         )
 
-        self.driver = GeckoDriver(
+        self.driver = IEDriver(
+            driver_version=version,
+            name=name,
+            url=url,
+            latest_release_url=latest_release_url,
+            ie_release_tag=ie_release_tag,
+            http_client=self.http_client,
+            os_system_manager=os_system_manager
+        )
+
+    def install(self) -> str:
+        return self._get_driver_binary_path(self.driver)
+
+    def get_os_type(self):
+        return "x64" if self._os_system_manager.get_os_type() == "win64" else "Win32"
+
+
+class EdgeChromiumDriverManager(DriverManager):
+    def __init__(
+            self,
+            version: Optional[str] = None,
+            name: str = "edgedriver",
+            url: str = "https://msedgedriver.azureedge.net",
+            latest_release_url: str = "https://msedgedriver.azureedge.net/LATEST_RELEASE",
+            download_manager: Optional[DownloadManager] = None,
+            cache_manager: Optional[DriverCacheManager] = None,
+            os_system_manager: Optional[OperationSystemManager] = None
+    ):
+        super().__init__(
+            download_manager=download_manager,
+            cache_manager=cache_manager,
+            os_system_manager=os_system_manager
+        )
+
+        self.driver = EdgeChromiumDriver(
             driver_version=version,
             name=name,
             url=url,
             latest_release_url=latest_release_url,
-            mozila_release_tag=mozila_release_tag,
             http_client=self.http_client,
             os_system_manager=os_system_manager
         )
 
     def install(self) -> str:
         driver_path = self._get_driver_binary_path(self.driver)
         os.chmod(driver_path, 0o755)
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/microsoft.py` & `webdriver_manager-4.0.0/webdriver_manager/chrome.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,71 +1,55 @@
 import os
 from typing import Optional
 
 from webdriver_manager.core.download_manager import DownloadManager
 from webdriver_manager.core.driver_cache import DriverCacheManager
-from webdriver_manager.core.os_manager import OperationSystemManager
-from webdriver_manager.drivers.edge import EdgeChromiumDriver
-from webdriver_manager.drivers.ie import IEDriver
 from webdriver_manager.core.manager import DriverManager
+from webdriver_manager.core.os_manager import OperationSystemManager, ChromeType
+from webdriver_manager.drivers.chrome import ChromeDriver
 
 
-class IEDriverManager(DriverManager):
+class ChromeDriverManager(DriverManager):
     def __init__(
             self,
-            version: Optional[str] = None,
-            name: str = "IEDriverServer",
-            url: str = "https://github.com/seleniumhq/selenium/releases/download",
-            latest_release_url: str = "https://api.github.com/repos/seleniumhq/selenium/releases",
-            ie_release_tag: str = "https://api.github.com/repos/seleniumhq/selenium/releases/tags/selenium-{0}",
+            driver_version: Optional[str] = None,
+            name: str = "chromedriver",
+            url: str = "https://chromedriver.storage.googleapis.com",
+            latest_release_url: str = "https://chromedriver.storage.googleapis.com/LATEST_RELEASE",
+            chrome_type: str = ChromeType.GOOGLE,
             download_manager: Optional[DownloadManager] = None,
             cache_manager: Optional[DriverCacheManager] = None,
             os_system_manager: Optional[OperationSystemManager] = None
     ):
         super().__init__(
             download_manager=download_manager,
-            cache_manager=cache_manager
-        )
-
-        self.driver = IEDriver(
-            driver_version=version,
-            name=name,
-            url=url,
-            latest_release_url=latest_release_url,
-            ie_release_tag=ie_release_tag,
-            http_client=self.http_client,
+            cache_manager=cache_manager,
             os_system_manager=os_system_manager
         )
 
-    def install(self) -> str:
-        return self._get_driver_binary_path(self.driver)
-
-
-class EdgeChromiumDriverManager(DriverManager):
-    def __init__(
-            self,
-            version: Optional[str] = None,
-            name: str = "edgedriver",
-            url: str = "https://msedgedriver.azureedge.net",
-            latest_release_url: str = "https://msedgedriver.azureedge.net/LATEST_RELEASE",
-            download_manager: Optional[DownloadManager] = None,
-            cache_manager: Optional[DriverCacheManager] = None,
-            os_system_manager: Optional[OperationSystemManager] = None
-    ):
-        super().__init__(
-            download_manager=download_manager,
-            cache_manager=cache_manager
-        )
-
-        self.driver = EdgeChromiumDriver(
-            driver_version=version,
+        self.driver = ChromeDriver(
             name=name,
+            driver_version=driver_version,
             url=url,
             latest_release_url=latest_release_url,
+            chrome_type=chrome_type,
             http_client=self.http_client,
             os_system_manager=os_system_manager
         )
 
     def install(self) -> str:
         driver_path = self._get_driver_binary_path(self.driver)
         os.chmod(driver_path, 0o755)
         return driver_path
+
+    def get_os_type(self):
+        os_type = super().get_os_type()
+        if "win" in os_type:
+            return "win32"
+
+        if not self._os_system_manager.is_mac_os(os_type):
+            return os_type
+
+        if self._os_system_manager.is_arch(os_type):
+            return "mac_arm64"
+
+        return os_type
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager/opera.py` & `webdriver_manager-4.0.0/webdriver_manager/opera.py`

 * *Files identical despite different names*

### Comparing `webdriver_manager-3.9.1/webdriver_manager.egg-info/PKG-INFO` & `webdriver_manager-4.0.0/webdriver_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver-manager
-Version: 3.9.1
+Version: 4.0.0
 Summary: Library provides the way to automatically manage drivers for different browsers
 Home-page: https://github.com/SergeyPirogov/webdriver_manager
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Keywords: testing,selenium,driver,test automation
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Information Technology
```

### Comparing `webdriver_manager-3.9.1/webdriver_manager.egg-info/SOURCES.txt` & `webdriver_manager-4.0.0/webdriver_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

