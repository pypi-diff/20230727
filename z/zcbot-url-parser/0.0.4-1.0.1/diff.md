# Comparing `tmp/zcbot-url-parser-0.0.4.tar.gz` & `tmp/zcbot-url-parser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zcbot-url-parser-0.0.4.tar", last modified: Wed Jun 28 06:27:52 2023, max compression
+gzip compressed data, was "dist\zcbot-url-parser-1.0.1.tar", last modified: Thu Jul 27 05:02:08 2023, max compression
```

## Comparing `zcbot-url-parser-0.0.4.tar` & `zcbot-url-parser-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 06:27:52.487358 zcbot-url-parser-0.0.4/
--rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-url-parser-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      379 2023-06-28 06:27:52.486358 zcbot-url-parser-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      135 2023-05-30 07:06:49.000000 zcbot-url-parser-0.0.4/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-28 06:27:52.487358 zcbot-url-parser-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-06-28 06:08:53.000000 zcbot-url-parser-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 06:27:52.478359 zcbot-url-parser-0.0.4/zcbot_url_parser/
--rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-url-parser-0.0.4/zcbot_url_parser/__init__.py
--rw-rw-rw-   0        0        0     3647 2023-06-28 05:34:27.000000 zcbot-url-parser-0.0.4/zcbot_url_parser/parser.py
--rw-rw-rw-   0        0        0     3013 2023-06-28 06:05:15.000000 zcbot-url-parser-0.0.4/zcbot_url_parser/rule.py
--rw-rw-rw-   0        0        0      272 2023-05-30 07:12:11.000000 zcbot-url-parser-0.0.4/zcbot_url_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-28 06:27:52.485358 zcbot-url-parser-0.0.4/zcbot_url_parser.egg-info/
--rw-rw-rw-   0        0        0      379 2023-06-28 06:27:52.000000 zcbot-url-parser-0.0.4/zcbot_url_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-06-28 06:27:52.000000 zcbot-url-parser-0.0.4/zcbot_url_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 06:27:52.000000 zcbot-url-parser-0.0.4/zcbot_url_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-28 06:27:52.000000 zcbot-url-parser-0.0.4/zcbot_url_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-28 06:27:52.000000 zcbot-url-parser-0.0.4/zcbot_url_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 05:02:08.695875 zcbot-url-parser-1.0.1/
+-rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-url-parser-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      379 2023-07-27 05:02:08.694875 zcbot-url-parser-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      135 2023-05-30 07:06:49.000000 zcbot-url-parser-1.0.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-27 05:02:08.695875 zcbot-url-parser-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-07-27 05:01:28.000000 zcbot-url-parser-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 05:02:08.685878 zcbot-url-parser-1.0.1/zcbot_url_parser/
+-rw-rw-rw-   0        0        0       40 2023-03-14 03:58:21.000000 zcbot-url-parser-1.0.1/zcbot_url_parser/__init__.py
+-rw-rw-rw-   0        0        0      604 2023-07-27 04:57:32.000000 zcbot-url-parser-1.0.1/zcbot_url_parser/constant.py
+-rw-rw-rw-   0        0        0     3531 2023-07-27 04:00:15.000000 zcbot-url-parser-1.0.1/zcbot_url_parser/parser.py
+-rw-rw-rw-   0        0        0     2935 2023-07-27 04:49:25.000000 zcbot-url-parser-1.0.1/zcbot_url_parser/rule.py
+-rw-rw-rw-   0        0        0     3511 2023-07-27 04:59:09.000000 zcbot-url-parser-1.0.1/zcbot_url_parser/spider.py
+-rw-rw-rw-   0        0        0      597 2023-07-27 03:12:39.000000 zcbot-url-parser-1.0.1/zcbot_url_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 05:02:08.692874 zcbot-url-parser-1.0.1/zcbot_url_parser.egg-info/
+-rw-rw-rw-   0        0        0      379 2023-07-27 05:02:08.000000 zcbot-url-parser-1.0.1/zcbot_url_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-07-27 05:02:08.000000 zcbot-url-parser-1.0.1/zcbot_url_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 05:02:08.000000 zcbot-url-parser-1.0.1/zcbot_url_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 05:02:08.000000 zcbot-url-parser-1.0.1/zcbot_url_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-27 05:02:08.000000 zcbot-url-parser-1.0.1/zcbot_url_parser.egg-info/top_level.txt
```

### Comparing `zcbot-url-parser-0.0.4/setup.py` & `zcbot-url-parser-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-url-parser',
-      version='0.0.4',
+      version='1.0.1',
       description='zcbot url parser for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
-      install_requires=['requests', 'pymongo'],
+      install_requires=['pymongo'],
       python_requires='>=3.7',
       license='BSD License',
       packages=find_packages(),
       platforms=['all'],
       include_package_data=True
       )
```

### Comparing `zcbot-url-parser-0.0.4/zcbot_url_parser/parser.py` & `zcbot-url-parser-1.0.1/zcbot_url_parser/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import urllib.parse as parser
 from typing import Union
-
 from pydantic import BaseModel
 from .rule import RuleHolder
+from .utils import clean_url
 
 LOGGER = logging.getLogger(__name__)
 rule_holder = RuleHolder()
 
 
 class UrlModel(BaseModel):
     """
@@ -16,15 +16,15 @@
     # 链接序列号（全局唯一）  如：jd:5129155、tmall:576748721316,3985068128611
     link_sn: str = None
     # 网站编码  如：jd
     plat_code: str = None
     # 网站名称  如：京东
     plat_name: str = None
     # 链接商品编码（多编码链接，编码之间逗号分隔）  如：5129155、576748721316,3985068128611
-    ec_sku_id: str = None
+    ec_sku_id: Union[str, tuple] = None
 
 
 def parse_url(url) -> Union[UrlModel]:
     """
     解析url链接
     """
     plat_code, plat_name, ec_sku_id = _match_url(url)
@@ -41,36 +41,19 @@
     """
     if plat_code and ec_sku_id:
         return f'{plat_code}:{ec_sku_id}'
 
     return None
 
 
-def _clean_url(url):
-    """
-    链接非法字符清理
-    """
-    fix_err = {
-        '&amp;': '&',
-        '＆': '&'
-    }
-    _url = url
-    if _url:
-        for key in fix_err:
-            if key in _url:
-                _url = _url.replace(key, fix_err.get(key))
-
-    return _url
-
-
 def _match_url(url):
     plat_code = ''
     plat_name = ''
     ec_sku_id = ''
-    _url = _clean_url(url)
+    _url = clean_url(url)
     if _url:
         host = parser.urlparse(_url).hostname
         rule = rule_holder.get_rule(host)
         if host and rule:
             plat_code = rule.get('plat_code')
             plat_name = rule.get('plat_name')
             sku_param = rule.get('sku_param', [])
@@ -90,26 +73,30 @@
         rule = rule_holder.get_rule(host)
         if host and rule:
             plat_code = rule.get('plat_code')
 
     return plat_code
 
 
-def _parse_sku_by_path(url, patterns):
+def _parse_sku_by_path(url, patterns, token=','):
     """
     根据url中path部分解析skuId
     :param url:
     :param patterns:
     :return:
     """
     try:
         for ptn in patterns:
             arr = ptn.findall(url.strip())
             if len(arr):
-                return arr[0].strip()
+                rs = arr[0]
+                if token and isinstance(rs, tuple):
+                    return token.join(rs)
+                else:
+                    return rs
     except Exception as e:
         LOGGER.error('match sku error[parse_sku_by_path]: url=%s, ex=%s' % (url, e))
 
     return ''
 
 
 def _parse_sku_by_param(url, sku_param, token=','):
```

### Comparing `zcbot-url-parser-0.0.4/zcbot_url_parser/rule.py` & `zcbot-url-parser-1.0.1/zcbot_url_parser/rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import logging
 import re
-import requests
 from pymongo import MongoClient
-
+from .constant import ZCBOT_PUBLIC_MONGO_URL, ZCBOT_PUBLIC_MONGO_DATABASE, ZCBOT_PUBLIC_MONGO_COLLECTION_PLATFORMS, ZCBOT_PUBLIC_MONGO_COLLECTION_RULES
 from .utils import singleton
 
 LOGGER = logging.getLogger(__name__)
 
 
 @singleton
 class RuleHolder(object):
     """
     常见电商平台商品编码解析规则
     """
     rule_map = {}
 
-    def __init__(self):
+    def __init__(self, mongo_url: str = None, mongo_database: str = None, mongo_collection_platforms: str = None, mongo_collection_rules: str = None):
+        self.mongo_url = mongo_url or ZCBOT_PUBLIC_MONGO_URL
+        self.mongo_database = mongo_database or ZCBOT_PUBLIC_MONGO_DATABASE
+        self.mongo_collection_platforms = mongo_collection_platforms or ZCBOT_PUBLIC_MONGO_COLLECTION_PLATFORMS
+        self.mongo_collection_rules = mongo_collection_rules or ZCBOT_PUBLIC_MONGO_COLLECTION_RULES
         self.reload()
 
     def get_rule(self, host):
         return self.rule_map.get(host)
 
     def reload(self):
         """
@@ -49,48 +52,31 @@
                 'sku_param': row.get('params', []),
                 'patterns': [
                     re.compile(x) for x in row.get('regex', [])
                 ],
             }
         LOGGER.info(f'更新链接分拣规则: {len(self.rule_map)}条')
 
-    # def _fetch_platforms(self):
-    #     platforms = []
-    #     # TODO 待优化
-    #     rs = requests.get('http://www.zcbot.cn/zcbot-api/api/meta/platforms', timeout=15)
-    #     if rs:
-    #         platforms = rs.json().get('data', []) or []
-    #
-    #     return platforms
-    #
-    # def _fetch_url_rules(self):
-    #     rules = []
-    #     # TODO 待优化
-    #     rs = requests.get('http://www.zcbot.cn/zcbot-api/api/meta/url-rules', timeout=15)
-    #     if rs:
-    #         rules = rs.json().get('data', []) or []
-    #
-    #     return rules
-
     def _fetch_platforms(self):
         try:
-            client = MongoClient('mongodb://public_read:public_read_zsodata@zcbot-outer.mongodb.rds.aliyuncs.com:3717')
-            rs = client.get_database('zcbot_pool').get_collection('zcbot_platforms').find()
+
+            client = MongoClient(self.mongo_url)
+            rs = client.get_database(self.mongo_database).get_collection(self.mongo_collection_platforms).find()
             rows = list(rs)
             client.close()
             return rows
         except Exception as e:
             print(e)
 
         return []
 
     def _fetch_url_rules(self):
         try:
-            client = MongoClient('mongodb://public_read:public_read_zsodata@zcbot-outer.mongodb.rds.aliyuncs.com:3717')
-            rs = client.get_database('zcbot_pool').get_collection('zcbot_url_parse_rule').find()
+            client = MongoClient(self.mongo_url)
+            rs = client.get_database(self.mongo_database).get_collection(self.mongo_collection_rules).find()
             rows = list(rs)
             client.close()
             return rows
         except Exception as e:
             print(e)
 
         return []
```

