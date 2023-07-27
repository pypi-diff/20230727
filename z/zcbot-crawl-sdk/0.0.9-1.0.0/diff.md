# Comparing `tmp/zcbot-crawl-sdk-0.0.9.tar.gz` & `tmp/zcbot-crawl-sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zcbot-crawl-sdk-0.0.9.tar", last modified: Fri Mar 31 09:03:30 2023, max compression
+gzip compressed data, was "dist\zcbot-crawl-sdk-1.0.0.tar", last modified: Thu Jul 27 01:11:17 2023, max compression
```

## Comparing `zcbot-crawl-sdk-0.0.9.tar` & `zcbot-crawl-sdk-1.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 09:03:30.632575 zcbot-crawl-sdk-0.0.9/
--rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-crawl-sdk-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0      375 2023-03-31 09:03:30.631575 zcbot-crawl-sdk-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      132 2023-03-29 06:37:01.000000 zcbot-crawl-sdk-0.0.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-03-31 09:03:30.632575 zcbot-crawl-sdk-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      610 2023-03-31 09:03:22.000000 zcbot-crawl-sdk-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:03:30.605576 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:03:30.618575 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/
--rw-rw-rw-   0        0        0        0 2022-03-23 07:19:36.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     5011 2023-03-29 06:40:27.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/api.py
--rw-rw-rw-   0        0        0      327 2022-03-23 00:45:58.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/auth.py
--rw-rw-rw-   0        0        0     1245 2022-03-23 07:09:21.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/exceptions.py
--rw-rw-rw-   0        0        0     2128 2023-03-29 06:41:13.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/http_client.py
--rw-rw-rw-   0        0        0     2802 2023-03-29 06:40:15.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/model.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:03:30.626576 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/
--rw-rw-rw-   0        0        0        0 2022-03-23 07:22:16.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/__init__.py
--rw-rw-rw-   0        0        0      317 2022-03-23 08:05:10.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/exceptions.py
--rw-rw-rw-   0        0        0     1039 2023-03-30 11:47:15.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/model.py
--rw-rw-rw-   0        0        0     3557 2023-03-30 12:39:24.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/processor.py
--rw-rw-rw-   0        0        0     1051 2023-03-30 14:41:55.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/rabbit_keys.py
--rw-rw-rw-   0        0        0     9249 2023-03-31 09:02:18.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/receiver.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:03:30.629575 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/util/
--rw-rw-rw-   0        0        0        0 2022-05-27 06:44:19.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/util/__init__.py
--rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/util/decator.py
--rw-rw-rw-   0        0        0     3908 2023-02-28 01:05:14.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/util/time.py
-drwxrwxrwx   0        0        0        0 2023-03-31 09:03:30.611575 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/
--rw-rw-rw-   0        0        0      375 2023-03-31 09:03:30.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      751 2023-03-31 09:03:30.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 09:03:30.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-03-31 09:03:30.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-31 09:03:30.000000 zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 01:11:17.218170 zcbot-crawl-sdk-1.0.0/
+-rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-crawl-sdk-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      375 2023-07-27 01:11:17.217174 zcbot-crawl-sdk-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      132 2023-03-29 06:37:01.000000 zcbot-crawl-sdk-1.0.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-27 01:11:17.218170 zcbot-crawl-sdk-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      610 2023-07-27 01:09:26.000000 zcbot-crawl-sdk-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:11:17.173171 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:11:17.194170 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/api/
+-rw-rw-rw-   0        0        0        0 2022-03-23 07:19:36.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     3173 2023-07-26 14:21:39.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/api/api.py
+-rw-rw-rw-   0        0        0      327 2022-03-23 00:45:58.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/api/auth.py
+-rw-rw-rw-   0        0        0     1245 2022-03-23 07:09:21.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/api/exceptions.py
+-rw-rw-rw-   0        0        0     2128 2023-03-29 06:41:13.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/api/http_client.py
+-rw-rw-rw-   0        0        0     4670 2023-07-26 14:36:48.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/api/model.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:11:17.208174 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/receive/
+-rw-rw-rw-   0        0        0        0 2022-03-23 07:22:16.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/receive/__init__.py
+-rw-rw-rw-   0        0        0      317 2022-03-23 08:05:10.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/receive/exceptions.py
+-rw-rw-rw-   0        0        0     1039 2023-03-30 11:47:15.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/receive/model.py
+-rw-rw-rw-   0        0        0     3695 2023-05-06 01:40:42.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/receive/processor.py
+-rw-rw-rw-   0        0        0     1051 2023-03-30 14:41:55.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/receive/rabbit_keys.py
+-rw-rw-rw-   0        0        0     9249 2023-03-31 09:02:18.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/receive/receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:11:17.215171 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/util/
+-rw-rw-rw-   0        0        0        0 2022-05-27 06:44:19.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0      272 2022-04-08 15:27:48.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/util/decator.py
+-rw-rw-rw-   0        0        0     3908 2023-02-28 01:05:14.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/util/time.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:11:17.182169 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk.egg-info/
+-rw-rw-rw-   0        0        0      375 2023-07-27 01:11:16.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      751 2023-07-27 01:11:17.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 01:11:16.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-27 01:11:16.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-27 01:11:16.000000 zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk.egg-info/top_level.txt
```

### Comparing `zcbot-crawl-sdk-0.0.9/setup.py` & `zcbot-crawl-sdk-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-crawl-sdk',
-      version='0.0.9',
+      version='1.0.0',
       description='zcbot celery sdk for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
       install_requires=['pika', 'demjson', 'requests'],
       python_requires='>=3.7',
```

### Comparing `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/api.py` & `zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/api/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 import json
 import logging
 import demjson
-from typing import List, Union
-from .model import ApiData, StreamApiData, TaskItem
+from .model import StreamApiData, BatchApiData
 from . import http_client
 from . import exceptions
 
 LOGGER = logging.getLogger(__name__)
 
 
 class _Base(object):
@@ -42,113 +41,65 @@
         if not js or not js.get('success', False) or js.get('code', -1) < 0:
             raise exceptions.BizException(rs, '业务操作失败')
 
         return js.get('data', {})
 
 
 class ZcbotApi(_Base):
-    # 简易分拣接口
-    def simple_classify(self, task_items: List[Union[TaskItem, dict]]):
-        rs = self._post(
-            url=f'{self.endpoint}/api/materiel/classify',
-            data=demjson.encode(task_items)
-        )
-        return self._parse_result(rs)
-
-    # 任务分拣接口
-    def classify_and_init_task(self, api_data: ApiData):
-        rs = self._post(
-            url=f'{self.endpoint}/api/materiel/classify-and-init-task',
-            data=api_data.json()
-        )
-        return self._parse_result(rs)
 
-    # 商品基础信息采集接口
-    def start_sku_info_job(self, api_data: ApiData):
-        rs = self._post(
-            url=f'{self.endpoint}/api/task/start/sku-info',
-            data=api_data.json()
+    # ====================
+    # 批次采集接口
+    # ====================
+    def batch_publish(self, api_data: BatchApiData):
+        """
+        批次采集任务发布接口
+        :param api_data:
+        :return:
+        """
+        rs = self._post(
+            url=f'{self.endpoint}/api/batch/publish',
+            data=demjson.encode(api_data)
         )
         return self._parse_result(rs)
 
-    # 商品价格采集接口
-    def start_sku_price_job(self, api_data: ApiData):
-        rs = self._post(
-            url=f'{self.endpoint}/api/task/start/sku-price',
-            data=api_data.json()
-        )
-        return self._parse_result(rs)
-
-    # 商品全量信息采集接口
-    def start_sku_full_job(self, api_data: ApiData):
-        rs = self._post(
-            url=f'{self.endpoint}/api/task/start/sku-full',
-            data=api_data.json()
+    def batch_cancel(self, node: str):
+        """
+        批次采集任务取消接口
+        :param node:
+        :return:
+        """
+        rs = self._get(
+            url=f'{self.endpoint}/api/batch/cancel',
+            params={'node': node},
         )
         return self._parse_result(rs)
 
-    # 商品主详图采集接口
-    def start_sku_image_job(self, api_data: ApiData):
+    # ====================
+    # 流式采集接口
+    # ====================
+    def stream_publish(self, api_data: StreamApiData):
+        """
+        流式采集发布采集任务接口
+        :param api_data:
+        :return:
+        """
         rs = self._post(
-            url=f'{self.endpoint}/api/task/start/sku-image',
+            url=f'{self.endpoint}/api/stream/publish',
             data=api_data.json()
         )
         return self._parse_result(rs)
 
-    # 图片结果打包接口
-    def start_zip(self, api_data: ApiData):
-        rs = self._get(
-            url=f'{self.endpoint}/api/zip/zip',
-            params=api_data.dict(),
-        )
-        return self._parse_result(rs)
-
-    # 采集任务取消接口
-    def cancel_job(self, batch_id: str, job_id: str = None):
-        rs = self._get(
-            url=f'{self.endpoint}/api/task/cancel',
-            params={'job_id': job_id, 'batch_id': batch_id},
-        )
-        return self._parse_result(rs)
-
-    # 删除批次接口
-    def delete_batch(self, batch_id: str):
-        rs = self._get(
-            url=f'{self.endpoint}/api/task/delete',
-            params={'batch_id': batch_id},
-        )
-        return self._parse_result(rs)
-
+    # ============================
     # 获取所有平台
     def get_all_platforms(self):
         rs = self._get(
             url=f'{self.endpoint}/api/meta/platforms',
         )
         return self._parse_result(rs)
 
     # 获取所有平台
-    def get_platforms_by_task_type(self, task_type: str):
+    def get_platforms_by_spider_group(self, spider_group: str):
         rs = self._get(
-            url=f'{self.endpoint}/api/meta/task-type/platforms',
-            params={'task_type': task_type},
-        )
-        return self._parse_result(rs)
-
-    # 流式采集发布采集任务接口
-    def stream_publish(self, api_data: StreamApiData):
-        rs = self._post(
-            url=f'{self.endpoint}/api/stream/publish',
-            data=api_data.json()
+            url=f'{self.endpoint}/api/meta/platforms/batch',
+            params={'spider_group': spider_group},
         )
         return self._parse_result(rs)
-
-    # 流式采集发布采集任务接口
-    def stream_simple_publish(self, api_data: StreamApiData):
-        rs = self._post(
-            url=f'{self.endpoint}/api/stream/simple-publish',
-            data=api_data.json()
-        )
-        return self._parse_result(rs)
-
-    # 条码截图接口
-    def barcode_screenshot(self, ):
-        pass
```

### Comparing `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/exceptions.py` & `zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/http_client.py` & `zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/api/http_client.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/api/model.py` & `zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/api/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,87 @@
 from enum import Enum
 from typing import List, Union, Dict
 from pydantic import BaseModel, Field
 from ..util import time as time_lib
 
 
+class BatchTaskItem(BaseModel):
+    """
+    任务明细模型
+    """
+    # 【输入】对象唯一序列号（全局唯一，可用于主键，等于_id）
+    sn: str = None
+    # 【输入】用户指定编号
+    rowId: str = None
+    # 【输入】商品链接
+    url: str = None
+    # 扩展字段，可是任意内容，透传
+    callback: Union[str, Dict, List] = None
+
+
+class BatchTask(BaseModel):
+    """
+    批次任务接收模型
+    """
+    # 【输入】任务爬虫编码清单
+    spiderId: str = None
+    # 【输入】任务链接明细清单
+    taskItems: List[BatchTaskItem] = []
+    # 【输入】文件名称配置键（主详图采集命名使用，非必要）
+    file_name_config: str = 'default'
+
+
+class BatchApiData(BaseModel):
+    """
+    批次接口接收模型
+    """
+    # 【输入】批次编号
+    batchId: str = None
+    # 【输入】应用编码
+    appCode: str = None
+    # 【输入】任务明细清单
+    taskList: List[BatchTask] = []
+
+
+class BatchTaskNodeResp(BaseModel):
+    """
+    任务明细模型
+    """
+    # 【输出】对象唯一序列号（全局唯一，可用于主键，等于_id）
+    nodeId: str = None
+    # 【输出】容器编号
+    containerId: str = None
+    # 【输出】服务器编号
+    hostId: str = None
+    # 【输出】商品状态
+    status: str = None
+    # 【输出】商品状态描述
+    statusText: str = None
+    # 创建时间
+    genTime: int = None
+    # 更新时间
+    updateTime: int = None
+
+
+class BatchTaskResp(BaseModel):
+    """
+    批次采集结果响应模型
+    """
+    # 【输出】爬虫编码
+    spiderId: str = None
+    # 【输出】批次编号
+    batchId: str = None
+    # 【输出】任务链接明细清单
+    nodes: List[BatchTaskNodeResp] = []
+
+
+# ========================
+# 以下待删除
+# ========================
+
 class TaskType(str, Enum):
     """
     任务类型枚举
     """
     # 商品基础信息
     SKU_INFO = 'sku_info'
     # 商品价格
@@ -21,17 +95,14 @@
     # 流式采集商品价格信息
     STREAM_SKU_PRICE = 'stream_sku_price'
     # 流式采集商品基础信息及价格等详细信息
     STREAM_SKU_FULL = 'stream_sku_full'
     # 流式采集商品主详图
     STREAM_SKU_IMAGE = 'stream_sku_image'
 
-    # 商品信息抽取
-    SKU_EXTRACT = 'sku_extract'
-
 
 class BaseData(BaseModel):
     """
     通用基础数据模型
     """
     # 主键
     _id: str = None
```

### Comparing `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/model.py` & `zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/receive/model.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/processor.py` & `zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/receive/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             elif msg_type == MsgType.ACT_CLOSED.name:
                 self.process_closed_action(tenant_code, batch_id, msg_data)
             elif msg_type == MsgType.ACT_OPENED.name:
                 self.process_opened_action(tenant_code, batch_id, msg_data)
             else:
                 self.process_others(tenant_code, batch_id, msg_data, msg_type)
         except Exception:
-            LOGGER.error(f'[消息处理]解析异常 batch_id={batch_id}, {traceback.format_exc()}')
+            LOGGER.error(f'[消息处理]解析异常 batch_id={batch_id}, msg_data={msg_data}, except={traceback.format_exc()}')
 
     def process_sku_text_data(self, tenant_code: str, batch_id: str, msg_data: Union[Dict, List]):
         print(f'[{threading.current_thread().name}]process: msg_type=process_sku_text_data, msg_data={msg_data}, tenant_code={tenant_code}, batch_id={batch_id}')
         pass
 
     def process_sku_images_data(self, tenant_code: str, batch_id: str, msg_data: Union[Dict, List]):
         print(f'[{threading.current_thread().name}]process: msg_type=process_sku_images_data, msg_data={msg_data}, tenant_code={tenant_code}, batch_id={batch_id}')
@@ -59,14 +59,15 @@
                 self.process_stream_sku_text(msg_data)
             elif msg_type == MsgType.STREAM_SKU_IMAGES.name:
                 self.process_stream_sku_images(msg_data)
             else:
                 self.process_others(msg_data, msg_type)
         except Exception:
             LOGGER.error(f'[流采消息]解析异常 {traceback.format_exc()}')
+            LOGGER.error(f'[流采消息]解析异常 msg_data={msg_data}, except={traceback.format_exc()}')
 
     def process_stream_sku_text(self, msg_data: dict):
         print(msg_data)
         pass
 
     def process_stream_sku_images(self, msg_data: dict):
         print(msg_data)
```

### Comparing `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/rabbit_keys.py` & `zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/receive/rabbit_keys.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/receive/receiver.py` & `zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/receive/receiver.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk/util/time.py` & `zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk/util/time.py`

 * *Files identical despite different names*

### Comparing `zcbot-crawl-sdk-0.0.9/zcbot_crawl_sdk.egg-info/SOURCES.txt` & `zcbot-crawl-sdk-1.0.0/zcbot_crawl_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

