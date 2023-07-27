# Comparing `tmp/tube_toolkit-0.0.8.tar.gz` & `tmp/tube_toolkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tube_toolkit-0.0.8.tar", last modified: Thu Jul  7 19:48:37 2022, max compression
+gzip compressed data, was "tube_toolkit-0.0.9.tar", last modified: Tue Jul 19 21:35:43 2022, max compression
```

## Comparing `tube_toolkit-0.0.8.tar` & `tube_toolkit-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ganhejuntomobile   (503) staff       (20)        0 2022-07-07 19:48:37.318783 tube_toolkit-0.0.8/
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)      414 2022-07-07 19:48:37.318984 tube_toolkit-0.0.8/PKG-INFO
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)      115 2022-07-05 17:57:58.000000 tube_toolkit-0.0.8/README.rst
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)       80 2022-07-05 14:55:53.000000 tube_toolkit-0.0.8/pyproject.toml
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)     1006 2022-07-07 19:48:37.319851 tube_toolkit-0.0.8/setup.cfg
-drwxr-xr-x   0 ganhejuntomobile   (503) staff       (20)        0 2022-07-07 19:48:37.290403 tube_toolkit-0.0.8/tube_toolkit/
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)       21 2022-07-07 19:48:25.000000 tube_toolkit-0.0.8/tube_toolkit/__init__.py
-drwxr-xr-x   0 ganhejuntomobile   (503) staff       (20)        0 2022-07-07 19:48:37.309705 tube_toolkit-0.0.8/tube_toolkit/core/
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)        0 2022-07-04 12:50:42.000000 tube_toolkit-0.0.8/tube_toolkit/core/__init__.py
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)     8560 2022-07-07 12:11:51.000000 tube_toolkit-0.0.8/tube_toolkit/core/actions.py
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)      262 2022-07-04 18:43:08.000000 tube_toolkit-0.0.8/tube_toolkit/core/logger.py
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)     1950 2022-07-06 14:05:06.000000 tube_toolkit-0.0.8/tube_toolkit/instance.py
-drwxr-xr-x   0 ganhejuntomobile   (503) staff       (20)        0 2022-07-07 19:48:37.305088 tube_toolkit-0.0.8/tube_toolkit.egg-info/
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)      414 2022-07-07 19:48:37.000000 tube_toolkit-0.0.8/tube_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)      386 2022-07-07 19:48:37.000000 tube_toolkit-0.0.8/tube_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)        1 2022-07-07 19:48:37.000000 tube_toolkit-0.0.8/tube_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)        1 2022-07-07 19:48:36.000000 tube_toolkit-0.0.8/tube_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)      417 2022-07-07 19:48:37.000000 tube_toolkit-0.0.8/tube_toolkit.egg-info/requires.txt
--rw-r--r--   0 ganhejuntomobile   (503) staff       (20)       13 2022-07-07 19:48:37.000000 tube_toolkit-0.0.8/tube_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 ganhejuntomobile   (503) staff       (20)        0 2022-07-19 21:35:43.966935 tube_toolkit-0.0.9/
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)      414 2022-07-19 21:35:43.968140 tube_toolkit-0.0.9/PKG-INFO
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)      115 2022-07-05 17:57:58.000000 tube_toolkit-0.0.9/README.rst
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)       80 2022-07-05 14:55:53.000000 tube_toolkit-0.0.9/pyproject.toml
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)     1006 2022-07-19 21:35:43.969979 tube_toolkit-0.0.9/setup.cfg
+drwxr-xr-x   0 ganhejuntomobile   (503) staff       (20)        0 2022-07-19 21:35:43.954125 tube_toolkit-0.0.9/tube_toolkit/
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)       21 2022-07-19 21:33:54.000000 tube_toolkit-0.0.9/tube_toolkit/__init__.py
+drwxr-xr-x   0 ganhejuntomobile   (503) staff       (20)        0 2022-07-19 21:35:43.966448 tube_toolkit-0.0.9/tube_toolkit/core/
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)        0 2022-07-04 12:50:42.000000 tube_toolkit-0.0.9/tube_toolkit/core/__init__.py
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)     7711 2022-07-19 21:33:33.000000 tube_toolkit-0.0.9/tube_toolkit/core/actions.py
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)      262 2022-07-04 18:43:08.000000 tube_toolkit-0.0.9/tube_toolkit/core/logger.py
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)     1950 2022-07-08 12:18:07.000000 tube_toolkit-0.0.9/tube_toolkit/main.py
+drwxr-xr-x   0 ganhejuntomobile   (503) staff       (20)        0 2022-07-19 21:35:43.961203 tube_toolkit-0.0.9/tube_toolkit.egg-info/
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)      414 2022-07-19 21:35:43.000000 tube_toolkit-0.0.9/tube_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)      382 2022-07-19 21:35:43.000000 tube_toolkit-0.0.9/tube_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)        1 2022-07-19 21:35:43.000000 tube_toolkit-0.0.9/tube_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)        1 2022-07-19 21:35:43.000000 tube_toolkit-0.0.9/tube_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)      417 2022-07-19 21:35:43.000000 tube_toolkit-0.0.9/tube_toolkit.egg-info/requires.txt
+-rw-r--r--   0 ganhejuntomobile   (503) staff       (20)       13 2022-07-19 21:35:43.000000 tube_toolkit-0.0.9/tube_toolkit.egg-info/top_level.txt
```

### Comparing `tube_toolkit-0.0.8/setup.cfg` & `tube_toolkit-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `tube_toolkit-0.0.8/tube_toolkit/core/actions.py` & `tube_toolkit-0.0.9/tube_toolkit/core/actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,42 +73,36 @@
 
         headers['Content-Type'] = 'application/json'
         headers['Accept'] = 'application/json'
 
         response = requests.get(url, headers=headers, verify=verifySSL)
         return response
 
-    def clear_input(self, by_type: By, by_value: str, timeout: Optional[int] = None, retry: Optional[int] = None) -> None:
+    def clear_input(self, by_type: By, by_value: str, timeout: Optional[int] = None) -> Union[str, bool]:
     
         """
         This method executes a clear if the element is found within a time range.
 
         Arguments:
             by_type: one of the By class constants, you can find them in selenium.webdriver.common.by module.
 
             by_value: the value of the element to be clicked, for example:
                 '//*[@id="element"]' for an element with id='element'
                 '//*[@class="element"]' for an element with class='element'
 
             timeout (Optional): Generates a error if can't locate the element in x seconds. (Standard timeout: 10 seconds).
-            retry (Optional): After logging the error, attempts X times again to locate the element, every try can generate a new error.
         """
         
-        while True:
-            try:
-                Wait(self.driver, timeout or self.timeout).until(EC.presence_of_element_located((by_type, by_value))).clear()
-                break
-            except Exception as e:
-                print(e)
-                if retry != None and retry > 0:
-                    retry -= 1
-                else:
-                    break
+        try:
+            Wait(self.driver, timeout or self.timeout).until(EC.presence_of_element_located((by_type, by_value))).clear()
+            return True
+        except Exception as e:
+            return f"Exception on element {by_value}, {e}"
 
-    def send_keys(self, by_type: By, by_value: str, keys_array: list[Union[str, Keys]], timeout: Optional[int] = None, retry: Optional[int] = None) -> None:
+    def send_keys(self, by_type: By, by_value: str, keys_array: list[Union[str, Keys]], timeout: Optional[int] = None) -> Union[str, bool]:
 
         """
         This method press the keys in the sent array if the element is found within a time range.
 
         Arguments:
             by_type: one of the By class constants, you can find them in selenium.webdriver.common.by module.
 
@@ -117,54 +111,42 @@
                 '//*[@class="element"]' for an element with class='element'
 
             keys_array: the array of keys to be sent to the element, the keys will send in order. For example:
                 ['a', 'b', 'c'] for the keys 'a', 'b' and 'c'.
                 you can use selenium.webdriver.common.keys module to get the keys too.
 
             timeout (Optional): Generates a error if can't locate the element in x seconds. (Standard timeout: 10 seconds).
-            retry (Optional): After logging the error, attempts X times again to locate the element, every try can generate a new error.
         """
 
-        while True:
-            try:
-                Wait(self.driver, timeout or self.timeout).until(EC.visibility_of_element_located((by_type, by_value))).send_keys(keys_array)
-                break
-            except Exception as e:
-                print(e)
-                if retry != None and retry > 0:
-                    retry -= 1
-                else:
-                    break
+        try:
+            Wait(self.driver, timeout or self.timeout).until(EC.visibility_of_element_located((by_type, by_value))).send_keys(keys_array)
+            return True
+        except Exception as e:
+            return f"Exception on element {by_value}, {e}"
 
-    def switch_to_frame(self, by_type: By, by_value: str, timeout: Optional[int] = None, retry: Optional[int] = None) -> None:
+    def switch_to_frame(self, by_type: By, by_value: str, timeout: Optional[int] = None) -> Union[str, bool]:
 
         """
         This method switches to the frame if the element is found within a time range.
 
         Arguments:
             by_type: one of the By class constants, you can find them in selenium.webdriver.common.by module.
 
             by_value: the value of the element to be clicked, for example:
                 '//*[@id="element"]' for an element with id='element'
                 '//*[@class="element"]' for an element with class='element'
 
             timeout (Optional): Generates a error if can't locate the element in x seconds. (Standard timeout: 10 seconds).
-            retry (Optional): After logging the error, attempts X times again to locate the element, every try can generate a new error.
         """
 
-        while True:
-            try:
-                Wait(self.driver, timeout or self.timeout).until(EC.frame_to_be_available_and_switch_to_it((by_type, by_value)))
-                break
-            except Exception as e:
-                print(e)
-                if retry != None and retry > 0:
-                    retry -= 1
-                else:
-                    break
+        try:
+            Wait(self.driver, timeout or self.timeout).until(EC.frame_to_be_available_and_switch_to_it((by_type, by_value)))
+            return True
+        except Exception as e:
+            return f"Exception on element {by_value}, {e}"
     
     def find_and_get_attribute(self, by_type: By, by_value: str, attribute: str, timeout: Optional[int] = None) -> Union[str, bool]:
 
         """
         This method finds the element if the element is found within a time range and returns the attribute value.
 
         Arguments:
```

### Comparing `tube_toolkit-0.0.8/tube_toolkit/instance.py` & `tube_toolkit-0.0.9/tube_toolkit/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-  Copyright (C) 2018 TUBE
+  Copyright (C) 2022 TUBE
   This program is private software: you can't redistribute it and/or modify
   it without the agreement of the author.
   This program is distributed in the hope that it will be useful,
   but WITHOUT ANY WARRANTY; without even the implied warranty of
   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 '''
```

