# Comparing `tmp/HawaData-0.8.9.tar.gz` & `tmp/HawaData-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.8.9.tar", last modified: Thu Jul 27 03:29:59 2023, max compression
+gzip compressed data, was "HawaData-0.9.0.tar", last modified: Thu Jul 27 05:28:38 2023, max compression
```

## Comparing `HawaData-0.8.9.tar` & `HawaData-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 03:29:59.459224 HawaData-0.8.9/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 03:29:59.444850 HawaData-0.8.9/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3508 2023-07-27 03:29:59.000000 HawaData-0.8.9/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-27 03:29:59.000000 HawaData-0.8.9/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-27 03:29:59.000000 HawaData-0.8.9/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-27 03:29:59.000000 HawaData-0.8.9/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3508 2023-07-27 03:29:59.458910 HawaData-0.8.9/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.8.9/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 03:29:59.445431 HawaData-0.8.9/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.8.9/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 03:29:59.448772 HawaData-0.8.9/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.8.9/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2807 2023-07-27 02:46:27.000000 HawaData-0.8.9/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      522 2023-07-24 09:22:05.000000 HawaData-0.8.9/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.8.9/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.8.9/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 03:29:59.450656 HawaData-0.8.9/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.8.9/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    17142 2023-07-27 03:29:51.000000 HawaData-0.8.9/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     6455 2023-07-26 15:07:30.000000 HawaData-0.8.9/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.8.9/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.8.9/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 03:29:59.455164 HawaData-0.8.9/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.8.9/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.8.9/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.8.9/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.8.9/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.8.9/hawa/data/province.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.8.9/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.8.9/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 03:29:59.457467 HawaData-0.8.9/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.8.9/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28951 2023-07-24 04:31:22.000000 HawaData-0.8.9/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.8.9/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-27 03:29:59.459327 HawaData-0.8.9/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.8.9/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 03:29:59.458122 HawaData-0.8.9/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.8.9/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.483112 HawaData-0.9.0/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.473611 HawaData-0.9.0/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3545 2023-07-27 05:28:38.000000 HawaData-0.9.0/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-27 05:28:38.000000 HawaData-0.9.0/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-27 05:28:38.000000 HawaData-0.9.0/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-27 05:28:38.000000 HawaData-0.9.0/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3545 2023-07-27 05:28:38.482816 HawaData-0.9.0/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.9.0/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.474063 HawaData-0.9.0/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.9.0/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.475861 HawaData-0.9.0/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.9.0/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2807 2023-07-27 02:46:27.000000 HawaData-0.9.0/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      522 2023-07-24 09:22:05.000000 HawaData-0.9.0/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.9.0/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.9.0/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.477123 HawaData-0.9.0/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.9.0/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    17368 2023-07-27 05:22:54.000000 HawaData-0.9.0/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     6517 2023-07-27 05:22:54.000000 HawaData-0.9.0/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.9.0/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.9.0/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.480781 HawaData-0.9.0/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.9.0/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.9.0/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.9.0/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.9.0/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.9.0/hawa/data/province.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.9.0/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.9.0/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.481947 HawaData-0.9.0/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.9.0/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28951 2023-07-24 04:31:22.000000 HawaData-0.9.0/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.9.0/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-27 05:28:38.483192 HawaData-0.9.0/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.9.0/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-27 05:28:38.482191 HawaData-0.9.0/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.9.0/test/test_query.py
```

### Comparing `HawaData-0.8.9/HawaData.egg-info/PKG-INFO` & `HawaData-0.9.0/HawaData.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.8.9
+Version: 0.9.0
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -120,7 +120,8 @@
 - 0.8.2 add global precision
 - 0.8.3 add global precision in func
 - 0.8.4 fix extra dim/field
 - 0.8.5 load less data
 - 0.8.7 add mongo params
 - 0.8.8 fix
 - 0.8.9 log
+- 0.9.0 use less item codes to upper
```

### Comparing `HawaData-0.8.9/HawaData.egg-info/SOURCES.txt` & `HawaData-0.9.0/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/PKG-INFO` & `HawaData-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.8.9
+Version: 0.9.0
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -120,7 +120,8 @@
 - 0.8.2 add global precision
 - 0.8.3 add global precision in func
 - 0.8.4 fix extra dim/field
 - 0.8.5 load less data
 - 0.8.7 add mongo params
 - 0.8.8 fix
 - 0.8.9 log
+- 0.9.0 use less item codes to upper
```

### Comparing `HawaData-0.8.9/README.md` & `HawaData-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/hawa/base/db.py` & `HawaData-0.9.0/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/hawa/base/decos.py` & `HawaData-0.9.0/hawa/base/decos.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/hawa/base/init.py` & `HawaData-0.9.0/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/hawa/common/data.py` & `HawaData-0.9.0/hawa/common/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """通用的 report data 构造器，支持 校、区、市、省、全国级别的通用报告数据构造"""
 import json
-import time
 from collections import Counter, defaultdict
 from dataclasses import dataclass, field
 from typing import Optional, ClassVar, Any, Set
 
 import pandas as pd
 import pendulum
 
@@ -56,14 +55,15 @@
     codebook: pd.DataFrame = field(default_factory=pd.DataFrame)
 
     cases: pd.DataFrame = field(default_factory=pd.DataFrame)
     case_ids: list[int] = field(default_factory=list)
     case_project_ids: Counter = field(default_factory=Counter)
 
     answers: pd.DataFrame = field(default_factory=pd.DataFrame)
+    item_codes: pd.DataFrame = field(default_factory=pd.DataFrame)
 
     students: pd.DataFrame = field(default_factory=pd.DataFrame)
     student_ids: list[int] = field(default_factory=list)
     student_count: Optional[int] = None
 
     item_ids: Optional[set[int]] = None
     items: Optional[pd.DataFrame] = None
@@ -153,22 +153,26 @@
         self.answers = self.query.query_answers(case_ids=self.case_ids)
         project.logger.debug(f'answers: {len(self.answers)}')
 
     def _to_init_f_students(self):
         self.student_ids = set(self.answers['student_id'].tolist())
         student_id_list = list(self.student_ids)
         self.students = self.query.query_students(student_id_list)
-        self.student_count = len(self.student_ids)
+        self.student_count = len(self.students)
         project.logger.debug(f'students: {self.student_count}')
 
     def _to_init_g_items(self):
         self.item_ids = set(self.answers['item_id'].drop_duplicates())
         self.items = self.query.query_items(self.item_ids)
         project.logger.debug(f'items: {len(self.items)}')
 
+    def _to_init_y_item_codes(self):
+        word_list = self.code_word_list | {'other'} if len(self.code_word_list) == 1 else self.code_word_list
+        self.item_codes = self.query.query_item_codes(self.item_ids, word_list)
+
     def _to_init_z_dim_field(self):
         cache_key = f"{project.PROJECT}:codebook"
         if data := self.redis.conn.get(cache_key):
             self.codebook = pd.DataFrame.from_records(json.loads(data))
         else:
             self.codebook = self.query.query_codebook()
             cache_data = self.codebook.to_json(orient='records', force_ascii=False)
@@ -177,30 +181,29 @@
     def _to_build_helper(self):
         self.grade = GradeData(case_ids=self.case_ids)
         self.case = CaseData(cases=self.cases)
 
     @log_func_time
     def _to_count_a_final_answers(self):
         items = {k: {} for k in self.code_word_list}
-        item_codes = self.query.query_item_codes(self.item_ids)
         # code-dimension/field  ~  item_id  ~ code   name
         project.logger.debug(f"{self.code_word_list=}")
-        for (item_id, category), codes in item_codes.groupby(['item_id', 'category']):
+        for (item_id, category), codes in self.item_codes.groupby(['item_id', 'category']):
             if category in self.code_word_list:
                 for _, code_data in codes.iterrows():
                     items[category][item_id] = code_data['name']
 
         data = pd.merge(
             self.answers, self.students.loc[:, ['id', 'gender', 'nickname']],
             left_on='student_id', right_on='id'
         )
         project.logger.debug(f"ans merge students {len(data)}")
         # inner 时，final_answers 和 answers 数目不等：final_answers 过滤掉了 没有 code_word_list（维度领域或其他）的题目
         # outer 时，数目相等，不过滤任何题目
-        data = pd.merge(data, item_codes, left_on='item_id', right_on='item_id', how='inner')
+        data = pd.merge(data, self.item_codes, left_on='item_id', right_on='item_id', how='inner')
 
         project.logger.debug(f'merge success {data.shape}')
 
         data['cls'] = data['id_y'].apply(lambda x: int(str(x)[13:15]))
         data['grade'] = data['case_id'].apply(lambda x: x % 100)
         data['username'] = data['nickname']
         for code_word in self.code_word_list:
```

### Comparing `HawaData-0.8.9/hawa/common/query.py` & `HawaData-0.9.0/hawa/common/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,18 +119,18 @@
     def query_items(self, item_ids: list[int]):
         item_cols = "id, item_text, choices, item_key, item_type, grade, test_type, pattern, " \
                     "`source`, created"
         sql = f"select {item_cols} from items where id in {tuple(item_ids)};"
         with self.db.engine_conn() as conn:
             return pd.read_sql(text(sql), conn)
 
-    def query_item_codes(self, item_ids: list[int]):
+    def query_item_codes(self, item_ids: list[int], categories: list[str]):
         item_code_sql = f'select ic.item_id,ic.code,ic.category,c.name ' \
                         f'from item_codes ic left join codebook c on ic.code = c.code ' \
-                        f'where ic.item_id in {tuple(item_ids)};'
+                        f'where ic.item_id in {tuple(item_ids)} and ic.category in {tuple(categories)};'
         with self.db.engine_conn() as conn:
             item_codes = pd.read_sql(text(item_code_sql), conn)
         return item_codes
 
     def query_locations(self, location_ids: list[int]):
         location_sql = f'select id, name, level from locations where id in {tuple(location_ids)};'
         with self.db.engine_conn() as conn:
```

### Comparing `HawaData-0.8.9/hawa/common/utils.py` & `HawaData-0.9.0/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/hawa/config.py` & `HawaData-0.9.0/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/hawa/data/klass.py` & `HawaData-0.9.0/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/hawa/data/province.py` & `HawaData-0.9.0/hawa/data/province.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/hawa/data/school.py` & `HawaData-0.9.0/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/hawa/data/student.py` & `HawaData-0.9.0/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/hawa/paper/health.py` & `HawaData-0.9.0/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/hawa/paper/mht.py` & `HawaData-0.9.0/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/setup.py` & `HawaData-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.9/test/test_query.py` & `HawaData-0.9.0/test/test_query.py`

 * *Files identical despite different names*

