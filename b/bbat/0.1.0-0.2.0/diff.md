# Comparing `tmp/bbat-0.1.0.tar.gz` & `tmp/bbat-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbat-0.1.0.tar", last modified: Fri Jul 21 03:34:33 2023, max compression
+gzip compressed data, was "bbat-0.2.0.tar", last modified: Thu Jul 27 07:45:28 2023, max compression
```

## Comparing `bbat-0.1.0.tar` & `bbat-0.2.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 03:34:33.364499 bbat-0.1.0/
--rw-rw-rw-   0        0        0      289 2023-07-21 03:34:33.363498 bbat-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-11 11:39:46.000000 bbat-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 03:34:33.223334 bbat-0.1.0/bbat/
--rw-rw-rw-   0        0        0        0 2023-07-09 13:29:18.000000 bbat-0.1.0/bbat/__init__.py
--rw-rw-rw-   0        0        0     1931 2023-07-18 01:38:19.000000 bbat-0.1.0/bbat/config.py
--rw-rw-rw-   0        0        0     3115 2023-07-17 07:29:02.000000 bbat-0.1.0/bbat/crypto.py
--rw-rw-rw-   0        0        0     1230 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/date.py
-drwxrwxrwx   0        0        0        0 2023-07-21 03:34:33.261849 bbat-0.1.0/bbat/db/
--rw-rw-rw-   0        0        0        0 2023-07-09 13:50:02.000000 bbat-0.1.0/bbat/db/__init__.py
--rw-rw-rw-   0        0        0     5722 2023-07-19 08:56:34.000000 bbat-0.1.0/bbat/db/aio_mysql.py
--rw-rw-rw-   0        0        0     2632 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/db/aio_sqlite.py
--rw-rw-rw-   0        0        0     2054 2023-07-15 12:58:24.000000 bbat-0.1.0/bbat/db/mysql.py
--rw-rw-rw-   0        0        0      491 2023-07-17 08:36:20.000000 bbat-0.1.0/bbat/document.py
--rw-rw-rw-   0        0        0       30 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/hi.py
--rw-rw-rw-   0        0        0     1978 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/image.py
-drwxrwxrwx   0        0        0        0 2023-07-21 03:34:33.264180 bbat-0.1.0/bbat/llm/
--rw-rw-rw-   0        0        0        0 2023-07-11 14:42:42.000000 bbat-0.1.0/bbat/llm/__init__.py
--rw-rw-rw-   0        0        0     2416 2023-07-12 14:36:12.000000 bbat-0.1.0/bbat/llm/chatgpt.py
--rw-rw-rw-   0        0        0      920 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/log.py
--rw-rw-rw-   0        0        0      828 2023-07-12 11:52:42.000000 bbat-0.1.0/bbat/machine.py
--rw-rw-rw-   0        0        0     1868 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/notice.py
--rw-rw-rw-   0        0        0     2497 2023-07-10 11:37:38.000000 bbat-0.1.0/bbat/np.py
--rw-rw-rw-   0        0        0     1764 2023-07-18 01:35:45.000000 bbat-0.1.0/bbat/path.py
--rw-rw-rw-   0        0        0     4198 2023-07-11 15:55:34.000000 bbat-0.1.0/bbat/text.py
-drwxrwxrwx   0        0        0        0 2023-07-21 03:34:33.289183 bbat-0.1.0/bbat/web/
--rw-rw-rw-   0        0        0        0 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/web/__init__.py
--rw-rw-rw-   0        0        0     1685 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/web/client.py
--rw-rw-rw-   0        0        0      504 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/web/cors.py
--rw-rw-rw-   0        0        0     4529 2023-07-19 09:03:04.000000 bbat-0.1.0/bbat/web/db_server.py
--rw-rw-rw-   0        0        0      177 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/web/flask_app.py
--rw-rw-rw-   0        0        0     1566 2023-07-13 12:06:02.000000 bbat-0.1.0/bbat/web/sanic_app.py
-drwxrwxrwx   0        0        0        0 2023-07-21 03:34:33.354506 bbat-0.1.0/bbat/web/url_to_sql/
--rw-rw-rw-   0        0        0        0 2023-07-10 11:37:38.000000 bbat-0.1.0/bbat/web/url_to_sql/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/web/url_to_sql/field.py
--rw-rw-rw-   0        0        0     7592 2023-07-19 09:04:00.000000 bbat-0.1.0/bbat/web/url_to_sql/query.py
--rw-rw-rw-   0        0        0     2256 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/web/url_to_sql/relation.py
--rw-rw-rw-   0        0        0      722 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/web/url_to_sql/test.py
--rw-rw-rw-   0        0        0      964 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/web/url_to_sql/util.py
--rw-rw-rw-   0        0        0     1473 2023-07-11 11:39:46.000000 bbat-0.1.0/bbat/web/url_to_sql/where.py
--rw-rw-rw-   0        0        0     1614 2023-07-12 11:52:42.000000 bbat-0.1.0/bbat/zcli.py
-drwxrwxrwx   0        0        0        0 2023-07-21 03:34:33.241811 bbat-0.1.0/bbat.egg-info/
--rw-rw-rw-   0        0        0      289 2023-07-21 03:34:32.000000 bbat-0.1.0/bbat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      876 2023-07-21 03:34:32.000000 bbat-0.1.0/bbat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 03:34:32.000000 bbat-0.1.0/bbat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-21 03:34:32.000000 bbat-0.1.0/bbat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-07-21 03:34:32.000000 bbat-0.1.0/bbat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-21 03:34:32.000000 bbat-0.1.0/bbat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 03:34:33.365498 bbat-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1027 2023-07-17 08:41:40.000000 bbat-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 03:34:33.362498 bbat-0.1.0/test/
--rw-rw-rw-   0        0        0      209 2023-07-11 11:39:46.000000 bbat-0.1.0/test/test_config.py
--rw-rw-rw-   0        0        0      194 2023-07-11 11:39:46.000000 bbat-0.1.0/test/test_db_mysql.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.036938 bbat-0.2.0/
+-rw-rw-rw-   0        0        0      289 2023-07-27 07:45:28.035939 bbat-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-11 11:39:46.000000 bbat-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.007691 bbat-0.2.0/bbat/
+-rw-rw-rw-   0        0        0        0 2023-07-09 13:29:18.000000 bbat-0.2.0/bbat/__init__.py
+-rw-rw-rw-   0        0        0     1931 2023-07-18 01:38:19.000000 bbat-0.2.0/bbat/config.py
+-rw-rw-rw-   0        0        0     3115 2023-07-17 07:29:02.000000 bbat-0.2.0/bbat/crypto.py
+-rw-rw-rw-   0        0        0     1230 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/date.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.019934 bbat-0.2.0/bbat/db/
+-rw-rw-rw-   0        0        0        0 2023-07-09 13:50:02.000000 bbat-0.2.0/bbat/db/__init__.py
+-rw-rw-rw-   0        0        0     5722 2023-07-19 08:56:34.000000 bbat-0.2.0/bbat/db/aio_mysql.py
+-rw-rw-rw-   0        0        0     2632 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/db/aio_sqlite.py
+-rw-rw-rw-   0        0        0     2054 2023-07-15 12:58:24.000000 bbat-0.2.0/bbat/db/mysql.py
+-rw-rw-rw-   0        0        0      491 2023-07-17 08:36:20.000000 bbat-0.2.0/bbat/document.py
+-rw-rw-rw-   0        0        0       30 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/hi.py
+-rw-rw-rw-   0        0        0     1978 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/image.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.020938 bbat-0.2.0/bbat/llm/
+-rw-rw-rw-   0        0        0        0 2023-07-11 14:42:42.000000 bbat-0.2.0/bbat/llm/__init__.py
+-rw-rw-rw-   0        0        0     2416 2023-07-12 14:36:12.000000 bbat-0.2.0/bbat/llm/chatgpt.py
+-rw-rw-rw-   0        0        0      920 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/log.py
+-rw-rw-rw-   0        0        0      828 2023-07-12 11:52:42.000000 bbat-0.2.0/bbat/machine.py
+-rw-rw-rw-   0        0        0     1868 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/notice.py
+-rw-rw-rw-   0        0        0     2497 2023-07-10 11:37:38.000000 bbat-0.2.0/bbat/np.py
+-rw-rw-rw-   0        0        0     1764 2023-07-18 01:35:45.000000 bbat-0.2.0/bbat/path.py
+-rw-rw-rw-   0        0        0     4198 2023-07-11 15:55:34.000000 bbat-0.2.0/bbat/text.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.026939 bbat-0.2.0/bbat/web/
+-rw-rw-rw-   0        0        0        0 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/__init__.py
+-rw-rw-rw-   0        0        0     1685 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/client.py
+-rw-rw-rw-   0        0        0      504 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/cors.py
+-rw-rw-rw-   0        0        0     4501 2023-07-27 07:39:54.000000 bbat-0.2.0/bbat/web/db_server.py
+-rw-rw-rw-   0        0        0      177 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/flask_app.py
+-rw-rw-rw-   0        0        0     1566 2023-07-13 12:06:02.000000 bbat-0.2.0/bbat/web/sanic_app.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.032938 bbat-0.2.0/bbat/web/url_to_sql/
+-rw-rw-rw-   0        0        0        0 2023-07-10 11:37:38.000000 bbat-0.2.0/bbat/web/url_to_sql/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/url_to_sql/field.py
+-rw-rw-rw-   0        0        0     7452 2023-07-27 07:40:43.000000 bbat-0.2.0/bbat/web/url_to_sql/query.py
+-rw-rw-rw-   0        0        0     2256 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/url_to_sql/relation.py
+-rw-rw-rw-   0        0        0      722 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/url_to_sql/test.py
+-rw-rw-rw-   0        0        0      964 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/url_to_sql/util.py
+-rw-rw-rw-   0        0        0     1473 2023-07-11 11:39:46.000000 bbat-0.2.0/bbat/web/url_to_sql/where.py
+-rw-rw-rw-   0        0        0     1614 2023-07-12 11:52:42.000000 bbat-0.2.0/bbat/zcli.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.015691 bbat-0.2.0/bbat.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-07-27 07:45:27.000000 bbat-0.2.0/bbat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      876 2023-07-27 07:45:27.000000 bbat-0.2.0/bbat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 07:45:27.000000 bbat-0.2.0/bbat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-27 07:45:27.000000 bbat-0.2.0/bbat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-07-27 07:45:27.000000 bbat-0.2.0/bbat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-27 07:45:27.000000 bbat-0.2.0/bbat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 07:45:28.036938 bbat-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2023-07-27 07:44:22.000000 bbat-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:45:28.034938 bbat-0.2.0/test/
+-rw-rw-rw-   0        0        0      209 2023-07-11 11:39:46.000000 bbat-0.2.0/test/test_config.py
+-rw-rw-rw-   0        0        0      194 2023-07-11 11:39:46.000000 bbat-0.2.0/test/test_db_mysql.py
```

### Comparing `bbat-0.1.0/bbat/config.py` & `bbat-0.2.0/bbat/config.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/crypto.py` & `bbat-0.2.0/bbat/crypto.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/date.py` & `bbat-0.2.0/bbat/date.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/db/aio_mysql.py` & `bbat-0.2.0/bbat/db/aio_mysql.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/db/aio_sqlite.py` & `bbat-0.2.0/bbat/db/aio_sqlite.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/db/mysql.py` & `bbat-0.2.0/bbat/db/mysql.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/image.py` & `bbat-0.2.0/bbat/image.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/llm/chatgpt.py` & `bbat-0.2.0/bbat/llm/chatgpt.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/log.py` & `bbat-0.2.0/bbat/log.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/machine.py` & `bbat-0.2.0/bbat/machine.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/notice.py` & `bbat-0.2.0/bbat/notice.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/np.py` & `bbat-0.2.0/bbat/np.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/path.py` & `bbat-0.2.0/bbat/path.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/text.py` & `bbat-0.2.0/bbat/text.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/web/client.py` & `bbat-0.2.0/bbat/web/client.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/web/db_server.py` & `bbat-0.2.0/bbat/web/db_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         # master表外键所有id
         idhub = set([str(i[relation.master_key]) for i in data])
         if len(idhub) == 0:
             continue
         ids = ",".join([f"'{i}'" for i in idhub])
         # 查子表数据
         sql = relation.to_sql(f"{relation.relate_key} IN ({ids})")
-        print("sql>", sql)
         relation_data = await db.query(sql)
         query.data_convert(relation.fields, relation_data)
         # 合并数据
         relation.merge_table_data(data, relation_data)
 
     result["list"] = data
     return success(result)
```

### Comparing `bbat-0.1.0/bbat/web/sanic_app.py` & `bbat-0.2.0/bbat/web/sanic_app.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/web/url_to_sql/field.py` & `bbat-0.2.0/bbat/web/url_to_sql/field.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/web/url_to_sql/query.py` & `bbat-0.2.0/bbat/web/url_to_sql/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,23 +148,21 @@
         return node
 
      # sql
     def to_sql(self):
         n = self.build_sql_node()
         sql = f"SELECT {n['field']} FROM {n['table']} {n['where']} {n['groupby']} {n['orderby']} {n['limit']}"
         sql = re.sub(r"\s+", " ", sql)
-        print("sql>", sql)
         return sql
     
     # meta 函数 查询总数
     def to_count_sql(self):
         n = self.build_sql_node()
         sql = f"SELECT count(1) cnt FROM {n['table']} {n['where']} {n['groupby']}"
         sql = re.sub(r"\s+", " ", sql)
-        print("sql>", sql)
         return sql
       
     # 插入sql
     def to_insert_sql(self, data, replace=False):
         length, keys, insert_data = self.data2sqlvalue(data)
         if type(insert_data) is tuple:
             insert_data = [insert_data]
@@ -173,15 +171,14 @@
             for i in d]) + ")" for d in insert_data
         ]
         sql = "INSERT INTO %s (%s) VALUES %s" % (self.table_name, ', '.join( [f"`{i}`" for i in keys]), ', '.join(data))
         if replace:
             sql += (' ON DUPLICATE KEY UPDATE ' + ', '.join(['%s=VALUES(%s)' % (x, x) for x in keys]))
         # sqlalcheme parse bug
         sql = sql.replace(":", "\:")
-        print("sql>", sql)
         return sql
     
     # 更新sql
     def to_update_sql(self, data):
         n = self.build_sql_node()
         set_ls = []
         for k, v in data.items():
@@ -191,24 +188,22 @@
             set_ls.append(string)
 
         sql = "UPDATE %s SET %s" % ( self.table_name, ",".join(set_ls), )
         # where 
         sql += n['where']
         # sqlalcheme parse bug
         sql = sql.replace(":", "\:")
-        print("sql>", sql)
         return sql
 
     # 删除sql
     def to_delete_sql(self):
         n = self.build_sql_node()
         sql = "DELETE FROM %s " % (self.table_name)
         sql += n['where']
         sql = sql.replace(':', '\:')
-        print("sql>", sql)
         return sql
 
     def data2sqlvalue(self, data):
         if isinstance(data, dict):
             item = data
             keys = item.keys()
             length = len(item)
```

### Comparing `bbat-0.1.0/bbat/web/url_to_sql/relation.py` & `bbat-0.2.0/bbat/web/url_to_sql/relation.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/web/url_to_sql/test.py` & `bbat-0.2.0/bbat/web/url_to_sql/test.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/web/url_to_sql/util.py` & `bbat-0.2.0/bbat/web/url_to_sql/util.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/web/url_to_sql/where.py` & `bbat-0.2.0/bbat/web/url_to_sql/where.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat/zcli.py` & `bbat-0.2.0/bbat/zcli.py`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/bbat.egg-info/SOURCES.txt` & `bbat-0.2.0/bbat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbat-0.1.0/setup.py` & `bbat-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import setuptools
 
 name = "bbat"
-version = "0.1.0"
+version = "0.2.0"
 
 def _process_requirements():
     packages = open('requirements.txt').read().strip().split('\n')
     requires = []
     for pkg in packages:
         if pkg.startswith('git+ssh'):
             return_code = os.system('pip install {}'.format(pkg))
```

