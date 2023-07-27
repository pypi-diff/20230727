# Comparing `tmp/mecord-cli-0.1.90.tar.gz` & `tmp/mecord-cli-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecord-cli-0.1.90.tar", last modified: Tue Jul 25 02:52:16 2023, max compression
+gzip compressed data, was "mecord-cli-0.1.91.tar", last modified: Thu Jul 27 06:34:36 2023, max compression
```

## Comparing `mecord-cli-0.1.90.tar` & `mecord-cli-0.1.91.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 02:52:16.346119 mecord-cli-0.1.90/
--rw-rw-rw-   0        0        0     1078 2023-02-16 06:18:02.000000 mecord-cli-0.1.90/LICENSE
--rw-rw-rw-   0        0        0     2364 2023-07-25 02:52:16.345119 mecord-cli-0.1.90/PKG-INFO
--rw-rw-rw-   0        0        0     1942 2023-04-21 14:39:36.000000 mecord-cli-0.1.90/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 02:52:16.324411 mecord-cli-0.1.90/mecord/
--rw-rw-rw-   0        0        0        0 2023-02-27 08:17:36.000000 mecord-cli-0.1.90/mecord/__init__.py
--rw-rw-rw-   0        0        0    56500 2023-06-09 09:58:53.000000 mecord-cli-0.1.90/mecord/aigc_ext_pb2.py
--rw-rw-rw-   0        0        0    10618 2023-07-21 03:43:25.000000 mecord-cli-0.1.90/mecord/capability_provider.py
--rw-rw-rw-   0        0        0    40930 2023-06-09 09:58:18.000000 mecord-cli-0.1.90/mecord/common_ext_pb2.py
--rw-rw-rw-   0        0        0      173 2023-07-25 02:52:15.000000 mecord-cli-0.1.90/mecord/constant.py
--rw-rw-rw-   0        0        0     1934 2023-07-17 07:17:48.000000 mecord-cli-0.1.90/mecord/main.py
--rw-rw-rw-   0        0        0    10590 2023-07-24 02:55:22.000000 mecord-cli-0.1.90/mecord/mecord_service.py
--rw-rw-rw-   0        0        0    11578 2023-07-19 09:58:48.000000 mecord-cli-0.1.90/mecord/mecord_widget.py
--rw-rw-rw-   0        0        0    10668 2023-07-24 04:00:36.000000 mecord-cli-0.1.90/mecord/progress_monitor.py
-drwxrwxrwx   0        0        0        0 2023-07-25 02:52:16.326428 mecord-cli-0.1.90/mecord/public_tools/
--rw-rw-rw-   0        0        0        0 2023-04-21 14:39:36.000000 mecord-cli-0.1.90/mecord/public_tools/__init__.py
--rw-rw-rw-   0        0        0      302 2023-04-21 14:39:36.000000 mecord-cli-0.1.90/mecord/public_tools/decorator_tools.py
--rw-rw-rw-   0        0        0     3250 2023-06-09 09:58:18.000000 mecord-cli-0.1.90/mecord/rpcinput_pb2.py
-drwxrwxrwx   0        0        0        0 2023-07-25 02:52:16.332377 mecord-cli-0.1.90/mecord/script_template/
--rw-rw-rw-   0        0        0        0 2023-03-01 01:46:57.000000 mecord-cli-0.1.90/mecord/script_template/__init__.py
--rw-rw-rw-   0        0        0      312 2023-04-21 14:39:36.000000 mecord-cli-0.1.90/mecord/script_template/launch.py
--rw-rw-rw-   0        0        0      915 2023-04-10 11:57:12.000000 mecord-cli-0.1.90/mecord/script_template/main.py
--rw-rw-rw-   0        0        0      801 2023-03-15 02:24:04.000000 mecord-cli-0.1.90/mecord/script_template/run.py
--rw-rw-rw-   0        0        0     6214 2023-07-20 09:18:18.000000 mecord-cli-0.1.90/mecord/store.py
--rw-rw-rw-   0        0        0     8745 2023-06-09 09:58:18.000000 mecord-cli-0.1.90/mecord/uauth_common_pb2.py
--rw-rw-rw-   0        0        0   108609 2023-06-09 09:58:56.000000 mecord-cli-0.1.90/mecord/uauth_ext_pb2.py
--rw-rw-rw-   0        0        0     2450 2023-07-25 02:51:50.000000 mecord-cli-0.1.90/mecord/upload.py
--rw-rw-rw-   0        0        0    12849 2023-06-09 09:58:55.000000 mecord-cli-0.1.90/mecord/user_status_ext_pb2.py
--rw-rw-rw-   0        0        0    12538 2023-07-17 06:01:30.000000 mecord-cli-0.1.90/mecord/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 02:52:16.338014 mecord-cli-0.1.90/mecord/widget_template/
--rw-rw-rw-   0        0        0     1977 2023-03-14 11:34:25.000000 mecord-cli-0.1.90/mecord/widget_template/MekongJS.js.py
--rw-rw-rw-   0        0        0        0 2023-03-01 01:46:57.000000 mecord-cli-0.1.90/mecord/widget_template/__init__.py
--rw-rw-rw-   0        0        0      219 2023-04-21 14:39:36.000000 mecord-cli-0.1.90/mecord/widget_template/config.json.py
--rw-rw-rw-   0        0        0     1678 2023-03-14 11:34:25.000000 mecord-cli-0.1.90/mecord/widget_template/icon.png.py
--rw-rw-rw-   0        0        0      719 2023-03-14 11:34:25.000000 mecord-cli-0.1.90/mecord/widget_template/index.html.py
--rw-rw-rw-   0        0        0     9981 2023-07-25 02:46:29.000000 mecord-cli-0.1.90/mecord/xy_pb.py
--rw-rw-rw-   0        0        0     2216 2023-04-10 11:57:12.000000 mecord-cli-0.1.90/mecord/xy_user.py
-drwxrwxrwx   0        0        0        0 2023-07-25 02:52:16.344123 mecord-cli-0.1.90/mecord_cli.egg-info/
--rw-rw-rw-   0        0        0     2364 2023-07-25 02:52:16.000000 mecord-cli-0.1.90/mecord_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1009 2023-07-25 02:52:16.000000 mecord-cli-0.1.90/mecord_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 02:52:16.000000 mecord-cli-0.1.90/mecord_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-25 02:52:16.000000 mecord-cli-0.1.90/mecord_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       78 2023-07-25 02:52:16.000000 mecord-cli-0.1.90/mecord_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-25 02:52:16.000000 mecord-cli-0.1.90/mecord_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 02:52:16.346119 mecord-cli-0.1.90/setup.cfg
--rw-rw-rw-   0        0        0     2523 2023-07-25 02:48:17.000000 mecord-cli-0.1.90/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:36.231057 mecord-cli-0.1.91/
+-rw-rw-rw-   0        0        0     1078 2023-04-19 06:54:05.000000 mecord-cli-0.1.91/LICENSE
+-rw-rw-rw-   0        0        0     2364 2023-07-27 06:34:36.230561 mecord-cli-0.1.91/PKG-INFO
+-rw-rw-rw-   0        0        0     1942 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:36.149749 mecord-cli-0.1.91/mecord/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/__init__.py
+-rw-rw-rw-   0        0        0    57424 2023-07-03 02:47:14.000000 mecord-cli-0.1.91/mecord/aigc_ext_pb2.py
+-rw-rw-rw-   0        0        0    10618 2023-07-27 06:26:10.000000 mecord-cli-0.1.91/mecord/capability_provider.py
+-rw-rw-rw-   0        0        0    41642 2023-07-03 02:47:14.000000 mecord-cli-0.1.91/mecord/common_ext_pb2.py
+-rw-rw-rw-   0        0        0      176 2023-07-27 06:34:35.000000 mecord-cli-0.1.91/mecord/constant.py
+-rw-rw-rw-   0        0        0     1934 2023-07-03 02:47:14.000000 mecord-cli-0.1.91/mecord/main.py
+-rw-rw-rw-   0        0        0    10604 2023-07-27 06:29:12.000000 mecord-cli-0.1.91/mecord/mecord_service.py
+-rw-rw-rw-   0        0        0    11578 2023-07-27 06:26:10.000000 mecord-cli-0.1.91/mecord/mecord_widget.py
+-rw-rw-rw-   0        0        0    11202 2023-07-27 06:26:17.000000 mecord-cli-0.1.91/mecord/progress_monitor.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:36.156666 mecord-cli-0.1.91/mecord/public_tools/
+-rw-rw-rw-   0        0        0        0 2023-04-21 11:01:50.000000 mecord-cli-0.1.91/mecord/public_tools/__init__.py
+-rw-rw-rw-   0        0        0      302 2023-04-20 10:06:00.000000 mecord-cli-0.1.91/mecord/public_tools/decorator_tools.py
+-rw-rw-rw-   0        0        0     3321 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/rpcinput_pb2.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:36.175043 mecord-cli-0.1.91/mecord/script_template/
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/script_template/__init__.py
+-rw-rw-rw-   0        0        0      312 2023-04-21 11:40:09.000000 mecord-cli-0.1.91/mecord/script_template/launch.py
+-rw-rw-rw-   0        0        0      915 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/script_template/main.py
+-rw-rw-rw-   0        0        0      801 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/script_template/run.py
+-rw-rw-rw-   0        0        0     6214 2023-07-27 06:26:10.000000 mecord-cli-0.1.91/mecord/store.py
+-rw-rw-rw-   0        0        0     8912 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/uauth_common_pb2.py
+-rw-rw-rw-   0        0        0   110273 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/uauth_ext_pb2.py
+-rw-rw-rw-   0        0        0     2450 2023-07-27 06:26:10.000000 mecord-cli-0.1.91/mecord/upload.py
+-rw-rw-rw-   0        0        0    13069 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/user_status_ext_pb2.py
+-rw-rw-rw-   0        0        0    12538 2023-07-27 06:26:10.000000 mecord-cli-0.1.91/mecord/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:36.207189 mecord-cli-0.1.91/mecord/widget_template/
+-rw-rw-rw-   0        0        0     1977 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/widget_template/MekongJS.js.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/widget_template/__init__.py
+-rw-rw-rw-   0        0        0      219 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/widget_template/config.json.py
+-rw-rw-rw-   0        0        0     1678 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/widget_template/icon.png.py
+-rw-rw-rw-   0        0        0      719 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/widget_template/index.html.py
+-rw-rw-rw-   0        0        0     9981 2023-07-27 06:26:10.000000 mecord-cli-0.1.91/mecord/xy_pb.py
+-rw-rw-rw-   0        0        0     2216 2023-04-19 07:17:07.000000 mecord-cli-0.1.91/mecord/xy_user.py
+drwxrwxrwx   0        0        0        0 2023-07-27 06:34:36.230063 mecord-cli-0.1.91/mecord_cli.egg-info/
+-rw-rw-rw-   0        0        0     2364 2023-07-27 06:34:35.000000 mecord-cli-0.1.91/mecord_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1009 2023-07-27 06:34:35.000000 mecord-cli-0.1.91/mecord_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 06:34:35.000000 mecord-cli-0.1.91/mecord_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-27 06:34:35.000000 mecord-cli-0.1.91/mecord_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2023-07-27 06:34:35.000000 mecord-cli-0.1.91/mecord_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-27 06:34:35.000000 mecord-cli-0.1.91/mecord_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 06:34:36.231552 mecord-cli-0.1.91/setup.cfg
+-rw-rw-rw-   0        0        0     2525 2023-07-27 06:30:13.000000 mecord-cli-0.1.91/setup.py
```

### Comparing `mecord-cli-0.1.90/LICENSE` & `mecord-cli-0.1.91/LICENSE`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/PKG-INFO` & `mecord-cli-0.1.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecord-cli
-Version: 0.1.90
+Version: 0.1.91
 Summary: mecord tools
 Home-page: https://github.com/mecordofficial
 Author: pengjun
 Author-email: mr_lonely@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mecord-cli-0.1.90/README.md` & `mecord-cli-0.1.91/README.md`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/aigc_ext_pb2.py` & `mecord-cli-0.1.91/mecord/aigc_ext_pb2.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,924 +1,924 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: aigc_ext.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from mecord import common_ext_pb2 as common__ext__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x61igc_ext.proto\x12\x02pb\x1a\x10\x63ommon_ext.proto\"J\n\x08TaskItem\x12\x0e\n\x06taskId\x18\x01 \x01(\x03\x12\x10\n\x08taskUUID\x18\x02 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\t\"o\n\nGetTaskReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x11\n\tDeviceKey\x18\x02 \x01(\t\x12\x0f\n\x07widgets\x18\x03 \x03(\t\x12\r\n\x05token\x18\x04 \x01(\t\x12\r\n\x05limit\x18\x05 \x01(\x05\x12\x0e\n\x06\x65xtend\x18\x06 \x01(\t\"F\n\nGetTaskRes\x12\x1a\n\x04list\x18\x01 \x03(\x0b\x32\x0c.pb.TaskItem\x12\r\n\x05limit\x18\x02 \x01(\x05\x12\r\n\x05\x63ount\x18\x03 \x01(\x03\"x\n\rTaskNotifyReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08taskUUID\x18\x02 \x01(\t\x12\"\n\ntaskStatus\x18\x03 \x01(\x0e\x32\x0e.pb.TaskStatus\x12\x12\n\nfailReason\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\t\"\x0f\n\rTaskNotifyRes\"o\n\x11\x41igcDeviceBindReq\x12\x11\n\tdeviceKey\x18\x01 \x01(\t\x12\x11\n\tGroupUUID\x18\x02 \x01(\t\x12 \n\tLabelType\x18\x03 \x01(\x0e\x32\r.pb.LabelType\x12\x12\n\nlabelValue\x18\x04 \x01(\t\"\x13\n\x11\x41igcDeviceBindRes\"*\n\x13\x41igcDeviceUnBindReq\x12\x13\n\x0b\x64\x65viceToken\x18\x03 \x01(\t\"\x15\n\x13\x41igcDeviceUnBindRes\"G\n\x11\x41igcDeviceInfoReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x11\n\tdeviceKey\x18\x02 \x01(\t\x12\x0e\n\x06\x65xtend\x18\x03 \x01(\t\"`\n\x11\x41igcDeviceInfoRes\x12\x11\n\tdeviceKey\x18\x01 \x01(\t\x12\x11\n\tgroupUUID\x18\x02 \x01(\t\x12\x16\n\x0eisCreateWidget\x18\x03 \x01(\x08\x12\r\n\x05token\x18\x04 \x01(\t\"\x10\n\x0e\x41pplyWidgetReq\"$\n\x0e\x41pplyWidgetRes\x12\x12\n\nwidgetUUID\x18\x01 \x01(\t\"\x11\n\x0f\x43reateWidgetReq\"%\n\x0f\x43reateWidgetRes\x12\x12\n\nwidgetUUID\x18\x01 \x01(\t\"9\n\x12UploadWidgetUrlReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x12\n\nwidgetUUID\x18\x02 \x01(\t\"6\n\x12UploadWidgetUrlRes\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x63ontentType\x18\x02 \x01(\t\"3\n\x0fUploadWidgetReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x0f\n\x07\x66ileUrl\x18\x02 \x01(\t\"\"\n\x0fUploadWidgetRes\x12\x0f\n\x07\x63heckId\x18\x01 \x01(\x03\"8\n\x14UploadWidgetCheckReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x0f\n\x07\x63heckId\x18\x02 \x01(\x03\"R\n\x14UploadWidgetCheckRes\x12&\n\x06status\x18\x01 \x01(\x0e\x32\x16.pb.UploadWidgetStatus\x12\x12\n\nfailReason\x18\x02 \x01(\t\"\x88\x01\n\x12\x41igcCreateGroupReq\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12 \n\tlabelType\x18\x05 \x01(\x0e\x32\r.pb.LabelType\x12\x0f\n\x07labelId\x18\x06 \x01(\x03\x12\x0e\n\x06status\x18\x07 \x01(\x05\".\n\x12\x41igcCreateGroupRes\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04uuid\x18\x02 \x01(\t\"V\n\x12\x41igcRemoveGroupReq\x12\n\n\x02id\x18\x01 \x01(\x03\x12 \n\tlabelType\x18\x02 \x01(\x0e\x32\r.pb.LabelType\x12\x12\n\nlabelValue\x18\x03 \x01(\t\"\x14\n\x12\x41igcRemoveGroupRes\",\n\x0e\x41igcTaskResult\x12\x1a\n\x04list\x18\x01 \x03(\x0b\x32\x0c.pb.AigcData\"S\n\x08\x41igcData\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x02 \x03(\t\x12(\n\textension\x18\x03 \x01(\x0b\x32\x15.pb.AigcDataExtension\"S\n\x11\x41igcDataExtension\x12\x0c\n\x04info\x18\x01 \x01(\t\x12\x11\n\tcover_url\x18\x02 \x01(\t\x12\x0e\n\x06height\x18\x03 \x01(\x05\x12\r\n\x05width\x18\x04 \x01(\x05\"C\n\x10UploadFileUrlReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\x12\x0f\n\x07\x66ileExt\x18\x03 \x01(\t\"4\n\x10UploadFileUrlRes\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x63ontentType\x18\x02 \x01(\t\"@\n\x16\x41igcDeviceExpansionReq\x12\x13\n\x0b\x44\x65viceToken\x18\x01 \x01(\t\x12\x11\n\tDeviceKey\x18\x02 \x01(\t\"S\n\x16\x41igcDeviceExpansionRes\x12\x11\n\tdeviceKey\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65viceToken\x18\x02 \x01(\t\x12\x11\n\tgroupUUID\x18\x03 \x01(\t\"6\n\rTaskCountItem\x12\x12\n\nwidgetUUID\x18\x01 \x01(\t\x12\x11\n\ttaskCount\x18\x02 \x01(\x03\"#\n\x0cTaskCountReq\x12\x13\n\x0b\x64\x65viceToken\x18\x01 \x01(\t\"0\n\x0cTaskCountRes\x12 \n\x05items\x18\x01 \x03(\x0b\x32\x11.pb.TaskCountItem\"@\n\x0e\x41igcWidgetItem\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nupdated_at\x18\x03 \x01(\t\"(\n\x11\x41igcWidgetListReq\x12\x13\n\x0b\x64\x65viceToken\x18\x01 \x01(\t\"6\n\x11\x41igcWidgetListRes\x12!\n\x05items\x18\x01 \x03(\x0b\x32\x12.pb.AigcWidgetItem\"J\n\x13\x44\x65leteAigcWidgetReq\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x12\n\nwidgetUUID\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65viceToken\x18\x03 \x01(\t\"\x15\n\x13\x44\x65leteAigcWidgetRes\")\n\x10\x41igcWidgetConfig\x12\x15\n\rmaxTaskNumber\x18\x01 \x01(\x03\"\x1f\n\x11\x41igcWidgetInfoReq\x12\n\n\x02id\x18\x01 \x01(\x03\"\x93\x02\n\x11\x41igcWidgetInfoRes\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04icon\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0b\n\x03url\x18\x05 \x01(\t\x12$\n\x06\x63onfig\x18\x06 \x01(\x0b\x32\x14.pb.AigcWidgetConfig\x12\x19\n\x11\x63urrentTaskNumber\x18\x07 \x01(\x03\x12\x0e\n\x06status\x18\x08 \x01(\x05\x12\r\n\x05price\x18\t \x01(\x01\x12(\n\rcalculateMode\x18\n \x01(\x0e\x32\x11.pb.CalculateMode\x12\x14\n\x0c\x63urTaskCount\x18\x0b \x01(\x03\x12\x14\n\x0cmaxTaskCount\x18\x0c \x01(\x05\"3\n\x11\x41igcBillReportReq\x12\x0f\n\x07useTime\x18\x01 \x01(\x03\x12\r\n\x05isEnd\x18\x02 \x01(\x08\"#\n\x11\x41igcBillReportRes\x12\x0e\n\x06\x61mount\x18\x01 \x01(\x01\"(\n\x14\x41igcTrainingModelReq\x12\x10\n\x08widgetId\x18\x01 \x01(\x03\"%\n\x14\x41igcTrainingModelRes\x12\r\n\x05items\x18\x01 \x03(\t\":\n\x13\x41igcEnableServerReq\x12\x10\n\x08widgetId\x18\x01 \x01(\x03\x12\x11\n\tgroupUUID\x18\x02 \x01(\t\"\"\n\x13\x41igcEnableServerRes\x12\x0b\n\x03url\x18\x01 \x01(\t\"W\n\x0b\x41\x64\x64GroupReq\x12\x10\n\x08group_id\x18\x01 \x01(\x03\x12!\n\nlabel_type\x18\x02 \x01(\x0e\x32\r.pb.LabelType\x12\x13\n\x0blabel_value\x18\x03 \x01(\t\"\r\n\x0b\x41\x64\x64GroupRes\"\x1e\n\x10\x41igcGroupInfoReq\x12\n\n\x02id\x18\x01 \x01(\x03\"\xff\x01\n\x10\x41igcGroupInfoRes\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x0f\n\x07user_id\x18\x03 \x01(\x03\x12\x10\n\x08nickname\x18\x04 \x01(\t\x12\x12\n\nhead_image\x18\x05 \x01(\t\x12\x0e\n\x06status\x18\x06 \x01(\x05\x12\x12\n\ndevice_num\x18\x07 \x01(\x03\x12)\n\x0cgroup_config\x18\x08 \x01(\x0b\x32\x13.pb.AigcGroupConfig\x12\x19\n\x11total_compute_num\x18\t \x01(\x01\x12\x18\n\x10used_compute_num\x18\n \x01(\x01\x12\x16\n\x0eis_edit_config\x18\x0b \x01(\x08\"\'\n\x0f\x41igcGroupConfig\x12\x14\n\x0cshare_config\x18\x01 \x01(\x08\"%\n\x11GetGroupDeviceReq\x12\x10\n\x08group_id\x18\x01 \x01(\x03\"<\n\x11GetGroupDeviceRes\x12\'\n\x0b\x64\x65vice_list\x18\x01 \x03(\x0b\x32\x12.pb.AigcDeviceInfo\"\xa2\x01\n\x0e\x41igcDeviceInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0f\n\x07user_id\x18\x02 \x01(\x03\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x12\n\nhead_image\x18\x04 \x01(\t\x12\x15\n\rgenerated_num\x18\x05 \x01(\x03\x12\x11\n\tis_online\x18\x06 \x01(\x08\x12#\n\x0b\x64\x65vice_info\x18\x07 \x01(\x0b\x32\x0e.pb.DeviceInfo\"\x1e\n\nDeviceInfo\x12\x10\n\x08gpu_name\x18\x01 \x01(\t\"k\n\x12\x45\x64itGroupConfigReq\x12\x10\n\x08group_id\x18\x01 \x01(\x03\x12$\n\x07op_type\x18\x02 \x01(\x0e\x32\x13.pb.GroupConfigType\x12\x14\n\nedit_value\x18\x03 \x01(\x08H\x00\x42\x07\n\x05Param\"\x14\n\x12\x45\x64itGroupConfigRes\"F\n\x11GetDeviceGroupReq\x12 \n\tlabelType\x18\x01 \x01(\x0e\x32\r.pb.LabelType\x12\x0f\n\x07labelId\x18\x02 \x01(\x03\"6\n\x11GetDeviceGroupRes\x12!\n\x04list\x18\x02 \x03(\x0b\x32\x13.pb.AigcDeviceGroup\"\x86\x01\n\x0f\x41igcDeviceGroup\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04icon\x18\x04 \x01(\t\x12\"\n\nwidgetList\x18\x05 \x03(\x0b\x32\x0e.pb.AigcWidget\x12\x19\n\x11total_compute_num\x18\x06 \x01(\x03\"\xd4\x01\n\nAigcWidget\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04icon\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0b\n\x03url\x18\x05 \x01(\t\x12\x1c\n\x04type\x18\x06 \x01(\x0e\x32\x0e.pb.WidgetType\x12\x14\n\x0cmaxTaskCount\x18\x07 \x01(\x05\x12\r\n\x05price\x18\x08 \x01(\x01\x12(\n\rcalculateMode\x18\t \x01(\x0e\x32\x11.pb.CalculateMode\x12\x0f\n\x07groupId\x18\n \x01(\x03\"9\n\x1a\x41igcOfficialMarketModelReq\x12\r\n\x05Limit\x18\x01 \x01(\x05\x12\x0c\n\x04Type\x18\x02 \x01(\t\"@\n\x1a\x41igcOfficialMarketModelRes\x12\"\n\x05items\x18\x01 \x03(\x0b\x32\x13.pb.AigcMarketModel\"\xe4\x01\n\x0f\x41igcMarketModel\x12\n\n\x02Id\x18\x01 \x01(\x03\x12\x0c\n\x04UUID\x18\x02 \x01(\t\x12\x0c\n\x04Name\x18\x03 \x01(\t\x12\x0c\n\x04Type\x18\x04 \x01(\t\x12\x13\n\x0b\x44\x65scription\x18\x05 \x01(\t\x12\r\n\x05\x43over\x18\x06 \x01(\t\x12\x0b\n\x03URL\x18\x07 \x01(\t\x12\x0f\n\x07\x66ileExt\x18\x08 \x01(\t\x12\x10\n\x08\x66ileName\x18\t \x01(\t\x12\x0f\n\x07user_id\x18\n \x01(\x03\x12\x10\n\x08nickname\x18\x0b \x01(\t\x12\x12\n\nhead_image\x18\x0c \x01(\t\x12\x10\n\x08official\x18\r \x01(\x08\"6\n\x17\x41igcTrainMarketModelReq\x12\r\n\x05Limit\x18\x01 \x01(\x05\x12\x0c\n\x04Type\x18\x02 \x01(\t\"=\n\x17\x41igcTrainMarketModelRes\x12\"\n\x05items\x18\x01 \x03(\x0b\x32\x13.pb.AigcMarketModel\"J\n\x17\x41igcAppVersionLatestReq\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08platform\x18\x03 \x01(\t\"v\n\x17\x41igcAppVersionLatestRes\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12(\n\x08\x64iffInfo\x18\x04 \x01(\x0b\x32\x16.pb.AigcAppVersionDiff\"l\n\x17\x43reateAigcAppVersionReq\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x10\n\x08platform\x18\x05 \x01(\t\"\x19\n\x17\x43reateAigcAppVersionRes\"g\n\x1b\x43reateAigcAppVersionDiffReq\x12\x0c\n\x04name\x18\x01 \x01(\t\x12(\n\x08\x64iffList\x18\x02 \x03(\x0b\x32\x16.pb.AigcAppVersionDiff\x12\x10\n\x08platform\x18\x03 \x01(\t\"\x1d\n\x1b\x43reateAigcAppVersionDiffRes\"K\n\x12\x41igcAppVersionDiff\x12\x14\n\x0cstartVersion\x18\x01 \x01(\t\x12\x12\n\nendVersion\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\"\xd2\x01\n\x12MarketModelListReq\x12\x0c\n\x04self\x18\x01 \x01(\x08\x12\x11\n\tsort_type\x18\x02 \x01(\x05\x12\x12\n\nmodel_type\x18\x03 \x03(\x03\x12\x11\n\tattribute\x18\x04 \x03(\x03\x12\x10\n\x08\x63\x61tegory\x18\x05 \x03(\x03\x12\x16\n\x0esearch_keyword\x18\x06 \x01(\t\x12\x0c\n\x04page\x18\x07 \x01(\x03\x12\x0c\n\x04size\x18\x08 \x01(\x03\x12\x17\n\x0fupdateStartTime\x18\t \x01(\t\x12\x15\n\rupdateEndTime\x18\n \x01(\t\"8\n\x12MarketModelListRes\x12\"\n\x05items\x18\x01 \x03(\x0b\x32\x13.pb.AigcMarketModel\"\x19\n\x17MarketModelFieldEnumReq\"\xa0\x01\n\x17MarketModelFieldEnumRes\x12,\n\nmodel_type\x18\x01 \x03(\x0b\x32\x18.pb.MarketModelFieldItem\x12+\n\tattribute\x18\x02 \x03(\x0b\x32\x18.pb.MarketModelFieldItem\x12*\n\x08\x63\x61tegory\x18\x03 \x03(\x0b\x32\x18.pb.MarketModelFieldItem\"0\n\x14MarketModelFieldItem\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\"$\n\x16MarketModelDownloadReq\x12\n\n\x02Id\x18\x01 \x01(\x03\"\x18\n\x16MarketModelDownloadRes\"h\n\x1cMarketModelCreateWithTaskReq\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x63over\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x10\n\x08TaskUUID\x18\x05 \x01(\t\"\x1e\n\x1cMarketModelCreateWithTaskRes\"\x15\n\x13MarketPluginListReq\"@\n\x13MarketPluginListRes\x12)\n\x0bplugin_list\x18\x01 \x03(\x0b\x32\x14.pb.MarketPluginItem\"j\n\x10MarketPluginItem\x12\n\n\x02Id\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0b\n\x03url\x18\x05 \x01(\t\x12\x0c\n\x04tags\x18\x06 \x03(\t*X\n\x12UploadWidgetStatus\x12\x0c\n\x08UWS_NONE\x10\x00\x12\x12\n\x0eUWS_PROCESSING\x10\x01\x12\x0f\n\x0bUWS_SUCCESS\x10\x02\x12\x0f\n\x0bUWS_FAILURE\x10\x03*7\n\x0fGroupConfigType\x12\x0f\n\x0bGCT_Unknown\x10\x00\x12\x13\n\x0fGCT_ShareConfig\x10\x01\x32\xa2\x12\n\nAigcExtObj\x12)\n\x07GetTask\x12\x0e.pb.GetTaskReq\x1a\x0e.pb.GetTaskRes\x12\x32\n\nTaskNotify\x12\x11.pb.TaskNotifyReq\x1a\x11.pb.TaskNotifyRes\x12/\n\tTaskCount\x12\x10.pb.TaskCountReq\x1a\x10.pb.TaskCountRes\x12:\n\nDeviceBind\x12\x15.pb.AigcDeviceBindReq\x1a\x15.pb.AigcDeviceBindRes\x12@\n\x0c\x44\x65viceUnBind\x12\x17.pb.AigcDeviceUnBindReq\x1a\x17.pb.AigcDeviceUnBindRes\x12:\n\nDeviceInfo\x12\x15.pb.AigcDeviceInfoReq\x1a\x15.pb.AigcDeviceInfoRes\x12I\n\x0f\x44\x65viceExpansion\x12\x1a.pb.AigcDeviceExpansionReq\x1a\x1a.pb.AigcDeviceExpansionRes\x12\x35\n\x0b\x41pplyWidget\x12\x12.pb.ApplyWidgetReq\x1a\x12.pb.ApplyWidgetRes\x12\x38\n\x0c\x43reateWidget\x12\x13.pb.CreateWidgetReq\x1a\x13.pb.CreateWidgetRes\x12@\n\x0c\x44\x65leteWidget\x12\x17.pb.DeleteAigcWidgetReq\x1a\x17.pb.DeleteAigcWidgetRes\x12:\n\nWidgetList\x12\x15.pb.AigcWidgetListReq\x1a\x15.pb.AigcWidgetListRes\x12:\n\nWidgetInfo\x12\x15.pb.AigcWidgetInfoReq\x1a\x15.pb.AigcWidgetInfoRes\x12\x38\n\x0cUploadWidget\x12\x13.pb.UploadWidgetReq\x1a\x13.pb.UploadWidgetRes\x12\x41\n\x0fUploadWidgetUrl\x12\x16.pb.UploadWidgetUrlReq\x1a\x16.pb.UploadWidgetUrlRes\x12;\n\rUploadFileUrl\x12\x14.pb.UploadFileUrlReq\x1a\x14.pb.UploadFileUrlRes\x12G\n\x11UploadWidgetCheck\x12\x18.pb.UploadWidgetCheckReq\x1a\x18.pb.UploadWidgetCheckRes\x12=\n\x0bRemoveGroup\x12\x16.pb.AigcRemoveGroupReq\x1a\x16.pb.AigcRemoveGroupRes\x12:\n\nBillReport\x12\x15.pb.AigcBillReportReq\x1a\x15.pb.AigcBillReportRes\x12\x43\n\rTrainingModel\x12\x18.pb.AigcTrainingModelReq\x1a\x18.pb.AigcTrainingModelRes\x12@\n\x0c\x45nableServer\x12\x17.pb.AigcEnableServerReq\x1a\x17.pb.AigcEnableServerRes\x12,\n\x08\x41\x64\x64Group\x12\x0f.pb.AddGroupReq\x1a\x0f.pb.AddGroupRes\x12:\n\x0cGetGroupInfo\x12\x14.pb.AigcGroupInfoReq\x1a\x14.pb.AigcGroupInfoRes\x12>\n\x0eGetGroupDevice\x12\x15.pb.GetGroupDeviceReq\x1a\x15.pb.GetGroupDeviceRes\x12\x41\n\x0f\x45\x64itGroupConfig\x12\x16.pb.EditGroupConfigReq\x1a\x16.pb.EditGroupConfigRes\x12<\n\x0cGetGroupList\x12\x15.pb.GetDeviceGroupReq\x1a\x15.pb.GetDeviceGroupRes\x12U\n\x13OfficialMarketModel\x12\x1e.pb.AigcOfficialMarketModelReq\x1a\x1e.pb.AigcOfficialMarketModelRes\x12L\n\x10TrainMarketModel\x12\x1b.pb.AigcTrainMarketModelReq\x1a\x1b.pb.AigcTrainMarketModelRes\x12L\n\x10\x41ppVersionLatest\x12\x1b.pb.AigcAppVersionLatestReq\x1a\x1b.pb.AigcAppVersionLatestRes\x12L\n\x10\x43reateAppVersion\x12\x1b.pb.CreateAigcAppVersionReq\x1a\x1b.pb.CreateAigcAppVersionRes\x12X\n\x14\x43reateAppVersionDiff\x12\x1f.pb.CreateAigcAppVersionDiffReq\x1a\x1f.pb.CreateAigcAppVersionDiffRes\x12\x41\n\x0fMarketModelList\x12\x16.pb.MarketModelListReq\x1a\x16.pb.MarketModelListRes\x12P\n\x14MarketModelFieldEnum\x12\x1b.pb.MarketModelFieldEnumReq\x1a\x1b.pb.MarketModelFieldEnumRes\x12M\n\x13MarketModelDownload\x12\x1a.pb.MarketModelDownloadReq\x1a\x1a.pb.MarketModelDownloadRes\x12_\n\x19MarketModelCreateWithTask\x12 .pb.MarketModelCreateWithTaskReq\x1a .pb.MarketModelCreateWithTaskRes\x12\x44\n\x10MarketPluginList\x12\x17.pb.MarketPluginListReq\x1a\x17.pb.MarketPluginListResB\x06\xa2\x02\x03PB3b\x06proto3')
-
-_UPLOADWIDGETSTATUS = DESCRIPTOR.enum_types_by_name['UploadWidgetStatus']
-UploadWidgetStatus = enum_type_wrapper.EnumTypeWrapper(_UPLOADWIDGETSTATUS)
-_GROUPCONFIGTYPE = DESCRIPTOR.enum_types_by_name['GroupConfigType']
-GroupConfigType = enum_type_wrapper.EnumTypeWrapper(_GROUPCONFIGTYPE)
-UWS_NONE = 0
-UWS_PROCESSING = 1
-UWS_SUCCESS = 2
-UWS_FAILURE = 3
-GCT_Unknown = 0
-GCT_ShareConfig = 1
-
-
-_TASKITEM = DESCRIPTOR.message_types_by_name['TaskItem']
-_GETTASKREQ = DESCRIPTOR.message_types_by_name['GetTaskReq']
-_GETTASKRES = DESCRIPTOR.message_types_by_name['GetTaskRes']
-_TASKNOTIFYREQ = DESCRIPTOR.message_types_by_name['TaskNotifyReq']
-_TASKNOTIFYRES = DESCRIPTOR.message_types_by_name['TaskNotifyRes']
-_AIGCDEVICEBINDREQ = DESCRIPTOR.message_types_by_name['AigcDeviceBindReq']
-_AIGCDEVICEBINDRES = DESCRIPTOR.message_types_by_name['AigcDeviceBindRes']
-_AIGCDEVICEUNBINDREQ = DESCRIPTOR.message_types_by_name['AigcDeviceUnBindReq']
-_AIGCDEVICEUNBINDRES = DESCRIPTOR.message_types_by_name['AigcDeviceUnBindRes']
-_AIGCDEVICEINFOREQ = DESCRIPTOR.message_types_by_name['AigcDeviceInfoReq']
-_AIGCDEVICEINFORES = DESCRIPTOR.message_types_by_name['AigcDeviceInfoRes']
-_APPLYWIDGETREQ = DESCRIPTOR.message_types_by_name['ApplyWidgetReq']
-_APPLYWIDGETRES = DESCRIPTOR.message_types_by_name['ApplyWidgetRes']
-_CREATEWIDGETREQ = DESCRIPTOR.message_types_by_name['CreateWidgetReq']
-_CREATEWIDGETRES = DESCRIPTOR.message_types_by_name['CreateWidgetRes']
-_UPLOADWIDGETURLREQ = DESCRIPTOR.message_types_by_name['UploadWidgetUrlReq']
-_UPLOADWIDGETURLRES = DESCRIPTOR.message_types_by_name['UploadWidgetUrlRes']
-_UPLOADWIDGETREQ = DESCRIPTOR.message_types_by_name['UploadWidgetReq']
-_UPLOADWIDGETRES = DESCRIPTOR.message_types_by_name['UploadWidgetRes']
-_UPLOADWIDGETCHECKREQ = DESCRIPTOR.message_types_by_name['UploadWidgetCheckReq']
-_UPLOADWIDGETCHECKRES = DESCRIPTOR.message_types_by_name['UploadWidgetCheckRes']
-_AIGCCREATEGROUPREQ = DESCRIPTOR.message_types_by_name['AigcCreateGroupReq']
-_AIGCCREATEGROUPRES = DESCRIPTOR.message_types_by_name['AigcCreateGroupRes']
-_AIGCREMOVEGROUPREQ = DESCRIPTOR.message_types_by_name['AigcRemoveGroupReq']
-_AIGCREMOVEGROUPRES = DESCRIPTOR.message_types_by_name['AigcRemoveGroupRes']
-_AIGCTASKRESULT = DESCRIPTOR.message_types_by_name['AigcTaskResult']
-_AIGCDATA = DESCRIPTOR.message_types_by_name['AigcData']
-_AIGCDATAEXTENSION = DESCRIPTOR.message_types_by_name['AigcDataExtension']
-_UPLOADFILEURLREQ = DESCRIPTOR.message_types_by_name['UploadFileUrlReq']
-_UPLOADFILEURLRES = DESCRIPTOR.message_types_by_name['UploadFileUrlRes']
-_AIGCDEVICEEXPANSIONREQ = DESCRIPTOR.message_types_by_name['AigcDeviceExpansionReq']
-_AIGCDEVICEEXPANSIONRES = DESCRIPTOR.message_types_by_name['AigcDeviceExpansionRes']
-_TASKCOUNTITEM = DESCRIPTOR.message_types_by_name['TaskCountItem']
-_TASKCOUNTREQ = DESCRIPTOR.message_types_by_name['TaskCountReq']
-_TASKCOUNTRES = DESCRIPTOR.message_types_by_name['TaskCountRes']
-_AIGCWIDGETITEM = DESCRIPTOR.message_types_by_name['AigcWidgetItem']
-_AIGCWIDGETLISTREQ = DESCRIPTOR.message_types_by_name['AigcWidgetListReq']
-_AIGCWIDGETLISTRES = DESCRIPTOR.message_types_by_name['AigcWidgetListRes']
-_DELETEAIGCWIDGETREQ = DESCRIPTOR.message_types_by_name['DeleteAigcWidgetReq']
-_DELETEAIGCWIDGETRES = DESCRIPTOR.message_types_by_name['DeleteAigcWidgetRes']
-_AIGCWIDGETCONFIG = DESCRIPTOR.message_types_by_name['AigcWidgetConfig']
-_AIGCWIDGETINFOREQ = DESCRIPTOR.message_types_by_name['AigcWidgetInfoReq']
-_AIGCWIDGETINFORES = DESCRIPTOR.message_types_by_name['AigcWidgetInfoRes']
-_AIGCBILLREPORTREQ = DESCRIPTOR.message_types_by_name['AigcBillReportReq']
-_AIGCBILLREPORTRES = DESCRIPTOR.message_types_by_name['AigcBillReportRes']
-_AIGCTRAININGMODELREQ = DESCRIPTOR.message_types_by_name['AigcTrainingModelReq']
-_AIGCTRAININGMODELRES = DESCRIPTOR.message_types_by_name['AigcTrainingModelRes']
-_AIGCENABLESERVERREQ = DESCRIPTOR.message_types_by_name['AigcEnableServerReq']
-_AIGCENABLESERVERRES = DESCRIPTOR.message_types_by_name['AigcEnableServerRes']
-_ADDGROUPREQ = DESCRIPTOR.message_types_by_name['AddGroupReq']
-_ADDGROUPRES = DESCRIPTOR.message_types_by_name['AddGroupRes']
-_AIGCGROUPINFOREQ = DESCRIPTOR.message_types_by_name['AigcGroupInfoReq']
-_AIGCGROUPINFORES = DESCRIPTOR.message_types_by_name['AigcGroupInfoRes']
-_AIGCGROUPCONFIG = DESCRIPTOR.message_types_by_name['AigcGroupConfig']
-_GETGROUPDEVICEREQ = DESCRIPTOR.message_types_by_name['GetGroupDeviceReq']
-_GETGROUPDEVICERES = DESCRIPTOR.message_types_by_name['GetGroupDeviceRes']
-_AIGCDEVICEINFO = DESCRIPTOR.message_types_by_name['AigcDeviceInfo']
-_DEVICEINFO = DESCRIPTOR.message_types_by_name['DeviceInfo']
-_EDITGROUPCONFIGREQ = DESCRIPTOR.message_types_by_name['EditGroupConfigReq']
-_EDITGROUPCONFIGRES = DESCRIPTOR.message_types_by_name['EditGroupConfigRes']
-_GETDEVICEGROUPREQ = DESCRIPTOR.message_types_by_name['GetDeviceGroupReq']
-_GETDEVICEGROUPRES = DESCRIPTOR.message_types_by_name['GetDeviceGroupRes']
-_AIGCDEVICEGROUP = DESCRIPTOR.message_types_by_name['AigcDeviceGroup']
-_AIGCWIDGET = DESCRIPTOR.message_types_by_name['AigcWidget']
-_AIGCOFFICIALMARKETMODELREQ = DESCRIPTOR.message_types_by_name['AigcOfficialMarketModelReq']
-_AIGCOFFICIALMARKETMODELRES = DESCRIPTOR.message_types_by_name['AigcOfficialMarketModelRes']
-_AIGCMARKETMODEL = DESCRIPTOR.message_types_by_name['AigcMarketModel']
-_AIGCTRAINMARKETMODELREQ = DESCRIPTOR.message_types_by_name['AigcTrainMarketModelReq']
-_AIGCTRAINMARKETMODELRES = DESCRIPTOR.message_types_by_name['AigcTrainMarketModelRes']
-_AIGCAPPVERSIONLATESTREQ = DESCRIPTOR.message_types_by_name['AigcAppVersionLatestReq']
-_AIGCAPPVERSIONLATESTRES = DESCRIPTOR.message_types_by_name['AigcAppVersionLatestRes']
-_CREATEAIGCAPPVERSIONREQ = DESCRIPTOR.message_types_by_name['CreateAigcAppVersionReq']
-_CREATEAIGCAPPVERSIONRES = DESCRIPTOR.message_types_by_name['CreateAigcAppVersionRes']
-_CREATEAIGCAPPVERSIONDIFFREQ = DESCRIPTOR.message_types_by_name['CreateAigcAppVersionDiffReq']
-_CREATEAIGCAPPVERSIONDIFFRES = DESCRIPTOR.message_types_by_name['CreateAigcAppVersionDiffRes']
-_AIGCAPPVERSIONDIFF = DESCRIPTOR.message_types_by_name['AigcAppVersionDiff']
-_MARKETMODELLISTREQ = DESCRIPTOR.message_types_by_name['MarketModelListReq']
-_MARKETMODELLISTRES = DESCRIPTOR.message_types_by_name['MarketModelListRes']
-_MARKETMODELFIELDENUMREQ = DESCRIPTOR.message_types_by_name['MarketModelFieldEnumReq']
-_MARKETMODELFIELDENUMRES = DESCRIPTOR.message_types_by_name['MarketModelFieldEnumRes']
-_MARKETMODELFIELDITEM = DESCRIPTOR.message_types_by_name['MarketModelFieldItem']
-_MARKETMODELDOWNLOADREQ = DESCRIPTOR.message_types_by_name['MarketModelDownloadReq']
-_MARKETMODELDOWNLOADRES = DESCRIPTOR.message_types_by_name['MarketModelDownloadRes']
-_MARKETMODELCREATEWITHTASKREQ = DESCRIPTOR.message_types_by_name['MarketModelCreateWithTaskReq']
-_MARKETMODELCREATEWITHTASKRES = DESCRIPTOR.message_types_by_name['MarketModelCreateWithTaskRes']
-_MARKETPLUGINLISTREQ = DESCRIPTOR.message_types_by_name['MarketPluginListReq']
-_MARKETPLUGINLISTRES = DESCRIPTOR.message_types_by_name['MarketPluginListRes']
-_MARKETPLUGINITEM = DESCRIPTOR.message_types_by_name['MarketPluginItem']
-TaskItem = _reflection.GeneratedProtocolMessageType('TaskItem', (_message.Message,), {
-  'DESCRIPTOR' : _TASKITEM,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.TaskItem)
-  })
-_sym_db.RegisterMessage(TaskItem)
-
-GetTaskReq = _reflection.GeneratedProtocolMessageType('GetTaskReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETTASKREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.GetTaskReq)
-  })
-_sym_db.RegisterMessage(GetTaskReq)
-
-GetTaskRes = _reflection.GeneratedProtocolMessageType('GetTaskRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETTASKRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.GetTaskRes)
-  })
-_sym_db.RegisterMessage(GetTaskRes)
-
-TaskNotifyReq = _reflection.GeneratedProtocolMessageType('TaskNotifyReq', (_message.Message,), {
-  'DESCRIPTOR' : _TASKNOTIFYREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.TaskNotifyReq)
-  })
-_sym_db.RegisterMessage(TaskNotifyReq)
-
-TaskNotifyRes = _reflection.GeneratedProtocolMessageType('TaskNotifyRes', (_message.Message,), {
-  'DESCRIPTOR' : _TASKNOTIFYRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.TaskNotifyRes)
-  })
-_sym_db.RegisterMessage(TaskNotifyRes)
-
-AigcDeviceBindReq = _reflection.GeneratedProtocolMessageType('AigcDeviceBindReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCDEVICEBINDREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcDeviceBindReq)
-  })
-_sym_db.RegisterMessage(AigcDeviceBindReq)
-
-AigcDeviceBindRes = _reflection.GeneratedProtocolMessageType('AigcDeviceBindRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCDEVICEBINDRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcDeviceBindRes)
-  })
-_sym_db.RegisterMessage(AigcDeviceBindRes)
-
-AigcDeviceUnBindReq = _reflection.GeneratedProtocolMessageType('AigcDeviceUnBindReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCDEVICEUNBINDREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcDeviceUnBindReq)
-  })
-_sym_db.RegisterMessage(AigcDeviceUnBindReq)
-
-AigcDeviceUnBindRes = _reflection.GeneratedProtocolMessageType('AigcDeviceUnBindRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCDEVICEUNBINDRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcDeviceUnBindRes)
-  })
-_sym_db.RegisterMessage(AigcDeviceUnBindRes)
-
-AigcDeviceInfoReq = _reflection.GeneratedProtocolMessageType('AigcDeviceInfoReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCDEVICEINFOREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcDeviceInfoReq)
-  })
-_sym_db.RegisterMessage(AigcDeviceInfoReq)
-
-AigcDeviceInfoRes = _reflection.GeneratedProtocolMessageType('AigcDeviceInfoRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCDEVICEINFORES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcDeviceInfoRes)
-  })
-_sym_db.RegisterMessage(AigcDeviceInfoRes)
-
-ApplyWidgetReq = _reflection.GeneratedProtocolMessageType('ApplyWidgetReq', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYWIDGETREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.ApplyWidgetReq)
-  })
-_sym_db.RegisterMessage(ApplyWidgetReq)
-
-ApplyWidgetRes = _reflection.GeneratedProtocolMessageType('ApplyWidgetRes', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYWIDGETRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.ApplyWidgetRes)
-  })
-_sym_db.RegisterMessage(ApplyWidgetRes)
-
-CreateWidgetReq = _reflection.GeneratedProtocolMessageType('CreateWidgetReq', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEWIDGETREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.CreateWidgetReq)
-  })
-_sym_db.RegisterMessage(CreateWidgetReq)
-
-CreateWidgetRes = _reflection.GeneratedProtocolMessageType('CreateWidgetRes', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEWIDGETRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.CreateWidgetRes)
-  })
-_sym_db.RegisterMessage(CreateWidgetRes)
-
-UploadWidgetUrlReq = _reflection.GeneratedProtocolMessageType('UploadWidgetUrlReq', (_message.Message,), {
-  'DESCRIPTOR' : _UPLOADWIDGETURLREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UploadWidgetUrlReq)
-  })
-_sym_db.RegisterMessage(UploadWidgetUrlReq)
-
-UploadWidgetUrlRes = _reflection.GeneratedProtocolMessageType('UploadWidgetUrlRes', (_message.Message,), {
-  'DESCRIPTOR' : _UPLOADWIDGETURLRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UploadWidgetUrlRes)
-  })
-_sym_db.RegisterMessage(UploadWidgetUrlRes)
-
-UploadWidgetReq = _reflection.GeneratedProtocolMessageType('UploadWidgetReq', (_message.Message,), {
-  'DESCRIPTOR' : _UPLOADWIDGETREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UploadWidgetReq)
-  })
-_sym_db.RegisterMessage(UploadWidgetReq)
-
-UploadWidgetRes = _reflection.GeneratedProtocolMessageType('UploadWidgetRes', (_message.Message,), {
-  'DESCRIPTOR' : _UPLOADWIDGETRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UploadWidgetRes)
-  })
-_sym_db.RegisterMessage(UploadWidgetRes)
-
-UploadWidgetCheckReq = _reflection.GeneratedProtocolMessageType('UploadWidgetCheckReq', (_message.Message,), {
-  'DESCRIPTOR' : _UPLOADWIDGETCHECKREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UploadWidgetCheckReq)
-  })
-_sym_db.RegisterMessage(UploadWidgetCheckReq)
-
-UploadWidgetCheckRes = _reflection.GeneratedProtocolMessageType('UploadWidgetCheckRes', (_message.Message,), {
-  'DESCRIPTOR' : _UPLOADWIDGETCHECKRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UploadWidgetCheckRes)
-  })
-_sym_db.RegisterMessage(UploadWidgetCheckRes)
-
-AigcCreateGroupReq = _reflection.GeneratedProtocolMessageType('AigcCreateGroupReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCCREATEGROUPREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcCreateGroupReq)
-  })
-_sym_db.RegisterMessage(AigcCreateGroupReq)
-
-AigcCreateGroupRes = _reflection.GeneratedProtocolMessageType('AigcCreateGroupRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCCREATEGROUPRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcCreateGroupRes)
-  })
-_sym_db.RegisterMessage(AigcCreateGroupRes)
-
-AigcRemoveGroupReq = _reflection.GeneratedProtocolMessageType('AigcRemoveGroupReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCREMOVEGROUPREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcRemoveGroupReq)
-  })
-_sym_db.RegisterMessage(AigcRemoveGroupReq)
-
-AigcRemoveGroupRes = _reflection.GeneratedProtocolMessageType('AigcRemoveGroupRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCREMOVEGROUPRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcRemoveGroupRes)
-  })
-_sym_db.RegisterMessage(AigcRemoveGroupRes)
-
-AigcTaskResult = _reflection.GeneratedProtocolMessageType('AigcTaskResult', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCTASKRESULT,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcTaskResult)
-  })
-_sym_db.RegisterMessage(AigcTaskResult)
-
-AigcData = _reflection.GeneratedProtocolMessageType('AigcData', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCDATA,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcData)
-  })
-_sym_db.RegisterMessage(AigcData)
-
-AigcDataExtension = _reflection.GeneratedProtocolMessageType('AigcDataExtension', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCDATAEXTENSION,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcDataExtension)
-  })
-_sym_db.RegisterMessage(AigcDataExtension)
-
-UploadFileUrlReq = _reflection.GeneratedProtocolMessageType('UploadFileUrlReq', (_message.Message,), {
-  'DESCRIPTOR' : _UPLOADFILEURLREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UploadFileUrlReq)
-  })
-_sym_db.RegisterMessage(UploadFileUrlReq)
-
-UploadFileUrlRes = _reflection.GeneratedProtocolMessageType('UploadFileUrlRes', (_message.Message,), {
-  'DESCRIPTOR' : _UPLOADFILEURLRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UploadFileUrlRes)
-  })
-_sym_db.RegisterMessage(UploadFileUrlRes)
-
-AigcDeviceExpansionReq = _reflection.GeneratedProtocolMessageType('AigcDeviceExpansionReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCDEVICEEXPANSIONREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcDeviceExpansionReq)
-  })
-_sym_db.RegisterMessage(AigcDeviceExpansionReq)
-
-AigcDeviceExpansionRes = _reflection.GeneratedProtocolMessageType('AigcDeviceExpansionRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCDEVICEEXPANSIONRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcDeviceExpansionRes)
-  })
-_sym_db.RegisterMessage(AigcDeviceExpansionRes)
-
-TaskCountItem = _reflection.GeneratedProtocolMessageType('TaskCountItem', (_message.Message,), {
-  'DESCRIPTOR' : _TASKCOUNTITEM,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.TaskCountItem)
-  })
-_sym_db.RegisterMessage(TaskCountItem)
-
-TaskCountReq = _reflection.GeneratedProtocolMessageType('TaskCountReq', (_message.Message,), {
-  'DESCRIPTOR' : _TASKCOUNTREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.TaskCountReq)
-  })
-_sym_db.RegisterMessage(TaskCountReq)
-
-TaskCountRes = _reflection.GeneratedProtocolMessageType('TaskCountRes', (_message.Message,), {
-  'DESCRIPTOR' : _TASKCOUNTRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.TaskCountRes)
-  })
-_sym_db.RegisterMessage(TaskCountRes)
-
-AigcWidgetItem = _reflection.GeneratedProtocolMessageType('AigcWidgetItem', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCWIDGETITEM,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcWidgetItem)
-  })
-_sym_db.RegisterMessage(AigcWidgetItem)
-
-AigcWidgetListReq = _reflection.GeneratedProtocolMessageType('AigcWidgetListReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCWIDGETLISTREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcWidgetListReq)
-  })
-_sym_db.RegisterMessage(AigcWidgetListReq)
-
-AigcWidgetListRes = _reflection.GeneratedProtocolMessageType('AigcWidgetListRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCWIDGETLISTRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcWidgetListRes)
-  })
-_sym_db.RegisterMessage(AigcWidgetListRes)
-
-DeleteAigcWidgetReq = _reflection.GeneratedProtocolMessageType('DeleteAigcWidgetReq', (_message.Message,), {
-  'DESCRIPTOR' : _DELETEAIGCWIDGETREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.DeleteAigcWidgetReq)
-  })
-_sym_db.RegisterMessage(DeleteAigcWidgetReq)
-
-DeleteAigcWidgetRes = _reflection.GeneratedProtocolMessageType('DeleteAigcWidgetRes', (_message.Message,), {
-  'DESCRIPTOR' : _DELETEAIGCWIDGETRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.DeleteAigcWidgetRes)
-  })
-_sym_db.RegisterMessage(DeleteAigcWidgetRes)
-
-AigcWidgetConfig = _reflection.GeneratedProtocolMessageType('AigcWidgetConfig', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCWIDGETCONFIG,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcWidgetConfig)
-  })
-_sym_db.RegisterMessage(AigcWidgetConfig)
-
-AigcWidgetInfoReq = _reflection.GeneratedProtocolMessageType('AigcWidgetInfoReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCWIDGETINFOREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcWidgetInfoReq)
-  })
-_sym_db.RegisterMessage(AigcWidgetInfoReq)
-
-AigcWidgetInfoRes = _reflection.GeneratedProtocolMessageType('AigcWidgetInfoRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCWIDGETINFORES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcWidgetInfoRes)
-  })
-_sym_db.RegisterMessage(AigcWidgetInfoRes)
-
-AigcBillReportReq = _reflection.GeneratedProtocolMessageType('AigcBillReportReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCBILLREPORTREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcBillReportReq)
-  })
-_sym_db.RegisterMessage(AigcBillReportReq)
-
-AigcBillReportRes = _reflection.GeneratedProtocolMessageType('AigcBillReportRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCBILLREPORTRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcBillReportRes)
-  })
-_sym_db.RegisterMessage(AigcBillReportRes)
-
-AigcTrainingModelReq = _reflection.GeneratedProtocolMessageType('AigcTrainingModelReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCTRAININGMODELREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcTrainingModelReq)
-  })
-_sym_db.RegisterMessage(AigcTrainingModelReq)
-
-AigcTrainingModelRes = _reflection.GeneratedProtocolMessageType('AigcTrainingModelRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCTRAININGMODELRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcTrainingModelRes)
-  })
-_sym_db.RegisterMessage(AigcTrainingModelRes)
-
-AigcEnableServerReq = _reflection.GeneratedProtocolMessageType('AigcEnableServerReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCENABLESERVERREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcEnableServerReq)
-  })
-_sym_db.RegisterMessage(AigcEnableServerReq)
-
-AigcEnableServerRes = _reflection.GeneratedProtocolMessageType('AigcEnableServerRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCENABLESERVERRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcEnableServerRes)
-  })
-_sym_db.RegisterMessage(AigcEnableServerRes)
-
-AddGroupReq = _reflection.GeneratedProtocolMessageType('AddGroupReq', (_message.Message,), {
-  'DESCRIPTOR' : _ADDGROUPREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AddGroupReq)
-  })
-_sym_db.RegisterMessage(AddGroupReq)
-
-AddGroupRes = _reflection.GeneratedProtocolMessageType('AddGroupRes', (_message.Message,), {
-  'DESCRIPTOR' : _ADDGROUPRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AddGroupRes)
-  })
-_sym_db.RegisterMessage(AddGroupRes)
-
-AigcGroupInfoReq = _reflection.GeneratedProtocolMessageType('AigcGroupInfoReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCGROUPINFOREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcGroupInfoReq)
-  })
-_sym_db.RegisterMessage(AigcGroupInfoReq)
-
-AigcGroupInfoRes = _reflection.GeneratedProtocolMessageType('AigcGroupInfoRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCGROUPINFORES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcGroupInfoRes)
-  })
-_sym_db.RegisterMessage(AigcGroupInfoRes)
-
-AigcGroupConfig = _reflection.GeneratedProtocolMessageType('AigcGroupConfig', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCGROUPCONFIG,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcGroupConfig)
-  })
-_sym_db.RegisterMessage(AigcGroupConfig)
-
-GetGroupDeviceReq = _reflection.GeneratedProtocolMessageType('GetGroupDeviceReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETGROUPDEVICEREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.GetGroupDeviceReq)
-  })
-_sym_db.RegisterMessage(GetGroupDeviceReq)
-
-GetGroupDeviceRes = _reflection.GeneratedProtocolMessageType('GetGroupDeviceRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETGROUPDEVICERES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.GetGroupDeviceRes)
-  })
-_sym_db.RegisterMessage(GetGroupDeviceRes)
-
-AigcDeviceInfo = _reflection.GeneratedProtocolMessageType('AigcDeviceInfo', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCDEVICEINFO,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcDeviceInfo)
-  })
-_sym_db.RegisterMessage(AigcDeviceInfo)
-
-DeviceInfo = _reflection.GeneratedProtocolMessageType('DeviceInfo', (_message.Message,), {
-  'DESCRIPTOR' : _DEVICEINFO,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.DeviceInfo)
-  })
-_sym_db.RegisterMessage(DeviceInfo)
-
-EditGroupConfigReq = _reflection.GeneratedProtocolMessageType('EditGroupConfigReq', (_message.Message,), {
-  'DESCRIPTOR' : _EDITGROUPCONFIGREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.EditGroupConfigReq)
-  })
-_sym_db.RegisterMessage(EditGroupConfigReq)
-
-EditGroupConfigRes = _reflection.GeneratedProtocolMessageType('EditGroupConfigRes', (_message.Message,), {
-  'DESCRIPTOR' : _EDITGROUPCONFIGRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.EditGroupConfigRes)
-  })
-_sym_db.RegisterMessage(EditGroupConfigRes)
-
-GetDeviceGroupReq = _reflection.GeneratedProtocolMessageType('GetDeviceGroupReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETDEVICEGROUPREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.GetDeviceGroupReq)
-  })
-_sym_db.RegisterMessage(GetDeviceGroupReq)
-
-GetDeviceGroupRes = _reflection.GeneratedProtocolMessageType('GetDeviceGroupRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETDEVICEGROUPRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.GetDeviceGroupRes)
-  })
-_sym_db.RegisterMessage(GetDeviceGroupRes)
-
-AigcDeviceGroup = _reflection.GeneratedProtocolMessageType('AigcDeviceGroup', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCDEVICEGROUP,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcDeviceGroup)
-  })
-_sym_db.RegisterMessage(AigcDeviceGroup)
-
-AigcWidget = _reflection.GeneratedProtocolMessageType('AigcWidget', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCWIDGET,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcWidget)
-  })
-_sym_db.RegisterMessage(AigcWidget)
-
-AigcOfficialMarketModelReq = _reflection.GeneratedProtocolMessageType('AigcOfficialMarketModelReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCOFFICIALMARKETMODELREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcOfficialMarketModelReq)
-  })
-_sym_db.RegisterMessage(AigcOfficialMarketModelReq)
-
-AigcOfficialMarketModelRes = _reflection.GeneratedProtocolMessageType('AigcOfficialMarketModelRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCOFFICIALMARKETMODELRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcOfficialMarketModelRes)
-  })
-_sym_db.RegisterMessage(AigcOfficialMarketModelRes)
-
-AigcMarketModel = _reflection.GeneratedProtocolMessageType('AigcMarketModel', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCMARKETMODEL,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcMarketModel)
-  })
-_sym_db.RegisterMessage(AigcMarketModel)
-
-AigcTrainMarketModelReq = _reflection.GeneratedProtocolMessageType('AigcTrainMarketModelReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCTRAINMARKETMODELREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcTrainMarketModelReq)
-  })
-_sym_db.RegisterMessage(AigcTrainMarketModelReq)
-
-AigcTrainMarketModelRes = _reflection.GeneratedProtocolMessageType('AigcTrainMarketModelRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCTRAINMARKETMODELRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcTrainMarketModelRes)
-  })
-_sym_db.RegisterMessage(AigcTrainMarketModelRes)
-
-AigcAppVersionLatestReq = _reflection.GeneratedProtocolMessageType('AigcAppVersionLatestReq', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCAPPVERSIONLATESTREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcAppVersionLatestReq)
-  })
-_sym_db.RegisterMessage(AigcAppVersionLatestReq)
-
-AigcAppVersionLatestRes = _reflection.GeneratedProtocolMessageType('AigcAppVersionLatestRes', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCAPPVERSIONLATESTRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcAppVersionLatestRes)
-  })
-_sym_db.RegisterMessage(AigcAppVersionLatestRes)
-
-CreateAigcAppVersionReq = _reflection.GeneratedProtocolMessageType('CreateAigcAppVersionReq', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEAIGCAPPVERSIONREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.CreateAigcAppVersionReq)
-  })
-_sym_db.RegisterMessage(CreateAigcAppVersionReq)
-
-CreateAigcAppVersionRes = _reflection.GeneratedProtocolMessageType('CreateAigcAppVersionRes', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEAIGCAPPVERSIONRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.CreateAigcAppVersionRes)
-  })
-_sym_db.RegisterMessage(CreateAigcAppVersionRes)
-
-CreateAigcAppVersionDiffReq = _reflection.GeneratedProtocolMessageType('CreateAigcAppVersionDiffReq', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEAIGCAPPVERSIONDIFFREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.CreateAigcAppVersionDiffReq)
-  })
-_sym_db.RegisterMessage(CreateAigcAppVersionDiffReq)
-
-CreateAigcAppVersionDiffRes = _reflection.GeneratedProtocolMessageType('CreateAigcAppVersionDiffRes', (_message.Message,), {
-  'DESCRIPTOR' : _CREATEAIGCAPPVERSIONDIFFRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.CreateAigcAppVersionDiffRes)
-  })
-_sym_db.RegisterMessage(CreateAigcAppVersionDiffRes)
-
-AigcAppVersionDiff = _reflection.GeneratedProtocolMessageType('AigcAppVersionDiff', (_message.Message,), {
-  'DESCRIPTOR' : _AIGCAPPVERSIONDIFF,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AigcAppVersionDiff)
-  })
-_sym_db.RegisterMessage(AigcAppVersionDiff)
-
-MarketModelListReq = _reflection.GeneratedProtocolMessageType('MarketModelListReq', (_message.Message,), {
-  'DESCRIPTOR' : _MARKETMODELLISTREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.MarketModelListReq)
-  })
-_sym_db.RegisterMessage(MarketModelListReq)
-
-MarketModelListRes = _reflection.GeneratedProtocolMessageType('MarketModelListRes', (_message.Message,), {
-  'DESCRIPTOR' : _MARKETMODELLISTRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.MarketModelListRes)
-  })
-_sym_db.RegisterMessage(MarketModelListRes)
-
-MarketModelFieldEnumReq = _reflection.GeneratedProtocolMessageType('MarketModelFieldEnumReq', (_message.Message,), {
-  'DESCRIPTOR' : _MARKETMODELFIELDENUMREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.MarketModelFieldEnumReq)
-  })
-_sym_db.RegisterMessage(MarketModelFieldEnumReq)
-
-MarketModelFieldEnumRes = _reflection.GeneratedProtocolMessageType('MarketModelFieldEnumRes', (_message.Message,), {
-  'DESCRIPTOR' : _MARKETMODELFIELDENUMRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.MarketModelFieldEnumRes)
-  })
-_sym_db.RegisterMessage(MarketModelFieldEnumRes)
-
-MarketModelFieldItem = _reflection.GeneratedProtocolMessageType('MarketModelFieldItem', (_message.Message,), {
-  'DESCRIPTOR' : _MARKETMODELFIELDITEM,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.MarketModelFieldItem)
-  })
-_sym_db.RegisterMessage(MarketModelFieldItem)
-
-MarketModelDownloadReq = _reflection.GeneratedProtocolMessageType('MarketModelDownloadReq', (_message.Message,), {
-  'DESCRIPTOR' : _MARKETMODELDOWNLOADREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.MarketModelDownloadReq)
-  })
-_sym_db.RegisterMessage(MarketModelDownloadReq)
-
-MarketModelDownloadRes = _reflection.GeneratedProtocolMessageType('MarketModelDownloadRes', (_message.Message,), {
-  'DESCRIPTOR' : _MARKETMODELDOWNLOADRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.MarketModelDownloadRes)
-  })
-_sym_db.RegisterMessage(MarketModelDownloadRes)
-
-MarketModelCreateWithTaskReq = _reflection.GeneratedProtocolMessageType('MarketModelCreateWithTaskReq', (_message.Message,), {
-  'DESCRIPTOR' : _MARKETMODELCREATEWITHTASKREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.MarketModelCreateWithTaskReq)
-  })
-_sym_db.RegisterMessage(MarketModelCreateWithTaskReq)
-
-MarketModelCreateWithTaskRes = _reflection.GeneratedProtocolMessageType('MarketModelCreateWithTaskRes', (_message.Message,), {
-  'DESCRIPTOR' : _MARKETMODELCREATEWITHTASKRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.MarketModelCreateWithTaskRes)
-  })
-_sym_db.RegisterMessage(MarketModelCreateWithTaskRes)
-
-MarketPluginListReq = _reflection.GeneratedProtocolMessageType('MarketPluginListReq', (_message.Message,), {
-  'DESCRIPTOR' : _MARKETPLUGINLISTREQ,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.MarketPluginListReq)
-  })
-_sym_db.RegisterMessage(MarketPluginListReq)
-
-MarketPluginListRes = _reflection.GeneratedProtocolMessageType('MarketPluginListRes', (_message.Message,), {
-  'DESCRIPTOR' : _MARKETPLUGINLISTRES,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.MarketPluginListRes)
-  })
-_sym_db.RegisterMessage(MarketPluginListRes)
-
-MarketPluginItem = _reflection.GeneratedProtocolMessageType('MarketPluginItem', (_message.Message,), {
-  'DESCRIPTOR' : _MARKETPLUGINITEM,
-  '__module__' : 'aigc_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.MarketPluginItem)
-  })
-_sym_db.RegisterMessage(MarketPluginItem)
-
-_AIGCEXTOBJ = DESCRIPTOR.services_by_name['AigcExtObj']
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\242\002\003PB3'
-  _UPLOADWIDGETSTATUS._serialized_start=6361
-  _UPLOADWIDGETSTATUS._serialized_end=6449
-  _GROUPCONFIGTYPE._serialized_start=6451
-  _GROUPCONFIGTYPE._serialized_end=6506
-  _TASKITEM._serialized_start=40
-  _TASKITEM._serialized_end=114
-  _GETTASKREQ._serialized_start=116
-  _GETTASKREQ._serialized_end=227
-  _GETTASKRES._serialized_start=229
-  _GETTASKRES._serialized_end=299
-  _TASKNOTIFYREQ._serialized_start=301
-  _TASKNOTIFYREQ._serialized_end=421
-  _TASKNOTIFYRES._serialized_start=423
-  _TASKNOTIFYRES._serialized_end=438
-  _AIGCDEVICEBINDREQ._serialized_start=440
-  _AIGCDEVICEBINDREQ._serialized_end=551
-  _AIGCDEVICEBINDRES._serialized_start=553
-  _AIGCDEVICEBINDRES._serialized_end=572
-  _AIGCDEVICEUNBINDREQ._serialized_start=574
-  _AIGCDEVICEUNBINDREQ._serialized_end=616
-  _AIGCDEVICEUNBINDRES._serialized_start=618
-  _AIGCDEVICEUNBINDRES._serialized_end=639
-  _AIGCDEVICEINFOREQ._serialized_start=641
-  _AIGCDEVICEINFOREQ._serialized_end=712
-  _AIGCDEVICEINFORES._serialized_start=714
-  _AIGCDEVICEINFORES._serialized_end=810
-  _APPLYWIDGETREQ._serialized_start=812
-  _APPLYWIDGETREQ._serialized_end=828
-  _APPLYWIDGETRES._serialized_start=830
-  _APPLYWIDGETRES._serialized_end=866
-  _CREATEWIDGETREQ._serialized_start=868
-  _CREATEWIDGETREQ._serialized_end=885
-  _CREATEWIDGETRES._serialized_start=887
-  _CREATEWIDGETRES._serialized_end=924
-  _UPLOADWIDGETURLREQ._serialized_start=926
-  _UPLOADWIDGETURLREQ._serialized_end=983
-  _UPLOADWIDGETURLRES._serialized_start=985
-  _UPLOADWIDGETURLRES._serialized_end=1039
-  _UPLOADWIDGETREQ._serialized_start=1041
-  _UPLOADWIDGETREQ._serialized_end=1092
-  _UPLOADWIDGETRES._serialized_start=1094
-  _UPLOADWIDGETRES._serialized_end=1128
-  _UPLOADWIDGETCHECKREQ._serialized_start=1130
-  _UPLOADWIDGETCHECKREQ._serialized_end=1186
-  _UPLOADWIDGETCHECKRES._serialized_start=1188
-  _UPLOADWIDGETCHECKRES._serialized_end=1270
-  _AIGCCREATEGROUPREQ._serialized_start=1273
-  _AIGCCREATEGROUPREQ._serialized_end=1409
-  _AIGCCREATEGROUPRES._serialized_start=1411
-  _AIGCCREATEGROUPRES._serialized_end=1457
-  _AIGCREMOVEGROUPREQ._serialized_start=1459
-  _AIGCREMOVEGROUPREQ._serialized_end=1545
-  _AIGCREMOVEGROUPRES._serialized_start=1547
-  _AIGCREMOVEGROUPRES._serialized_end=1567
-  _AIGCTASKRESULT._serialized_start=1569
-  _AIGCTASKRESULT._serialized_end=1613
-  _AIGCDATA._serialized_start=1615
-  _AIGCDATA._serialized_end=1698
-  _AIGCDATAEXTENSION._serialized_start=1700
-  _AIGCDATAEXTENSION._serialized_end=1783
-  _UPLOADFILEURLREQ._serialized_start=1785
-  _UPLOADFILEURLREQ._serialized_end=1852
-  _UPLOADFILEURLRES._serialized_start=1854
-  _UPLOADFILEURLRES._serialized_end=1906
-  _AIGCDEVICEEXPANSIONREQ._serialized_start=1908
-  _AIGCDEVICEEXPANSIONREQ._serialized_end=1972
-  _AIGCDEVICEEXPANSIONRES._serialized_start=1974
-  _AIGCDEVICEEXPANSIONRES._serialized_end=2057
-  _TASKCOUNTITEM._serialized_start=2059
-  _TASKCOUNTITEM._serialized_end=2113
-  _TASKCOUNTREQ._serialized_start=2115
-  _TASKCOUNTREQ._serialized_end=2150
-  _TASKCOUNTRES._serialized_start=2152
-  _TASKCOUNTRES._serialized_end=2200
-  _AIGCWIDGETITEM._serialized_start=2202
-  _AIGCWIDGETITEM._serialized_end=2266
-  _AIGCWIDGETLISTREQ._serialized_start=2268
-  _AIGCWIDGETLISTREQ._serialized_end=2308
-  _AIGCWIDGETLISTRES._serialized_start=2310
-  _AIGCWIDGETLISTRES._serialized_end=2364
-  _DELETEAIGCWIDGETREQ._serialized_start=2366
-  _DELETEAIGCWIDGETREQ._serialized_end=2440
-  _DELETEAIGCWIDGETRES._serialized_start=2442
-  _DELETEAIGCWIDGETRES._serialized_end=2463
-  _AIGCWIDGETCONFIG._serialized_start=2465
-  _AIGCWIDGETCONFIG._serialized_end=2506
-  _AIGCWIDGETINFOREQ._serialized_start=2508
-  _AIGCWIDGETINFOREQ._serialized_end=2539
-  _AIGCWIDGETINFORES._serialized_start=2542
-  _AIGCWIDGETINFORES._serialized_end=2817
-  _AIGCBILLREPORTREQ._serialized_start=2819
-  _AIGCBILLREPORTREQ._serialized_end=2870
-  _AIGCBILLREPORTRES._serialized_start=2872
-  _AIGCBILLREPORTRES._serialized_end=2907
-  _AIGCTRAININGMODELREQ._serialized_start=2909
-  _AIGCTRAININGMODELREQ._serialized_end=2949
-  _AIGCTRAININGMODELRES._serialized_start=2951
-  _AIGCTRAININGMODELRES._serialized_end=2988
-  _AIGCENABLESERVERREQ._serialized_start=2990
-  _AIGCENABLESERVERREQ._serialized_end=3048
-  _AIGCENABLESERVERRES._serialized_start=3050
-  _AIGCENABLESERVERRES._serialized_end=3084
-  _ADDGROUPREQ._serialized_start=3086
-  _ADDGROUPREQ._serialized_end=3173
-  _ADDGROUPRES._serialized_start=3175
-  _ADDGROUPRES._serialized_end=3188
-  _AIGCGROUPINFOREQ._serialized_start=3190
-  _AIGCGROUPINFOREQ._serialized_end=3220
-  _AIGCGROUPINFORES._serialized_start=3223
-  _AIGCGROUPINFORES._serialized_end=3478
-  _AIGCGROUPCONFIG._serialized_start=3480
-  _AIGCGROUPCONFIG._serialized_end=3519
-  _GETGROUPDEVICEREQ._serialized_start=3521
-  _GETGROUPDEVICEREQ._serialized_end=3558
-  _GETGROUPDEVICERES._serialized_start=3560
-  _GETGROUPDEVICERES._serialized_end=3620
-  _AIGCDEVICEINFO._serialized_start=3623
-  _AIGCDEVICEINFO._serialized_end=3785
-  _DEVICEINFO._serialized_start=3787
-  _DEVICEINFO._serialized_end=3817
-  _EDITGROUPCONFIGREQ._serialized_start=3819
-  _EDITGROUPCONFIGREQ._serialized_end=3926
-  _EDITGROUPCONFIGRES._serialized_start=3928
-  _EDITGROUPCONFIGRES._serialized_end=3948
-  _GETDEVICEGROUPREQ._serialized_start=3950
-  _GETDEVICEGROUPREQ._serialized_end=4020
-  _GETDEVICEGROUPRES._serialized_start=4022
-  _GETDEVICEGROUPRES._serialized_end=4076
-  _AIGCDEVICEGROUP._serialized_start=4079
-  _AIGCDEVICEGROUP._serialized_end=4213
-  _AIGCWIDGET._serialized_start=4216
-  _AIGCWIDGET._serialized_end=4428
-  _AIGCOFFICIALMARKETMODELREQ._serialized_start=4430
-  _AIGCOFFICIALMARKETMODELREQ._serialized_end=4487
-  _AIGCOFFICIALMARKETMODELRES._serialized_start=4489
-  _AIGCOFFICIALMARKETMODELRES._serialized_end=4553
-  _AIGCMARKETMODEL._serialized_start=4556
-  _AIGCMARKETMODEL._serialized_end=4784
-  _AIGCTRAINMARKETMODELREQ._serialized_start=4786
-  _AIGCTRAINMARKETMODELREQ._serialized_end=4840
-  _AIGCTRAINMARKETMODELRES._serialized_start=4842
-  _AIGCTRAINMARKETMODELRES._serialized_end=4903
-  _AIGCAPPVERSIONLATESTREQ._serialized_start=4905
-  _AIGCAPPVERSIONLATESTREQ._serialized_end=4979
-  _AIGCAPPVERSIONLATESTRES._serialized_start=4981
-  _AIGCAPPVERSIONLATESTRES._serialized_end=5099
-  _CREATEAIGCAPPVERSIONREQ._serialized_start=5101
-  _CREATEAIGCAPPVERSIONREQ._serialized_end=5209
-  _CREATEAIGCAPPVERSIONRES._serialized_start=5211
-  _CREATEAIGCAPPVERSIONRES._serialized_end=5236
-  _CREATEAIGCAPPVERSIONDIFFREQ._serialized_start=5238
-  _CREATEAIGCAPPVERSIONDIFFREQ._serialized_end=5341
-  _CREATEAIGCAPPVERSIONDIFFRES._serialized_start=5343
-  _CREATEAIGCAPPVERSIONDIFFRES._serialized_end=5372
-  _AIGCAPPVERSIONDIFF._serialized_start=5374
-  _AIGCAPPVERSIONDIFF._serialized_end=5449
-  _MARKETMODELLISTREQ._serialized_start=5452
-  _MARKETMODELLISTREQ._serialized_end=5662
-  _MARKETMODELLISTRES._serialized_start=5664
-  _MARKETMODELLISTRES._serialized_end=5720
-  _MARKETMODELFIELDENUMREQ._serialized_start=5722
-  _MARKETMODELFIELDENUMREQ._serialized_end=5747
-  _MARKETMODELFIELDENUMRES._serialized_start=5750
-  _MARKETMODELFIELDENUMRES._serialized_end=5910
-  _MARKETMODELFIELDITEM._serialized_start=5912
-  _MARKETMODELFIELDITEM._serialized_end=5960
-  _MARKETMODELDOWNLOADREQ._serialized_start=5962
-  _MARKETMODELDOWNLOADREQ._serialized_end=5998
-  _MARKETMODELDOWNLOADRES._serialized_start=6000
-  _MARKETMODELDOWNLOADRES._serialized_end=6024
-  _MARKETMODELCREATEWITHTASKREQ._serialized_start=6026
-  _MARKETMODELCREATEWITHTASKREQ._serialized_end=6130
-  _MARKETMODELCREATEWITHTASKRES._serialized_start=6132
-  _MARKETMODELCREATEWITHTASKRES._serialized_end=6162
-  _MARKETPLUGINLISTREQ._serialized_start=6164
-  _MARKETPLUGINLISTREQ._serialized_end=6185
-  _MARKETPLUGINLISTRES._serialized_start=6187
-  _MARKETPLUGINLISTRES._serialized_end=6251
-  _MARKETPLUGINITEM._serialized_start=6253
-  _MARKETPLUGINITEM._serialized_end=6359
-  _AIGCEXTOBJ._serialized_start=6509
-  _AIGCEXTOBJ._serialized_end=8847
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: aigc_ext.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import enum_type_wrapper
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from mecord import common_ext_pb2 as common__ext__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x61igc_ext.proto\x12\x02pb\x1a\x10\x63ommon_ext.proto\"J\n\x08TaskItem\x12\x0e\n\x06taskId\x18\x01 \x01(\x03\x12\x10\n\x08taskUUID\x18\x02 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\t\"o\n\nGetTaskReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x11\n\tDeviceKey\x18\x02 \x01(\t\x12\x0f\n\x07widgets\x18\x03 \x03(\t\x12\r\n\x05token\x18\x04 \x01(\t\x12\r\n\x05limit\x18\x05 \x01(\x05\x12\x0e\n\x06\x65xtend\x18\x06 \x01(\t\"F\n\nGetTaskRes\x12\x1a\n\x04list\x18\x01 \x03(\x0b\x32\x0c.pb.TaskItem\x12\r\n\x05limit\x18\x02 \x01(\x05\x12\r\n\x05\x63ount\x18\x03 \x01(\x03\"x\n\rTaskNotifyReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08taskUUID\x18\x02 \x01(\t\x12\"\n\ntaskStatus\x18\x03 \x01(\x0e\x32\x0e.pb.TaskStatus\x12\x12\n\nfailReason\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\t\"\x0f\n\rTaskNotifyRes\"o\n\x11\x41igcDeviceBindReq\x12\x11\n\tdeviceKey\x18\x01 \x01(\t\x12\x11\n\tGroupUUID\x18\x02 \x01(\t\x12 \n\tLabelType\x18\x03 \x01(\x0e\x32\r.pb.LabelType\x12\x12\n\nlabelValue\x18\x04 \x01(\t\"\x13\n\x11\x41igcDeviceBindRes\"*\n\x13\x41igcDeviceUnBindReq\x12\x13\n\x0b\x64\x65viceToken\x18\x03 \x01(\t\"\x15\n\x13\x41igcDeviceUnBindRes\"G\n\x11\x41igcDeviceInfoReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x11\n\tdeviceKey\x18\x02 \x01(\t\x12\x0e\n\x06\x65xtend\x18\x03 \x01(\t\"`\n\x11\x41igcDeviceInfoRes\x12\x11\n\tdeviceKey\x18\x01 \x01(\t\x12\x11\n\tgroupUUID\x18\x02 \x01(\t\x12\x16\n\x0eisCreateWidget\x18\x03 \x01(\x08\x12\r\n\x05token\x18\x04 \x01(\t\"\x10\n\x0e\x41pplyWidgetReq\"$\n\x0e\x41pplyWidgetRes\x12\x12\n\nwidgetUUID\x18\x01 \x01(\t\"\x11\n\x0f\x43reateWidgetReq\"%\n\x0f\x43reateWidgetRes\x12\x12\n\nwidgetUUID\x18\x01 \x01(\t\"9\n\x12UploadWidgetUrlReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x12\n\nwidgetUUID\x18\x02 \x01(\t\"6\n\x12UploadWidgetUrlRes\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x63ontentType\x18\x02 \x01(\t\"3\n\x0fUploadWidgetReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x0f\n\x07\x66ileUrl\x18\x02 \x01(\t\"\"\n\x0fUploadWidgetRes\x12\x0f\n\x07\x63heckId\x18\x01 \x01(\x03\"8\n\x14UploadWidgetCheckReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x0f\n\x07\x63heckId\x18\x02 \x01(\x03\"R\n\x14UploadWidgetCheckRes\x12&\n\x06status\x18\x01 \x01(\x0e\x32\x16.pb.UploadWidgetStatus\x12\x12\n\nfailReason\x18\x02 \x01(\t\"\x88\x01\n\x12\x41igcCreateGroupReq\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12 \n\tlabelType\x18\x05 \x01(\x0e\x32\r.pb.LabelType\x12\x0f\n\x07labelId\x18\x06 \x01(\x03\x12\x0e\n\x06status\x18\x07 \x01(\x05\".\n\x12\x41igcCreateGroupRes\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04uuid\x18\x02 \x01(\t\"V\n\x12\x41igcRemoveGroupReq\x12\n\n\x02id\x18\x01 \x01(\x03\x12 \n\tlabelType\x18\x02 \x01(\x0e\x32\r.pb.LabelType\x12\x12\n\nlabelValue\x18\x03 \x01(\t\"\x14\n\x12\x41igcRemoveGroupRes\",\n\x0e\x41igcTaskResult\x12\x1a\n\x04list\x18\x01 \x03(\x0b\x32\x0c.pb.AigcData\"S\n\x08\x41igcData\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x02 \x03(\t\x12(\n\textension\x18\x03 \x01(\x0b\x32\x15.pb.AigcDataExtension\"S\n\x11\x41igcDataExtension\x12\x0c\n\x04info\x18\x01 \x01(\t\x12\x11\n\tcover_url\x18\x02 \x01(\t\x12\x0e\n\x06height\x18\x03 \x01(\x05\x12\r\n\x05width\x18\x04 \x01(\x05\"C\n\x10UploadFileUrlReq\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\x12\x0f\n\x07\x66ileExt\x18\x03 \x01(\t\"4\n\x10UploadFileUrlRes\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x63ontentType\x18\x02 \x01(\t\"@\n\x16\x41igcDeviceExpansionReq\x12\x13\n\x0b\x44\x65viceToken\x18\x01 \x01(\t\x12\x11\n\tDeviceKey\x18\x02 \x01(\t\"S\n\x16\x41igcDeviceExpansionRes\x12\x11\n\tdeviceKey\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65viceToken\x18\x02 \x01(\t\x12\x11\n\tgroupUUID\x18\x03 \x01(\t\"6\n\rTaskCountItem\x12\x12\n\nwidgetUUID\x18\x01 \x01(\t\x12\x11\n\ttaskCount\x18\x02 \x01(\x03\"#\n\x0cTaskCountReq\x12\x13\n\x0b\x64\x65viceToken\x18\x01 \x01(\t\"0\n\x0cTaskCountRes\x12 \n\x05items\x18\x01 \x03(\x0b\x32\x11.pb.TaskCountItem\"@\n\x0e\x41igcWidgetItem\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nupdated_at\x18\x03 \x01(\t\"(\n\x11\x41igcWidgetListReq\x12\x13\n\x0b\x64\x65viceToken\x18\x01 \x01(\t\"6\n\x11\x41igcWidgetListRes\x12!\n\x05items\x18\x01 \x03(\x0b\x32\x12.pb.AigcWidgetItem\"J\n\x13\x44\x65leteAigcWidgetReq\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x12\n\nwidgetUUID\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65viceToken\x18\x03 \x01(\t\"\x15\n\x13\x44\x65leteAigcWidgetRes\")\n\x10\x41igcWidgetConfig\x12\x15\n\rmaxTaskNumber\x18\x01 \x01(\x03\"\x1f\n\x11\x41igcWidgetInfoReq\x12\n\n\x02id\x18\x01 \x01(\x03\"\x93\x02\n\x11\x41igcWidgetInfoRes\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04icon\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0b\n\x03url\x18\x05 \x01(\t\x12$\n\x06\x63onfig\x18\x06 \x01(\x0b\x32\x14.pb.AigcWidgetConfig\x12\x19\n\x11\x63urrentTaskNumber\x18\x07 \x01(\x03\x12\x0e\n\x06status\x18\x08 \x01(\x05\x12\r\n\x05price\x18\t \x01(\x01\x12(\n\rcalculateMode\x18\n \x01(\x0e\x32\x11.pb.CalculateMode\x12\x14\n\x0c\x63urTaskCount\x18\x0b \x01(\x03\x12\x14\n\x0cmaxTaskCount\x18\x0c \x01(\x05\"3\n\x11\x41igcBillReportReq\x12\x0f\n\x07useTime\x18\x01 \x01(\x03\x12\r\n\x05isEnd\x18\x02 \x01(\x08\"#\n\x11\x41igcBillReportRes\x12\x0e\n\x06\x61mount\x18\x01 \x01(\x01\"(\n\x14\x41igcTrainingModelReq\x12\x10\n\x08widgetId\x18\x01 \x01(\x03\"%\n\x14\x41igcTrainingModelRes\x12\r\n\x05items\x18\x01 \x03(\t\":\n\x13\x41igcEnableServerReq\x12\x10\n\x08widgetId\x18\x01 \x01(\x03\x12\x11\n\tgroupUUID\x18\x02 \x01(\t\"\"\n\x13\x41igcEnableServerRes\x12\x0b\n\x03url\x18\x01 \x01(\t\"W\n\x0b\x41\x64\x64GroupReq\x12\x10\n\x08group_id\x18\x01 \x01(\x03\x12!\n\nlabel_type\x18\x02 \x01(\x0e\x32\r.pb.LabelType\x12\x13\n\x0blabel_value\x18\x03 \x01(\t\"\r\n\x0b\x41\x64\x64GroupRes\"\x1e\n\x10\x41igcGroupInfoReq\x12\n\n\x02id\x18\x01 \x01(\x03\"\xff\x01\n\x10\x41igcGroupInfoRes\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x0f\n\x07user_id\x18\x03 \x01(\x03\x12\x10\n\x08nickname\x18\x04 \x01(\t\x12\x12\n\nhead_image\x18\x05 \x01(\t\x12\x0e\n\x06status\x18\x06 \x01(\x05\x12\x12\n\ndevice_num\x18\x07 \x01(\x03\x12)\n\x0cgroup_config\x18\x08 \x01(\x0b\x32\x13.pb.AigcGroupConfig\x12\x19\n\x11total_compute_num\x18\t \x01(\x01\x12\x18\n\x10used_compute_num\x18\n \x01(\x01\x12\x16\n\x0eis_edit_config\x18\x0b \x01(\x08\"\'\n\x0f\x41igcGroupConfig\x12\x14\n\x0cshare_config\x18\x01 \x01(\x08\"%\n\x11GetGroupDeviceReq\x12\x10\n\x08group_id\x18\x01 \x01(\x03\"<\n\x11GetGroupDeviceRes\x12\'\n\x0b\x64\x65vice_list\x18\x01 \x03(\x0b\x32\x12.pb.AigcDeviceInfo\"\xa2\x01\n\x0e\x41igcDeviceInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0f\n\x07user_id\x18\x02 \x01(\x03\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x12\n\nhead_image\x18\x04 \x01(\t\x12\x15\n\rgenerated_num\x18\x05 \x01(\x03\x12\x11\n\tis_online\x18\x06 \x01(\x08\x12#\n\x0b\x64\x65vice_info\x18\x07 \x01(\x0b\x32\x0e.pb.DeviceInfo\"\x1e\n\nDeviceInfo\x12\x10\n\x08gpu_name\x18\x01 \x01(\t\"k\n\x12\x45\x64itGroupConfigReq\x12\x10\n\x08group_id\x18\x01 \x01(\x03\x12$\n\x07op_type\x18\x02 \x01(\x0e\x32\x13.pb.GroupConfigType\x12\x14\n\nedit_value\x18\x03 \x01(\x08H\x00\x42\x07\n\x05Param\"\x14\n\x12\x45\x64itGroupConfigRes\"F\n\x11GetDeviceGroupReq\x12 \n\tlabelType\x18\x01 \x01(\x0e\x32\r.pb.LabelType\x12\x0f\n\x07labelId\x18\x02 \x01(\x03\"6\n\x11GetDeviceGroupRes\x12!\n\x04list\x18\x02 \x03(\x0b\x32\x13.pb.AigcDeviceGroup\"\x86\x01\n\x0f\x41igcDeviceGroup\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04uuid\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04icon\x18\x04 \x01(\t\x12\"\n\nwidgetList\x18\x05 \x03(\x0b\x32\x0e.pb.AigcWidget\x12\x19\n\x11total_compute_num\x18\x06 \x01(\x03\"\xd4\x01\n\nAigcWidget\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04icon\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0b\n\x03url\x18\x05 \x01(\t\x12\x1c\n\x04type\x18\x06 \x01(\x0e\x32\x0e.pb.WidgetType\x12\x14\n\x0cmaxTaskCount\x18\x07 \x01(\x05\x12\r\n\x05price\x18\x08 \x01(\x01\x12(\n\rcalculateMode\x18\t \x01(\x0e\x32\x11.pb.CalculateMode\x12\x0f\n\x07groupId\x18\n \x01(\x03\"9\n\x1a\x41igcOfficialMarketModelReq\x12\r\n\x05Limit\x18\x01 \x01(\x05\x12\x0c\n\x04Type\x18\x02 \x01(\t\"@\n\x1a\x41igcOfficialMarketModelRes\x12\"\n\x05items\x18\x01 \x03(\x0b\x32\x13.pb.AigcMarketModel\"\xe4\x01\n\x0f\x41igcMarketModel\x12\n\n\x02Id\x18\x01 \x01(\x03\x12\x0c\n\x04UUID\x18\x02 \x01(\t\x12\x0c\n\x04Name\x18\x03 \x01(\t\x12\x0c\n\x04Type\x18\x04 \x01(\t\x12\x13\n\x0b\x44\x65scription\x18\x05 \x01(\t\x12\r\n\x05\x43over\x18\x06 \x01(\t\x12\x0b\n\x03URL\x18\x07 \x01(\t\x12\x0f\n\x07\x66ileExt\x18\x08 \x01(\t\x12\x10\n\x08\x66ileName\x18\t \x01(\t\x12\x0f\n\x07user_id\x18\n \x01(\x03\x12\x10\n\x08nickname\x18\x0b \x01(\t\x12\x12\n\nhead_image\x18\x0c \x01(\t\x12\x10\n\x08official\x18\r \x01(\x08\"6\n\x17\x41igcTrainMarketModelReq\x12\r\n\x05Limit\x18\x01 \x01(\x05\x12\x0c\n\x04Type\x18\x02 \x01(\t\"=\n\x17\x41igcTrainMarketModelRes\x12\"\n\x05items\x18\x01 \x03(\x0b\x32\x13.pb.AigcMarketModel\"J\n\x17\x41igcAppVersionLatestReq\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08platform\x18\x03 \x01(\t\"v\n\x17\x41igcAppVersionLatestRes\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12(\n\x08\x64iffInfo\x18\x04 \x01(\x0b\x32\x16.pb.AigcAppVersionDiff\"l\n\x17\x43reateAigcAppVersionReq\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x10\n\x08platform\x18\x05 \x01(\t\"\x19\n\x17\x43reateAigcAppVersionRes\"g\n\x1b\x43reateAigcAppVersionDiffReq\x12\x0c\n\x04name\x18\x01 \x01(\t\x12(\n\x08\x64iffList\x18\x02 \x03(\x0b\x32\x16.pb.AigcAppVersionDiff\x12\x10\n\x08platform\x18\x03 \x01(\t\"\x1d\n\x1b\x43reateAigcAppVersionDiffRes\"K\n\x12\x41igcAppVersionDiff\x12\x14\n\x0cstartVersion\x18\x01 \x01(\t\x12\x12\n\nendVersion\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\"\xd2\x01\n\x12MarketModelListReq\x12\x0c\n\x04self\x18\x01 \x01(\x08\x12\x11\n\tsort_type\x18\x02 \x01(\x05\x12\x12\n\nmodel_type\x18\x03 \x03(\x03\x12\x11\n\tattribute\x18\x04 \x03(\x03\x12\x10\n\x08\x63\x61tegory\x18\x05 \x03(\x03\x12\x16\n\x0esearch_keyword\x18\x06 \x01(\t\x12\x0c\n\x04page\x18\x07 \x01(\x03\x12\x0c\n\x04size\x18\x08 \x01(\x03\x12\x17\n\x0fupdateStartTime\x18\t \x01(\t\x12\x15\n\rupdateEndTime\x18\n \x01(\t\"8\n\x12MarketModelListRes\x12\"\n\x05items\x18\x01 \x03(\x0b\x32\x13.pb.AigcMarketModel\"\x19\n\x17MarketModelFieldEnumReq\"\xa0\x01\n\x17MarketModelFieldEnumRes\x12,\n\nmodel_type\x18\x01 \x03(\x0b\x32\x18.pb.MarketModelFieldItem\x12+\n\tattribute\x18\x02 \x03(\x0b\x32\x18.pb.MarketModelFieldItem\x12*\n\x08\x63\x61tegory\x18\x03 \x03(\x0b\x32\x18.pb.MarketModelFieldItem\"0\n\x14MarketModelFieldItem\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\"$\n\x16MarketModelDownloadReq\x12\n\n\x02Id\x18\x01 \x01(\x03\"\x18\n\x16MarketModelDownloadRes\"h\n\x1cMarketModelCreateWithTaskReq\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x63over\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x10\n\x08TaskUUID\x18\x05 \x01(\t\"\x1e\n\x1cMarketModelCreateWithTaskRes\"\x15\n\x13MarketPluginListReq\"@\n\x13MarketPluginListRes\x12)\n\x0bplugin_list\x18\x01 \x03(\x0b\x32\x14.pb.MarketPluginItem\"j\n\x10MarketPluginItem\x12\n\n\x02Id\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0b\n\x03url\x18\x05 \x01(\t\x12\x0c\n\x04tags\x18\x06 \x03(\t*X\n\x12UploadWidgetStatus\x12\x0c\n\x08UWS_NONE\x10\x00\x12\x12\n\x0eUWS_PROCESSING\x10\x01\x12\x0f\n\x0bUWS_SUCCESS\x10\x02\x12\x0f\n\x0bUWS_FAILURE\x10\x03*7\n\x0fGroupConfigType\x12\x0f\n\x0bGCT_Unknown\x10\x00\x12\x13\n\x0fGCT_ShareConfig\x10\x01\x32\xa2\x12\n\nAigcExtObj\x12)\n\x07GetTask\x12\x0e.pb.GetTaskReq\x1a\x0e.pb.GetTaskRes\x12\x32\n\nTaskNotify\x12\x11.pb.TaskNotifyReq\x1a\x11.pb.TaskNotifyRes\x12/\n\tTaskCount\x12\x10.pb.TaskCountReq\x1a\x10.pb.TaskCountRes\x12:\n\nDeviceBind\x12\x15.pb.AigcDeviceBindReq\x1a\x15.pb.AigcDeviceBindRes\x12@\n\x0c\x44\x65viceUnBind\x12\x17.pb.AigcDeviceUnBindReq\x1a\x17.pb.AigcDeviceUnBindRes\x12:\n\nDeviceInfo\x12\x15.pb.AigcDeviceInfoReq\x1a\x15.pb.AigcDeviceInfoRes\x12I\n\x0f\x44\x65viceExpansion\x12\x1a.pb.AigcDeviceExpansionReq\x1a\x1a.pb.AigcDeviceExpansionRes\x12\x35\n\x0b\x41pplyWidget\x12\x12.pb.ApplyWidgetReq\x1a\x12.pb.ApplyWidgetRes\x12\x38\n\x0c\x43reateWidget\x12\x13.pb.CreateWidgetReq\x1a\x13.pb.CreateWidgetRes\x12@\n\x0c\x44\x65leteWidget\x12\x17.pb.DeleteAigcWidgetReq\x1a\x17.pb.DeleteAigcWidgetRes\x12:\n\nWidgetList\x12\x15.pb.AigcWidgetListReq\x1a\x15.pb.AigcWidgetListRes\x12:\n\nWidgetInfo\x12\x15.pb.AigcWidgetInfoReq\x1a\x15.pb.AigcWidgetInfoRes\x12\x38\n\x0cUploadWidget\x12\x13.pb.UploadWidgetReq\x1a\x13.pb.UploadWidgetRes\x12\x41\n\x0fUploadWidgetUrl\x12\x16.pb.UploadWidgetUrlReq\x1a\x16.pb.UploadWidgetUrlRes\x12;\n\rUploadFileUrl\x12\x14.pb.UploadFileUrlReq\x1a\x14.pb.UploadFileUrlRes\x12G\n\x11UploadWidgetCheck\x12\x18.pb.UploadWidgetCheckReq\x1a\x18.pb.UploadWidgetCheckRes\x12=\n\x0bRemoveGroup\x12\x16.pb.AigcRemoveGroupReq\x1a\x16.pb.AigcRemoveGroupRes\x12:\n\nBillReport\x12\x15.pb.AigcBillReportReq\x1a\x15.pb.AigcBillReportRes\x12\x43\n\rTrainingModel\x12\x18.pb.AigcTrainingModelReq\x1a\x18.pb.AigcTrainingModelRes\x12@\n\x0c\x45nableServer\x12\x17.pb.AigcEnableServerReq\x1a\x17.pb.AigcEnableServerRes\x12,\n\x08\x41\x64\x64Group\x12\x0f.pb.AddGroupReq\x1a\x0f.pb.AddGroupRes\x12:\n\x0cGetGroupInfo\x12\x14.pb.AigcGroupInfoReq\x1a\x14.pb.AigcGroupInfoRes\x12>\n\x0eGetGroupDevice\x12\x15.pb.GetGroupDeviceReq\x1a\x15.pb.GetGroupDeviceRes\x12\x41\n\x0f\x45\x64itGroupConfig\x12\x16.pb.EditGroupConfigReq\x1a\x16.pb.EditGroupConfigRes\x12<\n\x0cGetGroupList\x12\x15.pb.GetDeviceGroupReq\x1a\x15.pb.GetDeviceGroupRes\x12U\n\x13OfficialMarketModel\x12\x1e.pb.AigcOfficialMarketModelReq\x1a\x1e.pb.AigcOfficialMarketModelRes\x12L\n\x10TrainMarketModel\x12\x1b.pb.AigcTrainMarketModelReq\x1a\x1b.pb.AigcTrainMarketModelRes\x12L\n\x10\x41ppVersionLatest\x12\x1b.pb.AigcAppVersionLatestReq\x1a\x1b.pb.AigcAppVersionLatestRes\x12L\n\x10\x43reateAppVersion\x12\x1b.pb.CreateAigcAppVersionReq\x1a\x1b.pb.CreateAigcAppVersionRes\x12X\n\x14\x43reateAppVersionDiff\x12\x1f.pb.CreateAigcAppVersionDiffReq\x1a\x1f.pb.CreateAigcAppVersionDiffRes\x12\x41\n\x0fMarketModelList\x12\x16.pb.MarketModelListReq\x1a\x16.pb.MarketModelListRes\x12P\n\x14MarketModelFieldEnum\x12\x1b.pb.MarketModelFieldEnumReq\x1a\x1b.pb.MarketModelFieldEnumRes\x12M\n\x13MarketModelDownload\x12\x1a.pb.MarketModelDownloadReq\x1a\x1a.pb.MarketModelDownloadRes\x12_\n\x19MarketModelCreateWithTask\x12 .pb.MarketModelCreateWithTaskReq\x1a .pb.MarketModelCreateWithTaskRes\x12\x44\n\x10MarketPluginList\x12\x17.pb.MarketPluginListReq\x1a\x17.pb.MarketPluginListResB\x06\xa2\x02\x03PB3b\x06proto3')
+
+_UPLOADWIDGETSTATUS = DESCRIPTOR.enum_types_by_name['UploadWidgetStatus']
+UploadWidgetStatus = enum_type_wrapper.EnumTypeWrapper(_UPLOADWIDGETSTATUS)
+_GROUPCONFIGTYPE = DESCRIPTOR.enum_types_by_name['GroupConfigType']
+GroupConfigType = enum_type_wrapper.EnumTypeWrapper(_GROUPCONFIGTYPE)
+UWS_NONE = 0
+UWS_PROCESSING = 1
+UWS_SUCCESS = 2
+UWS_FAILURE = 3
+GCT_Unknown = 0
+GCT_ShareConfig = 1
+
+
+_TASKITEM = DESCRIPTOR.message_types_by_name['TaskItem']
+_GETTASKREQ = DESCRIPTOR.message_types_by_name['GetTaskReq']
+_GETTASKRES = DESCRIPTOR.message_types_by_name['GetTaskRes']
+_TASKNOTIFYREQ = DESCRIPTOR.message_types_by_name['TaskNotifyReq']
+_TASKNOTIFYRES = DESCRIPTOR.message_types_by_name['TaskNotifyRes']
+_AIGCDEVICEBINDREQ = DESCRIPTOR.message_types_by_name['AigcDeviceBindReq']
+_AIGCDEVICEBINDRES = DESCRIPTOR.message_types_by_name['AigcDeviceBindRes']
+_AIGCDEVICEUNBINDREQ = DESCRIPTOR.message_types_by_name['AigcDeviceUnBindReq']
+_AIGCDEVICEUNBINDRES = DESCRIPTOR.message_types_by_name['AigcDeviceUnBindRes']
+_AIGCDEVICEINFOREQ = DESCRIPTOR.message_types_by_name['AigcDeviceInfoReq']
+_AIGCDEVICEINFORES = DESCRIPTOR.message_types_by_name['AigcDeviceInfoRes']
+_APPLYWIDGETREQ = DESCRIPTOR.message_types_by_name['ApplyWidgetReq']
+_APPLYWIDGETRES = DESCRIPTOR.message_types_by_name['ApplyWidgetRes']
+_CREATEWIDGETREQ = DESCRIPTOR.message_types_by_name['CreateWidgetReq']
+_CREATEWIDGETRES = DESCRIPTOR.message_types_by_name['CreateWidgetRes']
+_UPLOADWIDGETURLREQ = DESCRIPTOR.message_types_by_name['UploadWidgetUrlReq']
+_UPLOADWIDGETURLRES = DESCRIPTOR.message_types_by_name['UploadWidgetUrlRes']
+_UPLOADWIDGETREQ = DESCRIPTOR.message_types_by_name['UploadWidgetReq']
+_UPLOADWIDGETRES = DESCRIPTOR.message_types_by_name['UploadWidgetRes']
+_UPLOADWIDGETCHECKREQ = DESCRIPTOR.message_types_by_name['UploadWidgetCheckReq']
+_UPLOADWIDGETCHECKRES = DESCRIPTOR.message_types_by_name['UploadWidgetCheckRes']
+_AIGCCREATEGROUPREQ = DESCRIPTOR.message_types_by_name['AigcCreateGroupReq']
+_AIGCCREATEGROUPRES = DESCRIPTOR.message_types_by_name['AigcCreateGroupRes']
+_AIGCREMOVEGROUPREQ = DESCRIPTOR.message_types_by_name['AigcRemoveGroupReq']
+_AIGCREMOVEGROUPRES = DESCRIPTOR.message_types_by_name['AigcRemoveGroupRes']
+_AIGCTASKRESULT = DESCRIPTOR.message_types_by_name['AigcTaskResult']
+_AIGCDATA = DESCRIPTOR.message_types_by_name['AigcData']
+_AIGCDATAEXTENSION = DESCRIPTOR.message_types_by_name['AigcDataExtension']
+_UPLOADFILEURLREQ = DESCRIPTOR.message_types_by_name['UploadFileUrlReq']
+_UPLOADFILEURLRES = DESCRIPTOR.message_types_by_name['UploadFileUrlRes']
+_AIGCDEVICEEXPANSIONREQ = DESCRIPTOR.message_types_by_name['AigcDeviceExpansionReq']
+_AIGCDEVICEEXPANSIONRES = DESCRIPTOR.message_types_by_name['AigcDeviceExpansionRes']
+_TASKCOUNTITEM = DESCRIPTOR.message_types_by_name['TaskCountItem']
+_TASKCOUNTREQ = DESCRIPTOR.message_types_by_name['TaskCountReq']
+_TASKCOUNTRES = DESCRIPTOR.message_types_by_name['TaskCountRes']
+_AIGCWIDGETITEM = DESCRIPTOR.message_types_by_name['AigcWidgetItem']
+_AIGCWIDGETLISTREQ = DESCRIPTOR.message_types_by_name['AigcWidgetListReq']
+_AIGCWIDGETLISTRES = DESCRIPTOR.message_types_by_name['AigcWidgetListRes']
+_DELETEAIGCWIDGETREQ = DESCRIPTOR.message_types_by_name['DeleteAigcWidgetReq']
+_DELETEAIGCWIDGETRES = DESCRIPTOR.message_types_by_name['DeleteAigcWidgetRes']
+_AIGCWIDGETCONFIG = DESCRIPTOR.message_types_by_name['AigcWidgetConfig']
+_AIGCWIDGETINFOREQ = DESCRIPTOR.message_types_by_name['AigcWidgetInfoReq']
+_AIGCWIDGETINFORES = DESCRIPTOR.message_types_by_name['AigcWidgetInfoRes']
+_AIGCBILLREPORTREQ = DESCRIPTOR.message_types_by_name['AigcBillReportReq']
+_AIGCBILLREPORTRES = DESCRIPTOR.message_types_by_name['AigcBillReportRes']
+_AIGCTRAININGMODELREQ = DESCRIPTOR.message_types_by_name['AigcTrainingModelReq']
+_AIGCTRAININGMODELRES = DESCRIPTOR.message_types_by_name['AigcTrainingModelRes']
+_AIGCENABLESERVERREQ = DESCRIPTOR.message_types_by_name['AigcEnableServerReq']
+_AIGCENABLESERVERRES = DESCRIPTOR.message_types_by_name['AigcEnableServerRes']
+_ADDGROUPREQ = DESCRIPTOR.message_types_by_name['AddGroupReq']
+_ADDGROUPRES = DESCRIPTOR.message_types_by_name['AddGroupRes']
+_AIGCGROUPINFOREQ = DESCRIPTOR.message_types_by_name['AigcGroupInfoReq']
+_AIGCGROUPINFORES = DESCRIPTOR.message_types_by_name['AigcGroupInfoRes']
+_AIGCGROUPCONFIG = DESCRIPTOR.message_types_by_name['AigcGroupConfig']
+_GETGROUPDEVICEREQ = DESCRIPTOR.message_types_by_name['GetGroupDeviceReq']
+_GETGROUPDEVICERES = DESCRIPTOR.message_types_by_name['GetGroupDeviceRes']
+_AIGCDEVICEINFO = DESCRIPTOR.message_types_by_name['AigcDeviceInfo']
+_DEVICEINFO = DESCRIPTOR.message_types_by_name['DeviceInfo']
+_EDITGROUPCONFIGREQ = DESCRIPTOR.message_types_by_name['EditGroupConfigReq']
+_EDITGROUPCONFIGRES = DESCRIPTOR.message_types_by_name['EditGroupConfigRes']
+_GETDEVICEGROUPREQ = DESCRIPTOR.message_types_by_name['GetDeviceGroupReq']
+_GETDEVICEGROUPRES = DESCRIPTOR.message_types_by_name['GetDeviceGroupRes']
+_AIGCDEVICEGROUP = DESCRIPTOR.message_types_by_name['AigcDeviceGroup']
+_AIGCWIDGET = DESCRIPTOR.message_types_by_name['AigcWidget']
+_AIGCOFFICIALMARKETMODELREQ = DESCRIPTOR.message_types_by_name['AigcOfficialMarketModelReq']
+_AIGCOFFICIALMARKETMODELRES = DESCRIPTOR.message_types_by_name['AigcOfficialMarketModelRes']
+_AIGCMARKETMODEL = DESCRIPTOR.message_types_by_name['AigcMarketModel']
+_AIGCTRAINMARKETMODELREQ = DESCRIPTOR.message_types_by_name['AigcTrainMarketModelReq']
+_AIGCTRAINMARKETMODELRES = DESCRIPTOR.message_types_by_name['AigcTrainMarketModelRes']
+_AIGCAPPVERSIONLATESTREQ = DESCRIPTOR.message_types_by_name['AigcAppVersionLatestReq']
+_AIGCAPPVERSIONLATESTRES = DESCRIPTOR.message_types_by_name['AigcAppVersionLatestRes']
+_CREATEAIGCAPPVERSIONREQ = DESCRIPTOR.message_types_by_name['CreateAigcAppVersionReq']
+_CREATEAIGCAPPVERSIONRES = DESCRIPTOR.message_types_by_name['CreateAigcAppVersionRes']
+_CREATEAIGCAPPVERSIONDIFFREQ = DESCRIPTOR.message_types_by_name['CreateAigcAppVersionDiffReq']
+_CREATEAIGCAPPVERSIONDIFFRES = DESCRIPTOR.message_types_by_name['CreateAigcAppVersionDiffRes']
+_AIGCAPPVERSIONDIFF = DESCRIPTOR.message_types_by_name['AigcAppVersionDiff']
+_MARKETMODELLISTREQ = DESCRIPTOR.message_types_by_name['MarketModelListReq']
+_MARKETMODELLISTRES = DESCRIPTOR.message_types_by_name['MarketModelListRes']
+_MARKETMODELFIELDENUMREQ = DESCRIPTOR.message_types_by_name['MarketModelFieldEnumReq']
+_MARKETMODELFIELDENUMRES = DESCRIPTOR.message_types_by_name['MarketModelFieldEnumRes']
+_MARKETMODELFIELDITEM = DESCRIPTOR.message_types_by_name['MarketModelFieldItem']
+_MARKETMODELDOWNLOADREQ = DESCRIPTOR.message_types_by_name['MarketModelDownloadReq']
+_MARKETMODELDOWNLOADRES = DESCRIPTOR.message_types_by_name['MarketModelDownloadRes']
+_MARKETMODELCREATEWITHTASKREQ = DESCRIPTOR.message_types_by_name['MarketModelCreateWithTaskReq']
+_MARKETMODELCREATEWITHTASKRES = DESCRIPTOR.message_types_by_name['MarketModelCreateWithTaskRes']
+_MARKETPLUGINLISTREQ = DESCRIPTOR.message_types_by_name['MarketPluginListReq']
+_MARKETPLUGINLISTRES = DESCRIPTOR.message_types_by_name['MarketPluginListRes']
+_MARKETPLUGINITEM = DESCRIPTOR.message_types_by_name['MarketPluginItem']
+TaskItem = _reflection.GeneratedProtocolMessageType('TaskItem', (_message.Message,), {
+  'DESCRIPTOR' : _TASKITEM,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.TaskItem)
+  })
+_sym_db.RegisterMessage(TaskItem)
+
+GetTaskReq = _reflection.GeneratedProtocolMessageType('GetTaskReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETTASKREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.GetTaskReq)
+  })
+_sym_db.RegisterMessage(GetTaskReq)
+
+GetTaskRes = _reflection.GeneratedProtocolMessageType('GetTaskRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETTASKRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.GetTaskRes)
+  })
+_sym_db.RegisterMessage(GetTaskRes)
+
+TaskNotifyReq = _reflection.GeneratedProtocolMessageType('TaskNotifyReq', (_message.Message,), {
+  'DESCRIPTOR' : _TASKNOTIFYREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.TaskNotifyReq)
+  })
+_sym_db.RegisterMessage(TaskNotifyReq)
+
+TaskNotifyRes = _reflection.GeneratedProtocolMessageType('TaskNotifyRes', (_message.Message,), {
+  'DESCRIPTOR' : _TASKNOTIFYRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.TaskNotifyRes)
+  })
+_sym_db.RegisterMessage(TaskNotifyRes)
+
+AigcDeviceBindReq = _reflection.GeneratedProtocolMessageType('AigcDeviceBindReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCDEVICEBINDREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcDeviceBindReq)
+  })
+_sym_db.RegisterMessage(AigcDeviceBindReq)
+
+AigcDeviceBindRes = _reflection.GeneratedProtocolMessageType('AigcDeviceBindRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCDEVICEBINDRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcDeviceBindRes)
+  })
+_sym_db.RegisterMessage(AigcDeviceBindRes)
+
+AigcDeviceUnBindReq = _reflection.GeneratedProtocolMessageType('AigcDeviceUnBindReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCDEVICEUNBINDREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcDeviceUnBindReq)
+  })
+_sym_db.RegisterMessage(AigcDeviceUnBindReq)
+
+AigcDeviceUnBindRes = _reflection.GeneratedProtocolMessageType('AigcDeviceUnBindRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCDEVICEUNBINDRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcDeviceUnBindRes)
+  })
+_sym_db.RegisterMessage(AigcDeviceUnBindRes)
+
+AigcDeviceInfoReq = _reflection.GeneratedProtocolMessageType('AigcDeviceInfoReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCDEVICEINFOREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcDeviceInfoReq)
+  })
+_sym_db.RegisterMessage(AigcDeviceInfoReq)
+
+AigcDeviceInfoRes = _reflection.GeneratedProtocolMessageType('AigcDeviceInfoRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCDEVICEINFORES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcDeviceInfoRes)
+  })
+_sym_db.RegisterMessage(AigcDeviceInfoRes)
+
+ApplyWidgetReq = _reflection.GeneratedProtocolMessageType('ApplyWidgetReq', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYWIDGETREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.ApplyWidgetReq)
+  })
+_sym_db.RegisterMessage(ApplyWidgetReq)
+
+ApplyWidgetRes = _reflection.GeneratedProtocolMessageType('ApplyWidgetRes', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYWIDGETRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.ApplyWidgetRes)
+  })
+_sym_db.RegisterMessage(ApplyWidgetRes)
+
+CreateWidgetReq = _reflection.GeneratedProtocolMessageType('CreateWidgetReq', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEWIDGETREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.CreateWidgetReq)
+  })
+_sym_db.RegisterMessage(CreateWidgetReq)
+
+CreateWidgetRes = _reflection.GeneratedProtocolMessageType('CreateWidgetRes', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEWIDGETRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.CreateWidgetRes)
+  })
+_sym_db.RegisterMessage(CreateWidgetRes)
+
+UploadWidgetUrlReq = _reflection.GeneratedProtocolMessageType('UploadWidgetUrlReq', (_message.Message,), {
+  'DESCRIPTOR' : _UPLOADWIDGETURLREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UploadWidgetUrlReq)
+  })
+_sym_db.RegisterMessage(UploadWidgetUrlReq)
+
+UploadWidgetUrlRes = _reflection.GeneratedProtocolMessageType('UploadWidgetUrlRes', (_message.Message,), {
+  'DESCRIPTOR' : _UPLOADWIDGETURLRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UploadWidgetUrlRes)
+  })
+_sym_db.RegisterMessage(UploadWidgetUrlRes)
+
+UploadWidgetReq = _reflection.GeneratedProtocolMessageType('UploadWidgetReq', (_message.Message,), {
+  'DESCRIPTOR' : _UPLOADWIDGETREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UploadWidgetReq)
+  })
+_sym_db.RegisterMessage(UploadWidgetReq)
+
+UploadWidgetRes = _reflection.GeneratedProtocolMessageType('UploadWidgetRes', (_message.Message,), {
+  'DESCRIPTOR' : _UPLOADWIDGETRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UploadWidgetRes)
+  })
+_sym_db.RegisterMessage(UploadWidgetRes)
+
+UploadWidgetCheckReq = _reflection.GeneratedProtocolMessageType('UploadWidgetCheckReq', (_message.Message,), {
+  'DESCRIPTOR' : _UPLOADWIDGETCHECKREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UploadWidgetCheckReq)
+  })
+_sym_db.RegisterMessage(UploadWidgetCheckReq)
+
+UploadWidgetCheckRes = _reflection.GeneratedProtocolMessageType('UploadWidgetCheckRes', (_message.Message,), {
+  'DESCRIPTOR' : _UPLOADWIDGETCHECKRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UploadWidgetCheckRes)
+  })
+_sym_db.RegisterMessage(UploadWidgetCheckRes)
+
+AigcCreateGroupReq = _reflection.GeneratedProtocolMessageType('AigcCreateGroupReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCCREATEGROUPREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcCreateGroupReq)
+  })
+_sym_db.RegisterMessage(AigcCreateGroupReq)
+
+AigcCreateGroupRes = _reflection.GeneratedProtocolMessageType('AigcCreateGroupRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCCREATEGROUPRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcCreateGroupRes)
+  })
+_sym_db.RegisterMessage(AigcCreateGroupRes)
+
+AigcRemoveGroupReq = _reflection.GeneratedProtocolMessageType('AigcRemoveGroupReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCREMOVEGROUPREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcRemoveGroupReq)
+  })
+_sym_db.RegisterMessage(AigcRemoveGroupReq)
+
+AigcRemoveGroupRes = _reflection.GeneratedProtocolMessageType('AigcRemoveGroupRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCREMOVEGROUPRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcRemoveGroupRes)
+  })
+_sym_db.RegisterMessage(AigcRemoveGroupRes)
+
+AigcTaskResult = _reflection.GeneratedProtocolMessageType('AigcTaskResult', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCTASKRESULT,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcTaskResult)
+  })
+_sym_db.RegisterMessage(AigcTaskResult)
+
+AigcData = _reflection.GeneratedProtocolMessageType('AigcData', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCDATA,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcData)
+  })
+_sym_db.RegisterMessage(AigcData)
+
+AigcDataExtension = _reflection.GeneratedProtocolMessageType('AigcDataExtension', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCDATAEXTENSION,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcDataExtension)
+  })
+_sym_db.RegisterMessage(AigcDataExtension)
+
+UploadFileUrlReq = _reflection.GeneratedProtocolMessageType('UploadFileUrlReq', (_message.Message,), {
+  'DESCRIPTOR' : _UPLOADFILEURLREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UploadFileUrlReq)
+  })
+_sym_db.RegisterMessage(UploadFileUrlReq)
+
+UploadFileUrlRes = _reflection.GeneratedProtocolMessageType('UploadFileUrlRes', (_message.Message,), {
+  'DESCRIPTOR' : _UPLOADFILEURLRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UploadFileUrlRes)
+  })
+_sym_db.RegisterMessage(UploadFileUrlRes)
+
+AigcDeviceExpansionReq = _reflection.GeneratedProtocolMessageType('AigcDeviceExpansionReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCDEVICEEXPANSIONREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcDeviceExpansionReq)
+  })
+_sym_db.RegisterMessage(AigcDeviceExpansionReq)
+
+AigcDeviceExpansionRes = _reflection.GeneratedProtocolMessageType('AigcDeviceExpansionRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCDEVICEEXPANSIONRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcDeviceExpansionRes)
+  })
+_sym_db.RegisterMessage(AigcDeviceExpansionRes)
+
+TaskCountItem = _reflection.GeneratedProtocolMessageType('TaskCountItem', (_message.Message,), {
+  'DESCRIPTOR' : _TASKCOUNTITEM,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.TaskCountItem)
+  })
+_sym_db.RegisterMessage(TaskCountItem)
+
+TaskCountReq = _reflection.GeneratedProtocolMessageType('TaskCountReq', (_message.Message,), {
+  'DESCRIPTOR' : _TASKCOUNTREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.TaskCountReq)
+  })
+_sym_db.RegisterMessage(TaskCountReq)
+
+TaskCountRes = _reflection.GeneratedProtocolMessageType('TaskCountRes', (_message.Message,), {
+  'DESCRIPTOR' : _TASKCOUNTRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.TaskCountRes)
+  })
+_sym_db.RegisterMessage(TaskCountRes)
+
+AigcWidgetItem = _reflection.GeneratedProtocolMessageType('AigcWidgetItem', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCWIDGETITEM,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcWidgetItem)
+  })
+_sym_db.RegisterMessage(AigcWidgetItem)
+
+AigcWidgetListReq = _reflection.GeneratedProtocolMessageType('AigcWidgetListReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCWIDGETLISTREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcWidgetListReq)
+  })
+_sym_db.RegisterMessage(AigcWidgetListReq)
+
+AigcWidgetListRes = _reflection.GeneratedProtocolMessageType('AigcWidgetListRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCWIDGETLISTRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcWidgetListRes)
+  })
+_sym_db.RegisterMessage(AigcWidgetListRes)
+
+DeleteAigcWidgetReq = _reflection.GeneratedProtocolMessageType('DeleteAigcWidgetReq', (_message.Message,), {
+  'DESCRIPTOR' : _DELETEAIGCWIDGETREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.DeleteAigcWidgetReq)
+  })
+_sym_db.RegisterMessage(DeleteAigcWidgetReq)
+
+DeleteAigcWidgetRes = _reflection.GeneratedProtocolMessageType('DeleteAigcWidgetRes', (_message.Message,), {
+  'DESCRIPTOR' : _DELETEAIGCWIDGETRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.DeleteAigcWidgetRes)
+  })
+_sym_db.RegisterMessage(DeleteAigcWidgetRes)
+
+AigcWidgetConfig = _reflection.GeneratedProtocolMessageType('AigcWidgetConfig', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCWIDGETCONFIG,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcWidgetConfig)
+  })
+_sym_db.RegisterMessage(AigcWidgetConfig)
+
+AigcWidgetInfoReq = _reflection.GeneratedProtocolMessageType('AigcWidgetInfoReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCWIDGETINFOREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcWidgetInfoReq)
+  })
+_sym_db.RegisterMessage(AigcWidgetInfoReq)
+
+AigcWidgetInfoRes = _reflection.GeneratedProtocolMessageType('AigcWidgetInfoRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCWIDGETINFORES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcWidgetInfoRes)
+  })
+_sym_db.RegisterMessage(AigcWidgetInfoRes)
+
+AigcBillReportReq = _reflection.GeneratedProtocolMessageType('AigcBillReportReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCBILLREPORTREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcBillReportReq)
+  })
+_sym_db.RegisterMessage(AigcBillReportReq)
+
+AigcBillReportRes = _reflection.GeneratedProtocolMessageType('AigcBillReportRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCBILLREPORTRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcBillReportRes)
+  })
+_sym_db.RegisterMessage(AigcBillReportRes)
+
+AigcTrainingModelReq = _reflection.GeneratedProtocolMessageType('AigcTrainingModelReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCTRAININGMODELREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcTrainingModelReq)
+  })
+_sym_db.RegisterMessage(AigcTrainingModelReq)
+
+AigcTrainingModelRes = _reflection.GeneratedProtocolMessageType('AigcTrainingModelRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCTRAININGMODELRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcTrainingModelRes)
+  })
+_sym_db.RegisterMessage(AigcTrainingModelRes)
+
+AigcEnableServerReq = _reflection.GeneratedProtocolMessageType('AigcEnableServerReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCENABLESERVERREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcEnableServerReq)
+  })
+_sym_db.RegisterMessage(AigcEnableServerReq)
+
+AigcEnableServerRes = _reflection.GeneratedProtocolMessageType('AigcEnableServerRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCENABLESERVERRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcEnableServerRes)
+  })
+_sym_db.RegisterMessage(AigcEnableServerRes)
+
+AddGroupReq = _reflection.GeneratedProtocolMessageType('AddGroupReq', (_message.Message,), {
+  'DESCRIPTOR' : _ADDGROUPREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AddGroupReq)
+  })
+_sym_db.RegisterMessage(AddGroupReq)
+
+AddGroupRes = _reflection.GeneratedProtocolMessageType('AddGroupRes', (_message.Message,), {
+  'DESCRIPTOR' : _ADDGROUPRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AddGroupRes)
+  })
+_sym_db.RegisterMessage(AddGroupRes)
+
+AigcGroupInfoReq = _reflection.GeneratedProtocolMessageType('AigcGroupInfoReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCGROUPINFOREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcGroupInfoReq)
+  })
+_sym_db.RegisterMessage(AigcGroupInfoReq)
+
+AigcGroupInfoRes = _reflection.GeneratedProtocolMessageType('AigcGroupInfoRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCGROUPINFORES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcGroupInfoRes)
+  })
+_sym_db.RegisterMessage(AigcGroupInfoRes)
+
+AigcGroupConfig = _reflection.GeneratedProtocolMessageType('AigcGroupConfig', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCGROUPCONFIG,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcGroupConfig)
+  })
+_sym_db.RegisterMessage(AigcGroupConfig)
+
+GetGroupDeviceReq = _reflection.GeneratedProtocolMessageType('GetGroupDeviceReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETGROUPDEVICEREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.GetGroupDeviceReq)
+  })
+_sym_db.RegisterMessage(GetGroupDeviceReq)
+
+GetGroupDeviceRes = _reflection.GeneratedProtocolMessageType('GetGroupDeviceRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETGROUPDEVICERES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.GetGroupDeviceRes)
+  })
+_sym_db.RegisterMessage(GetGroupDeviceRes)
+
+AigcDeviceInfo = _reflection.GeneratedProtocolMessageType('AigcDeviceInfo', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCDEVICEINFO,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcDeviceInfo)
+  })
+_sym_db.RegisterMessage(AigcDeviceInfo)
+
+DeviceInfo = _reflection.GeneratedProtocolMessageType('DeviceInfo', (_message.Message,), {
+  'DESCRIPTOR' : _DEVICEINFO,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.DeviceInfo)
+  })
+_sym_db.RegisterMessage(DeviceInfo)
+
+EditGroupConfigReq = _reflection.GeneratedProtocolMessageType('EditGroupConfigReq', (_message.Message,), {
+  'DESCRIPTOR' : _EDITGROUPCONFIGREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.EditGroupConfigReq)
+  })
+_sym_db.RegisterMessage(EditGroupConfigReq)
+
+EditGroupConfigRes = _reflection.GeneratedProtocolMessageType('EditGroupConfigRes', (_message.Message,), {
+  'DESCRIPTOR' : _EDITGROUPCONFIGRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.EditGroupConfigRes)
+  })
+_sym_db.RegisterMessage(EditGroupConfigRes)
+
+GetDeviceGroupReq = _reflection.GeneratedProtocolMessageType('GetDeviceGroupReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETDEVICEGROUPREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.GetDeviceGroupReq)
+  })
+_sym_db.RegisterMessage(GetDeviceGroupReq)
+
+GetDeviceGroupRes = _reflection.GeneratedProtocolMessageType('GetDeviceGroupRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETDEVICEGROUPRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.GetDeviceGroupRes)
+  })
+_sym_db.RegisterMessage(GetDeviceGroupRes)
+
+AigcDeviceGroup = _reflection.GeneratedProtocolMessageType('AigcDeviceGroup', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCDEVICEGROUP,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcDeviceGroup)
+  })
+_sym_db.RegisterMessage(AigcDeviceGroup)
+
+AigcWidget = _reflection.GeneratedProtocolMessageType('AigcWidget', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCWIDGET,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcWidget)
+  })
+_sym_db.RegisterMessage(AigcWidget)
+
+AigcOfficialMarketModelReq = _reflection.GeneratedProtocolMessageType('AigcOfficialMarketModelReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCOFFICIALMARKETMODELREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcOfficialMarketModelReq)
+  })
+_sym_db.RegisterMessage(AigcOfficialMarketModelReq)
+
+AigcOfficialMarketModelRes = _reflection.GeneratedProtocolMessageType('AigcOfficialMarketModelRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCOFFICIALMARKETMODELRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcOfficialMarketModelRes)
+  })
+_sym_db.RegisterMessage(AigcOfficialMarketModelRes)
+
+AigcMarketModel = _reflection.GeneratedProtocolMessageType('AigcMarketModel', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCMARKETMODEL,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcMarketModel)
+  })
+_sym_db.RegisterMessage(AigcMarketModel)
+
+AigcTrainMarketModelReq = _reflection.GeneratedProtocolMessageType('AigcTrainMarketModelReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCTRAINMARKETMODELREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcTrainMarketModelReq)
+  })
+_sym_db.RegisterMessage(AigcTrainMarketModelReq)
+
+AigcTrainMarketModelRes = _reflection.GeneratedProtocolMessageType('AigcTrainMarketModelRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCTRAINMARKETMODELRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcTrainMarketModelRes)
+  })
+_sym_db.RegisterMessage(AigcTrainMarketModelRes)
+
+AigcAppVersionLatestReq = _reflection.GeneratedProtocolMessageType('AigcAppVersionLatestReq', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCAPPVERSIONLATESTREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcAppVersionLatestReq)
+  })
+_sym_db.RegisterMessage(AigcAppVersionLatestReq)
+
+AigcAppVersionLatestRes = _reflection.GeneratedProtocolMessageType('AigcAppVersionLatestRes', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCAPPVERSIONLATESTRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcAppVersionLatestRes)
+  })
+_sym_db.RegisterMessage(AigcAppVersionLatestRes)
+
+CreateAigcAppVersionReq = _reflection.GeneratedProtocolMessageType('CreateAigcAppVersionReq', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEAIGCAPPVERSIONREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.CreateAigcAppVersionReq)
+  })
+_sym_db.RegisterMessage(CreateAigcAppVersionReq)
+
+CreateAigcAppVersionRes = _reflection.GeneratedProtocolMessageType('CreateAigcAppVersionRes', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEAIGCAPPVERSIONRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.CreateAigcAppVersionRes)
+  })
+_sym_db.RegisterMessage(CreateAigcAppVersionRes)
+
+CreateAigcAppVersionDiffReq = _reflection.GeneratedProtocolMessageType('CreateAigcAppVersionDiffReq', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEAIGCAPPVERSIONDIFFREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.CreateAigcAppVersionDiffReq)
+  })
+_sym_db.RegisterMessage(CreateAigcAppVersionDiffReq)
+
+CreateAigcAppVersionDiffRes = _reflection.GeneratedProtocolMessageType('CreateAigcAppVersionDiffRes', (_message.Message,), {
+  'DESCRIPTOR' : _CREATEAIGCAPPVERSIONDIFFRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.CreateAigcAppVersionDiffRes)
+  })
+_sym_db.RegisterMessage(CreateAigcAppVersionDiffRes)
+
+AigcAppVersionDiff = _reflection.GeneratedProtocolMessageType('AigcAppVersionDiff', (_message.Message,), {
+  'DESCRIPTOR' : _AIGCAPPVERSIONDIFF,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AigcAppVersionDiff)
+  })
+_sym_db.RegisterMessage(AigcAppVersionDiff)
+
+MarketModelListReq = _reflection.GeneratedProtocolMessageType('MarketModelListReq', (_message.Message,), {
+  'DESCRIPTOR' : _MARKETMODELLISTREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.MarketModelListReq)
+  })
+_sym_db.RegisterMessage(MarketModelListReq)
+
+MarketModelListRes = _reflection.GeneratedProtocolMessageType('MarketModelListRes', (_message.Message,), {
+  'DESCRIPTOR' : _MARKETMODELLISTRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.MarketModelListRes)
+  })
+_sym_db.RegisterMessage(MarketModelListRes)
+
+MarketModelFieldEnumReq = _reflection.GeneratedProtocolMessageType('MarketModelFieldEnumReq', (_message.Message,), {
+  'DESCRIPTOR' : _MARKETMODELFIELDENUMREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.MarketModelFieldEnumReq)
+  })
+_sym_db.RegisterMessage(MarketModelFieldEnumReq)
+
+MarketModelFieldEnumRes = _reflection.GeneratedProtocolMessageType('MarketModelFieldEnumRes', (_message.Message,), {
+  'DESCRIPTOR' : _MARKETMODELFIELDENUMRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.MarketModelFieldEnumRes)
+  })
+_sym_db.RegisterMessage(MarketModelFieldEnumRes)
+
+MarketModelFieldItem = _reflection.GeneratedProtocolMessageType('MarketModelFieldItem', (_message.Message,), {
+  'DESCRIPTOR' : _MARKETMODELFIELDITEM,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.MarketModelFieldItem)
+  })
+_sym_db.RegisterMessage(MarketModelFieldItem)
+
+MarketModelDownloadReq = _reflection.GeneratedProtocolMessageType('MarketModelDownloadReq', (_message.Message,), {
+  'DESCRIPTOR' : _MARKETMODELDOWNLOADREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.MarketModelDownloadReq)
+  })
+_sym_db.RegisterMessage(MarketModelDownloadReq)
+
+MarketModelDownloadRes = _reflection.GeneratedProtocolMessageType('MarketModelDownloadRes', (_message.Message,), {
+  'DESCRIPTOR' : _MARKETMODELDOWNLOADRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.MarketModelDownloadRes)
+  })
+_sym_db.RegisterMessage(MarketModelDownloadRes)
+
+MarketModelCreateWithTaskReq = _reflection.GeneratedProtocolMessageType('MarketModelCreateWithTaskReq', (_message.Message,), {
+  'DESCRIPTOR' : _MARKETMODELCREATEWITHTASKREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.MarketModelCreateWithTaskReq)
+  })
+_sym_db.RegisterMessage(MarketModelCreateWithTaskReq)
+
+MarketModelCreateWithTaskRes = _reflection.GeneratedProtocolMessageType('MarketModelCreateWithTaskRes', (_message.Message,), {
+  'DESCRIPTOR' : _MARKETMODELCREATEWITHTASKRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.MarketModelCreateWithTaskRes)
+  })
+_sym_db.RegisterMessage(MarketModelCreateWithTaskRes)
+
+MarketPluginListReq = _reflection.GeneratedProtocolMessageType('MarketPluginListReq', (_message.Message,), {
+  'DESCRIPTOR' : _MARKETPLUGINLISTREQ,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.MarketPluginListReq)
+  })
+_sym_db.RegisterMessage(MarketPluginListReq)
+
+MarketPluginListRes = _reflection.GeneratedProtocolMessageType('MarketPluginListRes', (_message.Message,), {
+  'DESCRIPTOR' : _MARKETPLUGINLISTRES,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.MarketPluginListRes)
+  })
+_sym_db.RegisterMessage(MarketPluginListRes)
+
+MarketPluginItem = _reflection.GeneratedProtocolMessageType('MarketPluginItem', (_message.Message,), {
+  'DESCRIPTOR' : _MARKETPLUGINITEM,
+  '__module__' : 'aigc_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.MarketPluginItem)
+  })
+_sym_db.RegisterMessage(MarketPluginItem)
+
+_AIGCEXTOBJ = DESCRIPTOR.services_by_name['AigcExtObj']
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\242\002\003PB3'
+  _UPLOADWIDGETSTATUS._serialized_start=6361
+  _UPLOADWIDGETSTATUS._serialized_end=6449
+  _GROUPCONFIGTYPE._serialized_start=6451
+  _GROUPCONFIGTYPE._serialized_end=6506
+  _TASKITEM._serialized_start=40
+  _TASKITEM._serialized_end=114
+  _GETTASKREQ._serialized_start=116
+  _GETTASKREQ._serialized_end=227
+  _GETTASKRES._serialized_start=229
+  _GETTASKRES._serialized_end=299
+  _TASKNOTIFYREQ._serialized_start=301
+  _TASKNOTIFYREQ._serialized_end=421
+  _TASKNOTIFYRES._serialized_start=423
+  _TASKNOTIFYRES._serialized_end=438
+  _AIGCDEVICEBINDREQ._serialized_start=440
+  _AIGCDEVICEBINDREQ._serialized_end=551
+  _AIGCDEVICEBINDRES._serialized_start=553
+  _AIGCDEVICEBINDRES._serialized_end=572
+  _AIGCDEVICEUNBINDREQ._serialized_start=574
+  _AIGCDEVICEUNBINDREQ._serialized_end=616
+  _AIGCDEVICEUNBINDRES._serialized_start=618
+  _AIGCDEVICEUNBINDRES._serialized_end=639
+  _AIGCDEVICEINFOREQ._serialized_start=641
+  _AIGCDEVICEINFOREQ._serialized_end=712
+  _AIGCDEVICEINFORES._serialized_start=714
+  _AIGCDEVICEINFORES._serialized_end=810
+  _APPLYWIDGETREQ._serialized_start=812
+  _APPLYWIDGETREQ._serialized_end=828
+  _APPLYWIDGETRES._serialized_start=830
+  _APPLYWIDGETRES._serialized_end=866
+  _CREATEWIDGETREQ._serialized_start=868
+  _CREATEWIDGETREQ._serialized_end=885
+  _CREATEWIDGETRES._serialized_start=887
+  _CREATEWIDGETRES._serialized_end=924
+  _UPLOADWIDGETURLREQ._serialized_start=926
+  _UPLOADWIDGETURLREQ._serialized_end=983
+  _UPLOADWIDGETURLRES._serialized_start=985
+  _UPLOADWIDGETURLRES._serialized_end=1039
+  _UPLOADWIDGETREQ._serialized_start=1041
+  _UPLOADWIDGETREQ._serialized_end=1092
+  _UPLOADWIDGETRES._serialized_start=1094
+  _UPLOADWIDGETRES._serialized_end=1128
+  _UPLOADWIDGETCHECKREQ._serialized_start=1130
+  _UPLOADWIDGETCHECKREQ._serialized_end=1186
+  _UPLOADWIDGETCHECKRES._serialized_start=1188
+  _UPLOADWIDGETCHECKRES._serialized_end=1270
+  _AIGCCREATEGROUPREQ._serialized_start=1273
+  _AIGCCREATEGROUPREQ._serialized_end=1409
+  _AIGCCREATEGROUPRES._serialized_start=1411
+  _AIGCCREATEGROUPRES._serialized_end=1457
+  _AIGCREMOVEGROUPREQ._serialized_start=1459
+  _AIGCREMOVEGROUPREQ._serialized_end=1545
+  _AIGCREMOVEGROUPRES._serialized_start=1547
+  _AIGCREMOVEGROUPRES._serialized_end=1567
+  _AIGCTASKRESULT._serialized_start=1569
+  _AIGCTASKRESULT._serialized_end=1613
+  _AIGCDATA._serialized_start=1615
+  _AIGCDATA._serialized_end=1698
+  _AIGCDATAEXTENSION._serialized_start=1700
+  _AIGCDATAEXTENSION._serialized_end=1783
+  _UPLOADFILEURLREQ._serialized_start=1785
+  _UPLOADFILEURLREQ._serialized_end=1852
+  _UPLOADFILEURLRES._serialized_start=1854
+  _UPLOADFILEURLRES._serialized_end=1906
+  _AIGCDEVICEEXPANSIONREQ._serialized_start=1908
+  _AIGCDEVICEEXPANSIONREQ._serialized_end=1972
+  _AIGCDEVICEEXPANSIONRES._serialized_start=1974
+  _AIGCDEVICEEXPANSIONRES._serialized_end=2057
+  _TASKCOUNTITEM._serialized_start=2059
+  _TASKCOUNTITEM._serialized_end=2113
+  _TASKCOUNTREQ._serialized_start=2115
+  _TASKCOUNTREQ._serialized_end=2150
+  _TASKCOUNTRES._serialized_start=2152
+  _TASKCOUNTRES._serialized_end=2200
+  _AIGCWIDGETITEM._serialized_start=2202
+  _AIGCWIDGETITEM._serialized_end=2266
+  _AIGCWIDGETLISTREQ._serialized_start=2268
+  _AIGCWIDGETLISTREQ._serialized_end=2308
+  _AIGCWIDGETLISTRES._serialized_start=2310
+  _AIGCWIDGETLISTRES._serialized_end=2364
+  _DELETEAIGCWIDGETREQ._serialized_start=2366
+  _DELETEAIGCWIDGETREQ._serialized_end=2440
+  _DELETEAIGCWIDGETRES._serialized_start=2442
+  _DELETEAIGCWIDGETRES._serialized_end=2463
+  _AIGCWIDGETCONFIG._serialized_start=2465
+  _AIGCWIDGETCONFIG._serialized_end=2506
+  _AIGCWIDGETINFOREQ._serialized_start=2508
+  _AIGCWIDGETINFOREQ._serialized_end=2539
+  _AIGCWIDGETINFORES._serialized_start=2542
+  _AIGCWIDGETINFORES._serialized_end=2817
+  _AIGCBILLREPORTREQ._serialized_start=2819
+  _AIGCBILLREPORTREQ._serialized_end=2870
+  _AIGCBILLREPORTRES._serialized_start=2872
+  _AIGCBILLREPORTRES._serialized_end=2907
+  _AIGCTRAININGMODELREQ._serialized_start=2909
+  _AIGCTRAININGMODELREQ._serialized_end=2949
+  _AIGCTRAININGMODELRES._serialized_start=2951
+  _AIGCTRAININGMODELRES._serialized_end=2988
+  _AIGCENABLESERVERREQ._serialized_start=2990
+  _AIGCENABLESERVERREQ._serialized_end=3048
+  _AIGCENABLESERVERRES._serialized_start=3050
+  _AIGCENABLESERVERRES._serialized_end=3084
+  _ADDGROUPREQ._serialized_start=3086
+  _ADDGROUPREQ._serialized_end=3173
+  _ADDGROUPRES._serialized_start=3175
+  _ADDGROUPRES._serialized_end=3188
+  _AIGCGROUPINFOREQ._serialized_start=3190
+  _AIGCGROUPINFOREQ._serialized_end=3220
+  _AIGCGROUPINFORES._serialized_start=3223
+  _AIGCGROUPINFORES._serialized_end=3478
+  _AIGCGROUPCONFIG._serialized_start=3480
+  _AIGCGROUPCONFIG._serialized_end=3519
+  _GETGROUPDEVICEREQ._serialized_start=3521
+  _GETGROUPDEVICEREQ._serialized_end=3558
+  _GETGROUPDEVICERES._serialized_start=3560
+  _GETGROUPDEVICERES._serialized_end=3620
+  _AIGCDEVICEINFO._serialized_start=3623
+  _AIGCDEVICEINFO._serialized_end=3785
+  _DEVICEINFO._serialized_start=3787
+  _DEVICEINFO._serialized_end=3817
+  _EDITGROUPCONFIGREQ._serialized_start=3819
+  _EDITGROUPCONFIGREQ._serialized_end=3926
+  _EDITGROUPCONFIGRES._serialized_start=3928
+  _EDITGROUPCONFIGRES._serialized_end=3948
+  _GETDEVICEGROUPREQ._serialized_start=3950
+  _GETDEVICEGROUPREQ._serialized_end=4020
+  _GETDEVICEGROUPRES._serialized_start=4022
+  _GETDEVICEGROUPRES._serialized_end=4076
+  _AIGCDEVICEGROUP._serialized_start=4079
+  _AIGCDEVICEGROUP._serialized_end=4213
+  _AIGCWIDGET._serialized_start=4216
+  _AIGCWIDGET._serialized_end=4428
+  _AIGCOFFICIALMARKETMODELREQ._serialized_start=4430
+  _AIGCOFFICIALMARKETMODELREQ._serialized_end=4487
+  _AIGCOFFICIALMARKETMODELRES._serialized_start=4489
+  _AIGCOFFICIALMARKETMODELRES._serialized_end=4553
+  _AIGCMARKETMODEL._serialized_start=4556
+  _AIGCMARKETMODEL._serialized_end=4784
+  _AIGCTRAINMARKETMODELREQ._serialized_start=4786
+  _AIGCTRAINMARKETMODELREQ._serialized_end=4840
+  _AIGCTRAINMARKETMODELRES._serialized_start=4842
+  _AIGCTRAINMARKETMODELRES._serialized_end=4903
+  _AIGCAPPVERSIONLATESTREQ._serialized_start=4905
+  _AIGCAPPVERSIONLATESTREQ._serialized_end=4979
+  _AIGCAPPVERSIONLATESTRES._serialized_start=4981
+  _AIGCAPPVERSIONLATESTRES._serialized_end=5099
+  _CREATEAIGCAPPVERSIONREQ._serialized_start=5101
+  _CREATEAIGCAPPVERSIONREQ._serialized_end=5209
+  _CREATEAIGCAPPVERSIONRES._serialized_start=5211
+  _CREATEAIGCAPPVERSIONRES._serialized_end=5236
+  _CREATEAIGCAPPVERSIONDIFFREQ._serialized_start=5238
+  _CREATEAIGCAPPVERSIONDIFFREQ._serialized_end=5341
+  _CREATEAIGCAPPVERSIONDIFFRES._serialized_start=5343
+  _CREATEAIGCAPPVERSIONDIFFRES._serialized_end=5372
+  _AIGCAPPVERSIONDIFF._serialized_start=5374
+  _AIGCAPPVERSIONDIFF._serialized_end=5449
+  _MARKETMODELLISTREQ._serialized_start=5452
+  _MARKETMODELLISTREQ._serialized_end=5662
+  _MARKETMODELLISTRES._serialized_start=5664
+  _MARKETMODELLISTRES._serialized_end=5720
+  _MARKETMODELFIELDENUMREQ._serialized_start=5722
+  _MARKETMODELFIELDENUMREQ._serialized_end=5747
+  _MARKETMODELFIELDENUMRES._serialized_start=5750
+  _MARKETMODELFIELDENUMRES._serialized_end=5910
+  _MARKETMODELFIELDITEM._serialized_start=5912
+  _MARKETMODELFIELDITEM._serialized_end=5960
+  _MARKETMODELDOWNLOADREQ._serialized_start=5962
+  _MARKETMODELDOWNLOADREQ._serialized_end=5998
+  _MARKETMODELDOWNLOADRES._serialized_start=6000
+  _MARKETMODELDOWNLOADRES._serialized_end=6024
+  _MARKETMODELCREATEWITHTASKREQ._serialized_start=6026
+  _MARKETMODELCREATEWITHTASKREQ._serialized_end=6130
+  _MARKETMODELCREATEWITHTASKRES._serialized_start=6132
+  _MARKETMODELCREATEWITHTASKRES._serialized_end=6162
+  _MARKETPLUGINLISTREQ._serialized_start=6164
+  _MARKETPLUGINLISTREQ._serialized_end=6185
+  _MARKETPLUGINLISTRES._serialized_start=6187
+  _MARKETPLUGINLISTRES._serialized_end=6251
+  _MARKETPLUGINITEM._serialized_start=6253
+  _MARKETPLUGINITEM._serialized_end=6359
+  _AIGCEXTOBJ._serialized_start=6509
+  _AIGCEXTOBJ._serialized_end=8847
+# @@protoc_insertion_point(module_scope)
```

### Comparing `mecord-cli-0.1.90/mecord/capability_provider.py` & `mecord-cli-0.1.91/mecord/capability_provider.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/common_ext_pb2.py` & `mecord-cli-0.1.91/mecord/common_ext_pb2.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,712 +1,712 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: common_ext.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63ommon_ext.proto\x12\x02pb\"\xf7\x02\n\x06Player\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08nickname\x18\x02 \x01(\t\x12\x18\n\x03sex\x18\x03 \x01(\x0e\x32\x0b.pb.SexType\x12\x0b\n\x03id2\x18\x04 \x01(\x03\x12\x0c\n\x04icon\x18\x05 \x01(\t\x12\r\n\x05\x66lags\x18\x06 \x01(\x03\x12\r\n\x05\x63harm\x18\x08 \x01(\x03\x12\x13\n\x0b\x63harm_level\x18\t \x01(\x05\x12\x14\n\x0cwealth_level\x18\n \x01(\x05\x12\x0e\n\x06wealth\x18\x0b \x01(\x03\x12\x12\n\nonline_exp\x18\x0c \x01(\r\x12\x11\n\tcreate_at\x18\r \x01(\r\x12\x11\n\tis_delete\x18\x0e \x01(\x08\x12\r\n\x05point\x18\x0f \x01(\x03\x12\x13\n\x0bpoint_level\x18\x10 \x01(\x05\x12\x11\n\tsignature\x18\x11 \x01(\t\x12\x0c\n\x04\x63ity\x18\x12 \x01(\t\x12\x10\n\x08\x62irthday\x18\x13 \x01(\t\x12\x14\n\x0conline_state\x18\x14 \x01(\x05\x12\x1a\n\x12NicknameUpdateTime\x18\x15 \x01(\r\"\x81\x01\n\x08UserInfo\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0c\n\x04\x63ity\x18\x02 \x01(\t\x12\x11\n\tsignature\x18\x03 \x01(\t\x12\x0c\n\x04mind\x18\x04 \x01(\t\x12\x10\n\x08\x62irthday\x18\x05 \x01(\t\x12\x15\n\rintimate_slot\x18\x06 \x01(\x11\x12\x11\n\tnameplate\x18\x07 \x01(\t\"\xd7\x02\n\nPlayerInfo\x12\x1a\n\x06player\x18\x01 \x01(\x0b\x32\n.pb.Player\x12\x1a\n\x06\x65\x66\x66\x65\x63t\x18\x02 \x03(\x0b\x32\n.pb.Effect\x12\x1a\n\x04\x63lan\x18\x03 \x01(\x0b\x32\x0c.pb.ClanInfo\x12\x10\n\x08\x66\x61ns_num\x18\x04 \x01(\x05\x12\x15\n\rfollowing_num\x18\x05 \x01(\x05\x12\x14\n\x0c\x66riend_alias\x18\x06 \x01(\t\x12\x1f\n\x07\x65\x66\x66\x65\x63ts\x18\x07 \x03(\x0b\x32\x0e.pb.EffectInfo\x12\x18\n\x10\x61ttitude_yes_num\x18\x08 \x01(\x03\x12\x17\n\x0ftotal_visit_num\x18\t \x01(\x03\x12\x15\n\radd_visit_num\x18\n \x01(\x03\x12\x1c\n\x05label\x18\x0b \x03(\x0b\x32\r.pb.LabelInfo\x12-\n\x0c\x64\x65grees_info\x18\x0c \x01(\x0b\x32\x17.pb.AttitudeDegreesInfo\"=\n\x07\x42\x61gItem\x12\x0f\n\x07gift_id\x18\x01 \x01(\r\x12\x0e\n\x06\x61mount\x18\x02 \x01(\r\x12\x11\n\tcteate_at\x18\x03 \x01(\t\"\"\n\x08\x41godaKey\x12\x16\n\x0epermission_key\x18\x01 \x01(\t\":\n\x0bOnOffStatus\x12\x0e\n\x06status\x18\x01 \x01(\x11\x12\x1b\n\x04type\x18\x02 \x01(\x0e\x32\r.pb.OnOffType\"\xf8\x01\n\x11SearchPlayerEntry\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0b\n\x03id2\x18\x02 \x01(\x12\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x18\n\x03sex\x18\x04 \x01(\x0e\x32\x0b.pb.SexType\x12\x0c\n\x04icon\x18\x05 \x01(\t\x12\r\n\x05\x63harm\x18\x06 \x01(\x12\x12\x13\n\x0b\x63harm_level\x18\x07 \x01(\x11\x12\x0e\n\x06wealth\x18\x08 \x01(\x12\x12\x14\n\x0cwealth_level\x18\t \x01(\x11\x12\x0e\n\x06online\x18\n \x01(\x08\x12\x0f\n\x07room_id\x18\x0b \x01(\x12\x12\x12\n\nhas_passwd\x18\r \x01(\x08\x12\x11\n\tsignature\x18\x0e \x01(\t\"\x9f\x01\n\nEffectInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12%\n\ttime_type\x18\x02 \x01(\x0e\x32\x12.pb.EffectTimeType\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\x03\x12\'\n\nuse_status\x18\x04 \x01(\x0e\x32\x13.pb.EffectUseStatus\x12#\n\x0b\x65\x66\x66\x65\x63t_type\x18\x05 \x01(\x0e\x32\x0e.pb.EffectType\"\xaf\x01\n\x06\x45\x66\x66\x65\x63t\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04\x66lag\x18\x02 \x01(\x05\x12\x0b\n\x03str\x18\x03 \x01(\t\x12%\n\ttime_type\x18\x04 \x01(\x0e\x32\x12.pb.EffectTimeType\x12\x10\n\x08\x65nd_time\x18\x05 \x01(\x05\x12\'\n\nuse_status\x18\x06 \x01(\x0e\x32\x13.pb.EffectUseStatus\x12\x1c\n\x04type\x18\x07 \x01(\x0e\x32\x0e.pb.EffectType\"T\n\x0c\x45\x66\x66\x65\x63tConfig\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x1c\n\x04type\x18\x02 \x01(\x0e\x32\x0e.pb.EffectType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\"6\n\x15\x45\x66\x66\x65\x63tNicknamePendant\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x10\n\x08show_url\x18\x02 \x01(\t\"G\n\rEffectSerConf\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x1c\n\x04type\x18\x02 \x01(\x0e\x32\x0e.pb.EffectType\x12\x0c\n\x04name\x18\x03 \x01(\t\"0\n\rIndexTipRooms\x12\x0f\n\x07room_id\x18\x01 \x01(\x03\x12\x0e\n\x06tip_id\x18\x02 \x01(\x05\"=\n\x07RegisId\x12\x0b\n\x03ios\x18\x01 \x01(\t\x12\x0f\n\x07\x61ndroid\x18\x02 \x01(\t\x12\x14\n\x0cmanufacturer\x18\x03 \x01(\t\"P\n\nModelOnOff\x12\x1c\n\x05onOff\x18\x01 \x01(\x0e\x32\r.pb.OnOffType\x12$\n\x06status\x18\x02 \x01(\x0e\x32\x14.pb.ModelOnOffStatus\"\xd0\x01\n\x04Rank\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x18\n\x03sex\x18\x03 \x01(\x0e\x32\x0b.pb.SexType\x12\r\n\x05level\x18\x04 \x01(\r\x12\r\n\x05value\x18\x05 \x01(\x04\x12\x10\n\x08res_time\x18\x06 \x01(\r\x12\x0f\n\x07gap_val\x18\x07 \x01(\r\x12\x0c\n\x04icon\x18\x08 \x01(\t\x12\x0f\n\x07gift_id\x18\t \x01(\x04\x12\x10\n\x08gift_num\x18\n \x01(\r\x12\x0f\n\x07ranking\x18\x0b \x01(\r\x12\x11\n\tgift_name\x18\x0c \x01(\t\"5\n\x0fPlayerChairRoom\x12\x11\n\tplayer_id\x18\x01 \x01(\x03\x12\x0f\n\x07room_id\x18\x02 \x01(\x03\"l\n\x08\x43lanInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x11\n\ticon_word\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\x03\x12\x12\n\nlevel_name\x18\x05 \x01(\t\x12\x10\n\x08is_admin\x18\x06 \x01(\x08\"*\n\x06Period\x12\x10\n\x08\x62\x65gin_at\x18\x01 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x02 \x01(\x03\",\n\tLabelInfo\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63lassify_id\x18\x02 \x01(\x05\"Y\n\x13PlayerResourceShort\x12-\n\rresource_type\x18\x01 \x01(\x0e\x32\x16.pb.PlayerResourceType\x12\x13\n\x0bresource_id\x18\x02 \x01(\t\"\x96\x01\n\x0ePlayerResource\x12-\n\rresource_type\x18\x01 \x01(\x0e\x32\x16.pb.PlayerResourceType\x12\x13\n\x0bresource_id\x18\x02 \x01(\t\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x14\n\x0chead_img_url\x18\x04 \x01(\t\x12\x18\n\x03sex\x18\x05 \x01(\x0e\x32\x0b.pb.SexType\"c\n\x17PlayerResourceWithScore\x12+\n\x0fplayer_resource\x18\x01 \x01(\x0b\x32\x12.pb.PlayerResource\x12\r\n\x05score\x18\x02 \x01(\x03\x12\x0c\n\x04rank\x18\x03 \x01(\x05\"\xb4\x01\n\x13\x41ttitudeDegreesInfo\x12\x35\n\x0e\x64\x65grees_status\x18\x01 \x01(\x0e\x32\x1d.pb.AttitudeDegreesStatusType\x12\x36\n\rcategory_info\x18\x02 \x03(\x0b\x32\x1f.pb.AttitudeCategoryDegreesInfo\x12\x14\n\x0ctotal_degree\x18\x03 \x01(\x05\x12\x18\n\x10\x61nalysis_content\x18\x04 \x01(\t\"g\n\x1b\x41ttitudeCategoryDegreesInfo\x12\x13\n\x0b\x63\x61tegory_id\x18\x01 \x01(\x05\x12\x15\n\rcategory_name\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65gree\x18\x03 \x01(\x05\x12\x0c\n\x04icon\x18\x04 \x01(\t\"\x85\x01\n\x0e\x43MediaResource\x12\"\n\nmedia_type\x18\x01 \x01(\x0e\x32\x0e.pb.CMediaType\x12\x11\n\tmedia_url\x18\x02 \x01(\t\x12\x11\n\tcover_url\x18\x03 \x01(\t\x12\x13\n\x0bmedia_width\x18\x04 \x01(\x05\x12\x14\n\x0cmedia_height\x18\x05 \x01(\x05\"\x1b\n\x0bSayHelloReq\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1c\n\x0bSayHelloRes\x12\r\n\x05reply\x18\x01 \x01(\t\"b\n\x0cHeartbeatReq\x12\x0f\n\x07goim_id\x18\x01 \x01(\x03\x12\x11\n\tplayer_id\x18\x02 \x01(\x03\x12\n\n\x02ip\x18\x03 \x01(\t\x12\"\n\ndeviceType\x18\x04 \x01(\x0e\x32\x0e.pb.DeviceType\"!\n\x0cHeartbeatRes\x12\x11\n\ttimestamp\x18\x02 \x01(\x03*\xad\x01\n\tCommonErr\x12\x0f\n\x0b\x45rrCodeNone\x10\x00\x12\x11\n\x0c\x45rrCodeRedis\x10\x91N\x12\x11\n\x0c\x45rrCodeMysql\x10\x92N\x12\x15\n\x10\x45rrCodeFrequency\x10\x93N\x12\x11\n\x0c\x45rrCodeParam\x10\x94N\x12\x16\n\x11\x45rrCodeNoMatchObj\x10\x95N\x12\x10\n\x0b\x45rrCodeBusy\x10\x96N\x12\x15\n\x0f\x45rrCodeMaintain\x10\x9a\x82\x01*,\n\x07SexType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04MALE\x10\x01\x12\n\n\x06\x46\x45MALE\x10\x02*0\n\x0bOwnerInRoom\x12\x11\n\rNotInSelfRoom\x10\x00\x12\x0e\n\nInSelfRoom\x10\x01*%\n\tSceneType\x12\x0b\n\x07ST_ZERO\x10\x00\x12\x0b\n\x07ST_HOME\x10\x01*y\n\rRoomAdminType\x12\r\n\tRAT_GUEST\x10\x00\x12\x0e\n\nRAT_NORMAL\x10\n\x12\r\n\tRAT_ADMIN\x10\x14\x12\r\n\tRAT_OWNER\x10\x1e\x12\x13\n\x0fRAT_SUPER_ADMIN\x10(\x12\x16\n\tRAT_BLACK\x10\xfb\xff\xff\xff\xff\xff\xff\xff\xff\x01*\xfb\x01\n\nDeviceType\x12\x0e\n\nDT_UNKNOWN\x10\x00\x12\x12\n\x0e\x44T_FLASHPLAYER\x10\x01\x12\x14\n\x10\x44T_ANDROID_PHONE\x10\x14\x12\x10\n\x0c\x44T_IOS_PHONE\x10(\x12\x18\n\x14\x44T_WINDOWS_ASSISTANT\x10P\x12\x11\n\rDT_WINDOWS_PC\x10Z\x12\x0c\n\x08\x44T_ROBOT\x10\x64\x12\x1a\n\x16\x44T_WECHAT_SUBSCRIPTION\x10n\x12\x17\n\x13\x44T_QQ_SMALL_PROGRAM\x10x\x12\x17\n\x12\x44T_WX_MINI_PROGRAM\x10\x82\x01\x12\x0b\n\x06\x44T_WEB\x10\x8c\x01\x12\x0b\n\x06\x44T_MAC\x10\x96\x01*\x99\x01\n\x0bPlayerFlags\x12\x0b\n\x07PF_ZERO\x10\x00\x12\x14\n\x10PF_CERTIFICATION\x10\x01\x12\x10\n\x0cPF_BIND_BANK\x10\x04\x12\r\n\tPF_INVITE\x10\x05\x12\x13\n\x0fPF_CHARGE_FIRST\x10\x0c\x12\x18\n\x14PF_ATTITUDE_QUESTION\x10\r\x12\x17\n\x13PF_END_REGISTRATION\x10\x0e*2\n\x0c\x41\x63\x63ountFlags\x12\x0b\n\x07\x41\x46_ZERO\x10\x00\x12\x15\n\x11\x41\x46_PHONE_VERIFIED\x10\x01*\xfc\r\n\tOnOffType\x12\x0c\n\x08YEAR_BAG\x10\x00\x12\r\n\tCRACK_EGG\x10\x01\x12\x0e\n\nGOOGLE_PAY\x10\x05\x12\x0b\n\x07IAP_PAY\x10\x06\x12\n\n\x06INVITE\x10\x07\x12\x12\n\x0eINDEX_CATEGORY\x10\x08\x12\n\n\x06\x43\x45RTIF\x10\t\x12\t\n\x05GUARD\x10\n\x12\x10\n\x0cLOTTERY_DRAW\x10\x0c\x12\x0f\n\x0bMENTOR_SHIP\x10\r\x12\x0e\n\nCERTIF_IOS\x10\x0e\x12\x11\n\rREAL_IDENTITY\x10\x0f\x12\x0f\n\x0bNOVICE_GIFT\x10\x10\x12\x12\n\x0eROOM_SET_MODEL\x10\x12\x12\x11\n\rACTIVITY_TYPE\x10\x14\x12\x0c\n\x08\x41\x43TIVITY\x10\x15\x12\x0c\n\x08HOT_SONG\x10\x17\x12\x0e\n\nROOM_ENTER\x10\"\x12\x1d\n\x19ROOM_PATTERN_HIGH_QUALITY\x10#\x12\x11\n\rAUTH_LOGIN_UI\x10&\x12\x12\n\x0eUSER_DATA_EDIT\x10)\x12\x11\n\rCERTIFICATION\x10+\x12\x1b\n\x17\x43\x45RTIFICATION_ROOM_SHOW\x10,\x12%\n!CERTIFICATION_ROOM_WIN_OPEN_CLOSE\x10-\x12\x10\n\x0c\x43\x45RTIFY_WORD\x10.\x12\x11\n\rCERTIFY_CHAIR\x10/\x12\x1c\n\x18\x43\x45RTIFY_UPDATE_USER_INFO\x10\x30\x12\x1c\n\x18\x43\x45RTIFY_BROADCAST_FRIEND\x10\x31\x12\x15\n\x11\x43\x45RTIFY_HEAD_LINE\x10\x32\x12\x15\n\x11\x43\x45RTIFY_TIAO_TIAO\x10\x33\x12\x14\n\x10LOGIN_BIND_PHONE\x10\x34\x12\x1c\n\x18\x43\x45RTIFY_OWNER_ENTER_ROOM\x10\x35\x12\x0f\n\x0bYoung_Model\x10:\x12\x14\n\x10\x43USTOMER_SERVICE\x10;\x12\x15\n\x11OVERSEAS_IP_LIMIT\x10\x42\x12\x12\n\x0eOLD_NAME_LIMIT\x10\x43\x12\x12\n\x0e\x43RACK_SELF_MSG\x10\x44\x12\x12\n\x0eORDER_LOCATION\x10G\x12\x12\n\x0e\x44\x45LETE_ACCOUNT\x10I\x12\x0f\n\x0bYUNPIAN_SMS\x10J\x12\x11\n\rBIND_PHONE_V2\x10K\x12\x14\n\x10\x42IND_PHONE_LOGIN\x10L\x12\x0e\n\nCOUNT_DOWN\x10N\x12\x0e\n\nOXYGEN_BAR\x10^\x12\x13\n\x0fPRIVACY_SETTING\x10_\x12\x1f\n\x1bOXYGEN_BAR_CLAN_MEMBER_ONLY\x10`\x12\x18\n\x14OXYGEN_BAR_TREND_GIF\x10\x61\x12\x0e\n\nDATA_AUDIT\x10\x62\x12\r\n\tInner_Tec\x10\x64\x12\r\n\tInner_Ali\x10\x65\x12\x16\n\x12\x43\x45RTIFY_IM_PICTURE\x10g\x12\x0b\n\x07\x43MB_VIP\x10h\x12\x13\n\x0f\x43RACKEGG_FOREST\x10i\x12\x13\n\x0e\x41NTI_ADDICTION\x10\xc8\x01\x12&\n!TEXT_FILTER_ROOM_SCREEN_ENCRYPTED\x10\xc9\x01\x12(\n#TEXT_FILTER_ROOM_SCREEN_UNENCRYPTED\x10\xca\x01\x12!\n\x1cTEXT_FILTER_BROADCAST_FRIEND\x10\xcb\x01\x12\x1d\n\x18TEXT_FILTER_PRIVATE_CHAT\x10\xcc\x01\x12\x10\n\x0c\x42\x43_HEAD_LINE\x10n\x12\x13\n\x0fONE_CLICK_LOGIN\x10o\x12\x0e\n\nCERTIFY_PM\x10p\x12\x13\n\x0f\x43\x45RTIFY_PICTURE\x10q\x12\x19\n\x15\x43HANNEL_ADVERT_AUDITS\x10r\x12\x1a\n\x16\x43\x45RTIFY_CREATE_CHANNEL\x10t\x12\x18\n\x14\x43\x45RTIFY_JOIN_CHANNEL\x10u\x12\x10\n\x0c\x43\x45RTIFY_GIVE\x10v\x12\x17\n\x13\x43\x45RTIFY_ROOM_NOTICE\x10w\x12\x14\n\x10\x43\x45RTIFY_RECHARGE\x10x\x12\x19\n\x15\x43\x45RTIFY_PUBLISH_TREND\x10y\x12\x19\n\x15\x43\x45RTIFY_COMMENT_TREND\x10z\x12\x11\n\rHOME_NAV_TYPE\x10{\x12\x11\n\rLOGIN_CHECKED\x10|\x12\x0e\n\nHIGH_SOUND\x10}\x12\x16\n\x12HIGH_SOUND_CHANNEL\x10~\x12\x1a\n\x16\x43HANNEL_STAR_CHALLENGE\x10\x7f\x12\x11\n\x0c\x43HANNEL_STAT\x10\x80\x01\x12\x11\n\x0cREGISTER_SEX\x10\x82\x01\x12\x16\n\x11REGISTER_NICKNAME\x10\x83\x01\x12\x16\n\x11REGISTER_ATTITUDE\x10\x84\x01\x12\x13\n\x0e\x43REATE_CHANNEL\x10\x85\x01\x12\x1a\n\x15\x43OMMUNITY_TREND_AUDIO\x10\x86\x01\x12\x0c\n\x07IM_TIPS\x10\x87\x01\x12\x18\n\x13MULTI_CLIENT_ONLINE\x10\xfd\x01*)\n\nStatusCode\x12\x0b\n\x07SC_FAIL\x10\x00\x12\x0e\n\nSC_SUCCESS\x10\x01*?\n\nEffectType\x12\x12\n\x0e\x45\x66\x66\x65\x63tTypeNone\x10\x00\x12\x1d\n\x19\x45\x66\x66\x65\x63tTypeNicknamePendant\x10\x01*\x7f\n\x0e\x45\x66\x66\x65\x63tTimeType\x12\x18\n\x14\x45\x66\x66\x65\x63tTimeTypeAlways\x10\x00\x12\x16\n\x12\x45\x66\x66\x65\x63tTimeTypeMike\x10\x01\x12\x1e\n\x1a\x45\x66\x66\x65\x63tTimeTypeWearInPacket\x10\x02\x12\x1b\n\x17\x45\x66\x66\x65\x63tTimeTypePermanent\x10\x03*,\n\x0f\x45\x66\x66\x65\x63tUseStatus\x12\n\n\x06\x45S_Use\x10\x00\x12\r\n\tES_NotUse\x10\x01*I\n\x10\x45\x66\x66\x65\x63tNoticeType\x12\x18\n\x14\x45\x66\x66\x65\x63tNoticeTypeGain\x10\x00\x12\x1b\n\x17\x45\x66\x66\x65\x63tNoticeTypeTimeout\x10\x01*:\n\x10ModelOnOffStatus\x12\x0b\n\x07\x41LL_OFF\x10\x00\x12\n\n\x06\x41LL_ON\x10\x01\x12\r\n\tWHITELIST\x10\x02*A\n\x08RankType\x12\x0b\n\x07RT_ZERO\x10\x00\x12\x0c\n\x08RT_CHARM\x10\x01\x12\r\n\tRT_WEALTH\x10\x02\x12\x0b\n\x07RT_GIFT\x10\x03*N\n\rLoadClickType\x12\x0c\n\x08LCT_ZERO\x10\x00\x12\x17\n\x13LCT_INTIMATE_DETAIL\x10\x01\x12\x16\n\x12LCT_INTIMATE_STORE\x10\x02*F\n\x0b\x41uditStatus\x12\x11\n\rAS_Audit_Pass\x10\x00\x12\x0f\n\x0b\x41S_Auditing\x10\x01\x12\x13\n\x0f\x41S_Audit_Refuse\x10\x02*\xf3\x01\n\nUploadType\x12\x0c\n\x08TypeZero\x10\x00\x12\x10\n\x0cHeadAlbumImg\x10\x01\x12\x0f\n\x0bHeadIconImg\x10\x02\x12\x0f\n\x0b\x44ynamicsImg\x10\x03\x12\r\n\tClientLog\x10\x04\x12\x0e\n\nTipOffsImg\x10\x05\x12\x0c\n\x08Indetity\x10\x06\x12\x0b\n\x07PMMedia\x10\x07\x12\t\n\x05Voice\x10\x08\x12\x11\n\rBackgroundImg\x10\x17\x12\x0f\n\x0b\x43hannelIcon\x10\x18\x12\x11\n\rWXRobotQRcode\x10\x19\x12\x13\n\x0f\x43ommunityTagImg\x10\x1c\x12\x12\n\x0ePersonLabelImg\x10\x1d*\xe9\x01\n\x0ePayChannelType\x12\x0c\n\x08PCT_NULL\x10\x00\x12\x11\n\rPCT_ALIPAY_H5\x10\x02\x12\x12\n\x0ePCT_ALIPAY_APP\x10\x03\x12\x11\n\rPCT_WXPAY_APP\x10\x04\x12\x10\n\x0cPCT_WXPAY_H5\x10\x05\x12\x0b\n\x07PCT_IAP\x10\x06\x12\x0c\n\x08PCT_PLAY\x10\x08\x12\x0e\n\nPCT_PAYPAL\x10\n\x12\r\n\tPCT_BOING\x10\x0b\x12\x10\n\x0cPCT_UNIONPAY\x10\x0c\x12\x0e\n\tPCT_AGENT\x10\xfd\x01\x12\x0f\n\nPCT_MANUAL\x10\xfe\x01\x12\x10\n\x0bPCT_DEVTEST\x10\xff\x01*i\n\x04Role\x12\n\n\x06R_NONE\x10\x00\x12\x0f\n\x0bR_SUPERUSER\x10\x01\x12\x08\n\x04R_OW\x10\x02\x12\x08\n\x04R_VP\x10\x03\x12\x08\n\x04R_MA\x10\x04\x12\t\n\x05R_CA1\x10\x05\x12\t\n\x05R_CA2\x10\x06\x12\x07\n\x03R_R\x10\x07\x12\x07\n\x03R_U\x10\x08*]\n\x0eNameplateStyle\x12\x0b\n\x07NS_NONE\x10\x00\x12\x0e\n\nNS_STYLE_1\x10\x01\x12\x0e\n\nNS_STYLE_2\x10\x02\x12\x0e\n\nNS_STYLE_3\x10\x03\x12\x0e\n\nNS_STYLE_4\x10\x04*E\n\x12PlayerResourceType\x12\x0c\n\x08PRT_NONE\x10\x00\x12\x15\n\x11PRT_FIRST_ACCOUNT\x10\x01\x12\n\n\x06PRT_WX\x10\x02*f\n\x19\x41ttitudeDegreesStatusType\x12\x13\n\x0f\x41\x44ST_BOTH_EVERY\x10\x00\x12\x17\n\x13\x41\x44ST_OPPOSITE_EVERY\x10\x01\x12\x1b\n\x17\x41\x44ST_OPPOSITE_NOTENOUGH\x10\x02*u\n\nCMediaType\x12\x13\n\x0f\x43MediaType_None\x10\x00\x12\x12\n\x0e\x43MediaType_Png\x10\x01\x12\x12\n\x0e\x43MediaType_Gif\x10\x02\x12\x14\n\x10\x43MediaType_Video\x10\x03\x12\x14\n\x10\x43MediaType_Audio\x10\x04*w\n\x11\x44\x65viceConnectOper\x12\x0c\n\x08\x44\x43S_None\x10\x00\x12\x12\n\x0e\x44\x43S_Requesting\x10\x01\x12\x0f\n\x0b\x44\x43S_Receive\x10\x02\x12\x0e\n\nDCS_Refuse\x10\x03\x12\x0f\n\x0b\x44\x43S_Timeout\x10\x04\x12\x0e\n\nDCS_Cancel\x10\x05*\xa7\x01\n\x0b\x44\x65viceCmdId\x12\x11\n\rDC_DeviceZero\x10\x00\x12\x14\n\x0e\x44\x43_DeviceLogin\x10\x99\x98\x1f\x12\x1e\n\x18\x44\x43_MessageConnectOperate\x10\x9a\x98\x1f\x12\x1c\n\x16\x44\x43_MessageStatusUpdate\x10\x9b\x98\x1f\x12\x1a\n\x14\x44\x43_DeviceShareStatus\x10\x9c\x98\x1f\x12\x15\n\x0f\x44\x43_SingoConnect\x10\xb9\xa5%*L\n\nTaskStatus\x12\x0b\n\x07TS_None\x10\x00\x12\x11\n\rTS_Processing\x10\x01\x12\x0e\n\nTS_Success\x10\x02\x12\x0e\n\nTS_Failure\x10\x03*N\n\x08TaskType\x12\x0b\n\x07TT_None\x10\x00\x12\x0c\n\x08TT_Image\x10\x01\x12\x0c\n\x08TT_Video\x10\x02\x12\x0c\n\x08TT_Audio\x10\x03\x12\x0b\n\x07TT_Text\x10\x04*o\n\tLabelType\x12\x0b\n\x07LT_NONE\x10\x00\x12\x0b\n\x07LT_POST\x10\x01\x12\x0e\n\nLT_Gallery\x10\x02\x12\x0c\n\x08LT_Group\x10\x03\x12\x0e\n\nLT_Comment\x10\x04\x12\x0b\n\x07LT_Lora\x10\x05\x12\r\n\tLT_Client\x10\x06*N\n\x08\x41igcType\x12\x0b\n\x07\x41T_NONE\x10\x00\x12\x0c\n\x08\x41T_IMAGE\x10\x01\x12\x0c\n\x08\x41T_VIDEO\x10\x02\x12\x0c\n\x08\x41T_AUDIO\x10\x03\x12\x0b\n\x07\x41T_TEXT\x10\x04*%\n\x06Module\x12\n\n\x06M_None\x10\x00\x12\x0f\n\x0bM_Subscribe\x10\x01*A\n\nWidgetType\x12\x0b\n\x07WT_None\x10\x00\x12\x0e\n\nWT_General\x10\x01\x12\t\n\x05WT_SD\x10\x02\x12\x0b\n\x07WT_Lora\x10\x03*:\n\rCalculateMode\x12\x0b\n\x07\x43M_None\x10\x00\x12\r\n\tCM_Single\x10\x01\x12\r\n\tCM_Minute\x10\x02*1\n\x0e\x43hargeCateType\x12\x0e\n\nCCT_Normal\x10\x00\x12\x0f\n\x0b\x43\x43T_ActCard\x10\x01\x42\x06\xa2\x02\x03PB3b\x06proto3')
-
-_COMMONERR = DESCRIPTOR.enum_types_by_name['CommonErr']
-CommonErr = enum_type_wrapper.EnumTypeWrapper(_COMMONERR)
-_SEXTYPE = DESCRIPTOR.enum_types_by_name['SexType']
-SexType = enum_type_wrapper.EnumTypeWrapper(_SEXTYPE)
-_OWNERINROOM = DESCRIPTOR.enum_types_by_name['OwnerInRoom']
-OwnerInRoom = enum_type_wrapper.EnumTypeWrapper(_OWNERINROOM)
-_SCENETYPE = DESCRIPTOR.enum_types_by_name['SceneType']
-SceneType = enum_type_wrapper.EnumTypeWrapper(_SCENETYPE)
-_ROOMADMINTYPE = DESCRIPTOR.enum_types_by_name['RoomAdminType']
-RoomAdminType = enum_type_wrapper.EnumTypeWrapper(_ROOMADMINTYPE)
-_DEVICETYPE = DESCRIPTOR.enum_types_by_name['DeviceType']
-DeviceType = enum_type_wrapper.EnumTypeWrapper(_DEVICETYPE)
-_PLAYERFLAGS = DESCRIPTOR.enum_types_by_name['PlayerFlags']
-PlayerFlags = enum_type_wrapper.EnumTypeWrapper(_PLAYERFLAGS)
-_ACCOUNTFLAGS = DESCRIPTOR.enum_types_by_name['AccountFlags']
-AccountFlags = enum_type_wrapper.EnumTypeWrapper(_ACCOUNTFLAGS)
-_ONOFFTYPE = DESCRIPTOR.enum_types_by_name['OnOffType']
-OnOffType = enum_type_wrapper.EnumTypeWrapper(_ONOFFTYPE)
-_STATUSCODE = DESCRIPTOR.enum_types_by_name['StatusCode']
-StatusCode = enum_type_wrapper.EnumTypeWrapper(_STATUSCODE)
-_EFFECTTYPE = DESCRIPTOR.enum_types_by_name['EffectType']
-EffectType = enum_type_wrapper.EnumTypeWrapper(_EFFECTTYPE)
-_EFFECTTIMETYPE = DESCRIPTOR.enum_types_by_name['EffectTimeType']
-EffectTimeType = enum_type_wrapper.EnumTypeWrapper(_EFFECTTIMETYPE)
-_EFFECTUSESTATUS = DESCRIPTOR.enum_types_by_name['EffectUseStatus']
-EffectUseStatus = enum_type_wrapper.EnumTypeWrapper(_EFFECTUSESTATUS)
-_EFFECTNOTICETYPE = DESCRIPTOR.enum_types_by_name['EffectNoticeType']
-EffectNoticeType = enum_type_wrapper.EnumTypeWrapper(_EFFECTNOTICETYPE)
-_MODELONOFFSTATUS = DESCRIPTOR.enum_types_by_name['ModelOnOffStatus']
-ModelOnOffStatus = enum_type_wrapper.EnumTypeWrapper(_MODELONOFFSTATUS)
-_RANKTYPE = DESCRIPTOR.enum_types_by_name['RankType']
-RankType = enum_type_wrapper.EnumTypeWrapper(_RANKTYPE)
-_LOADCLICKTYPE = DESCRIPTOR.enum_types_by_name['LoadClickType']
-LoadClickType = enum_type_wrapper.EnumTypeWrapper(_LOADCLICKTYPE)
-_AUDITSTATUS = DESCRIPTOR.enum_types_by_name['AuditStatus']
-AuditStatus = enum_type_wrapper.EnumTypeWrapper(_AUDITSTATUS)
-_UPLOADTYPE = DESCRIPTOR.enum_types_by_name['UploadType']
-UploadType = enum_type_wrapper.EnumTypeWrapper(_UPLOADTYPE)
-_PAYCHANNELTYPE = DESCRIPTOR.enum_types_by_name['PayChannelType']
-PayChannelType = enum_type_wrapper.EnumTypeWrapper(_PAYCHANNELTYPE)
-_ROLE = DESCRIPTOR.enum_types_by_name['Role']
-Role = enum_type_wrapper.EnumTypeWrapper(_ROLE)
-_NAMEPLATESTYLE = DESCRIPTOR.enum_types_by_name['NameplateStyle']
-NameplateStyle = enum_type_wrapper.EnumTypeWrapper(_NAMEPLATESTYLE)
-_PLAYERRESOURCETYPE = DESCRIPTOR.enum_types_by_name['PlayerResourceType']
-PlayerResourceType = enum_type_wrapper.EnumTypeWrapper(_PLAYERRESOURCETYPE)
-_ATTITUDEDEGREESSTATUSTYPE = DESCRIPTOR.enum_types_by_name['AttitudeDegreesStatusType']
-AttitudeDegreesStatusType = enum_type_wrapper.EnumTypeWrapper(_ATTITUDEDEGREESSTATUSTYPE)
-_CMEDIATYPE = DESCRIPTOR.enum_types_by_name['CMediaType']
-CMediaType = enum_type_wrapper.EnumTypeWrapper(_CMEDIATYPE)
-_DEVICECONNECTOPER = DESCRIPTOR.enum_types_by_name['DeviceConnectOper']
-DeviceConnectOper = enum_type_wrapper.EnumTypeWrapper(_DEVICECONNECTOPER)
-_DEVICECMDID = DESCRIPTOR.enum_types_by_name['DeviceCmdId']
-DeviceCmdId = enum_type_wrapper.EnumTypeWrapper(_DEVICECMDID)
-_TASKSTATUS = DESCRIPTOR.enum_types_by_name['TaskStatus']
-TaskStatus = enum_type_wrapper.EnumTypeWrapper(_TASKSTATUS)
-_TASKTYPE = DESCRIPTOR.enum_types_by_name['TaskType']
-TaskType = enum_type_wrapper.EnumTypeWrapper(_TASKTYPE)
-_LABELTYPE = DESCRIPTOR.enum_types_by_name['LabelType']
-LabelType = enum_type_wrapper.EnumTypeWrapper(_LABELTYPE)
-_AIGCTYPE = DESCRIPTOR.enum_types_by_name['AigcType']
-AigcType = enum_type_wrapper.EnumTypeWrapper(_AIGCTYPE)
-_MODULE = DESCRIPTOR.enum_types_by_name['Module']
-Module = enum_type_wrapper.EnumTypeWrapper(_MODULE)
-_WIDGETTYPE = DESCRIPTOR.enum_types_by_name['WidgetType']
-WidgetType = enum_type_wrapper.EnumTypeWrapper(_WIDGETTYPE)
-_CALCULATEMODE = DESCRIPTOR.enum_types_by_name['CalculateMode']
-CalculateMode = enum_type_wrapper.EnumTypeWrapper(_CALCULATEMODE)
-_CHARGECATETYPE = DESCRIPTOR.enum_types_by_name['ChargeCateType']
-ChargeCateType = enum_type_wrapper.EnumTypeWrapper(_CHARGECATETYPE)
-ErrCodeNone = 0
-ErrCodeRedis = 10001
-ErrCodeMysql = 10002
-ErrCodeFrequency = 10003
-ErrCodeParam = 10004
-ErrCodeNoMatchObj = 10005
-ErrCodeBusy = 10006
-ErrCodeMaintain = 16666
-UNKNOWN = 0
-MALE = 1
-FEMALE = 2
-NotInSelfRoom = 0
-InSelfRoom = 1
-ST_ZERO = 0
-ST_HOME = 1
-RAT_GUEST = 0
-RAT_NORMAL = 10
-RAT_ADMIN = 20
-RAT_OWNER = 30
-RAT_SUPER_ADMIN = 40
-RAT_BLACK = -5
-DT_UNKNOWN = 0
-DT_FLASHPLAYER = 1
-DT_ANDROID_PHONE = 20
-DT_IOS_PHONE = 40
-DT_WINDOWS_ASSISTANT = 80
-DT_WINDOWS_PC = 90
-DT_ROBOT = 100
-DT_WECHAT_SUBSCRIPTION = 110
-DT_QQ_SMALL_PROGRAM = 120
-DT_WX_MINI_PROGRAM = 130
-DT_WEB = 140
-DT_MAC = 150
-PF_ZERO = 0
-PF_CERTIFICATION = 1
-PF_BIND_BANK = 4
-PF_INVITE = 5
-PF_CHARGE_FIRST = 12
-PF_ATTITUDE_QUESTION = 13
-PF_END_REGISTRATION = 14
-AF_ZERO = 0
-AF_PHONE_VERIFIED = 1
-YEAR_BAG = 0
-CRACK_EGG = 1
-GOOGLE_PAY = 5
-IAP_PAY = 6
-INVITE = 7
-INDEX_CATEGORY = 8
-CERTIF = 9
-GUARD = 10
-LOTTERY_DRAW = 12
-MENTOR_SHIP = 13
-CERTIF_IOS = 14
-REAL_IDENTITY = 15
-NOVICE_GIFT = 16
-ROOM_SET_MODEL = 18
-ACTIVITY_TYPE = 20
-ACTIVITY = 21
-HOT_SONG = 23
-ROOM_ENTER = 34
-ROOM_PATTERN_HIGH_QUALITY = 35
-AUTH_LOGIN_UI = 38
-USER_DATA_EDIT = 41
-CERTIFICATION = 43
-CERTIFICATION_ROOM_SHOW = 44
-CERTIFICATION_ROOM_WIN_OPEN_CLOSE = 45
-CERTIFY_WORD = 46
-CERTIFY_CHAIR = 47
-CERTIFY_UPDATE_USER_INFO = 48
-CERTIFY_BROADCAST_FRIEND = 49
-CERTIFY_HEAD_LINE = 50
-CERTIFY_TIAO_TIAO = 51
-LOGIN_BIND_PHONE = 52
-CERTIFY_OWNER_ENTER_ROOM = 53
-Young_Model = 58
-CUSTOMER_SERVICE = 59
-OVERSEAS_IP_LIMIT = 66
-OLD_NAME_LIMIT = 67
-CRACK_SELF_MSG = 68
-ORDER_LOCATION = 71
-DELETE_ACCOUNT = 73
-YUNPIAN_SMS = 74
-BIND_PHONE_V2 = 75
-BIND_PHONE_LOGIN = 76
-COUNT_DOWN = 78
-OXYGEN_BAR = 94
-PRIVACY_SETTING = 95
-OXYGEN_BAR_CLAN_MEMBER_ONLY = 96
-OXYGEN_BAR_TREND_GIF = 97
-DATA_AUDIT = 98
-Inner_Tec = 100
-Inner_Ali = 101
-CERTIFY_IM_PICTURE = 103
-CMB_VIP = 104
-CRACKEGG_FOREST = 105
-ANTI_ADDICTION = 200
-TEXT_FILTER_ROOM_SCREEN_ENCRYPTED = 201
-TEXT_FILTER_ROOM_SCREEN_UNENCRYPTED = 202
-TEXT_FILTER_BROADCAST_FRIEND = 203
-TEXT_FILTER_PRIVATE_CHAT = 204
-BC_HEAD_LINE = 110
-ONE_CLICK_LOGIN = 111
-CERTIFY_PM = 112
-CERTIFY_PICTURE = 113
-CHANNEL_ADVERT_AUDITS = 114
-CERTIFY_CREATE_CHANNEL = 116
-CERTIFY_JOIN_CHANNEL = 117
-CERTIFY_GIVE = 118
-CERTIFY_ROOM_NOTICE = 119
-CERTIFY_RECHARGE = 120
-CERTIFY_PUBLISH_TREND = 121
-CERTIFY_COMMENT_TREND = 122
-HOME_NAV_TYPE = 123
-LOGIN_CHECKED = 124
-HIGH_SOUND = 125
-HIGH_SOUND_CHANNEL = 126
-CHANNEL_STAR_CHALLENGE = 127
-CHANNEL_STAT = 128
-REGISTER_SEX = 130
-REGISTER_NICKNAME = 131
-REGISTER_ATTITUDE = 132
-CREATE_CHANNEL = 133
-COMMUNITY_TREND_AUDIO = 134
-IM_TIPS = 135
-MULTI_CLIENT_ONLINE = 253
-SC_FAIL = 0
-SC_SUCCESS = 1
-EffectTypeNone = 0
-EffectTypeNicknamePendant = 1
-EffectTimeTypeAlways = 0
-EffectTimeTypeMike = 1
-EffectTimeTypeWearInPacket = 2
-EffectTimeTypePermanent = 3
-ES_Use = 0
-ES_NotUse = 1
-EffectNoticeTypeGain = 0
-EffectNoticeTypeTimeout = 1
-ALL_OFF = 0
-ALL_ON = 1
-WHITELIST = 2
-RT_ZERO = 0
-RT_CHARM = 1
-RT_WEALTH = 2
-RT_GIFT = 3
-LCT_ZERO = 0
-LCT_INTIMATE_DETAIL = 1
-LCT_INTIMATE_STORE = 2
-AS_Audit_Pass = 0
-AS_Auditing = 1
-AS_Audit_Refuse = 2
-TypeZero = 0
-HeadAlbumImg = 1
-HeadIconImg = 2
-DynamicsImg = 3
-ClientLog = 4
-TipOffsImg = 5
-Indetity = 6
-PMMedia = 7
-Voice = 8
-BackgroundImg = 23
-ChannelIcon = 24
-WXRobotQRcode = 25
-CommunityTagImg = 28
-PersonLabelImg = 29
-PCT_NULL = 0
-PCT_ALIPAY_H5 = 2
-PCT_ALIPAY_APP = 3
-PCT_WXPAY_APP = 4
-PCT_WXPAY_H5 = 5
-PCT_IAP = 6
-PCT_PLAY = 8
-PCT_PAYPAL = 10
-PCT_BOING = 11
-PCT_UNIONPAY = 12
-PCT_AGENT = 253
-PCT_MANUAL = 254
-PCT_DEVTEST = 255
-R_NONE = 0
-R_SUPERUSER = 1
-R_OW = 2
-R_VP = 3
-R_MA = 4
-R_CA1 = 5
-R_CA2 = 6
-R_R = 7
-R_U = 8
-NS_NONE = 0
-NS_STYLE_1 = 1
-NS_STYLE_2 = 2
-NS_STYLE_3 = 3
-NS_STYLE_4 = 4
-PRT_NONE = 0
-PRT_FIRST_ACCOUNT = 1
-PRT_WX = 2
-ADST_BOTH_EVERY = 0
-ADST_OPPOSITE_EVERY = 1
-ADST_OPPOSITE_NOTENOUGH = 2
-CMediaType_None = 0
-CMediaType_Png = 1
-CMediaType_Gif = 2
-CMediaType_Video = 3
-CMediaType_Audio = 4
-DCS_None = 0
-DCS_Requesting = 1
-DCS_Receive = 2
-DCS_Refuse = 3
-DCS_Timeout = 4
-DCS_Cancel = 5
-DC_DeviceZero = 0
-DC_DeviceLogin = 511001
-DC_MessageConnectOperate = 511002
-DC_MessageStatusUpdate = 511003
-DC_DeviceShareStatus = 511004
-DC_SingoConnect = 611001
-TS_None = 0
-TS_Processing = 1
-TS_Success = 2
-TS_Failure = 3
-TT_None = 0
-TT_Image = 1
-TT_Video = 2
-TT_Audio = 3
-TT_Text = 4
-LT_NONE = 0
-LT_POST = 1
-LT_Gallery = 2
-LT_Group = 3
-LT_Comment = 4
-LT_Lora = 5
-LT_Client = 6
-AT_NONE = 0
-AT_IMAGE = 1
-AT_VIDEO = 2
-AT_AUDIO = 3
-AT_TEXT = 4
-M_None = 0
-M_Subscribe = 1
-WT_None = 0
-WT_General = 1
-WT_SD = 2
-WT_Lora = 3
-CM_None = 0
-CM_Single = 1
-CM_Minute = 2
-CCT_Normal = 0
-CCT_ActCard = 1
-
-
-_PLAYER = DESCRIPTOR.message_types_by_name['Player']
-_USERINFO = DESCRIPTOR.message_types_by_name['UserInfo']
-_PLAYERINFO = DESCRIPTOR.message_types_by_name['PlayerInfo']
-_BAGITEM = DESCRIPTOR.message_types_by_name['BagItem']
-_AGODAKEY = DESCRIPTOR.message_types_by_name['AgodaKey']
-_ONOFFSTATUS = DESCRIPTOR.message_types_by_name['OnOffStatus']
-_SEARCHPLAYERENTRY = DESCRIPTOR.message_types_by_name['SearchPlayerEntry']
-_EFFECTINFO = DESCRIPTOR.message_types_by_name['EffectInfo']
-_EFFECT = DESCRIPTOR.message_types_by_name['Effect']
-_EFFECTCONFIG = DESCRIPTOR.message_types_by_name['EffectConfig']
-_EFFECTNICKNAMEPENDANT = DESCRIPTOR.message_types_by_name['EffectNicknamePendant']
-_EFFECTSERCONF = DESCRIPTOR.message_types_by_name['EffectSerConf']
-_INDEXTIPROOMS = DESCRIPTOR.message_types_by_name['IndexTipRooms']
-_REGISID = DESCRIPTOR.message_types_by_name['RegisId']
-_MODELONOFF = DESCRIPTOR.message_types_by_name['ModelOnOff']
-_RANK = DESCRIPTOR.message_types_by_name['Rank']
-_PLAYERCHAIRROOM = DESCRIPTOR.message_types_by_name['PlayerChairRoom']
-_CLANINFO = DESCRIPTOR.message_types_by_name['ClanInfo']
-_PERIOD = DESCRIPTOR.message_types_by_name['Period']
-_LABELINFO = DESCRIPTOR.message_types_by_name['LabelInfo']
-_PLAYERRESOURCESHORT = DESCRIPTOR.message_types_by_name['PlayerResourceShort']
-_PLAYERRESOURCE = DESCRIPTOR.message_types_by_name['PlayerResource']
-_PLAYERRESOURCEWITHSCORE = DESCRIPTOR.message_types_by_name['PlayerResourceWithScore']
-_ATTITUDEDEGREESINFO = DESCRIPTOR.message_types_by_name['AttitudeDegreesInfo']
-_ATTITUDECATEGORYDEGREESINFO = DESCRIPTOR.message_types_by_name['AttitudeCategoryDegreesInfo']
-_CMEDIARESOURCE = DESCRIPTOR.message_types_by_name['CMediaResource']
-_SAYHELLOREQ = DESCRIPTOR.message_types_by_name['SayHelloReq']
-_SAYHELLORES = DESCRIPTOR.message_types_by_name['SayHelloRes']
-_HEARTBEATREQ = DESCRIPTOR.message_types_by_name['HeartbeatReq']
-_HEARTBEATRES = DESCRIPTOR.message_types_by_name['HeartbeatRes']
-Player = _reflection.GeneratedProtocolMessageType('Player', (_message.Message,), {
-  'DESCRIPTOR' : _PLAYER,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.Player)
-  })
-_sym_db.RegisterMessage(Player)
-
-UserInfo = _reflection.GeneratedProtocolMessageType('UserInfo', (_message.Message,), {
-  'DESCRIPTOR' : _USERINFO,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UserInfo)
-  })
-_sym_db.RegisterMessage(UserInfo)
-
-PlayerInfo = _reflection.GeneratedProtocolMessageType('PlayerInfo', (_message.Message,), {
-  'DESCRIPTOR' : _PLAYERINFO,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.PlayerInfo)
-  })
-_sym_db.RegisterMessage(PlayerInfo)
-
-BagItem = _reflection.GeneratedProtocolMessageType('BagItem', (_message.Message,), {
-  'DESCRIPTOR' : _BAGITEM,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.BagItem)
-  })
-_sym_db.RegisterMessage(BagItem)
-
-AgodaKey = _reflection.GeneratedProtocolMessageType('AgodaKey', (_message.Message,), {
-  'DESCRIPTOR' : _AGODAKEY,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AgodaKey)
-  })
-_sym_db.RegisterMessage(AgodaKey)
-
-OnOffStatus = _reflection.GeneratedProtocolMessageType('OnOffStatus', (_message.Message,), {
-  'DESCRIPTOR' : _ONOFFSTATUS,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.OnOffStatus)
-  })
-_sym_db.RegisterMessage(OnOffStatus)
-
-SearchPlayerEntry = _reflection.GeneratedProtocolMessageType('SearchPlayerEntry', (_message.Message,), {
-  'DESCRIPTOR' : _SEARCHPLAYERENTRY,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.SearchPlayerEntry)
-  })
-_sym_db.RegisterMessage(SearchPlayerEntry)
-
-EffectInfo = _reflection.GeneratedProtocolMessageType('EffectInfo', (_message.Message,), {
-  'DESCRIPTOR' : _EFFECTINFO,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.EffectInfo)
-  })
-_sym_db.RegisterMessage(EffectInfo)
-
-Effect = _reflection.GeneratedProtocolMessageType('Effect', (_message.Message,), {
-  'DESCRIPTOR' : _EFFECT,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.Effect)
-  })
-_sym_db.RegisterMessage(Effect)
-
-EffectConfig = _reflection.GeneratedProtocolMessageType('EffectConfig', (_message.Message,), {
-  'DESCRIPTOR' : _EFFECTCONFIG,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.EffectConfig)
-  })
-_sym_db.RegisterMessage(EffectConfig)
-
-EffectNicknamePendant = _reflection.GeneratedProtocolMessageType('EffectNicknamePendant', (_message.Message,), {
-  'DESCRIPTOR' : _EFFECTNICKNAMEPENDANT,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.EffectNicknamePendant)
-  })
-_sym_db.RegisterMessage(EffectNicknamePendant)
-
-EffectSerConf = _reflection.GeneratedProtocolMessageType('EffectSerConf', (_message.Message,), {
-  'DESCRIPTOR' : _EFFECTSERCONF,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.EffectSerConf)
-  })
-_sym_db.RegisterMessage(EffectSerConf)
-
-IndexTipRooms = _reflection.GeneratedProtocolMessageType('IndexTipRooms', (_message.Message,), {
-  'DESCRIPTOR' : _INDEXTIPROOMS,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.IndexTipRooms)
-  })
-_sym_db.RegisterMessage(IndexTipRooms)
-
-RegisId = _reflection.GeneratedProtocolMessageType('RegisId', (_message.Message,), {
-  'DESCRIPTOR' : _REGISID,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.RegisId)
-  })
-_sym_db.RegisterMessage(RegisId)
-
-ModelOnOff = _reflection.GeneratedProtocolMessageType('ModelOnOff', (_message.Message,), {
-  'DESCRIPTOR' : _MODELONOFF,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.ModelOnOff)
-  })
-_sym_db.RegisterMessage(ModelOnOff)
-
-Rank = _reflection.GeneratedProtocolMessageType('Rank', (_message.Message,), {
-  'DESCRIPTOR' : _RANK,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.Rank)
-  })
-_sym_db.RegisterMessage(Rank)
-
-PlayerChairRoom = _reflection.GeneratedProtocolMessageType('PlayerChairRoom', (_message.Message,), {
-  'DESCRIPTOR' : _PLAYERCHAIRROOM,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.PlayerChairRoom)
-  })
-_sym_db.RegisterMessage(PlayerChairRoom)
-
-ClanInfo = _reflection.GeneratedProtocolMessageType('ClanInfo', (_message.Message,), {
-  'DESCRIPTOR' : _CLANINFO,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.ClanInfo)
-  })
-_sym_db.RegisterMessage(ClanInfo)
-
-Period = _reflection.GeneratedProtocolMessageType('Period', (_message.Message,), {
-  'DESCRIPTOR' : _PERIOD,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.Period)
-  })
-_sym_db.RegisterMessage(Period)
-
-LabelInfo = _reflection.GeneratedProtocolMessageType('LabelInfo', (_message.Message,), {
-  'DESCRIPTOR' : _LABELINFO,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.LabelInfo)
-  })
-_sym_db.RegisterMessage(LabelInfo)
-
-PlayerResourceShort = _reflection.GeneratedProtocolMessageType('PlayerResourceShort', (_message.Message,), {
-  'DESCRIPTOR' : _PLAYERRESOURCESHORT,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.PlayerResourceShort)
-  })
-_sym_db.RegisterMessage(PlayerResourceShort)
-
-PlayerResource = _reflection.GeneratedProtocolMessageType('PlayerResource', (_message.Message,), {
-  'DESCRIPTOR' : _PLAYERRESOURCE,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.PlayerResource)
-  })
-_sym_db.RegisterMessage(PlayerResource)
-
-PlayerResourceWithScore = _reflection.GeneratedProtocolMessageType('PlayerResourceWithScore', (_message.Message,), {
-  'DESCRIPTOR' : _PLAYERRESOURCEWITHSCORE,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.PlayerResourceWithScore)
-  })
-_sym_db.RegisterMessage(PlayerResourceWithScore)
-
-AttitudeDegreesInfo = _reflection.GeneratedProtocolMessageType('AttitudeDegreesInfo', (_message.Message,), {
-  'DESCRIPTOR' : _ATTITUDEDEGREESINFO,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AttitudeDegreesInfo)
-  })
-_sym_db.RegisterMessage(AttitudeDegreesInfo)
-
-AttitudeCategoryDegreesInfo = _reflection.GeneratedProtocolMessageType('AttitudeCategoryDegreesInfo', (_message.Message,), {
-  'DESCRIPTOR' : _ATTITUDECATEGORYDEGREESINFO,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.AttitudeCategoryDegreesInfo)
-  })
-_sym_db.RegisterMessage(AttitudeCategoryDegreesInfo)
-
-CMediaResource = _reflection.GeneratedProtocolMessageType('CMediaResource', (_message.Message,), {
-  'DESCRIPTOR' : _CMEDIARESOURCE,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.CMediaResource)
-  })
-_sym_db.RegisterMessage(CMediaResource)
-
-SayHelloReq = _reflection.GeneratedProtocolMessageType('SayHelloReq', (_message.Message,), {
-  'DESCRIPTOR' : _SAYHELLOREQ,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.SayHelloReq)
-  })
-_sym_db.RegisterMessage(SayHelloReq)
-
-SayHelloRes = _reflection.GeneratedProtocolMessageType('SayHelloRes', (_message.Message,), {
-  'DESCRIPTOR' : _SAYHELLORES,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.SayHelloRes)
-  })
-_sym_db.RegisterMessage(SayHelloRes)
-
-HeartbeatReq = _reflection.GeneratedProtocolMessageType('HeartbeatReq', (_message.Message,), {
-  'DESCRIPTOR' : _HEARTBEATREQ,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.HeartbeatReq)
-  })
-_sym_db.RegisterMessage(HeartbeatReq)
-
-HeartbeatRes = _reflection.GeneratedProtocolMessageType('HeartbeatRes', (_message.Message,), {
-  'DESCRIPTOR' : _HEARTBEATRES,
-  '__module__' : 'common_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.HeartbeatRes)
-  })
-_sym_db.RegisterMessage(HeartbeatRes)
-
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\242\002\003PB3'
-  _COMMONERR._serialized_start=3470
-  _COMMONERR._serialized_end=3643
-  _SEXTYPE._serialized_start=3645
-  _SEXTYPE._serialized_end=3689
-  _OWNERINROOM._serialized_start=3691
-  _OWNERINROOM._serialized_end=3739
-  _SCENETYPE._serialized_start=3741
-  _SCENETYPE._serialized_end=3778
-  _ROOMADMINTYPE._serialized_start=3780
-  _ROOMADMINTYPE._serialized_end=3901
-  _DEVICETYPE._serialized_start=3904
-  _DEVICETYPE._serialized_end=4155
-  _PLAYERFLAGS._serialized_start=4158
-  _PLAYERFLAGS._serialized_end=4311
-  _ACCOUNTFLAGS._serialized_start=4313
-  _ACCOUNTFLAGS._serialized_end=4363
-  _ONOFFTYPE._serialized_start=4366
-  _ONOFFTYPE._serialized_end=6154
-  _STATUSCODE._serialized_start=6156
-  _STATUSCODE._serialized_end=6197
-  _EFFECTTYPE._serialized_start=6199
-  _EFFECTTYPE._serialized_end=6262
-  _EFFECTTIMETYPE._serialized_start=6264
-  _EFFECTTIMETYPE._serialized_end=6391
-  _EFFECTUSESTATUS._serialized_start=6393
-  _EFFECTUSESTATUS._serialized_end=6437
-  _EFFECTNOTICETYPE._serialized_start=6439
-  _EFFECTNOTICETYPE._serialized_end=6512
-  _MODELONOFFSTATUS._serialized_start=6514
-  _MODELONOFFSTATUS._serialized_end=6572
-  _RANKTYPE._serialized_start=6574
-  _RANKTYPE._serialized_end=6639
-  _LOADCLICKTYPE._serialized_start=6641
-  _LOADCLICKTYPE._serialized_end=6719
-  _AUDITSTATUS._serialized_start=6721
-  _AUDITSTATUS._serialized_end=6791
-  _UPLOADTYPE._serialized_start=6794
-  _UPLOADTYPE._serialized_end=7037
-  _PAYCHANNELTYPE._serialized_start=7040
-  _PAYCHANNELTYPE._serialized_end=7273
-  _ROLE._serialized_start=7275
-  _ROLE._serialized_end=7380
-  _NAMEPLATESTYLE._serialized_start=7382
-  _NAMEPLATESTYLE._serialized_end=7475
-  _PLAYERRESOURCETYPE._serialized_start=7477
-  _PLAYERRESOURCETYPE._serialized_end=7546
-  _ATTITUDEDEGREESSTATUSTYPE._serialized_start=7548
-  _ATTITUDEDEGREESSTATUSTYPE._serialized_end=7650
-  _CMEDIATYPE._serialized_start=7652
-  _CMEDIATYPE._serialized_end=7769
-  _DEVICECONNECTOPER._serialized_start=7771
-  _DEVICECONNECTOPER._serialized_end=7890
-  _DEVICECMDID._serialized_start=7893
-  _DEVICECMDID._serialized_end=8060
-  _TASKSTATUS._serialized_start=8062
-  _TASKSTATUS._serialized_end=8138
-  _TASKTYPE._serialized_start=8140
-  _TASKTYPE._serialized_end=8218
-  _LABELTYPE._serialized_start=8220
-  _LABELTYPE._serialized_end=8331
-  _AIGCTYPE._serialized_start=8333
-  _AIGCTYPE._serialized_end=8411
-  _MODULE._serialized_start=8413
-  _MODULE._serialized_end=8450
-  _WIDGETTYPE._serialized_start=8452
-  _WIDGETTYPE._serialized_end=8517
-  _CALCULATEMODE._serialized_start=8519
-  _CALCULATEMODE._serialized_end=8577
-  _CHARGECATETYPE._serialized_start=8579
-  _CHARGECATETYPE._serialized_end=8628
-  _PLAYER._serialized_start=25
-  _PLAYER._serialized_end=400
-  _USERINFO._serialized_start=403
-  _USERINFO._serialized_end=532
-  _PLAYERINFO._serialized_start=535
-  _PLAYERINFO._serialized_end=878
-  _BAGITEM._serialized_start=880
-  _BAGITEM._serialized_end=941
-  _AGODAKEY._serialized_start=943
-  _AGODAKEY._serialized_end=977
-  _ONOFFSTATUS._serialized_start=979
-  _ONOFFSTATUS._serialized_end=1037
-  _SEARCHPLAYERENTRY._serialized_start=1040
-  _SEARCHPLAYERENTRY._serialized_end=1288
-  _EFFECTINFO._serialized_start=1291
-  _EFFECTINFO._serialized_end=1450
-  _EFFECT._serialized_start=1453
-  _EFFECT._serialized_end=1628
-  _EFFECTCONFIG._serialized_start=1630
-  _EFFECTCONFIG._serialized_end=1714
-  _EFFECTNICKNAMEPENDANT._serialized_start=1716
-  _EFFECTNICKNAMEPENDANT._serialized_end=1770
-  _EFFECTSERCONF._serialized_start=1772
-  _EFFECTSERCONF._serialized_end=1843
-  _INDEXTIPROOMS._serialized_start=1845
-  _INDEXTIPROOMS._serialized_end=1893
-  _REGISID._serialized_start=1895
-  _REGISID._serialized_end=1956
-  _MODELONOFF._serialized_start=1958
-  _MODELONOFF._serialized_end=2038
-  _RANK._serialized_start=2041
-  _RANK._serialized_end=2249
-  _PLAYERCHAIRROOM._serialized_start=2251
-  _PLAYERCHAIRROOM._serialized_end=2304
-  _CLANINFO._serialized_start=2306
-  _CLANINFO._serialized_end=2414
-  _PERIOD._serialized_start=2416
-  _PERIOD._serialized_end=2458
-  _LABELINFO._serialized_start=2460
-  _LABELINFO._serialized_end=2504
-  _PLAYERRESOURCESHORT._serialized_start=2506
-  _PLAYERRESOURCESHORT._serialized_end=2595
-  _PLAYERRESOURCE._serialized_start=2598
-  _PLAYERRESOURCE._serialized_end=2748
-  _PLAYERRESOURCEWITHSCORE._serialized_start=2750
-  _PLAYERRESOURCEWITHSCORE._serialized_end=2849
-  _ATTITUDEDEGREESINFO._serialized_start=2852
-  _ATTITUDEDEGREESINFO._serialized_end=3032
-  _ATTITUDECATEGORYDEGREESINFO._serialized_start=3034
-  _ATTITUDECATEGORYDEGREESINFO._serialized_end=3137
-  _CMEDIARESOURCE._serialized_start=3140
-  _CMEDIARESOURCE._serialized_end=3273
-  _SAYHELLOREQ._serialized_start=3275
-  _SAYHELLOREQ._serialized_end=3302
-  _SAYHELLORES._serialized_start=3304
-  _SAYHELLORES._serialized_end=3332
-  _HEARTBEATREQ._serialized_start=3334
-  _HEARTBEATREQ._serialized_end=3432
-  _HEARTBEATRES._serialized_start=3434
-  _HEARTBEATRES._serialized_end=3467
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: common_ext.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import enum_type_wrapper
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63ommon_ext.proto\x12\x02pb\"\xf7\x02\n\x06Player\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x10\n\x08nickname\x18\x02 \x01(\t\x12\x18\n\x03sex\x18\x03 \x01(\x0e\x32\x0b.pb.SexType\x12\x0b\n\x03id2\x18\x04 \x01(\x03\x12\x0c\n\x04icon\x18\x05 \x01(\t\x12\r\n\x05\x66lags\x18\x06 \x01(\x03\x12\r\n\x05\x63harm\x18\x08 \x01(\x03\x12\x13\n\x0b\x63harm_level\x18\t \x01(\x05\x12\x14\n\x0cwealth_level\x18\n \x01(\x05\x12\x0e\n\x06wealth\x18\x0b \x01(\x03\x12\x12\n\nonline_exp\x18\x0c \x01(\r\x12\x11\n\tcreate_at\x18\r \x01(\r\x12\x11\n\tis_delete\x18\x0e \x01(\x08\x12\r\n\x05point\x18\x0f \x01(\x03\x12\x13\n\x0bpoint_level\x18\x10 \x01(\x05\x12\x11\n\tsignature\x18\x11 \x01(\t\x12\x0c\n\x04\x63ity\x18\x12 \x01(\t\x12\x10\n\x08\x62irthday\x18\x13 \x01(\t\x12\x14\n\x0conline_state\x18\x14 \x01(\x05\x12\x1a\n\x12NicknameUpdateTime\x18\x15 \x01(\r\"\x81\x01\n\x08UserInfo\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0c\n\x04\x63ity\x18\x02 \x01(\t\x12\x11\n\tsignature\x18\x03 \x01(\t\x12\x0c\n\x04mind\x18\x04 \x01(\t\x12\x10\n\x08\x62irthday\x18\x05 \x01(\t\x12\x15\n\rintimate_slot\x18\x06 \x01(\x11\x12\x11\n\tnameplate\x18\x07 \x01(\t\"\xd7\x02\n\nPlayerInfo\x12\x1a\n\x06player\x18\x01 \x01(\x0b\x32\n.pb.Player\x12\x1a\n\x06\x65\x66\x66\x65\x63t\x18\x02 \x03(\x0b\x32\n.pb.Effect\x12\x1a\n\x04\x63lan\x18\x03 \x01(\x0b\x32\x0c.pb.ClanInfo\x12\x10\n\x08\x66\x61ns_num\x18\x04 \x01(\x05\x12\x15\n\rfollowing_num\x18\x05 \x01(\x05\x12\x14\n\x0c\x66riend_alias\x18\x06 \x01(\t\x12\x1f\n\x07\x65\x66\x66\x65\x63ts\x18\x07 \x03(\x0b\x32\x0e.pb.EffectInfo\x12\x18\n\x10\x61ttitude_yes_num\x18\x08 \x01(\x03\x12\x17\n\x0ftotal_visit_num\x18\t \x01(\x03\x12\x15\n\radd_visit_num\x18\n \x01(\x03\x12\x1c\n\x05label\x18\x0b \x03(\x0b\x32\r.pb.LabelInfo\x12-\n\x0c\x64\x65grees_info\x18\x0c \x01(\x0b\x32\x17.pb.AttitudeDegreesInfo\"=\n\x07\x42\x61gItem\x12\x0f\n\x07gift_id\x18\x01 \x01(\r\x12\x0e\n\x06\x61mount\x18\x02 \x01(\r\x12\x11\n\tcteate_at\x18\x03 \x01(\t\"\"\n\x08\x41godaKey\x12\x16\n\x0epermission_key\x18\x01 \x01(\t\":\n\x0bOnOffStatus\x12\x0e\n\x06status\x18\x01 \x01(\x11\x12\x1b\n\x04type\x18\x02 \x01(\x0e\x32\r.pb.OnOffType\"\xf8\x01\n\x11SearchPlayerEntry\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0b\n\x03id2\x18\x02 \x01(\x12\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x18\n\x03sex\x18\x04 \x01(\x0e\x32\x0b.pb.SexType\x12\x0c\n\x04icon\x18\x05 \x01(\t\x12\r\n\x05\x63harm\x18\x06 \x01(\x12\x12\x13\n\x0b\x63harm_level\x18\x07 \x01(\x11\x12\x0e\n\x06wealth\x18\x08 \x01(\x12\x12\x14\n\x0cwealth_level\x18\t \x01(\x11\x12\x0e\n\x06online\x18\n \x01(\x08\x12\x0f\n\x07room_id\x18\x0b \x01(\x12\x12\x12\n\nhas_passwd\x18\r \x01(\x08\x12\x11\n\tsignature\x18\x0e \x01(\t\"\x9f\x01\n\nEffectInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12%\n\ttime_type\x18\x02 \x01(\x0e\x32\x12.pb.EffectTimeType\x12\x10\n\x08\x65nd_time\x18\x03 \x01(\x03\x12\'\n\nuse_status\x18\x04 \x01(\x0e\x32\x13.pb.EffectUseStatus\x12#\n\x0b\x65\x66\x66\x65\x63t_type\x18\x05 \x01(\x0e\x32\x0e.pb.EffectType\"\xaf\x01\n\x06\x45\x66\x66\x65\x63t\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04\x66lag\x18\x02 \x01(\x05\x12\x0b\n\x03str\x18\x03 \x01(\t\x12%\n\ttime_type\x18\x04 \x01(\x0e\x32\x12.pb.EffectTimeType\x12\x10\n\x08\x65nd_time\x18\x05 \x01(\x05\x12\'\n\nuse_status\x18\x06 \x01(\x0e\x32\x13.pb.EffectUseStatus\x12\x1c\n\x04type\x18\x07 \x01(\x0e\x32\x0e.pb.EffectType\"T\n\x0c\x45\x66\x66\x65\x63tConfig\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x1c\n\x04type\x18\x02 \x01(\x0e\x32\x0e.pb.EffectType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\"6\n\x15\x45\x66\x66\x65\x63tNicknamePendant\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x10\n\x08show_url\x18\x02 \x01(\t\"G\n\rEffectSerConf\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x1c\n\x04type\x18\x02 \x01(\x0e\x32\x0e.pb.EffectType\x12\x0c\n\x04name\x18\x03 \x01(\t\"0\n\rIndexTipRooms\x12\x0f\n\x07room_id\x18\x01 \x01(\x03\x12\x0e\n\x06tip_id\x18\x02 \x01(\x05\"=\n\x07RegisId\x12\x0b\n\x03ios\x18\x01 \x01(\t\x12\x0f\n\x07\x61ndroid\x18\x02 \x01(\t\x12\x14\n\x0cmanufacturer\x18\x03 \x01(\t\"P\n\nModelOnOff\x12\x1c\n\x05onOff\x18\x01 \x01(\x0e\x32\r.pb.OnOffType\x12$\n\x06status\x18\x02 \x01(\x0e\x32\x14.pb.ModelOnOffStatus\"\xd0\x01\n\x04Rank\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x18\n\x03sex\x18\x03 \x01(\x0e\x32\x0b.pb.SexType\x12\r\n\x05level\x18\x04 \x01(\r\x12\r\n\x05value\x18\x05 \x01(\x04\x12\x10\n\x08res_time\x18\x06 \x01(\r\x12\x0f\n\x07gap_val\x18\x07 \x01(\r\x12\x0c\n\x04icon\x18\x08 \x01(\t\x12\x0f\n\x07gift_id\x18\t \x01(\x04\x12\x10\n\x08gift_num\x18\n \x01(\r\x12\x0f\n\x07ranking\x18\x0b \x01(\r\x12\x11\n\tgift_name\x18\x0c \x01(\t\"5\n\x0fPlayerChairRoom\x12\x11\n\tplayer_id\x18\x01 \x01(\x03\x12\x0f\n\x07room_id\x18\x02 \x01(\x03\"l\n\x08\x43lanInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x11\n\ticon_word\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\x03\x12\x12\n\nlevel_name\x18\x05 \x01(\t\x12\x10\n\x08is_admin\x18\x06 \x01(\x08\"*\n\x06Period\x12\x10\n\x08\x62\x65gin_at\x18\x01 \x01(\x03\x12\x0e\n\x06\x65nd_at\x18\x02 \x01(\x03\",\n\tLabelInfo\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63lassify_id\x18\x02 \x01(\x05\"Y\n\x13PlayerResourceShort\x12-\n\rresource_type\x18\x01 \x01(\x0e\x32\x16.pb.PlayerResourceType\x12\x13\n\x0bresource_id\x18\x02 \x01(\t\"\x96\x01\n\x0ePlayerResource\x12-\n\rresource_type\x18\x01 \x01(\x0e\x32\x16.pb.PlayerResourceType\x12\x13\n\x0bresource_id\x18\x02 \x01(\t\x12\x10\n\x08nickname\x18\x03 \x01(\t\x12\x14\n\x0chead_img_url\x18\x04 \x01(\t\x12\x18\n\x03sex\x18\x05 \x01(\x0e\x32\x0b.pb.SexType\"c\n\x17PlayerResourceWithScore\x12+\n\x0fplayer_resource\x18\x01 \x01(\x0b\x32\x12.pb.PlayerResource\x12\r\n\x05score\x18\x02 \x01(\x03\x12\x0c\n\x04rank\x18\x03 \x01(\x05\"\xb4\x01\n\x13\x41ttitudeDegreesInfo\x12\x35\n\x0e\x64\x65grees_status\x18\x01 \x01(\x0e\x32\x1d.pb.AttitudeDegreesStatusType\x12\x36\n\rcategory_info\x18\x02 \x03(\x0b\x32\x1f.pb.AttitudeCategoryDegreesInfo\x12\x14\n\x0ctotal_degree\x18\x03 \x01(\x05\x12\x18\n\x10\x61nalysis_content\x18\x04 \x01(\t\"g\n\x1b\x41ttitudeCategoryDegreesInfo\x12\x13\n\x0b\x63\x61tegory_id\x18\x01 \x01(\x05\x12\x15\n\rcategory_name\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65gree\x18\x03 \x01(\x05\x12\x0c\n\x04icon\x18\x04 \x01(\t\"\x85\x01\n\x0e\x43MediaResource\x12\"\n\nmedia_type\x18\x01 \x01(\x0e\x32\x0e.pb.CMediaType\x12\x11\n\tmedia_url\x18\x02 \x01(\t\x12\x11\n\tcover_url\x18\x03 \x01(\t\x12\x13\n\x0bmedia_width\x18\x04 \x01(\x05\x12\x14\n\x0cmedia_height\x18\x05 \x01(\x05\"\x1b\n\x0bSayHelloReq\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1c\n\x0bSayHelloRes\x12\r\n\x05reply\x18\x01 \x01(\t\"b\n\x0cHeartbeatReq\x12\x0f\n\x07goim_id\x18\x01 \x01(\x03\x12\x11\n\tplayer_id\x18\x02 \x01(\x03\x12\n\n\x02ip\x18\x03 \x01(\t\x12\"\n\ndeviceType\x18\x04 \x01(\x0e\x32\x0e.pb.DeviceType\"!\n\x0cHeartbeatRes\x12\x11\n\ttimestamp\x18\x02 \x01(\x03*\xad\x01\n\tCommonErr\x12\x0f\n\x0b\x45rrCodeNone\x10\x00\x12\x11\n\x0c\x45rrCodeRedis\x10\x91N\x12\x11\n\x0c\x45rrCodeMysql\x10\x92N\x12\x15\n\x10\x45rrCodeFrequency\x10\x93N\x12\x11\n\x0c\x45rrCodeParam\x10\x94N\x12\x16\n\x11\x45rrCodeNoMatchObj\x10\x95N\x12\x10\n\x0b\x45rrCodeBusy\x10\x96N\x12\x15\n\x0f\x45rrCodeMaintain\x10\x9a\x82\x01*,\n\x07SexType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04MALE\x10\x01\x12\n\n\x06\x46\x45MALE\x10\x02*0\n\x0bOwnerInRoom\x12\x11\n\rNotInSelfRoom\x10\x00\x12\x0e\n\nInSelfRoom\x10\x01*%\n\tSceneType\x12\x0b\n\x07ST_ZERO\x10\x00\x12\x0b\n\x07ST_HOME\x10\x01*y\n\rRoomAdminType\x12\r\n\tRAT_GUEST\x10\x00\x12\x0e\n\nRAT_NORMAL\x10\n\x12\r\n\tRAT_ADMIN\x10\x14\x12\r\n\tRAT_OWNER\x10\x1e\x12\x13\n\x0fRAT_SUPER_ADMIN\x10(\x12\x16\n\tRAT_BLACK\x10\xfb\xff\xff\xff\xff\xff\xff\xff\xff\x01*\xfb\x01\n\nDeviceType\x12\x0e\n\nDT_UNKNOWN\x10\x00\x12\x12\n\x0e\x44T_FLASHPLAYER\x10\x01\x12\x14\n\x10\x44T_ANDROID_PHONE\x10\x14\x12\x10\n\x0c\x44T_IOS_PHONE\x10(\x12\x18\n\x14\x44T_WINDOWS_ASSISTANT\x10P\x12\x11\n\rDT_WINDOWS_PC\x10Z\x12\x0c\n\x08\x44T_ROBOT\x10\x64\x12\x1a\n\x16\x44T_WECHAT_SUBSCRIPTION\x10n\x12\x17\n\x13\x44T_QQ_SMALL_PROGRAM\x10x\x12\x17\n\x12\x44T_WX_MINI_PROGRAM\x10\x82\x01\x12\x0b\n\x06\x44T_WEB\x10\x8c\x01\x12\x0b\n\x06\x44T_MAC\x10\x96\x01*\x99\x01\n\x0bPlayerFlags\x12\x0b\n\x07PF_ZERO\x10\x00\x12\x14\n\x10PF_CERTIFICATION\x10\x01\x12\x10\n\x0cPF_BIND_BANK\x10\x04\x12\r\n\tPF_INVITE\x10\x05\x12\x13\n\x0fPF_CHARGE_FIRST\x10\x0c\x12\x18\n\x14PF_ATTITUDE_QUESTION\x10\r\x12\x17\n\x13PF_END_REGISTRATION\x10\x0e*2\n\x0c\x41\x63\x63ountFlags\x12\x0b\n\x07\x41\x46_ZERO\x10\x00\x12\x15\n\x11\x41\x46_PHONE_VERIFIED\x10\x01*\xfc\r\n\tOnOffType\x12\x0c\n\x08YEAR_BAG\x10\x00\x12\r\n\tCRACK_EGG\x10\x01\x12\x0e\n\nGOOGLE_PAY\x10\x05\x12\x0b\n\x07IAP_PAY\x10\x06\x12\n\n\x06INVITE\x10\x07\x12\x12\n\x0eINDEX_CATEGORY\x10\x08\x12\n\n\x06\x43\x45RTIF\x10\t\x12\t\n\x05GUARD\x10\n\x12\x10\n\x0cLOTTERY_DRAW\x10\x0c\x12\x0f\n\x0bMENTOR_SHIP\x10\r\x12\x0e\n\nCERTIF_IOS\x10\x0e\x12\x11\n\rREAL_IDENTITY\x10\x0f\x12\x0f\n\x0bNOVICE_GIFT\x10\x10\x12\x12\n\x0eROOM_SET_MODEL\x10\x12\x12\x11\n\rACTIVITY_TYPE\x10\x14\x12\x0c\n\x08\x41\x43TIVITY\x10\x15\x12\x0c\n\x08HOT_SONG\x10\x17\x12\x0e\n\nROOM_ENTER\x10\"\x12\x1d\n\x19ROOM_PATTERN_HIGH_QUALITY\x10#\x12\x11\n\rAUTH_LOGIN_UI\x10&\x12\x12\n\x0eUSER_DATA_EDIT\x10)\x12\x11\n\rCERTIFICATION\x10+\x12\x1b\n\x17\x43\x45RTIFICATION_ROOM_SHOW\x10,\x12%\n!CERTIFICATION_ROOM_WIN_OPEN_CLOSE\x10-\x12\x10\n\x0c\x43\x45RTIFY_WORD\x10.\x12\x11\n\rCERTIFY_CHAIR\x10/\x12\x1c\n\x18\x43\x45RTIFY_UPDATE_USER_INFO\x10\x30\x12\x1c\n\x18\x43\x45RTIFY_BROADCAST_FRIEND\x10\x31\x12\x15\n\x11\x43\x45RTIFY_HEAD_LINE\x10\x32\x12\x15\n\x11\x43\x45RTIFY_TIAO_TIAO\x10\x33\x12\x14\n\x10LOGIN_BIND_PHONE\x10\x34\x12\x1c\n\x18\x43\x45RTIFY_OWNER_ENTER_ROOM\x10\x35\x12\x0f\n\x0bYoung_Model\x10:\x12\x14\n\x10\x43USTOMER_SERVICE\x10;\x12\x15\n\x11OVERSEAS_IP_LIMIT\x10\x42\x12\x12\n\x0eOLD_NAME_LIMIT\x10\x43\x12\x12\n\x0e\x43RACK_SELF_MSG\x10\x44\x12\x12\n\x0eORDER_LOCATION\x10G\x12\x12\n\x0e\x44\x45LETE_ACCOUNT\x10I\x12\x0f\n\x0bYUNPIAN_SMS\x10J\x12\x11\n\rBIND_PHONE_V2\x10K\x12\x14\n\x10\x42IND_PHONE_LOGIN\x10L\x12\x0e\n\nCOUNT_DOWN\x10N\x12\x0e\n\nOXYGEN_BAR\x10^\x12\x13\n\x0fPRIVACY_SETTING\x10_\x12\x1f\n\x1bOXYGEN_BAR_CLAN_MEMBER_ONLY\x10`\x12\x18\n\x14OXYGEN_BAR_TREND_GIF\x10\x61\x12\x0e\n\nDATA_AUDIT\x10\x62\x12\r\n\tInner_Tec\x10\x64\x12\r\n\tInner_Ali\x10\x65\x12\x16\n\x12\x43\x45RTIFY_IM_PICTURE\x10g\x12\x0b\n\x07\x43MB_VIP\x10h\x12\x13\n\x0f\x43RACKEGG_FOREST\x10i\x12\x13\n\x0e\x41NTI_ADDICTION\x10\xc8\x01\x12&\n!TEXT_FILTER_ROOM_SCREEN_ENCRYPTED\x10\xc9\x01\x12(\n#TEXT_FILTER_ROOM_SCREEN_UNENCRYPTED\x10\xca\x01\x12!\n\x1cTEXT_FILTER_BROADCAST_FRIEND\x10\xcb\x01\x12\x1d\n\x18TEXT_FILTER_PRIVATE_CHAT\x10\xcc\x01\x12\x10\n\x0c\x42\x43_HEAD_LINE\x10n\x12\x13\n\x0fONE_CLICK_LOGIN\x10o\x12\x0e\n\nCERTIFY_PM\x10p\x12\x13\n\x0f\x43\x45RTIFY_PICTURE\x10q\x12\x19\n\x15\x43HANNEL_ADVERT_AUDITS\x10r\x12\x1a\n\x16\x43\x45RTIFY_CREATE_CHANNEL\x10t\x12\x18\n\x14\x43\x45RTIFY_JOIN_CHANNEL\x10u\x12\x10\n\x0c\x43\x45RTIFY_GIVE\x10v\x12\x17\n\x13\x43\x45RTIFY_ROOM_NOTICE\x10w\x12\x14\n\x10\x43\x45RTIFY_RECHARGE\x10x\x12\x19\n\x15\x43\x45RTIFY_PUBLISH_TREND\x10y\x12\x19\n\x15\x43\x45RTIFY_COMMENT_TREND\x10z\x12\x11\n\rHOME_NAV_TYPE\x10{\x12\x11\n\rLOGIN_CHECKED\x10|\x12\x0e\n\nHIGH_SOUND\x10}\x12\x16\n\x12HIGH_SOUND_CHANNEL\x10~\x12\x1a\n\x16\x43HANNEL_STAR_CHALLENGE\x10\x7f\x12\x11\n\x0c\x43HANNEL_STAT\x10\x80\x01\x12\x11\n\x0cREGISTER_SEX\x10\x82\x01\x12\x16\n\x11REGISTER_NICKNAME\x10\x83\x01\x12\x16\n\x11REGISTER_ATTITUDE\x10\x84\x01\x12\x13\n\x0e\x43REATE_CHANNEL\x10\x85\x01\x12\x1a\n\x15\x43OMMUNITY_TREND_AUDIO\x10\x86\x01\x12\x0c\n\x07IM_TIPS\x10\x87\x01\x12\x18\n\x13MULTI_CLIENT_ONLINE\x10\xfd\x01*)\n\nStatusCode\x12\x0b\n\x07SC_FAIL\x10\x00\x12\x0e\n\nSC_SUCCESS\x10\x01*?\n\nEffectType\x12\x12\n\x0e\x45\x66\x66\x65\x63tTypeNone\x10\x00\x12\x1d\n\x19\x45\x66\x66\x65\x63tTypeNicknamePendant\x10\x01*\x7f\n\x0e\x45\x66\x66\x65\x63tTimeType\x12\x18\n\x14\x45\x66\x66\x65\x63tTimeTypeAlways\x10\x00\x12\x16\n\x12\x45\x66\x66\x65\x63tTimeTypeMike\x10\x01\x12\x1e\n\x1a\x45\x66\x66\x65\x63tTimeTypeWearInPacket\x10\x02\x12\x1b\n\x17\x45\x66\x66\x65\x63tTimeTypePermanent\x10\x03*,\n\x0f\x45\x66\x66\x65\x63tUseStatus\x12\n\n\x06\x45S_Use\x10\x00\x12\r\n\tES_NotUse\x10\x01*I\n\x10\x45\x66\x66\x65\x63tNoticeType\x12\x18\n\x14\x45\x66\x66\x65\x63tNoticeTypeGain\x10\x00\x12\x1b\n\x17\x45\x66\x66\x65\x63tNoticeTypeTimeout\x10\x01*:\n\x10ModelOnOffStatus\x12\x0b\n\x07\x41LL_OFF\x10\x00\x12\n\n\x06\x41LL_ON\x10\x01\x12\r\n\tWHITELIST\x10\x02*A\n\x08RankType\x12\x0b\n\x07RT_ZERO\x10\x00\x12\x0c\n\x08RT_CHARM\x10\x01\x12\r\n\tRT_WEALTH\x10\x02\x12\x0b\n\x07RT_GIFT\x10\x03*N\n\rLoadClickType\x12\x0c\n\x08LCT_ZERO\x10\x00\x12\x17\n\x13LCT_INTIMATE_DETAIL\x10\x01\x12\x16\n\x12LCT_INTIMATE_STORE\x10\x02*F\n\x0b\x41uditStatus\x12\x11\n\rAS_Audit_Pass\x10\x00\x12\x0f\n\x0b\x41S_Auditing\x10\x01\x12\x13\n\x0f\x41S_Audit_Refuse\x10\x02*\xf3\x01\n\nUploadType\x12\x0c\n\x08TypeZero\x10\x00\x12\x10\n\x0cHeadAlbumImg\x10\x01\x12\x0f\n\x0bHeadIconImg\x10\x02\x12\x0f\n\x0b\x44ynamicsImg\x10\x03\x12\r\n\tClientLog\x10\x04\x12\x0e\n\nTipOffsImg\x10\x05\x12\x0c\n\x08Indetity\x10\x06\x12\x0b\n\x07PMMedia\x10\x07\x12\t\n\x05Voice\x10\x08\x12\x11\n\rBackgroundImg\x10\x17\x12\x0f\n\x0b\x43hannelIcon\x10\x18\x12\x11\n\rWXRobotQRcode\x10\x19\x12\x13\n\x0f\x43ommunityTagImg\x10\x1c\x12\x12\n\x0ePersonLabelImg\x10\x1d*\xe9\x01\n\x0ePayChannelType\x12\x0c\n\x08PCT_NULL\x10\x00\x12\x11\n\rPCT_ALIPAY_H5\x10\x02\x12\x12\n\x0ePCT_ALIPAY_APP\x10\x03\x12\x11\n\rPCT_WXPAY_APP\x10\x04\x12\x10\n\x0cPCT_WXPAY_H5\x10\x05\x12\x0b\n\x07PCT_IAP\x10\x06\x12\x0c\n\x08PCT_PLAY\x10\x08\x12\x0e\n\nPCT_PAYPAL\x10\n\x12\r\n\tPCT_BOING\x10\x0b\x12\x10\n\x0cPCT_UNIONPAY\x10\x0c\x12\x0e\n\tPCT_AGENT\x10\xfd\x01\x12\x0f\n\nPCT_MANUAL\x10\xfe\x01\x12\x10\n\x0bPCT_DEVTEST\x10\xff\x01*i\n\x04Role\x12\n\n\x06R_NONE\x10\x00\x12\x0f\n\x0bR_SUPERUSER\x10\x01\x12\x08\n\x04R_OW\x10\x02\x12\x08\n\x04R_VP\x10\x03\x12\x08\n\x04R_MA\x10\x04\x12\t\n\x05R_CA1\x10\x05\x12\t\n\x05R_CA2\x10\x06\x12\x07\n\x03R_R\x10\x07\x12\x07\n\x03R_U\x10\x08*]\n\x0eNameplateStyle\x12\x0b\n\x07NS_NONE\x10\x00\x12\x0e\n\nNS_STYLE_1\x10\x01\x12\x0e\n\nNS_STYLE_2\x10\x02\x12\x0e\n\nNS_STYLE_3\x10\x03\x12\x0e\n\nNS_STYLE_4\x10\x04*E\n\x12PlayerResourceType\x12\x0c\n\x08PRT_NONE\x10\x00\x12\x15\n\x11PRT_FIRST_ACCOUNT\x10\x01\x12\n\n\x06PRT_WX\x10\x02*f\n\x19\x41ttitudeDegreesStatusType\x12\x13\n\x0f\x41\x44ST_BOTH_EVERY\x10\x00\x12\x17\n\x13\x41\x44ST_OPPOSITE_EVERY\x10\x01\x12\x1b\n\x17\x41\x44ST_OPPOSITE_NOTENOUGH\x10\x02*u\n\nCMediaType\x12\x13\n\x0f\x43MediaType_None\x10\x00\x12\x12\n\x0e\x43MediaType_Png\x10\x01\x12\x12\n\x0e\x43MediaType_Gif\x10\x02\x12\x14\n\x10\x43MediaType_Video\x10\x03\x12\x14\n\x10\x43MediaType_Audio\x10\x04*w\n\x11\x44\x65viceConnectOper\x12\x0c\n\x08\x44\x43S_None\x10\x00\x12\x12\n\x0e\x44\x43S_Requesting\x10\x01\x12\x0f\n\x0b\x44\x43S_Receive\x10\x02\x12\x0e\n\nDCS_Refuse\x10\x03\x12\x0f\n\x0b\x44\x43S_Timeout\x10\x04\x12\x0e\n\nDCS_Cancel\x10\x05*\xa7\x01\n\x0b\x44\x65viceCmdId\x12\x11\n\rDC_DeviceZero\x10\x00\x12\x14\n\x0e\x44\x43_DeviceLogin\x10\x99\x98\x1f\x12\x1e\n\x18\x44\x43_MessageConnectOperate\x10\x9a\x98\x1f\x12\x1c\n\x16\x44\x43_MessageStatusUpdate\x10\x9b\x98\x1f\x12\x1a\n\x14\x44\x43_DeviceShareStatus\x10\x9c\x98\x1f\x12\x15\n\x0f\x44\x43_SingoConnect\x10\xb9\xa5%*L\n\nTaskStatus\x12\x0b\n\x07TS_None\x10\x00\x12\x11\n\rTS_Processing\x10\x01\x12\x0e\n\nTS_Success\x10\x02\x12\x0e\n\nTS_Failure\x10\x03*N\n\x08TaskType\x12\x0b\n\x07TT_None\x10\x00\x12\x0c\n\x08TT_Image\x10\x01\x12\x0c\n\x08TT_Video\x10\x02\x12\x0c\n\x08TT_Audio\x10\x03\x12\x0b\n\x07TT_Text\x10\x04*o\n\tLabelType\x12\x0b\n\x07LT_NONE\x10\x00\x12\x0b\n\x07LT_POST\x10\x01\x12\x0e\n\nLT_Gallery\x10\x02\x12\x0c\n\x08LT_Group\x10\x03\x12\x0e\n\nLT_Comment\x10\x04\x12\x0b\n\x07LT_Lora\x10\x05\x12\r\n\tLT_Client\x10\x06*N\n\x08\x41igcType\x12\x0b\n\x07\x41T_NONE\x10\x00\x12\x0c\n\x08\x41T_IMAGE\x10\x01\x12\x0c\n\x08\x41T_VIDEO\x10\x02\x12\x0c\n\x08\x41T_AUDIO\x10\x03\x12\x0b\n\x07\x41T_TEXT\x10\x04*%\n\x06Module\x12\n\n\x06M_None\x10\x00\x12\x0f\n\x0bM_Subscribe\x10\x01*A\n\nWidgetType\x12\x0b\n\x07WT_None\x10\x00\x12\x0e\n\nWT_General\x10\x01\x12\t\n\x05WT_SD\x10\x02\x12\x0b\n\x07WT_Lora\x10\x03*:\n\rCalculateMode\x12\x0b\n\x07\x43M_None\x10\x00\x12\r\n\tCM_Single\x10\x01\x12\r\n\tCM_Minute\x10\x02*1\n\x0e\x43hargeCateType\x12\x0e\n\nCCT_Normal\x10\x00\x12\x0f\n\x0b\x43\x43T_ActCard\x10\x01\x42\x06\xa2\x02\x03PB3b\x06proto3')
+
+_COMMONERR = DESCRIPTOR.enum_types_by_name['CommonErr']
+CommonErr = enum_type_wrapper.EnumTypeWrapper(_COMMONERR)
+_SEXTYPE = DESCRIPTOR.enum_types_by_name['SexType']
+SexType = enum_type_wrapper.EnumTypeWrapper(_SEXTYPE)
+_OWNERINROOM = DESCRIPTOR.enum_types_by_name['OwnerInRoom']
+OwnerInRoom = enum_type_wrapper.EnumTypeWrapper(_OWNERINROOM)
+_SCENETYPE = DESCRIPTOR.enum_types_by_name['SceneType']
+SceneType = enum_type_wrapper.EnumTypeWrapper(_SCENETYPE)
+_ROOMADMINTYPE = DESCRIPTOR.enum_types_by_name['RoomAdminType']
+RoomAdminType = enum_type_wrapper.EnumTypeWrapper(_ROOMADMINTYPE)
+_DEVICETYPE = DESCRIPTOR.enum_types_by_name['DeviceType']
+DeviceType = enum_type_wrapper.EnumTypeWrapper(_DEVICETYPE)
+_PLAYERFLAGS = DESCRIPTOR.enum_types_by_name['PlayerFlags']
+PlayerFlags = enum_type_wrapper.EnumTypeWrapper(_PLAYERFLAGS)
+_ACCOUNTFLAGS = DESCRIPTOR.enum_types_by_name['AccountFlags']
+AccountFlags = enum_type_wrapper.EnumTypeWrapper(_ACCOUNTFLAGS)
+_ONOFFTYPE = DESCRIPTOR.enum_types_by_name['OnOffType']
+OnOffType = enum_type_wrapper.EnumTypeWrapper(_ONOFFTYPE)
+_STATUSCODE = DESCRIPTOR.enum_types_by_name['StatusCode']
+StatusCode = enum_type_wrapper.EnumTypeWrapper(_STATUSCODE)
+_EFFECTTYPE = DESCRIPTOR.enum_types_by_name['EffectType']
+EffectType = enum_type_wrapper.EnumTypeWrapper(_EFFECTTYPE)
+_EFFECTTIMETYPE = DESCRIPTOR.enum_types_by_name['EffectTimeType']
+EffectTimeType = enum_type_wrapper.EnumTypeWrapper(_EFFECTTIMETYPE)
+_EFFECTUSESTATUS = DESCRIPTOR.enum_types_by_name['EffectUseStatus']
+EffectUseStatus = enum_type_wrapper.EnumTypeWrapper(_EFFECTUSESTATUS)
+_EFFECTNOTICETYPE = DESCRIPTOR.enum_types_by_name['EffectNoticeType']
+EffectNoticeType = enum_type_wrapper.EnumTypeWrapper(_EFFECTNOTICETYPE)
+_MODELONOFFSTATUS = DESCRIPTOR.enum_types_by_name['ModelOnOffStatus']
+ModelOnOffStatus = enum_type_wrapper.EnumTypeWrapper(_MODELONOFFSTATUS)
+_RANKTYPE = DESCRIPTOR.enum_types_by_name['RankType']
+RankType = enum_type_wrapper.EnumTypeWrapper(_RANKTYPE)
+_LOADCLICKTYPE = DESCRIPTOR.enum_types_by_name['LoadClickType']
+LoadClickType = enum_type_wrapper.EnumTypeWrapper(_LOADCLICKTYPE)
+_AUDITSTATUS = DESCRIPTOR.enum_types_by_name['AuditStatus']
+AuditStatus = enum_type_wrapper.EnumTypeWrapper(_AUDITSTATUS)
+_UPLOADTYPE = DESCRIPTOR.enum_types_by_name['UploadType']
+UploadType = enum_type_wrapper.EnumTypeWrapper(_UPLOADTYPE)
+_PAYCHANNELTYPE = DESCRIPTOR.enum_types_by_name['PayChannelType']
+PayChannelType = enum_type_wrapper.EnumTypeWrapper(_PAYCHANNELTYPE)
+_ROLE = DESCRIPTOR.enum_types_by_name['Role']
+Role = enum_type_wrapper.EnumTypeWrapper(_ROLE)
+_NAMEPLATESTYLE = DESCRIPTOR.enum_types_by_name['NameplateStyle']
+NameplateStyle = enum_type_wrapper.EnumTypeWrapper(_NAMEPLATESTYLE)
+_PLAYERRESOURCETYPE = DESCRIPTOR.enum_types_by_name['PlayerResourceType']
+PlayerResourceType = enum_type_wrapper.EnumTypeWrapper(_PLAYERRESOURCETYPE)
+_ATTITUDEDEGREESSTATUSTYPE = DESCRIPTOR.enum_types_by_name['AttitudeDegreesStatusType']
+AttitudeDegreesStatusType = enum_type_wrapper.EnumTypeWrapper(_ATTITUDEDEGREESSTATUSTYPE)
+_CMEDIATYPE = DESCRIPTOR.enum_types_by_name['CMediaType']
+CMediaType = enum_type_wrapper.EnumTypeWrapper(_CMEDIATYPE)
+_DEVICECONNECTOPER = DESCRIPTOR.enum_types_by_name['DeviceConnectOper']
+DeviceConnectOper = enum_type_wrapper.EnumTypeWrapper(_DEVICECONNECTOPER)
+_DEVICECMDID = DESCRIPTOR.enum_types_by_name['DeviceCmdId']
+DeviceCmdId = enum_type_wrapper.EnumTypeWrapper(_DEVICECMDID)
+_TASKSTATUS = DESCRIPTOR.enum_types_by_name['TaskStatus']
+TaskStatus = enum_type_wrapper.EnumTypeWrapper(_TASKSTATUS)
+_TASKTYPE = DESCRIPTOR.enum_types_by_name['TaskType']
+TaskType = enum_type_wrapper.EnumTypeWrapper(_TASKTYPE)
+_LABELTYPE = DESCRIPTOR.enum_types_by_name['LabelType']
+LabelType = enum_type_wrapper.EnumTypeWrapper(_LABELTYPE)
+_AIGCTYPE = DESCRIPTOR.enum_types_by_name['AigcType']
+AigcType = enum_type_wrapper.EnumTypeWrapper(_AIGCTYPE)
+_MODULE = DESCRIPTOR.enum_types_by_name['Module']
+Module = enum_type_wrapper.EnumTypeWrapper(_MODULE)
+_WIDGETTYPE = DESCRIPTOR.enum_types_by_name['WidgetType']
+WidgetType = enum_type_wrapper.EnumTypeWrapper(_WIDGETTYPE)
+_CALCULATEMODE = DESCRIPTOR.enum_types_by_name['CalculateMode']
+CalculateMode = enum_type_wrapper.EnumTypeWrapper(_CALCULATEMODE)
+_CHARGECATETYPE = DESCRIPTOR.enum_types_by_name['ChargeCateType']
+ChargeCateType = enum_type_wrapper.EnumTypeWrapper(_CHARGECATETYPE)
+ErrCodeNone = 0
+ErrCodeRedis = 10001
+ErrCodeMysql = 10002
+ErrCodeFrequency = 10003
+ErrCodeParam = 10004
+ErrCodeNoMatchObj = 10005
+ErrCodeBusy = 10006
+ErrCodeMaintain = 16666
+UNKNOWN = 0
+MALE = 1
+FEMALE = 2
+NotInSelfRoom = 0
+InSelfRoom = 1
+ST_ZERO = 0
+ST_HOME = 1
+RAT_GUEST = 0
+RAT_NORMAL = 10
+RAT_ADMIN = 20
+RAT_OWNER = 30
+RAT_SUPER_ADMIN = 40
+RAT_BLACK = -5
+DT_UNKNOWN = 0
+DT_FLASHPLAYER = 1
+DT_ANDROID_PHONE = 20
+DT_IOS_PHONE = 40
+DT_WINDOWS_ASSISTANT = 80
+DT_WINDOWS_PC = 90
+DT_ROBOT = 100
+DT_WECHAT_SUBSCRIPTION = 110
+DT_QQ_SMALL_PROGRAM = 120
+DT_WX_MINI_PROGRAM = 130
+DT_WEB = 140
+DT_MAC = 150
+PF_ZERO = 0
+PF_CERTIFICATION = 1
+PF_BIND_BANK = 4
+PF_INVITE = 5
+PF_CHARGE_FIRST = 12
+PF_ATTITUDE_QUESTION = 13
+PF_END_REGISTRATION = 14
+AF_ZERO = 0
+AF_PHONE_VERIFIED = 1
+YEAR_BAG = 0
+CRACK_EGG = 1
+GOOGLE_PAY = 5
+IAP_PAY = 6
+INVITE = 7
+INDEX_CATEGORY = 8
+CERTIF = 9
+GUARD = 10
+LOTTERY_DRAW = 12
+MENTOR_SHIP = 13
+CERTIF_IOS = 14
+REAL_IDENTITY = 15
+NOVICE_GIFT = 16
+ROOM_SET_MODEL = 18
+ACTIVITY_TYPE = 20
+ACTIVITY = 21
+HOT_SONG = 23
+ROOM_ENTER = 34
+ROOM_PATTERN_HIGH_QUALITY = 35
+AUTH_LOGIN_UI = 38
+USER_DATA_EDIT = 41
+CERTIFICATION = 43
+CERTIFICATION_ROOM_SHOW = 44
+CERTIFICATION_ROOM_WIN_OPEN_CLOSE = 45
+CERTIFY_WORD = 46
+CERTIFY_CHAIR = 47
+CERTIFY_UPDATE_USER_INFO = 48
+CERTIFY_BROADCAST_FRIEND = 49
+CERTIFY_HEAD_LINE = 50
+CERTIFY_TIAO_TIAO = 51
+LOGIN_BIND_PHONE = 52
+CERTIFY_OWNER_ENTER_ROOM = 53
+Young_Model = 58
+CUSTOMER_SERVICE = 59
+OVERSEAS_IP_LIMIT = 66
+OLD_NAME_LIMIT = 67
+CRACK_SELF_MSG = 68
+ORDER_LOCATION = 71
+DELETE_ACCOUNT = 73
+YUNPIAN_SMS = 74
+BIND_PHONE_V2 = 75
+BIND_PHONE_LOGIN = 76
+COUNT_DOWN = 78
+OXYGEN_BAR = 94
+PRIVACY_SETTING = 95
+OXYGEN_BAR_CLAN_MEMBER_ONLY = 96
+OXYGEN_BAR_TREND_GIF = 97
+DATA_AUDIT = 98
+Inner_Tec = 100
+Inner_Ali = 101
+CERTIFY_IM_PICTURE = 103
+CMB_VIP = 104
+CRACKEGG_FOREST = 105
+ANTI_ADDICTION = 200
+TEXT_FILTER_ROOM_SCREEN_ENCRYPTED = 201
+TEXT_FILTER_ROOM_SCREEN_UNENCRYPTED = 202
+TEXT_FILTER_BROADCAST_FRIEND = 203
+TEXT_FILTER_PRIVATE_CHAT = 204
+BC_HEAD_LINE = 110
+ONE_CLICK_LOGIN = 111
+CERTIFY_PM = 112
+CERTIFY_PICTURE = 113
+CHANNEL_ADVERT_AUDITS = 114
+CERTIFY_CREATE_CHANNEL = 116
+CERTIFY_JOIN_CHANNEL = 117
+CERTIFY_GIVE = 118
+CERTIFY_ROOM_NOTICE = 119
+CERTIFY_RECHARGE = 120
+CERTIFY_PUBLISH_TREND = 121
+CERTIFY_COMMENT_TREND = 122
+HOME_NAV_TYPE = 123
+LOGIN_CHECKED = 124
+HIGH_SOUND = 125
+HIGH_SOUND_CHANNEL = 126
+CHANNEL_STAR_CHALLENGE = 127
+CHANNEL_STAT = 128
+REGISTER_SEX = 130
+REGISTER_NICKNAME = 131
+REGISTER_ATTITUDE = 132
+CREATE_CHANNEL = 133
+COMMUNITY_TREND_AUDIO = 134
+IM_TIPS = 135
+MULTI_CLIENT_ONLINE = 253
+SC_FAIL = 0
+SC_SUCCESS = 1
+EffectTypeNone = 0
+EffectTypeNicknamePendant = 1
+EffectTimeTypeAlways = 0
+EffectTimeTypeMike = 1
+EffectTimeTypeWearInPacket = 2
+EffectTimeTypePermanent = 3
+ES_Use = 0
+ES_NotUse = 1
+EffectNoticeTypeGain = 0
+EffectNoticeTypeTimeout = 1
+ALL_OFF = 0
+ALL_ON = 1
+WHITELIST = 2
+RT_ZERO = 0
+RT_CHARM = 1
+RT_WEALTH = 2
+RT_GIFT = 3
+LCT_ZERO = 0
+LCT_INTIMATE_DETAIL = 1
+LCT_INTIMATE_STORE = 2
+AS_Audit_Pass = 0
+AS_Auditing = 1
+AS_Audit_Refuse = 2
+TypeZero = 0
+HeadAlbumImg = 1
+HeadIconImg = 2
+DynamicsImg = 3
+ClientLog = 4
+TipOffsImg = 5
+Indetity = 6
+PMMedia = 7
+Voice = 8
+BackgroundImg = 23
+ChannelIcon = 24
+WXRobotQRcode = 25
+CommunityTagImg = 28
+PersonLabelImg = 29
+PCT_NULL = 0
+PCT_ALIPAY_H5 = 2
+PCT_ALIPAY_APP = 3
+PCT_WXPAY_APP = 4
+PCT_WXPAY_H5 = 5
+PCT_IAP = 6
+PCT_PLAY = 8
+PCT_PAYPAL = 10
+PCT_BOING = 11
+PCT_UNIONPAY = 12
+PCT_AGENT = 253
+PCT_MANUAL = 254
+PCT_DEVTEST = 255
+R_NONE = 0
+R_SUPERUSER = 1
+R_OW = 2
+R_VP = 3
+R_MA = 4
+R_CA1 = 5
+R_CA2 = 6
+R_R = 7
+R_U = 8
+NS_NONE = 0
+NS_STYLE_1 = 1
+NS_STYLE_2 = 2
+NS_STYLE_3 = 3
+NS_STYLE_4 = 4
+PRT_NONE = 0
+PRT_FIRST_ACCOUNT = 1
+PRT_WX = 2
+ADST_BOTH_EVERY = 0
+ADST_OPPOSITE_EVERY = 1
+ADST_OPPOSITE_NOTENOUGH = 2
+CMediaType_None = 0
+CMediaType_Png = 1
+CMediaType_Gif = 2
+CMediaType_Video = 3
+CMediaType_Audio = 4
+DCS_None = 0
+DCS_Requesting = 1
+DCS_Receive = 2
+DCS_Refuse = 3
+DCS_Timeout = 4
+DCS_Cancel = 5
+DC_DeviceZero = 0
+DC_DeviceLogin = 511001
+DC_MessageConnectOperate = 511002
+DC_MessageStatusUpdate = 511003
+DC_DeviceShareStatus = 511004
+DC_SingoConnect = 611001
+TS_None = 0
+TS_Processing = 1
+TS_Success = 2
+TS_Failure = 3
+TT_None = 0
+TT_Image = 1
+TT_Video = 2
+TT_Audio = 3
+TT_Text = 4
+LT_NONE = 0
+LT_POST = 1
+LT_Gallery = 2
+LT_Group = 3
+LT_Comment = 4
+LT_Lora = 5
+LT_Client = 6
+AT_NONE = 0
+AT_IMAGE = 1
+AT_VIDEO = 2
+AT_AUDIO = 3
+AT_TEXT = 4
+M_None = 0
+M_Subscribe = 1
+WT_None = 0
+WT_General = 1
+WT_SD = 2
+WT_Lora = 3
+CM_None = 0
+CM_Single = 1
+CM_Minute = 2
+CCT_Normal = 0
+CCT_ActCard = 1
+
+
+_PLAYER = DESCRIPTOR.message_types_by_name['Player']
+_USERINFO = DESCRIPTOR.message_types_by_name['UserInfo']
+_PLAYERINFO = DESCRIPTOR.message_types_by_name['PlayerInfo']
+_BAGITEM = DESCRIPTOR.message_types_by_name['BagItem']
+_AGODAKEY = DESCRIPTOR.message_types_by_name['AgodaKey']
+_ONOFFSTATUS = DESCRIPTOR.message_types_by_name['OnOffStatus']
+_SEARCHPLAYERENTRY = DESCRIPTOR.message_types_by_name['SearchPlayerEntry']
+_EFFECTINFO = DESCRIPTOR.message_types_by_name['EffectInfo']
+_EFFECT = DESCRIPTOR.message_types_by_name['Effect']
+_EFFECTCONFIG = DESCRIPTOR.message_types_by_name['EffectConfig']
+_EFFECTNICKNAMEPENDANT = DESCRIPTOR.message_types_by_name['EffectNicknamePendant']
+_EFFECTSERCONF = DESCRIPTOR.message_types_by_name['EffectSerConf']
+_INDEXTIPROOMS = DESCRIPTOR.message_types_by_name['IndexTipRooms']
+_REGISID = DESCRIPTOR.message_types_by_name['RegisId']
+_MODELONOFF = DESCRIPTOR.message_types_by_name['ModelOnOff']
+_RANK = DESCRIPTOR.message_types_by_name['Rank']
+_PLAYERCHAIRROOM = DESCRIPTOR.message_types_by_name['PlayerChairRoom']
+_CLANINFO = DESCRIPTOR.message_types_by_name['ClanInfo']
+_PERIOD = DESCRIPTOR.message_types_by_name['Period']
+_LABELINFO = DESCRIPTOR.message_types_by_name['LabelInfo']
+_PLAYERRESOURCESHORT = DESCRIPTOR.message_types_by_name['PlayerResourceShort']
+_PLAYERRESOURCE = DESCRIPTOR.message_types_by_name['PlayerResource']
+_PLAYERRESOURCEWITHSCORE = DESCRIPTOR.message_types_by_name['PlayerResourceWithScore']
+_ATTITUDEDEGREESINFO = DESCRIPTOR.message_types_by_name['AttitudeDegreesInfo']
+_ATTITUDECATEGORYDEGREESINFO = DESCRIPTOR.message_types_by_name['AttitudeCategoryDegreesInfo']
+_CMEDIARESOURCE = DESCRIPTOR.message_types_by_name['CMediaResource']
+_SAYHELLOREQ = DESCRIPTOR.message_types_by_name['SayHelloReq']
+_SAYHELLORES = DESCRIPTOR.message_types_by_name['SayHelloRes']
+_HEARTBEATREQ = DESCRIPTOR.message_types_by_name['HeartbeatReq']
+_HEARTBEATRES = DESCRIPTOR.message_types_by_name['HeartbeatRes']
+Player = _reflection.GeneratedProtocolMessageType('Player', (_message.Message,), {
+  'DESCRIPTOR' : _PLAYER,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.Player)
+  })
+_sym_db.RegisterMessage(Player)
+
+UserInfo = _reflection.GeneratedProtocolMessageType('UserInfo', (_message.Message,), {
+  'DESCRIPTOR' : _USERINFO,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UserInfo)
+  })
+_sym_db.RegisterMessage(UserInfo)
+
+PlayerInfo = _reflection.GeneratedProtocolMessageType('PlayerInfo', (_message.Message,), {
+  'DESCRIPTOR' : _PLAYERINFO,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.PlayerInfo)
+  })
+_sym_db.RegisterMessage(PlayerInfo)
+
+BagItem = _reflection.GeneratedProtocolMessageType('BagItem', (_message.Message,), {
+  'DESCRIPTOR' : _BAGITEM,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.BagItem)
+  })
+_sym_db.RegisterMessage(BagItem)
+
+AgodaKey = _reflection.GeneratedProtocolMessageType('AgodaKey', (_message.Message,), {
+  'DESCRIPTOR' : _AGODAKEY,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AgodaKey)
+  })
+_sym_db.RegisterMessage(AgodaKey)
+
+OnOffStatus = _reflection.GeneratedProtocolMessageType('OnOffStatus', (_message.Message,), {
+  'DESCRIPTOR' : _ONOFFSTATUS,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.OnOffStatus)
+  })
+_sym_db.RegisterMessage(OnOffStatus)
+
+SearchPlayerEntry = _reflection.GeneratedProtocolMessageType('SearchPlayerEntry', (_message.Message,), {
+  'DESCRIPTOR' : _SEARCHPLAYERENTRY,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.SearchPlayerEntry)
+  })
+_sym_db.RegisterMessage(SearchPlayerEntry)
+
+EffectInfo = _reflection.GeneratedProtocolMessageType('EffectInfo', (_message.Message,), {
+  'DESCRIPTOR' : _EFFECTINFO,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.EffectInfo)
+  })
+_sym_db.RegisterMessage(EffectInfo)
+
+Effect = _reflection.GeneratedProtocolMessageType('Effect', (_message.Message,), {
+  'DESCRIPTOR' : _EFFECT,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.Effect)
+  })
+_sym_db.RegisterMessage(Effect)
+
+EffectConfig = _reflection.GeneratedProtocolMessageType('EffectConfig', (_message.Message,), {
+  'DESCRIPTOR' : _EFFECTCONFIG,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.EffectConfig)
+  })
+_sym_db.RegisterMessage(EffectConfig)
+
+EffectNicknamePendant = _reflection.GeneratedProtocolMessageType('EffectNicknamePendant', (_message.Message,), {
+  'DESCRIPTOR' : _EFFECTNICKNAMEPENDANT,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.EffectNicknamePendant)
+  })
+_sym_db.RegisterMessage(EffectNicknamePendant)
+
+EffectSerConf = _reflection.GeneratedProtocolMessageType('EffectSerConf', (_message.Message,), {
+  'DESCRIPTOR' : _EFFECTSERCONF,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.EffectSerConf)
+  })
+_sym_db.RegisterMessage(EffectSerConf)
+
+IndexTipRooms = _reflection.GeneratedProtocolMessageType('IndexTipRooms', (_message.Message,), {
+  'DESCRIPTOR' : _INDEXTIPROOMS,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.IndexTipRooms)
+  })
+_sym_db.RegisterMessage(IndexTipRooms)
+
+RegisId = _reflection.GeneratedProtocolMessageType('RegisId', (_message.Message,), {
+  'DESCRIPTOR' : _REGISID,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.RegisId)
+  })
+_sym_db.RegisterMessage(RegisId)
+
+ModelOnOff = _reflection.GeneratedProtocolMessageType('ModelOnOff', (_message.Message,), {
+  'DESCRIPTOR' : _MODELONOFF,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.ModelOnOff)
+  })
+_sym_db.RegisterMessage(ModelOnOff)
+
+Rank = _reflection.GeneratedProtocolMessageType('Rank', (_message.Message,), {
+  'DESCRIPTOR' : _RANK,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.Rank)
+  })
+_sym_db.RegisterMessage(Rank)
+
+PlayerChairRoom = _reflection.GeneratedProtocolMessageType('PlayerChairRoom', (_message.Message,), {
+  'DESCRIPTOR' : _PLAYERCHAIRROOM,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.PlayerChairRoom)
+  })
+_sym_db.RegisterMessage(PlayerChairRoom)
+
+ClanInfo = _reflection.GeneratedProtocolMessageType('ClanInfo', (_message.Message,), {
+  'DESCRIPTOR' : _CLANINFO,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.ClanInfo)
+  })
+_sym_db.RegisterMessage(ClanInfo)
+
+Period = _reflection.GeneratedProtocolMessageType('Period', (_message.Message,), {
+  'DESCRIPTOR' : _PERIOD,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.Period)
+  })
+_sym_db.RegisterMessage(Period)
+
+LabelInfo = _reflection.GeneratedProtocolMessageType('LabelInfo', (_message.Message,), {
+  'DESCRIPTOR' : _LABELINFO,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.LabelInfo)
+  })
+_sym_db.RegisterMessage(LabelInfo)
+
+PlayerResourceShort = _reflection.GeneratedProtocolMessageType('PlayerResourceShort', (_message.Message,), {
+  'DESCRIPTOR' : _PLAYERRESOURCESHORT,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.PlayerResourceShort)
+  })
+_sym_db.RegisterMessage(PlayerResourceShort)
+
+PlayerResource = _reflection.GeneratedProtocolMessageType('PlayerResource', (_message.Message,), {
+  'DESCRIPTOR' : _PLAYERRESOURCE,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.PlayerResource)
+  })
+_sym_db.RegisterMessage(PlayerResource)
+
+PlayerResourceWithScore = _reflection.GeneratedProtocolMessageType('PlayerResourceWithScore', (_message.Message,), {
+  'DESCRIPTOR' : _PLAYERRESOURCEWITHSCORE,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.PlayerResourceWithScore)
+  })
+_sym_db.RegisterMessage(PlayerResourceWithScore)
+
+AttitudeDegreesInfo = _reflection.GeneratedProtocolMessageType('AttitudeDegreesInfo', (_message.Message,), {
+  'DESCRIPTOR' : _ATTITUDEDEGREESINFO,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AttitudeDegreesInfo)
+  })
+_sym_db.RegisterMessage(AttitudeDegreesInfo)
+
+AttitudeCategoryDegreesInfo = _reflection.GeneratedProtocolMessageType('AttitudeCategoryDegreesInfo', (_message.Message,), {
+  'DESCRIPTOR' : _ATTITUDECATEGORYDEGREESINFO,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.AttitudeCategoryDegreesInfo)
+  })
+_sym_db.RegisterMessage(AttitudeCategoryDegreesInfo)
+
+CMediaResource = _reflection.GeneratedProtocolMessageType('CMediaResource', (_message.Message,), {
+  'DESCRIPTOR' : _CMEDIARESOURCE,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.CMediaResource)
+  })
+_sym_db.RegisterMessage(CMediaResource)
+
+SayHelloReq = _reflection.GeneratedProtocolMessageType('SayHelloReq', (_message.Message,), {
+  'DESCRIPTOR' : _SAYHELLOREQ,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.SayHelloReq)
+  })
+_sym_db.RegisterMessage(SayHelloReq)
+
+SayHelloRes = _reflection.GeneratedProtocolMessageType('SayHelloRes', (_message.Message,), {
+  'DESCRIPTOR' : _SAYHELLORES,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.SayHelloRes)
+  })
+_sym_db.RegisterMessage(SayHelloRes)
+
+HeartbeatReq = _reflection.GeneratedProtocolMessageType('HeartbeatReq', (_message.Message,), {
+  'DESCRIPTOR' : _HEARTBEATREQ,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.HeartbeatReq)
+  })
+_sym_db.RegisterMessage(HeartbeatReq)
+
+HeartbeatRes = _reflection.GeneratedProtocolMessageType('HeartbeatRes', (_message.Message,), {
+  'DESCRIPTOR' : _HEARTBEATRES,
+  '__module__' : 'common_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.HeartbeatRes)
+  })
+_sym_db.RegisterMessage(HeartbeatRes)
+
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\242\002\003PB3'
+  _COMMONERR._serialized_start=3470
+  _COMMONERR._serialized_end=3643
+  _SEXTYPE._serialized_start=3645
+  _SEXTYPE._serialized_end=3689
+  _OWNERINROOM._serialized_start=3691
+  _OWNERINROOM._serialized_end=3739
+  _SCENETYPE._serialized_start=3741
+  _SCENETYPE._serialized_end=3778
+  _ROOMADMINTYPE._serialized_start=3780
+  _ROOMADMINTYPE._serialized_end=3901
+  _DEVICETYPE._serialized_start=3904
+  _DEVICETYPE._serialized_end=4155
+  _PLAYERFLAGS._serialized_start=4158
+  _PLAYERFLAGS._serialized_end=4311
+  _ACCOUNTFLAGS._serialized_start=4313
+  _ACCOUNTFLAGS._serialized_end=4363
+  _ONOFFTYPE._serialized_start=4366
+  _ONOFFTYPE._serialized_end=6154
+  _STATUSCODE._serialized_start=6156
+  _STATUSCODE._serialized_end=6197
+  _EFFECTTYPE._serialized_start=6199
+  _EFFECTTYPE._serialized_end=6262
+  _EFFECTTIMETYPE._serialized_start=6264
+  _EFFECTTIMETYPE._serialized_end=6391
+  _EFFECTUSESTATUS._serialized_start=6393
+  _EFFECTUSESTATUS._serialized_end=6437
+  _EFFECTNOTICETYPE._serialized_start=6439
+  _EFFECTNOTICETYPE._serialized_end=6512
+  _MODELONOFFSTATUS._serialized_start=6514
+  _MODELONOFFSTATUS._serialized_end=6572
+  _RANKTYPE._serialized_start=6574
+  _RANKTYPE._serialized_end=6639
+  _LOADCLICKTYPE._serialized_start=6641
+  _LOADCLICKTYPE._serialized_end=6719
+  _AUDITSTATUS._serialized_start=6721
+  _AUDITSTATUS._serialized_end=6791
+  _UPLOADTYPE._serialized_start=6794
+  _UPLOADTYPE._serialized_end=7037
+  _PAYCHANNELTYPE._serialized_start=7040
+  _PAYCHANNELTYPE._serialized_end=7273
+  _ROLE._serialized_start=7275
+  _ROLE._serialized_end=7380
+  _NAMEPLATESTYLE._serialized_start=7382
+  _NAMEPLATESTYLE._serialized_end=7475
+  _PLAYERRESOURCETYPE._serialized_start=7477
+  _PLAYERRESOURCETYPE._serialized_end=7546
+  _ATTITUDEDEGREESSTATUSTYPE._serialized_start=7548
+  _ATTITUDEDEGREESSTATUSTYPE._serialized_end=7650
+  _CMEDIATYPE._serialized_start=7652
+  _CMEDIATYPE._serialized_end=7769
+  _DEVICECONNECTOPER._serialized_start=7771
+  _DEVICECONNECTOPER._serialized_end=7890
+  _DEVICECMDID._serialized_start=7893
+  _DEVICECMDID._serialized_end=8060
+  _TASKSTATUS._serialized_start=8062
+  _TASKSTATUS._serialized_end=8138
+  _TASKTYPE._serialized_start=8140
+  _TASKTYPE._serialized_end=8218
+  _LABELTYPE._serialized_start=8220
+  _LABELTYPE._serialized_end=8331
+  _AIGCTYPE._serialized_start=8333
+  _AIGCTYPE._serialized_end=8411
+  _MODULE._serialized_start=8413
+  _MODULE._serialized_end=8450
+  _WIDGETTYPE._serialized_start=8452
+  _WIDGETTYPE._serialized_end=8517
+  _CALCULATEMODE._serialized_start=8519
+  _CALCULATEMODE._serialized_end=8577
+  _CHARGECATETYPE._serialized_start=8579
+  _CHARGECATETYPE._serialized_end=8628
+  _PLAYER._serialized_start=25
+  _PLAYER._serialized_end=400
+  _USERINFO._serialized_start=403
+  _USERINFO._serialized_end=532
+  _PLAYERINFO._serialized_start=535
+  _PLAYERINFO._serialized_end=878
+  _BAGITEM._serialized_start=880
+  _BAGITEM._serialized_end=941
+  _AGODAKEY._serialized_start=943
+  _AGODAKEY._serialized_end=977
+  _ONOFFSTATUS._serialized_start=979
+  _ONOFFSTATUS._serialized_end=1037
+  _SEARCHPLAYERENTRY._serialized_start=1040
+  _SEARCHPLAYERENTRY._serialized_end=1288
+  _EFFECTINFO._serialized_start=1291
+  _EFFECTINFO._serialized_end=1450
+  _EFFECT._serialized_start=1453
+  _EFFECT._serialized_end=1628
+  _EFFECTCONFIG._serialized_start=1630
+  _EFFECTCONFIG._serialized_end=1714
+  _EFFECTNICKNAMEPENDANT._serialized_start=1716
+  _EFFECTNICKNAMEPENDANT._serialized_end=1770
+  _EFFECTSERCONF._serialized_start=1772
+  _EFFECTSERCONF._serialized_end=1843
+  _INDEXTIPROOMS._serialized_start=1845
+  _INDEXTIPROOMS._serialized_end=1893
+  _REGISID._serialized_start=1895
+  _REGISID._serialized_end=1956
+  _MODELONOFF._serialized_start=1958
+  _MODELONOFF._serialized_end=2038
+  _RANK._serialized_start=2041
+  _RANK._serialized_end=2249
+  _PLAYERCHAIRROOM._serialized_start=2251
+  _PLAYERCHAIRROOM._serialized_end=2304
+  _CLANINFO._serialized_start=2306
+  _CLANINFO._serialized_end=2414
+  _PERIOD._serialized_start=2416
+  _PERIOD._serialized_end=2458
+  _LABELINFO._serialized_start=2460
+  _LABELINFO._serialized_end=2504
+  _PLAYERRESOURCESHORT._serialized_start=2506
+  _PLAYERRESOURCESHORT._serialized_end=2595
+  _PLAYERRESOURCE._serialized_start=2598
+  _PLAYERRESOURCE._serialized_end=2748
+  _PLAYERRESOURCEWITHSCORE._serialized_start=2750
+  _PLAYERRESOURCEWITHSCORE._serialized_end=2849
+  _ATTITUDEDEGREESINFO._serialized_start=2852
+  _ATTITUDEDEGREESINFO._serialized_end=3032
+  _ATTITUDECATEGORYDEGREESINFO._serialized_start=3034
+  _ATTITUDECATEGORYDEGREESINFO._serialized_end=3137
+  _CMEDIARESOURCE._serialized_start=3140
+  _CMEDIARESOURCE._serialized_end=3273
+  _SAYHELLOREQ._serialized_start=3275
+  _SAYHELLOREQ._serialized_end=3302
+  _SAYHELLORES._serialized_start=3304
+  _SAYHELLORES._serialized_end=3332
+  _HEARTBEATREQ._serialized_start=3334
+  _HEARTBEATREQ._serialized_end=3432
+  _HEARTBEATRES._serialized_start=3434
+  _HEARTBEATRES._serialized_end=3467
+# @@protoc_insertion_point(module_scope)
```

### Comparing `mecord-cli-0.1.90/mecord/main.py` & `mecord-cli-0.1.91/mecord/main.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/mecord_service.py` & `mecord-cli-0.1.91/mecord/mecord_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,22 +120,22 @@
             path = os.path.dirname(cmd)
             config_file = os.path.join(path, 'config.json')
             with open(config_file, "r") as f:
                 data = json.load(f)
 
             
             process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
-            if data is not None and 'type' in data and data['type'].lower() == 'sd':
-                widget_infos = [{"widget":"SD", "port":6006, "name":"", "path":path}]
-            else:
-                widget_infos = [{"widget":"other", "port":"", "name":"", "pid": process.pid, "path":path}]
-            print(f"monitor process: {path}")
-            progress_monitor.start(widget_infos)
+            # if data is not None and 'type' in data and data['type'].lower() == 'sd':
+            #     widget_infos = [{"widget":"SD", "port":6006, "name":"", "path":path}]
+            # else:
+            #     widget_infos = [{"widget":"other", "port":"", "name":"", "pid": process.pid, "path":path}]
+            # print(f"monitor process: {path}")
+            # progress_monitor.start(widget_infos)
             output, error = process.communicate()
-            progress_monitor.stop()
+            # progress_monitor.stop()
             if process.returncode == 0:
                 print(output.decode(encoding="utf8", errors="ignore"))
                 if os.path.exists(outArgs):
                     with open(outArgs, 'r', encoding='UTF-8') as f:
                         outData = json.load(f)
                     executeSuccess = True
                     print(f"exec success result => {outData}")
```

### Comparing `mecord-cli-0.1.90/mecord/mecord_widget.py` & `mecord-cli-0.1.91/mecord/mecord_widget.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/progress_monitor.py` & `mecord-cli-0.1.91/mecord/progress_monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -232,14 +232,30 @@
         process = psutil.Process(pid)
         return process.cpu_percent(interval=1)
     except psutil.NoSuchProcess:
         return None
 
 def get_process_status(pid: int) -> Optional[str]:
     try:
+<<<<<<< Updated upstream
+=======
+        # if platform.system() == 'Linux':
+        #     status = os.stat(f"/proc/{pid}").st_state
+        #     if status == "R":
+        #         return 'RUNNING'
+        #     elif status == "S" or status == 'D':
+        #         return 'SLEEPING'
+        #     elif status == "T":
+        #         return 'STOPPED'
+        #     elif status == "Z":
+        #         return 'ZOMBIE'
+        #     else:
+        #         return 'UNKNOWN'
+        # else:
+>>>>>>> Stashed changes
         process = psutil.Process(pid)
         pstatus = process.status()
         if pstatus == psutil.STATUS_RUNNING:
             return 'RUNNING'
         elif pstatus == psutil.STATUS_SLEEPING:
             return 'SLEEPING'
         elif pstatus == psutil.STATUS_STOPPED:
```

### Comparing `mecord-cli-0.1.90/mecord/rpcinput_pb2.py` & `mecord-cli-0.1.91/mecord/rpcinput_pb2.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: rpcinput.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0erpcinput.proto\x12\x02pb\"\x82\x01\n\x08RPCInput\x12\x0b\n\x03obj\x18\x01 \x01(\t\x12\x0c\n\x04\x66unc\x18\x02 \x01(\t\x12\x0b\n\x03req\x18\x03 \x01(\x0c\x12\"\n\x03opt\x18\x04 \x03(\x0b\x32\x15.pb.RPCInput.OptEntry\x1a*\n\x08OptEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9f\x01\n\tRPCOutput\x12\x0b\n\x03ret\x18\x01 \x01(\x05\x12\x0b\n\x03rsp\x18\x02 \x01(\x0c\x12#\n\x03opt\x18\x03 \x03(\x0b\x32\x16.pb.RPCOutput.OptEntry\x12\x0c\n\x04\x64\x65sc\x18\x04 \x01(\t\x12\x0b\n\x03obj\x18\x05 \x01(\t\x12\x0c\n\x04\x66unc\x18\x06 \x01(\t\x1a*\n\x08OptEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x08\xa2\x02\x05PROTOb\x06proto3')
-
-
-
-_RPCINPUT = DESCRIPTOR.message_types_by_name['RPCInput']
-_RPCINPUT_OPTENTRY = _RPCINPUT.nested_types_by_name['OptEntry']
-_RPCOUTPUT = DESCRIPTOR.message_types_by_name['RPCOutput']
-_RPCOUTPUT_OPTENTRY = _RPCOUTPUT.nested_types_by_name['OptEntry']
-RPCInput = _reflection.GeneratedProtocolMessageType('RPCInput', (_message.Message,), {
-
-  'OptEntry' : _reflection.GeneratedProtocolMessageType('OptEntry', (_message.Message,), {
-    'DESCRIPTOR' : _RPCINPUT_OPTENTRY,
-    '__module__' : 'rpcinput_pb2'
-    # @@protoc_insertion_point(class_scope:pb.RPCInput.OptEntry)
-    })
-  ,
-  'DESCRIPTOR' : _RPCINPUT,
-  '__module__' : 'rpcinput_pb2'
-  # @@protoc_insertion_point(class_scope:pb.RPCInput)
-  })
-_sym_db.RegisterMessage(RPCInput)
-_sym_db.RegisterMessage(RPCInput.OptEntry)
-
-RPCOutput = _reflection.GeneratedProtocolMessageType('RPCOutput', (_message.Message,), {
-
-  'OptEntry' : _reflection.GeneratedProtocolMessageType('OptEntry', (_message.Message,), {
-    'DESCRIPTOR' : _RPCOUTPUT_OPTENTRY,
-    '__module__' : 'rpcinput_pb2'
-    # @@protoc_insertion_point(class_scope:pb.RPCOutput.OptEntry)
-    })
-  ,
-  'DESCRIPTOR' : _RPCOUTPUT,
-  '__module__' : 'rpcinput_pb2'
-  # @@protoc_insertion_point(class_scope:pb.RPCOutput)
-  })
-_sym_db.RegisterMessage(RPCOutput)
-_sym_db.RegisterMessage(RPCOutput.OptEntry)
-
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\242\002\005PROTO'
-  _RPCINPUT_OPTENTRY._options = None
-  _RPCINPUT_OPTENTRY._serialized_options = b'8\001'
-  _RPCOUTPUT_OPTENTRY._options = None
-  _RPCOUTPUT_OPTENTRY._serialized_options = b'8\001'
-  _RPCINPUT._serialized_start=23
-  _RPCINPUT._serialized_end=153
-  _RPCINPUT_OPTENTRY._serialized_start=111
-  _RPCINPUT_OPTENTRY._serialized_end=153
-  _RPCOUTPUT._serialized_start=156
-  _RPCOUTPUT._serialized_end=315
-  _RPCOUTPUT_OPTENTRY._serialized_start=111
-  _RPCOUTPUT_OPTENTRY._serialized_end=153
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: rpcinput.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0erpcinput.proto\x12\x02pb\"\x82\x01\n\x08RPCInput\x12\x0b\n\x03obj\x18\x01 \x01(\t\x12\x0c\n\x04\x66unc\x18\x02 \x01(\t\x12\x0b\n\x03req\x18\x03 \x01(\x0c\x12\"\n\x03opt\x18\x04 \x03(\x0b\x32\x15.pb.RPCInput.OptEntry\x1a*\n\x08OptEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9f\x01\n\tRPCOutput\x12\x0b\n\x03ret\x18\x01 \x01(\x05\x12\x0b\n\x03rsp\x18\x02 \x01(\x0c\x12#\n\x03opt\x18\x03 \x03(\x0b\x32\x16.pb.RPCOutput.OptEntry\x12\x0c\n\x04\x64\x65sc\x18\x04 \x01(\t\x12\x0b\n\x03obj\x18\x05 \x01(\t\x12\x0c\n\x04\x66unc\x18\x06 \x01(\t\x1a*\n\x08OptEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x08\xa2\x02\x05PROTOb\x06proto3')
+
+
+
+_RPCINPUT = DESCRIPTOR.message_types_by_name['RPCInput']
+_RPCINPUT_OPTENTRY = _RPCINPUT.nested_types_by_name['OptEntry']
+_RPCOUTPUT = DESCRIPTOR.message_types_by_name['RPCOutput']
+_RPCOUTPUT_OPTENTRY = _RPCOUTPUT.nested_types_by_name['OptEntry']
+RPCInput = _reflection.GeneratedProtocolMessageType('RPCInput', (_message.Message,), {
+
+  'OptEntry' : _reflection.GeneratedProtocolMessageType('OptEntry', (_message.Message,), {
+    'DESCRIPTOR' : _RPCINPUT_OPTENTRY,
+    '__module__' : 'rpcinput_pb2'
+    # @@protoc_insertion_point(class_scope:pb.RPCInput.OptEntry)
+    })
+  ,
+  'DESCRIPTOR' : _RPCINPUT,
+  '__module__' : 'rpcinput_pb2'
+  # @@protoc_insertion_point(class_scope:pb.RPCInput)
+  })
+_sym_db.RegisterMessage(RPCInput)
+_sym_db.RegisterMessage(RPCInput.OptEntry)
+
+RPCOutput = _reflection.GeneratedProtocolMessageType('RPCOutput', (_message.Message,), {
+
+  'OptEntry' : _reflection.GeneratedProtocolMessageType('OptEntry', (_message.Message,), {
+    'DESCRIPTOR' : _RPCOUTPUT_OPTENTRY,
+    '__module__' : 'rpcinput_pb2'
+    # @@protoc_insertion_point(class_scope:pb.RPCOutput.OptEntry)
+    })
+  ,
+  'DESCRIPTOR' : _RPCOUTPUT,
+  '__module__' : 'rpcinput_pb2'
+  # @@protoc_insertion_point(class_scope:pb.RPCOutput)
+  })
+_sym_db.RegisterMessage(RPCOutput)
+_sym_db.RegisterMessage(RPCOutput.OptEntry)
+
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\242\002\005PROTO'
+  _RPCINPUT_OPTENTRY._options = None
+  _RPCINPUT_OPTENTRY._serialized_options = b'8\001'
+  _RPCOUTPUT_OPTENTRY._options = None
+  _RPCOUTPUT_OPTENTRY._serialized_options = b'8\001'
+  _RPCINPUT._serialized_start=23
+  _RPCINPUT._serialized_end=153
+  _RPCINPUT_OPTENTRY._serialized_start=111
+  _RPCINPUT_OPTENTRY._serialized_end=153
+  _RPCOUTPUT._serialized_start=156
+  _RPCOUTPUT._serialized_end=315
+  _RPCOUTPUT_OPTENTRY._serialized_start=111
+  _RPCOUTPUT_OPTENTRY._serialized_end=153
+# @@protoc_insertion_point(module_scope)
```

### Comparing `mecord-cli-0.1.90/mecord/script_template/main.py` & `mecord-cli-0.1.91/mecord/script_template/main.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/script_template/run.py` & `mecord-cli-0.1.91/mecord/script_template/run.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/store.py` & `mecord-cli-0.1.91/mecord/store.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/uauth_common_pb2.py` & `mecord-cli-0.1.91/mecord/uauth_common_pb2.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: uauth_common.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12uauth_common.proto\x12\x08uauth_pb\"B\n\x12UauthLoginPassword\x12\x10\n\x08password\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x03\x12\x0c\n\x04rand\x18\x03 \x01(\x05\"\xc4\x01\n\rDeviceMessage\x12\x0c\n\x04oaid\x18\x01 \x01(\t\x12\x12\n\nandroid_id\x18\x02 \x01(\t\x12\x0c\n\x04idfa\x18\x03 \x01(\t\x12\x0c\n\x04idfv\x18\x04 \x01(\t\x12\x13\n\x0b\x61ppflyer_id\x18\x05 \x01(\t\x12\x0c\n\x04gaid\x18\x06 \x01(\t\x12\x18\n\x10referrer_user_id\x18\x07 \x01(\t\x12\x1f\n\x17\x61\x66_referrer_customer_id\x18\x08 \x01(\t\x12\x17\n\x0f\x61\x66_referrer_uid\x18\t \x01(\t*9\n\x0fUauthWeightType\x12\n\n\x06UWT_H5\x10\x00\x12\r\n\tUWT_INNER\x10\x01\x12\x0b\n\x07UWT_ALL\x10\x02*4\n\x0cUauthPayType\x12\n\n\x06UPT_WX\x10\x00\x12\x0b\n\x07UPT_ALI\x10\x01\x12\x0b\n\x07UPT_ALL\x10\x02*\xde\x02\n\x0fUPayChannelType\x12\r\n\tUPCT_NULL\x10\x00\x12\x11\n\rUPCT_ZFBZF_H5\x10\x02\x12\x12\n\x0eUPCT_ZFBZF_APP\x10\x03\x12\x11\n\rUPCT_WXZF_APP\x10\x04\x12\x10\n\x0cUPCT_WXZF_H5\x10\x05\x12\x0c\n\x08UPCT_IAP\x10\x06\x12\r\n\tUPCT_PLAY\x10\x08\x12\x0e\n\nUPCT_PALZF\x10\n\x12\x0e\n\nUPCT_BOING\x10\x0b\x12\x10\n\x0cUPCT_UNIONZF\x10\x0c\x12\x0f\n\x0bUPCT_CMBPAY\x10\r\x12\x0f\n\x0bUPCT_MYCARD\x10\x0e\x12\x11\n\rUPCT_PAYSSION\x10\x16\x12\x12\n\x0eUPCT_MYCARD_TW\x10\x17\x12\x12\n\x0eUPCT_MYCARD_HK\x10\x18\x12\x0e\n\nUPCT_E_COM\x10(\x12\x0f\n\nUPCT_AGENT\x10\xfd\x01\x12\x10\n\x0bUPCT_MANUAL\x10\xfe\x01\x12\x11\n\x0cUPCT_DEVTEST\x10\xff\x01*\xa3\x03\n\x10UauthAccountType\x12\n\n\x06\x41T_DEV\x10\x00\x12\r\n\tAT_NATIVE\x10\x01\x12\t\n\x05\x41T_QQ\x10\x02\x12\r\n\tAT_WEIXIN\x10\x03\x12\x13\n\x0f\x41T_CHINA_MOBILE\x10\n\x12\x14\n\x10\x41T_CHINA_TELECOM\x10\x0b\x12\x0c\n\x08\x41T_UMENG\x10\x0c\x12\r\n\tAT_GOOGLE\x10\x64\x12\x0f\n\x0b\x41T_FACEBOOK\x10\x65\x12\x0c\n\x08\x41T_CAIJI\x10\x66\x12\x0c\n\x08\x41T_APPLE\x10g\x12\x1a\n\x16\x41T_WECHAT_SUBSCRIPTION\x10h\x12\x16\n\x12\x41T_QQ_MINI_PROGRAM\x10i\x12\x16\n\x12\x41T_WX_MINI_PROGRAM\x10j\x12\r\n\tAT_QQ_WEB\x10k\x12\x11\n\rAT_WEIXIN_WEB\x10l\x12\r\n\x08\x41T_ROBOT\x10\xc8\x01\x12\x18\n\x13\x41T_PHONE_SUBSIDIARY\x10\xcb\x01\x12\r\n\x08\x41T_GUEST\x10\xcc\x01\x12\x0f\n\nAT_TWITTER\x10\xcd\x01\x12\r\n\x08\x41T_EMAIL\x10\xce\x01\x12\x0c\n\x07\x41T_LINE\x10\xcf\x01\x12\x11\n\x0c\x41T_OPERATION\x10\xd2\x01*\xbd\x03\n\x0eUauthLoginType\x12\n\n\x06LT_DEV\x10\x00\x12\r\n\tLT_NATIVE\x10\x01\x12\t\n\x05LT_QQ\x10\x02\x12\r\n\tLT_WEIXIN\x10\x03\x12\n\n\x06LT_SMS\x10\x04\x12\x0c\n\x08LT_QUICK\x10\x05\x12\x0c\n\x08LT_APPLE\x10\x06\x12\x0f\n\x0bLT_FACEBOOK\x10\x07\x12\x15\n\x11LT_PHONE_PASSWORD\x10\x08\x12\x1a\n\x16LT_WECHAT_SUBSCRIPTION\x10\t\x12\r\n\tLT_GOOGLE\x10\n\x12\x17\n\x13LT_QQ_SMALL_PROGRAM\x10\x0b\x12\x16\n\x12LT_WX_MINI_PROGRAM\x10\x0c\x12\r\n\tLT_QQ_WEB\x10\r\x12\x11\n\rLT_WEIXIN_WEB\x10\x0e\x12\x0c\n\x08LT_GUEST\x10\x0f\x12\x0e\n\nLT_TWITTER\x10\x10\x12\n\n\x06LT_SES\x10\x11\x12\x15\n\x11LT_EMAIL_PASSWORD\x10\x12\x12\x15\n\x11LT_REMOTE_MESSAGE\x10\x13\x12\x16\n\x12LT_PROTECT_MESSAGE\x10\x14\x12\x17\n\x13LT_WECHAR_MINI_SCAN\x10\x15\x12\x0b\n\x07LT_LINE\x10\x16\x12\x12\n\x0eLT_QRCODE_SCAN\x10\x17*\xf2\x01\n\x0fUauthDeviceType\x12\x0e\n\nDT_UNKNOWN\x10\x00\x12\x12\n\x0e\x44T_FLASHPLAYER\x10\x01\x12\x14\n\x10\x44T_ANDROID_PHONE\x10\x14\x12\x10\n\x0c\x44T_IOS_PHONE\x10(\x12\x18\n\x14\x44T_WINDOWS_ASSISTANT\x10P\x12\x11\n\rDT_WINDOWS_PC\x10Z\x12\x0c\n\x08\x44T_ROBOT\x10\x64\x12\x1a\n\x16\x44T_WECHAT_SUBSCRIPTION\x10n\x12\x16\n\x12\x44T_QQ_MINI_PROGRAM\x10x\x12\x17\n\x12\x44T_WX_MINI_PROGRAM\x10\x82\x01\x12\x0b\n\x06\x44T_WEB\x10\x8c\x01*1\n\x0cUauthSexType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04MAIL\x10\x01\x12\n\n\x06\x46\x45MAIL\x10\x02*K\n\x11UauthAccountFlags\x12\x0b\n\x07\x41\x46_ZERO\x10\x00\x12\x15\n\x11\x41\x46_PHONE_VERIFIED\x10\x01\x12\x12\n\x0e\x41\x46_BIND_DEVICE\x10\x02\x42\x08\xa2\x02\x05PROTOb\x06proto3')
-
-_UAUTHWEIGHTTYPE = DESCRIPTOR.enum_types_by_name['UauthWeightType']
-UauthWeightType = enum_type_wrapper.EnumTypeWrapper(_UAUTHWEIGHTTYPE)
-_UAUTHPAYTYPE = DESCRIPTOR.enum_types_by_name['UauthPayType']
-UauthPayType = enum_type_wrapper.EnumTypeWrapper(_UAUTHPAYTYPE)
-_UPAYCHANNELTYPE = DESCRIPTOR.enum_types_by_name['UPayChannelType']
-UPayChannelType = enum_type_wrapper.EnumTypeWrapper(_UPAYCHANNELTYPE)
-_UAUTHACCOUNTTYPE = DESCRIPTOR.enum_types_by_name['UauthAccountType']
-UauthAccountType = enum_type_wrapper.EnumTypeWrapper(_UAUTHACCOUNTTYPE)
-_UAUTHLOGINTYPE = DESCRIPTOR.enum_types_by_name['UauthLoginType']
-UauthLoginType = enum_type_wrapper.EnumTypeWrapper(_UAUTHLOGINTYPE)
-_UAUTHDEVICETYPE = DESCRIPTOR.enum_types_by_name['UauthDeviceType']
-UauthDeviceType = enum_type_wrapper.EnumTypeWrapper(_UAUTHDEVICETYPE)
-_UAUTHSEXTYPE = DESCRIPTOR.enum_types_by_name['UauthSexType']
-UauthSexType = enum_type_wrapper.EnumTypeWrapper(_UAUTHSEXTYPE)
-_UAUTHACCOUNTFLAGS = DESCRIPTOR.enum_types_by_name['UauthAccountFlags']
-UauthAccountFlags = enum_type_wrapper.EnumTypeWrapper(_UAUTHACCOUNTFLAGS)
-UWT_H5 = 0
-UWT_INNER = 1
-UWT_ALL = 2
-UPT_WX = 0
-UPT_ALI = 1
-UPT_ALL = 2
-UPCT_NULL = 0
-UPCT_ZFBZF_H5 = 2
-UPCT_ZFBZF_APP = 3
-UPCT_WXZF_APP = 4
-UPCT_WXZF_H5 = 5
-UPCT_IAP = 6
-UPCT_PLAY = 8
-UPCT_PALZF = 10
-UPCT_BOING = 11
-UPCT_UNIONZF = 12
-UPCT_CMBPAY = 13
-UPCT_MYCARD = 14
-UPCT_PAYSSION = 22
-UPCT_MYCARD_TW = 23
-UPCT_MYCARD_HK = 24
-UPCT_E_COM = 40
-UPCT_AGENT = 253
-UPCT_MANUAL = 254
-UPCT_DEVTEST = 255
-AT_DEV = 0
-AT_NATIVE = 1
-AT_QQ = 2
-AT_WEIXIN = 3
-AT_CHINA_MOBILE = 10
-AT_CHINA_TELECOM = 11
-AT_UMENG = 12
-AT_GOOGLE = 100
-AT_FACEBOOK = 101
-AT_CAIJI = 102
-AT_APPLE = 103
-AT_WECHAT_SUBSCRIPTION = 104
-AT_QQ_MINI_PROGRAM = 105
-AT_WX_MINI_PROGRAM = 106
-AT_QQ_WEB = 107
-AT_WEIXIN_WEB = 108
-AT_ROBOT = 200
-AT_PHONE_SUBSIDIARY = 203
-AT_GUEST = 204
-AT_TWITTER = 205
-AT_EMAIL = 206
-AT_LINE = 207
-AT_OPERATION = 210
-LT_DEV = 0
-LT_NATIVE = 1
-LT_QQ = 2
-LT_WEIXIN = 3
-LT_SMS = 4
-LT_QUICK = 5
-LT_APPLE = 6
-LT_FACEBOOK = 7
-LT_PHONE_PASSWORD = 8
-LT_WECHAT_SUBSCRIPTION = 9
-LT_GOOGLE = 10
-LT_QQ_SMALL_PROGRAM = 11
-LT_WX_MINI_PROGRAM = 12
-LT_QQ_WEB = 13
-LT_WEIXIN_WEB = 14
-LT_GUEST = 15
-LT_TWITTER = 16
-LT_SES = 17
-LT_EMAIL_PASSWORD = 18
-LT_REMOTE_MESSAGE = 19
-LT_PROTECT_MESSAGE = 20
-LT_WECHAR_MINI_SCAN = 21
-LT_LINE = 22
-LT_QRCODE_SCAN = 23
-DT_UNKNOWN = 0
-DT_FLASHPLAYER = 1
-DT_ANDROID_PHONE = 20
-DT_IOS_PHONE = 40
-DT_WINDOWS_ASSISTANT = 80
-DT_WINDOWS_PC = 90
-DT_ROBOT = 100
-DT_WECHAT_SUBSCRIPTION = 110
-DT_QQ_MINI_PROGRAM = 120
-DT_WX_MINI_PROGRAM = 130
-DT_WEB = 140
-UNKNOWN = 0
-MAIL = 1
-FEMAIL = 2
-AF_ZERO = 0
-AF_PHONE_VERIFIED = 1
-AF_BIND_DEVICE = 2
-
-
-_UAUTHLOGINPASSWORD = DESCRIPTOR.message_types_by_name['UauthLoginPassword']
-_DEVICEMESSAGE = DESCRIPTOR.message_types_by_name['DeviceMessage']
-UauthLoginPassword = _reflection.GeneratedProtocolMessageType('UauthLoginPassword', (_message.Message,), {
-  'DESCRIPTOR' : _UAUTHLOGINPASSWORD,
-  '__module__' : 'uauth_common_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.UauthLoginPassword)
-  })
-_sym_db.RegisterMessage(UauthLoginPassword)
-
-DeviceMessage = _reflection.GeneratedProtocolMessageType('DeviceMessage', (_message.Message,), {
-  'DESCRIPTOR' : _DEVICEMESSAGE,
-  '__module__' : 'uauth_common_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.DeviceMessage)
-  })
-_sym_db.RegisterMessage(DeviceMessage)
-
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\242\002\005PROTO'
-  _UAUTHWEIGHTTYPE._serialized_start=299
-  _UAUTHWEIGHTTYPE._serialized_end=356
-  _UAUTHPAYTYPE._serialized_start=358
-  _UAUTHPAYTYPE._serialized_end=410
-  _UPAYCHANNELTYPE._serialized_start=413
-  _UPAYCHANNELTYPE._serialized_end=763
-  _UAUTHACCOUNTTYPE._serialized_start=766
-  _UAUTHACCOUNTTYPE._serialized_end=1185
-  _UAUTHLOGINTYPE._serialized_start=1188
-  _UAUTHLOGINTYPE._serialized_end=1633
-  _UAUTHDEVICETYPE._serialized_start=1636
-  _UAUTHDEVICETYPE._serialized_end=1878
-  _UAUTHSEXTYPE._serialized_start=1880
-  _UAUTHSEXTYPE._serialized_end=1929
-  _UAUTHACCOUNTFLAGS._serialized_start=1931
-  _UAUTHACCOUNTFLAGS._serialized_end=2006
-  _UAUTHLOGINPASSWORD._serialized_start=32
-  _UAUTHLOGINPASSWORD._serialized_end=98
-  _DEVICEMESSAGE._serialized_start=101
-  _DEVICEMESSAGE._serialized_end=297
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: uauth_common.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import enum_type_wrapper
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12uauth_common.proto\x12\x08uauth_pb\"B\n\x12UauthLoginPassword\x12\x10\n\x08password\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x03\x12\x0c\n\x04rand\x18\x03 \x01(\x05\"\xc4\x01\n\rDeviceMessage\x12\x0c\n\x04oaid\x18\x01 \x01(\t\x12\x12\n\nandroid_id\x18\x02 \x01(\t\x12\x0c\n\x04idfa\x18\x03 \x01(\t\x12\x0c\n\x04idfv\x18\x04 \x01(\t\x12\x13\n\x0b\x61ppflyer_id\x18\x05 \x01(\t\x12\x0c\n\x04gaid\x18\x06 \x01(\t\x12\x18\n\x10referrer_user_id\x18\x07 \x01(\t\x12\x1f\n\x17\x61\x66_referrer_customer_id\x18\x08 \x01(\t\x12\x17\n\x0f\x61\x66_referrer_uid\x18\t \x01(\t*9\n\x0fUauthWeightType\x12\n\n\x06UWT_H5\x10\x00\x12\r\n\tUWT_INNER\x10\x01\x12\x0b\n\x07UWT_ALL\x10\x02*4\n\x0cUauthPayType\x12\n\n\x06UPT_WX\x10\x00\x12\x0b\n\x07UPT_ALI\x10\x01\x12\x0b\n\x07UPT_ALL\x10\x02*\xde\x02\n\x0fUPayChannelType\x12\r\n\tUPCT_NULL\x10\x00\x12\x11\n\rUPCT_ZFBZF_H5\x10\x02\x12\x12\n\x0eUPCT_ZFBZF_APP\x10\x03\x12\x11\n\rUPCT_WXZF_APP\x10\x04\x12\x10\n\x0cUPCT_WXZF_H5\x10\x05\x12\x0c\n\x08UPCT_IAP\x10\x06\x12\r\n\tUPCT_PLAY\x10\x08\x12\x0e\n\nUPCT_PALZF\x10\n\x12\x0e\n\nUPCT_BOING\x10\x0b\x12\x10\n\x0cUPCT_UNIONZF\x10\x0c\x12\x0f\n\x0bUPCT_CMBPAY\x10\r\x12\x0f\n\x0bUPCT_MYCARD\x10\x0e\x12\x11\n\rUPCT_PAYSSION\x10\x16\x12\x12\n\x0eUPCT_MYCARD_TW\x10\x17\x12\x12\n\x0eUPCT_MYCARD_HK\x10\x18\x12\x0e\n\nUPCT_E_COM\x10(\x12\x0f\n\nUPCT_AGENT\x10\xfd\x01\x12\x10\n\x0bUPCT_MANUAL\x10\xfe\x01\x12\x11\n\x0cUPCT_DEVTEST\x10\xff\x01*\xa3\x03\n\x10UauthAccountType\x12\n\n\x06\x41T_DEV\x10\x00\x12\r\n\tAT_NATIVE\x10\x01\x12\t\n\x05\x41T_QQ\x10\x02\x12\r\n\tAT_WEIXIN\x10\x03\x12\x13\n\x0f\x41T_CHINA_MOBILE\x10\n\x12\x14\n\x10\x41T_CHINA_TELECOM\x10\x0b\x12\x0c\n\x08\x41T_UMENG\x10\x0c\x12\r\n\tAT_GOOGLE\x10\x64\x12\x0f\n\x0b\x41T_FACEBOOK\x10\x65\x12\x0c\n\x08\x41T_CAIJI\x10\x66\x12\x0c\n\x08\x41T_APPLE\x10g\x12\x1a\n\x16\x41T_WECHAT_SUBSCRIPTION\x10h\x12\x16\n\x12\x41T_QQ_MINI_PROGRAM\x10i\x12\x16\n\x12\x41T_WX_MINI_PROGRAM\x10j\x12\r\n\tAT_QQ_WEB\x10k\x12\x11\n\rAT_WEIXIN_WEB\x10l\x12\r\n\x08\x41T_ROBOT\x10\xc8\x01\x12\x18\n\x13\x41T_PHONE_SUBSIDIARY\x10\xcb\x01\x12\r\n\x08\x41T_GUEST\x10\xcc\x01\x12\x0f\n\nAT_TWITTER\x10\xcd\x01\x12\r\n\x08\x41T_EMAIL\x10\xce\x01\x12\x0c\n\x07\x41T_LINE\x10\xcf\x01\x12\x11\n\x0c\x41T_OPERATION\x10\xd2\x01*\xbd\x03\n\x0eUauthLoginType\x12\n\n\x06LT_DEV\x10\x00\x12\r\n\tLT_NATIVE\x10\x01\x12\t\n\x05LT_QQ\x10\x02\x12\r\n\tLT_WEIXIN\x10\x03\x12\n\n\x06LT_SMS\x10\x04\x12\x0c\n\x08LT_QUICK\x10\x05\x12\x0c\n\x08LT_APPLE\x10\x06\x12\x0f\n\x0bLT_FACEBOOK\x10\x07\x12\x15\n\x11LT_PHONE_PASSWORD\x10\x08\x12\x1a\n\x16LT_WECHAT_SUBSCRIPTION\x10\t\x12\r\n\tLT_GOOGLE\x10\n\x12\x17\n\x13LT_QQ_SMALL_PROGRAM\x10\x0b\x12\x16\n\x12LT_WX_MINI_PROGRAM\x10\x0c\x12\r\n\tLT_QQ_WEB\x10\r\x12\x11\n\rLT_WEIXIN_WEB\x10\x0e\x12\x0c\n\x08LT_GUEST\x10\x0f\x12\x0e\n\nLT_TWITTER\x10\x10\x12\n\n\x06LT_SES\x10\x11\x12\x15\n\x11LT_EMAIL_PASSWORD\x10\x12\x12\x15\n\x11LT_REMOTE_MESSAGE\x10\x13\x12\x16\n\x12LT_PROTECT_MESSAGE\x10\x14\x12\x17\n\x13LT_WECHAR_MINI_SCAN\x10\x15\x12\x0b\n\x07LT_LINE\x10\x16\x12\x12\n\x0eLT_QRCODE_SCAN\x10\x17*\xf2\x01\n\x0fUauthDeviceType\x12\x0e\n\nDT_UNKNOWN\x10\x00\x12\x12\n\x0e\x44T_FLASHPLAYER\x10\x01\x12\x14\n\x10\x44T_ANDROID_PHONE\x10\x14\x12\x10\n\x0c\x44T_IOS_PHONE\x10(\x12\x18\n\x14\x44T_WINDOWS_ASSISTANT\x10P\x12\x11\n\rDT_WINDOWS_PC\x10Z\x12\x0c\n\x08\x44T_ROBOT\x10\x64\x12\x1a\n\x16\x44T_WECHAT_SUBSCRIPTION\x10n\x12\x16\n\x12\x44T_QQ_MINI_PROGRAM\x10x\x12\x17\n\x12\x44T_WX_MINI_PROGRAM\x10\x82\x01\x12\x0b\n\x06\x44T_WEB\x10\x8c\x01*1\n\x0cUauthSexType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04MAIL\x10\x01\x12\n\n\x06\x46\x45MAIL\x10\x02*K\n\x11UauthAccountFlags\x12\x0b\n\x07\x41\x46_ZERO\x10\x00\x12\x15\n\x11\x41\x46_PHONE_VERIFIED\x10\x01\x12\x12\n\x0e\x41\x46_BIND_DEVICE\x10\x02\x42\x08\xa2\x02\x05PROTOb\x06proto3')
+
+_UAUTHWEIGHTTYPE = DESCRIPTOR.enum_types_by_name['UauthWeightType']
+UauthWeightType = enum_type_wrapper.EnumTypeWrapper(_UAUTHWEIGHTTYPE)
+_UAUTHPAYTYPE = DESCRIPTOR.enum_types_by_name['UauthPayType']
+UauthPayType = enum_type_wrapper.EnumTypeWrapper(_UAUTHPAYTYPE)
+_UPAYCHANNELTYPE = DESCRIPTOR.enum_types_by_name['UPayChannelType']
+UPayChannelType = enum_type_wrapper.EnumTypeWrapper(_UPAYCHANNELTYPE)
+_UAUTHACCOUNTTYPE = DESCRIPTOR.enum_types_by_name['UauthAccountType']
+UauthAccountType = enum_type_wrapper.EnumTypeWrapper(_UAUTHACCOUNTTYPE)
+_UAUTHLOGINTYPE = DESCRIPTOR.enum_types_by_name['UauthLoginType']
+UauthLoginType = enum_type_wrapper.EnumTypeWrapper(_UAUTHLOGINTYPE)
+_UAUTHDEVICETYPE = DESCRIPTOR.enum_types_by_name['UauthDeviceType']
+UauthDeviceType = enum_type_wrapper.EnumTypeWrapper(_UAUTHDEVICETYPE)
+_UAUTHSEXTYPE = DESCRIPTOR.enum_types_by_name['UauthSexType']
+UauthSexType = enum_type_wrapper.EnumTypeWrapper(_UAUTHSEXTYPE)
+_UAUTHACCOUNTFLAGS = DESCRIPTOR.enum_types_by_name['UauthAccountFlags']
+UauthAccountFlags = enum_type_wrapper.EnumTypeWrapper(_UAUTHACCOUNTFLAGS)
+UWT_H5 = 0
+UWT_INNER = 1
+UWT_ALL = 2
+UPT_WX = 0
+UPT_ALI = 1
+UPT_ALL = 2
+UPCT_NULL = 0
+UPCT_ZFBZF_H5 = 2
+UPCT_ZFBZF_APP = 3
+UPCT_WXZF_APP = 4
+UPCT_WXZF_H5 = 5
+UPCT_IAP = 6
+UPCT_PLAY = 8
+UPCT_PALZF = 10
+UPCT_BOING = 11
+UPCT_UNIONZF = 12
+UPCT_CMBPAY = 13
+UPCT_MYCARD = 14
+UPCT_PAYSSION = 22
+UPCT_MYCARD_TW = 23
+UPCT_MYCARD_HK = 24
+UPCT_E_COM = 40
+UPCT_AGENT = 253
+UPCT_MANUAL = 254
+UPCT_DEVTEST = 255
+AT_DEV = 0
+AT_NATIVE = 1
+AT_QQ = 2
+AT_WEIXIN = 3
+AT_CHINA_MOBILE = 10
+AT_CHINA_TELECOM = 11
+AT_UMENG = 12
+AT_GOOGLE = 100
+AT_FACEBOOK = 101
+AT_CAIJI = 102
+AT_APPLE = 103
+AT_WECHAT_SUBSCRIPTION = 104
+AT_QQ_MINI_PROGRAM = 105
+AT_WX_MINI_PROGRAM = 106
+AT_QQ_WEB = 107
+AT_WEIXIN_WEB = 108
+AT_ROBOT = 200
+AT_PHONE_SUBSIDIARY = 203
+AT_GUEST = 204
+AT_TWITTER = 205
+AT_EMAIL = 206
+AT_LINE = 207
+AT_OPERATION = 210
+LT_DEV = 0
+LT_NATIVE = 1
+LT_QQ = 2
+LT_WEIXIN = 3
+LT_SMS = 4
+LT_QUICK = 5
+LT_APPLE = 6
+LT_FACEBOOK = 7
+LT_PHONE_PASSWORD = 8
+LT_WECHAT_SUBSCRIPTION = 9
+LT_GOOGLE = 10
+LT_QQ_SMALL_PROGRAM = 11
+LT_WX_MINI_PROGRAM = 12
+LT_QQ_WEB = 13
+LT_WEIXIN_WEB = 14
+LT_GUEST = 15
+LT_TWITTER = 16
+LT_SES = 17
+LT_EMAIL_PASSWORD = 18
+LT_REMOTE_MESSAGE = 19
+LT_PROTECT_MESSAGE = 20
+LT_WECHAR_MINI_SCAN = 21
+LT_LINE = 22
+LT_QRCODE_SCAN = 23
+DT_UNKNOWN = 0
+DT_FLASHPLAYER = 1
+DT_ANDROID_PHONE = 20
+DT_IOS_PHONE = 40
+DT_WINDOWS_ASSISTANT = 80
+DT_WINDOWS_PC = 90
+DT_ROBOT = 100
+DT_WECHAT_SUBSCRIPTION = 110
+DT_QQ_MINI_PROGRAM = 120
+DT_WX_MINI_PROGRAM = 130
+DT_WEB = 140
+UNKNOWN = 0
+MAIL = 1
+FEMAIL = 2
+AF_ZERO = 0
+AF_PHONE_VERIFIED = 1
+AF_BIND_DEVICE = 2
+
+
+_UAUTHLOGINPASSWORD = DESCRIPTOR.message_types_by_name['UauthLoginPassword']
+_DEVICEMESSAGE = DESCRIPTOR.message_types_by_name['DeviceMessage']
+UauthLoginPassword = _reflection.GeneratedProtocolMessageType('UauthLoginPassword', (_message.Message,), {
+  'DESCRIPTOR' : _UAUTHLOGINPASSWORD,
+  '__module__' : 'uauth_common_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.UauthLoginPassword)
+  })
+_sym_db.RegisterMessage(UauthLoginPassword)
+
+DeviceMessage = _reflection.GeneratedProtocolMessageType('DeviceMessage', (_message.Message,), {
+  'DESCRIPTOR' : _DEVICEMESSAGE,
+  '__module__' : 'uauth_common_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.DeviceMessage)
+  })
+_sym_db.RegisterMessage(DeviceMessage)
+
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\242\002\005PROTO'
+  _UAUTHWEIGHTTYPE._serialized_start=299
+  _UAUTHWEIGHTTYPE._serialized_end=356
+  _UAUTHPAYTYPE._serialized_start=358
+  _UAUTHPAYTYPE._serialized_end=410
+  _UPAYCHANNELTYPE._serialized_start=413
+  _UPAYCHANNELTYPE._serialized_end=763
+  _UAUTHACCOUNTTYPE._serialized_start=766
+  _UAUTHACCOUNTTYPE._serialized_end=1185
+  _UAUTHLOGINTYPE._serialized_start=1188
+  _UAUTHLOGINTYPE._serialized_end=1633
+  _UAUTHDEVICETYPE._serialized_start=1636
+  _UAUTHDEVICETYPE._serialized_end=1878
+  _UAUTHSEXTYPE._serialized_start=1880
+  _UAUTHSEXTYPE._serialized_end=1929
+  _UAUTHACCOUNTFLAGS._serialized_start=1931
+  _UAUTHACCOUNTFLAGS._serialized_end=2006
+  _UAUTHLOGINPASSWORD._serialized_start=32
+  _UAUTHLOGINPASSWORD._serialized_end=98
+  _DEVICEMESSAGE._serialized_start=101
+  _DEVICEMESSAGE._serialized_end=297
+# @@protoc_insertion_point(module_scope)
```

### Comparing `mecord-cli-0.1.90/mecord/uauth_ext_pb2.py` & `mecord-cli-0.1.91/mecord/uauth_ext_pb2.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,1664 +1,1664 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: uauth_ext.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from mecord import uauth_common_pb2 as uauth__common__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fuauth_ext.proto\x12\x08uauth_pb\x1a\x12uauth_common.proto\"m\n\x0cVerifyIAPReq\x12\x11\n\taccountId\x18\x01 \x01(\x03\x12\x0f\n\x07receipt\x18\x02 \x01(\t\x12\x15\n\rtransactionId\x18\x03 \x01(\t\x12\x10\n\x08order_no\x18\x04 \x01(\t\x12\x10\n\x08goods_id\x18\x05 \x01(\t\"\x0e\n\x0cVerifyIAPRes\"a\n\x08GoldCard\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x05\x12\r\n\x05golds\x18\x03 \x01(\x05\x12\x16\n\x0egiveaway_golds\x18\x04 \x01(\x05\x12\x12\n\nidentifier\x18\x05 \x01(\t\"\x10\n\x0eGetGoodListReq\"H\n\x0eGetGoodListRes\x12%\n\tgood_list\x18\x01 \x03(\x0b\x32\x12.uauth_pb.GoldCard\x12\x0f\n\x07version\x18\x02 \x01(\x05\",\n\x0bOrderIAPReq\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x11\n\taccountId\x18\x02 \x01(\x03\"\x1f\n\x0bOrderIAPRes\x12\x10\n\x08order_no\x18\x01 \x01(\t\"M\n\x10\x43loseOrderIAPReq\x12\x10\n\x08order_no\x18\x01 \x01(\t\x12\'\n\x06status\x18\x02 \x01(\x0e\x32\x17.uauth_pb.IAPStatusType\"\x12\n\x10\x43loseOrderIAPRes\"%\n\x17VIPChargeAccountInfoReq\x12\n\n\x02id\x18\x01 \x01(\x03\"\x8d\x01\n\x17VIPChargeAccountInfoRes\x12\x10\n\x08\x64ue_bank\x18\x01 \x01(\t\x12\r\n\x05payee\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x63\x63ount_number\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65posit_bank\x18\x04 \x01(\t\x12\x10\n\x08nickname\x18\x05 \x01(\t\x12\x11\n\tplayer_id\x18\x06 \x01(\x03\"\x11\n\x0fVIPChargeLogReq\"8\n\x0fVIPChargeLogRes\x12%\n\x04list\x18\x01 \x03(\x0b\x32\x17.uauth_pb.VIPChargeLogs\"C\n\rVIPChargeLogs\x12\x0b\n\x03\x64\x61y\x18\x01 \x01(\t\x12%\n\x04list\x18\x02 \x03(\x0b\x32\x17.uauth_pb.VIPChargeItem\"x\n\rVIPChargeItem\x12\x11\n\tcharge_at\x18\x01 \x01(\x03\x12\x11\n\tfinish_at\x18\x02 \x01(\x03\x12\x0b\n\x03rmb\x18\x03 \x01(\x03\x12\x0c\n\x04gold\x18\x04 \x01(\x03\x12&\n\x06status\x18\x05 \x01(\x0e\x32\x16.uauth_pb.ChargeStatus\"E\n\rReportDataReq\x12&\n\x04type\x18\x01 \x01(\x0e\x32\x18.uauth_pb.ReportDataType\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x0f\n\rReportDataRes\"\xf8\x02\n\x0cGetChargeReq\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x12\n\naccount_id\x18\x02 \x01(\x03\x12+\n\x08pay_type\x18\x03 \x01(\x0e\x32\x19.uauth_pb.UPayChannelType\x12\x0c\n\x04gold\x18\x04 \x01(\x03\x12\x0e\n\x06remark\x18\x05 \x01(\t\x12\x34\n\x07\x65xtends\x18\x06 \x03(\x0b\x32#.uauth_pb.GetChargeReq.ExtendsEntry\x12\x39\n\nextra_data\x18\x07 \x03(\x0b\x32%.uauth_pb.GetChargeReq.ExtraDataEntry\x12\x10\n\x08sub_type\x18\x08 \x01(\t\x12\x12\n\nreturn_url\x18\t \x01(\t\x1a.\n\x0c\x45xtendsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x30\n\x0e\x45xtraDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"P\n\x0cGetChargeRes\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65tail\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\t\x12\x14\n\x0credirect_url\x18\x04 \x01(\t\"r\n\rGetSmsCodeReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\x10\n\x08phone_no\x18\x02 \x01(\t\x12\x12\n\nphone_sign\x18\x03 \x01(\t\x12*\n\x0csms_code_tpl\x18\x04 \x01(\x0e\x32\x14.uauth_pb.SMSCodeTpl\"\x0f\n\rGetSmsCodeRes\"\x85\x01\n\x0eGetSmsTokenReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\x10\n\x08phone_no\x18\x02 \x01(\t\x12\x10\n\x08sms_code\x18\x03 \x01(\t\x12\x12\n\nphone_sign\x18\x04 \x01(\t\x12*\n\x0csms_code_tpl\x18\x05 \x01(\x0e\x32\x14.uauth_pb.SMSCodeTpl\"#\n\x0eGetSmsTokenRes\x12\x11\n\tsms_token\x18\x01 \x01(\t\"=\n\x0fPhoneSmsCodeReq\x12*\n\x0csms_code_tpl\x18\x01 \x01(\x0e\x32\x14.uauth_pb.SMSCodeTpl\"\x11\n\x0fPhoneSmsCodeRes\"T\n\x14\x43heckPhoneSmsCodeReq\x12*\n\x0csms_code_tpl\x18\x01 \x01(\x0e\x32\x14.uauth_pb.SMSCodeTpl\x12\x10\n\x08sms_code\x18\x02 \x01(\t\"\x16\n\x14\x43heckPhoneSmsCodeRes\"\xde\x01\n\x0f\x43ommonSignInRes\x12\x13\n\x0blogin_token\x18\x01 \x01(\t\x12\x0e\n\x06is_new\x18\x02 \x01(\x08\x12\x0f\n\x07user_id\x18\x03 \x01(\x12\x12\x37\n\x07\x65xtends\x18\x04 \x03(\x0b\x32&.uauth_pb.CommonSignInRes.ExtendsEntry\x12,\n\nlogin_type\x18\x05 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x1a.\n\x0c\x45xtendsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xce\x01\n\x12SignInWithAppleReq\x12\x16\n\x0eidentity_token\x18\x01 \x01(\t\x12\x1a\n\x12\x61uthorization_code\x18\x02 \x01(\t\x12\x11\n\tfull_name\x18\x03 \x01(\t\x12\x11\n\tdevice_id\x18\x04 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x05 \x01(\t\x12\x13\n\x0byidun_token\x18\x06 \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x07 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\x95\x01\n\x11IdOrPhoneLoginReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x0c\n\x04sign\x18\x04 \x01(\t\x12\x11\n\tdevice_id\x18\x05 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x06 \x01(\t\x12\x13\n\x0byidun_token\x18\x07 \x01(\t\"\xa3\x02\n\x14LoginWithPhoneSMSReq\x12\r\n\x05phone\x18\x01 \x01(\t\x12\x11\n\tsms_token\x18\x02 \x01(\t\x12\x11\n\tdevice_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x05 \x01(\x05\x12\x10\n\x08sms_code\x18\x06 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x08 \x01(\t\x12\x13\n\x0byidun_token\x18\t \x01(\t\x12\x12\n\nphone_sign\x18\n \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x0b \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\x12*\n\x0csms_code_tpl\x18\x0c \x01(\x0e\x32\x14.uauth_pb.SMSCodeTpl\"\xa0\x02\n\rThirdLoginReq\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x11\n\tdevice_id\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x05 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x06 \x01(\x05\x12,\n\nlogin_type\x18\x07 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12\x18\n\x10u_meng_device_id\x18\x08 \x01(\t\x12\x13\n\x0byidun_token\x18\t \x01(\t\x12\x14\n\x0ctoken_secret\x18\n \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x0b \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\xd2\x01\n\x18\x43hinaMobileQuickLoginReq\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\x12\x11\n\tdevice_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x05 \x01(\x05\x12\x18\n\x10u_meng_device_id\x18\x06 \x01(\t\x12\x13\n\x0byidun_token\x18\x07 \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x08 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\xc4\x01\n\x13\x43hinaTelecomAuthReq\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12\x11\n\tdevice_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x05 \x01(\x05\x12\x18\n\x10u_meng_device_id\x18\x06 \x01(\t\x12\x13\n\x0byidun_token\x18\x07 \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x08 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\xcd\x01\n\x12UmengQuickLoginReq\x12\x0f\n\x07\x61pp_key\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\x12\x11\n\tdevice_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x05 \x01(\x05\x12\x18\n\x10u_meng_device_id\x18\x08 \x01(\t\x12\x13\n\x0byidun_token\x18\t \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\n \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\xb4\x01\n\x0b\x44\x65vLoginReq\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tdevice_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x05 \x01(\x05\x12\x18\n\x10u_meng_device_id\x18\x06 \x01(\t\x12\x13\n\x0byidun_token\x18\x07 \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x08 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\x8f\x01\n\x10ResetPasswordReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\x10\n\x08phone_no\x18\x02 \x01(\t\x12\x11\n\tsms_token\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x0c\n\x04sign\x18\x05 \x01(\t\x12\x12\n\nphone_sign\x18\x06 \x01(\t\x12\x11\n\tplayer_id\x18\x07 \x01(\x03\"\x12\n\x10ResetPasswordRes\"\x10\n\x0eLoginSecretReq\"\x1d\n\x0eLoginSecretRes\x12\x0b\n\x03key\x18\x01 \x01(\t\"W\n\x0fUpdatePasswdReq\x12\x12\n\nold_passwd\x18\x01 \x01(\t\x12\x12\n\nnew_passwd\x18\x02 \x01(\t\x12\x0c\n\x04sign\x18\x03 \x01(\t\x12\x0e\n\x06is_new\x18\x04 \x01(\x08\"\x11\n\x0fUpdatePasswdRes\"<\n\tInviteReq\x12\x11\n\tplayer_id\x18\x01 \x01(\x03\x12\x0c\n\x04type\x18\x02 \x01(\x05\x12\x0e\n\x06\x65xtend\x18\x03 \x01(\t\"\x0b\n\tInviteRes\"\x10\n\x0eGetSyncTimeReq\"\x10\n\x0eGetSyncTimeRes\";\n\x14ReportBuyNobilityReq\x12\x0f\n\x07room_id\x18\x01 \x01(\x03\x12\x12\n\nbenefit_id\x18\x02 \x01(\x03\"\x16\n\x14ReportBuyNobilityRes\"\xb3\x01\n\x12GoogleIABNotifyReq\x12\x0f\n\x07user_id\x18\x01 \x01(\x03\x12\x14\n\x0cpackage_name\x18\x02 \x01(\t\x12:\n\nbuy_intent\x18\x03 \x01(\x0b\x32&.uauth_pb.GoogleIABNotifyReq.BuyIntent\x1a:\n\tBuyIntent\x12\x15\n\rpurchase_data\x18\x01 \x01(\t\x12\x16\n\x0e\x64\x61ta_signature\x18\x02 \x01(\t\"\x14\n\x12GoogleIABNotifyRes\"M\n\x14GoogleIABProductItem\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05price\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x04 \x01(\t\"\x1a\n\x18GoogleIABProductItemsReq\"I\n\x18GoogleIABProductItemsRes\x12-\n\x05items\x18\x01 \x03(\x0b\x32\x1e.uauth_pb.GoogleIABProductItem\"\x13\n\x11GetWeChatAppIdReq\"#\n\x11GetWeChatAppIdRes\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\"#\n\x13GetWeChatIdLoginReq\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"G\n\x13GetWeChatIdLoginRes\x12\r\n\x05token\x18\x01 \x01(\t\x12\x10\n\x08union_id\x18\x02 \x01(\t\x12\x0f\n\x07open_id\x18\x03 \x01(\t\":\n\x08UserInfo\x12\x10\n\x08nickname\x18\x01 \x01(\t\x12\x0c\n\x04icon\x18\x02 \x01(\t\x12\x0e\n\x06gender\x18\x03 \x01(\x05\"\xf0\x01\n\x16GetMiniProgramLoginReq\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\r\n\x05\x61ppid\x18\x02 \x01(\t\x12,\n\nlogin_type\x18\x03 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12%\n\tuser_info\x18\x04 \x01(\x0b\x32\x12.uauth_pb.UserInfo\x12\x16\n\x0e\x65ncrypted_data\x18\x05 \x01(\t\x12\n\n\x02iv\x18\x06 \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x07 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\x12\x0f\n\x07\x63ode_id\x18\x08 \x01(\t\"u\n\x13MiniProgramPhoneReq\x12\x16\n\x0e\x65ncrypted_data\x18\x01 \x01(\t\x12\n\n\x02iv\x18\x02 \x01(\t\x12,\n\nlogin_type\x18\x03 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\"\x15\n\x13MiniProgramPhoneRes\"]\n\x0f\x41pplyCertifyReq\x12+\n\x0c\x63\x65rtify_type\x18\x01 \x01(\x0e\x32\x15.uauth_pb.CertifyType\x12\x0f\n\x07id_card\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"b\n\x0f\x41pplyCertifyRes\x12\x0f\n\x07\x66\x61\x63\x65_id\x18\x01 \x01(\t\x12\x10\n\x08trade_no\x18\x02 \x01(\t\x12\r\n\x05nonce\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0c\n\x04sign\x18\x05 \x01(\t\"\x8a\x01\n\x13\x41pplyCertifySignReq\x12+\n\x0c\x63\x65rtify_type\x18\x01 \x01(\x0e\x32\x15.uauth_pb.CertifyType\x12\x0f\n\x07id_card\x18\x02 \x01(\t\x12\x14\n\x0cid_card_sign\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x11\n\tname_sign\x18\x05 \x01(\t\"\x12\n\x10\x43\x65rtifyResultReq\"^\n\x10\x43\x65rtifyResultRes\x12+\n\x0c\x63\x65rtify_type\x18\x01 \x01(\x0e\x32\x15.uauth_pb.CertifyType\x12\x0f\n\x07id_card\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"\x18\n\x16\x41\x63\x63ountPhoneSmsCodeReq\"\x18\n\x16\x41\x63\x63ountPhoneSmsCodeRes\"\xc6\x01\n\x19\x41\x63\x63ountSubsidiaryLoginReq\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\x05\x12\x10\n\x08sms_code\x18\x04 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x05 \x01(\t\x12\x13\n\x0byidun_token\x18\x06 \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x07 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\x8a\x01\n\x10GetGuestLoginReq\x12\x11\n\tguest_key\x18\x01 \x01(\t\x12\x0c\n\x04sign\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x03 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x04 \x01(\x05\x12/\n\x0e\x64\x65vice_message\x18\x05 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"a\n\x16\x41\x63\x63ountBindPhoneSMSReq\x12\r\n\x05phone\x18\x01 \x01(\t\x12\x10\n\x08sms_code\x18\x02 \x01(\t\x12\x12\n\nverify_old\x18\x03 \x01(\x08\x12\x12\n\nphone_sign\x18\x04 \x01(\t\"\x18\n\x16\x41\x63\x63ountBindPhoneSMSRes\"\x8d\x01\n\x13\x41\x63\x63ountBindThirdReq\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12,\n\nlogin_type\x18\x04 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12\x14\n\x0ctoken_secret\x18\x05 \x01(\t\"\x15\n\x13\x41\x63\x63ountBindThirdRes\"\x14\n\x12\x41\x63\x63ountBindListReq\"Z\n\x12\x41\x63\x63ountBindListRes\x12&\n\x04list\x18\x01 \x03(\x0e\x32\x18.uauth_pb.UauthLoginType\x12\r\n\x05phone\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\"`\n\x13\x42indPhoneSmsCodeReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\x10\n\x08phone_no\x18\x02 \x01(\t\x12\x12\n\nverify_old\x18\x03 \x01(\x08\x12\x12\n\nphone_sign\x18\x04 \x01(\t\"\x15\n\x13\x42indPhoneSmsCodeRes\"L\n\x13\x42indEmailSesCodeReq\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x12\n\nemail_sign\x18\x02 \x01(\t\x12\x12\n\nverify_old\x18\x03 \x01(\x08\"\x15\n\x13\x42indEmailSesCodeRes\"a\n\x16\x41\x63\x63ountBindEmailSESReq\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x12\n\nemail_sign\x18\x02 \x01(\t\x12\x10\n\x08ses_code\x18\x03 \x01(\t\x12\x12\n\nverify_old\x18\x04 \x01(\x08\"\x18\n\x16\x41\x63\x63ountBindEmailSESRes\"\xe2\x01\n\x15GetAccountRegisterReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x04 \x01(\x05\x12\x10\n\x08nickname\x18\x05 \x01(\t\x12/\n\rregister_type\x18\x06 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12\x0c\n\x04\x63ode\x18\x07 \x01(\t\x12\x0c\n\x04sign\x18\x08 \x01(\t\x12\x12\n\nvalue_sign\x18\t \x01(\t\x12\x0f\n\x07\x63hannel\x18\n \x01(\x05\"\xb3\x01\n\x1aGetAccountPasswordLoginReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12,\n\nlogin_type\x18\x04 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12\x13\n\x0b\x64\x65vice_type\x18\x05 \x01(\x05\x12\x0c\n\x04sign\x18\x06 \x01(\t\x12\x12\n\nvalue_sign\x18\x07 \x01(\t\"2\n\rGetSesCodeReq\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x12\n\nemail_sign\x18\x02 \x01(\t\"\x0f\n\rGetSesCodeRes\"E\n\x0eGetSesTokenReq\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x12\n\nemail_sign\x18\x02 \x01(\t\x12\x10\n\x08ses_code\x18\x03 \x01(\t\"#\n\x0eGetSesTokenRes\x12\x11\n\tses_token\x18\x01 \x01(\t\"m\n\x15ResetPasswordBySesReq\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x12\n\nemail_sign\x18\x02 \x01(\t\x12\x11\n\tses_token\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x0c\n\x04sign\x18\x05 \x01(\t\"\x17\n\x15ResetPasswordBySesRes\")\n\x16RemoteLoginSendCodeReq\x12\x0f\n\x07user_id\x18\x01 \x01(\x12\"\x18\n\x16RemoteLoginSendCodeRes\":\n\x19RemoteLoginConfirmCodeReq\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x02 \x01(\x12\"C\n\x19RemoteLoginConfirmCodeRes\x12&\n\x03res\x18\x01 \x01(\x0b\x32\x19.uauth_pb.CommonSignInRes\"T\n\x1eVerifyCancelSignInWithAppleReq\x12\x16\n\x0eidentity_token\x18\x01 \x01(\t\x12\x1a\n\x12\x61uthorization_code\x18\x02 \x01(\t\" \n\x1eVerifyCancelSignInWithAppleRes\"*\n\x18WechatCodeLoginTicketReq\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\"*\n\x18WechatCodeLoginTicketRes\x12\x0e\n\x06ticket\x18\x01 \x01(\t\"&\n\x14GetWechatMiniCodeReq\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\"5\n\x14GetWechatMiniCodeRes\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63ode_id\x18\x02 \x01(\t\"A\n\x18GetWechatMiniCodeScanReq\x12\x0f\n\x07\x63ode_id\x18\x01 \x01(\t\x12\x14\n\x0c\x63ode_id_sign\x18\x02 \x01(\t\"}\n\x18GetWechatMiniCodeScanRes\x12\x32\n\x06status\x18\x01 \x01(\x0e\x32\".uauth_pb.WechatMiniCodeScanStatus\x12-\n\nlogin_data\x18\x02 \x01(\x0b\x32\x19.uauth_pb.CommonSignInRes\"(\n\x15RefusePhoneLicenseReq\x12\x0f\n\x07\x63ode_id\x18\x01 \x01(\t\"\x17\n\x15RefusePhoneLicenseRes\"5\n\x16WechatMiniBindPhoneReq\x12\r\n\x05\x61ppid\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"\x18\n\x16WechatMiniBindPhoneRes\".\n\x1aThirdAccountBindWeChatInfo\x12\x10\n\x08nickname\x18\x01 \x01(\t\"*\n\x16ThirdAccountBindQqInfo\x12\x10\n\x08nickname\x18\x02 \x01(\t\"\x95\x01\n\x14ThirdAccountBindInfo\x12;\n\x0bwechat_info\x18\x01 \x01(\x0b\x32$.uauth_pb.ThirdAccountBindWeChatInfoH\x00\x12\x33\n\x07qq_info\x18\x02 \x01(\x0b\x32 .uauth_pb.ThirdAccountBindQqInfoH\x00\x42\x0b\n\tbind_info\"{\n\x18ThirdAccountBindInfoData\x12\x31\n\tbind_type\x18\x01 \x01(\x0e\x32\x1e.uauth_pb.ThirdAccountBindType\x12,\n\x04info\x18\x02 \x01(\x0b\x32\x1e.uauth_pb.ThirdAccountBindInfo\"\x19\n\x17ThirdAccountBindInfoReq\"P\n\x17ThirdAccountBindInfoRes\x12\x35\n\tinfo_data\x18\x01 \x03(\x0b\x32\".uauth_pb.ThirdAccountBindInfoData\"|\n\x13\x42indThirdAccountReq\x12\x31\n\tbind_type\x18\x01 \x01(\x0e\x32\x1e.uauth_pb.ThirdAccountBindType\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x04 \x01(\t\"\x15\n\x13\x42indThirdAccountRes\"`\n\x15UnbindThirdAccountReq\x12\x35\n\x08opt_type\x18\x01 \x01(\x0e\x32#.uauth_pb.UnbindThirdAccountOptType\x12\x10\n\x08sms_code\x18\x02 \x01(\t\"\x17\n\x15UnbindThirdAccountRes\"\xa2\x01\n\x15GetQrcodeLoginCodeReq\x12,\n\nlogin_type\x18\x01 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12.\n\x0b\x64\x65vice_type\x18\x02 \x01(\x0e\x32\x19.uauth_pb.UauthDeviceType\x12\x11\n\tdevice_id\x18\x03 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x04 \x01(\t\"+\n\x15GetQrcodeLoginCodeRes\x12\x12\n\nlogin_code\x18\x01 \x01(\t\"a\n\x12QrcodeScanLoginReq\x12\x12\n\nlogin_code\x18\x01 \x01(\t\x12\x17\n\x0flogin_device_id\x18\x02 \x01(\t\x12\x1e\n\x16login_u_meng_device_id\x18\x03 \x01(\t\"\x14\n\x12QrcodeScanLoginRes\"Z\n\x17GetQrcodeLoginStatusReq\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x02 \x01(\t\x12\x12\n\nlogin_code\x18\x03 \x01(\t\"\xa8\x01\n\x17GetQrcodeLoginStatusRes\x12.\n\x06status\x18\x01 \x01(\x0e\x32\x1e.uauth_pb.GetQrcodeLoginStatus\x12\x32\n\x0f\x63ommonSignInRes\x18\x02 \x01(\x0b\x32\x19.uauth_pb.CommonSignInRes\x12\x14\n\x0cuserNickname\x18\x03 \x01(\t\x12\x13\n\x0buserIconUrl\x18\x04 \x01(\t\"\xba\x01\n\x17SetQrcodeLoginStatusReq\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x02 \x01(\t\x12\x12\n\nlogin_code\x18\x03 \x01(\t\x12\x33\n\x0bloginStatus\x18\x04 \x01(\x0e\x32\x1e.uauth_pb.GetQrcodeLoginStatus\x12\x14\n\x0cuserNickname\x18\x05 \x01(\t\x12\x13\n\x0buserIconUrl\x18\x06 \x01(\t\"\x19\n\x17SetQrcodeLoginStatusRes\"x\n\x1bGetAccountRegisterStatusReq\x12+\n\x04type\x18\x01 \x01(\x0e\x32\x1d.uauth_pb.AccountRegisterType\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04sign\x18\x03 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\x05\"3\n\x1bGetAccountRegisterStatusRes\x12\x14\n\x0cisRegistered\x18\x01 \x01(\x08\"2\n\x10GetUmengPhoneReq\x12\x0f\n\x07\x61pp_key\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"!\n\x10GetUmengPhoneRes\x12\r\n\x05phone\x18\x01 \x01(\t\"I\n\x14\x41\x63\x63ountCrossTypeInfo\x12\x31\n\ncross_type\x18\x01 \x01(\x0e\x32\x1d.uauth_pb.AccountAppCrossType\"\x19\n\x17\x41\x63\x63ountCrossTypeInfoReq\"L\n\x17\x41\x63\x63ountCrossTypeInfoRes\x12\x31\n\tinfo_list\x18\x01 \x03(\x0b\x32\x1e.uauth_pb.AccountCrossTypeInfo\"\x1a\n\x18\x41pplyAccountCrossTypeReq\"\x1a\n\x18\x41pplyAccountCrossTypeRes\"H\n\x18\x43heckInAppChargeLimitReq\x12,\n\x0b\x63harge_type\x18\x01 \x01(\x0e\x32\x17.uauth_pb.AppChargeType\".\n\x18\x43heckInAppChargeLimitRes\x12\x12\n\ncan_charge\x18\x01 \x01(\x08\"\x98\x02\n\x15GetAlipayMiniOrderReq\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\x12\x12\n\naccount_id\x18\x02 \x01(\x03\x12+\n\x08pay_type\x18\x03 \x01(\x0e\x32\x19.uauth_pb.UPayChannelType\x12\x0c\n\x04gold\x18\x04 \x01(\x03\x12\x0b\n\x03num\x18\x05 \x01(\x05\x12\x10\n\x08store_id\x18\x06 \x01(\x05\x12\x12\n\nreturn_url\x18\x07 \x01(\t\x12=\n\x07\x65xtends\x18\x08 \x03(\x0b\x32,.uauth_pb.GetAlipayMiniOrderReq.ExtendsEntry\x1a.\n\x0c\x45xtendsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\")\n\x15GetAlipayMiniOrderRes\x12\x10\n\x08trade_no\x18\x01 \x01(\t\"!\n\x0fGetGoodsListReq\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\">\n\x0fGetGoodsListRes\x12+\n\x04list\x18\x01 \x03(\x0b\x32\x1d.uauth_pb.AlipayMiniIndexItem\"\xb6\x01\n\x13\x41lipayMiniIndexItem\x12\x30\n\tdata_type\x18\x01 \x01(\x0e\x32\x1d.uauth_pb.AlipayMiniIndexType\x12\x31\n\x06\x62\x61nner\x18\x02 \x01(\x0b\x32\x1f.uauth_pb.AlipayMiniIndexBannerH\x00\x12\x32\n\x04list\x18\x03 \x01(\x0b\x32\".uauth_pb.AlipayMiniIndexGoodsListH\x00\x42\x06\n\x04\x64\x61ta\"+\n\x15\x41lipayMiniIndexBanner\x12\x12\n\nbanner_url\x18\x01 \x01(\t\"R\n\x18\x41lipayMiniIndexGoodsList\x12\x36\n\ngoods_list\x18\x01 \x03(\x0b\x32\".uauth_pb.AlipayMiniIndexGoodsItem\"\xad\x01\n\x18\x41lipayMiniIndexGoodsItem\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07img_url\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x04 \x01(\t\x12\r\n\x05price\x18\x05 \x01(\t\x12\x31\n\ngoods_type\x18\x06 \x01(\x0e\x32\x1d.uauth_pb.AlipayMiniGoodsType\x12\x0e\n\x04gold\x18\x07 \x01(\x03H\x00\x42\x06\n\x04\x64\x61ta*\x86\x07\n\x0e\x45rrorUAuthCode\x12\x13\n\x0f\x45rrorUAuth_Zero\x10\x00\x12\x1d\n\x17\x45rrorUAuthRegisterParam\x10\xd9\xb0\x02\x12\x1c\n\x16\x45rrorUAuthAccountExist\x10\xda\xb0\x02\x12\x1e\n\x18\x45rrorUAuthSessionTimeOut\x10\xdb\xb0\x02\x12\x1f\n\x19\x45rrorUAuthSessionNotFound\x10\xdc\xb0\x02\x12\x1c\n\x16\x45rrorUAuthUserNotFound\x10\xdd\xb0\x02\x12\x1f\n\x19\x45rrorUAuthAccountNotExist\x10\xde\xb0\x02\x12!\n\x1b\x45rrorUAuthPassWordNoCorrect\x10\xdf\xb0\x02\x12\x1d\n\x17\x45rrorUAuthCodeIncorrect\x10\xe0\xb0\x02\x12\x1d\n\x17\x45rrorUAuthPhoneNotExist\x10\xe1\xb0\x02\x12\x1b\n\x15\x45rrorUAuthUserNoRight\x10\xe2\xb0\x02\x12\x1a\n\x14\x45rrorUAuthInvalidWay\x10\xe3\xb0\x02\x12\x19\n\x13\x45rrorUAuthNeedLogin\x10\xe4\xb0\x02\x12\x18\n\x12\x45rrorUAuthGetToken\x10\xe5\xb0\x02\x12\x1b\n\x15\x45rrorUAuthAccessToken\x10\xe6\xb0\x02\x12\x1d\n\x17\x45rrorUAuthWrongPhoneNum\x10\xe7\xb0\x02\x12\x1d\n\x17\x45rrorUAuthServerOffLine\x10\xe8\xb0\x02\x12!\n\x1b\x45rrorUAuthPhoneAlreadyExist\x10\xe9\xb0\x02\x12\x18\n\x12\x45rrorIAPHasNoOrder\x10\xaa\xcb\x0e\x12\x18\n\x12\x45rrorCheckIAPOrder\x10\xab\xcb\x0e\x12\x1b\n\x15\x45rrorCheckIAPBundleID\x10\xac\xcb\x0e\x12\x16\n\x10\x45rrorTooFrequent\x10\xb6\xcb\x0e\x12\x0e\n\x08\x45rror3rd\x10\xb7\xcb\x0e\x12\x1a\n\x14\x45rrorPasswordInvalid\x10\xb8\xcb\x0e\x12\x1b\n\x15\x45rrorWrongOldPassword\x10\xb9\xcb\x0e\x12\x15\n\x0f\x45rrorLoginBlack\x10\xba\xcb\x0e\x12\x15\n\x0f\x45rrorHasAccount\x10\xbb\xcb\x0e\x12\x1c\n\x16\x45rrorUAuthPswNoCorrect\x10\xbc\xcb\x0e\x12\x1e\n\x18\x45rrorUAuthPhoneNoCorrect\x10\xbd\xcb\x0e\x12\x19\n\x13\x45rrorUserLimitLogin\x10\xd2\xcb\x0e\x12\x1c\n\x16\x45rrorRefusePhoneLicens\x10\xd4\xcb\x0e*I\n\rIAPStatusType\x12\x0c\n\x08IAP_NONE\x10\x00\x12\x13\n\x0fIAP_STATUS_FAIL\x10\x01\x12\x15\n\x11IAP_STATUS_CANCEL\x10\x02*=\n\x0c\x43hargeStatus\x12\x0f\n\x0b\x43S_CHARGING\x10\x00\x12\r\n\tCS_FINISH\x10\x01\x12\r\n\tCS_REFUND\x10\x02*9\n\x0eReportDataType\x12\x0c\n\x08RDT_Null\x10\x00\x12\x19\n\x15RDT_CMB_VIP_Expedited\x10\x01*R\n\nVerifyType\x12\x0b\n\x07VT_NULL\x10\x00\x12\x12\n\x0eVT_RemoteLogin\x10\x01\x12\x0e\n\nVT_Protect\x10\x02\x12\x13\n\x0fVT_AnomalyLogin\x10\x03*k\n\nSMSCodeTpl\x12\x13\n\x0fSMSCodeTpl_Zero\x10\x00\x12\x14\n\x10SMSCodeTpl_Login\x10\x01\x12\x17\n\x13SMSCodeTpl_ResetPwd\x10\x02\x12\x19\n\x15SMSCodeTpl_VerifyCode\x10\x03*)\n\x0b\x43\x65rtifyType\x12\x0b\n\x07\x43T_None\x10\x00\x12\r\n\tCT_IdCard\x10\x01*\x82\x01\n\x18WechatMiniCodeScanStatus\x12\x10\n\x0cWMCSS_NoScan\x10\x00\x12\x11\n\rWMCSS_Timeout\x10\x01\x12\x10\n\x0cWMCSS_ScanIn\x10\x02\x12\x11\n\rWMCSS_ScanEnd\x10\x03\x12\x1c\n\x18WMCSS_RefusePhoneLicense\x10\x04*C\n\x14ThirdAccountBindType\x12\r\n\tTABT_NONE\x10\x00\x12\x0f\n\x0bTABT_WEIXIN\x10\x01\x12\x0b\n\x07TABT_QQ\x10\x02*=\n\x19UnbindThirdAccountOptType\x12\x0e\n\nUTAOT_Send\x10\x00\x12\x10\n\x0cUTAOT_Verify\x10\x01*S\n\x14GetQrcodeLoginStatus\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\x0b\n\x07SUCCESS\x10\x02\x12\x0b\n\x07\x45XPIRED\x10\x03\x12\n\n\x06\x43\x41NCEL\x10\x04*>\n\x13\x41\x63\x63ountRegisterType\x12\x0b\n\x07RT_NONE\x10\x00\x12\x0c\n\x08RT_PHONE\x10\x01\x12\x0c\n\x08RT_EMAIL\x10\x02*3\n\x13\x41\x63\x63ountAppCrossType\x12\r\n\tAACT_None\x10\x00\x12\r\n\tAACT_Neon\x10\x01*<\n\rAppChargeType\x12\x0c\n\x08\x41\x43T_None\x10\x00\x12\r\n\tACT_Apple\x10\x01\x12\x0e\n\nACT_Google\x10\x02*E\n\x13\x41lipayMiniIndexType\x12\r\n\tAMIT_NONE\x10\x00\x12\x0f\n\x0b\x41MIT_BANNER\x10\x01\x12\x0e\n\nAMIT_GOODS\x10\x02*3\n\x13\x41lipayMiniGoodsType\x12\r\n\tAMGT_NONE\x10\x00\x12\r\n\tAMGT_GOLD\x10\x01\x32\x9a/\n\x0bUauthExtObj\x12;\n\tVerifyIAP\x12\x16.uauth_pb.VerifyIAPReq\x1a\x16.uauth_pb.VerifyIAPRes\x12\x41\n\x0bGetGoodList\x12\x18.uauth_pb.GetGoodListReq\x1a\x18.uauth_pb.GetGoodListRes\x12\x38\n\x08OrderIAP\x12\x15.uauth_pb.OrderIAPReq\x1a\x15.uauth_pb.OrderIAPRes\x12G\n\rCloseOrderIAP\x12\x1a.uauth_pb.CloseOrderIAPReq\x1a\x1a.uauth_pb.CloseOrderIAPRes\x12_\n\x17GetVIPChargeAccountInfo\x12!.uauth_pb.VIPChargeAccountInfoReq\x1a!.uauth_pb.VIPChargeAccountInfoRes\x12\x44\n\x0cVIPChargeLog\x12\x19.uauth_pb.VIPChargeLogReq\x1a\x19.uauth_pb.VIPChargeLogRes\x12>\n\nReportData\x12\x17.uauth_pb.ReportDataReq\x1a\x17.uauth_pb.ReportDataRes\x12;\n\tGetCharge\x12\x16.uauth_pb.GetChargeReq\x1a\x16.uauth_pb.GetChargeRes\x12M\n\x12GetSignInWithApple\x12\x1c.uauth_pb.SignInWithAppleReq\x1a\x19.uauth_pb.CommonSignInRes\x12>\n\nGetSmsCode\x12\x17.uauth_pb.GetSmsCodeReq\x1a\x17.uauth_pb.GetSmsCodeRes\x12\x44\n\x10GetSmsCodeBySign\x12\x17.uauth_pb.GetSmsCodeReq\x1a\x17.uauth_pb.GetSmsCodeRes\x12\x41\n\x0bGetSmsToken\x12\x18.uauth_pb.GetSmsTokenReq\x1a\x18.uauth_pb.GetSmsTokenRes\x12G\n\x11GetSmsTokenBySign\x12\x18.uauth_pb.GetSmsTokenReq\x1a\x18.uauth_pb.GetSmsTokenRes\x12?\n\x0bGetDevLogin\x12\x15.uauth_pb.DevLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12K\n\x11GetIdOrPhoneLogin\x12\x1b.uauth_pb.IdOrPhoneLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12\x43\n\rGetThirdLogin\x12\x17.uauth_pb.ThirdLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12Q\n\x14GetLoginWithPhoneSMS\x12\x1e.uauth_pb.LoginWithPhoneSMSReq\x1a\x19.uauth_pb.CommonSignInRes\x12W\n\x1aGetLoginWithPhoneSMSBySign\x12\x1e.uauth_pb.LoginWithPhoneSMSReq\x1a\x19.uauth_pb.CommonSignInRes\x12Y\n\x18GetChinaMobileQuickLogin\x12\".uauth_pb.ChinaMobileQuickLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12O\n\x13GetChinaTelecomAuth\x12\x1d.uauth_pb.ChinaTelecomAuthReq\x1a\x19.uauth_pb.CommonSignInRes\x12M\n\x12GetUmengQuickLogin\x12\x1c.uauth_pb.UmengQuickLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12J\n\x10GetResetPassword\x12\x1a.uauth_pb.ResetPasswordReq\x1a\x1a.uauth_pb.ResetPasswordRes\x12P\n\x16GetResetPasswordBySign\x12\x1a.uauth_pb.ResetPasswordReq\x1a\x1a.uauth_pb.ResetPasswordRes\x12\x44\n\x0cUpdatePasswd\x12\x19.uauth_pb.UpdatePasswdReq\x1a\x19.uauth_pb.UpdatePasswdRes\x12\x35\n\tGetInvite\x12\x13.uauth_pb.InviteReq\x1a\x13.uauth_pb.InviteRes\x12\x41\n\x0bGetSyncTime\x12\x18.uauth_pb.GetSyncTimeReq\x1a\x18.uauth_pb.GetSyncTimeRes\x12S\n\x11ReportBuyNobility\x12\x1e.uauth_pb.ReportBuyNobilityReq\x1a\x1e.uauth_pb.ReportBuyNobilityRes\x12J\n\x0eGetWeChatAppId\x12\x1b.uauth_pb.GetWeChatAppIdReq\x1a\x1b.uauth_pb.GetWeChatAppIdRes\x12P\n\x10GetWeChatIdLogin\x12\x1d.uauth_pb.GetWeChatIdLoginReq\x1a\x1d.uauth_pb.GetWeChatIdLoginRes\x12\x61\n\x15GoogleIABProductItems\x12\".uauth_pb.GoogleIABProductItemsReq\x1a\".uauth_pb.GoogleIABProductItemsRes\"\x00\x12O\n\x0fGoogleIABNotify\x12\x1c.uauth_pb.GoogleIABNotifyReq\x1a\x1c.uauth_pb.GoogleIABNotifyRes\"\x00\x12R\n\x13GetMiniProgramLogin\x12 .uauth_pb.GetMiniProgramLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12P\n\x10MiniProgramPhone\x12\x1d.uauth_pb.MiniProgramPhoneReq\x1a\x1d.uauth_pb.MiniProgramPhoneRes\x12\x44\n\x0c\x41pplyCertify\x12\x19.uauth_pb.ApplyCertifyReq\x1a\x19.uauth_pb.ApplyCertifyRes\x12L\n\x10\x41pplyCertifySign\x12\x1d.uauth_pb.ApplyCertifySignReq\x1a\x19.uauth_pb.ApplyCertifyRes\x12G\n\rCertifyResult\x12\x1a.uauth_pb.CertifyResultReq\x1a\x1a.uauth_pb.CertifyResultRes\x12Y\n\x13\x41\x63\x63ountPhoneSmsCode\x12 .uauth_pb.AccountPhoneSmsCodeReq\x1a .uauth_pb.AccountPhoneSmsCodeRes\x12X\n\x16\x41\x63\x63ountSubsidiaryLogin\x12#.uauth_pb.AccountSubsidiaryLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12\x46\n\rGetGuestLogin\x12\x1a.uauth_pb.GetGuestLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12P\n\x10\x42indPhoneSmsCode\x12\x1d.uauth_pb.BindPhoneSmsCodeReq\x1a\x1d.uauth_pb.BindPhoneSmsCodeRes\x12Y\n\x13\x41\x63\x63ountBindPhoneSMS\x12 .uauth_pb.AccountBindPhoneSMSReq\x1a .uauth_pb.AccountBindPhoneSMSRes\x12P\n\x10\x41\x63\x63ountBindThird\x12\x1d.uauth_pb.AccountBindThirdReq\x1a\x1d.uauth_pb.AccountBindThirdRes\x12M\n\x0f\x41\x63\x63ountBindList\x12\x1c.uauth_pb.AccountBindListReq\x1a\x1c.uauth_pb.AccountBindListRes\x12P\n\x10\x42indEmailSesCode\x12\x1d.uauth_pb.BindEmailSesCodeReq\x1a\x1d.uauth_pb.BindEmailSesCodeRes\x12Y\n\x13\x41\x63\x63ountBindEmailSES\x12 .uauth_pb.AccountBindEmailSESReq\x1a .uauth_pb.AccountBindEmailSESRes\x12P\n\x12GetAccountRegister\x12\x1f.uauth_pb.GetAccountRegisterReq\x1a\x19.uauth_pb.CommonSignInRes\x12Z\n\x17GetAccountPasswordLogin\x12$.uauth_pb.GetAccountPasswordLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12>\n\nGetSesCode\x12\x17.uauth_pb.GetSesCodeReq\x1a\x17.uauth_pb.GetSesCodeRes\x12\x41\n\x0bGetSesToken\x12\x18.uauth_pb.GetSesTokenReq\x1a\x18.uauth_pb.GetSesTokenRes\x12Y\n\x15GetResetPasswordBySes\x12\x1f.uauth_pb.ResetPasswordBySesReq\x1a\x1f.uauth_pb.ResetPasswordBySesRes\x12\\\n\x16GetRemoteLoginSendCode\x12 .uauth_pb.RemoteLoginSendCodeReq\x1a .uauth_pb.RemoteLoginSendCodeRes\x12\x65\n\x19GetRemoteLoginConfirmCode\x12#.uauth_pb.RemoteLoginConfirmCodeReq\x1a#.uauth_pb.RemoteLoginConfirmCodeRes\x12q\n\x1bVerifyCancelSignInWithApple\x12(.uauth_pb.VerifyCancelSignInWithAppleReq\x1a(.uauth_pb.VerifyCancelSignInWithAppleRes\x12\x44\n\x0cPhoneSmsCode\x12\x19.uauth_pb.PhoneSmsCodeReq\x1a\x19.uauth_pb.PhoneSmsCodeRes\x12S\n\x11\x43heckPhoneSmsCode\x12\x1e.uauth_pb.CheckPhoneSmsCodeReq\x1a\x1e.uauth_pb.CheckPhoneSmsCodeRes\x12\x62\n\x18GetWechatCodeLoginTicket\x12\".uauth_pb.WechatCodeLoginTicketReq\x1a\".uauth_pb.WechatCodeLoginTicketRes\x12S\n\x11GetWechatMiniCode\x12\x1e.uauth_pb.GetWechatMiniCodeReq\x1a\x1e.uauth_pb.GetWechatMiniCodeRes\x12_\n\x15GetWechatMiniCodeScan\x12\".uauth_pb.GetWechatMiniCodeScanReq\x1a\".uauth_pb.GetWechatMiniCodeScanRes\x12Y\n\x15GetRefusePhoneLicense\x12\x1f.uauth_pb.RefusePhoneLicenseReq\x1a\x1f.uauth_pb.RefusePhoneLicenseRes\x12Y\n\x13WechatMiniBindPhone\x12 .uauth_pb.WechatMiniBindPhoneReq\x1a .uauth_pb.WechatMiniBindPhoneRes\x12\\\n\x14ThirdAccountBindInfo\x12!.uauth_pb.ThirdAccountBindInfoReq\x1a!.uauth_pb.ThirdAccountBindInfoRes\x12P\n\x10\x42indThirdAccount\x12\x1d.uauth_pb.BindThirdAccountReq\x1a\x1d.uauth_pb.BindThirdAccountRes\x12V\n\x12UnbindThirdAccount\x12\x1f.uauth_pb.UnbindThirdAccountReq\x1a\x1f.uauth_pb.UnbindThirdAccountRes\x12V\n\x12GetQrcodeLoginCode\x12\x1f.uauth_pb.GetQrcodeLoginCodeReq\x1a\x1f.uauth_pb.GetQrcodeLoginCodeRes\x12\\\n\x14GetQrcodeLoginStatus\x12!.uauth_pb.GetQrcodeLoginStatusReq\x1a!.uauth_pb.GetQrcodeLoginStatusRes\x12\\\n\x14SetQrcodeLoginStatus\x12!.uauth_pb.SetQrcodeLoginStatusReq\x1a!.uauth_pb.SetQrcodeLoginStatusRes\x12M\n\x0fQrcodeScanLogin\x12\x1c.uauth_pb.QrcodeScanLoginReq\x1a\x1c.uauth_pb.QrcodeScanLoginRes\x12h\n\x18GetAccountRegisterStatus\x12%.uauth_pb.GetAccountRegisterStatusReq\x1a%.uauth_pb.GetAccountRegisterStatusRes\x12G\n\rGetUmengPhone\x12\x1a.uauth_pb.GetUmengPhoneReq\x1a\x1a.uauth_pb.GetUmengPhoneRes\x12\\\n\x14\x41\x63\x63ountCrossTypeInfo\x12!.uauth_pb.AccountCrossTypeInfoReq\x1a!.uauth_pb.AccountCrossTypeInfoRes\x12_\n\x15\x41pplyAccountCrossType\x12\".uauth_pb.ApplyAccountCrossTypeReq\x1a\".uauth_pb.ApplyAccountCrossTypeRes\x12_\n\x15\x43heckInAppChargeLimit\x12\".uauth_pb.CheckInAppChargeLimitReq\x1a\".uauth_pb.CheckInAppChargeLimitRes\x12V\n\x12GetAlipayMiniOrder\x12\x1f.uauth_pb.GetAlipayMiniOrderReq\x1a\x1f.uauth_pb.GetAlipayMiniOrderRes\x12\x44\n\x0cGetGoodsList\x12\x19.uauth_pb.GetGoodsListReq\x1a\x19.uauth_pb.GetGoodsListResB\x08\xa2\x02\x05PROTOb\x06proto3')
-
-_ERRORUAUTHCODE = DESCRIPTOR.enum_types_by_name['ErrorUAuthCode']
-ErrorUAuthCode = enum_type_wrapper.EnumTypeWrapper(_ERRORUAUTHCODE)
-_IAPSTATUSTYPE = DESCRIPTOR.enum_types_by_name['IAPStatusType']
-IAPStatusType = enum_type_wrapper.EnumTypeWrapper(_IAPSTATUSTYPE)
-_CHARGESTATUS = DESCRIPTOR.enum_types_by_name['ChargeStatus']
-ChargeStatus = enum_type_wrapper.EnumTypeWrapper(_CHARGESTATUS)
-_REPORTDATATYPE = DESCRIPTOR.enum_types_by_name['ReportDataType']
-ReportDataType = enum_type_wrapper.EnumTypeWrapper(_REPORTDATATYPE)
-_VERIFYTYPE = DESCRIPTOR.enum_types_by_name['VerifyType']
-VerifyType = enum_type_wrapper.EnumTypeWrapper(_VERIFYTYPE)
-_SMSCODETPL = DESCRIPTOR.enum_types_by_name['SMSCodeTpl']
-SMSCodeTpl = enum_type_wrapper.EnumTypeWrapper(_SMSCODETPL)
-_CERTIFYTYPE = DESCRIPTOR.enum_types_by_name['CertifyType']
-CertifyType = enum_type_wrapper.EnumTypeWrapper(_CERTIFYTYPE)
-_WECHATMINICODESCANSTATUS = DESCRIPTOR.enum_types_by_name['WechatMiniCodeScanStatus']
-WechatMiniCodeScanStatus = enum_type_wrapper.EnumTypeWrapper(_WECHATMINICODESCANSTATUS)
-_THIRDACCOUNTBINDTYPE = DESCRIPTOR.enum_types_by_name['ThirdAccountBindType']
-ThirdAccountBindType = enum_type_wrapper.EnumTypeWrapper(_THIRDACCOUNTBINDTYPE)
-_UNBINDTHIRDACCOUNTOPTTYPE = DESCRIPTOR.enum_types_by_name['UnbindThirdAccountOptType']
-UnbindThirdAccountOptType = enum_type_wrapper.EnumTypeWrapper(_UNBINDTHIRDACCOUNTOPTTYPE)
-_GETQRCODELOGINSTATUS = DESCRIPTOR.enum_types_by_name['GetQrcodeLoginStatus']
-GetQrcodeLoginStatus = enum_type_wrapper.EnumTypeWrapper(_GETQRCODELOGINSTATUS)
-_ACCOUNTREGISTERTYPE = DESCRIPTOR.enum_types_by_name['AccountRegisterType']
-AccountRegisterType = enum_type_wrapper.EnumTypeWrapper(_ACCOUNTREGISTERTYPE)
-_ACCOUNTAPPCROSSTYPE = DESCRIPTOR.enum_types_by_name['AccountAppCrossType']
-AccountAppCrossType = enum_type_wrapper.EnumTypeWrapper(_ACCOUNTAPPCROSSTYPE)
-_APPCHARGETYPE = DESCRIPTOR.enum_types_by_name['AppChargeType']
-AppChargeType = enum_type_wrapper.EnumTypeWrapper(_APPCHARGETYPE)
-_ALIPAYMINIINDEXTYPE = DESCRIPTOR.enum_types_by_name['AlipayMiniIndexType']
-AlipayMiniIndexType = enum_type_wrapper.EnumTypeWrapper(_ALIPAYMINIINDEXTYPE)
-_ALIPAYMINIGOODSTYPE = DESCRIPTOR.enum_types_by_name['AlipayMiniGoodsType']
-AlipayMiniGoodsType = enum_type_wrapper.EnumTypeWrapper(_ALIPAYMINIGOODSTYPE)
-ErrorUAuth_Zero = 0
-ErrorUAuthRegisterParam = 39001
-ErrorUAuthAccountExist = 39002
-ErrorUAuthSessionTimeOut = 39003
-ErrorUAuthSessionNotFound = 39004
-ErrorUAuthUserNotFound = 39005
-ErrorUAuthAccountNotExist = 39006
-ErrorUAuthPassWordNoCorrect = 39007
-ErrorUAuthCodeIncorrect = 39008
-ErrorUAuthPhoneNotExist = 39009
-ErrorUAuthUserNoRight = 39010
-ErrorUAuthInvalidWay = 39011
-ErrorUAuthNeedLogin = 39012
-ErrorUAuthGetToken = 39013
-ErrorUAuthAccessToken = 39014
-ErrorUAuthWrongPhoneNum = 39015
-ErrorUAuthServerOffLine = 39016
-ErrorUAuthPhoneAlreadyExist = 39017
-ErrorIAPHasNoOrder = 239018
-ErrorCheckIAPOrder = 239019
-ErrorCheckIAPBundleID = 239020
-ErrorTooFrequent = 239030
-Error3rd = 239031
-ErrorPasswordInvalid = 239032
-ErrorWrongOldPassword = 239033
-ErrorLoginBlack = 239034
-ErrorHasAccount = 239035
-ErrorUAuthPswNoCorrect = 239036
-ErrorUAuthPhoneNoCorrect = 239037
-ErrorUserLimitLogin = 239058
-ErrorRefusePhoneLicens = 239060
-IAP_NONE = 0
-IAP_STATUS_FAIL = 1
-IAP_STATUS_CANCEL = 2
-CS_CHARGING = 0
-CS_FINISH = 1
-CS_REFUND = 2
-RDT_Null = 0
-RDT_CMB_VIP_Expedited = 1
-VT_NULL = 0
-VT_RemoteLogin = 1
-VT_Protect = 2
-VT_AnomalyLogin = 3
-SMSCodeTpl_Zero = 0
-SMSCodeTpl_Login = 1
-SMSCodeTpl_ResetPwd = 2
-SMSCodeTpl_VerifyCode = 3
-CT_None = 0
-CT_IdCard = 1
-WMCSS_NoScan = 0
-WMCSS_Timeout = 1
-WMCSS_ScanIn = 2
-WMCSS_ScanEnd = 3
-WMCSS_RefusePhoneLicense = 4
-TABT_NONE = 0
-TABT_WEIXIN = 1
-TABT_QQ = 2
-UTAOT_Send = 0
-UTAOT_Verify = 1
-NONE = 0
-PENDING = 1
-SUCCESS = 2
-EXPIRED = 3
-CANCEL = 4
-RT_NONE = 0
-RT_PHONE = 1
-RT_EMAIL = 2
-AACT_None = 0
-AACT_Neon = 1
-ACT_None = 0
-ACT_Apple = 1
-ACT_Google = 2
-AMIT_NONE = 0
-AMIT_BANNER = 1
-AMIT_GOODS = 2
-AMGT_NONE = 0
-AMGT_GOLD = 1
-
-
-_VERIFYIAPREQ = DESCRIPTOR.message_types_by_name['VerifyIAPReq']
-_VERIFYIAPRES = DESCRIPTOR.message_types_by_name['VerifyIAPRes']
-_GOLDCARD = DESCRIPTOR.message_types_by_name['GoldCard']
-_GETGOODLISTREQ = DESCRIPTOR.message_types_by_name['GetGoodListReq']
-_GETGOODLISTRES = DESCRIPTOR.message_types_by_name['GetGoodListRes']
-_ORDERIAPREQ = DESCRIPTOR.message_types_by_name['OrderIAPReq']
-_ORDERIAPRES = DESCRIPTOR.message_types_by_name['OrderIAPRes']
-_CLOSEORDERIAPREQ = DESCRIPTOR.message_types_by_name['CloseOrderIAPReq']
-_CLOSEORDERIAPRES = DESCRIPTOR.message_types_by_name['CloseOrderIAPRes']
-_VIPCHARGEACCOUNTINFOREQ = DESCRIPTOR.message_types_by_name['VIPChargeAccountInfoReq']
-_VIPCHARGEACCOUNTINFORES = DESCRIPTOR.message_types_by_name['VIPChargeAccountInfoRes']
-_VIPCHARGELOGREQ = DESCRIPTOR.message_types_by_name['VIPChargeLogReq']
-_VIPCHARGELOGRES = DESCRIPTOR.message_types_by_name['VIPChargeLogRes']
-_VIPCHARGELOGS = DESCRIPTOR.message_types_by_name['VIPChargeLogs']
-_VIPCHARGEITEM = DESCRIPTOR.message_types_by_name['VIPChargeItem']
-_REPORTDATAREQ = DESCRIPTOR.message_types_by_name['ReportDataReq']
-_REPORTDATARES = DESCRIPTOR.message_types_by_name['ReportDataRes']
-_GETCHARGEREQ = DESCRIPTOR.message_types_by_name['GetChargeReq']
-_GETCHARGEREQ_EXTENDSENTRY = _GETCHARGEREQ.nested_types_by_name['ExtendsEntry']
-_GETCHARGEREQ_EXTRADATAENTRY = _GETCHARGEREQ.nested_types_by_name['ExtraDataEntry']
-_GETCHARGERES = DESCRIPTOR.message_types_by_name['GetChargeRes']
-_GETSMSCODEREQ = DESCRIPTOR.message_types_by_name['GetSmsCodeReq']
-_GETSMSCODERES = DESCRIPTOR.message_types_by_name['GetSmsCodeRes']
-_GETSMSTOKENREQ = DESCRIPTOR.message_types_by_name['GetSmsTokenReq']
-_GETSMSTOKENRES = DESCRIPTOR.message_types_by_name['GetSmsTokenRes']
-_PHONESMSCODEREQ = DESCRIPTOR.message_types_by_name['PhoneSmsCodeReq']
-_PHONESMSCODERES = DESCRIPTOR.message_types_by_name['PhoneSmsCodeRes']
-_CHECKPHONESMSCODEREQ = DESCRIPTOR.message_types_by_name['CheckPhoneSmsCodeReq']
-_CHECKPHONESMSCODERES = DESCRIPTOR.message_types_by_name['CheckPhoneSmsCodeRes']
-_COMMONSIGNINRES = DESCRIPTOR.message_types_by_name['CommonSignInRes']
-_COMMONSIGNINRES_EXTENDSENTRY = _COMMONSIGNINRES.nested_types_by_name['ExtendsEntry']
-_SIGNINWITHAPPLEREQ = DESCRIPTOR.message_types_by_name['SignInWithAppleReq']
-_IDORPHONELOGINREQ = DESCRIPTOR.message_types_by_name['IdOrPhoneLoginReq']
-_LOGINWITHPHONESMSREQ = DESCRIPTOR.message_types_by_name['LoginWithPhoneSMSReq']
-_THIRDLOGINREQ = DESCRIPTOR.message_types_by_name['ThirdLoginReq']
-_CHINAMOBILEQUICKLOGINREQ = DESCRIPTOR.message_types_by_name['ChinaMobileQuickLoginReq']
-_CHINATELECOMAUTHREQ = DESCRIPTOR.message_types_by_name['ChinaTelecomAuthReq']
-_UMENGQUICKLOGINREQ = DESCRIPTOR.message_types_by_name['UmengQuickLoginReq']
-_DEVLOGINREQ = DESCRIPTOR.message_types_by_name['DevLoginReq']
-_RESETPASSWORDREQ = DESCRIPTOR.message_types_by_name['ResetPasswordReq']
-_RESETPASSWORDRES = DESCRIPTOR.message_types_by_name['ResetPasswordRes']
-_LOGINSECRETREQ = DESCRIPTOR.message_types_by_name['LoginSecretReq']
-_LOGINSECRETRES = DESCRIPTOR.message_types_by_name['LoginSecretRes']
-_UPDATEPASSWDREQ = DESCRIPTOR.message_types_by_name['UpdatePasswdReq']
-_UPDATEPASSWDRES = DESCRIPTOR.message_types_by_name['UpdatePasswdRes']
-_INVITEREQ = DESCRIPTOR.message_types_by_name['InviteReq']
-_INVITERES = DESCRIPTOR.message_types_by_name['InviteRes']
-_GETSYNCTIMEREQ = DESCRIPTOR.message_types_by_name['GetSyncTimeReq']
-_GETSYNCTIMERES = DESCRIPTOR.message_types_by_name['GetSyncTimeRes']
-_REPORTBUYNOBILITYREQ = DESCRIPTOR.message_types_by_name['ReportBuyNobilityReq']
-_REPORTBUYNOBILITYRES = DESCRIPTOR.message_types_by_name['ReportBuyNobilityRes']
-_GOOGLEIABNOTIFYREQ = DESCRIPTOR.message_types_by_name['GoogleIABNotifyReq']
-_GOOGLEIABNOTIFYREQ_BUYINTENT = _GOOGLEIABNOTIFYREQ.nested_types_by_name['BuyIntent']
-_GOOGLEIABNOTIFYRES = DESCRIPTOR.message_types_by_name['GoogleIABNotifyRes']
-_GOOGLEIABPRODUCTITEM = DESCRIPTOR.message_types_by_name['GoogleIABProductItem']
-_GOOGLEIABPRODUCTITEMSREQ = DESCRIPTOR.message_types_by_name['GoogleIABProductItemsReq']
-_GOOGLEIABPRODUCTITEMSRES = DESCRIPTOR.message_types_by_name['GoogleIABProductItemsRes']
-_GETWECHATAPPIDREQ = DESCRIPTOR.message_types_by_name['GetWeChatAppIdReq']
-_GETWECHATAPPIDRES = DESCRIPTOR.message_types_by_name['GetWeChatAppIdRes']
-_GETWECHATIDLOGINREQ = DESCRIPTOR.message_types_by_name['GetWeChatIdLoginReq']
-_GETWECHATIDLOGINRES = DESCRIPTOR.message_types_by_name['GetWeChatIdLoginRes']
-_USERINFO = DESCRIPTOR.message_types_by_name['UserInfo']
-_GETMINIPROGRAMLOGINREQ = DESCRIPTOR.message_types_by_name['GetMiniProgramLoginReq']
-_MINIPROGRAMPHONEREQ = DESCRIPTOR.message_types_by_name['MiniProgramPhoneReq']
-_MINIPROGRAMPHONERES = DESCRIPTOR.message_types_by_name['MiniProgramPhoneRes']
-_APPLYCERTIFYREQ = DESCRIPTOR.message_types_by_name['ApplyCertifyReq']
-_APPLYCERTIFYRES = DESCRIPTOR.message_types_by_name['ApplyCertifyRes']
-_APPLYCERTIFYSIGNREQ = DESCRIPTOR.message_types_by_name['ApplyCertifySignReq']
-_CERTIFYRESULTREQ = DESCRIPTOR.message_types_by_name['CertifyResultReq']
-_CERTIFYRESULTRES = DESCRIPTOR.message_types_by_name['CertifyResultRes']
-_ACCOUNTPHONESMSCODEREQ = DESCRIPTOR.message_types_by_name['AccountPhoneSmsCodeReq']
-_ACCOUNTPHONESMSCODERES = DESCRIPTOR.message_types_by_name['AccountPhoneSmsCodeRes']
-_ACCOUNTSUBSIDIARYLOGINREQ = DESCRIPTOR.message_types_by_name['AccountSubsidiaryLoginReq']
-_GETGUESTLOGINREQ = DESCRIPTOR.message_types_by_name['GetGuestLoginReq']
-_ACCOUNTBINDPHONESMSREQ = DESCRIPTOR.message_types_by_name['AccountBindPhoneSMSReq']
-_ACCOUNTBINDPHONESMSRES = DESCRIPTOR.message_types_by_name['AccountBindPhoneSMSRes']
-_ACCOUNTBINDTHIRDREQ = DESCRIPTOR.message_types_by_name['AccountBindThirdReq']
-_ACCOUNTBINDTHIRDRES = DESCRIPTOR.message_types_by_name['AccountBindThirdRes']
-_ACCOUNTBINDLISTREQ = DESCRIPTOR.message_types_by_name['AccountBindListReq']
-_ACCOUNTBINDLISTRES = DESCRIPTOR.message_types_by_name['AccountBindListRes']
-_BINDPHONESMSCODEREQ = DESCRIPTOR.message_types_by_name['BindPhoneSmsCodeReq']
-_BINDPHONESMSCODERES = DESCRIPTOR.message_types_by_name['BindPhoneSmsCodeRes']
-_BINDEMAILSESCODEREQ = DESCRIPTOR.message_types_by_name['BindEmailSesCodeReq']
-_BINDEMAILSESCODERES = DESCRIPTOR.message_types_by_name['BindEmailSesCodeRes']
-_ACCOUNTBINDEMAILSESREQ = DESCRIPTOR.message_types_by_name['AccountBindEmailSESReq']
-_ACCOUNTBINDEMAILSESRES = DESCRIPTOR.message_types_by_name['AccountBindEmailSESRes']
-_GETACCOUNTREGISTERREQ = DESCRIPTOR.message_types_by_name['GetAccountRegisterReq']
-_GETACCOUNTPASSWORDLOGINREQ = DESCRIPTOR.message_types_by_name['GetAccountPasswordLoginReq']
-_GETSESCODEREQ = DESCRIPTOR.message_types_by_name['GetSesCodeReq']
-_GETSESCODERES = DESCRIPTOR.message_types_by_name['GetSesCodeRes']
-_GETSESTOKENREQ = DESCRIPTOR.message_types_by_name['GetSesTokenReq']
-_GETSESTOKENRES = DESCRIPTOR.message_types_by_name['GetSesTokenRes']
-_RESETPASSWORDBYSESREQ = DESCRIPTOR.message_types_by_name['ResetPasswordBySesReq']
-_RESETPASSWORDBYSESRES = DESCRIPTOR.message_types_by_name['ResetPasswordBySesRes']
-_REMOTELOGINSENDCODEREQ = DESCRIPTOR.message_types_by_name['RemoteLoginSendCodeReq']
-_REMOTELOGINSENDCODERES = DESCRIPTOR.message_types_by_name['RemoteLoginSendCodeRes']
-_REMOTELOGINCONFIRMCODEREQ = DESCRIPTOR.message_types_by_name['RemoteLoginConfirmCodeReq']
-_REMOTELOGINCONFIRMCODERES = DESCRIPTOR.message_types_by_name['RemoteLoginConfirmCodeRes']
-_VERIFYCANCELSIGNINWITHAPPLEREQ = DESCRIPTOR.message_types_by_name['VerifyCancelSignInWithAppleReq']
-_VERIFYCANCELSIGNINWITHAPPLERES = DESCRIPTOR.message_types_by_name['VerifyCancelSignInWithAppleRes']
-_WECHATCODELOGINTICKETREQ = DESCRIPTOR.message_types_by_name['WechatCodeLoginTicketReq']
-_WECHATCODELOGINTICKETRES = DESCRIPTOR.message_types_by_name['WechatCodeLoginTicketRes']
-_GETWECHATMINICODEREQ = DESCRIPTOR.message_types_by_name['GetWechatMiniCodeReq']
-_GETWECHATMINICODERES = DESCRIPTOR.message_types_by_name['GetWechatMiniCodeRes']
-_GETWECHATMINICODESCANREQ = DESCRIPTOR.message_types_by_name['GetWechatMiniCodeScanReq']
-_GETWECHATMINICODESCANRES = DESCRIPTOR.message_types_by_name['GetWechatMiniCodeScanRes']
-_REFUSEPHONELICENSEREQ = DESCRIPTOR.message_types_by_name['RefusePhoneLicenseReq']
-_REFUSEPHONELICENSERES = DESCRIPTOR.message_types_by_name['RefusePhoneLicenseRes']
-_WECHATMINIBINDPHONEREQ = DESCRIPTOR.message_types_by_name['WechatMiniBindPhoneReq']
-_WECHATMINIBINDPHONERES = DESCRIPTOR.message_types_by_name['WechatMiniBindPhoneRes']
-_THIRDACCOUNTBINDWECHATINFO = DESCRIPTOR.message_types_by_name['ThirdAccountBindWeChatInfo']
-_THIRDACCOUNTBINDQQINFO = DESCRIPTOR.message_types_by_name['ThirdAccountBindQqInfo']
-_THIRDACCOUNTBINDINFO = DESCRIPTOR.message_types_by_name['ThirdAccountBindInfo']
-_THIRDACCOUNTBINDINFODATA = DESCRIPTOR.message_types_by_name['ThirdAccountBindInfoData']
-_THIRDACCOUNTBINDINFOREQ = DESCRIPTOR.message_types_by_name['ThirdAccountBindInfoReq']
-_THIRDACCOUNTBINDINFORES = DESCRIPTOR.message_types_by_name['ThirdAccountBindInfoRes']
-_BINDTHIRDACCOUNTREQ = DESCRIPTOR.message_types_by_name['BindThirdAccountReq']
-_BINDTHIRDACCOUNTRES = DESCRIPTOR.message_types_by_name['BindThirdAccountRes']
-_UNBINDTHIRDACCOUNTREQ = DESCRIPTOR.message_types_by_name['UnbindThirdAccountReq']
-_UNBINDTHIRDACCOUNTRES = DESCRIPTOR.message_types_by_name['UnbindThirdAccountRes']
-_GETQRCODELOGINCODEREQ = DESCRIPTOR.message_types_by_name['GetQrcodeLoginCodeReq']
-_GETQRCODELOGINCODERES = DESCRIPTOR.message_types_by_name['GetQrcodeLoginCodeRes']
-_QRCODESCANLOGINREQ = DESCRIPTOR.message_types_by_name['QrcodeScanLoginReq']
-_QRCODESCANLOGINRES = DESCRIPTOR.message_types_by_name['QrcodeScanLoginRes']
-_GETQRCODELOGINSTATUSREQ = DESCRIPTOR.message_types_by_name['GetQrcodeLoginStatusReq']
-_GETQRCODELOGINSTATUSRES = DESCRIPTOR.message_types_by_name['GetQrcodeLoginStatusRes']
-_SETQRCODELOGINSTATUSREQ = DESCRIPTOR.message_types_by_name['SetQrcodeLoginStatusReq']
-_SETQRCODELOGINSTATUSRES = DESCRIPTOR.message_types_by_name['SetQrcodeLoginStatusRes']
-_GETACCOUNTREGISTERSTATUSREQ = DESCRIPTOR.message_types_by_name['GetAccountRegisterStatusReq']
-_GETACCOUNTREGISTERSTATUSRES = DESCRIPTOR.message_types_by_name['GetAccountRegisterStatusRes']
-_GETUMENGPHONEREQ = DESCRIPTOR.message_types_by_name['GetUmengPhoneReq']
-_GETUMENGPHONERES = DESCRIPTOR.message_types_by_name['GetUmengPhoneRes']
-_ACCOUNTCROSSTYPEINFO = DESCRIPTOR.message_types_by_name['AccountCrossTypeInfo']
-_ACCOUNTCROSSTYPEINFOREQ = DESCRIPTOR.message_types_by_name['AccountCrossTypeInfoReq']
-_ACCOUNTCROSSTYPEINFORES = DESCRIPTOR.message_types_by_name['AccountCrossTypeInfoRes']
-_APPLYACCOUNTCROSSTYPEREQ = DESCRIPTOR.message_types_by_name['ApplyAccountCrossTypeReq']
-_APPLYACCOUNTCROSSTYPERES = DESCRIPTOR.message_types_by_name['ApplyAccountCrossTypeRes']
-_CHECKINAPPCHARGELIMITREQ = DESCRIPTOR.message_types_by_name['CheckInAppChargeLimitReq']
-_CHECKINAPPCHARGELIMITRES = DESCRIPTOR.message_types_by_name['CheckInAppChargeLimitRes']
-_GETALIPAYMINIORDERREQ = DESCRIPTOR.message_types_by_name['GetAlipayMiniOrderReq']
-_GETALIPAYMINIORDERREQ_EXTENDSENTRY = _GETALIPAYMINIORDERREQ.nested_types_by_name['ExtendsEntry']
-_GETALIPAYMINIORDERRES = DESCRIPTOR.message_types_by_name['GetAlipayMiniOrderRes']
-_GETGOODSLISTREQ = DESCRIPTOR.message_types_by_name['GetGoodsListReq']
-_GETGOODSLISTRES = DESCRIPTOR.message_types_by_name['GetGoodsListRes']
-_ALIPAYMINIINDEXITEM = DESCRIPTOR.message_types_by_name['AlipayMiniIndexItem']
-_ALIPAYMINIINDEXBANNER = DESCRIPTOR.message_types_by_name['AlipayMiniIndexBanner']
-_ALIPAYMINIINDEXGOODSLIST = DESCRIPTOR.message_types_by_name['AlipayMiniIndexGoodsList']
-_ALIPAYMINIINDEXGOODSITEM = DESCRIPTOR.message_types_by_name['AlipayMiniIndexGoodsItem']
-VerifyIAPReq = _reflection.GeneratedProtocolMessageType('VerifyIAPReq', (_message.Message,), {
-  'DESCRIPTOR' : _VERIFYIAPREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.VerifyIAPReq)
-  })
-_sym_db.RegisterMessage(VerifyIAPReq)
-
-VerifyIAPRes = _reflection.GeneratedProtocolMessageType('VerifyIAPRes', (_message.Message,), {
-  'DESCRIPTOR' : _VERIFYIAPRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.VerifyIAPRes)
-  })
-_sym_db.RegisterMessage(VerifyIAPRes)
-
-GoldCard = _reflection.GeneratedProtocolMessageType('GoldCard', (_message.Message,), {
-  'DESCRIPTOR' : _GOLDCARD,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GoldCard)
-  })
-_sym_db.RegisterMessage(GoldCard)
-
-GetGoodListReq = _reflection.GeneratedProtocolMessageType('GetGoodListReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETGOODLISTREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetGoodListReq)
-  })
-_sym_db.RegisterMessage(GetGoodListReq)
-
-GetGoodListRes = _reflection.GeneratedProtocolMessageType('GetGoodListRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETGOODLISTRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetGoodListRes)
-  })
-_sym_db.RegisterMessage(GetGoodListRes)
-
-OrderIAPReq = _reflection.GeneratedProtocolMessageType('OrderIAPReq', (_message.Message,), {
-  'DESCRIPTOR' : _ORDERIAPREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.OrderIAPReq)
-  })
-_sym_db.RegisterMessage(OrderIAPReq)
-
-OrderIAPRes = _reflection.GeneratedProtocolMessageType('OrderIAPRes', (_message.Message,), {
-  'DESCRIPTOR' : _ORDERIAPRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.OrderIAPRes)
-  })
-_sym_db.RegisterMessage(OrderIAPRes)
-
-CloseOrderIAPReq = _reflection.GeneratedProtocolMessageType('CloseOrderIAPReq', (_message.Message,), {
-  'DESCRIPTOR' : _CLOSEORDERIAPREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.CloseOrderIAPReq)
-  })
-_sym_db.RegisterMessage(CloseOrderIAPReq)
-
-CloseOrderIAPRes = _reflection.GeneratedProtocolMessageType('CloseOrderIAPRes', (_message.Message,), {
-  'DESCRIPTOR' : _CLOSEORDERIAPRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.CloseOrderIAPRes)
-  })
-_sym_db.RegisterMessage(CloseOrderIAPRes)
-
-VIPChargeAccountInfoReq = _reflection.GeneratedProtocolMessageType('VIPChargeAccountInfoReq', (_message.Message,), {
-  'DESCRIPTOR' : _VIPCHARGEACCOUNTINFOREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.VIPChargeAccountInfoReq)
-  })
-_sym_db.RegisterMessage(VIPChargeAccountInfoReq)
-
-VIPChargeAccountInfoRes = _reflection.GeneratedProtocolMessageType('VIPChargeAccountInfoRes', (_message.Message,), {
-  'DESCRIPTOR' : _VIPCHARGEACCOUNTINFORES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.VIPChargeAccountInfoRes)
-  })
-_sym_db.RegisterMessage(VIPChargeAccountInfoRes)
-
-VIPChargeLogReq = _reflection.GeneratedProtocolMessageType('VIPChargeLogReq', (_message.Message,), {
-  'DESCRIPTOR' : _VIPCHARGELOGREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.VIPChargeLogReq)
-  })
-_sym_db.RegisterMessage(VIPChargeLogReq)
-
-VIPChargeLogRes = _reflection.GeneratedProtocolMessageType('VIPChargeLogRes', (_message.Message,), {
-  'DESCRIPTOR' : _VIPCHARGELOGRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.VIPChargeLogRes)
-  })
-_sym_db.RegisterMessage(VIPChargeLogRes)
-
-VIPChargeLogs = _reflection.GeneratedProtocolMessageType('VIPChargeLogs', (_message.Message,), {
-  'DESCRIPTOR' : _VIPCHARGELOGS,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.VIPChargeLogs)
-  })
-_sym_db.RegisterMessage(VIPChargeLogs)
-
-VIPChargeItem = _reflection.GeneratedProtocolMessageType('VIPChargeItem', (_message.Message,), {
-  'DESCRIPTOR' : _VIPCHARGEITEM,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.VIPChargeItem)
-  })
-_sym_db.RegisterMessage(VIPChargeItem)
-
-ReportDataReq = _reflection.GeneratedProtocolMessageType('ReportDataReq', (_message.Message,), {
-  'DESCRIPTOR' : _REPORTDATAREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ReportDataReq)
-  })
-_sym_db.RegisterMessage(ReportDataReq)
-
-ReportDataRes = _reflection.GeneratedProtocolMessageType('ReportDataRes', (_message.Message,), {
-  'DESCRIPTOR' : _REPORTDATARES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ReportDataRes)
-  })
-_sym_db.RegisterMessage(ReportDataRes)
-
-GetChargeReq = _reflection.GeneratedProtocolMessageType('GetChargeReq', (_message.Message,), {
-
-  'ExtendsEntry' : _reflection.GeneratedProtocolMessageType('ExtendsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _GETCHARGEREQ_EXTENDSENTRY,
-    '__module__' : 'uauth_ext_pb2'
-    # @@protoc_insertion_point(class_scope:uauth_pb.GetChargeReq.ExtendsEntry)
-    })
-  ,
-
-  'ExtraDataEntry' : _reflection.GeneratedProtocolMessageType('ExtraDataEntry', (_message.Message,), {
-    'DESCRIPTOR' : _GETCHARGEREQ_EXTRADATAENTRY,
-    '__module__' : 'uauth_ext_pb2'
-    # @@protoc_insertion_point(class_scope:uauth_pb.GetChargeReq.ExtraDataEntry)
-    })
-  ,
-  'DESCRIPTOR' : _GETCHARGEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetChargeReq)
-  })
-_sym_db.RegisterMessage(GetChargeReq)
-_sym_db.RegisterMessage(GetChargeReq.ExtendsEntry)
-_sym_db.RegisterMessage(GetChargeReq.ExtraDataEntry)
-
-GetChargeRes = _reflection.GeneratedProtocolMessageType('GetChargeRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETCHARGERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetChargeRes)
-  })
-_sym_db.RegisterMessage(GetChargeRes)
-
-GetSmsCodeReq = _reflection.GeneratedProtocolMessageType('GetSmsCodeReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETSMSCODEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetSmsCodeReq)
-  })
-_sym_db.RegisterMessage(GetSmsCodeReq)
-
-GetSmsCodeRes = _reflection.GeneratedProtocolMessageType('GetSmsCodeRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETSMSCODERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetSmsCodeRes)
-  })
-_sym_db.RegisterMessage(GetSmsCodeRes)
-
-GetSmsTokenReq = _reflection.GeneratedProtocolMessageType('GetSmsTokenReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETSMSTOKENREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetSmsTokenReq)
-  })
-_sym_db.RegisterMessage(GetSmsTokenReq)
-
-GetSmsTokenRes = _reflection.GeneratedProtocolMessageType('GetSmsTokenRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETSMSTOKENRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetSmsTokenRes)
-  })
-_sym_db.RegisterMessage(GetSmsTokenRes)
-
-PhoneSmsCodeReq = _reflection.GeneratedProtocolMessageType('PhoneSmsCodeReq', (_message.Message,), {
-  'DESCRIPTOR' : _PHONESMSCODEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.PhoneSmsCodeReq)
-  })
-_sym_db.RegisterMessage(PhoneSmsCodeReq)
-
-PhoneSmsCodeRes = _reflection.GeneratedProtocolMessageType('PhoneSmsCodeRes', (_message.Message,), {
-  'DESCRIPTOR' : _PHONESMSCODERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.PhoneSmsCodeRes)
-  })
-_sym_db.RegisterMessage(PhoneSmsCodeRes)
-
-CheckPhoneSmsCodeReq = _reflection.GeneratedProtocolMessageType('CheckPhoneSmsCodeReq', (_message.Message,), {
-  'DESCRIPTOR' : _CHECKPHONESMSCODEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.CheckPhoneSmsCodeReq)
-  })
-_sym_db.RegisterMessage(CheckPhoneSmsCodeReq)
-
-CheckPhoneSmsCodeRes = _reflection.GeneratedProtocolMessageType('CheckPhoneSmsCodeRes', (_message.Message,), {
-  'DESCRIPTOR' : _CHECKPHONESMSCODERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.CheckPhoneSmsCodeRes)
-  })
-_sym_db.RegisterMessage(CheckPhoneSmsCodeRes)
-
-CommonSignInRes = _reflection.GeneratedProtocolMessageType('CommonSignInRes', (_message.Message,), {
-
-  'ExtendsEntry' : _reflection.GeneratedProtocolMessageType('ExtendsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _COMMONSIGNINRES_EXTENDSENTRY,
-    '__module__' : 'uauth_ext_pb2'
-    # @@protoc_insertion_point(class_scope:uauth_pb.CommonSignInRes.ExtendsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _COMMONSIGNINRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.CommonSignInRes)
-  })
-_sym_db.RegisterMessage(CommonSignInRes)
-_sym_db.RegisterMessage(CommonSignInRes.ExtendsEntry)
-
-SignInWithAppleReq = _reflection.GeneratedProtocolMessageType('SignInWithAppleReq', (_message.Message,), {
-  'DESCRIPTOR' : _SIGNINWITHAPPLEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.SignInWithAppleReq)
-  })
-_sym_db.RegisterMessage(SignInWithAppleReq)
-
-IdOrPhoneLoginReq = _reflection.GeneratedProtocolMessageType('IdOrPhoneLoginReq', (_message.Message,), {
-  'DESCRIPTOR' : _IDORPHONELOGINREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.IdOrPhoneLoginReq)
-  })
-_sym_db.RegisterMessage(IdOrPhoneLoginReq)
-
-LoginWithPhoneSMSReq = _reflection.GeneratedProtocolMessageType('LoginWithPhoneSMSReq', (_message.Message,), {
-  'DESCRIPTOR' : _LOGINWITHPHONESMSREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.LoginWithPhoneSMSReq)
-  })
-_sym_db.RegisterMessage(LoginWithPhoneSMSReq)
-
-ThirdLoginReq = _reflection.GeneratedProtocolMessageType('ThirdLoginReq', (_message.Message,), {
-  'DESCRIPTOR' : _THIRDLOGINREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdLoginReq)
-  })
-_sym_db.RegisterMessage(ThirdLoginReq)
-
-ChinaMobileQuickLoginReq = _reflection.GeneratedProtocolMessageType('ChinaMobileQuickLoginReq', (_message.Message,), {
-  'DESCRIPTOR' : _CHINAMOBILEQUICKLOGINREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ChinaMobileQuickLoginReq)
-  })
-_sym_db.RegisterMessage(ChinaMobileQuickLoginReq)
-
-ChinaTelecomAuthReq = _reflection.GeneratedProtocolMessageType('ChinaTelecomAuthReq', (_message.Message,), {
-  'DESCRIPTOR' : _CHINATELECOMAUTHREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ChinaTelecomAuthReq)
-  })
-_sym_db.RegisterMessage(ChinaTelecomAuthReq)
-
-UmengQuickLoginReq = _reflection.GeneratedProtocolMessageType('UmengQuickLoginReq', (_message.Message,), {
-  'DESCRIPTOR' : _UMENGQUICKLOGINREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.UmengQuickLoginReq)
-  })
-_sym_db.RegisterMessage(UmengQuickLoginReq)
-
-DevLoginReq = _reflection.GeneratedProtocolMessageType('DevLoginReq', (_message.Message,), {
-  'DESCRIPTOR' : _DEVLOGINREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.DevLoginReq)
-  })
-_sym_db.RegisterMessage(DevLoginReq)
-
-ResetPasswordReq = _reflection.GeneratedProtocolMessageType('ResetPasswordReq', (_message.Message,), {
-  'DESCRIPTOR' : _RESETPASSWORDREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ResetPasswordReq)
-  })
-_sym_db.RegisterMessage(ResetPasswordReq)
-
-ResetPasswordRes = _reflection.GeneratedProtocolMessageType('ResetPasswordRes', (_message.Message,), {
-  'DESCRIPTOR' : _RESETPASSWORDRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ResetPasswordRes)
-  })
-_sym_db.RegisterMessage(ResetPasswordRes)
-
-LoginSecretReq = _reflection.GeneratedProtocolMessageType('LoginSecretReq', (_message.Message,), {
-  'DESCRIPTOR' : _LOGINSECRETREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.LoginSecretReq)
-  })
-_sym_db.RegisterMessage(LoginSecretReq)
-
-LoginSecretRes = _reflection.GeneratedProtocolMessageType('LoginSecretRes', (_message.Message,), {
-  'DESCRIPTOR' : _LOGINSECRETRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.LoginSecretRes)
-  })
-_sym_db.RegisterMessage(LoginSecretRes)
-
-UpdatePasswdReq = _reflection.GeneratedProtocolMessageType('UpdatePasswdReq', (_message.Message,), {
-  'DESCRIPTOR' : _UPDATEPASSWDREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.UpdatePasswdReq)
-  })
-_sym_db.RegisterMessage(UpdatePasswdReq)
-
-UpdatePasswdRes = _reflection.GeneratedProtocolMessageType('UpdatePasswdRes', (_message.Message,), {
-  'DESCRIPTOR' : _UPDATEPASSWDRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.UpdatePasswdRes)
-  })
-_sym_db.RegisterMessage(UpdatePasswdRes)
-
-InviteReq = _reflection.GeneratedProtocolMessageType('InviteReq', (_message.Message,), {
-  'DESCRIPTOR' : _INVITEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.InviteReq)
-  })
-_sym_db.RegisterMessage(InviteReq)
-
-InviteRes = _reflection.GeneratedProtocolMessageType('InviteRes', (_message.Message,), {
-  'DESCRIPTOR' : _INVITERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.InviteRes)
-  })
-_sym_db.RegisterMessage(InviteRes)
-
-GetSyncTimeReq = _reflection.GeneratedProtocolMessageType('GetSyncTimeReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETSYNCTIMEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetSyncTimeReq)
-  })
-_sym_db.RegisterMessage(GetSyncTimeReq)
-
-GetSyncTimeRes = _reflection.GeneratedProtocolMessageType('GetSyncTimeRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETSYNCTIMERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetSyncTimeRes)
-  })
-_sym_db.RegisterMessage(GetSyncTimeRes)
-
-ReportBuyNobilityReq = _reflection.GeneratedProtocolMessageType('ReportBuyNobilityReq', (_message.Message,), {
-  'DESCRIPTOR' : _REPORTBUYNOBILITYREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ReportBuyNobilityReq)
-  })
-_sym_db.RegisterMessage(ReportBuyNobilityReq)
-
-ReportBuyNobilityRes = _reflection.GeneratedProtocolMessageType('ReportBuyNobilityRes', (_message.Message,), {
-  'DESCRIPTOR' : _REPORTBUYNOBILITYRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ReportBuyNobilityRes)
-  })
-_sym_db.RegisterMessage(ReportBuyNobilityRes)
-
-GoogleIABNotifyReq = _reflection.GeneratedProtocolMessageType('GoogleIABNotifyReq', (_message.Message,), {
-
-  'BuyIntent' : _reflection.GeneratedProtocolMessageType('BuyIntent', (_message.Message,), {
-    'DESCRIPTOR' : _GOOGLEIABNOTIFYREQ_BUYINTENT,
-    '__module__' : 'uauth_ext_pb2'
-    # @@protoc_insertion_point(class_scope:uauth_pb.GoogleIABNotifyReq.BuyIntent)
-    })
-  ,
-  'DESCRIPTOR' : _GOOGLEIABNOTIFYREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GoogleIABNotifyReq)
-  })
-_sym_db.RegisterMessage(GoogleIABNotifyReq)
-_sym_db.RegisterMessage(GoogleIABNotifyReq.BuyIntent)
-
-GoogleIABNotifyRes = _reflection.GeneratedProtocolMessageType('GoogleIABNotifyRes', (_message.Message,), {
-  'DESCRIPTOR' : _GOOGLEIABNOTIFYRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GoogleIABNotifyRes)
-  })
-_sym_db.RegisterMessage(GoogleIABNotifyRes)
-
-GoogleIABProductItem = _reflection.GeneratedProtocolMessageType('GoogleIABProductItem', (_message.Message,), {
-  'DESCRIPTOR' : _GOOGLEIABPRODUCTITEM,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GoogleIABProductItem)
-  })
-_sym_db.RegisterMessage(GoogleIABProductItem)
-
-GoogleIABProductItemsReq = _reflection.GeneratedProtocolMessageType('GoogleIABProductItemsReq', (_message.Message,), {
-  'DESCRIPTOR' : _GOOGLEIABPRODUCTITEMSREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GoogleIABProductItemsReq)
-  })
-_sym_db.RegisterMessage(GoogleIABProductItemsReq)
-
-GoogleIABProductItemsRes = _reflection.GeneratedProtocolMessageType('GoogleIABProductItemsRes', (_message.Message,), {
-  'DESCRIPTOR' : _GOOGLEIABPRODUCTITEMSRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GoogleIABProductItemsRes)
-  })
-_sym_db.RegisterMessage(GoogleIABProductItemsRes)
-
-GetWeChatAppIdReq = _reflection.GeneratedProtocolMessageType('GetWeChatAppIdReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETWECHATAPPIDREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetWeChatAppIdReq)
-  })
-_sym_db.RegisterMessage(GetWeChatAppIdReq)
-
-GetWeChatAppIdRes = _reflection.GeneratedProtocolMessageType('GetWeChatAppIdRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETWECHATAPPIDRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetWeChatAppIdRes)
-  })
-_sym_db.RegisterMessage(GetWeChatAppIdRes)
-
-GetWeChatIdLoginReq = _reflection.GeneratedProtocolMessageType('GetWeChatIdLoginReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETWECHATIDLOGINREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetWeChatIdLoginReq)
-  })
-_sym_db.RegisterMessage(GetWeChatIdLoginReq)
-
-GetWeChatIdLoginRes = _reflection.GeneratedProtocolMessageType('GetWeChatIdLoginRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETWECHATIDLOGINRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetWeChatIdLoginRes)
-  })
-_sym_db.RegisterMessage(GetWeChatIdLoginRes)
-
-UserInfo = _reflection.GeneratedProtocolMessageType('UserInfo', (_message.Message,), {
-  'DESCRIPTOR' : _USERINFO,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.UserInfo)
-  })
-_sym_db.RegisterMessage(UserInfo)
-
-GetMiniProgramLoginReq = _reflection.GeneratedProtocolMessageType('GetMiniProgramLoginReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETMINIPROGRAMLOGINREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetMiniProgramLoginReq)
-  })
-_sym_db.RegisterMessage(GetMiniProgramLoginReq)
-
-MiniProgramPhoneReq = _reflection.GeneratedProtocolMessageType('MiniProgramPhoneReq', (_message.Message,), {
-  'DESCRIPTOR' : _MINIPROGRAMPHONEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.MiniProgramPhoneReq)
-  })
-_sym_db.RegisterMessage(MiniProgramPhoneReq)
-
-MiniProgramPhoneRes = _reflection.GeneratedProtocolMessageType('MiniProgramPhoneRes', (_message.Message,), {
-  'DESCRIPTOR' : _MINIPROGRAMPHONERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.MiniProgramPhoneRes)
-  })
-_sym_db.RegisterMessage(MiniProgramPhoneRes)
-
-ApplyCertifyReq = _reflection.GeneratedProtocolMessageType('ApplyCertifyReq', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTIFYREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ApplyCertifyReq)
-  })
-_sym_db.RegisterMessage(ApplyCertifyReq)
-
-ApplyCertifyRes = _reflection.GeneratedProtocolMessageType('ApplyCertifyRes', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTIFYRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ApplyCertifyRes)
-  })
-_sym_db.RegisterMessage(ApplyCertifyRes)
-
-ApplyCertifySignReq = _reflection.GeneratedProtocolMessageType('ApplyCertifySignReq', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYCERTIFYSIGNREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ApplyCertifySignReq)
-  })
-_sym_db.RegisterMessage(ApplyCertifySignReq)
-
-CertifyResultReq = _reflection.GeneratedProtocolMessageType('CertifyResultReq', (_message.Message,), {
-  'DESCRIPTOR' : _CERTIFYRESULTREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.CertifyResultReq)
-  })
-_sym_db.RegisterMessage(CertifyResultReq)
-
-CertifyResultRes = _reflection.GeneratedProtocolMessageType('CertifyResultRes', (_message.Message,), {
-  'DESCRIPTOR' : _CERTIFYRESULTRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.CertifyResultRes)
-  })
-_sym_db.RegisterMessage(CertifyResultRes)
-
-AccountPhoneSmsCodeReq = _reflection.GeneratedProtocolMessageType('AccountPhoneSmsCodeReq', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTPHONESMSCODEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountPhoneSmsCodeReq)
-  })
-_sym_db.RegisterMessage(AccountPhoneSmsCodeReq)
-
-AccountPhoneSmsCodeRes = _reflection.GeneratedProtocolMessageType('AccountPhoneSmsCodeRes', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTPHONESMSCODERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountPhoneSmsCodeRes)
-  })
-_sym_db.RegisterMessage(AccountPhoneSmsCodeRes)
-
-AccountSubsidiaryLoginReq = _reflection.GeneratedProtocolMessageType('AccountSubsidiaryLoginReq', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTSUBSIDIARYLOGINREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountSubsidiaryLoginReq)
-  })
-_sym_db.RegisterMessage(AccountSubsidiaryLoginReq)
-
-GetGuestLoginReq = _reflection.GeneratedProtocolMessageType('GetGuestLoginReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETGUESTLOGINREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetGuestLoginReq)
-  })
-_sym_db.RegisterMessage(GetGuestLoginReq)
-
-AccountBindPhoneSMSReq = _reflection.GeneratedProtocolMessageType('AccountBindPhoneSMSReq', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTBINDPHONESMSREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindPhoneSMSReq)
-  })
-_sym_db.RegisterMessage(AccountBindPhoneSMSReq)
-
-AccountBindPhoneSMSRes = _reflection.GeneratedProtocolMessageType('AccountBindPhoneSMSRes', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTBINDPHONESMSRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindPhoneSMSRes)
-  })
-_sym_db.RegisterMessage(AccountBindPhoneSMSRes)
-
-AccountBindThirdReq = _reflection.GeneratedProtocolMessageType('AccountBindThirdReq', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTBINDTHIRDREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindThirdReq)
-  })
-_sym_db.RegisterMessage(AccountBindThirdReq)
-
-AccountBindThirdRes = _reflection.GeneratedProtocolMessageType('AccountBindThirdRes', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTBINDTHIRDRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindThirdRes)
-  })
-_sym_db.RegisterMessage(AccountBindThirdRes)
-
-AccountBindListReq = _reflection.GeneratedProtocolMessageType('AccountBindListReq', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTBINDLISTREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindListReq)
-  })
-_sym_db.RegisterMessage(AccountBindListReq)
-
-AccountBindListRes = _reflection.GeneratedProtocolMessageType('AccountBindListRes', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTBINDLISTRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindListRes)
-  })
-_sym_db.RegisterMessage(AccountBindListRes)
-
-BindPhoneSmsCodeReq = _reflection.GeneratedProtocolMessageType('BindPhoneSmsCodeReq', (_message.Message,), {
-  'DESCRIPTOR' : _BINDPHONESMSCODEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.BindPhoneSmsCodeReq)
-  })
-_sym_db.RegisterMessage(BindPhoneSmsCodeReq)
-
-BindPhoneSmsCodeRes = _reflection.GeneratedProtocolMessageType('BindPhoneSmsCodeRes', (_message.Message,), {
-  'DESCRIPTOR' : _BINDPHONESMSCODERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.BindPhoneSmsCodeRes)
-  })
-_sym_db.RegisterMessage(BindPhoneSmsCodeRes)
-
-BindEmailSesCodeReq = _reflection.GeneratedProtocolMessageType('BindEmailSesCodeReq', (_message.Message,), {
-  'DESCRIPTOR' : _BINDEMAILSESCODEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.BindEmailSesCodeReq)
-  })
-_sym_db.RegisterMessage(BindEmailSesCodeReq)
-
-BindEmailSesCodeRes = _reflection.GeneratedProtocolMessageType('BindEmailSesCodeRes', (_message.Message,), {
-  'DESCRIPTOR' : _BINDEMAILSESCODERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.BindEmailSesCodeRes)
-  })
-_sym_db.RegisterMessage(BindEmailSesCodeRes)
-
-AccountBindEmailSESReq = _reflection.GeneratedProtocolMessageType('AccountBindEmailSESReq', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTBINDEMAILSESREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindEmailSESReq)
-  })
-_sym_db.RegisterMessage(AccountBindEmailSESReq)
-
-AccountBindEmailSESRes = _reflection.GeneratedProtocolMessageType('AccountBindEmailSESRes', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTBINDEMAILSESRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindEmailSESRes)
-  })
-_sym_db.RegisterMessage(AccountBindEmailSESRes)
-
-GetAccountRegisterReq = _reflection.GeneratedProtocolMessageType('GetAccountRegisterReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETACCOUNTREGISTERREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetAccountRegisterReq)
-  })
-_sym_db.RegisterMessage(GetAccountRegisterReq)
-
-GetAccountPasswordLoginReq = _reflection.GeneratedProtocolMessageType('GetAccountPasswordLoginReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETACCOUNTPASSWORDLOGINREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetAccountPasswordLoginReq)
-  })
-_sym_db.RegisterMessage(GetAccountPasswordLoginReq)
-
-GetSesCodeReq = _reflection.GeneratedProtocolMessageType('GetSesCodeReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETSESCODEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetSesCodeReq)
-  })
-_sym_db.RegisterMessage(GetSesCodeReq)
-
-GetSesCodeRes = _reflection.GeneratedProtocolMessageType('GetSesCodeRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETSESCODERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetSesCodeRes)
-  })
-_sym_db.RegisterMessage(GetSesCodeRes)
-
-GetSesTokenReq = _reflection.GeneratedProtocolMessageType('GetSesTokenReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETSESTOKENREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetSesTokenReq)
-  })
-_sym_db.RegisterMessage(GetSesTokenReq)
-
-GetSesTokenRes = _reflection.GeneratedProtocolMessageType('GetSesTokenRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETSESTOKENRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetSesTokenRes)
-  })
-_sym_db.RegisterMessage(GetSesTokenRes)
-
-ResetPasswordBySesReq = _reflection.GeneratedProtocolMessageType('ResetPasswordBySesReq', (_message.Message,), {
-  'DESCRIPTOR' : _RESETPASSWORDBYSESREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ResetPasswordBySesReq)
-  })
-_sym_db.RegisterMessage(ResetPasswordBySesReq)
-
-ResetPasswordBySesRes = _reflection.GeneratedProtocolMessageType('ResetPasswordBySesRes', (_message.Message,), {
-  'DESCRIPTOR' : _RESETPASSWORDBYSESRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ResetPasswordBySesRes)
-  })
-_sym_db.RegisterMessage(ResetPasswordBySesRes)
-
-RemoteLoginSendCodeReq = _reflection.GeneratedProtocolMessageType('RemoteLoginSendCodeReq', (_message.Message,), {
-  'DESCRIPTOR' : _REMOTELOGINSENDCODEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.RemoteLoginSendCodeReq)
-  })
-_sym_db.RegisterMessage(RemoteLoginSendCodeReq)
-
-RemoteLoginSendCodeRes = _reflection.GeneratedProtocolMessageType('RemoteLoginSendCodeRes', (_message.Message,), {
-  'DESCRIPTOR' : _REMOTELOGINSENDCODERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.RemoteLoginSendCodeRes)
-  })
-_sym_db.RegisterMessage(RemoteLoginSendCodeRes)
-
-RemoteLoginConfirmCodeReq = _reflection.GeneratedProtocolMessageType('RemoteLoginConfirmCodeReq', (_message.Message,), {
-  'DESCRIPTOR' : _REMOTELOGINCONFIRMCODEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.RemoteLoginConfirmCodeReq)
-  })
-_sym_db.RegisterMessage(RemoteLoginConfirmCodeReq)
-
-RemoteLoginConfirmCodeRes = _reflection.GeneratedProtocolMessageType('RemoteLoginConfirmCodeRes', (_message.Message,), {
-  'DESCRIPTOR' : _REMOTELOGINCONFIRMCODERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.RemoteLoginConfirmCodeRes)
-  })
-_sym_db.RegisterMessage(RemoteLoginConfirmCodeRes)
-
-VerifyCancelSignInWithAppleReq = _reflection.GeneratedProtocolMessageType('VerifyCancelSignInWithAppleReq', (_message.Message,), {
-  'DESCRIPTOR' : _VERIFYCANCELSIGNINWITHAPPLEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.VerifyCancelSignInWithAppleReq)
-  })
-_sym_db.RegisterMessage(VerifyCancelSignInWithAppleReq)
-
-VerifyCancelSignInWithAppleRes = _reflection.GeneratedProtocolMessageType('VerifyCancelSignInWithAppleRes', (_message.Message,), {
-  'DESCRIPTOR' : _VERIFYCANCELSIGNINWITHAPPLERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.VerifyCancelSignInWithAppleRes)
-  })
-_sym_db.RegisterMessage(VerifyCancelSignInWithAppleRes)
-
-WechatCodeLoginTicketReq = _reflection.GeneratedProtocolMessageType('WechatCodeLoginTicketReq', (_message.Message,), {
-  'DESCRIPTOR' : _WECHATCODELOGINTICKETREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.WechatCodeLoginTicketReq)
-  })
-_sym_db.RegisterMessage(WechatCodeLoginTicketReq)
-
-WechatCodeLoginTicketRes = _reflection.GeneratedProtocolMessageType('WechatCodeLoginTicketRes', (_message.Message,), {
-  'DESCRIPTOR' : _WECHATCODELOGINTICKETRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.WechatCodeLoginTicketRes)
-  })
-_sym_db.RegisterMessage(WechatCodeLoginTicketRes)
-
-GetWechatMiniCodeReq = _reflection.GeneratedProtocolMessageType('GetWechatMiniCodeReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETWECHATMINICODEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetWechatMiniCodeReq)
-  })
-_sym_db.RegisterMessage(GetWechatMiniCodeReq)
-
-GetWechatMiniCodeRes = _reflection.GeneratedProtocolMessageType('GetWechatMiniCodeRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETWECHATMINICODERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetWechatMiniCodeRes)
-  })
-_sym_db.RegisterMessage(GetWechatMiniCodeRes)
-
-GetWechatMiniCodeScanReq = _reflection.GeneratedProtocolMessageType('GetWechatMiniCodeScanReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETWECHATMINICODESCANREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetWechatMiniCodeScanReq)
-  })
-_sym_db.RegisterMessage(GetWechatMiniCodeScanReq)
-
-GetWechatMiniCodeScanRes = _reflection.GeneratedProtocolMessageType('GetWechatMiniCodeScanRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETWECHATMINICODESCANRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetWechatMiniCodeScanRes)
-  })
-_sym_db.RegisterMessage(GetWechatMiniCodeScanRes)
-
-RefusePhoneLicenseReq = _reflection.GeneratedProtocolMessageType('RefusePhoneLicenseReq', (_message.Message,), {
-  'DESCRIPTOR' : _REFUSEPHONELICENSEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.RefusePhoneLicenseReq)
-  })
-_sym_db.RegisterMessage(RefusePhoneLicenseReq)
-
-RefusePhoneLicenseRes = _reflection.GeneratedProtocolMessageType('RefusePhoneLicenseRes', (_message.Message,), {
-  'DESCRIPTOR' : _REFUSEPHONELICENSERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.RefusePhoneLicenseRes)
-  })
-_sym_db.RegisterMessage(RefusePhoneLicenseRes)
-
-WechatMiniBindPhoneReq = _reflection.GeneratedProtocolMessageType('WechatMiniBindPhoneReq', (_message.Message,), {
-  'DESCRIPTOR' : _WECHATMINIBINDPHONEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.WechatMiniBindPhoneReq)
-  })
-_sym_db.RegisterMessage(WechatMiniBindPhoneReq)
-
-WechatMiniBindPhoneRes = _reflection.GeneratedProtocolMessageType('WechatMiniBindPhoneRes', (_message.Message,), {
-  'DESCRIPTOR' : _WECHATMINIBINDPHONERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.WechatMiniBindPhoneRes)
-  })
-_sym_db.RegisterMessage(WechatMiniBindPhoneRes)
-
-ThirdAccountBindWeChatInfo = _reflection.GeneratedProtocolMessageType('ThirdAccountBindWeChatInfo', (_message.Message,), {
-  'DESCRIPTOR' : _THIRDACCOUNTBINDWECHATINFO,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdAccountBindWeChatInfo)
-  })
-_sym_db.RegisterMessage(ThirdAccountBindWeChatInfo)
-
-ThirdAccountBindQqInfo = _reflection.GeneratedProtocolMessageType('ThirdAccountBindQqInfo', (_message.Message,), {
-  'DESCRIPTOR' : _THIRDACCOUNTBINDQQINFO,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdAccountBindQqInfo)
-  })
-_sym_db.RegisterMessage(ThirdAccountBindQqInfo)
-
-ThirdAccountBindInfo = _reflection.GeneratedProtocolMessageType('ThirdAccountBindInfo', (_message.Message,), {
-  'DESCRIPTOR' : _THIRDACCOUNTBINDINFO,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdAccountBindInfo)
-  })
-_sym_db.RegisterMessage(ThirdAccountBindInfo)
-
-ThirdAccountBindInfoData = _reflection.GeneratedProtocolMessageType('ThirdAccountBindInfoData', (_message.Message,), {
-  'DESCRIPTOR' : _THIRDACCOUNTBINDINFODATA,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdAccountBindInfoData)
-  })
-_sym_db.RegisterMessage(ThirdAccountBindInfoData)
-
-ThirdAccountBindInfoReq = _reflection.GeneratedProtocolMessageType('ThirdAccountBindInfoReq', (_message.Message,), {
-  'DESCRIPTOR' : _THIRDACCOUNTBINDINFOREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdAccountBindInfoReq)
-  })
-_sym_db.RegisterMessage(ThirdAccountBindInfoReq)
-
-ThirdAccountBindInfoRes = _reflection.GeneratedProtocolMessageType('ThirdAccountBindInfoRes', (_message.Message,), {
-  'DESCRIPTOR' : _THIRDACCOUNTBINDINFORES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdAccountBindInfoRes)
-  })
-_sym_db.RegisterMessage(ThirdAccountBindInfoRes)
-
-BindThirdAccountReq = _reflection.GeneratedProtocolMessageType('BindThirdAccountReq', (_message.Message,), {
-  'DESCRIPTOR' : _BINDTHIRDACCOUNTREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.BindThirdAccountReq)
-  })
-_sym_db.RegisterMessage(BindThirdAccountReq)
-
-BindThirdAccountRes = _reflection.GeneratedProtocolMessageType('BindThirdAccountRes', (_message.Message,), {
-  'DESCRIPTOR' : _BINDTHIRDACCOUNTRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.BindThirdAccountRes)
-  })
-_sym_db.RegisterMessage(BindThirdAccountRes)
-
-UnbindThirdAccountReq = _reflection.GeneratedProtocolMessageType('UnbindThirdAccountReq', (_message.Message,), {
-  'DESCRIPTOR' : _UNBINDTHIRDACCOUNTREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.UnbindThirdAccountReq)
-  })
-_sym_db.RegisterMessage(UnbindThirdAccountReq)
-
-UnbindThirdAccountRes = _reflection.GeneratedProtocolMessageType('UnbindThirdAccountRes', (_message.Message,), {
-  'DESCRIPTOR' : _UNBINDTHIRDACCOUNTRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.UnbindThirdAccountRes)
-  })
-_sym_db.RegisterMessage(UnbindThirdAccountRes)
-
-GetQrcodeLoginCodeReq = _reflection.GeneratedProtocolMessageType('GetQrcodeLoginCodeReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETQRCODELOGINCODEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetQrcodeLoginCodeReq)
-  })
-_sym_db.RegisterMessage(GetQrcodeLoginCodeReq)
-
-GetQrcodeLoginCodeRes = _reflection.GeneratedProtocolMessageType('GetQrcodeLoginCodeRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETQRCODELOGINCODERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetQrcodeLoginCodeRes)
-  })
-_sym_db.RegisterMessage(GetQrcodeLoginCodeRes)
-
-QrcodeScanLoginReq = _reflection.GeneratedProtocolMessageType('QrcodeScanLoginReq', (_message.Message,), {
-  'DESCRIPTOR' : _QRCODESCANLOGINREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.QrcodeScanLoginReq)
-  })
-_sym_db.RegisterMessage(QrcodeScanLoginReq)
-
-QrcodeScanLoginRes = _reflection.GeneratedProtocolMessageType('QrcodeScanLoginRes', (_message.Message,), {
-  'DESCRIPTOR' : _QRCODESCANLOGINRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.QrcodeScanLoginRes)
-  })
-_sym_db.RegisterMessage(QrcodeScanLoginRes)
-
-GetQrcodeLoginStatusReq = _reflection.GeneratedProtocolMessageType('GetQrcodeLoginStatusReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETQRCODELOGINSTATUSREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetQrcodeLoginStatusReq)
-  })
-_sym_db.RegisterMessage(GetQrcodeLoginStatusReq)
-
-GetQrcodeLoginStatusRes = _reflection.GeneratedProtocolMessageType('GetQrcodeLoginStatusRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETQRCODELOGINSTATUSRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetQrcodeLoginStatusRes)
-  })
-_sym_db.RegisterMessage(GetQrcodeLoginStatusRes)
-
-SetQrcodeLoginStatusReq = _reflection.GeneratedProtocolMessageType('SetQrcodeLoginStatusReq', (_message.Message,), {
-  'DESCRIPTOR' : _SETQRCODELOGINSTATUSREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.SetQrcodeLoginStatusReq)
-  })
-_sym_db.RegisterMessage(SetQrcodeLoginStatusReq)
-
-SetQrcodeLoginStatusRes = _reflection.GeneratedProtocolMessageType('SetQrcodeLoginStatusRes', (_message.Message,), {
-  'DESCRIPTOR' : _SETQRCODELOGINSTATUSRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.SetQrcodeLoginStatusRes)
-  })
-_sym_db.RegisterMessage(SetQrcodeLoginStatusRes)
-
-GetAccountRegisterStatusReq = _reflection.GeneratedProtocolMessageType('GetAccountRegisterStatusReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETACCOUNTREGISTERSTATUSREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetAccountRegisterStatusReq)
-  })
-_sym_db.RegisterMessage(GetAccountRegisterStatusReq)
-
-GetAccountRegisterStatusRes = _reflection.GeneratedProtocolMessageType('GetAccountRegisterStatusRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETACCOUNTREGISTERSTATUSRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetAccountRegisterStatusRes)
-  })
-_sym_db.RegisterMessage(GetAccountRegisterStatusRes)
-
-GetUmengPhoneReq = _reflection.GeneratedProtocolMessageType('GetUmengPhoneReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETUMENGPHONEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetUmengPhoneReq)
-  })
-_sym_db.RegisterMessage(GetUmengPhoneReq)
-
-GetUmengPhoneRes = _reflection.GeneratedProtocolMessageType('GetUmengPhoneRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETUMENGPHONERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetUmengPhoneRes)
-  })
-_sym_db.RegisterMessage(GetUmengPhoneRes)
-
-AccountCrossTypeInfo = _reflection.GeneratedProtocolMessageType('AccountCrossTypeInfo', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTCROSSTYPEINFO,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountCrossTypeInfo)
-  })
-_sym_db.RegisterMessage(AccountCrossTypeInfo)
-
-AccountCrossTypeInfoReq = _reflection.GeneratedProtocolMessageType('AccountCrossTypeInfoReq', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTCROSSTYPEINFOREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountCrossTypeInfoReq)
-  })
-_sym_db.RegisterMessage(AccountCrossTypeInfoReq)
-
-AccountCrossTypeInfoRes = _reflection.GeneratedProtocolMessageType('AccountCrossTypeInfoRes', (_message.Message,), {
-  'DESCRIPTOR' : _ACCOUNTCROSSTYPEINFORES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AccountCrossTypeInfoRes)
-  })
-_sym_db.RegisterMessage(AccountCrossTypeInfoRes)
-
-ApplyAccountCrossTypeReq = _reflection.GeneratedProtocolMessageType('ApplyAccountCrossTypeReq', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYACCOUNTCROSSTYPEREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ApplyAccountCrossTypeReq)
-  })
-_sym_db.RegisterMessage(ApplyAccountCrossTypeReq)
-
-ApplyAccountCrossTypeRes = _reflection.GeneratedProtocolMessageType('ApplyAccountCrossTypeRes', (_message.Message,), {
-  'DESCRIPTOR' : _APPLYACCOUNTCROSSTYPERES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.ApplyAccountCrossTypeRes)
-  })
-_sym_db.RegisterMessage(ApplyAccountCrossTypeRes)
-
-CheckInAppChargeLimitReq = _reflection.GeneratedProtocolMessageType('CheckInAppChargeLimitReq', (_message.Message,), {
-  'DESCRIPTOR' : _CHECKINAPPCHARGELIMITREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.CheckInAppChargeLimitReq)
-  })
-_sym_db.RegisterMessage(CheckInAppChargeLimitReq)
-
-CheckInAppChargeLimitRes = _reflection.GeneratedProtocolMessageType('CheckInAppChargeLimitRes', (_message.Message,), {
-  'DESCRIPTOR' : _CHECKINAPPCHARGELIMITRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.CheckInAppChargeLimitRes)
-  })
-_sym_db.RegisterMessage(CheckInAppChargeLimitRes)
-
-GetAlipayMiniOrderReq = _reflection.GeneratedProtocolMessageType('GetAlipayMiniOrderReq', (_message.Message,), {
-
-  'ExtendsEntry' : _reflection.GeneratedProtocolMessageType('ExtendsEntry', (_message.Message,), {
-    'DESCRIPTOR' : _GETALIPAYMINIORDERREQ_EXTENDSENTRY,
-    '__module__' : 'uauth_ext_pb2'
-    # @@protoc_insertion_point(class_scope:uauth_pb.GetAlipayMiniOrderReq.ExtendsEntry)
-    })
-  ,
-  'DESCRIPTOR' : _GETALIPAYMINIORDERREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetAlipayMiniOrderReq)
-  })
-_sym_db.RegisterMessage(GetAlipayMiniOrderReq)
-_sym_db.RegisterMessage(GetAlipayMiniOrderReq.ExtendsEntry)
-
-GetAlipayMiniOrderRes = _reflection.GeneratedProtocolMessageType('GetAlipayMiniOrderRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETALIPAYMINIORDERRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetAlipayMiniOrderRes)
-  })
-_sym_db.RegisterMessage(GetAlipayMiniOrderRes)
-
-GetGoodsListReq = _reflection.GeneratedProtocolMessageType('GetGoodsListReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETGOODSLISTREQ,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetGoodsListReq)
-  })
-_sym_db.RegisterMessage(GetGoodsListReq)
-
-GetGoodsListRes = _reflection.GeneratedProtocolMessageType('GetGoodsListRes', (_message.Message,), {
-  'DESCRIPTOR' : _GETGOODSLISTRES,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.GetGoodsListRes)
-  })
-_sym_db.RegisterMessage(GetGoodsListRes)
-
-AlipayMiniIndexItem = _reflection.GeneratedProtocolMessageType('AlipayMiniIndexItem', (_message.Message,), {
-  'DESCRIPTOR' : _ALIPAYMINIINDEXITEM,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AlipayMiniIndexItem)
-  })
-_sym_db.RegisterMessage(AlipayMiniIndexItem)
-
-AlipayMiniIndexBanner = _reflection.GeneratedProtocolMessageType('AlipayMiniIndexBanner', (_message.Message,), {
-  'DESCRIPTOR' : _ALIPAYMINIINDEXBANNER,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AlipayMiniIndexBanner)
-  })
-_sym_db.RegisterMessage(AlipayMiniIndexBanner)
-
-AlipayMiniIndexGoodsList = _reflection.GeneratedProtocolMessageType('AlipayMiniIndexGoodsList', (_message.Message,), {
-  'DESCRIPTOR' : _ALIPAYMINIINDEXGOODSLIST,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AlipayMiniIndexGoodsList)
-  })
-_sym_db.RegisterMessage(AlipayMiniIndexGoodsList)
-
-AlipayMiniIndexGoodsItem = _reflection.GeneratedProtocolMessageType('AlipayMiniIndexGoodsItem', (_message.Message,), {
-  'DESCRIPTOR' : _ALIPAYMINIINDEXGOODSITEM,
-  '__module__' : 'uauth_ext_pb2'
-  # @@protoc_insertion_point(class_scope:uauth_pb.AlipayMiniIndexGoodsItem)
-  })
-_sym_db.RegisterMessage(AlipayMiniIndexGoodsItem)
-
-_UAUTHEXTOBJ = DESCRIPTOR.services_by_name['UauthExtObj']
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\242\002\005PROTO'
-  _GETCHARGEREQ_EXTENDSENTRY._options = None
-  _GETCHARGEREQ_EXTENDSENTRY._serialized_options = b'8\001'
-  _GETCHARGEREQ_EXTRADATAENTRY._options = None
-  _GETCHARGEREQ_EXTRADATAENTRY._serialized_options = b'8\001'
-  _COMMONSIGNINRES_EXTENDSENTRY._options = None
-  _COMMONSIGNINRES_EXTENDSENTRY._serialized_options = b'8\001'
-  _GETALIPAYMINIORDERREQ_EXTENDSENTRY._options = None
-  _GETALIPAYMINIORDERREQ_EXTENDSENTRY._serialized_options = b'8\001'
-  _ERRORUAUTHCODE._serialized_start=11797
-  _ERRORUAUTHCODE._serialized_end=12699
-  _IAPSTATUSTYPE._serialized_start=12701
-  _IAPSTATUSTYPE._serialized_end=12774
-  _CHARGESTATUS._serialized_start=12776
-  _CHARGESTATUS._serialized_end=12837
-  _REPORTDATATYPE._serialized_start=12839
-  _REPORTDATATYPE._serialized_end=12896
-  _VERIFYTYPE._serialized_start=12898
-  _VERIFYTYPE._serialized_end=12980
-  _SMSCODETPL._serialized_start=12982
-  _SMSCODETPL._serialized_end=13089
-  _CERTIFYTYPE._serialized_start=13091
-  _CERTIFYTYPE._serialized_end=13132
-  _WECHATMINICODESCANSTATUS._serialized_start=13135
-  _WECHATMINICODESCANSTATUS._serialized_end=13265
-  _THIRDACCOUNTBINDTYPE._serialized_start=13267
-  _THIRDACCOUNTBINDTYPE._serialized_end=13334
-  _UNBINDTHIRDACCOUNTOPTTYPE._serialized_start=13336
-  _UNBINDTHIRDACCOUNTOPTTYPE._serialized_end=13397
-  _GETQRCODELOGINSTATUS._serialized_start=13399
-  _GETQRCODELOGINSTATUS._serialized_end=13482
-  _ACCOUNTREGISTERTYPE._serialized_start=13484
-  _ACCOUNTREGISTERTYPE._serialized_end=13546
-  _ACCOUNTAPPCROSSTYPE._serialized_start=13548
-  _ACCOUNTAPPCROSSTYPE._serialized_end=13599
-  _APPCHARGETYPE._serialized_start=13601
-  _APPCHARGETYPE._serialized_end=13661
-  _ALIPAYMINIINDEXTYPE._serialized_start=13663
-  _ALIPAYMINIINDEXTYPE._serialized_end=13732
-  _ALIPAYMINIGOODSTYPE._serialized_start=13734
-  _ALIPAYMINIGOODSTYPE._serialized_end=13785
-  _VERIFYIAPREQ._serialized_start=49
-  _VERIFYIAPREQ._serialized_end=158
-  _VERIFYIAPRES._serialized_start=160
-  _VERIFYIAPRES._serialized_end=174
-  _GOLDCARD._serialized_start=176
-  _GOLDCARD._serialized_end=273
-  _GETGOODLISTREQ._serialized_start=275
-  _GETGOODLISTREQ._serialized_end=291
-  _GETGOODLISTRES._serialized_start=293
-  _GETGOODLISTRES._serialized_end=365
-  _ORDERIAPREQ._serialized_start=367
-  _ORDERIAPREQ._serialized_end=411
-  _ORDERIAPRES._serialized_start=413
-  _ORDERIAPRES._serialized_end=444
-  _CLOSEORDERIAPREQ._serialized_start=446
-  _CLOSEORDERIAPREQ._serialized_end=523
-  _CLOSEORDERIAPRES._serialized_start=525
-  _CLOSEORDERIAPRES._serialized_end=543
-  _VIPCHARGEACCOUNTINFOREQ._serialized_start=545
-  _VIPCHARGEACCOUNTINFOREQ._serialized_end=582
-  _VIPCHARGEACCOUNTINFORES._serialized_start=585
-  _VIPCHARGEACCOUNTINFORES._serialized_end=726
-  _VIPCHARGELOGREQ._serialized_start=728
-  _VIPCHARGELOGREQ._serialized_end=745
-  _VIPCHARGELOGRES._serialized_start=747
-  _VIPCHARGELOGRES._serialized_end=803
-  _VIPCHARGELOGS._serialized_start=805
-  _VIPCHARGELOGS._serialized_end=872
-  _VIPCHARGEITEM._serialized_start=874
-  _VIPCHARGEITEM._serialized_end=994
-  _REPORTDATAREQ._serialized_start=996
-  _REPORTDATAREQ._serialized_end=1065
-  _REPORTDATARES._serialized_start=1067
-  _REPORTDATARES._serialized_end=1082
-  _GETCHARGEREQ._serialized_start=1085
-  _GETCHARGEREQ._serialized_end=1461
-  _GETCHARGEREQ_EXTENDSENTRY._serialized_start=1365
-  _GETCHARGEREQ_EXTENDSENTRY._serialized_end=1411
-  _GETCHARGEREQ_EXTRADATAENTRY._serialized_start=1413
-  _GETCHARGEREQ_EXTRADATAENTRY._serialized_end=1461
-  _GETCHARGERES._serialized_start=1463
-  _GETCHARGERES._serialized_end=1543
-  _GETSMSCODEREQ._serialized_start=1545
-  _GETSMSCODEREQ._serialized_end=1659
-  _GETSMSCODERES._serialized_start=1661
-  _GETSMSCODERES._serialized_end=1676
-  _GETSMSTOKENREQ._serialized_start=1679
-  _GETSMSTOKENREQ._serialized_end=1812
-  _GETSMSTOKENRES._serialized_start=1814
-  _GETSMSTOKENRES._serialized_end=1849
-  _PHONESMSCODEREQ._serialized_start=1851
-  _PHONESMSCODEREQ._serialized_end=1912
-  _PHONESMSCODERES._serialized_start=1914
-  _PHONESMSCODERES._serialized_end=1931
-  _CHECKPHONESMSCODEREQ._serialized_start=1933
-  _CHECKPHONESMSCODEREQ._serialized_end=2017
-  _CHECKPHONESMSCODERES._serialized_start=2019
-  _CHECKPHONESMSCODERES._serialized_end=2041
-  _COMMONSIGNINRES._serialized_start=2044
-  _COMMONSIGNINRES._serialized_end=2266
-  _COMMONSIGNINRES_EXTENDSENTRY._serialized_start=1365
-  _COMMONSIGNINRES_EXTENDSENTRY._serialized_end=1411
-  _SIGNINWITHAPPLEREQ._serialized_start=2269
-  _SIGNINWITHAPPLEREQ._serialized_end=2475
-  _IDORPHONELOGINREQ._serialized_start=2478
-  _IDORPHONELOGINREQ._serialized_end=2627
-  _LOGINWITHPHONESMSREQ._serialized_start=2630
-  _LOGINWITHPHONESMSREQ._serialized_end=2921
-  _THIRDLOGINREQ._serialized_start=2924
-  _THIRDLOGINREQ._serialized_end=3212
-  _CHINAMOBILEQUICKLOGINREQ._serialized_start=3215
-  _CHINAMOBILEQUICKLOGINREQ._serialized_end=3425
-  _CHINATELECOMAUTHREQ._serialized_start=3428
-  _CHINATELECOMAUTHREQ._serialized_end=3624
-  _UMENGQUICKLOGINREQ._serialized_start=3627
-  _UMENGQUICKLOGINREQ._serialized_end=3832
-  _DEVLOGINREQ._serialized_start=3835
-  _DEVLOGINREQ._serialized_end=4015
-  _RESETPASSWORDREQ._serialized_start=4018
-  _RESETPASSWORDREQ._serialized_end=4161
-  _RESETPASSWORDRES._serialized_start=4163
-  _RESETPASSWORDRES._serialized_end=4181
-  _LOGINSECRETREQ._serialized_start=4183
-  _LOGINSECRETREQ._serialized_end=4199
-  _LOGINSECRETRES._serialized_start=4201
-  _LOGINSECRETRES._serialized_end=4230
-  _UPDATEPASSWDREQ._serialized_start=4232
-  _UPDATEPASSWDREQ._serialized_end=4319
-  _UPDATEPASSWDRES._serialized_start=4321
-  _UPDATEPASSWDRES._serialized_end=4338
-  _INVITEREQ._serialized_start=4340
-  _INVITEREQ._serialized_end=4400
-  _INVITERES._serialized_start=4402
-  _INVITERES._serialized_end=4413
-  _GETSYNCTIMEREQ._serialized_start=4415
-  _GETSYNCTIMEREQ._serialized_end=4431
-  _GETSYNCTIMERES._serialized_start=4433
-  _GETSYNCTIMERES._serialized_end=4449
-  _REPORTBUYNOBILITYREQ._serialized_start=4451
-  _REPORTBUYNOBILITYREQ._serialized_end=4510
-  _REPORTBUYNOBILITYRES._serialized_start=4512
-  _REPORTBUYNOBILITYRES._serialized_end=4534
-  _GOOGLEIABNOTIFYREQ._serialized_start=4537
-  _GOOGLEIABNOTIFYREQ._serialized_end=4716
-  _GOOGLEIABNOTIFYREQ_BUYINTENT._serialized_start=4658
-  _GOOGLEIABNOTIFYREQ_BUYINTENT._serialized_end=4716
-  _GOOGLEIABNOTIFYRES._serialized_start=4718
-  _GOOGLEIABNOTIFYRES._serialized_end=4738
-  _GOOGLEIABPRODUCTITEM._serialized_start=4740
-  _GOOGLEIABPRODUCTITEM._serialized_end=4817
-  _GOOGLEIABPRODUCTITEMSREQ._serialized_start=4819
-  _GOOGLEIABPRODUCTITEMSREQ._serialized_end=4845
-  _GOOGLEIABPRODUCTITEMSRES._serialized_start=4847
-  _GOOGLEIABPRODUCTITEMSRES._serialized_end=4920
-  _GETWECHATAPPIDREQ._serialized_start=4922
-  _GETWECHATAPPIDREQ._serialized_end=4941
-  _GETWECHATAPPIDRES._serialized_start=4943
-  _GETWECHATAPPIDRES._serialized_end=4978
-  _GETWECHATIDLOGINREQ._serialized_start=4980
-  _GETWECHATIDLOGINREQ._serialized_end=5015
-  _GETWECHATIDLOGINRES._serialized_start=5017
-  _GETWECHATIDLOGINRES._serialized_end=5088
-  _USERINFO._serialized_start=5090
-  _USERINFO._serialized_end=5148
-  _GETMINIPROGRAMLOGINREQ._serialized_start=5151
-  _GETMINIPROGRAMLOGINREQ._serialized_end=5391
-  _MINIPROGRAMPHONEREQ._serialized_start=5393
-  _MINIPROGRAMPHONEREQ._serialized_end=5510
-  _MINIPROGRAMPHONERES._serialized_start=5512
-  _MINIPROGRAMPHONERES._serialized_end=5533
-  _APPLYCERTIFYREQ._serialized_start=5535
-  _APPLYCERTIFYREQ._serialized_end=5628
-  _APPLYCERTIFYRES._serialized_start=5630
-  _APPLYCERTIFYRES._serialized_end=5728
-  _APPLYCERTIFYSIGNREQ._serialized_start=5731
-  _APPLYCERTIFYSIGNREQ._serialized_end=5869
-  _CERTIFYRESULTREQ._serialized_start=5871
-  _CERTIFYRESULTREQ._serialized_end=5889
-  _CERTIFYRESULTRES._serialized_start=5891
-  _CERTIFYRESULTRES._serialized_end=5985
-  _ACCOUNTPHONESMSCODEREQ._serialized_start=5987
-  _ACCOUNTPHONESMSCODEREQ._serialized_end=6011
-  _ACCOUNTPHONESMSCODERES._serialized_start=6013
-  _ACCOUNTPHONESMSCODERES._serialized_end=6037
-  _ACCOUNTSUBSIDIARYLOGINREQ._serialized_start=6040
-  _ACCOUNTSUBSIDIARYLOGINREQ._serialized_end=6238
-  _GETGUESTLOGINREQ._serialized_start=6241
-  _GETGUESTLOGINREQ._serialized_end=6379
-  _ACCOUNTBINDPHONESMSREQ._serialized_start=6381
-  _ACCOUNTBINDPHONESMSREQ._serialized_end=6478
-  _ACCOUNTBINDPHONESMSRES._serialized_start=6480
-  _ACCOUNTBINDPHONESMSRES._serialized_end=6504
-  _ACCOUNTBINDTHIRDREQ._serialized_start=6507
-  _ACCOUNTBINDTHIRDREQ._serialized_end=6648
-  _ACCOUNTBINDTHIRDRES._serialized_start=6650
-  _ACCOUNTBINDTHIRDRES._serialized_end=6671
-  _ACCOUNTBINDLISTREQ._serialized_start=6673
-  _ACCOUNTBINDLISTREQ._serialized_end=6693
-  _ACCOUNTBINDLISTRES._serialized_start=6695
-  _ACCOUNTBINDLISTRES._serialized_end=6785
-  _BINDPHONESMSCODEREQ._serialized_start=6787
-  _BINDPHONESMSCODEREQ._serialized_end=6883
-  _BINDPHONESMSCODERES._serialized_start=6885
-  _BINDPHONESMSCODERES._serialized_end=6906
-  _BINDEMAILSESCODEREQ._serialized_start=6908
-  _BINDEMAILSESCODEREQ._serialized_end=6984
-  _BINDEMAILSESCODERES._serialized_start=6986
-  _BINDEMAILSESCODERES._serialized_end=7007
-  _ACCOUNTBINDEMAILSESREQ._serialized_start=7009
-  _ACCOUNTBINDEMAILSESREQ._serialized_end=7106
-  _ACCOUNTBINDEMAILSESRES._serialized_start=7108
-  _ACCOUNTBINDEMAILSESRES._serialized_end=7132
-  _GETACCOUNTREGISTERREQ._serialized_start=7135
-  _GETACCOUNTREGISTERREQ._serialized_end=7361
-  _GETACCOUNTPASSWORDLOGINREQ._serialized_start=7364
-  _GETACCOUNTPASSWORDLOGINREQ._serialized_end=7543
-  _GETSESCODEREQ._serialized_start=7545
-  _GETSESCODEREQ._serialized_end=7595
-  _GETSESCODERES._serialized_start=7597
-  _GETSESCODERES._serialized_end=7612
-  _GETSESTOKENREQ._serialized_start=7614
-  _GETSESTOKENREQ._serialized_end=7683
-  _GETSESTOKENRES._serialized_start=7685
-  _GETSESTOKENRES._serialized_end=7720
-  _RESETPASSWORDBYSESREQ._serialized_start=7722
-  _RESETPASSWORDBYSESREQ._serialized_end=7831
-  _RESETPASSWORDBYSESRES._serialized_start=7833
-  _RESETPASSWORDBYSESRES._serialized_end=7856
-  _REMOTELOGINSENDCODEREQ._serialized_start=7858
-  _REMOTELOGINSENDCODEREQ._serialized_end=7899
-  _REMOTELOGINSENDCODERES._serialized_start=7901
-  _REMOTELOGINSENDCODERES._serialized_end=7925
-  _REMOTELOGINCONFIRMCODEREQ._serialized_start=7927
-  _REMOTELOGINCONFIRMCODEREQ._serialized_end=7985
-  _REMOTELOGINCONFIRMCODERES._serialized_start=7987
-  _REMOTELOGINCONFIRMCODERES._serialized_end=8054
-  _VERIFYCANCELSIGNINWITHAPPLEREQ._serialized_start=8056
-  _VERIFYCANCELSIGNINWITHAPPLEREQ._serialized_end=8140
-  _VERIFYCANCELSIGNINWITHAPPLERES._serialized_start=8142
-  _VERIFYCANCELSIGNINWITHAPPLERES._serialized_end=8174
-  _WECHATCODELOGINTICKETREQ._serialized_start=8176
-  _WECHATCODELOGINTICKETREQ._serialized_end=8218
-  _WECHATCODELOGINTICKETRES._serialized_start=8220
-  _WECHATCODELOGINTICKETRES._serialized_end=8262
-  _GETWECHATMINICODEREQ._serialized_start=8264
-  _GETWECHATMINICODEREQ._serialized_end=8302
-  _GETWECHATMINICODERES._serialized_start=8304
-  _GETWECHATMINICODERES._serialized_end=8357
-  _GETWECHATMINICODESCANREQ._serialized_start=8359
-  _GETWECHATMINICODESCANREQ._serialized_end=8424
-  _GETWECHATMINICODESCANRES._serialized_start=8426
-  _GETWECHATMINICODESCANRES._serialized_end=8551
-  _REFUSEPHONELICENSEREQ._serialized_start=8553
-  _REFUSEPHONELICENSEREQ._serialized_end=8593
-  _REFUSEPHONELICENSERES._serialized_start=8595
-  _REFUSEPHONELICENSERES._serialized_end=8618
-  _WECHATMINIBINDPHONEREQ._serialized_start=8620
-  _WECHATMINIBINDPHONEREQ._serialized_end=8673
-  _WECHATMINIBINDPHONERES._serialized_start=8675
-  _WECHATMINIBINDPHONERES._serialized_end=8699
-  _THIRDACCOUNTBINDWECHATINFO._serialized_start=8701
-  _THIRDACCOUNTBINDWECHATINFO._serialized_end=8747
-  _THIRDACCOUNTBINDQQINFO._serialized_start=8749
-  _THIRDACCOUNTBINDQQINFO._serialized_end=8791
-  _THIRDACCOUNTBINDINFO._serialized_start=8794
-  _THIRDACCOUNTBINDINFO._serialized_end=8943
-  _THIRDACCOUNTBINDINFODATA._serialized_start=8945
-  _THIRDACCOUNTBINDINFODATA._serialized_end=9068
-  _THIRDACCOUNTBINDINFOREQ._serialized_start=9070
-  _THIRDACCOUNTBINDINFOREQ._serialized_end=9095
-  _THIRDACCOUNTBINDINFORES._serialized_start=9097
-  _THIRDACCOUNTBINDINFORES._serialized_end=9177
-  _BINDTHIRDACCOUNTREQ._serialized_start=9179
-  _BINDTHIRDACCOUNTREQ._serialized_end=9303
-  _BINDTHIRDACCOUNTRES._serialized_start=9305
-  _BINDTHIRDACCOUNTRES._serialized_end=9326
-  _UNBINDTHIRDACCOUNTREQ._serialized_start=9328
-  _UNBINDTHIRDACCOUNTREQ._serialized_end=9424
-  _UNBINDTHIRDACCOUNTRES._serialized_start=9426
-  _UNBINDTHIRDACCOUNTRES._serialized_end=9449
-  _GETQRCODELOGINCODEREQ._serialized_start=9452
-  _GETQRCODELOGINCODEREQ._serialized_end=9614
-  _GETQRCODELOGINCODERES._serialized_start=9616
-  _GETQRCODELOGINCODERES._serialized_end=9659
-  _QRCODESCANLOGINREQ._serialized_start=9661
-  _QRCODESCANLOGINREQ._serialized_end=9758
-  _QRCODESCANLOGINRES._serialized_start=9760
-  _QRCODESCANLOGINRES._serialized_end=9780
-  _GETQRCODELOGINSTATUSREQ._serialized_start=9782
-  _GETQRCODELOGINSTATUSREQ._serialized_end=9872
-  _GETQRCODELOGINSTATUSRES._serialized_start=9875
-  _GETQRCODELOGINSTATUSRES._serialized_end=10043
-  _SETQRCODELOGINSTATUSREQ._serialized_start=10046
-  _SETQRCODELOGINSTATUSREQ._serialized_end=10232
-  _SETQRCODELOGINSTATUSRES._serialized_start=10234
-  _SETQRCODELOGINSTATUSRES._serialized_end=10259
-  _GETACCOUNTREGISTERSTATUSREQ._serialized_start=10261
-  _GETACCOUNTREGISTERSTATUSREQ._serialized_end=10381
-  _GETACCOUNTREGISTERSTATUSRES._serialized_start=10383
-  _GETACCOUNTREGISTERSTATUSRES._serialized_end=10434
-  _GETUMENGPHONEREQ._serialized_start=10436
-  _GETUMENGPHONEREQ._serialized_end=10486
-  _GETUMENGPHONERES._serialized_start=10488
-  _GETUMENGPHONERES._serialized_end=10521
-  _ACCOUNTCROSSTYPEINFO._serialized_start=10523
-  _ACCOUNTCROSSTYPEINFO._serialized_end=10596
-  _ACCOUNTCROSSTYPEINFOREQ._serialized_start=10598
-  _ACCOUNTCROSSTYPEINFOREQ._serialized_end=10623
-  _ACCOUNTCROSSTYPEINFORES._serialized_start=10625
-  _ACCOUNTCROSSTYPEINFORES._serialized_end=10701
-  _APPLYACCOUNTCROSSTYPEREQ._serialized_start=10703
-  _APPLYACCOUNTCROSSTYPEREQ._serialized_end=10729
-  _APPLYACCOUNTCROSSTYPERES._serialized_start=10731
-  _APPLYACCOUNTCROSSTYPERES._serialized_end=10757
-  _CHECKINAPPCHARGELIMITREQ._serialized_start=10759
-  _CHECKINAPPCHARGELIMITREQ._serialized_end=10831
-  _CHECKINAPPCHARGELIMITRES._serialized_start=10833
-  _CHECKINAPPCHARGELIMITRES._serialized_end=10879
-  _GETALIPAYMINIORDERREQ._serialized_start=10882
-  _GETALIPAYMINIORDERREQ._serialized_end=11162
-  _GETALIPAYMINIORDERREQ_EXTENDSENTRY._serialized_start=1365
-  _GETALIPAYMINIORDERREQ_EXTENDSENTRY._serialized_end=1411
-  _GETALIPAYMINIORDERRES._serialized_start=11164
-  _GETALIPAYMINIORDERRES._serialized_end=11205
-  _GETGOODSLISTREQ._serialized_start=11207
-  _GETGOODSLISTREQ._serialized_end=11240
-  _GETGOODSLISTRES._serialized_start=11242
-  _GETGOODSLISTRES._serialized_end=11304
-  _ALIPAYMINIINDEXITEM._serialized_start=11307
-  _ALIPAYMINIINDEXITEM._serialized_end=11489
-  _ALIPAYMINIINDEXBANNER._serialized_start=11491
-  _ALIPAYMINIINDEXBANNER._serialized_end=11534
-  _ALIPAYMINIINDEXGOODSLIST._serialized_start=11536
-  _ALIPAYMINIINDEXGOODSLIST._serialized_end=11618
-  _ALIPAYMINIINDEXGOODSITEM._serialized_start=11621
-  _ALIPAYMINIINDEXGOODSITEM._serialized_end=11794
-  _UAUTHEXTOBJ._serialized_start=13788
-  _UAUTHEXTOBJ._serialized_end=19830
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: uauth_ext.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import enum_type_wrapper
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from mecord import uauth_common_pb2 as uauth__common__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fuauth_ext.proto\x12\x08uauth_pb\x1a\x12uauth_common.proto\"m\n\x0cVerifyIAPReq\x12\x11\n\taccountId\x18\x01 \x01(\x03\x12\x0f\n\x07receipt\x18\x02 \x01(\t\x12\x15\n\rtransactionId\x18\x03 \x01(\t\x12\x10\n\x08order_no\x18\x04 \x01(\t\x12\x10\n\x08goods_id\x18\x05 \x01(\t\"\x0e\n\x0cVerifyIAPRes\"a\n\x08GoldCard\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x05\x12\r\n\x05golds\x18\x03 \x01(\x05\x12\x16\n\x0egiveaway_golds\x18\x04 \x01(\x05\x12\x12\n\nidentifier\x18\x05 \x01(\t\"\x10\n\x0eGetGoodListReq\"H\n\x0eGetGoodListRes\x12%\n\tgood_list\x18\x01 \x03(\x0b\x32\x12.uauth_pb.GoldCard\x12\x0f\n\x07version\x18\x02 \x01(\x05\",\n\x0bOrderIAPReq\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x11\n\taccountId\x18\x02 \x01(\x03\"\x1f\n\x0bOrderIAPRes\x12\x10\n\x08order_no\x18\x01 \x01(\t\"M\n\x10\x43loseOrderIAPReq\x12\x10\n\x08order_no\x18\x01 \x01(\t\x12\'\n\x06status\x18\x02 \x01(\x0e\x32\x17.uauth_pb.IAPStatusType\"\x12\n\x10\x43loseOrderIAPRes\"%\n\x17VIPChargeAccountInfoReq\x12\n\n\x02id\x18\x01 \x01(\x03\"\x8d\x01\n\x17VIPChargeAccountInfoRes\x12\x10\n\x08\x64ue_bank\x18\x01 \x01(\t\x12\r\n\x05payee\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x63\x63ount_number\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65posit_bank\x18\x04 \x01(\t\x12\x10\n\x08nickname\x18\x05 \x01(\t\x12\x11\n\tplayer_id\x18\x06 \x01(\x03\"\x11\n\x0fVIPChargeLogReq\"8\n\x0fVIPChargeLogRes\x12%\n\x04list\x18\x01 \x03(\x0b\x32\x17.uauth_pb.VIPChargeLogs\"C\n\rVIPChargeLogs\x12\x0b\n\x03\x64\x61y\x18\x01 \x01(\t\x12%\n\x04list\x18\x02 \x03(\x0b\x32\x17.uauth_pb.VIPChargeItem\"x\n\rVIPChargeItem\x12\x11\n\tcharge_at\x18\x01 \x01(\x03\x12\x11\n\tfinish_at\x18\x02 \x01(\x03\x12\x0b\n\x03rmb\x18\x03 \x01(\x03\x12\x0c\n\x04gold\x18\x04 \x01(\x03\x12&\n\x06status\x18\x05 \x01(\x0e\x32\x16.uauth_pb.ChargeStatus\"E\n\rReportDataReq\x12&\n\x04type\x18\x01 \x01(\x0e\x32\x18.uauth_pb.ReportDataType\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x0f\n\rReportDataRes\"\xf8\x02\n\x0cGetChargeReq\x12\x10\n\x08order_id\x18\x01 \x01(\t\x12\x12\n\naccount_id\x18\x02 \x01(\x03\x12+\n\x08pay_type\x18\x03 \x01(\x0e\x32\x19.uauth_pb.UPayChannelType\x12\x0c\n\x04gold\x18\x04 \x01(\x03\x12\x0e\n\x06remark\x18\x05 \x01(\t\x12\x34\n\x07\x65xtends\x18\x06 \x03(\x0b\x32#.uauth_pb.GetChargeReq.ExtendsEntry\x12\x39\n\nextra_data\x18\x07 \x03(\x0b\x32%.uauth_pb.GetChargeReq.ExtraDataEntry\x12\x10\n\x08sub_type\x18\x08 \x01(\t\x12\x12\n\nreturn_url\x18\t \x01(\t\x1a.\n\x0c\x45xtendsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x30\n\x0e\x45xtraDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"P\n\x0cGetChargeRes\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65tail\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\t\x12\x14\n\x0credirect_url\x18\x04 \x01(\t\"r\n\rGetSmsCodeReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\x10\n\x08phone_no\x18\x02 \x01(\t\x12\x12\n\nphone_sign\x18\x03 \x01(\t\x12*\n\x0csms_code_tpl\x18\x04 \x01(\x0e\x32\x14.uauth_pb.SMSCodeTpl\"\x0f\n\rGetSmsCodeRes\"\x85\x01\n\x0eGetSmsTokenReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\x10\n\x08phone_no\x18\x02 \x01(\t\x12\x10\n\x08sms_code\x18\x03 \x01(\t\x12\x12\n\nphone_sign\x18\x04 \x01(\t\x12*\n\x0csms_code_tpl\x18\x05 \x01(\x0e\x32\x14.uauth_pb.SMSCodeTpl\"#\n\x0eGetSmsTokenRes\x12\x11\n\tsms_token\x18\x01 \x01(\t\"=\n\x0fPhoneSmsCodeReq\x12*\n\x0csms_code_tpl\x18\x01 \x01(\x0e\x32\x14.uauth_pb.SMSCodeTpl\"\x11\n\x0fPhoneSmsCodeRes\"T\n\x14\x43heckPhoneSmsCodeReq\x12*\n\x0csms_code_tpl\x18\x01 \x01(\x0e\x32\x14.uauth_pb.SMSCodeTpl\x12\x10\n\x08sms_code\x18\x02 \x01(\t\"\x16\n\x14\x43heckPhoneSmsCodeRes\"\xde\x01\n\x0f\x43ommonSignInRes\x12\x13\n\x0blogin_token\x18\x01 \x01(\t\x12\x0e\n\x06is_new\x18\x02 \x01(\x08\x12\x0f\n\x07user_id\x18\x03 \x01(\x12\x12\x37\n\x07\x65xtends\x18\x04 \x03(\x0b\x32&.uauth_pb.CommonSignInRes.ExtendsEntry\x12,\n\nlogin_type\x18\x05 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x1a.\n\x0c\x45xtendsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xce\x01\n\x12SignInWithAppleReq\x12\x16\n\x0eidentity_token\x18\x01 \x01(\t\x12\x1a\n\x12\x61uthorization_code\x18\x02 \x01(\t\x12\x11\n\tfull_name\x18\x03 \x01(\t\x12\x11\n\tdevice_id\x18\x04 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x05 \x01(\t\x12\x13\n\x0byidun_token\x18\x06 \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x07 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\x95\x01\n\x11IdOrPhoneLoginReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x0c\n\x04sign\x18\x04 \x01(\t\x12\x11\n\tdevice_id\x18\x05 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x06 \x01(\t\x12\x13\n\x0byidun_token\x18\x07 \x01(\t\"\xa3\x02\n\x14LoginWithPhoneSMSReq\x12\r\n\x05phone\x18\x01 \x01(\t\x12\x11\n\tsms_token\x18\x02 \x01(\t\x12\x11\n\tdevice_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x05 \x01(\x05\x12\x10\n\x08sms_code\x18\x06 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x08 \x01(\t\x12\x13\n\x0byidun_token\x18\t \x01(\t\x12\x12\n\nphone_sign\x18\n \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x0b \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\x12*\n\x0csms_code_tpl\x18\x0c \x01(\x0e\x32\x14.uauth_pb.SMSCodeTpl\"\xa0\x02\n\rThirdLoginReq\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12\x11\n\tdevice_id\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x05 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x06 \x01(\x05\x12,\n\nlogin_type\x18\x07 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12\x18\n\x10u_meng_device_id\x18\x08 \x01(\t\x12\x13\n\x0byidun_token\x18\t \x01(\t\x12\x14\n\x0ctoken_secret\x18\n \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x0b \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\xd2\x01\n\x18\x43hinaMobileQuickLoginReq\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\x12\x11\n\tdevice_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x05 \x01(\x05\x12\x18\n\x10u_meng_device_id\x18\x06 \x01(\t\x12\x13\n\x0byidun_token\x18\x07 \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x08 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\xc4\x01\n\x13\x43hinaTelecomAuthReq\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12\x11\n\tdevice_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x05 \x01(\x05\x12\x18\n\x10u_meng_device_id\x18\x06 \x01(\t\x12\x13\n\x0byidun_token\x18\x07 \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x08 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\xcd\x01\n\x12UmengQuickLoginReq\x12\x0f\n\x07\x61pp_key\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\x12\x11\n\tdevice_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x05 \x01(\x05\x12\x18\n\x10u_meng_device_id\x18\x08 \x01(\t\x12\x13\n\x0byidun_token\x18\t \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\n \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\xb4\x01\n\x0b\x44\x65vLoginReq\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tdevice_id\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x04 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x05 \x01(\x05\x12\x18\n\x10u_meng_device_id\x18\x06 \x01(\t\x12\x13\n\x0byidun_token\x18\x07 \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x08 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\x8f\x01\n\x10ResetPasswordReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\x10\n\x08phone_no\x18\x02 \x01(\t\x12\x11\n\tsms_token\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x0c\n\x04sign\x18\x05 \x01(\t\x12\x12\n\nphone_sign\x18\x06 \x01(\t\x12\x11\n\tplayer_id\x18\x07 \x01(\x03\"\x12\n\x10ResetPasswordRes\"\x10\n\x0eLoginSecretReq\"\x1d\n\x0eLoginSecretRes\x12\x0b\n\x03key\x18\x01 \x01(\t\"W\n\x0fUpdatePasswdReq\x12\x12\n\nold_passwd\x18\x01 \x01(\t\x12\x12\n\nnew_passwd\x18\x02 \x01(\t\x12\x0c\n\x04sign\x18\x03 \x01(\t\x12\x0e\n\x06is_new\x18\x04 \x01(\x08\"\x11\n\x0fUpdatePasswdRes\"<\n\tInviteReq\x12\x11\n\tplayer_id\x18\x01 \x01(\x03\x12\x0c\n\x04type\x18\x02 \x01(\x05\x12\x0e\n\x06\x65xtend\x18\x03 \x01(\t\"\x0b\n\tInviteRes\"\x10\n\x0eGetSyncTimeReq\"\x10\n\x0eGetSyncTimeRes\";\n\x14ReportBuyNobilityReq\x12\x0f\n\x07room_id\x18\x01 \x01(\x03\x12\x12\n\nbenefit_id\x18\x02 \x01(\x03\"\x16\n\x14ReportBuyNobilityRes\"\xb3\x01\n\x12GoogleIABNotifyReq\x12\x0f\n\x07user_id\x18\x01 \x01(\x03\x12\x14\n\x0cpackage_name\x18\x02 \x01(\t\x12:\n\nbuy_intent\x18\x03 \x01(\x0b\x32&.uauth_pb.GoogleIABNotifyReq.BuyIntent\x1a:\n\tBuyIntent\x12\x15\n\rpurchase_data\x18\x01 \x01(\t\x12\x16\n\x0e\x64\x61ta_signature\x18\x02 \x01(\t\"\x14\n\x12GoogleIABNotifyRes\"M\n\x14GoogleIABProductItem\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05price\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x04 \x01(\t\"\x1a\n\x18GoogleIABProductItemsReq\"I\n\x18GoogleIABProductItemsRes\x12-\n\x05items\x18\x01 \x03(\x0b\x32\x1e.uauth_pb.GoogleIABProductItem\"\x13\n\x11GetWeChatAppIdReq\"#\n\x11GetWeChatAppIdRes\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\"#\n\x13GetWeChatIdLoginReq\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"G\n\x13GetWeChatIdLoginRes\x12\r\n\x05token\x18\x01 \x01(\t\x12\x10\n\x08union_id\x18\x02 \x01(\t\x12\x0f\n\x07open_id\x18\x03 \x01(\t\":\n\x08UserInfo\x12\x10\n\x08nickname\x18\x01 \x01(\t\x12\x0c\n\x04icon\x18\x02 \x01(\t\x12\x0e\n\x06gender\x18\x03 \x01(\x05\"\xf0\x01\n\x16GetMiniProgramLoginReq\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\r\n\x05\x61ppid\x18\x02 \x01(\t\x12,\n\nlogin_type\x18\x03 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12%\n\tuser_info\x18\x04 \x01(\x0b\x32\x12.uauth_pb.UserInfo\x12\x16\n\x0e\x65ncrypted_data\x18\x05 \x01(\t\x12\n\n\x02iv\x18\x06 \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x07 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\x12\x0f\n\x07\x63ode_id\x18\x08 \x01(\t\"u\n\x13MiniProgramPhoneReq\x12\x16\n\x0e\x65ncrypted_data\x18\x01 \x01(\t\x12\n\n\x02iv\x18\x02 \x01(\t\x12,\n\nlogin_type\x18\x03 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12\x0c\n\x04\x63ode\x18\x04 \x01(\t\"\x15\n\x13MiniProgramPhoneRes\"]\n\x0f\x41pplyCertifyReq\x12+\n\x0c\x63\x65rtify_type\x18\x01 \x01(\x0e\x32\x15.uauth_pb.CertifyType\x12\x0f\n\x07id_card\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"b\n\x0f\x41pplyCertifyRes\x12\x0f\n\x07\x66\x61\x63\x65_id\x18\x01 \x01(\t\x12\x10\n\x08trade_no\x18\x02 \x01(\t\x12\r\n\x05nonce\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t\x12\x0c\n\x04sign\x18\x05 \x01(\t\"\x8a\x01\n\x13\x41pplyCertifySignReq\x12+\n\x0c\x63\x65rtify_type\x18\x01 \x01(\x0e\x32\x15.uauth_pb.CertifyType\x12\x0f\n\x07id_card\x18\x02 \x01(\t\x12\x14\n\x0cid_card_sign\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x11\n\tname_sign\x18\x05 \x01(\t\"\x12\n\x10\x43\x65rtifyResultReq\"^\n\x10\x43\x65rtifyResultRes\x12+\n\x0c\x63\x65rtify_type\x18\x01 \x01(\x0e\x32\x15.uauth_pb.CertifyType\x12\x0f\n\x07id_card\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"\x18\n\x16\x41\x63\x63ountPhoneSmsCodeReq\"\x18\n\x16\x41\x63\x63ountPhoneSmsCodeRes\"\xc6\x01\n\x19\x41\x63\x63ountSubsidiaryLoginReq\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\x05\x12\x10\n\x08sms_code\x18\x04 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x05 \x01(\t\x12\x13\n\x0byidun_token\x18\x06 \x01(\t\x12/\n\x0e\x64\x65vice_message\x18\x07 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"\x8a\x01\n\x10GetGuestLoginReq\x12\x11\n\tguest_key\x18\x01 \x01(\t\x12\x0c\n\x04sign\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x03 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x04 \x01(\x05\x12/\n\x0e\x64\x65vice_message\x18\x05 \x01(\x0b\x32\x17.uauth_pb.DeviceMessage\"a\n\x16\x41\x63\x63ountBindPhoneSMSReq\x12\r\n\x05phone\x18\x01 \x01(\t\x12\x10\n\x08sms_code\x18\x02 \x01(\t\x12\x12\n\nverify_old\x18\x03 \x01(\x08\x12\x12\n\nphone_sign\x18\x04 \x01(\t\"\x18\n\x16\x41\x63\x63ountBindPhoneSMSRes\"\x8d\x01\n\x13\x41\x63\x63ountBindThirdReq\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x02 \x01(\t\x12\x0e\n\x06\x61pp_id\x18\x03 \x01(\t\x12,\n\nlogin_type\x18\x04 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12\x14\n\x0ctoken_secret\x18\x05 \x01(\t\"\x15\n\x13\x41\x63\x63ountBindThirdRes\"\x14\n\x12\x41\x63\x63ountBindListReq\"Z\n\x12\x41\x63\x63ountBindListRes\x12&\n\x04list\x18\x01 \x03(\x0e\x32\x18.uauth_pb.UauthLoginType\x12\r\n\x05phone\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\"`\n\x13\x42indPhoneSmsCodeReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\x10\n\x08phone_no\x18\x02 \x01(\t\x12\x12\n\nverify_old\x18\x03 \x01(\x08\x12\x12\n\nphone_sign\x18\x04 \x01(\t\"\x15\n\x13\x42indPhoneSmsCodeRes\"L\n\x13\x42indEmailSesCodeReq\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x12\n\nemail_sign\x18\x02 \x01(\t\x12\x12\n\nverify_old\x18\x03 \x01(\x08\"\x15\n\x13\x42indEmailSesCodeRes\"a\n\x16\x41\x63\x63ountBindEmailSESReq\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x12\n\nemail_sign\x18\x02 \x01(\t\x12\x10\n\x08ses_code\x18\x03 \x01(\t\x12\x12\n\nverify_old\x18\x04 \x01(\x08\"\x18\n\x16\x41\x63\x63ountBindEmailSESRes\"\xe2\x01\n\x15GetAccountRegisterReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65vice_type\x18\x04 \x01(\x05\x12\x10\n\x08nickname\x18\x05 \x01(\t\x12/\n\rregister_type\x18\x06 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12\x0c\n\x04\x63ode\x18\x07 \x01(\t\x12\x0c\n\x04sign\x18\x08 \x01(\t\x12\x12\n\nvalue_sign\x18\t \x01(\t\x12\x0f\n\x07\x63hannel\x18\n \x01(\x05\"\xb3\x01\n\x1aGetAccountPasswordLoginReq\x12\x0f\n\x07\x63ountry\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12,\n\nlogin_type\x18\x04 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12\x13\n\x0b\x64\x65vice_type\x18\x05 \x01(\x05\x12\x0c\n\x04sign\x18\x06 \x01(\t\x12\x12\n\nvalue_sign\x18\x07 \x01(\t\"2\n\rGetSesCodeReq\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x12\n\nemail_sign\x18\x02 \x01(\t\"\x0f\n\rGetSesCodeRes\"E\n\x0eGetSesTokenReq\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x12\n\nemail_sign\x18\x02 \x01(\t\x12\x10\n\x08ses_code\x18\x03 \x01(\t\"#\n\x0eGetSesTokenRes\x12\x11\n\tses_token\x18\x01 \x01(\t\"m\n\x15ResetPasswordBySesReq\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x12\n\nemail_sign\x18\x02 \x01(\t\x12\x11\n\tses_token\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x0c\n\x04sign\x18\x05 \x01(\t\"\x17\n\x15ResetPasswordBySesRes\")\n\x16RemoteLoginSendCodeReq\x12\x0f\n\x07user_id\x18\x01 \x01(\x12\"\x18\n\x16RemoteLoginSendCodeRes\":\n\x19RemoteLoginConfirmCodeReq\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x02 \x01(\x12\"C\n\x19RemoteLoginConfirmCodeRes\x12&\n\x03res\x18\x01 \x01(\x0b\x32\x19.uauth_pb.CommonSignInRes\"T\n\x1eVerifyCancelSignInWithAppleReq\x12\x16\n\x0eidentity_token\x18\x01 \x01(\t\x12\x1a\n\x12\x61uthorization_code\x18\x02 \x01(\t\" \n\x1eVerifyCancelSignInWithAppleRes\"*\n\x18WechatCodeLoginTicketReq\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\"*\n\x18WechatCodeLoginTicketRes\x12\x0e\n\x06ticket\x18\x01 \x01(\t\"&\n\x14GetWechatMiniCodeReq\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\"5\n\x14GetWechatMiniCodeRes\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63ode_id\x18\x02 \x01(\t\"A\n\x18GetWechatMiniCodeScanReq\x12\x0f\n\x07\x63ode_id\x18\x01 \x01(\t\x12\x14\n\x0c\x63ode_id_sign\x18\x02 \x01(\t\"}\n\x18GetWechatMiniCodeScanRes\x12\x32\n\x06status\x18\x01 \x01(\x0e\x32\".uauth_pb.WechatMiniCodeScanStatus\x12-\n\nlogin_data\x18\x02 \x01(\x0b\x32\x19.uauth_pb.CommonSignInRes\"(\n\x15RefusePhoneLicenseReq\x12\x0f\n\x07\x63ode_id\x18\x01 \x01(\t\"\x17\n\x15RefusePhoneLicenseRes\"5\n\x16WechatMiniBindPhoneReq\x12\r\n\x05\x61ppid\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"\x18\n\x16WechatMiniBindPhoneRes\".\n\x1aThirdAccountBindWeChatInfo\x12\x10\n\x08nickname\x18\x01 \x01(\t\"*\n\x16ThirdAccountBindQqInfo\x12\x10\n\x08nickname\x18\x02 \x01(\t\"\x95\x01\n\x14ThirdAccountBindInfo\x12;\n\x0bwechat_info\x18\x01 \x01(\x0b\x32$.uauth_pb.ThirdAccountBindWeChatInfoH\x00\x12\x33\n\x07qq_info\x18\x02 \x01(\x0b\x32 .uauth_pb.ThirdAccountBindQqInfoH\x00\x42\x0b\n\tbind_info\"{\n\x18ThirdAccountBindInfoData\x12\x31\n\tbind_type\x18\x01 \x01(\x0e\x32\x1e.uauth_pb.ThirdAccountBindType\x12,\n\x04info\x18\x02 \x01(\x0b\x32\x1e.uauth_pb.ThirdAccountBindInfo\"\x19\n\x17ThirdAccountBindInfoReq\"P\n\x17ThirdAccountBindInfoRes\x12\x35\n\tinfo_data\x18\x01 \x03(\x0b\x32\".uauth_pb.ThirdAccountBindInfoData\"|\n\x13\x42indThirdAccountReq\x12\x31\n\tbind_type\x18\x01 \x01(\x0e\x32\x1e.uauth_pb.ThirdAccountBindType\x12\x0e\n\x06\x61pp_id\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x04 \x01(\t\"\x15\n\x13\x42indThirdAccountRes\"`\n\x15UnbindThirdAccountReq\x12\x35\n\x08opt_type\x18\x01 \x01(\x0e\x32#.uauth_pb.UnbindThirdAccountOptType\x12\x10\n\x08sms_code\x18\x02 \x01(\t\"\x17\n\x15UnbindThirdAccountRes\"\xa2\x01\n\x15GetQrcodeLoginCodeReq\x12,\n\nlogin_type\x18\x01 \x01(\x0e\x32\x18.uauth_pb.UauthLoginType\x12.\n\x0b\x64\x65vice_type\x18\x02 \x01(\x0e\x32\x19.uauth_pb.UauthDeviceType\x12\x11\n\tdevice_id\x18\x03 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x04 \x01(\t\"+\n\x15GetQrcodeLoginCodeRes\x12\x12\n\nlogin_code\x18\x01 \x01(\t\"a\n\x12QrcodeScanLoginReq\x12\x12\n\nlogin_code\x18\x01 \x01(\t\x12\x17\n\x0flogin_device_id\x18\x02 \x01(\t\x12\x1e\n\x16login_u_meng_device_id\x18\x03 \x01(\t\"\x14\n\x12QrcodeScanLoginRes\"Z\n\x17GetQrcodeLoginStatusReq\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x02 \x01(\t\x12\x12\n\nlogin_code\x18\x03 \x01(\t\"\xa8\x01\n\x17GetQrcodeLoginStatusRes\x12.\n\x06status\x18\x01 \x01(\x0e\x32\x1e.uauth_pb.GetQrcodeLoginStatus\x12\x32\n\x0f\x63ommonSignInRes\x18\x02 \x01(\x0b\x32\x19.uauth_pb.CommonSignInRes\x12\x14\n\x0cuserNickname\x18\x03 \x01(\t\x12\x13\n\x0buserIconUrl\x18\x04 \x01(\t\"\xba\x01\n\x17SetQrcodeLoginStatusReq\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x18\n\x10u_meng_device_id\x18\x02 \x01(\t\x12\x12\n\nlogin_code\x18\x03 \x01(\t\x12\x33\n\x0bloginStatus\x18\x04 \x01(\x0e\x32\x1e.uauth_pb.GetQrcodeLoginStatus\x12\x14\n\x0cuserNickname\x18\x05 \x01(\t\x12\x13\n\x0buserIconUrl\x18\x06 \x01(\t\"\x19\n\x17SetQrcodeLoginStatusRes\"x\n\x1bGetAccountRegisterStatusReq\x12+\n\x04type\x18\x01 \x01(\x0e\x32\x1d.uauth_pb.AccountRegisterType\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04sign\x18\x03 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\x05\"3\n\x1bGetAccountRegisterStatusRes\x12\x14\n\x0cisRegistered\x18\x01 \x01(\x08\"2\n\x10GetUmengPhoneReq\x12\x0f\n\x07\x61pp_key\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"!\n\x10GetUmengPhoneRes\x12\r\n\x05phone\x18\x01 \x01(\t\"I\n\x14\x41\x63\x63ountCrossTypeInfo\x12\x31\n\ncross_type\x18\x01 \x01(\x0e\x32\x1d.uauth_pb.AccountAppCrossType\"\x19\n\x17\x41\x63\x63ountCrossTypeInfoReq\"L\n\x17\x41\x63\x63ountCrossTypeInfoRes\x12\x31\n\tinfo_list\x18\x01 \x03(\x0b\x32\x1e.uauth_pb.AccountCrossTypeInfo\"\x1a\n\x18\x41pplyAccountCrossTypeReq\"\x1a\n\x18\x41pplyAccountCrossTypeRes\"H\n\x18\x43heckInAppChargeLimitReq\x12,\n\x0b\x63harge_type\x18\x01 \x01(\x0e\x32\x17.uauth_pb.AppChargeType\".\n\x18\x43heckInAppChargeLimitRes\x12\x12\n\ncan_charge\x18\x01 \x01(\x08\"\x98\x02\n\x15GetAlipayMiniOrderReq\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\x12\x12\n\naccount_id\x18\x02 \x01(\x03\x12+\n\x08pay_type\x18\x03 \x01(\x0e\x32\x19.uauth_pb.UPayChannelType\x12\x0c\n\x04gold\x18\x04 \x01(\x03\x12\x0b\n\x03num\x18\x05 \x01(\x05\x12\x10\n\x08store_id\x18\x06 \x01(\x05\x12\x12\n\nreturn_url\x18\x07 \x01(\t\x12=\n\x07\x65xtends\x18\x08 \x03(\x0b\x32,.uauth_pb.GetAlipayMiniOrderReq.ExtendsEntry\x1a.\n\x0c\x45xtendsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\")\n\x15GetAlipayMiniOrderRes\x12\x10\n\x08trade_no\x18\x01 \x01(\t\"!\n\x0fGetGoodsListReq\x12\x0e\n\x06\x61pp_id\x18\x01 \x01(\t\">\n\x0fGetGoodsListRes\x12+\n\x04list\x18\x01 \x03(\x0b\x32\x1d.uauth_pb.AlipayMiniIndexItem\"\xb6\x01\n\x13\x41lipayMiniIndexItem\x12\x30\n\tdata_type\x18\x01 \x01(\x0e\x32\x1d.uauth_pb.AlipayMiniIndexType\x12\x31\n\x06\x62\x61nner\x18\x02 \x01(\x0b\x32\x1f.uauth_pb.AlipayMiniIndexBannerH\x00\x12\x32\n\x04list\x18\x03 \x01(\x0b\x32\".uauth_pb.AlipayMiniIndexGoodsListH\x00\x42\x06\n\x04\x64\x61ta\"+\n\x15\x41lipayMiniIndexBanner\x12\x12\n\nbanner_url\x18\x01 \x01(\t\"R\n\x18\x41lipayMiniIndexGoodsList\x12\x36\n\ngoods_list\x18\x01 \x03(\x0b\x32\".uauth_pb.AlipayMiniIndexGoodsItem\"\xad\x01\n\x18\x41lipayMiniIndexGoodsItem\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07img_url\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x65sc\x18\x04 \x01(\t\x12\r\n\x05price\x18\x05 \x01(\t\x12\x31\n\ngoods_type\x18\x06 \x01(\x0e\x32\x1d.uauth_pb.AlipayMiniGoodsType\x12\x0e\n\x04gold\x18\x07 \x01(\x03H\x00\x42\x06\n\x04\x64\x61ta*\x86\x07\n\x0e\x45rrorUAuthCode\x12\x13\n\x0f\x45rrorUAuth_Zero\x10\x00\x12\x1d\n\x17\x45rrorUAuthRegisterParam\x10\xd9\xb0\x02\x12\x1c\n\x16\x45rrorUAuthAccountExist\x10\xda\xb0\x02\x12\x1e\n\x18\x45rrorUAuthSessionTimeOut\x10\xdb\xb0\x02\x12\x1f\n\x19\x45rrorUAuthSessionNotFound\x10\xdc\xb0\x02\x12\x1c\n\x16\x45rrorUAuthUserNotFound\x10\xdd\xb0\x02\x12\x1f\n\x19\x45rrorUAuthAccountNotExist\x10\xde\xb0\x02\x12!\n\x1b\x45rrorUAuthPassWordNoCorrect\x10\xdf\xb0\x02\x12\x1d\n\x17\x45rrorUAuthCodeIncorrect\x10\xe0\xb0\x02\x12\x1d\n\x17\x45rrorUAuthPhoneNotExist\x10\xe1\xb0\x02\x12\x1b\n\x15\x45rrorUAuthUserNoRight\x10\xe2\xb0\x02\x12\x1a\n\x14\x45rrorUAuthInvalidWay\x10\xe3\xb0\x02\x12\x19\n\x13\x45rrorUAuthNeedLogin\x10\xe4\xb0\x02\x12\x18\n\x12\x45rrorUAuthGetToken\x10\xe5\xb0\x02\x12\x1b\n\x15\x45rrorUAuthAccessToken\x10\xe6\xb0\x02\x12\x1d\n\x17\x45rrorUAuthWrongPhoneNum\x10\xe7\xb0\x02\x12\x1d\n\x17\x45rrorUAuthServerOffLine\x10\xe8\xb0\x02\x12!\n\x1b\x45rrorUAuthPhoneAlreadyExist\x10\xe9\xb0\x02\x12\x18\n\x12\x45rrorIAPHasNoOrder\x10\xaa\xcb\x0e\x12\x18\n\x12\x45rrorCheckIAPOrder\x10\xab\xcb\x0e\x12\x1b\n\x15\x45rrorCheckIAPBundleID\x10\xac\xcb\x0e\x12\x16\n\x10\x45rrorTooFrequent\x10\xb6\xcb\x0e\x12\x0e\n\x08\x45rror3rd\x10\xb7\xcb\x0e\x12\x1a\n\x14\x45rrorPasswordInvalid\x10\xb8\xcb\x0e\x12\x1b\n\x15\x45rrorWrongOldPassword\x10\xb9\xcb\x0e\x12\x15\n\x0f\x45rrorLoginBlack\x10\xba\xcb\x0e\x12\x15\n\x0f\x45rrorHasAccount\x10\xbb\xcb\x0e\x12\x1c\n\x16\x45rrorUAuthPswNoCorrect\x10\xbc\xcb\x0e\x12\x1e\n\x18\x45rrorUAuthPhoneNoCorrect\x10\xbd\xcb\x0e\x12\x19\n\x13\x45rrorUserLimitLogin\x10\xd2\xcb\x0e\x12\x1c\n\x16\x45rrorRefusePhoneLicens\x10\xd4\xcb\x0e*I\n\rIAPStatusType\x12\x0c\n\x08IAP_NONE\x10\x00\x12\x13\n\x0fIAP_STATUS_FAIL\x10\x01\x12\x15\n\x11IAP_STATUS_CANCEL\x10\x02*=\n\x0c\x43hargeStatus\x12\x0f\n\x0b\x43S_CHARGING\x10\x00\x12\r\n\tCS_FINISH\x10\x01\x12\r\n\tCS_REFUND\x10\x02*9\n\x0eReportDataType\x12\x0c\n\x08RDT_Null\x10\x00\x12\x19\n\x15RDT_CMB_VIP_Expedited\x10\x01*R\n\nVerifyType\x12\x0b\n\x07VT_NULL\x10\x00\x12\x12\n\x0eVT_RemoteLogin\x10\x01\x12\x0e\n\nVT_Protect\x10\x02\x12\x13\n\x0fVT_AnomalyLogin\x10\x03*k\n\nSMSCodeTpl\x12\x13\n\x0fSMSCodeTpl_Zero\x10\x00\x12\x14\n\x10SMSCodeTpl_Login\x10\x01\x12\x17\n\x13SMSCodeTpl_ResetPwd\x10\x02\x12\x19\n\x15SMSCodeTpl_VerifyCode\x10\x03*)\n\x0b\x43\x65rtifyType\x12\x0b\n\x07\x43T_None\x10\x00\x12\r\n\tCT_IdCard\x10\x01*\x82\x01\n\x18WechatMiniCodeScanStatus\x12\x10\n\x0cWMCSS_NoScan\x10\x00\x12\x11\n\rWMCSS_Timeout\x10\x01\x12\x10\n\x0cWMCSS_ScanIn\x10\x02\x12\x11\n\rWMCSS_ScanEnd\x10\x03\x12\x1c\n\x18WMCSS_RefusePhoneLicense\x10\x04*C\n\x14ThirdAccountBindType\x12\r\n\tTABT_NONE\x10\x00\x12\x0f\n\x0bTABT_WEIXIN\x10\x01\x12\x0b\n\x07TABT_QQ\x10\x02*=\n\x19UnbindThirdAccountOptType\x12\x0e\n\nUTAOT_Send\x10\x00\x12\x10\n\x0cUTAOT_Verify\x10\x01*S\n\x14GetQrcodeLoginStatus\x12\x08\n\x04NONE\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\x0b\n\x07SUCCESS\x10\x02\x12\x0b\n\x07\x45XPIRED\x10\x03\x12\n\n\x06\x43\x41NCEL\x10\x04*>\n\x13\x41\x63\x63ountRegisterType\x12\x0b\n\x07RT_NONE\x10\x00\x12\x0c\n\x08RT_PHONE\x10\x01\x12\x0c\n\x08RT_EMAIL\x10\x02*3\n\x13\x41\x63\x63ountAppCrossType\x12\r\n\tAACT_None\x10\x00\x12\r\n\tAACT_Neon\x10\x01*<\n\rAppChargeType\x12\x0c\n\x08\x41\x43T_None\x10\x00\x12\r\n\tACT_Apple\x10\x01\x12\x0e\n\nACT_Google\x10\x02*E\n\x13\x41lipayMiniIndexType\x12\r\n\tAMIT_NONE\x10\x00\x12\x0f\n\x0b\x41MIT_BANNER\x10\x01\x12\x0e\n\nAMIT_GOODS\x10\x02*3\n\x13\x41lipayMiniGoodsType\x12\r\n\tAMGT_NONE\x10\x00\x12\r\n\tAMGT_GOLD\x10\x01\x32\x9a/\n\x0bUauthExtObj\x12;\n\tVerifyIAP\x12\x16.uauth_pb.VerifyIAPReq\x1a\x16.uauth_pb.VerifyIAPRes\x12\x41\n\x0bGetGoodList\x12\x18.uauth_pb.GetGoodListReq\x1a\x18.uauth_pb.GetGoodListRes\x12\x38\n\x08OrderIAP\x12\x15.uauth_pb.OrderIAPReq\x1a\x15.uauth_pb.OrderIAPRes\x12G\n\rCloseOrderIAP\x12\x1a.uauth_pb.CloseOrderIAPReq\x1a\x1a.uauth_pb.CloseOrderIAPRes\x12_\n\x17GetVIPChargeAccountInfo\x12!.uauth_pb.VIPChargeAccountInfoReq\x1a!.uauth_pb.VIPChargeAccountInfoRes\x12\x44\n\x0cVIPChargeLog\x12\x19.uauth_pb.VIPChargeLogReq\x1a\x19.uauth_pb.VIPChargeLogRes\x12>\n\nReportData\x12\x17.uauth_pb.ReportDataReq\x1a\x17.uauth_pb.ReportDataRes\x12;\n\tGetCharge\x12\x16.uauth_pb.GetChargeReq\x1a\x16.uauth_pb.GetChargeRes\x12M\n\x12GetSignInWithApple\x12\x1c.uauth_pb.SignInWithAppleReq\x1a\x19.uauth_pb.CommonSignInRes\x12>\n\nGetSmsCode\x12\x17.uauth_pb.GetSmsCodeReq\x1a\x17.uauth_pb.GetSmsCodeRes\x12\x44\n\x10GetSmsCodeBySign\x12\x17.uauth_pb.GetSmsCodeReq\x1a\x17.uauth_pb.GetSmsCodeRes\x12\x41\n\x0bGetSmsToken\x12\x18.uauth_pb.GetSmsTokenReq\x1a\x18.uauth_pb.GetSmsTokenRes\x12G\n\x11GetSmsTokenBySign\x12\x18.uauth_pb.GetSmsTokenReq\x1a\x18.uauth_pb.GetSmsTokenRes\x12?\n\x0bGetDevLogin\x12\x15.uauth_pb.DevLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12K\n\x11GetIdOrPhoneLogin\x12\x1b.uauth_pb.IdOrPhoneLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12\x43\n\rGetThirdLogin\x12\x17.uauth_pb.ThirdLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12Q\n\x14GetLoginWithPhoneSMS\x12\x1e.uauth_pb.LoginWithPhoneSMSReq\x1a\x19.uauth_pb.CommonSignInRes\x12W\n\x1aGetLoginWithPhoneSMSBySign\x12\x1e.uauth_pb.LoginWithPhoneSMSReq\x1a\x19.uauth_pb.CommonSignInRes\x12Y\n\x18GetChinaMobileQuickLogin\x12\".uauth_pb.ChinaMobileQuickLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12O\n\x13GetChinaTelecomAuth\x12\x1d.uauth_pb.ChinaTelecomAuthReq\x1a\x19.uauth_pb.CommonSignInRes\x12M\n\x12GetUmengQuickLogin\x12\x1c.uauth_pb.UmengQuickLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12J\n\x10GetResetPassword\x12\x1a.uauth_pb.ResetPasswordReq\x1a\x1a.uauth_pb.ResetPasswordRes\x12P\n\x16GetResetPasswordBySign\x12\x1a.uauth_pb.ResetPasswordReq\x1a\x1a.uauth_pb.ResetPasswordRes\x12\x44\n\x0cUpdatePasswd\x12\x19.uauth_pb.UpdatePasswdReq\x1a\x19.uauth_pb.UpdatePasswdRes\x12\x35\n\tGetInvite\x12\x13.uauth_pb.InviteReq\x1a\x13.uauth_pb.InviteRes\x12\x41\n\x0bGetSyncTime\x12\x18.uauth_pb.GetSyncTimeReq\x1a\x18.uauth_pb.GetSyncTimeRes\x12S\n\x11ReportBuyNobility\x12\x1e.uauth_pb.ReportBuyNobilityReq\x1a\x1e.uauth_pb.ReportBuyNobilityRes\x12J\n\x0eGetWeChatAppId\x12\x1b.uauth_pb.GetWeChatAppIdReq\x1a\x1b.uauth_pb.GetWeChatAppIdRes\x12P\n\x10GetWeChatIdLogin\x12\x1d.uauth_pb.GetWeChatIdLoginReq\x1a\x1d.uauth_pb.GetWeChatIdLoginRes\x12\x61\n\x15GoogleIABProductItems\x12\".uauth_pb.GoogleIABProductItemsReq\x1a\".uauth_pb.GoogleIABProductItemsRes\"\x00\x12O\n\x0fGoogleIABNotify\x12\x1c.uauth_pb.GoogleIABNotifyReq\x1a\x1c.uauth_pb.GoogleIABNotifyRes\"\x00\x12R\n\x13GetMiniProgramLogin\x12 .uauth_pb.GetMiniProgramLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12P\n\x10MiniProgramPhone\x12\x1d.uauth_pb.MiniProgramPhoneReq\x1a\x1d.uauth_pb.MiniProgramPhoneRes\x12\x44\n\x0c\x41pplyCertify\x12\x19.uauth_pb.ApplyCertifyReq\x1a\x19.uauth_pb.ApplyCertifyRes\x12L\n\x10\x41pplyCertifySign\x12\x1d.uauth_pb.ApplyCertifySignReq\x1a\x19.uauth_pb.ApplyCertifyRes\x12G\n\rCertifyResult\x12\x1a.uauth_pb.CertifyResultReq\x1a\x1a.uauth_pb.CertifyResultRes\x12Y\n\x13\x41\x63\x63ountPhoneSmsCode\x12 .uauth_pb.AccountPhoneSmsCodeReq\x1a .uauth_pb.AccountPhoneSmsCodeRes\x12X\n\x16\x41\x63\x63ountSubsidiaryLogin\x12#.uauth_pb.AccountSubsidiaryLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12\x46\n\rGetGuestLogin\x12\x1a.uauth_pb.GetGuestLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12P\n\x10\x42indPhoneSmsCode\x12\x1d.uauth_pb.BindPhoneSmsCodeReq\x1a\x1d.uauth_pb.BindPhoneSmsCodeRes\x12Y\n\x13\x41\x63\x63ountBindPhoneSMS\x12 .uauth_pb.AccountBindPhoneSMSReq\x1a .uauth_pb.AccountBindPhoneSMSRes\x12P\n\x10\x41\x63\x63ountBindThird\x12\x1d.uauth_pb.AccountBindThirdReq\x1a\x1d.uauth_pb.AccountBindThirdRes\x12M\n\x0f\x41\x63\x63ountBindList\x12\x1c.uauth_pb.AccountBindListReq\x1a\x1c.uauth_pb.AccountBindListRes\x12P\n\x10\x42indEmailSesCode\x12\x1d.uauth_pb.BindEmailSesCodeReq\x1a\x1d.uauth_pb.BindEmailSesCodeRes\x12Y\n\x13\x41\x63\x63ountBindEmailSES\x12 .uauth_pb.AccountBindEmailSESReq\x1a .uauth_pb.AccountBindEmailSESRes\x12P\n\x12GetAccountRegister\x12\x1f.uauth_pb.GetAccountRegisterReq\x1a\x19.uauth_pb.CommonSignInRes\x12Z\n\x17GetAccountPasswordLogin\x12$.uauth_pb.GetAccountPasswordLoginReq\x1a\x19.uauth_pb.CommonSignInRes\x12>\n\nGetSesCode\x12\x17.uauth_pb.GetSesCodeReq\x1a\x17.uauth_pb.GetSesCodeRes\x12\x41\n\x0bGetSesToken\x12\x18.uauth_pb.GetSesTokenReq\x1a\x18.uauth_pb.GetSesTokenRes\x12Y\n\x15GetResetPasswordBySes\x12\x1f.uauth_pb.ResetPasswordBySesReq\x1a\x1f.uauth_pb.ResetPasswordBySesRes\x12\\\n\x16GetRemoteLoginSendCode\x12 .uauth_pb.RemoteLoginSendCodeReq\x1a .uauth_pb.RemoteLoginSendCodeRes\x12\x65\n\x19GetRemoteLoginConfirmCode\x12#.uauth_pb.RemoteLoginConfirmCodeReq\x1a#.uauth_pb.RemoteLoginConfirmCodeRes\x12q\n\x1bVerifyCancelSignInWithApple\x12(.uauth_pb.VerifyCancelSignInWithAppleReq\x1a(.uauth_pb.VerifyCancelSignInWithAppleRes\x12\x44\n\x0cPhoneSmsCode\x12\x19.uauth_pb.PhoneSmsCodeReq\x1a\x19.uauth_pb.PhoneSmsCodeRes\x12S\n\x11\x43heckPhoneSmsCode\x12\x1e.uauth_pb.CheckPhoneSmsCodeReq\x1a\x1e.uauth_pb.CheckPhoneSmsCodeRes\x12\x62\n\x18GetWechatCodeLoginTicket\x12\".uauth_pb.WechatCodeLoginTicketReq\x1a\".uauth_pb.WechatCodeLoginTicketRes\x12S\n\x11GetWechatMiniCode\x12\x1e.uauth_pb.GetWechatMiniCodeReq\x1a\x1e.uauth_pb.GetWechatMiniCodeRes\x12_\n\x15GetWechatMiniCodeScan\x12\".uauth_pb.GetWechatMiniCodeScanReq\x1a\".uauth_pb.GetWechatMiniCodeScanRes\x12Y\n\x15GetRefusePhoneLicense\x12\x1f.uauth_pb.RefusePhoneLicenseReq\x1a\x1f.uauth_pb.RefusePhoneLicenseRes\x12Y\n\x13WechatMiniBindPhone\x12 .uauth_pb.WechatMiniBindPhoneReq\x1a .uauth_pb.WechatMiniBindPhoneRes\x12\\\n\x14ThirdAccountBindInfo\x12!.uauth_pb.ThirdAccountBindInfoReq\x1a!.uauth_pb.ThirdAccountBindInfoRes\x12P\n\x10\x42indThirdAccount\x12\x1d.uauth_pb.BindThirdAccountReq\x1a\x1d.uauth_pb.BindThirdAccountRes\x12V\n\x12UnbindThirdAccount\x12\x1f.uauth_pb.UnbindThirdAccountReq\x1a\x1f.uauth_pb.UnbindThirdAccountRes\x12V\n\x12GetQrcodeLoginCode\x12\x1f.uauth_pb.GetQrcodeLoginCodeReq\x1a\x1f.uauth_pb.GetQrcodeLoginCodeRes\x12\\\n\x14GetQrcodeLoginStatus\x12!.uauth_pb.GetQrcodeLoginStatusReq\x1a!.uauth_pb.GetQrcodeLoginStatusRes\x12\\\n\x14SetQrcodeLoginStatus\x12!.uauth_pb.SetQrcodeLoginStatusReq\x1a!.uauth_pb.SetQrcodeLoginStatusRes\x12M\n\x0fQrcodeScanLogin\x12\x1c.uauth_pb.QrcodeScanLoginReq\x1a\x1c.uauth_pb.QrcodeScanLoginRes\x12h\n\x18GetAccountRegisterStatus\x12%.uauth_pb.GetAccountRegisterStatusReq\x1a%.uauth_pb.GetAccountRegisterStatusRes\x12G\n\rGetUmengPhone\x12\x1a.uauth_pb.GetUmengPhoneReq\x1a\x1a.uauth_pb.GetUmengPhoneRes\x12\\\n\x14\x41\x63\x63ountCrossTypeInfo\x12!.uauth_pb.AccountCrossTypeInfoReq\x1a!.uauth_pb.AccountCrossTypeInfoRes\x12_\n\x15\x41pplyAccountCrossType\x12\".uauth_pb.ApplyAccountCrossTypeReq\x1a\".uauth_pb.ApplyAccountCrossTypeRes\x12_\n\x15\x43heckInAppChargeLimit\x12\".uauth_pb.CheckInAppChargeLimitReq\x1a\".uauth_pb.CheckInAppChargeLimitRes\x12V\n\x12GetAlipayMiniOrder\x12\x1f.uauth_pb.GetAlipayMiniOrderReq\x1a\x1f.uauth_pb.GetAlipayMiniOrderRes\x12\x44\n\x0cGetGoodsList\x12\x19.uauth_pb.GetGoodsListReq\x1a\x19.uauth_pb.GetGoodsListResB\x08\xa2\x02\x05PROTOb\x06proto3')
+
+_ERRORUAUTHCODE = DESCRIPTOR.enum_types_by_name['ErrorUAuthCode']
+ErrorUAuthCode = enum_type_wrapper.EnumTypeWrapper(_ERRORUAUTHCODE)
+_IAPSTATUSTYPE = DESCRIPTOR.enum_types_by_name['IAPStatusType']
+IAPStatusType = enum_type_wrapper.EnumTypeWrapper(_IAPSTATUSTYPE)
+_CHARGESTATUS = DESCRIPTOR.enum_types_by_name['ChargeStatus']
+ChargeStatus = enum_type_wrapper.EnumTypeWrapper(_CHARGESTATUS)
+_REPORTDATATYPE = DESCRIPTOR.enum_types_by_name['ReportDataType']
+ReportDataType = enum_type_wrapper.EnumTypeWrapper(_REPORTDATATYPE)
+_VERIFYTYPE = DESCRIPTOR.enum_types_by_name['VerifyType']
+VerifyType = enum_type_wrapper.EnumTypeWrapper(_VERIFYTYPE)
+_SMSCODETPL = DESCRIPTOR.enum_types_by_name['SMSCodeTpl']
+SMSCodeTpl = enum_type_wrapper.EnumTypeWrapper(_SMSCODETPL)
+_CERTIFYTYPE = DESCRIPTOR.enum_types_by_name['CertifyType']
+CertifyType = enum_type_wrapper.EnumTypeWrapper(_CERTIFYTYPE)
+_WECHATMINICODESCANSTATUS = DESCRIPTOR.enum_types_by_name['WechatMiniCodeScanStatus']
+WechatMiniCodeScanStatus = enum_type_wrapper.EnumTypeWrapper(_WECHATMINICODESCANSTATUS)
+_THIRDACCOUNTBINDTYPE = DESCRIPTOR.enum_types_by_name['ThirdAccountBindType']
+ThirdAccountBindType = enum_type_wrapper.EnumTypeWrapper(_THIRDACCOUNTBINDTYPE)
+_UNBINDTHIRDACCOUNTOPTTYPE = DESCRIPTOR.enum_types_by_name['UnbindThirdAccountOptType']
+UnbindThirdAccountOptType = enum_type_wrapper.EnumTypeWrapper(_UNBINDTHIRDACCOUNTOPTTYPE)
+_GETQRCODELOGINSTATUS = DESCRIPTOR.enum_types_by_name['GetQrcodeLoginStatus']
+GetQrcodeLoginStatus = enum_type_wrapper.EnumTypeWrapper(_GETQRCODELOGINSTATUS)
+_ACCOUNTREGISTERTYPE = DESCRIPTOR.enum_types_by_name['AccountRegisterType']
+AccountRegisterType = enum_type_wrapper.EnumTypeWrapper(_ACCOUNTREGISTERTYPE)
+_ACCOUNTAPPCROSSTYPE = DESCRIPTOR.enum_types_by_name['AccountAppCrossType']
+AccountAppCrossType = enum_type_wrapper.EnumTypeWrapper(_ACCOUNTAPPCROSSTYPE)
+_APPCHARGETYPE = DESCRIPTOR.enum_types_by_name['AppChargeType']
+AppChargeType = enum_type_wrapper.EnumTypeWrapper(_APPCHARGETYPE)
+_ALIPAYMINIINDEXTYPE = DESCRIPTOR.enum_types_by_name['AlipayMiniIndexType']
+AlipayMiniIndexType = enum_type_wrapper.EnumTypeWrapper(_ALIPAYMINIINDEXTYPE)
+_ALIPAYMINIGOODSTYPE = DESCRIPTOR.enum_types_by_name['AlipayMiniGoodsType']
+AlipayMiniGoodsType = enum_type_wrapper.EnumTypeWrapper(_ALIPAYMINIGOODSTYPE)
+ErrorUAuth_Zero = 0
+ErrorUAuthRegisterParam = 39001
+ErrorUAuthAccountExist = 39002
+ErrorUAuthSessionTimeOut = 39003
+ErrorUAuthSessionNotFound = 39004
+ErrorUAuthUserNotFound = 39005
+ErrorUAuthAccountNotExist = 39006
+ErrorUAuthPassWordNoCorrect = 39007
+ErrorUAuthCodeIncorrect = 39008
+ErrorUAuthPhoneNotExist = 39009
+ErrorUAuthUserNoRight = 39010
+ErrorUAuthInvalidWay = 39011
+ErrorUAuthNeedLogin = 39012
+ErrorUAuthGetToken = 39013
+ErrorUAuthAccessToken = 39014
+ErrorUAuthWrongPhoneNum = 39015
+ErrorUAuthServerOffLine = 39016
+ErrorUAuthPhoneAlreadyExist = 39017
+ErrorIAPHasNoOrder = 239018
+ErrorCheckIAPOrder = 239019
+ErrorCheckIAPBundleID = 239020
+ErrorTooFrequent = 239030
+Error3rd = 239031
+ErrorPasswordInvalid = 239032
+ErrorWrongOldPassword = 239033
+ErrorLoginBlack = 239034
+ErrorHasAccount = 239035
+ErrorUAuthPswNoCorrect = 239036
+ErrorUAuthPhoneNoCorrect = 239037
+ErrorUserLimitLogin = 239058
+ErrorRefusePhoneLicens = 239060
+IAP_NONE = 0
+IAP_STATUS_FAIL = 1
+IAP_STATUS_CANCEL = 2
+CS_CHARGING = 0
+CS_FINISH = 1
+CS_REFUND = 2
+RDT_Null = 0
+RDT_CMB_VIP_Expedited = 1
+VT_NULL = 0
+VT_RemoteLogin = 1
+VT_Protect = 2
+VT_AnomalyLogin = 3
+SMSCodeTpl_Zero = 0
+SMSCodeTpl_Login = 1
+SMSCodeTpl_ResetPwd = 2
+SMSCodeTpl_VerifyCode = 3
+CT_None = 0
+CT_IdCard = 1
+WMCSS_NoScan = 0
+WMCSS_Timeout = 1
+WMCSS_ScanIn = 2
+WMCSS_ScanEnd = 3
+WMCSS_RefusePhoneLicense = 4
+TABT_NONE = 0
+TABT_WEIXIN = 1
+TABT_QQ = 2
+UTAOT_Send = 0
+UTAOT_Verify = 1
+NONE = 0
+PENDING = 1
+SUCCESS = 2
+EXPIRED = 3
+CANCEL = 4
+RT_NONE = 0
+RT_PHONE = 1
+RT_EMAIL = 2
+AACT_None = 0
+AACT_Neon = 1
+ACT_None = 0
+ACT_Apple = 1
+ACT_Google = 2
+AMIT_NONE = 0
+AMIT_BANNER = 1
+AMIT_GOODS = 2
+AMGT_NONE = 0
+AMGT_GOLD = 1
+
+
+_VERIFYIAPREQ = DESCRIPTOR.message_types_by_name['VerifyIAPReq']
+_VERIFYIAPRES = DESCRIPTOR.message_types_by_name['VerifyIAPRes']
+_GOLDCARD = DESCRIPTOR.message_types_by_name['GoldCard']
+_GETGOODLISTREQ = DESCRIPTOR.message_types_by_name['GetGoodListReq']
+_GETGOODLISTRES = DESCRIPTOR.message_types_by_name['GetGoodListRes']
+_ORDERIAPREQ = DESCRIPTOR.message_types_by_name['OrderIAPReq']
+_ORDERIAPRES = DESCRIPTOR.message_types_by_name['OrderIAPRes']
+_CLOSEORDERIAPREQ = DESCRIPTOR.message_types_by_name['CloseOrderIAPReq']
+_CLOSEORDERIAPRES = DESCRIPTOR.message_types_by_name['CloseOrderIAPRes']
+_VIPCHARGEACCOUNTINFOREQ = DESCRIPTOR.message_types_by_name['VIPChargeAccountInfoReq']
+_VIPCHARGEACCOUNTINFORES = DESCRIPTOR.message_types_by_name['VIPChargeAccountInfoRes']
+_VIPCHARGELOGREQ = DESCRIPTOR.message_types_by_name['VIPChargeLogReq']
+_VIPCHARGELOGRES = DESCRIPTOR.message_types_by_name['VIPChargeLogRes']
+_VIPCHARGELOGS = DESCRIPTOR.message_types_by_name['VIPChargeLogs']
+_VIPCHARGEITEM = DESCRIPTOR.message_types_by_name['VIPChargeItem']
+_REPORTDATAREQ = DESCRIPTOR.message_types_by_name['ReportDataReq']
+_REPORTDATARES = DESCRIPTOR.message_types_by_name['ReportDataRes']
+_GETCHARGEREQ = DESCRIPTOR.message_types_by_name['GetChargeReq']
+_GETCHARGEREQ_EXTENDSENTRY = _GETCHARGEREQ.nested_types_by_name['ExtendsEntry']
+_GETCHARGEREQ_EXTRADATAENTRY = _GETCHARGEREQ.nested_types_by_name['ExtraDataEntry']
+_GETCHARGERES = DESCRIPTOR.message_types_by_name['GetChargeRes']
+_GETSMSCODEREQ = DESCRIPTOR.message_types_by_name['GetSmsCodeReq']
+_GETSMSCODERES = DESCRIPTOR.message_types_by_name['GetSmsCodeRes']
+_GETSMSTOKENREQ = DESCRIPTOR.message_types_by_name['GetSmsTokenReq']
+_GETSMSTOKENRES = DESCRIPTOR.message_types_by_name['GetSmsTokenRes']
+_PHONESMSCODEREQ = DESCRIPTOR.message_types_by_name['PhoneSmsCodeReq']
+_PHONESMSCODERES = DESCRIPTOR.message_types_by_name['PhoneSmsCodeRes']
+_CHECKPHONESMSCODEREQ = DESCRIPTOR.message_types_by_name['CheckPhoneSmsCodeReq']
+_CHECKPHONESMSCODERES = DESCRIPTOR.message_types_by_name['CheckPhoneSmsCodeRes']
+_COMMONSIGNINRES = DESCRIPTOR.message_types_by_name['CommonSignInRes']
+_COMMONSIGNINRES_EXTENDSENTRY = _COMMONSIGNINRES.nested_types_by_name['ExtendsEntry']
+_SIGNINWITHAPPLEREQ = DESCRIPTOR.message_types_by_name['SignInWithAppleReq']
+_IDORPHONELOGINREQ = DESCRIPTOR.message_types_by_name['IdOrPhoneLoginReq']
+_LOGINWITHPHONESMSREQ = DESCRIPTOR.message_types_by_name['LoginWithPhoneSMSReq']
+_THIRDLOGINREQ = DESCRIPTOR.message_types_by_name['ThirdLoginReq']
+_CHINAMOBILEQUICKLOGINREQ = DESCRIPTOR.message_types_by_name['ChinaMobileQuickLoginReq']
+_CHINATELECOMAUTHREQ = DESCRIPTOR.message_types_by_name['ChinaTelecomAuthReq']
+_UMENGQUICKLOGINREQ = DESCRIPTOR.message_types_by_name['UmengQuickLoginReq']
+_DEVLOGINREQ = DESCRIPTOR.message_types_by_name['DevLoginReq']
+_RESETPASSWORDREQ = DESCRIPTOR.message_types_by_name['ResetPasswordReq']
+_RESETPASSWORDRES = DESCRIPTOR.message_types_by_name['ResetPasswordRes']
+_LOGINSECRETREQ = DESCRIPTOR.message_types_by_name['LoginSecretReq']
+_LOGINSECRETRES = DESCRIPTOR.message_types_by_name['LoginSecretRes']
+_UPDATEPASSWDREQ = DESCRIPTOR.message_types_by_name['UpdatePasswdReq']
+_UPDATEPASSWDRES = DESCRIPTOR.message_types_by_name['UpdatePasswdRes']
+_INVITEREQ = DESCRIPTOR.message_types_by_name['InviteReq']
+_INVITERES = DESCRIPTOR.message_types_by_name['InviteRes']
+_GETSYNCTIMEREQ = DESCRIPTOR.message_types_by_name['GetSyncTimeReq']
+_GETSYNCTIMERES = DESCRIPTOR.message_types_by_name['GetSyncTimeRes']
+_REPORTBUYNOBILITYREQ = DESCRIPTOR.message_types_by_name['ReportBuyNobilityReq']
+_REPORTBUYNOBILITYRES = DESCRIPTOR.message_types_by_name['ReportBuyNobilityRes']
+_GOOGLEIABNOTIFYREQ = DESCRIPTOR.message_types_by_name['GoogleIABNotifyReq']
+_GOOGLEIABNOTIFYREQ_BUYINTENT = _GOOGLEIABNOTIFYREQ.nested_types_by_name['BuyIntent']
+_GOOGLEIABNOTIFYRES = DESCRIPTOR.message_types_by_name['GoogleIABNotifyRes']
+_GOOGLEIABPRODUCTITEM = DESCRIPTOR.message_types_by_name['GoogleIABProductItem']
+_GOOGLEIABPRODUCTITEMSREQ = DESCRIPTOR.message_types_by_name['GoogleIABProductItemsReq']
+_GOOGLEIABPRODUCTITEMSRES = DESCRIPTOR.message_types_by_name['GoogleIABProductItemsRes']
+_GETWECHATAPPIDREQ = DESCRIPTOR.message_types_by_name['GetWeChatAppIdReq']
+_GETWECHATAPPIDRES = DESCRIPTOR.message_types_by_name['GetWeChatAppIdRes']
+_GETWECHATIDLOGINREQ = DESCRIPTOR.message_types_by_name['GetWeChatIdLoginReq']
+_GETWECHATIDLOGINRES = DESCRIPTOR.message_types_by_name['GetWeChatIdLoginRes']
+_USERINFO = DESCRIPTOR.message_types_by_name['UserInfo']
+_GETMINIPROGRAMLOGINREQ = DESCRIPTOR.message_types_by_name['GetMiniProgramLoginReq']
+_MINIPROGRAMPHONEREQ = DESCRIPTOR.message_types_by_name['MiniProgramPhoneReq']
+_MINIPROGRAMPHONERES = DESCRIPTOR.message_types_by_name['MiniProgramPhoneRes']
+_APPLYCERTIFYREQ = DESCRIPTOR.message_types_by_name['ApplyCertifyReq']
+_APPLYCERTIFYRES = DESCRIPTOR.message_types_by_name['ApplyCertifyRes']
+_APPLYCERTIFYSIGNREQ = DESCRIPTOR.message_types_by_name['ApplyCertifySignReq']
+_CERTIFYRESULTREQ = DESCRIPTOR.message_types_by_name['CertifyResultReq']
+_CERTIFYRESULTRES = DESCRIPTOR.message_types_by_name['CertifyResultRes']
+_ACCOUNTPHONESMSCODEREQ = DESCRIPTOR.message_types_by_name['AccountPhoneSmsCodeReq']
+_ACCOUNTPHONESMSCODERES = DESCRIPTOR.message_types_by_name['AccountPhoneSmsCodeRes']
+_ACCOUNTSUBSIDIARYLOGINREQ = DESCRIPTOR.message_types_by_name['AccountSubsidiaryLoginReq']
+_GETGUESTLOGINREQ = DESCRIPTOR.message_types_by_name['GetGuestLoginReq']
+_ACCOUNTBINDPHONESMSREQ = DESCRIPTOR.message_types_by_name['AccountBindPhoneSMSReq']
+_ACCOUNTBINDPHONESMSRES = DESCRIPTOR.message_types_by_name['AccountBindPhoneSMSRes']
+_ACCOUNTBINDTHIRDREQ = DESCRIPTOR.message_types_by_name['AccountBindThirdReq']
+_ACCOUNTBINDTHIRDRES = DESCRIPTOR.message_types_by_name['AccountBindThirdRes']
+_ACCOUNTBINDLISTREQ = DESCRIPTOR.message_types_by_name['AccountBindListReq']
+_ACCOUNTBINDLISTRES = DESCRIPTOR.message_types_by_name['AccountBindListRes']
+_BINDPHONESMSCODEREQ = DESCRIPTOR.message_types_by_name['BindPhoneSmsCodeReq']
+_BINDPHONESMSCODERES = DESCRIPTOR.message_types_by_name['BindPhoneSmsCodeRes']
+_BINDEMAILSESCODEREQ = DESCRIPTOR.message_types_by_name['BindEmailSesCodeReq']
+_BINDEMAILSESCODERES = DESCRIPTOR.message_types_by_name['BindEmailSesCodeRes']
+_ACCOUNTBINDEMAILSESREQ = DESCRIPTOR.message_types_by_name['AccountBindEmailSESReq']
+_ACCOUNTBINDEMAILSESRES = DESCRIPTOR.message_types_by_name['AccountBindEmailSESRes']
+_GETACCOUNTREGISTERREQ = DESCRIPTOR.message_types_by_name['GetAccountRegisterReq']
+_GETACCOUNTPASSWORDLOGINREQ = DESCRIPTOR.message_types_by_name['GetAccountPasswordLoginReq']
+_GETSESCODEREQ = DESCRIPTOR.message_types_by_name['GetSesCodeReq']
+_GETSESCODERES = DESCRIPTOR.message_types_by_name['GetSesCodeRes']
+_GETSESTOKENREQ = DESCRIPTOR.message_types_by_name['GetSesTokenReq']
+_GETSESTOKENRES = DESCRIPTOR.message_types_by_name['GetSesTokenRes']
+_RESETPASSWORDBYSESREQ = DESCRIPTOR.message_types_by_name['ResetPasswordBySesReq']
+_RESETPASSWORDBYSESRES = DESCRIPTOR.message_types_by_name['ResetPasswordBySesRes']
+_REMOTELOGINSENDCODEREQ = DESCRIPTOR.message_types_by_name['RemoteLoginSendCodeReq']
+_REMOTELOGINSENDCODERES = DESCRIPTOR.message_types_by_name['RemoteLoginSendCodeRes']
+_REMOTELOGINCONFIRMCODEREQ = DESCRIPTOR.message_types_by_name['RemoteLoginConfirmCodeReq']
+_REMOTELOGINCONFIRMCODERES = DESCRIPTOR.message_types_by_name['RemoteLoginConfirmCodeRes']
+_VERIFYCANCELSIGNINWITHAPPLEREQ = DESCRIPTOR.message_types_by_name['VerifyCancelSignInWithAppleReq']
+_VERIFYCANCELSIGNINWITHAPPLERES = DESCRIPTOR.message_types_by_name['VerifyCancelSignInWithAppleRes']
+_WECHATCODELOGINTICKETREQ = DESCRIPTOR.message_types_by_name['WechatCodeLoginTicketReq']
+_WECHATCODELOGINTICKETRES = DESCRIPTOR.message_types_by_name['WechatCodeLoginTicketRes']
+_GETWECHATMINICODEREQ = DESCRIPTOR.message_types_by_name['GetWechatMiniCodeReq']
+_GETWECHATMINICODERES = DESCRIPTOR.message_types_by_name['GetWechatMiniCodeRes']
+_GETWECHATMINICODESCANREQ = DESCRIPTOR.message_types_by_name['GetWechatMiniCodeScanReq']
+_GETWECHATMINICODESCANRES = DESCRIPTOR.message_types_by_name['GetWechatMiniCodeScanRes']
+_REFUSEPHONELICENSEREQ = DESCRIPTOR.message_types_by_name['RefusePhoneLicenseReq']
+_REFUSEPHONELICENSERES = DESCRIPTOR.message_types_by_name['RefusePhoneLicenseRes']
+_WECHATMINIBINDPHONEREQ = DESCRIPTOR.message_types_by_name['WechatMiniBindPhoneReq']
+_WECHATMINIBINDPHONERES = DESCRIPTOR.message_types_by_name['WechatMiniBindPhoneRes']
+_THIRDACCOUNTBINDWECHATINFO = DESCRIPTOR.message_types_by_name['ThirdAccountBindWeChatInfo']
+_THIRDACCOUNTBINDQQINFO = DESCRIPTOR.message_types_by_name['ThirdAccountBindQqInfo']
+_THIRDACCOUNTBINDINFO = DESCRIPTOR.message_types_by_name['ThirdAccountBindInfo']
+_THIRDACCOUNTBINDINFODATA = DESCRIPTOR.message_types_by_name['ThirdAccountBindInfoData']
+_THIRDACCOUNTBINDINFOREQ = DESCRIPTOR.message_types_by_name['ThirdAccountBindInfoReq']
+_THIRDACCOUNTBINDINFORES = DESCRIPTOR.message_types_by_name['ThirdAccountBindInfoRes']
+_BINDTHIRDACCOUNTREQ = DESCRIPTOR.message_types_by_name['BindThirdAccountReq']
+_BINDTHIRDACCOUNTRES = DESCRIPTOR.message_types_by_name['BindThirdAccountRes']
+_UNBINDTHIRDACCOUNTREQ = DESCRIPTOR.message_types_by_name['UnbindThirdAccountReq']
+_UNBINDTHIRDACCOUNTRES = DESCRIPTOR.message_types_by_name['UnbindThirdAccountRes']
+_GETQRCODELOGINCODEREQ = DESCRIPTOR.message_types_by_name['GetQrcodeLoginCodeReq']
+_GETQRCODELOGINCODERES = DESCRIPTOR.message_types_by_name['GetQrcodeLoginCodeRes']
+_QRCODESCANLOGINREQ = DESCRIPTOR.message_types_by_name['QrcodeScanLoginReq']
+_QRCODESCANLOGINRES = DESCRIPTOR.message_types_by_name['QrcodeScanLoginRes']
+_GETQRCODELOGINSTATUSREQ = DESCRIPTOR.message_types_by_name['GetQrcodeLoginStatusReq']
+_GETQRCODELOGINSTATUSRES = DESCRIPTOR.message_types_by_name['GetQrcodeLoginStatusRes']
+_SETQRCODELOGINSTATUSREQ = DESCRIPTOR.message_types_by_name['SetQrcodeLoginStatusReq']
+_SETQRCODELOGINSTATUSRES = DESCRIPTOR.message_types_by_name['SetQrcodeLoginStatusRes']
+_GETACCOUNTREGISTERSTATUSREQ = DESCRIPTOR.message_types_by_name['GetAccountRegisterStatusReq']
+_GETACCOUNTREGISTERSTATUSRES = DESCRIPTOR.message_types_by_name['GetAccountRegisterStatusRes']
+_GETUMENGPHONEREQ = DESCRIPTOR.message_types_by_name['GetUmengPhoneReq']
+_GETUMENGPHONERES = DESCRIPTOR.message_types_by_name['GetUmengPhoneRes']
+_ACCOUNTCROSSTYPEINFO = DESCRIPTOR.message_types_by_name['AccountCrossTypeInfo']
+_ACCOUNTCROSSTYPEINFOREQ = DESCRIPTOR.message_types_by_name['AccountCrossTypeInfoReq']
+_ACCOUNTCROSSTYPEINFORES = DESCRIPTOR.message_types_by_name['AccountCrossTypeInfoRes']
+_APPLYACCOUNTCROSSTYPEREQ = DESCRIPTOR.message_types_by_name['ApplyAccountCrossTypeReq']
+_APPLYACCOUNTCROSSTYPERES = DESCRIPTOR.message_types_by_name['ApplyAccountCrossTypeRes']
+_CHECKINAPPCHARGELIMITREQ = DESCRIPTOR.message_types_by_name['CheckInAppChargeLimitReq']
+_CHECKINAPPCHARGELIMITRES = DESCRIPTOR.message_types_by_name['CheckInAppChargeLimitRes']
+_GETALIPAYMINIORDERREQ = DESCRIPTOR.message_types_by_name['GetAlipayMiniOrderReq']
+_GETALIPAYMINIORDERREQ_EXTENDSENTRY = _GETALIPAYMINIORDERREQ.nested_types_by_name['ExtendsEntry']
+_GETALIPAYMINIORDERRES = DESCRIPTOR.message_types_by_name['GetAlipayMiniOrderRes']
+_GETGOODSLISTREQ = DESCRIPTOR.message_types_by_name['GetGoodsListReq']
+_GETGOODSLISTRES = DESCRIPTOR.message_types_by_name['GetGoodsListRes']
+_ALIPAYMINIINDEXITEM = DESCRIPTOR.message_types_by_name['AlipayMiniIndexItem']
+_ALIPAYMINIINDEXBANNER = DESCRIPTOR.message_types_by_name['AlipayMiniIndexBanner']
+_ALIPAYMINIINDEXGOODSLIST = DESCRIPTOR.message_types_by_name['AlipayMiniIndexGoodsList']
+_ALIPAYMINIINDEXGOODSITEM = DESCRIPTOR.message_types_by_name['AlipayMiniIndexGoodsItem']
+VerifyIAPReq = _reflection.GeneratedProtocolMessageType('VerifyIAPReq', (_message.Message,), {
+  'DESCRIPTOR' : _VERIFYIAPREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.VerifyIAPReq)
+  })
+_sym_db.RegisterMessage(VerifyIAPReq)
+
+VerifyIAPRes = _reflection.GeneratedProtocolMessageType('VerifyIAPRes', (_message.Message,), {
+  'DESCRIPTOR' : _VERIFYIAPRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.VerifyIAPRes)
+  })
+_sym_db.RegisterMessage(VerifyIAPRes)
+
+GoldCard = _reflection.GeneratedProtocolMessageType('GoldCard', (_message.Message,), {
+  'DESCRIPTOR' : _GOLDCARD,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GoldCard)
+  })
+_sym_db.RegisterMessage(GoldCard)
+
+GetGoodListReq = _reflection.GeneratedProtocolMessageType('GetGoodListReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETGOODLISTREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetGoodListReq)
+  })
+_sym_db.RegisterMessage(GetGoodListReq)
+
+GetGoodListRes = _reflection.GeneratedProtocolMessageType('GetGoodListRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETGOODLISTRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetGoodListRes)
+  })
+_sym_db.RegisterMessage(GetGoodListRes)
+
+OrderIAPReq = _reflection.GeneratedProtocolMessageType('OrderIAPReq', (_message.Message,), {
+  'DESCRIPTOR' : _ORDERIAPREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.OrderIAPReq)
+  })
+_sym_db.RegisterMessage(OrderIAPReq)
+
+OrderIAPRes = _reflection.GeneratedProtocolMessageType('OrderIAPRes', (_message.Message,), {
+  'DESCRIPTOR' : _ORDERIAPRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.OrderIAPRes)
+  })
+_sym_db.RegisterMessage(OrderIAPRes)
+
+CloseOrderIAPReq = _reflection.GeneratedProtocolMessageType('CloseOrderIAPReq', (_message.Message,), {
+  'DESCRIPTOR' : _CLOSEORDERIAPREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.CloseOrderIAPReq)
+  })
+_sym_db.RegisterMessage(CloseOrderIAPReq)
+
+CloseOrderIAPRes = _reflection.GeneratedProtocolMessageType('CloseOrderIAPRes', (_message.Message,), {
+  'DESCRIPTOR' : _CLOSEORDERIAPRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.CloseOrderIAPRes)
+  })
+_sym_db.RegisterMessage(CloseOrderIAPRes)
+
+VIPChargeAccountInfoReq = _reflection.GeneratedProtocolMessageType('VIPChargeAccountInfoReq', (_message.Message,), {
+  'DESCRIPTOR' : _VIPCHARGEACCOUNTINFOREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.VIPChargeAccountInfoReq)
+  })
+_sym_db.RegisterMessage(VIPChargeAccountInfoReq)
+
+VIPChargeAccountInfoRes = _reflection.GeneratedProtocolMessageType('VIPChargeAccountInfoRes', (_message.Message,), {
+  'DESCRIPTOR' : _VIPCHARGEACCOUNTINFORES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.VIPChargeAccountInfoRes)
+  })
+_sym_db.RegisterMessage(VIPChargeAccountInfoRes)
+
+VIPChargeLogReq = _reflection.GeneratedProtocolMessageType('VIPChargeLogReq', (_message.Message,), {
+  'DESCRIPTOR' : _VIPCHARGELOGREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.VIPChargeLogReq)
+  })
+_sym_db.RegisterMessage(VIPChargeLogReq)
+
+VIPChargeLogRes = _reflection.GeneratedProtocolMessageType('VIPChargeLogRes', (_message.Message,), {
+  'DESCRIPTOR' : _VIPCHARGELOGRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.VIPChargeLogRes)
+  })
+_sym_db.RegisterMessage(VIPChargeLogRes)
+
+VIPChargeLogs = _reflection.GeneratedProtocolMessageType('VIPChargeLogs', (_message.Message,), {
+  'DESCRIPTOR' : _VIPCHARGELOGS,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.VIPChargeLogs)
+  })
+_sym_db.RegisterMessage(VIPChargeLogs)
+
+VIPChargeItem = _reflection.GeneratedProtocolMessageType('VIPChargeItem', (_message.Message,), {
+  'DESCRIPTOR' : _VIPCHARGEITEM,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.VIPChargeItem)
+  })
+_sym_db.RegisterMessage(VIPChargeItem)
+
+ReportDataReq = _reflection.GeneratedProtocolMessageType('ReportDataReq', (_message.Message,), {
+  'DESCRIPTOR' : _REPORTDATAREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ReportDataReq)
+  })
+_sym_db.RegisterMessage(ReportDataReq)
+
+ReportDataRes = _reflection.GeneratedProtocolMessageType('ReportDataRes', (_message.Message,), {
+  'DESCRIPTOR' : _REPORTDATARES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ReportDataRes)
+  })
+_sym_db.RegisterMessage(ReportDataRes)
+
+GetChargeReq = _reflection.GeneratedProtocolMessageType('GetChargeReq', (_message.Message,), {
+
+  'ExtendsEntry' : _reflection.GeneratedProtocolMessageType('ExtendsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _GETCHARGEREQ_EXTENDSENTRY,
+    '__module__' : 'uauth_ext_pb2'
+    # @@protoc_insertion_point(class_scope:uauth_pb.GetChargeReq.ExtendsEntry)
+    })
+  ,
+
+  'ExtraDataEntry' : _reflection.GeneratedProtocolMessageType('ExtraDataEntry', (_message.Message,), {
+    'DESCRIPTOR' : _GETCHARGEREQ_EXTRADATAENTRY,
+    '__module__' : 'uauth_ext_pb2'
+    # @@protoc_insertion_point(class_scope:uauth_pb.GetChargeReq.ExtraDataEntry)
+    })
+  ,
+  'DESCRIPTOR' : _GETCHARGEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetChargeReq)
+  })
+_sym_db.RegisterMessage(GetChargeReq)
+_sym_db.RegisterMessage(GetChargeReq.ExtendsEntry)
+_sym_db.RegisterMessage(GetChargeReq.ExtraDataEntry)
+
+GetChargeRes = _reflection.GeneratedProtocolMessageType('GetChargeRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETCHARGERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetChargeRes)
+  })
+_sym_db.RegisterMessage(GetChargeRes)
+
+GetSmsCodeReq = _reflection.GeneratedProtocolMessageType('GetSmsCodeReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETSMSCODEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetSmsCodeReq)
+  })
+_sym_db.RegisterMessage(GetSmsCodeReq)
+
+GetSmsCodeRes = _reflection.GeneratedProtocolMessageType('GetSmsCodeRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETSMSCODERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetSmsCodeRes)
+  })
+_sym_db.RegisterMessage(GetSmsCodeRes)
+
+GetSmsTokenReq = _reflection.GeneratedProtocolMessageType('GetSmsTokenReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETSMSTOKENREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetSmsTokenReq)
+  })
+_sym_db.RegisterMessage(GetSmsTokenReq)
+
+GetSmsTokenRes = _reflection.GeneratedProtocolMessageType('GetSmsTokenRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETSMSTOKENRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetSmsTokenRes)
+  })
+_sym_db.RegisterMessage(GetSmsTokenRes)
+
+PhoneSmsCodeReq = _reflection.GeneratedProtocolMessageType('PhoneSmsCodeReq', (_message.Message,), {
+  'DESCRIPTOR' : _PHONESMSCODEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.PhoneSmsCodeReq)
+  })
+_sym_db.RegisterMessage(PhoneSmsCodeReq)
+
+PhoneSmsCodeRes = _reflection.GeneratedProtocolMessageType('PhoneSmsCodeRes', (_message.Message,), {
+  'DESCRIPTOR' : _PHONESMSCODERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.PhoneSmsCodeRes)
+  })
+_sym_db.RegisterMessage(PhoneSmsCodeRes)
+
+CheckPhoneSmsCodeReq = _reflection.GeneratedProtocolMessageType('CheckPhoneSmsCodeReq', (_message.Message,), {
+  'DESCRIPTOR' : _CHECKPHONESMSCODEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.CheckPhoneSmsCodeReq)
+  })
+_sym_db.RegisterMessage(CheckPhoneSmsCodeReq)
+
+CheckPhoneSmsCodeRes = _reflection.GeneratedProtocolMessageType('CheckPhoneSmsCodeRes', (_message.Message,), {
+  'DESCRIPTOR' : _CHECKPHONESMSCODERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.CheckPhoneSmsCodeRes)
+  })
+_sym_db.RegisterMessage(CheckPhoneSmsCodeRes)
+
+CommonSignInRes = _reflection.GeneratedProtocolMessageType('CommonSignInRes', (_message.Message,), {
+
+  'ExtendsEntry' : _reflection.GeneratedProtocolMessageType('ExtendsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _COMMONSIGNINRES_EXTENDSENTRY,
+    '__module__' : 'uauth_ext_pb2'
+    # @@protoc_insertion_point(class_scope:uauth_pb.CommonSignInRes.ExtendsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _COMMONSIGNINRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.CommonSignInRes)
+  })
+_sym_db.RegisterMessage(CommonSignInRes)
+_sym_db.RegisterMessage(CommonSignInRes.ExtendsEntry)
+
+SignInWithAppleReq = _reflection.GeneratedProtocolMessageType('SignInWithAppleReq', (_message.Message,), {
+  'DESCRIPTOR' : _SIGNINWITHAPPLEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.SignInWithAppleReq)
+  })
+_sym_db.RegisterMessage(SignInWithAppleReq)
+
+IdOrPhoneLoginReq = _reflection.GeneratedProtocolMessageType('IdOrPhoneLoginReq', (_message.Message,), {
+  'DESCRIPTOR' : _IDORPHONELOGINREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.IdOrPhoneLoginReq)
+  })
+_sym_db.RegisterMessage(IdOrPhoneLoginReq)
+
+LoginWithPhoneSMSReq = _reflection.GeneratedProtocolMessageType('LoginWithPhoneSMSReq', (_message.Message,), {
+  'DESCRIPTOR' : _LOGINWITHPHONESMSREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.LoginWithPhoneSMSReq)
+  })
+_sym_db.RegisterMessage(LoginWithPhoneSMSReq)
+
+ThirdLoginReq = _reflection.GeneratedProtocolMessageType('ThirdLoginReq', (_message.Message,), {
+  'DESCRIPTOR' : _THIRDLOGINREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdLoginReq)
+  })
+_sym_db.RegisterMessage(ThirdLoginReq)
+
+ChinaMobileQuickLoginReq = _reflection.GeneratedProtocolMessageType('ChinaMobileQuickLoginReq', (_message.Message,), {
+  'DESCRIPTOR' : _CHINAMOBILEQUICKLOGINREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ChinaMobileQuickLoginReq)
+  })
+_sym_db.RegisterMessage(ChinaMobileQuickLoginReq)
+
+ChinaTelecomAuthReq = _reflection.GeneratedProtocolMessageType('ChinaTelecomAuthReq', (_message.Message,), {
+  'DESCRIPTOR' : _CHINATELECOMAUTHREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ChinaTelecomAuthReq)
+  })
+_sym_db.RegisterMessage(ChinaTelecomAuthReq)
+
+UmengQuickLoginReq = _reflection.GeneratedProtocolMessageType('UmengQuickLoginReq', (_message.Message,), {
+  'DESCRIPTOR' : _UMENGQUICKLOGINREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.UmengQuickLoginReq)
+  })
+_sym_db.RegisterMessage(UmengQuickLoginReq)
+
+DevLoginReq = _reflection.GeneratedProtocolMessageType('DevLoginReq', (_message.Message,), {
+  'DESCRIPTOR' : _DEVLOGINREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.DevLoginReq)
+  })
+_sym_db.RegisterMessage(DevLoginReq)
+
+ResetPasswordReq = _reflection.GeneratedProtocolMessageType('ResetPasswordReq', (_message.Message,), {
+  'DESCRIPTOR' : _RESETPASSWORDREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ResetPasswordReq)
+  })
+_sym_db.RegisterMessage(ResetPasswordReq)
+
+ResetPasswordRes = _reflection.GeneratedProtocolMessageType('ResetPasswordRes', (_message.Message,), {
+  'DESCRIPTOR' : _RESETPASSWORDRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ResetPasswordRes)
+  })
+_sym_db.RegisterMessage(ResetPasswordRes)
+
+LoginSecretReq = _reflection.GeneratedProtocolMessageType('LoginSecretReq', (_message.Message,), {
+  'DESCRIPTOR' : _LOGINSECRETREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.LoginSecretReq)
+  })
+_sym_db.RegisterMessage(LoginSecretReq)
+
+LoginSecretRes = _reflection.GeneratedProtocolMessageType('LoginSecretRes', (_message.Message,), {
+  'DESCRIPTOR' : _LOGINSECRETRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.LoginSecretRes)
+  })
+_sym_db.RegisterMessage(LoginSecretRes)
+
+UpdatePasswdReq = _reflection.GeneratedProtocolMessageType('UpdatePasswdReq', (_message.Message,), {
+  'DESCRIPTOR' : _UPDATEPASSWDREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.UpdatePasswdReq)
+  })
+_sym_db.RegisterMessage(UpdatePasswdReq)
+
+UpdatePasswdRes = _reflection.GeneratedProtocolMessageType('UpdatePasswdRes', (_message.Message,), {
+  'DESCRIPTOR' : _UPDATEPASSWDRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.UpdatePasswdRes)
+  })
+_sym_db.RegisterMessage(UpdatePasswdRes)
+
+InviteReq = _reflection.GeneratedProtocolMessageType('InviteReq', (_message.Message,), {
+  'DESCRIPTOR' : _INVITEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.InviteReq)
+  })
+_sym_db.RegisterMessage(InviteReq)
+
+InviteRes = _reflection.GeneratedProtocolMessageType('InviteRes', (_message.Message,), {
+  'DESCRIPTOR' : _INVITERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.InviteRes)
+  })
+_sym_db.RegisterMessage(InviteRes)
+
+GetSyncTimeReq = _reflection.GeneratedProtocolMessageType('GetSyncTimeReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETSYNCTIMEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetSyncTimeReq)
+  })
+_sym_db.RegisterMessage(GetSyncTimeReq)
+
+GetSyncTimeRes = _reflection.GeneratedProtocolMessageType('GetSyncTimeRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETSYNCTIMERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetSyncTimeRes)
+  })
+_sym_db.RegisterMessage(GetSyncTimeRes)
+
+ReportBuyNobilityReq = _reflection.GeneratedProtocolMessageType('ReportBuyNobilityReq', (_message.Message,), {
+  'DESCRIPTOR' : _REPORTBUYNOBILITYREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ReportBuyNobilityReq)
+  })
+_sym_db.RegisterMessage(ReportBuyNobilityReq)
+
+ReportBuyNobilityRes = _reflection.GeneratedProtocolMessageType('ReportBuyNobilityRes', (_message.Message,), {
+  'DESCRIPTOR' : _REPORTBUYNOBILITYRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ReportBuyNobilityRes)
+  })
+_sym_db.RegisterMessage(ReportBuyNobilityRes)
+
+GoogleIABNotifyReq = _reflection.GeneratedProtocolMessageType('GoogleIABNotifyReq', (_message.Message,), {
+
+  'BuyIntent' : _reflection.GeneratedProtocolMessageType('BuyIntent', (_message.Message,), {
+    'DESCRIPTOR' : _GOOGLEIABNOTIFYREQ_BUYINTENT,
+    '__module__' : 'uauth_ext_pb2'
+    # @@protoc_insertion_point(class_scope:uauth_pb.GoogleIABNotifyReq.BuyIntent)
+    })
+  ,
+  'DESCRIPTOR' : _GOOGLEIABNOTIFYREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GoogleIABNotifyReq)
+  })
+_sym_db.RegisterMessage(GoogleIABNotifyReq)
+_sym_db.RegisterMessage(GoogleIABNotifyReq.BuyIntent)
+
+GoogleIABNotifyRes = _reflection.GeneratedProtocolMessageType('GoogleIABNotifyRes', (_message.Message,), {
+  'DESCRIPTOR' : _GOOGLEIABNOTIFYRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GoogleIABNotifyRes)
+  })
+_sym_db.RegisterMessage(GoogleIABNotifyRes)
+
+GoogleIABProductItem = _reflection.GeneratedProtocolMessageType('GoogleIABProductItem', (_message.Message,), {
+  'DESCRIPTOR' : _GOOGLEIABPRODUCTITEM,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GoogleIABProductItem)
+  })
+_sym_db.RegisterMessage(GoogleIABProductItem)
+
+GoogleIABProductItemsReq = _reflection.GeneratedProtocolMessageType('GoogleIABProductItemsReq', (_message.Message,), {
+  'DESCRIPTOR' : _GOOGLEIABPRODUCTITEMSREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GoogleIABProductItemsReq)
+  })
+_sym_db.RegisterMessage(GoogleIABProductItemsReq)
+
+GoogleIABProductItemsRes = _reflection.GeneratedProtocolMessageType('GoogleIABProductItemsRes', (_message.Message,), {
+  'DESCRIPTOR' : _GOOGLEIABPRODUCTITEMSRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GoogleIABProductItemsRes)
+  })
+_sym_db.RegisterMessage(GoogleIABProductItemsRes)
+
+GetWeChatAppIdReq = _reflection.GeneratedProtocolMessageType('GetWeChatAppIdReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETWECHATAPPIDREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetWeChatAppIdReq)
+  })
+_sym_db.RegisterMessage(GetWeChatAppIdReq)
+
+GetWeChatAppIdRes = _reflection.GeneratedProtocolMessageType('GetWeChatAppIdRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETWECHATAPPIDRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetWeChatAppIdRes)
+  })
+_sym_db.RegisterMessage(GetWeChatAppIdRes)
+
+GetWeChatIdLoginReq = _reflection.GeneratedProtocolMessageType('GetWeChatIdLoginReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETWECHATIDLOGINREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetWeChatIdLoginReq)
+  })
+_sym_db.RegisterMessage(GetWeChatIdLoginReq)
+
+GetWeChatIdLoginRes = _reflection.GeneratedProtocolMessageType('GetWeChatIdLoginRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETWECHATIDLOGINRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetWeChatIdLoginRes)
+  })
+_sym_db.RegisterMessage(GetWeChatIdLoginRes)
+
+UserInfo = _reflection.GeneratedProtocolMessageType('UserInfo', (_message.Message,), {
+  'DESCRIPTOR' : _USERINFO,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.UserInfo)
+  })
+_sym_db.RegisterMessage(UserInfo)
+
+GetMiniProgramLoginReq = _reflection.GeneratedProtocolMessageType('GetMiniProgramLoginReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETMINIPROGRAMLOGINREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetMiniProgramLoginReq)
+  })
+_sym_db.RegisterMessage(GetMiniProgramLoginReq)
+
+MiniProgramPhoneReq = _reflection.GeneratedProtocolMessageType('MiniProgramPhoneReq', (_message.Message,), {
+  'DESCRIPTOR' : _MINIPROGRAMPHONEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.MiniProgramPhoneReq)
+  })
+_sym_db.RegisterMessage(MiniProgramPhoneReq)
+
+MiniProgramPhoneRes = _reflection.GeneratedProtocolMessageType('MiniProgramPhoneRes', (_message.Message,), {
+  'DESCRIPTOR' : _MINIPROGRAMPHONERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.MiniProgramPhoneRes)
+  })
+_sym_db.RegisterMessage(MiniProgramPhoneRes)
+
+ApplyCertifyReq = _reflection.GeneratedProtocolMessageType('ApplyCertifyReq', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTIFYREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ApplyCertifyReq)
+  })
+_sym_db.RegisterMessage(ApplyCertifyReq)
+
+ApplyCertifyRes = _reflection.GeneratedProtocolMessageType('ApplyCertifyRes', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTIFYRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ApplyCertifyRes)
+  })
+_sym_db.RegisterMessage(ApplyCertifyRes)
+
+ApplyCertifySignReq = _reflection.GeneratedProtocolMessageType('ApplyCertifySignReq', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYCERTIFYSIGNREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ApplyCertifySignReq)
+  })
+_sym_db.RegisterMessage(ApplyCertifySignReq)
+
+CertifyResultReq = _reflection.GeneratedProtocolMessageType('CertifyResultReq', (_message.Message,), {
+  'DESCRIPTOR' : _CERTIFYRESULTREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.CertifyResultReq)
+  })
+_sym_db.RegisterMessage(CertifyResultReq)
+
+CertifyResultRes = _reflection.GeneratedProtocolMessageType('CertifyResultRes', (_message.Message,), {
+  'DESCRIPTOR' : _CERTIFYRESULTRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.CertifyResultRes)
+  })
+_sym_db.RegisterMessage(CertifyResultRes)
+
+AccountPhoneSmsCodeReq = _reflection.GeneratedProtocolMessageType('AccountPhoneSmsCodeReq', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTPHONESMSCODEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountPhoneSmsCodeReq)
+  })
+_sym_db.RegisterMessage(AccountPhoneSmsCodeReq)
+
+AccountPhoneSmsCodeRes = _reflection.GeneratedProtocolMessageType('AccountPhoneSmsCodeRes', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTPHONESMSCODERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountPhoneSmsCodeRes)
+  })
+_sym_db.RegisterMessage(AccountPhoneSmsCodeRes)
+
+AccountSubsidiaryLoginReq = _reflection.GeneratedProtocolMessageType('AccountSubsidiaryLoginReq', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTSUBSIDIARYLOGINREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountSubsidiaryLoginReq)
+  })
+_sym_db.RegisterMessage(AccountSubsidiaryLoginReq)
+
+GetGuestLoginReq = _reflection.GeneratedProtocolMessageType('GetGuestLoginReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETGUESTLOGINREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetGuestLoginReq)
+  })
+_sym_db.RegisterMessage(GetGuestLoginReq)
+
+AccountBindPhoneSMSReq = _reflection.GeneratedProtocolMessageType('AccountBindPhoneSMSReq', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTBINDPHONESMSREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindPhoneSMSReq)
+  })
+_sym_db.RegisterMessage(AccountBindPhoneSMSReq)
+
+AccountBindPhoneSMSRes = _reflection.GeneratedProtocolMessageType('AccountBindPhoneSMSRes', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTBINDPHONESMSRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindPhoneSMSRes)
+  })
+_sym_db.RegisterMessage(AccountBindPhoneSMSRes)
+
+AccountBindThirdReq = _reflection.GeneratedProtocolMessageType('AccountBindThirdReq', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTBINDTHIRDREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindThirdReq)
+  })
+_sym_db.RegisterMessage(AccountBindThirdReq)
+
+AccountBindThirdRes = _reflection.GeneratedProtocolMessageType('AccountBindThirdRes', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTBINDTHIRDRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindThirdRes)
+  })
+_sym_db.RegisterMessage(AccountBindThirdRes)
+
+AccountBindListReq = _reflection.GeneratedProtocolMessageType('AccountBindListReq', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTBINDLISTREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindListReq)
+  })
+_sym_db.RegisterMessage(AccountBindListReq)
+
+AccountBindListRes = _reflection.GeneratedProtocolMessageType('AccountBindListRes', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTBINDLISTRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindListRes)
+  })
+_sym_db.RegisterMessage(AccountBindListRes)
+
+BindPhoneSmsCodeReq = _reflection.GeneratedProtocolMessageType('BindPhoneSmsCodeReq', (_message.Message,), {
+  'DESCRIPTOR' : _BINDPHONESMSCODEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.BindPhoneSmsCodeReq)
+  })
+_sym_db.RegisterMessage(BindPhoneSmsCodeReq)
+
+BindPhoneSmsCodeRes = _reflection.GeneratedProtocolMessageType('BindPhoneSmsCodeRes', (_message.Message,), {
+  'DESCRIPTOR' : _BINDPHONESMSCODERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.BindPhoneSmsCodeRes)
+  })
+_sym_db.RegisterMessage(BindPhoneSmsCodeRes)
+
+BindEmailSesCodeReq = _reflection.GeneratedProtocolMessageType('BindEmailSesCodeReq', (_message.Message,), {
+  'DESCRIPTOR' : _BINDEMAILSESCODEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.BindEmailSesCodeReq)
+  })
+_sym_db.RegisterMessage(BindEmailSesCodeReq)
+
+BindEmailSesCodeRes = _reflection.GeneratedProtocolMessageType('BindEmailSesCodeRes', (_message.Message,), {
+  'DESCRIPTOR' : _BINDEMAILSESCODERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.BindEmailSesCodeRes)
+  })
+_sym_db.RegisterMessage(BindEmailSesCodeRes)
+
+AccountBindEmailSESReq = _reflection.GeneratedProtocolMessageType('AccountBindEmailSESReq', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTBINDEMAILSESREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindEmailSESReq)
+  })
+_sym_db.RegisterMessage(AccountBindEmailSESReq)
+
+AccountBindEmailSESRes = _reflection.GeneratedProtocolMessageType('AccountBindEmailSESRes', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTBINDEMAILSESRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountBindEmailSESRes)
+  })
+_sym_db.RegisterMessage(AccountBindEmailSESRes)
+
+GetAccountRegisterReq = _reflection.GeneratedProtocolMessageType('GetAccountRegisterReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETACCOUNTREGISTERREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetAccountRegisterReq)
+  })
+_sym_db.RegisterMessage(GetAccountRegisterReq)
+
+GetAccountPasswordLoginReq = _reflection.GeneratedProtocolMessageType('GetAccountPasswordLoginReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETACCOUNTPASSWORDLOGINREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetAccountPasswordLoginReq)
+  })
+_sym_db.RegisterMessage(GetAccountPasswordLoginReq)
+
+GetSesCodeReq = _reflection.GeneratedProtocolMessageType('GetSesCodeReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETSESCODEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetSesCodeReq)
+  })
+_sym_db.RegisterMessage(GetSesCodeReq)
+
+GetSesCodeRes = _reflection.GeneratedProtocolMessageType('GetSesCodeRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETSESCODERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetSesCodeRes)
+  })
+_sym_db.RegisterMessage(GetSesCodeRes)
+
+GetSesTokenReq = _reflection.GeneratedProtocolMessageType('GetSesTokenReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETSESTOKENREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetSesTokenReq)
+  })
+_sym_db.RegisterMessage(GetSesTokenReq)
+
+GetSesTokenRes = _reflection.GeneratedProtocolMessageType('GetSesTokenRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETSESTOKENRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetSesTokenRes)
+  })
+_sym_db.RegisterMessage(GetSesTokenRes)
+
+ResetPasswordBySesReq = _reflection.GeneratedProtocolMessageType('ResetPasswordBySesReq', (_message.Message,), {
+  'DESCRIPTOR' : _RESETPASSWORDBYSESREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ResetPasswordBySesReq)
+  })
+_sym_db.RegisterMessage(ResetPasswordBySesReq)
+
+ResetPasswordBySesRes = _reflection.GeneratedProtocolMessageType('ResetPasswordBySesRes', (_message.Message,), {
+  'DESCRIPTOR' : _RESETPASSWORDBYSESRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ResetPasswordBySesRes)
+  })
+_sym_db.RegisterMessage(ResetPasswordBySesRes)
+
+RemoteLoginSendCodeReq = _reflection.GeneratedProtocolMessageType('RemoteLoginSendCodeReq', (_message.Message,), {
+  'DESCRIPTOR' : _REMOTELOGINSENDCODEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.RemoteLoginSendCodeReq)
+  })
+_sym_db.RegisterMessage(RemoteLoginSendCodeReq)
+
+RemoteLoginSendCodeRes = _reflection.GeneratedProtocolMessageType('RemoteLoginSendCodeRes', (_message.Message,), {
+  'DESCRIPTOR' : _REMOTELOGINSENDCODERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.RemoteLoginSendCodeRes)
+  })
+_sym_db.RegisterMessage(RemoteLoginSendCodeRes)
+
+RemoteLoginConfirmCodeReq = _reflection.GeneratedProtocolMessageType('RemoteLoginConfirmCodeReq', (_message.Message,), {
+  'DESCRIPTOR' : _REMOTELOGINCONFIRMCODEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.RemoteLoginConfirmCodeReq)
+  })
+_sym_db.RegisterMessage(RemoteLoginConfirmCodeReq)
+
+RemoteLoginConfirmCodeRes = _reflection.GeneratedProtocolMessageType('RemoteLoginConfirmCodeRes', (_message.Message,), {
+  'DESCRIPTOR' : _REMOTELOGINCONFIRMCODERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.RemoteLoginConfirmCodeRes)
+  })
+_sym_db.RegisterMessage(RemoteLoginConfirmCodeRes)
+
+VerifyCancelSignInWithAppleReq = _reflection.GeneratedProtocolMessageType('VerifyCancelSignInWithAppleReq', (_message.Message,), {
+  'DESCRIPTOR' : _VERIFYCANCELSIGNINWITHAPPLEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.VerifyCancelSignInWithAppleReq)
+  })
+_sym_db.RegisterMessage(VerifyCancelSignInWithAppleReq)
+
+VerifyCancelSignInWithAppleRes = _reflection.GeneratedProtocolMessageType('VerifyCancelSignInWithAppleRes', (_message.Message,), {
+  'DESCRIPTOR' : _VERIFYCANCELSIGNINWITHAPPLERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.VerifyCancelSignInWithAppleRes)
+  })
+_sym_db.RegisterMessage(VerifyCancelSignInWithAppleRes)
+
+WechatCodeLoginTicketReq = _reflection.GeneratedProtocolMessageType('WechatCodeLoginTicketReq', (_message.Message,), {
+  'DESCRIPTOR' : _WECHATCODELOGINTICKETREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.WechatCodeLoginTicketReq)
+  })
+_sym_db.RegisterMessage(WechatCodeLoginTicketReq)
+
+WechatCodeLoginTicketRes = _reflection.GeneratedProtocolMessageType('WechatCodeLoginTicketRes', (_message.Message,), {
+  'DESCRIPTOR' : _WECHATCODELOGINTICKETRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.WechatCodeLoginTicketRes)
+  })
+_sym_db.RegisterMessage(WechatCodeLoginTicketRes)
+
+GetWechatMiniCodeReq = _reflection.GeneratedProtocolMessageType('GetWechatMiniCodeReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETWECHATMINICODEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetWechatMiniCodeReq)
+  })
+_sym_db.RegisterMessage(GetWechatMiniCodeReq)
+
+GetWechatMiniCodeRes = _reflection.GeneratedProtocolMessageType('GetWechatMiniCodeRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETWECHATMINICODERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetWechatMiniCodeRes)
+  })
+_sym_db.RegisterMessage(GetWechatMiniCodeRes)
+
+GetWechatMiniCodeScanReq = _reflection.GeneratedProtocolMessageType('GetWechatMiniCodeScanReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETWECHATMINICODESCANREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetWechatMiniCodeScanReq)
+  })
+_sym_db.RegisterMessage(GetWechatMiniCodeScanReq)
+
+GetWechatMiniCodeScanRes = _reflection.GeneratedProtocolMessageType('GetWechatMiniCodeScanRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETWECHATMINICODESCANRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetWechatMiniCodeScanRes)
+  })
+_sym_db.RegisterMessage(GetWechatMiniCodeScanRes)
+
+RefusePhoneLicenseReq = _reflection.GeneratedProtocolMessageType('RefusePhoneLicenseReq', (_message.Message,), {
+  'DESCRIPTOR' : _REFUSEPHONELICENSEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.RefusePhoneLicenseReq)
+  })
+_sym_db.RegisterMessage(RefusePhoneLicenseReq)
+
+RefusePhoneLicenseRes = _reflection.GeneratedProtocolMessageType('RefusePhoneLicenseRes', (_message.Message,), {
+  'DESCRIPTOR' : _REFUSEPHONELICENSERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.RefusePhoneLicenseRes)
+  })
+_sym_db.RegisterMessage(RefusePhoneLicenseRes)
+
+WechatMiniBindPhoneReq = _reflection.GeneratedProtocolMessageType('WechatMiniBindPhoneReq', (_message.Message,), {
+  'DESCRIPTOR' : _WECHATMINIBINDPHONEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.WechatMiniBindPhoneReq)
+  })
+_sym_db.RegisterMessage(WechatMiniBindPhoneReq)
+
+WechatMiniBindPhoneRes = _reflection.GeneratedProtocolMessageType('WechatMiniBindPhoneRes', (_message.Message,), {
+  'DESCRIPTOR' : _WECHATMINIBINDPHONERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.WechatMiniBindPhoneRes)
+  })
+_sym_db.RegisterMessage(WechatMiniBindPhoneRes)
+
+ThirdAccountBindWeChatInfo = _reflection.GeneratedProtocolMessageType('ThirdAccountBindWeChatInfo', (_message.Message,), {
+  'DESCRIPTOR' : _THIRDACCOUNTBINDWECHATINFO,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdAccountBindWeChatInfo)
+  })
+_sym_db.RegisterMessage(ThirdAccountBindWeChatInfo)
+
+ThirdAccountBindQqInfo = _reflection.GeneratedProtocolMessageType('ThirdAccountBindQqInfo', (_message.Message,), {
+  'DESCRIPTOR' : _THIRDACCOUNTBINDQQINFO,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdAccountBindQqInfo)
+  })
+_sym_db.RegisterMessage(ThirdAccountBindQqInfo)
+
+ThirdAccountBindInfo = _reflection.GeneratedProtocolMessageType('ThirdAccountBindInfo', (_message.Message,), {
+  'DESCRIPTOR' : _THIRDACCOUNTBINDINFO,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdAccountBindInfo)
+  })
+_sym_db.RegisterMessage(ThirdAccountBindInfo)
+
+ThirdAccountBindInfoData = _reflection.GeneratedProtocolMessageType('ThirdAccountBindInfoData', (_message.Message,), {
+  'DESCRIPTOR' : _THIRDACCOUNTBINDINFODATA,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdAccountBindInfoData)
+  })
+_sym_db.RegisterMessage(ThirdAccountBindInfoData)
+
+ThirdAccountBindInfoReq = _reflection.GeneratedProtocolMessageType('ThirdAccountBindInfoReq', (_message.Message,), {
+  'DESCRIPTOR' : _THIRDACCOUNTBINDINFOREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdAccountBindInfoReq)
+  })
+_sym_db.RegisterMessage(ThirdAccountBindInfoReq)
+
+ThirdAccountBindInfoRes = _reflection.GeneratedProtocolMessageType('ThirdAccountBindInfoRes', (_message.Message,), {
+  'DESCRIPTOR' : _THIRDACCOUNTBINDINFORES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ThirdAccountBindInfoRes)
+  })
+_sym_db.RegisterMessage(ThirdAccountBindInfoRes)
+
+BindThirdAccountReq = _reflection.GeneratedProtocolMessageType('BindThirdAccountReq', (_message.Message,), {
+  'DESCRIPTOR' : _BINDTHIRDACCOUNTREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.BindThirdAccountReq)
+  })
+_sym_db.RegisterMessage(BindThirdAccountReq)
+
+BindThirdAccountRes = _reflection.GeneratedProtocolMessageType('BindThirdAccountRes', (_message.Message,), {
+  'DESCRIPTOR' : _BINDTHIRDACCOUNTRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.BindThirdAccountRes)
+  })
+_sym_db.RegisterMessage(BindThirdAccountRes)
+
+UnbindThirdAccountReq = _reflection.GeneratedProtocolMessageType('UnbindThirdAccountReq', (_message.Message,), {
+  'DESCRIPTOR' : _UNBINDTHIRDACCOUNTREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.UnbindThirdAccountReq)
+  })
+_sym_db.RegisterMessage(UnbindThirdAccountReq)
+
+UnbindThirdAccountRes = _reflection.GeneratedProtocolMessageType('UnbindThirdAccountRes', (_message.Message,), {
+  'DESCRIPTOR' : _UNBINDTHIRDACCOUNTRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.UnbindThirdAccountRes)
+  })
+_sym_db.RegisterMessage(UnbindThirdAccountRes)
+
+GetQrcodeLoginCodeReq = _reflection.GeneratedProtocolMessageType('GetQrcodeLoginCodeReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETQRCODELOGINCODEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetQrcodeLoginCodeReq)
+  })
+_sym_db.RegisterMessage(GetQrcodeLoginCodeReq)
+
+GetQrcodeLoginCodeRes = _reflection.GeneratedProtocolMessageType('GetQrcodeLoginCodeRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETQRCODELOGINCODERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetQrcodeLoginCodeRes)
+  })
+_sym_db.RegisterMessage(GetQrcodeLoginCodeRes)
+
+QrcodeScanLoginReq = _reflection.GeneratedProtocolMessageType('QrcodeScanLoginReq', (_message.Message,), {
+  'DESCRIPTOR' : _QRCODESCANLOGINREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.QrcodeScanLoginReq)
+  })
+_sym_db.RegisterMessage(QrcodeScanLoginReq)
+
+QrcodeScanLoginRes = _reflection.GeneratedProtocolMessageType('QrcodeScanLoginRes', (_message.Message,), {
+  'DESCRIPTOR' : _QRCODESCANLOGINRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.QrcodeScanLoginRes)
+  })
+_sym_db.RegisterMessage(QrcodeScanLoginRes)
+
+GetQrcodeLoginStatusReq = _reflection.GeneratedProtocolMessageType('GetQrcodeLoginStatusReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETQRCODELOGINSTATUSREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetQrcodeLoginStatusReq)
+  })
+_sym_db.RegisterMessage(GetQrcodeLoginStatusReq)
+
+GetQrcodeLoginStatusRes = _reflection.GeneratedProtocolMessageType('GetQrcodeLoginStatusRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETQRCODELOGINSTATUSRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetQrcodeLoginStatusRes)
+  })
+_sym_db.RegisterMessage(GetQrcodeLoginStatusRes)
+
+SetQrcodeLoginStatusReq = _reflection.GeneratedProtocolMessageType('SetQrcodeLoginStatusReq', (_message.Message,), {
+  'DESCRIPTOR' : _SETQRCODELOGINSTATUSREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.SetQrcodeLoginStatusReq)
+  })
+_sym_db.RegisterMessage(SetQrcodeLoginStatusReq)
+
+SetQrcodeLoginStatusRes = _reflection.GeneratedProtocolMessageType('SetQrcodeLoginStatusRes', (_message.Message,), {
+  'DESCRIPTOR' : _SETQRCODELOGINSTATUSRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.SetQrcodeLoginStatusRes)
+  })
+_sym_db.RegisterMessage(SetQrcodeLoginStatusRes)
+
+GetAccountRegisterStatusReq = _reflection.GeneratedProtocolMessageType('GetAccountRegisterStatusReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETACCOUNTREGISTERSTATUSREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetAccountRegisterStatusReq)
+  })
+_sym_db.RegisterMessage(GetAccountRegisterStatusReq)
+
+GetAccountRegisterStatusRes = _reflection.GeneratedProtocolMessageType('GetAccountRegisterStatusRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETACCOUNTREGISTERSTATUSRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetAccountRegisterStatusRes)
+  })
+_sym_db.RegisterMessage(GetAccountRegisterStatusRes)
+
+GetUmengPhoneReq = _reflection.GeneratedProtocolMessageType('GetUmengPhoneReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETUMENGPHONEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetUmengPhoneReq)
+  })
+_sym_db.RegisterMessage(GetUmengPhoneReq)
+
+GetUmengPhoneRes = _reflection.GeneratedProtocolMessageType('GetUmengPhoneRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETUMENGPHONERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetUmengPhoneRes)
+  })
+_sym_db.RegisterMessage(GetUmengPhoneRes)
+
+AccountCrossTypeInfo = _reflection.GeneratedProtocolMessageType('AccountCrossTypeInfo', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTCROSSTYPEINFO,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountCrossTypeInfo)
+  })
+_sym_db.RegisterMessage(AccountCrossTypeInfo)
+
+AccountCrossTypeInfoReq = _reflection.GeneratedProtocolMessageType('AccountCrossTypeInfoReq', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTCROSSTYPEINFOREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountCrossTypeInfoReq)
+  })
+_sym_db.RegisterMessage(AccountCrossTypeInfoReq)
+
+AccountCrossTypeInfoRes = _reflection.GeneratedProtocolMessageType('AccountCrossTypeInfoRes', (_message.Message,), {
+  'DESCRIPTOR' : _ACCOUNTCROSSTYPEINFORES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AccountCrossTypeInfoRes)
+  })
+_sym_db.RegisterMessage(AccountCrossTypeInfoRes)
+
+ApplyAccountCrossTypeReq = _reflection.GeneratedProtocolMessageType('ApplyAccountCrossTypeReq', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYACCOUNTCROSSTYPEREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ApplyAccountCrossTypeReq)
+  })
+_sym_db.RegisterMessage(ApplyAccountCrossTypeReq)
+
+ApplyAccountCrossTypeRes = _reflection.GeneratedProtocolMessageType('ApplyAccountCrossTypeRes', (_message.Message,), {
+  'DESCRIPTOR' : _APPLYACCOUNTCROSSTYPERES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.ApplyAccountCrossTypeRes)
+  })
+_sym_db.RegisterMessage(ApplyAccountCrossTypeRes)
+
+CheckInAppChargeLimitReq = _reflection.GeneratedProtocolMessageType('CheckInAppChargeLimitReq', (_message.Message,), {
+  'DESCRIPTOR' : _CHECKINAPPCHARGELIMITREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.CheckInAppChargeLimitReq)
+  })
+_sym_db.RegisterMessage(CheckInAppChargeLimitReq)
+
+CheckInAppChargeLimitRes = _reflection.GeneratedProtocolMessageType('CheckInAppChargeLimitRes', (_message.Message,), {
+  'DESCRIPTOR' : _CHECKINAPPCHARGELIMITRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.CheckInAppChargeLimitRes)
+  })
+_sym_db.RegisterMessage(CheckInAppChargeLimitRes)
+
+GetAlipayMiniOrderReq = _reflection.GeneratedProtocolMessageType('GetAlipayMiniOrderReq', (_message.Message,), {
+
+  'ExtendsEntry' : _reflection.GeneratedProtocolMessageType('ExtendsEntry', (_message.Message,), {
+    'DESCRIPTOR' : _GETALIPAYMINIORDERREQ_EXTENDSENTRY,
+    '__module__' : 'uauth_ext_pb2'
+    # @@protoc_insertion_point(class_scope:uauth_pb.GetAlipayMiniOrderReq.ExtendsEntry)
+    })
+  ,
+  'DESCRIPTOR' : _GETALIPAYMINIORDERREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetAlipayMiniOrderReq)
+  })
+_sym_db.RegisterMessage(GetAlipayMiniOrderReq)
+_sym_db.RegisterMessage(GetAlipayMiniOrderReq.ExtendsEntry)
+
+GetAlipayMiniOrderRes = _reflection.GeneratedProtocolMessageType('GetAlipayMiniOrderRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETALIPAYMINIORDERRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetAlipayMiniOrderRes)
+  })
+_sym_db.RegisterMessage(GetAlipayMiniOrderRes)
+
+GetGoodsListReq = _reflection.GeneratedProtocolMessageType('GetGoodsListReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETGOODSLISTREQ,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetGoodsListReq)
+  })
+_sym_db.RegisterMessage(GetGoodsListReq)
+
+GetGoodsListRes = _reflection.GeneratedProtocolMessageType('GetGoodsListRes', (_message.Message,), {
+  'DESCRIPTOR' : _GETGOODSLISTRES,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.GetGoodsListRes)
+  })
+_sym_db.RegisterMessage(GetGoodsListRes)
+
+AlipayMiniIndexItem = _reflection.GeneratedProtocolMessageType('AlipayMiniIndexItem', (_message.Message,), {
+  'DESCRIPTOR' : _ALIPAYMINIINDEXITEM,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AlipayMiniIndexItem)
+  })
+_sym_db.RegisterMessage(AlipayMiniIndexItem)
+
+AlipayMiniIndexBanner = _reflection.GeneratedProtocolMessageType('AlipayMiniIndexBanner', (_message.Message,), {
+  'DESCRIPTOR' : _ALIPAYMINIINDEXBANNER,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AlipayMiniIndexBanner)
+  })
+_sym_db.RegisterMessage(AlipayMiniIndexBanner)
+
+AlipayMiniIndexGoodsList = _reflection.GeneratedProtocolMessageType('AlipayMiniIndexGoodsList', (_message.Message,), {
+  'DESCRIPTOR' : _ALIPAYMINIINDEXGOODSLIST,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AlipayMiniIndexGoodsList)
+  })
+_sym_db.RegisterMessage(AlipayMiniIndexGoodsList)
+
+AlipayMiniIndexGoodsItem = _reflection.GeneratedProtocolMessageType('AlipayMiniIndexGoodsItem', (_message.Message,), {
+  'DESCRIPTOR' : _ALIPAYMINIINDEXGOODSITEM,
+  '__module__' : 'uauth_ext_pb2'
+  # @@protoc_insertion_point(class_scope:uauth_pb.AlipayMiniIndexGoodsItem)
+  })
+_sym_db.RegisterMessage(AlipayMiniIndexGoodsItem)
+
+_UAUTHEXTOBJ = DESCRIPTOR.services_by_name['UauthExtObj']
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\242\002\005PROTO'
+  _GETCHARGEREQ_EXTENDSENTRY._options = None
+  _GETCHARGEREQ_EXTENDSENTRY._serialized_options = b'8\001'
+  _GETCHARGEREQ_EXTRADATAENTRY._options = None
+  _GETCHARGEREQ_EXTRADATAENTRY._serialized_options = b'8\001'
+  _COMMONSIGNINRES_EXTENDSENTRY._options = None
+  _COMMONSIGNINRES_EXTENDSENTRY._serialized_options = b'8\001'
+  _GETALIPAYMINIORDERREQ_EXTENDSENTRY._options = None
+  _GETALIPAYMINIORDERREQ_EXTENDSENTRY._serialized_options = b'8\001'
+  _ERRORUAUTHCODE._serialized_start=11797
+  _ERRORUAUTHCODE._serialized_end=12699
+  _IAPSTATUSTYPE._serialized_start=12701
+  _IAPSTATUSTYPE._serialized_end=12774
+  _CHARGESTATUS._serialized_start=12776
+  _CHARGESTATUS._serialized_end=12837
+  _REPORTDATATYPE._serialized_start=12839
+  _REPORTDATATYPE._serialized_end=12896
+  _VERIFYTYPE._serialized_start=12898
+  _VERIFYTYPE._serialized_end=12980
+  _SMSCODETPL._serialized_start=12982
+  _SMSCODETPL._serialized_end=13089
+  _CERTIFYTYPE._serialized_start=13091
+  _CERTIFYTYPE._serialized_end=13132
+  _WECHATMINICODESCANSTATUS._serialized_start=13135
+  _WECHATMINICODESCANSTATUS._serialized_end=13265
+  _THIRDACCOUNTBINDTYPE._serialized_start=13267
+  _THIRDACCOUNTBINDTYPE._serialized_end=13334
+  _UNBINDTHIRDACCOUNTOPTTYPE._serialized_start=13336
+  _UNBINDTHIRDACCOUNTOPTTYPE._serialized_end=13397
+  _GETQRCODELOGINSTATUS._serialized_start=13399
+  _GETQRCODELOGINSTATUS._serialized_end=13482
+  _ACCOUNTREGISTERTYPE._serialized_start=13484
+  _ACCOUNTREGISTERTYPE._serialized_end=13546
+  _ACCOUNTAPPCROSSTYPE._serialized_start=13548
+  _ACCOUNTAPPCROSSTYPE._serialized_end=13599
+  _APPCHARGETYPE._serialized_start=13601
+  _APPCHARGETYPE._serialized_end=13661
+  _ALIPAYMINIINDEXTYPE._serialized_start=13663
+  _ALIPAYMINIINDEXTYPE._serialized_end=13732
+  _ALIPAYMINIGOODSTYPE._serialized_start=13734
+  _ALIPAYMINIGOODSTYPE._serialized_end=13785
+  _VERIFYIAPREQ._serialized_start=49
+  _VERIFYIAPREQ._serialized_end=158
+  _VERIFYIAPRES._serialized_start=160
+  _VERIFYIAPRES._serialized_end=174
+  _GOLDCARD._serialized_start=176
+  _GOLDCARD._serialized_end=273
+  _GETGOODLISTREQ._serialized_start=275
+  _GETGOODLISTREQ._serialized_end=291
+  _GETGOODLISTRES._serialized_start=293
+  _GETGOODLISTRES._serialized_end=365
+  _ORDERIAPREQ._serialized_start=367
+  _ORDERIAPREQ._serialized_end=411
+  _ORDERIAPRES._serialized_start=413
+  _ORDERIAPRES._serialized_end=444
+  _CLOSEORDERIAPREQ._serialized_start=446
+  _CLOSEORDERIAPREQ._serialized_end=523
+  _CLOSEORDERIAPRES._serialized_start=525
+  _CLOSEORDERIAPRES._serialized_end=543
+  _VIPCHARGEACCOUNTINFOREQ._serialized_start=545
+  _VIPCHARGEACCOUNTINFOREQ._serialized_end=582
+  _VIPCHARGEACCOUNTINFORES._serialized_start=585
+  _VIPCHARGEACCOUNTINFORES._serialized_end=726
+  _VIPCHARGELOGREQ._serialized_start=728
+  _VIPCHARGELOGREQ._serialized_end=745
+  _VIPCHARGELOGRES._serialized_start=747
+  _VIPCHARGELOGRES._serialized_end=803
+  _VIPCHARGELOGS._serialized_start=805
+  _VIPCHARGELOGS._serialized_end=872
+  _VIPCHARGEITEM._serialized_start=874
+  _VIPCHARGEITEM._serialized_end=994
+  _REPORTDATAREQ._serialized_start=996
+  _REPORTDATAREQ._serialized_end=1065
+  _REPORTDATARES._serialized_start=1067
+  _REPORTDATARES._serialized_end=1082
+  _GETCHARGEREQ._serialized_start=1085
+  _GETCHARGEREQ._serialized_end=1461
+  _GETCHARGEREQ_EXTENDSENTRY._serialized_start=1365
+  _GETCHARGEREQ_EXTENDSENTRY._serialized_end=1411
+  _GETCHARGEREQ_EXTRADATAENTRY._serialized_start=1413
+  _GETCHARGEREQ_EXTRADATAENTRY._serialized_end=1461
+  _GETCHARGERES._serialized_start=1463
+  _GETCHARGERES._serialized_end=1543
+  _GETSMSCODEREQ._serialized_start=1545
+  _GETSMSCODEREQ._serialized_end=1659
+  _GETSMSCODERES._serialized_start=1661
+  _GETSMSCODERES._serialized_end=1676
+  _GETSMSTOKENREQ._serialized_start=1679
+  _GETSMSTOKENREQ._serialized_end=1812
+  _GETSMSTOKENRES._serialized_start=1814
+  _GETSMSTOKENRES._serialized_end=1849
+  _PHONESMSCODEREQ._serialized_start=1851
+  _PHONESMSCODEREQ._serialized_end=1912
+  _PHONESMSCODERES._serialized_start=1914
+  _PHONESMSCODERES._serialized_end=1931
+  _CHECKPHONESMSCODEREQ._serialized_start=1933
+  _CHECKPHONESMSCODEREQ._serialized_end=2017
+  _CHECKPHONESMSCODERES._serialized_start=2019
+  _CHECKPHONESMSCODERES._serialized_end=2041
+  _COMMONSIGNINRES._serialized_start=2044
+  _COMMONSIGNINRES._serialized_end=2266
+  _COMMONSIGNINRES_EXTENDSENTRY._serialized_start=1365
+  _COMMONSIGNINRES_EXTENDSENTRY._serialized_end=1411
+  _SIGNINWITHAPPLEREQ._serialized_start=2269
+  _SIGNINWITHAPPLEREQ._serialized_end=2475
+  _IDORPHONELOGINREQ._serialized_start=2478
+  _IDORPHONELOGINREQ._serialized_end=2627
+  _LOGINWITHPHONESMSREQ._serialized_start=2630
+  _LOGINWITHPHONESMSREQ._serialized_end=2921
+  _THIRDLOGINREQ._serialized_start=2924
+  _THIRDLOGINREQ._serialized_end=3212
+  _CHINAMOBILEQUICKLOGINREQ._serialized_start=3215
+  _CHINAMOBILEQUICKLOGINREQ._serialized_end=3425
+  _CHINATELECOMAUTHREQ._serialized_start=3428
+  _CHINATELECOMAUTHREQ._serialized_end=3624
+  _UMENGQUICKLOGINREQ._serialized_start=3627
+  _UMENGQUICKLOGINREQ._serialized_end=3832
+  _DEVLOGINREQ._serialized_start=3835
+  _DEVLOGINREQ._serialized_end=4015
+  _RESETPASSWORDREQ._serialized_start=4018
+  _RESETPASSWORDREQ._serialized_end=4161
+  _RESETPASSWORDRES._serialized_start=4163
+  _RESETPASSWORDRES._serialized_end=4181
+  _LOGINSECRETREQ._serialized_start=4183
+  _LOGINSECRETREQ._serialized_end=4199
+  _LOGINSECRETRES._serialized_start=4201
+  _LOGINSECRETRES._serialized_end=4230
+  _UPDATEPASSWDREQ._serialized_start=4232
+  _UPDATEPASSWDREQ._serialized_end=4319
+  _UPDATEPASSWDRES._serialized_start=4321
+  _UPDATEPASSWDRES._serialized_end=4338
+  _INVITEREQ._serialized_start=4340
+  _INVITEREQ._serialized_end=4400
+  _INVITERES._serialized_start=4402
+  _INVITERES._serialized_end=4413
+  _GETSYNCTIMEREQ._serialized_start=4415
+  _GETSYNCTIMEREQ._serialized_end=4431
+  _GETSYNCTIMERES._serialized_start=4433
+  _GETSYNCTIMERES._serialized_end=4449
+  _REPORTBUYNOBILITYREQ._serialized_start=4451
+  _REPORTBUYNOBILITYREQ._serialized_end=4510
+  _REPORTBUYNOBILITYRES._serialized_start=4512
+  _REPORTBUYNOBILITYRES._serialized_end=4534
+  _GOOGLEIABNOTIFYREQ._serialized_start=4537
+  _GOOGLEIABNOTIFYREQ._serialized_end=4716
+  _GOOGLEIABNOTIFYREQ_BUYINTENT._serialized_start=4658
+  _GOOGLEIABNOTIFYREQ_BUYINTENT._serialized_end=4716
+  _GOOGLEIABNOTIFYRES._serialized_start=4718
+  _GOOGLEIABNOTIFYRES._serialized_end=4738
+  _GOOGLEIABPRODUCTITEM._serialized_start=4740
+  _GOOGLEIABPRODUCTITEM._serialized_end=4817
+  _GOOGLEIABPRODUCTITEMSREQ._serialized_start=4819
+  _GOOGLEIABPRODUCTITEMSREQ._serialized_end=4845
+  _GOOGLEIABPRODUCTITEMSRES._serialized_start=4847
+  _GOOGLEIABPRODUCTITEMSRES._serialized_end=4920
+  _GETWECHATAPPIDREQ._serialized_start=4922
+  _GETWECHATAPPIDREQ._serialized_end=4941
+  _GETWECHATAPPIDRES._serialized_start=4943
+  _GETWECHATAPPIDRES._serialized_end=4978
+  _GETWECHATIDLOGINREQ._serialized_start=4980
+  _GETWECHATIDLOGINREQ._serialized_end=5015
+  _GETWECHATIDLOGINRES._serialized_start=5017
+  _GETWECHATIDLOGINRES._serialized_end=5088
+  _USERINFO._serialized_start=5090
+  _USERINFO._serialized_end=5148
+  _GETMINIPROGRAMLOGINREQ._serialized_start=5151
+  _GETMINIPROGRAMLOGINREQ._serialized_end=5391
+  _MINIPROGRAMPHONEREQ._serialized_start=5393
+  _MINIPROGRAMPHONEREQ._serialized_end=5510
+  _MINIPROGRAMPHONERES._serialized_start=5512
+  _MINIPROGRAMPHONERES._serialized_end=5533
+  _APPLYCERTIFYREQ._serialized_start=5535
+  _APPLYCERTIFYREQ._serialized_end=5628
+  _APPLYCERTIFYRES._serialized_start=5630
+  _APPLYCERTIFYRES._serialized_end=5728
+  _APPLYCERTIFYSIGNREQ._serialized_start=5731
+  _APPLYCERTIFYSIGNREQ._serialized_end=5869
+  _CERTIFYRESULTREQ._serialized_start=5871
+  _CERTIFYRESULTREQ._serialized_end=5889
+  _CERTIFYRESULTRES._serialized_start=5891
+  _CERTIFYRESULTRES._serialized_end=5985
+  _ACCOUNTPHONESMSCODEREQ._serialized_start=5987
+  _ACCOUNTPHONESMSCODEREQ._serialized_end=6011
+  _ACCOUNTPHONESMSCODERES._serialized_start=6013
+  _ACCOUNTPHONESMSCODERES._serialized_end=6037
+  _ACCOUNTSUBSIDIARYLOGINREQ._serialized_start=6040
+  _ACCOUNTSUBSIDIARYLOGINREQ._serialized_end=6238
+  _GETGUESTLOGINREQ._serialized_start=6241
+  _GETGUESTLOGINREQ._serialized_end=6379
+  _ACCOUNTBINDPHONESMSREQ._serialized_start=6381
+  _ACCOUNTBINDPHONESMSREQ._serialized_end=6478
+  _ACCOUNTBINDPHONESMSRES._serialized_start=6480
+  _ACCOUNTBINDPHONESMSRES._serialized_end=6504
+  _ACCOUNTBINDTHIRDREQ._serialized_start=6507
+  _ACCOUNTBINDTHIRDREQ._serialized_end=6648
+  _ACCOUNTBINDTHIRDRES._serialized_start=6650
+  _ACCOUNTBINDTHIRDRES._serialized_end=6671
+  _ACCOUNTBINDLISTREQ._serialized_start=6673
+  _ACCOUNTBINDLISTREQ._serialized_end=6693
+  _ACCOUNTBINDLISTRES._serialized_start=6695
+  _ACCOUNTBINDLISTRES._serialized_end=6785
+  _BINDPHONESMSCODEREQ._serialized_start=6787
+  _BINDPHONESMSCODEREQ._serialized_end=6883
+  _BINDPHONESMSCODERES._serialized_start=6885
+  _BINDPHONESMSCODERES._serialized_end=6906
+  _BINDEMAILSESCODEREQ._serialized_start=6908
+  _BINDEMAILSESCODEREQ._serialized_end=6984
+  _BINDEMAILSESCODERES._serialized_start=6986
+  _BINDEMAILSESCODERES._serialized_end=7007
+  _ACCOUNTBINDEMAILSESREQ._serialized_start=7009
+  _ACCOUNTBINDEMAILSESREQ._serialized_end=7106
+  _ACCOUNTBINDEMAILSESRES._serialized_start=7108
+  _ACCOUNTBINDEMAILSESRES._serialized_end=7132
+  _GETACCOUNTREGISTERREQ._serialized_start=7135
+  _GETACCOUNTREGISTERREQ._serialized_end=7361
+  _GETACCOUNTPASSWORDLOGINREQ._serialized_start=7364
+  _GETACCOUNTPASSWORDLOGINREQ._serialized_end=7543
+  _GETSESCODEREQ._serialized_start=7545
+  _GETSESCODEREQ._serialized_end=7595
+  _GETSESCODERES._serialized_start=7597
+  _GETSESCODERES._serialized_end=7612
+  _GETSESTOKENREQ._serialized_start=7614
+  _GETSESTOKENREQ._serialized_end=7683
+  _GETSESTOKENRES._serialized_start=7685
+  _GETSESTOKENRES._serialized_end=7720
+  _RESETPASSWORDBYSESREQ._serialized_start=7722
+  _RESETPASSWORDBYSESREQ._serialized_end=7831
+  _RESETPASSWORDBYSESRES._serialized_start=7833
+  _RESETPASSWORDBYSESRES._serialized_end=7856
+  _REMOTELOGINSENDCODEREQ._serialized_start=7858
+  _REMOTELOGINSENDCODEREQ._serialized_end=7899
+  _REMOTELOGINSENDCODERES._serialized_start=7901
+  _REMOTELOGINSENDCODERES._serialized_end=7925
+  _REMOTELOGINCONFIRMCODEREQ._serialized_start=7927
+  _REMOTELOGINCONFIRMCODEREQ._serialized_end=7985
+  _REMOTELOGINCONFIRMCODERES._serialized_start=7987
+  _REMOTELOGINCONFIRMCODERES._serialized_end=8054
+  _VERIFYCANCELSIGNINWITHAPPLEREQ._serialized_start=8056
+  _VERIFYCANCELSIGNINWITHAPPLEREQ._serialized_end=8140
+  _VERIFYCANCELSIGNINWITHAPPLERES._serialized_start=8142
+  _VERIFYCANCELSIGNINWITHAPPLERES._serialized_end=8174
+  _WECHATCODELOGINTICKETREQ._serialized_start=8176
+  _WECHATCODELOGINTICKETREQ._serialized_end=8218
+  _WECHATCODELOGINTICKETRES._serialized_start=8220
+  _WECHATCODELOGINTICKETRES._serialized_end=8262
+  _GETWECHATMINICODEREQ._serialized_start=8264
+  _GETWECHATMINICODEREQ._serialized_end=8302
+  _GETWECHATMINICODERES._serialized_start=8304
+  _GETWECHATMINICODERES._serialized_end=8357
+  _GETWECHATMINICODESCANREQ._serialized_start=8359
+  _GETWECHATMINICODESCANREQ._serialized_end=8424
+  _GETWECHATMINICODESCANRES._serialized_start=8426
+  _GETWECHATMINICODESCANRES._serialized_end=8551
+  _REFUSEPHONELICENSEREQ._serialized_start=8553
+  _REFUSEPHONELICENSEREQ._serialized_end=8593
+  _REFUSEPHONELICENSERES._serialized_start=8595
+  _REFUSEPHONELICENSERES._serialized_end=8618
+  _WECHATMINIBINDPHONEREQ._serialized_start=8620
+  _WECHATMINIBINDPHONEREQ._serialized_end=8673
+  _WECHATMINIBINDPHONERES._serialized_start=8675
+  _WECHATMINIBINDPHONERES._serialized_end=8699
+  _THIRDACCOUNTBINDWECHATINFO._serialized_start=8701
+  _THIRDACCOUNTBINDWECHATINFO._serialized_end=8747
+  _THIRDACCOUNTBINDQQINFO._serialized_start=8749
+  _THIRDACCOUNTBINDQQINFO._serialized_end=8791
+  _THIRDACCOUNTBINDINFO._serialized_start=8794
+  _THIRDACCOUNTBINDINFO._serialized_end=8943
+  _THIRDACCOUNTBINDINFODATA._serialized_start=8945
+  _THIRDACCOUNTBINDINFODATA._serialized_end=9068
+  _THIRDACCOUNTBINDINFOREQ._serialized_start=9070
+  _THIRDACCOUNTBINDINFOREQ._serialized_end=9095
+  _THIRDACCOUNTBINDINFORES._serialized_start=9097
+  _THIRDACCOUNTBINDINFORES._serialized_end=9177
+  _BINDTHIRDACCOUNTREQ._serialized_start=9179
+  _BINDTHIRDACCOUNTREQ._serialized_end=9303
+  _BINDTHIRDACCOUNTRES._serialized_start=9305
+  _BINDTHIRDACCOUNTRES._serialized_end=9326
+  _UNBINDTHIRDACCOUNTREQ._serialized_start=9328
+  _UNBINDTHIRDACCOUNTREQ._serialized_end=9424
+  _UNBINDTHIRDACCOUNTRES._serialized_start=9426
+  _UNBINDTHIRDACCOUNTRES._serialized_end=9449
+  _GETQRCODELOGINCODEREQ._serialized_start=9452
+  _GETQRCODELOGINCODEREQ._serialized_end=9614
+  _GETQRCODELOGINCODERES._serialized_start=9616
+  _GETQRCODELOGINCODERES._serialized_end=9659
+  _QRCODESCANLOGINREQ._serialized_start=9661
+  _QRCODESCANLOGINREQ._serialized_end=9758
+  _QRCODESCANLOGINRES._serialized_start=9760
+  _QRCODESCANLOGINRES._serialized_end=9780
+  _GETQRCODELOGINSTATUSREQ._serialized_start=9782
+  _GETQRCODELOGINSTATUSREQ._serialized_end=9872
+  _GETQRCODELOGINSTATUSRES._serialized_start=9875
+  _GETQRCODELOGINSTATUSRES._serialized_end=10043
+  _SETQRCODELOGINSTATUSREQ._serialized_start=10046
+  _SETQRCODELOGINSTATUSREQ._serialized_end=10232
+  _SETQRCODELOGINSTATUSRES._serialized_start=10234
+  _SETQRCODELOGINSTATUSRES._serialized_end=10259
+  _GETACCOUNTREGISTERSTATUSREQ._serialized_start=10261
+  _GETACCOUNTREGISTERSTATUSREQ._serialized_end=10381
+  _GETACCOUNTREGISTERSTATUSRES._serialized_start=10383
+  _GETACCOUNTREGISTERSTATUSRES._serialized_end=10434
+  _GETUMENGPHONEREQ._serialized_start=10436
+  _GETUMENGPHONEREQ._serialized_end=10486
+  _GETUMENGPHONERES._serialized_start=10488
+  _GETUMENGPHONERES._serialized_end=10521
+  _ACCOUNTCROSSTYPEINFO._serialized_start=10523
+  _ACCOUNTCROSSTYPEINFO._serialized_end=10596
+  _ACCOUNTCROSSTYPEINFOREQ._serialized_start=10598
+  _ACCOUNTCROSSTYPEINFOREQ._serialized_end=10623
+  _ACCOUNTCROSSTYPEINFORES._serialized_start=10625
+  _ACCOUNTCROSSTYPEINFORES._serialized_end=10701
+  _APPLYACCOUNTCROSSTYPEREQ._serialized_start=10703
+  _APPLYACCOUNTCROSSTYPEREQ._serialized_end=10729
+  _APPLYACCOUNTCROSSTYPERES._serialized_start=10731
+  _APPLYACCOUNTCROSSTYPERES._serialized_end=10757
+  _CHECKINAPPCHARGELIMITREQ._serialized_start=10759
+  _CHECKINAPPCHARGELIMITREQ._serialized_end=10831
+  _CHECKINAPPCHARGELIMITRES._serialized_start=10833
+  _CHECKINAPPCHARGELIMITRES._serialized_end=10879
+  _GETALIPAYMINIORDERREQ._serialized_start=10882
+  _GETALIPAYMINIORDERREQ._serialized_end=11162
+  _GETALIPAYMINIORDERREQ_EXTENDSENTRY._serialized_start=1365
+  _GETALIPAYMINIORDERREQ_EXTENDSENTRY._serialized_end=1411
+  _GETALIPAYMINIORDERRES._serialized_start=11164
+  _GETALIPAYMINIORDERRES._serialized_end=11205
+  _GETGOODSLISTREQ._serialized_start=11207
+  _GETGOODSLISTREQ._serialized_end=11240
+  _GETGOODSLISTRES._serialized_start=11242
+  _GETGOODSLISTRES._serialized_end=11304
+  _ALIPAYMINIINDEXITEM._serialized_start=11307
+  _ALIPAYMINIINDEXITEM._serialized_end=11489
+  _ALIPAYMINIINDEXBANNER._serialized_start=11491
+  _ALIPAYMINIINDEXBANNER._serialized_end=11534
+  _ALIPAYMINIINDEXGOODSLIST._serialized_start=11536
+  _ALIPAYMINIINDEXGOODSLIST._serialized_end=11618
+  _ALIPAYMINIINDEXGOODSITEM._serialized_start=11621
+  _ALIPAYMINIINDEXGOODSITEM._serialized_end=11794
+  _UAUTHEXTOBJ._serialized_start=13788
+  _UAUTHEXTOBJ._serialized_end=19830
+# @@protoc_insertion_point(module_scope)
```

### Comparing `mecord-cli-0.1.90/mecord/upload.py` & `mecord-cli-0.1.91/mecord/upload.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/user_status_ext_pb2.py` & `mecord-cli-0.1.91/mecord/user_status_ext_pb2.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,220 +1,220 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: user_status_ext.proto
-"""Generated protocol buffer code."""
-from google.protobuf.internal import enum_type_wrapper
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
-from google.protobuf import symbol_database as _symbol_database
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from mecord import common_ext_pb2 as common__ext__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15user_status_ext.proto\x12\x02pb\x1a\x10\x63ommon_ext.proto\"a\n\x08LoginReq\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\ndeviceType\x18\x02 \x01(\x0e\x32\x0e.pb.DeviceType\x12\x10\n\x08\x64\x65viceId\x18\x03 \x01(\t\x12\x12\n\npush_token\x18\x04 \x01(\t\"\x1e\n\x08LoginRes\x12\x12\n\naccount_id\x18\x01 \x01(\x12\"_\n\x10\x42roadcastRelogin\x12\x10\n\x08\x64\x65viceId\x18\x01 \x01(\t\x12#\n\x0b\x64\x65vice_type\x18\x02 \x01(\x0e\x32\x0e.pb.DeviceType\x12\x14\n\x0cmulti_client\x18\x03 \x01(\x08\"5\n\x12\x42roadcastTakeLeave\x12\x12\n\naccount_id\x18\x01 \x01(\x12\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\x7f\n\x1b\x42roadcastDeviceDisconnected\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12#\n\x0b\x64\x65vice_type\x18\x02 \x01(\x0e\x32\x0e.pb.DeviceType\x12(\n\x06reason\x18\x03 \x01(\x0e\x32\x18.pb.DisconnectReasonType\"?\n\tLogoutReq\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x11\n\taccountId\x18\x02 \x01(\x03\x12\x12\n\ndeviceCode\x18\x03 \x01(\x03\"\x0b\n\tLogoutRes\"/\n\rDisconnectReq\x12\x0e\n\x06\x63onnId\x18\x01 \x01(\x12\x12\x0e\n\x06userId\x18\x02 \x01(\x12\"\x0f\n\rDisconnectRes\"\x14\n\x12UserConInfoListReq\"3\n\x12UserConInfoListRes\x12\x1d\n\x04list\x18\x01 \x03(\x0b\x32\x0f.pb.UserConInfo\"\x97\x01\n\x0bUserConInfo\x12\n\n\x02id\x18\x01 \x01(\x12\x12\n\n\x02ip\x18\x02 \x01(\t\x12#\n\x0b\x64\x65vice_type\x18\x03 \x01(\x0e\x32\x0e.pb.DeviceType\x12\x11\n\tdevice_id\x18\x04 \x01(\t\x12\x10\n\x08\x64ie_time\x18\x05 \x01(\x12\x12\x11\n\tplayer_id\x18\x06 \x01(\x12\x12\x13\n\x0b\x63reate_time\x18\x07 \x01(\x12\"S\n\x19UserDeviceDisconnectedReq\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12#\n\x0b\x64\x65vice_type\x18\x02 \x01(\x0e\x32\x0e.pb.DeviceType\"\x1b\n\x19UserDeviceDisconnectedRes\"f\n\x1bNotifyDeviceDisconnectedReq\x12\x10\n\x08phone_no\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\x12&\n\x04type\x18\x03 \x01(\x0e\x32\x18.pb.DisconnectReasonType\"\x1d\n\x1bNotifyDeviceDisconnectedRes*\xdc\x01\n\rUserStatusErr\x12\x15\n\x11UserStatusSUCCESS\x10\x00\x12\x1d\n\x17\x45rrUserStatusKeyExpired\x10\x89\xa1\x02\x12\x1d\n\x17\x45rrUserStatusBanAccount\x10\x8a\xa1\x02\x12\x18\n\x12\x45rrUserStatusBanIp\x10\x8b\xa1\x02\x12\x1a\n\x14\x45rrUserStatusRelogin\x10\x8c\xa1\x02\x12\x1c\n\x16\x45rrUserStatusTakeLeave\x10\x8d\xa1\x02\x12\"\n\x1c\x45rrUserStatusAccountDeleting\x10\x92\xa1\x02*\x89\x01\n\x0fUserStatusCmdId\x12\x15\n\x11UC_UserStatusZero\x10\x00\x12\x1a\n\x14UC_UserStatusRelogin\x10\x89\xca\x1e\x12\x1c\n\x16UC_UserStatusTakeLeave\x10\x8a\xca\x1e\x12%\n\x1fUC_UserStatusDeviceDisconnected\x10\x8b\xca\x1e*\x98\x01\n\x14\x44isconnectReasonType\x12\x0c\n\x08\x44RT_None\x10\x00\x12\x14\n\x10\x44RT_RefreshState\x10\x01\x12\x14\n\x10\x44RT_RemoveDevice\x10\x02\x12\x0b\n\x07\x44RT_Ban\x10\x03\x12\x12\n\x0e\x44RT_DelAccount\x10\x04\x12\x11\n\rDRT_ResetPass\x10\x05\x12\x12\n\x0e\x44RT_ModifyPass\x10\x06\x32\xc6\x03\n\x10UserStatusExtObj\x12#\n\x05Login\x12\x0c.pb.LoginReq\x1a\x0c.pb.LoginRes\x12&\n\x06Logout\x12\r.pb.LogoutReq\x1a\r.pb.LogoutRes\x12\x38\n\x10NotifyDisConnect\x12\x11.pb.DisconnectReq\x1a\x11.pb.DisconnectRes\x12/\n\tHeartbeat\x12\x10.pb.HeartbeatReq\x1a\x10.pb.HeartbeatRes\x12\x41\n\x0fUserConInfoList\x12\x16.pb.UserConInfoListReq\x1a\x16.pb.UserConInfoListRes\x12V\n\x16UserDeviceDisconnected\x12\x1d.pb.UserDeviceDisconnectedReq\x1a\x1d.pb.UserDeviceDisconnectedRes\x12_\n\x1bGetNotifyDeviceDisconnected\x12\x1f.pb.NotifyDeviceDisconnectedReq\x1a\x1f.pb.NotifyDeviceDisconnectedResB\x06\xa2\x02\x03PB3b\x06proto3')
-
-_USERSTATUSERR = DESCRIPTOR.enum_types_by_name['UserStatusErr']
-UserStatusErr = enum_type_wrapper.EnumTypeWrapper(_USERSTATUSERR)
-_USERSTATUSCMDID = DESCRIPTOR.enum_types_by_name['UserStatusCmdId']
-UserStatusCmdId = enum_type_wrapper.EnumTypeWrapper(_USERSTATUSCMDID)
-_DISCONNECTREASONTYPE = DESCRIPTOR.enum_types_by_name['DisconnectReasonType']
-DisconnectReasonType = enum_type_wrapper.EnumTypeWrapper(_DISCONNECTREASONTYPE)
-UserStatusSUCCESS = 0
-ErrUserStatusKeyExpired = 37001
-ErrUserStatusBanAccount = 37002
-ErrUserStatusBanIp = 37003
-ErrUserStatusRelogin = 37004
-ErrUserStatusTakeLeave = 37005
-ErrUserStatusAccountDeleting = 37010
-UC_UserStatusZero = 0
-UC_UserStatusRelogin = 501001
-UC_UserStatusTakeLeave = 501002
-UC_UserStatusDeviceDisconnected = 501003
-DRT_None = 0
-DRT_RefreshState = 1
-DRT_RemoveDevice = 2
-DRT_Ban = 3
-DRT_DelAccount = 4
-DRT_ResetPass = 5
-DRT_ModifyPass = 6
-
-
-_LOGINREQ = DESCRIPTOR.message_types_by_name['LoginReq']
-_LOGINRES = DESCRIPTOR.message_types_by_name['LoginRes']
-_BROADCASTRELOGIN = DESCRIPTOR.message_types_by_name['BroadcastRelogin']
-_BROADCASTTAKELEAVE = DESCRIPTOR.message_types_by_name['BroadcastTakeLeave']
-_BROADCASTDEVICEDISCONNECTED = DESCRIPTOR.message_types_by_name['BroadcastDeviceDisconnected']
-_LOGOUTREQ = DESCRIPTOR.message_types_by_name['LogoutReq']
-_LOGOUTRES = DESCRIPTOR.message_types_by_name['LogoutRes']
-_DISCONNECTREQ = DESCRIPTOR.message_types_by_name['DisconnectReq']
-_DISCONNECTRES = DESCRIPTOR.message_types_by_name['DisconnectRes']
-_USERCONINFOLISTREQ = DESCRIPTOR.message_types_by_name['UserConInfoListReq']
-_USERCONINFOLISTRES = DESCRIPTOR.message_types_by_name['UserConInfoListRes']
-_USERCONINFO = DESCRIPTOR.message_types_by_name['UserConInfo']
-_USERDEVICEDISCONNECTEDREQ = DESCRIPTOR.message_types_by_name['UserDeviceDisconnectedReq']
-_USERDEVICEDISCONNECTEDRES = DESCRIPTOR.message_types_by_name['UserDeviceDisconnectedRes']
-_NOTIFYDEVICEDISCONNECTEDREQ = DESCRIPTOR.message_types_by_name['NotifyDeviceDisconnectedReq']
-_NOTIFYDEVICEDISCONNECTEDRES = DESCRIPTOR.message_types_by_name['NotifyDeviceDisconnectedRes']
-LoginReq = _reflection.GeneratedProtocolMessageType('LoginReq', (_message.Message,), {
-  'DESCRIPTOR' : _LOGINREQ,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.LoginReq)
-  })
-_sym_db.RegisterMessage(LoginReq)
-
-LoginRes = _reflection.GeneratedProtocolMessageType('LoginRes', (_message.Message,), {
-  'DESCRIPTOR' : _LOGINRES,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.LoginRes)
-  })
-_sym_db.RegisterMessage(LoginRes)
-
-BroadcastRelogin = _reflection.GeneratedProtocolMessageType('BroadcastRelogin', (_message.Message,), {
-  'DESCRIPTOR' : _BROADCASTRELOGIN,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.BroadcastRelogin)
-  })
-_sym_db.RegisterMessage(BroadcastRelogin)
-
-BroadcastTakeLeave = _reflection.GeneratedProtocolMessageType('BroadcastTakeLeave', (_message.Message,), {
-  'DESCRIPTOR' : _BROADCASTTAKELEAVE,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.BroadcastTakeLeave)
-  })
-_sym_db.RegisterMessage(BroadcastTakeLeave)
-
-BroadcastDeviceDisconnected = _reflection.GeneratedProtocolMessageType('BroadcastDeviceDisconnected', (_message.Message,), {
-  'DESCRIPTOR' : _BROADCASTDEVICEDISCONNECTED,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.BroadcastDeviceDisconnected)
-  })
-_sym_db.RegisterMessage(BroadcastDeviceDisconnected)
-
-LogoutReq = _reflection.GeneratedProtocolMessageType('LogoutReq', (_message.Message,), {
-  'DESCRIPTOR' : _LOGOUTREQ,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.LogoutReq)
-  })
-_sym_db.RegisterMessage(LogoutReq)
-
-LogoutRes = _reflection.GeneratedProtocolMessageType('LogoutRes', (_message.Message,), {
-  'DESCRIPTOR' : _LOGOUTRES,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.LogoutRes)
-  })
-_sym_db.RegisterMessage(LogoutRes)
-
-DisconnectReq = _reflection.GeneratedProtocolMessageType('DisconnectReq', (_message.Message,), {
-  'DESCRIPTOR' : _DISCONNECTREQ,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.DisconnectReq)
-  })
-_sym_db.RegisterMessage(DisconnectReq)
-
-DisconnectRes = _reflection.GeneratedProtocolMessageType('DisconnectRes', (_message.Message,), {
-  'DESCRIPTOR' : _DISCONNECTRES,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.DisconnectRes)
-  })
-_sym_db.RegisterMessage(DisconnectRes)
-
-UserConInfoListReq = _reflection.GeneratedProtocolMessageType('UserConInfoListReq', (_message.Message,), {
-  'DESCRIPTOR' : _USERCONINFOLISTREQ,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UserConInfoListReq)
-  })
-_sym_db.RegisterMessage(UserConInfoListReq)
-
-UserConInfoListRes = _reflection.GeneratedProtocolMessageType('UserConInfoListRes', (_message.Message,), {
-  'DESCRIPTOR' : _USERCONINFOLISTRES,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UserConInfoListRes)
-  })
-_sym_db.RegisterMessage(UserConInfoListRes)
-
-UserConInfo = _reflection.GeneratedProtocolMessageType('UserConInfo', (_message.Message,), {
-  'DESCRIPTOR' : _USERCONINFO,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UserConInfo)
-  })
-_sym_db.RegisterMessage(UserConInfo)
-
-UserDeviceDisconnectedReq = _reflection.GeneratedProtocolMessageType('UserDeviceDisconnectedReq', (_message.Message,), {
-  'DESCRIPTOR' : _USERDEVICEDISCONNECTEDREQ,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UserDeviceDisconnectedReq)
-  })
-_sym_db.RegisterMessage(UserDeviceDisconnectedReq)
-
-UserDeviceDisconnectedRes = _reflection.GeneratedProtocolMessageType('UserDeviceDisconnectedRes', (_message.Message,), {
-  'DESCRIPTOR' : _USERDEVICEDISCONNECTEDRES,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.UserDeviceDisconnectedRes)
-  })
-_sym_db.RegisterMessage(UserDeviceDisconnectedRes)
-
-NotifyDeviceDisconnectedReq = _reflection.GeneratedProtocolMessageType('NotifyDeviceDisconnectedReq', (_message.Message,), {
-  'DESCRIPTOR' : _NOTIFYDEVICEDISCONNECTEDREQ,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.NotifyDeviceDisconnectedReq)
-  })
-_sym_db.RegisterMessage(NotifyDeviceDisconnectedReq)
-
-NotifyDeviceDisconnectedRes = _reflection.GeneratedProtocolMessageType('NotifyDeviceDisconnectedRes', (_message.Message,), {
-  'DESCRIPTOR' : _NOTIFYDEVICEDISCONNECTEDRES,
-  '__module__' : 'user_status_ext_pb2'
-  # @@protoc_insertion_point(class_scope:pb.NotifyDeviceDisconnectedRes)
-  })
-_sym_db.RegisterMessage(NotifyDeviceDisconnectedRes)
-
-_USERSTATUSEXTOBJ = DESCRIPTOR.services_by_name['UserStatusExtObj']
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\242\002\003PB3'
-  _USERSTATUSERR._serialized_start=1082
-  _USERSTATUSERR._serialized_end=1302
-  _USERSTATUSCMDID._serialized_start=1305
-  _USERSTATUSCMDID._serialized_end=1442
-  _DISCONNECTREASONTYPE._serialized_start=1445
-  _DISCONNECTREASONTYPE._serialized_end=1597
-  _LOGINREQ._serialized_start=47
-  _LOGINREQ._serialized_end=144
-  _LOGINRES._serialized_start=146
-  _LOGINRES._serialized_end=176
-  _BROADCASTRELOGIN._serialized_start=178
-  _BROADCASTRELOGIN._serialized_end=273
-  _BROADCASTTAKELEAVE._serialized_start=275
-  _BROADCASTTAKELEAVE._serialized_end=328
-  _BROADCASTDEVICEDISCONNECTED._serialized_start=330
-  _BROADCASTDEVICEDISCONNECTED._serialized_end=457
-  _LOGOUTREQ._serialized_start=459
-  _LOGOUTREQ._serialized_end=522
-  _LOGOUTRES._serialized_start=524
-  _LOGOUTRES._serialized_end=535
-  _DISCONNECTREQ._serialized_start=537
-  _DISCONNECTREQ._serialized_end=584
-  _DISCONNECTRES._serialized_start=586
-  _DISCONNECTRES._serialized_end=601
-  _USERCONINFOLISTREQ._serialized_start=603
-  _USERCONINFOLISTREQ._serialized_end=623
-  _USERCONINFOLISTRES._serialized_start=625
-  _USERCONINFOLISTRES._serialized_end=676
-  _USERCONINFO._serialized_start=679
-  _USERCONINFO._serialized_end=830
-  _USERDEVICEDISCONNECTEDREQ._serialized_start=832
-  _USERDEVICEDISCONNECTEDREQ._serialized_end=915
-  _USERDEVICEDISCONNECTEDRES._serialized_start=917
-  _USERDEVICEDISCONNECTEDRES._serialized_end=944
-  _NOTIFYDEVICEDISCONNECTEDREQ._serialized_start=946
-  _NOTIFYDEVICEDISCONNECTEDREQ._serialized_end=1048
-  _NOTIFYDEVICEDISCONNECTEDRES._serialized_start=1050
-  _NOTIFYDEVICEDISCONNECTEDRES._serialized_end=1079
-  _USERSTATUSEXTOBJ._serialized_start=1600
-  _USERSTATUSEXTOBJ._serialized_end=2054
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: user_status_ext.proto
+"""Generated protocol buffer code."""
+from google.protobuf.internal import enum_type_wrapper
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import message as _message
+from google.protobuf import reflection as _reflection
+from google.protobuf import symbol_database as _symbol_database
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from mecord import common_ext_pb2 as common__ext__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15user_status_ext.proto\x12\x02pb\x1a\x10\x63ommon_ext.proto\"a\n\x08LoginReq\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\"\n\ndeviceType\x18\x02 \x01(\x0e\x32\x0e.pb.DeviceType\x12\x10\n\x08\x64\x65viceId\x18\x03 \x01(\t\x12\x12\n\npush_token\x18\x04 \x01(\t\"\x1e\n\x08LoginRes\x12\x12\n\naccount_id\x18\x01 \x01(\x12\"_\n\x10\x42roadcastRelogin\x12\x10\n\x08\x64\x65viceId\x18\x01 \x01(\t\x12#\n\x0b\x64\x65vice_type\x18\x02 \x01(\x0e\x32\x0e.pb.DeviceType\x12\x14\n\x0cmulti_client\x18\x03 \x01(\x08\"5\n\x12\x42roadcastTakeLeave\x12\x12\n\naccount_id\x18\x01 \x01(\x12\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\x7f\n\x1b\x42roadcastDeviceDisconnected\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12#\n\x0b\x64\x65vice_type\x18\x02 \x01(\x0e\x32\x0e.pb.DeviceType\x12(\n\x06reason\x18\x03 \x01(\x0e\x32\x18.pb.DisconnectReasonType\"?\n\tLogoutReq\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x11\n\taccountId\x18\x02 \x01(\x03\x12\x12\n\ndeviceCode\x18\x03 \x01(\x03\"\x0b\n\tLogoutRes\"/\n\rDisconnectReq\x12\x0e\n\x06\x63onnId\x18\x01 \x01(\x12\x12\x0e\n\x06userId\x18\x02 \x01(\x12\"\x0f\n\rDisconnectRes\"\x14\n\x12UserConInfoListReq\"3\n\x12UserConInfoListRes\x12\x1d\n\x04list\x18\x01 \x03(\x0b\x32\x0f.pb.UserConInfo\"\x97\x01\n\x0bUserConInfo\x12\n\n\x02id\x18\x01 \x01(\x12\x12\n\n\x02ip\x18\x02 \x01(\t\x12#\n\x0b\x64\x65vice_type\x18\x03 \x01(\x0e\x32\x0e.pb.DeviceType\x12\x11\n\tdevice_id\x18\x04 \x01(\t\x12\x10\n\x08\x64ie_time\x18\x05 \x01(\x12\x12\x11\n\tplayer_id\x18\x06 \x01(\x12\x12\x13\n\x0b\x63reate_time\x18\x07 \x01(\x12\"S\n\x19UserDeviceDisconnectedReq\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12#\n\x0b\x64\x65vice_type\x18\x02 \x01(\x0e\x32\x0e.pb.DeviceType\"\x1b\n\x19UserDeviceDisconnectedRes\"f\n\x1bNotifyDeviceDisconnectedReq\x12\x10\n\x08phone_no\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\x12&\n\x04type\x18\x03 \x01(\x0e\x32\x18.pb.DisconnectReasonType\"\x1d\n\x1bNotifyDeviceDisconnectedRes*\xdc\x01\n\rUserStatusErr\x12\x15\n\x11UserStatusSUCCESS\x10\x00\x12\x1d\n\x17\x45rrUserStatusKeyExpired\x10\x89\xa1\x02\x12\x1d\n\x17\x45rrUserStatusBanAccount\x10\x8a\xa1\x02\x12\x18\n\x12\x45rrUserStatusBanIp\x10\x8b\xa1\x02\x12\x1a\n\x14\x45rrUserStatusRelogin\x10\x8c\xa1\x02\x12\x1c\n\x16\x45rrUserStatusTakeLeave\x10\x8d\xa1\x02\x12\"\n\x1c\x45rrUserStatusAccountDeleting\x10\x92\xa1\x02*\x89\x01\n\x0fUserStatusCmdId\x12\x15\n\x11UC_UserStatusZero\x10\x00\x12\x1a\n\x14UC_UserStatusRelogin\x10\x89\xca\x1e\x12\x1c\n\x16UC_UserStatusTakeLeave\x10\x8a\xca\x1e\x12%\n\x1fUC_UserStatusDeviceDisconnected\x10\x8b\xca\x1e*\x98\x01\n\x14\x44isconnectReasonType\x12\x0c\n\x08\x44RT_None\x10\x00\x12\x14\n\x10\x44RT_RefreshState\x10\x01\x12\x14\n\x10\x44RT_RemoveDevice\x10\x02\x12\x0b\n\x07\x44RT_Ban\x10\x03\x12\x12\n\x0e\x44RT_DelAccount\x10\x04\x12\x11\n\rDRT_ResetPass\x10\x05\x12\x12\n\x0e\x44RT_ModifyPass\x10\x06\x32\xc6\x03\n\x10UserStatusExtObj\x12#\n\x05Login\x12\x0c.pb.LoginReq\x1a\x0c.pb.LoginRes\x12&\n\x06Logout\x12\r.pb.LogoutReq\x1a\r.pb.LogoutRes\x12\x38\n\x10NotifyDisConnect\x12\x11.pb.DisconnectReq\x1a\x11.pb.DisconnectRes\x12/\n\tHeartbeat\x12\x10.pb.HeartbeatReq\x1a\x10.pb.HeartbeatRes\x12\x41\n\x0fUserConInfoList\x12\x16.pb.UserConInfoListReq\x1a\x16.pb.UserConInfoListRes\x12V\n\x16UserDeviceDisconnected\x12\x1d.pb.UserDeviceDisconnectedReq\x1a\x1d.pb.UserDeviceDisconnectedRes\x12_\n\x1bGetNotifyDeviceDisconnected\x12\x1f.pb.NotifyDeviceDisconnectedReq\x1a\x1f.pb.NotifyDeviceDisconnectedResB\x06\xa2\x02\x03PB3b\x06proto3')
+
+_USERSTATUSERR = DESCRIPTOR.enum_types_by_name['UserStatusErr']
+UserStatusErr = enum_type_wrapper.EnumTypeWrapper(_USERSTATUSERR)
+_USERSTATUSCMDID = DESCRIPTOR.enum_types_by_name['UserStatusCmdId']
+UserStatusCmdId = enum_type_wrapper.EnumTypeWrapper(_USERSTATUSCMDID)
+_DISCONNECTREASONTYPE = DESCRIPTOR.enum_types_by_name['DisconnectReasonType']
+DisconnectReasonType = enum_type_wrapper.EnumTypeWrapper(_DISCONNECTREASONTYPE)
+UserStatusSUCCESS = 0
+ErrUserStatusKeyExpired = 37001
+ErrUserStatusBanAccount = 37002
+ErrUserStatusBanIp = 37003
+ErrUserStatusRelogin = 37004
+ErrUserStatusTakeLeave = 37005
+ErrUserStatusAccountDeleting = 37010
+UC_UserStatusZero = 0
+UC_UserStatusRelogin = 501001
+UC_UserStatusTakeLeave = 501002
+UC_UserStatusDeviceDisconnected = 501003
+DRT_None = 0
+DRT_RefreshState = 1
+DRT_RemoveDevice = 2
+DRT_Ban = 3
+DRT_DelAccount = 4
+DRT_ResetPass = 5
+DRT_ModifyPass = 6
+
+
+_LOGINREQ = DESCRIPTOR.message_types_by_name['LoginReq']
+_LOGINRES = DESCRIPTOR.message_types_by_name['LoginRes']
+_BROADCASTRELOGIN = DESCRIPTOR.message_types_by_name['BroadcastRelogin']
+_BROADCASTTAKELEAVE = DESCRIPTOR.message_types_by_name['BroadcastTakeLeave']
+_BROADCASTDEVICEDISCONNECTED = DESCRIPTOR.message_types_by_name['BroadcastDeviceDisconnected']
+_LOGOUTREQ = DESCRIPTOR.message_types_by_name['LogoutReq']
+_LOGOUTRES = DESCRIPTOR.message_types_by_name['LogoutRes']
+_DISCONNECTREQ = DESCRIPTOR.message_types_by_name['DisconnectReq']
+_DISCONNECTRES = DESCRIPTOR.message_types_by_name['DisconnectRes']
+_USERCONINFOLISTREQ = DESCRIPTOR.message_types_by_name['UserConInfoListReq']
+_USERCONINFOLISTRES = DESCRIPTOR.message_types_by_name['UserConInfoListRes']
+_USERCONINFO = DESCRIPTOR.message_types_by_name['UserConInfo']
+_USERDEVICEDISCONNECTEDREQ = DESCRIPTOR.message_types_by_name['UserDeviceDisconnectedReq']
+_USERDEVICEDISCONNECTEDRES = DESCRIPTOR.message_types_by_name['UserDeviceDisconnectedRes']
+_NOTIFYDEVICEDISCONNECTEDREQ = DESCRIPTOR.message_types_by_name['NotifyDeviceDisconnectedReq']
+_NOTIFYDEVICEDISCONNECTEDRES = DESCRIPTOR.message_types_by_name['NotifyDeviceDisconnectedRes']
+LoginReq = _reflection.GeneratedProtocolMessageType('LoginReq', (_message.Message,), {
+  'DESCRIPTOR' : _LOGINREQ,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.LoginReq)
+  })
+_sym_db.RegisterMessage(LoginReq)
+
+LoginRes = _reflection.GeneratedProtocolMessageType('LoginRes', (_message.Message,), {
+  'DESCRIPTOR' : _LOGINRES,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.LoginRes)
+  })
+_sym_db.RegisterMessage(LoginRes)
+
+BroadcastRelogin = _reflection.GeneratedProtocolMessageType('BroadcastRelogin', (_message.Message,), {
+  'DESCRIPTOR' : _BROADCASTRELOGIN,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.BroadcastRelogin)
+  })
+_sym_db.RegisterMessage(BroadcastRelogin)
+
+BroadcastTakeLeave = _reflection.GeneratedProtocolMessageType('BroadcastTakeLeave', (_message.Message,), {
+  'DESCRIPTOR' : _BROADCASTTAKELEAVE,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.BroadcastTakeLeave)
+  })
+_sym_db.RegisterMessage(BroadcastTakeLeave)
+
+BroadcastDeviceDisconnected = _reflection.GeneratedProtocolMessageType('BroadcastDeviceDisconnected', (_message.Message,), {
+  'DESCRIPTOR' : _BROADCASTDEVICEDISCONNECTED,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.BroadcastDeviceDisconnected)
+  })
+_sym_db.RegisterMessage(BroadcastDeviceDisconnected)
+
+LogoutReq = _reflection.GeneratedProtocolMessageType('LogoutReq', (_message.Message,), {
+  'DESCRIPTOR' : _LOGOUTREQ,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.LogoutReq)
+  })
+_sym_db.RegisterMessage(LogoutReq)
+
+LogoutRes = _reflection.GeneratedProtocolMessageType('LogoutRes', (_message.Message,), {
+  'DESCRIPTOR' : _LOGOUTRES,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.LogoutRes)
+  })
+_sym_db.RegisterMessage(LogoutRes)
+
+DisconnectReq = _reflection.GeneratedProtocolMessageType('DisconnectReq', (_message.Message,), {
+  'DESCRIPTOR' : _DISCONNECTREQ,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.DisconnectReq)
+  })
+_sym_db.RegisterMessage(DisconnectReq)
+
+DisconnectRes = _reflection.GeneratedProtocolMessageType('DisconnectRes', (_message.Message,), {
+  'DESCRIPTOR' : _DISCONNECTRES,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.DisconnectRes)
+  })
+_sym_db.RegisterMessage(DisconnectRes)
+
+UserConInfoListReq = _reflection.GeneratedProtocolMessageType('UserConInfoListReq', (_message.Message,), {
+  'DESCRIPTOR' : _USERCONINFOLISTREQ,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UserConInfoListReq)
+  })
+_sym_db.RegisterMessage(UserConInfoListReq)
+
+UserConInfoListRes = _reflection.GeneratedProtocolMessageType('UserConInfoListRes', (_message.Message,), {
+  'DESCRIPTOR' : _USERCONINFOLISTRES,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UserConInfoListRes)
+  })
+_sym_db.RegisterMessage(UserConInfoListRes)
+
+UserConInfo = _reflection.GeneratedProtocolMessageType('UserConInfo', (_message.Message,), {
+  'DESCRIPTOR' : _USERCONINFO,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UserConInfo)
+  })
+_sym_db.RegisterMessage(UserConInfo)
+
+UserDeviceDisconnectedReq = _reflection.GeneratedProtocolMessageType('UserDeviceDisconnectedReq', (_message.Message,), {
+  'DESCRIPTOR' : _USERDEVICEDISCONNECTEDREQ,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UserDeviceDisconnectedReq)
+  })
+_sym_db.RegisterMessage(UserDeviceDisconnectedReq)
+
+UserDeviceDisconnectedRes = _reflection.GeneratedProtocolMessageType('UserDeviceDisconnectedRes', (_message.Message,), {
+  'DESCRIPTOR' : _USERDEVICEDISCONNECTEDRES,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.UserDeviceDisconnectedRes)
+  })
+_sym_db.RegisterMessage(UserDeviceDisconnectedRes)
+
+NotifyDeviceDisconnectedReq = _reflection.GeneratedProtocolMessageType('NotifyDeviceDisconnectedReq', (_message.Message,), {
+  'DESCRIPTOR' : _NOTIFYDEVICEDISCONNECTEDREQ,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.NotifyDeviceDisconnectedReq)
+  })
+_sym_db.RegisterMessage(NotifyDeviceDisconnectedReq)
+
+NotifyDeviceDisconnectedRes = _reflection.GeneratedProtocolMessageType('NotifyDeviceDisconnectedRes', (_message.Message,), {
+  'DESCRIPTOR' : _NOTIFYDEVICEDISCONNECTEDRES,
+  '__module__' : 'user_status_ext_pb2'
+  # @@protoc_insertion_point(class_scope:pb.NotifyDeviceDisconnectedRes)
+  })
+_sym_db.RegisterMessage(NotifyDeviceDisconnectedRes)
+
+_USERSTATUSEXTOBJ = DESCRIPTOR.services_by_name['UserStatusExtObj']
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\242\002\003PB3'
+  _USERSTATUSERR._serialized_start=1082
+  _USERSTATUSERR._serialized_end=1302
+  _USERSTATUSCMDID._serialized_start=1305
+  _USERSTATUSCMDID._serialized_end=1442
+  _DISCONNECTREASONTYPE._serialized_start=1445
+  _DISCONNECTREASONTYPE._serialized_end=1597
+  _LOGINREQ._serialized_start=47
+  _LOGINREQ._serialized_end=144
+  _LOGINRES._serialized_start=146
+  _LOGINRES._serialized_end=176
+  _BROADCASTRELOGIN._serialized_start=178
+  _BROADCASTRELOGIN._serialized_end=273
+  _BROADCASTTAKELEAVE._serialized_start=275
+  _BROADCASTTAKELEAVE._serialized_end=328
+  _BROADCASTDEVICEDISCONNECTED._serialized_start=330
+  _BROADCASTDEVICEDISCONNECTED._serialized_end=457
+  _LOGOUTREQ._serialized_start=459
+  _LOGOUTREQ._serialized_end=522
+  _LOGOUTRES._serialized_start=524
+  _LOGOUTRES._serialized_end=535
+  _DISCONNECTREQ._serialized_start=537
+  _DISCONNECTREQ._serialized_end=584
+  _DISCONNECTRES._serialized_start=586
+  _DISCONNECTRES._serialized_end=601
+  _USERCONINFOLISTREQ._serialized_start=603
+  _USERCONINFOLISTREQ._serialized_end=623
+  _USERCONINFOLISTRES._serialized_start=625
+  _USERCONINFOLISTRES._serialized_end=676
+  _USERCONINFO._serialized_start=679
+  _USERCONINFO._serialized_end=830
+  _USERDEVICEDISCONNECTEDREQ._serialized_start=832
+  _USERDEVICEDISCONNECTEDREQ._serialized_end=915
+  _USERDEVICEDISCONNECTEDRES._serialized_start=917
+  _USERDEVICEDISCONNECTEDRES._serialized_end=944
+  _NOTIFYDEVICEDISCONNECTEDREQ._serialized_start=946
+  _NOTIFYDEVICEDISCONNECTEDREQ._serialized_end=1048
+  _NOTIFYDEVICEDISCONNECTEDRES._serialized_start=1050
+  _NOTIFYDEVICEDISCONNECTEDRES._serialized_end=1079
+  _USERSTATUSEXTOBJ._serialized_start=1600
+  _USERSTATUSEXTOBJ._serialized_end=2054
+# @@protoc_insertion_point(module_scope)
```

### Comparing `mecord-cli-0.1.90/mecord/utils.py` & `mecord-cli-0.1.91/mecord/utils.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/widget_template/MekongJS.js.py` & `mecord-cli-0.1.91/mecord/widget_template/MekongJS.js.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/widget_template/icon.png.py` & `mecord-cli-0.1.91/mecord/widget_template/icon.png.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/widget_template/index.html.py` & `mecord-cli-0.1.91/mecord/widget_template/index.html.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/xy_pb.py` & `mecord-cli-0.1.91/mecord/xy_pb.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord/xy_user.py` & `mecord-cli-0.1.91/mecord/xy_user.py`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/mecord_cli.egg-info/PKG-INFO` & `mecord-cli-0.1.91/mecord_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecord-cli
-Version: 0.1.90
+Version: 0.1.91
 Summary: mecord tools
 Home-page: https://github.com/mecordofficial
 Author: pengjun
 Author-email: mr_lonely@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mecord-cli-0.1.90/mecord_cli.egg-info/SOURCES.txt` & `mecord-cli-0.1.91/mecord_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mecord-cli-0.1.90/setup.py` & `mecord-cli-0.1.91/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import setuptools
 import os
 import subprocess
 import datetime
 
-mecord_version = "0.1.90"
+mecord_version = "0.1.91"
+
 mecord_build_number = int(mecord_version.replace(".",""))
 cur_dir = os.path.dirname(os.path.abspath(__file__))
 constanspy = os.path.join(cur_dir, "mecord", "constant.py")
 try:
     result = subprocess.run("git config user.email", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
     build_user = "Noh"
     if result.returncode == 0:
```

