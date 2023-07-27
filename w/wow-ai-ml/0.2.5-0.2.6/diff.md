# Comparing `tmp/wow_ai_ml-0.2.5.tar.gz` & `tmp/wow_ai_ml-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow_ai_ml-0.2.5.tar", max compression
+gzip compressed data, was "wow_ai_ml-0.2.6.tar", max compression
```

## Comparing `wow_ai_ml-0.2.5.tar` & `wow_ai_ml-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.2.5/README.md
--rw-r--r--   0        0        0      261 2023-07-22 09:46:51.230680 wow_ai_ml-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.2.5/wow_ai_ml/__init__.py
--rw-r--r--   0        0        0     8957 2023-07-22 09:40:33.052501 wow_ai_ml-0.2.5/wow_ai_ml/api.py
--rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.2.5/wow_ai_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.2.5/wow_ai_ml/default_configs/README.md
--rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.2.5/wow_ai_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.2.5/wow_ai_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.2.5/wow_ai_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.2.5/wow_ai_ml/exceptions.py
--rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.2.5/wow_ai_ml/helpers.py
--rw-r--r--   0        0        0    34614 2023-07-22 09:46:19.605016 wow_ai_ml-0.2.5/wow_ai_ml/model.py
--rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.2.5/wow_ai_ml/server.py
--rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.2.5/wow_ai_ml/templates/preview.html
--rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.2.5/wow_ai_ml/utils.py
--rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.2.6/README.md
+-rw-r--r--   0        0        0      261 2023-07-27 03:41:54.789033 wow_ai_ml-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.2.6/wow_ai_ml/__init__.py
+-rw-r--r--   0        0        0     8994 2023-07-27 02:50:37.385627 wow_ai_ml-0.2.6/wow_ai_ml/api.py
+-rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.2.6/wow_ai_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.2.6/wow_ai_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.2.6/wow_ai_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.2.6/wow_ai_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.2.6/wow_ai_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.2.6/wow_ai_ml/exceptions.py
+-rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.2.6/wow_ai_ml/helpers.py
+-rw-r--r--   0        0        0    34613 2023-07-27 02:51:53.869231 wow_ai_ml-0.2.6/wow_ai_ml/model.py
+-rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.2.6/wow_ai_ml/server.py
+-rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.2.6/wow_ai_ml/templates/preview.html
+-rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.2.6/wow_ai_ml/utils.py
+-rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.2.6/PKG-INFO
```

### Comparing `wow_ai_ml-0.2.5/README.md` & `wow_ai_ml-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.5/wow_ai_ml/api.py` & `wow_ai_ml-0.2.6/wow_ai_ml/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,21 +41,22 @@
 
 @_server.route('/setup', methods=['POST'])
 @exception_handler
 def _setup():
     data = request.json
     logger.debug(data)
     project = data.get('project')
+    ml_id = data.get('ml_id')
     schema = data.get('schema')
     force_reload = data.get('force_reload', False)
     # host name for uploaded files and building urls
     hostname = data.get('hostname', '')
     # user access token to retrieve data
     access_token = data.get('access_token', '')
-    model = _manager.fetch(project, schema, force_reload,
+    model = _manager.fetch(project,ml_id, schema, force_reload,
                            hostname=hostname, access_token=access_token)
     logger.debug('Fetch model version: {}'.format(model.model_version))
     return jsonify({'model_version': model.model_version})
 
 
 @_server.route('/train', methods=['POST'])
 @exception_handler
```

### Comparing `wow_ai_ml-0.2.5/wow_ai_ml/default_configs/README.md` & `wow_ai_ml-0.2.6/wow_ai_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.5/wow_ai_ml/default_configs/_wsgi.py.tmpl` & `wow_ai_ml-0.2.6/wow_ai_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.5/wow_ai_ml/default_configs/docker-compose.yml` & `wow_ai_ml-0.2.6/wow_ai_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.5/wow_ai_ml/exceptions.py` & `wow_ai_ml-0.2.6/wow_ai_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.5/wow_ai_ml/helpers.py` & `wow_ai_ml-0.2.6/wow_ai_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.5/wow_ai_ml/model.py` & `wow_ai_ml-0.2.6/wow_ai_ml/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,15 +507,15 @@
         if not cls.has_active_model(project) or force_reload or (cls.get(project).model_version != version and version is not None):  # noqa
             logger.debug('Reload model for project={project} with version={version}'.format(
                 project=project, version=version))
             cls.create(project, label_config, train_output, version, **kwargs)
         return cls.get(project)
 
     @classmethod
-    def fetch(cls, project=None, label_config=None, force_reload=False, **kwargs):
+    def fetch(cls, project=None,label_config=None, force_reload=False, **kwargs):
         if not os.getenv('LABEL_STUDIO_ML_BACKEND_V2', default=LABEL_STUDIO_ML_BACKEND_V2_DEFAULT):
             # TODO: Deprecated branch since LS 1.5
             if cls.without_redis():
                 logger.debug('Fetch ' + project + ' from local directory')
                 job_result = cls._get_latest_job_result_from_workdir(project) or {}
             else:
                 logger.debug('Fetch ' + project + ' from Redis')
```

### Comparing `wow_ai_ml-0.2.5/wow_ai_ml/server.py` & `wow_ai_ml-0.2.6/wow_ai_ml/server.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.5/wow_ai_ml/utils.py` & `wow_ai_ml-0.2.6/wow_ai_ml/utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.5/PKG-INFO` & `wow_ai_ml-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ai-ml
-Version: 0.2.5
+Version: 0.2.6
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.inc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

