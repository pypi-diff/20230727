# Comparing `tmp/reolink_aio-0.7.4.tar.gz` & `tmp/reolink_aio-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reolink_aio-0.7.4.tar", last modified: Thu Jul 27 20:03:29 2023, max compression
+gzip compressed data, was "reolink_aio-0.7.5.tar", last modified: Thu Jul 27 20:43:57 2023, max compression
```

## Comparing `reolink_aio-0.7.4.tar` & `reolink_aio-0.7.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:03:29.029451 reolink_aio-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-27 20:03:29.029451 reolink_aio-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:03:29.025451 reolink_aio-0.7.4/reolink_aio/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   194003 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/software_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    15330 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/typings.py
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/reolink_aio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:03:29.029451 reolink_aio-0.7.4/reolink_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-27 20:03:29.000000 reolink_aio-0.7.4/reolink_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-07-27 20:03:29.000000 reolink_aio-0.7.4/reolink_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 20:03:29.000000 reolink_aio-0.7.4/reolink_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 20:03:28.000000 reolink_aio-0.7.4/reolink_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-27 20:03:29.000000 reolink_aio-0.7.4/reolink_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-27 20:03:29.000000 reolink_aio-0.7.4/reolink_aio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 20:03:29.029451 reolink_aio-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:03:29.029451 reolink_aio-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-07-27 20:03:18.000000 reolink_aio-0.7.4/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:43:57.823860 reolink_aio-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-27 20:43:57.823860 reolink_aio-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3912 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:43:57.823860 reolink_aio-0.7.5/reolink_aio/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   194199 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/software_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15330 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/typings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/reolink_aio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:43:57.823860 reolink_aio-0.7.5/reolink_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4720 2023-07-27 20:43:57.000000 reolink_aio-0.7.5/reolink_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-07-27 20:43:57.000000 reolink_aio-0.7.5/reolink_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 20:43:57.000000 reolink_aio-0.7.5/reolink_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 20:43:57.000000 reolink_aio-0.7.5/reolink_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-27 20:43:57.000000 reolink_aio-0.7.5/reolink_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-27 20:43:57.000000 reolink_aio-0.7.5/reolink_aio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 20:43:57.823860 reolink_aio-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 20:43:57.823860 reolink_aio-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    15443 2023-07-27 20:43:44.000000 reolink_aio-0.7.5/tests/test.py
```

### Comparing `reolink_aio-0.7.4/LICENSE` & `reolink_aio-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.4/PKG-INFO` & `reolink_aio-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink_aio
-Version: 0.7.4
+Version: 0.7.5
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.4 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink_aio Version: 0.7.5 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.7.4/README.md` & `reolink_aio-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.4/reolink_aio/api.py` & `reolink_aio-0.7.5/reolink_aio/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -920,15 +920,15 @@
 
             if channel in self._recording_settings and (self.api_version("GetRec") < 1 or "scheduleEnable" in self._recording_settings[channel]["Rec"]):
                 self._capabilities[channel].append("recording")
 
             if channel in self._email_settings and (self.api_version("GetEmail") < 1 or "scheduleEnable" in self._email_settings[channel]["Email"]):
                 self._capabilities[channel].append("email")
 
-            if self.api_version("supportBuzzer") > 0 and "scheduleEnable" in self._buzzer_settings[channel]["Buzzer"]:
+            if channel in self._buzzer_settings and self.api_version("supportBuzzer") > 0 and "scheduleEnable" in self._buzzer_settings[channel]["Buzzer"]:
                 self._capabilities[channel].append("buzzer")
 
             if self.api_version("ledControl", channel) > 0 and channel in self._ir_settings:
                 self._capabilities[channel].append("ir_lights")
 
             if self.api_version("powerLed", channel) > 0:
                 # powerLed == statusLed = doorbell_led
@@ -1364,14 +1364,16 @@
             if self.supported(channel, "pan_tilt") and self.api_version("ptzPreset", channel) >= 1:
                 ch_body.append({"cmd": "GetPtzPreset", "action": 0, "param": {"channel": channel}})
                 ch_body.append({"cmd": "GetPtzGuard", "action": 0, "param": {"channel": channel}})
                 ch_body.append({"cmd": "GetPtzCurPos", "action": 0, "param": {"PtzCurPos": {"channel": channel}}})
             if self.supported(channel, "auto_track"):
                 ch_body.append({"cmd": "GetAiCfg", "action": 1, "param": {"channel": channel}})
             # checking API versions
+            if self.api_version("supportBuzzer") > 0:
+                ch_body.append({"cmd": "GetBuzzerAlarmV20", "action": 0, "param": {"channel": channel}})
             if self.api_version("scheduleVersion") >= 1:
                 ch_body.extend(
                     [
                         {"cmd": "GetEmailV20", "action": 0, "param": {"channel": channel}},
                         {"cmd": "GetPushV20", "action": 0, "param": {"channel": channel}},
                         {"cmd": "GetFtpV20", "action": 0, "param": {"channel": channel}},
                         {"cmd": "GetRecV20", "action": 0, "param": {"channel": channel}},
```

### Comparing `reolink_aio-0.7.4/reolink_aio/enums.py` & `reolink_aio-0.7.5/reolink_aio/enums.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.4/reolink_aio/exceptions.py` & `reolink_aio-0.7.5/reolink_aio/exceptions.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.4/reolink_aio/software_version.py` & `reolink_aio-0.7.5/reolink_aio/software_version.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.4/reolink_aio/templates.py` & `reolink_aio-0.7.5/reolink_aio/templates.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.4/reolink_aio/typings.py` & `reolink_aio-0.7.5/reolink_aio/typings.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.4/reolink_aio/utils.py` & `reolink_aio-0.7.5/reolink_aio/utils.py`

 * *Files identical despite different names*

### Comparing `reolink_aio-0.7.4/reolink_aio.egg-info/PKG-INFO` & `reolink_aio-0.7.5/reolink_aio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reolink-aio
-Version: 0.7.4
+Version: 0.7.5
 Summary: Reolink NVR/cameras API package
 Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.4 Summary: Reolink NVR/
+Metadata-Version: 2.1 Name: reolink-aio Version: 0.7.5 Summary: Reolink NVR/
 cameras API package Home-page: https://github.com/starkillerOG/reolink_aio
 Author: starkillerOG Author-email: starkiller.og@gmail.com License: MIT
 Platform: any Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier: Topic
 :: Software Development :: Libraries Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `reolink_aio-0.7.4/setup.py` & `reolink_aio-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='reolink_aio',
-      version='0.7.4',
+      version='0.7.5',
       description='Reolink NVR/cameras API package',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/starkillerOG/reolink_aio',
       author='starkillerOG',
       author_email='starkiller.og@gmail.com',
       license='MIT',
```

### Comparing `reolink_aio-0.7.4/tests/test.py` & `reolink_aio-0.7.5/tests/test.py`

 * *Files identical despite different names*

