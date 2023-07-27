# Comparing `tmp/mypy-boto3-chime-sdk-meetings-1.28.0.tar.gz` & `tmp/mypy-boto3-chime-sdk-meetings-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-meetings-1.28.0.tar", last modified: Thu Jul  6 20:59:05 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-meetings-1.28.12.tar", last modified: Thu Jul 27 05:34:23 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-meetings-1.28.0.tar` & `mypy-boto3-chime-sdk-meetings-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.750235 mypy-boto3-chime-sdk-meetings-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:43.000000 mypy-boto3-chime-sdk-meetings-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-06 20:59:05.746235 mypy-boto3-chime-sdk-meetings-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-07-06 20:34:43.000000 mypy-boto3-chime-sdk-meetings-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.738235 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-06 20:34:43.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-06 20:34:43.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 20:34:43.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-07-06 20:34:44.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-07-06 20:34:44.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-06 20:34:44.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-07-06 20:34:44.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:43.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-07-06 20:34:44.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-07-06 20:34:44.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:43.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.746235 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-06 20:59:05.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-06 20:59:05.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:05.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 20:59:05.000000 mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:05.750235 mypy-boto3-chime-sdk-meetings-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-06 20:34:43.000000 mypy-boto3-chime-sdk-meetings-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:23.036567 mypy-boto3-chime-sdk-meetings-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-27 05:34:23.036567 mypy-boto3-chime-sdk-meetings-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:23.036567 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-07-27 05:18:17.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:23.036567 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 05:34:22.000000 mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:23.036567 mypy-boto3-chime-sdk-meetings-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-27 05:18:16.000000 mypy-boto3-chime-sdk-meetings-1.28.12/setup.py
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/LICENSE` & `mypy-boto3-chime-sdk-meetings-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/PKG-INFO` & `mypy-boto3-chime-sdk-meetings-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-meetings
-Version: 1.28.0
-Summary: Type annotations for boto3.ChimeSDKMeetings 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ChimeSDKMeetings 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-chime-sdk-meetings"></a>
 
 # mypy-boto3-chime-sdk-meetings
 
 [![PyPI - mypy-boto3-chime-sdk-meetings](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-meetings?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-meetings)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-meetings)](https://pepy.tech/project/mypy-boto3-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMeetings 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[boto3.ChimeSDKMeetings 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-meetings docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,59 +310,63 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime_sdk_meetings.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_meetings.type_defs import (
+    AttendeeCapabilitiesOutputTypeDef,
     AttendeeCapabilitiesTypeDef,
     AttendeeIdItemTypeDef,
+    AudioFeaturesOutputTypeDef,
     AudioFeaturesTypeDef,
     CreateAttendeeErrorTypeDef,
     NotificationsConfigurationTypeDef,
     TagTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
     DeleteMeetingRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     MediaPlacementTypeDef,
     ResponseMetadataTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     UpdateAttendeeCapabilitiesRequestRequestTypeDef,
     BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
+    MeetingFeaturesConfigurationOutputTypeDef,
     MeetingFeaturesConfigurationTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TranscriptionConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     UpdateAttendeeCapabilitiesResponseTypeDef,
     BatchCreateAttendeeRequestRequestTypeDef,
+    MeetingTypeDef,
     CreateMeetingRequestRequestTypeDef,
     CreateMeetingWithAttendeesRequestRequestTypeDef,
-    MeetingTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
 )
 
 
-def get_structure() -> AttendeeCapabilitiesTypeDef:
+def get_structure() -> AttendeeCapabilitiesOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/README.md` & `mypy-boto3-chime-sdk-meetings-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-chime-sdk-meetings"></a>
 
 # mypy-boto3-chime-sdk-meetings
 
 [![PyPI - mypy-boto3-chime-sdk-meetings](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-meetings?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-meetings)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-meetings)](https://pepy.tech/project/mypy-boto3-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMeetings 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[boto3.ChimeSDKMeetings 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-meetings docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -278,59 +278,63 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime_sdk_meetings.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_meetings.type_defs import (
+    AttendeeCapabilitiesOutputTypeDef,
     AttendeeCapabilitiesTypeDef,
     AttendeeIdItemTypeDef,
+    AudioFeaturesOutputTypeDef,
     AudioFeaturesTypeDef,
     CreateAttendeeErrorTypeDef,
     NotificationsConfigurationTypeDef,
     TagTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
     DeleteMeetingRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     MediaPlacementTypeDef,
     ResponseMetadataTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     UpdateAttendeeCapabilitiesRequestRequestTypeDef,
     BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
+    MeetingFeaturesConfigurationOutputTypeDef,
     MeetingFeaturesConfigurationTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TranscriptionConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     UpdateAttendeeCapabilitiesResponseTypeDef,
     BatchCreateAttendeeRequestRequestTypeDef,
+    MeetingTypeDef,
     CreateMeetingRequestRequestTypeDef,
     CreateMeetingWithAttendeesRequestRequestTypeDef,
-    MeetingTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
 )
 
 
-def get_structure() -> AttendeeCapabilitiesTypeDef:
+def get_structure() -> AttendeeCapabilitiesOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/__main__.py` & `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMeetings 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMeetings 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/client.py` & `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/client.pyi` & `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/literals.py` & `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -288,26 +289,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/literals.pyi` & `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -286,26 +287,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/type_defs.py` & `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for chime-sdk-meetings service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime_sdk_meetings.type_defs import AttendeeCapabilitiesTypeDef
+    from mypy_boto3_chime_sdk_meetings.type_defs import AttendeeCapabilitiesOutputTypeDef
 
-    data: AttendeeCapabilitiesTypeDef = {...}
+    data: AttendeeCapabilitiesOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import (
     MediaCapabilitiesType,
@@ -33,57 +33,70 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AttendeeCapabilitiesOutputTypeDef",
     "AttendeeCapabilitiesTypeDef",
     "AttendeeIdItemTypeDef",
+    "AudioFeaturesOutputTypeDef",
     "AudioFeaturesTypeDef",
     "CreateAttendeeErrorTypeDef",
     "NotificationsConfigurationTypeDef",
     "TagTypeDef",
     "DeleteAttendeeRequestRequestTypeDef",
     "DeleteMeetingRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "GetAttendeeRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "MediaPlacementTypeDef",
     "ResponseMetadataTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeRequestItemTypeDef",
     "CreateAttendeeRequestRequestTypeDef",
     "UpdateAttendeeCapabilitiesRequestRequestTypeDef",
     "BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef",
+    "MeetingFeaturesConfigurationOutputTypeDef",
     "MeetingFeaturesConfigurationTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TranscriptionConfigurationTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
     "UpdateAttendeeCapabilitiesResponseTypeDef",
     "BatchCreateAttendeeRequestRequestTypeDef",
+    "MeetingTypeDef",
     "CreateMeetingRequestRequestTypeDef",
     "CreateMeetingWithAttendeesRequestRequestTypeDef",
-    "MeetingTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
 )
 
+AttendeeCapabilitiesOutputTypeDef = TypedDict(
+    "AttendeeCapabilitiesOutputTypeDef",
+    {
+        "Audio": MediaCapabilitiesType,
+        "Video": MediaCapabilitiesType,
+        "Content": MediaCapabilitiesType,
+    },
+)
+
 AttendeeCapabilitiesTypeDef = TypedDict(
     "AttendeeCapabilitiesTypeDef",
     {
         "Audio": MediaCapabilitiesType,
         "Video": MediaCapabilitiesType,
         "Content": MediaCapabilitiesType,
     },
@@ -92,14 +105,22 @@
 AttendeeIdItemTypeDef = TypedDict(
     "AttendeeIdItemTypeDef",
     {
         "AttendeeId": str,
     },
 )
 
+AudioFeaturesOutputTypeDef = TypedDict(
+    "AudioFeaturesOutputTypeDef",
+    {
+        "EchoReduction": MeetingFeatureStatusType,
+    },
+    total=False,
+)
+
 AudioFeaturesTypeDef = TypedDict(
     "AudioFeaturesTypeDef",
     {
         "EchoReduction": MeetingFeatureStatusType,
     },
     total=False,
 )
@@ -242,14 +263,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 MediaPlacementTypeDef = TypedDict(
     "MediaPlacementTypeDef",
     {
         "AudioHostUrl": str,
         "AudioFallbackUrl": str,
         "SignalingUrl": str,
         "TurnControlUrl": str,
@@ -289,15 +318,15 @@
 
 AttendeeTypeDef = TypedDict(
     "AttendeeTypeDef",
     {
         "ExternalUserId": str,
         "AttendeeId": str,
         "JoinToken": str,
-        "Capabilities": AttendeeCapabilitiesTypeDef,
+        "Capabilities": AttendeeCapabilitiesOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateAttendeeRequestItemTypeDef = TypedDict(
     "_RequiredCreateAttendeeRequestItemTypeDef",
     {
@@ -355,28 +384,28 @@
     {
         "MeetingId": str,
         "ExcludedAttendeeIds": Sequence[AttendeeIdItemTypeDef],
         "Capabilities": AttendeeCapabilitiesTypeDef,
     },
 )
 
-MeetingFeaturesConfigurationTypeDef = TypedDict(
-    "MeetingFeaturesConfigurationTypeDef",
+MeetingFeaturesConfigurationOutputTypeDef = TypedDict(
+    "MeetingFeaturesConfigurationOutputTypeDef",
     {
-        "Audio": AudioFeaturesTypeDef,
+        "Audio": AudioFeaturesOutputTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+MeetingFeaturesConfigurationTypeDef = TypedDict(
+    "MeetingFeaturesConfigurationTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Audio": AudioFeaturesTypeDef,
     },
+    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
@@ -388,14 +417,22 @@
     {
         "EngineTranscribeSettings": EngineTranscribeSettingsTypeDef,
         "EngineTranscribeMedicalSettings": EngineTranscribeMedicalSettingsTypeDef,
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchCreateAttendeeResponseTypeDef = TypedDict(
     "BatchCreateAttendeeResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -438,14 +475,30 @@
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
         "Attendees": Sequence[CreateAttendeeRequestItemTypeDef],
     },
 )
 
+MeetingTypeDef = TypedDict(
+    "MeetingTypeDef",
+    {
+        "MeetingId": str,
+        "MeetingHostId": str,
+        "ExternalMeetingId": str,
+        "MediaRegion": str,
+        "MediaPlacement": MediaPlacementTypeDef,
+        "MeetingFeatures": MeetingFeaturesConfigurationOutputTypeDef,
+        "PrimaryMeetingId": str,
+        "TenantIds": List[str],
+        "MeetingArn": str,
+    },
+    total=False,
+)
+
 _RequiredCreateMeetingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMeetingRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "MediaRegion": str,
         "ExternalMeetingId": str,
     },
@@ -496,30 +549,14 @@
 class CreateMeetingWithAttendeesRequestRequestTypeDef(
     _RequiredCreateMeetingWithAttendeesRequestRequestTypeDef,
     _OptionalCreateMeetingWithAttendeesRequestRequestTypeDef,
 ):
     pass
 
 
-MeetingTypeDef = TypedDict(
-    "MeetingTypeDef",
-    {
-        "MeetingId": str,
-        "MeetingHostId": str,
-        "ExternalMeetingId": str,
-        "MediaRegion": str,
-        "MediaPlacement": MediaPlacementTypeDef,
-        "MeetingFeatures": MeetingFeaturesConfigurationTypeDef,
-        "PrimaryMeetingId": str,
-        "TenantIds": List[str],
-        "MeetingArn": str,
-    },
-    total=False,
-)
-
 StartMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StartMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
         "TranscriptionConfiguration": TranscriptionConfigurationTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings/type_defs.pyi` & `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for chime-sdk-meetings service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chime_sdk_meetings.type_defs import AttendeeCapabilitiesTypeDef
+    from mypy_boto3_chime_sdk_meetings.type_defs import AttendeeCapabilitiesOutputTypeDef
 
-    data: AttendeeCapabilitiesTypeDef = {...}
+    data: AttendeeCapabilitiesOutputTypeDef = {...}
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import (
     MediaCapabilitiesType,
@@ -32,57 +32,70 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AttendeeCapabilitiesOutputTypeDef",
     "AttendeeCapabilitiesTypeDef",
     "AttendeeIdItemTypeDef",
+    "AudioFeaturesOutputTypeDef",
     "AudioFeaturesTypeDef",
     "CreateAttendeeErrorTypeDef",
     "NotificationsConfigurationTypeDef",
     "TagTypeDef",
     "DeleteAttendeeRequestRequestTypeDef",
     "DeleteMeetingRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "GetAttendeeRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "MediaPlacementTypeDef",
     "ResponseMetadataTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeRequestItemTypeDef",
     "CreateAttendeeRequestRequestTypeDef",
     "UpdateAttendeeCapabilitiesRequestRequestTypeDef",
     "BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef",
+    "MeetingFeaturesConfigurationOutputTypeDef",
     "MeetingFeaturesConfigurationTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TranscriptionConfigurationTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
     "UpdateAttendeeCapabilitiesResponseTypeDef",
     "BatchCreateAttendeeRequestRequestTypeDef",
+    "MeetingTypeDef",
     "CreateMeetingRequestRequestTypeDef",
     "CreateMeetingWithAttendeesRequestRequestTypeDef",
-    "MeetingTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
 )
 
+AttendeeCapabilitiesOutputTypeDef = TypedDict(
+    "AttendeeCapabilitiesOutputTypeDef",
+    {
+        "Audio": MediaCapabilitiesType,
+        "Video": MediaCapabilitiesType,
+        "Content": MediaCapabilitiesType,
+    },
+)
+
 AttendeeCapabilitiesTypeDef = TypedDict(
     "AttendeeCapabilitiesTypeDef",
     {
         "Audio": MediaCapabilitiesType,
         "Video": MediaCapabilitiesType,
         "Content": MediaCapabilitiesType,
     },
@@ -91,14 +104,22 @@
 AttendeeIdItemTypeDef = TypedDict(
     "AttendeeIdItemTypeDef",
     {
         "AttendeeId": str,
     },
 )
 
+AudioFeaturesOutputTypeDef = TypedDict(
+    "AudioFeaturesOutputTypeDef",
+    {
+        "EchoReduction": MeetingFeatureStatusType,
+    },
+    total=False,
+)
+
 AudioFeaturesTypeDef = TypedDict(
     "AudioFeaturesTypeDef",
     {
         "EchoReduction": MeetingFeatureStatusType,
     },
     total=False,
 )
@@ -237,14 +258,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 MediaPlacementTypeDef = TypedDict(
     "MediaPlacementTypeDef",
     {
         "AudioHostUrl": str,
         "AudioFallbackUrl": str,
         "SignalingUrl": str,
         "TurnControlUrl": str,
@@ -284,15 +313,15 @@
 
 AttendeeTypeDef = TypedDict(
     "AttendeeTypeDef",
     {
         "ExternalUserId": str,
         "AttendeeId": str,
         "JoinToken": str,
-        "Capabilities": AttendeeCapabilitiesTypeDef,
+        "Capabilities": AttendeeCapabilitiesOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateAttendeeRequestItemTypeDef = TypedDict(
     "_RequiredCreateAttendeeRequestItemTypeDef",
     {
@@ -346,28 +375,28 @@
     {
         "MeetingId": str,
         "ExcludedAttendeeIds": Sequence[AttendeeIdItemTypeDef],
         "Capabilities": AttendeeCapabilitiesTypeDef,
     },
 )
 
-MeetingFeaturesConfigurationTypeDef = TypedDict(
-    "MeetingFeaturesConfigurationTypeDef",
+MeetingFeaturesConfigurationOutputTypeDef = TypedDict(
+    "MeetingFeaturesConfigurationOutputTypeDef",
     {
-        "Audio": AudioFeaturesTypeDef,
+        "Audio": AudioFeaturesOutputTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+MeetingFeaturesConfigurationTypeDef = TypedDict(
+    "MeetingFeaturesConfigurationTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Audio": AudioFeaturesTypeDef,
     },
+    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
@@ -379,14 +408,22 @@
     {
         "EngineTranscribeSettings": EngineTranscribeSettingsTypeDef,
         "EngineTranscribeMedicalSettings": EngineTranscribeMedicalSettingsTypeDef,
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchCreateAttendeeResponseTypeDef = TypedDict(
     "BatchCreateAttendeeResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -429,14 +466,30 @@
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
         "Attendees": Sequence[CreateAttendeeRequestItemTypeDef],
     },
 )
 
+MeetingTypeDef = TypedDict(
+    "MeetingTypeDef",
+    {
+        "MeetingId": str,
+        "MeetingHostId": str,
+        "ExternalMeetingId": str,
+        "MediaRegion": str,
+        "MediaPlacement": MediaPlacementTypeDef,
+        "MeetingFeatures": MeetingFeaturesConfigurationOutputTypeDef,
+        "PrimaryMeetingId": str,
+        "TenantIds": List[str],
+        "MeetingArn": str,
+    },
+    total=False,
+)
+
 _RequiredCreateMeetingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMeetingRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "MediaRegion": str,
         "ExternalMeetingId": str,
     },
@@ -483,30 +536,14 @@
 
 class CreateMeetingWithAttendeesRequestRequestTypeDef(
     _RequiredCreateMeetingWithAttendeesRequestRequestTypeDef,
     _OptionalCreateMeetingWithAttendeesRequestRequestTypeDef,
 ):
     pass
 
-MeetingTypeDef = TypedDict(
-    "MeetingTypeDef",
-    {
-        "MeetingId": str,
-        "MeetingHostId": str,
-        "ExternalMeetingId": str,
-        "MediaRegion": str,
-        "MediaPlacement": MediaPlacementTypeDef,
-        "MeetingFeatures": MeetingFeaturesConfigurationTypeDef,
-        "PrimaryMeetingId": str,
-        "TenantIds": List[str],
-        "MeetingArn": str,
-    },
-    total=False,
-)
-
 StartMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StartMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
         "TranscriptionConfiguration": TranscriptionConfigurationTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-meetings
-Version: 1.28.0
-Summary: Type annotations for boto3.ChimeSDKMeetings 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ChimeSDKMeetings 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-chime-sdk-meetings"></a>
 
 # mypy-boto3-chime-sdk-meetings
 
 [![PyPI - mypy-boto3-chime-sdk-meetings](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-meetings?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-meetings)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chime-sdk-meetings)](https://pepy.tech/project/mypy-boto3-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMeetings 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
+[boto3.ChimeSDKMeetings 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-meetings docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_meetings/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,59 +310,63 @@
 ### Typed dictionaries
 
 `mypy_boto3_chime_sdk_meetings.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_chime_sdk_meetings.type_defs import (
+    AttendeeCapabilitiesOutputTypeDef,
     AttendeeCapabilitiesTypeDef,
     AttendeeIdItemTypeDef,
+    AudioFeaturesOutputTypeDef,
     AudioFeaturesTypeDef,
     CreateAttendeeErrorTypeDef,
     NotificationsConfigurationTypeDef,
     TagTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
     DeleteMeetingRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     MediaPlacementTypeDef,
     ResponseMetadataTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     UpdateAttendeeCapabilitiesRequestRequestTypeDef,
     BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
+    MeetingFeaturesConfigurationOutputTypeDef,
     MeetingFeaturesConfigurationTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TranscriptionConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     UpdateAttendeeCapabilitiesResponseTypeDef,
     BatchCreateAttendeeRequestRequestTypeDef,
+    MeetingTypeDef,
     CreateMeetingRequestRequestTypeDef,
     CreateMeetingWithAttendeesRequestRequestTypeDef,
-    MeetingTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
 )
 
 
-def get_structure() -> AttendeeCapabilitiesTypeDef:
+def get_structure() -> AttendeeCapabilitiesOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-meetings-1.28.12/mypy_boto3_chime_sdk_meetings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-meetings-1.28.0/setup.py` & `mypy-boto3-chime-sdk-meetings-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-meetings",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_chime_sdk_meetings"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMeetings 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ChimeSDKMeetings 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

