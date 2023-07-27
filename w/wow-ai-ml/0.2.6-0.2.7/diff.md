# Comparing `tmp/wow_ai_ml-0.2.6.tar.gz` & `tmp/wow_ai_ml-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow_ai_ml-0.2.6.tar", max compression
+gzip compressed data, was "wow_ai_ml-0.2.7.tar", max compression
```

## Comparing `wow_ai_ml-0.2.6.tar` & `wow_ai_ml-0.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.2.6/README.md
--rw-r--r--   0        0        0      261 2023-07-27 03:41:54.789033 wow_ai_ml-0.2.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.2.6/wow_ai_ml/__init__.py
--rw-r--r--   0        0        0     8994 2023-07-27 02:50:37.385627 wow_ai_ml-0.2.6/wow_ai_ml/api.py
--rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.2.6/wow_ai_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.2.6/wow_ai_ml/default_configs/README.md
--rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.2.6/wow_ai_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.2.6/wow_ai_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.2.6/wow_ai_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.2.6/wow_ai_ml/exceptions.py
--rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.2.6/wow_ai_ml/helpers.py
--rw-r--r--   0        0        0    34613 2023-07-27 02:51:53.869231 wow_ai_ml-0.2.6/wow_ai_ml/model.py
--rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.2.6/wow_ai_ml/server.py
--rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.2.6/wow_ai_ml/templates/preview.html
--rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.2.6/wow_ai_ml/utils.py
--rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.2.7/README.md
+-rw-r--r--   0        0        0      261 2023-07-27 03:53:54.916068 wow_ai_ml-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.2.7/wow_ai_ml/__init__.py
+-rw-r--r--   0        0        0     8994 2023-07-27 02:50:37.385627 wow_ai_ml-0.2.7/wow_ai_ml/api.py
+-rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.2.7/wow_ai_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.2.7/wow_ai_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.2.7/wow_ai_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.2.7/wow_ai_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.2.7/wow_ai_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.2.7/wow_ai_ml/exceptions.py
+-rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.2.7/wow_ai_ml/helpers.py
+-rw-r--r--   0        0        0    34792 2023-07-27 03:53:13.143511 wow_ai_ml-0.2.7/wow_ai_ml/model.py
+-rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.2.7/wow_ai_ml/server.py
+-rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.2.7/wow_ai_ml/templates/preview.html
+-rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.2.7/wow_ai_ml/utils.py
+-rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.2.7/PKG-INFO
```

### Comparing `wow_ai_ml-0.2.6/README.md` & `wow_ai_ml-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.6/wow_ai_ml/api.py` & `wow_ai_ml-0.2.7/wow_ai_ml/api.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.6/wow_ai_ml/default_configs/README.md` & `wow_ai_ml-0.2.7/wow_ai_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.6/wow_ai_ml/default_configs/_wsgi.py.tmpl` & `wow_ai_ml-0.2.7/wow_ai_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.6/wow_ai_ml/default_configs/docker-compose.yml` & `wow_ai_ml-0.2.7/wow_ai_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.6/wow_ai_ml/exceptions.py` & `wow_ai_ml-0.2.7/wow_ai_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.6/wow_ai_ml/helpers.py` & `wow_ai_ml-0.2.7/wow_ai_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.6/wow_ai_ml/model.py` & `wow_ai_ml-0.2.7/wow_ai_ml/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 logger = logging.getLogger(__name__)
 
 LABEL_STUDIO_ML_BACKEND_V2_DEFAULT = False
 
 @attr.s
 class ModelWrapper(object):
+    ml_id = attr.ib()
     model = attr.ib()
     model_version = attr.ib()
     is_training = attr.attrib(default=False)
 
 
 class JobManager(object):
     """Job Manager provides a facility to spin up background jobs for LabelStudioMLBase models"""
@@ -292,16 +293,17 @@
     TRAIN_EVENTS = (
         'ANNOTATION_CREATED',
         'ANNOTATION_UPDATED',
         'ANNOTATION_DELETED',
         'PROJECT_UPDATED'
     )
 
-    def __init__(self, label_config=None, train_output=None, **kwargs):
+    def __init__(self, ml_id=None, label_config=None, train_output=None, **kwargs):
         """Model loader"""
+        self.ml_id = ml_id
         self.label_config = label_config
         self.parsed_label_config = parse_config(self.label_config) if self.label_config else {}
         self.train_output = train_output or {}
         self.hostname = kwargs.get('hostname', '')
         self.access_token = kwargs.get('access_token', '')
 
     @abstractmethod
@@ -477,69 +479,70 @@
             key = cls._key(project)
             logger.debug('Get project ' + str(key))
             return cls._current_model.get(key)
         else:
             return cls._current_model
 
     @classmethod
-    def create(cls, project=None, label_config=None, train_output=None, version=None, **kwargs):
+    def create(cls, project=None,ml_id=None, label_config=None, train_output=None, version=None, **kwargs):
         key = cls._key(project)
         logger.debug('Create project ' + str(key))
         kwargs.update(cls.init_kwargs)
         if not os.getenv('LABEL_STUDIO_ML_BACKEND_V2', default=LABEL_STUDIO_ML_BACKEND_V2_DEFAULT):
             # TODO: Deprecated branch since LS 1.5
             cls._current_model[key] = ModelWrapper(
-                model=cls.model_class(label_config=label_config, train_output=train_output, **kwargs),
+                model=cls.model_class(ml_id=ml_id,label_config=label_config, train_output=train_output, **kwargs),
                 model_version=version or cls._generate_version()
             )
             return cls._current_model[key]
         else:
             cls._current_model = ModelWrapper(
-                model=cls.model_class(label_config=label_config, train_output=train_output, **kwargs),
+                model=cls.model_class(ml_id=ml_id,label_config=label_config, train_output=train_output, **kwargs),
                 model_version=version or cls._generate_version()
             )
             return cls._current_model
 
     @classmethod
     def get_or_create(
-        cls, project=None, label_config=None, force_reload=False, train_output=None, version=None, **kwargs
+        cls, project=None, ml_id=None,label_config=None, force_reload=False, train_output=None, version=None, **kwargs
     ):
         # reload new model if model is not loaded into memory OR force_reload=True OR model versions are mismatched
         if not cls.has_active_model(project) or force_reload or (cls.get(project).model_version != version and version is not None):  # noqa
             logger.debug('Reload model for project={project} with version={version}'.format(
                 project=project, version=version))
-            cls.create(project, label_config, train_output, version, **kwargs)
+            cls.create(project,ml_id, label_config, train_output, version, **kwargs)
         return cls.get(project)
 
     @classmethod
-    def fetch(cls, project=None,label_config=None, force_reload=False, **kwargs):
+    def fetch(cls, project=None,ml_id=None,label_config=None, force_reload=False, **kwargs):
         if not os.getenv('LABEL_STUDIO_ML_BACKEND_V2', default=LABEL_STUDIO_ML_BACKEND_V2_DEFAULT):
             # TODO: Deprecated branch since LS 1.5
             if cls.without_redis():
                 logger.debug('Fetch ' + project + ' from local directory')
                 job_result = cls._get_latest_job_result_from_workdir(project) or {}
             else:
                 logger.debug('Fetch ' + project + ' from Redis')
                 job_result = cls._get_latest_job_result_from_redis(project) or {}
             train_output = job_result.get('train_output')
             version = job_result.get('version')
-            return cls.get_or_create(project, label_config, force_reload, train_output, version, **kwargs)
+            return cls.get_or_create(project,ml_id, label_config, force_reload, train_output, version, **kwargs)
 
         model_version = kwargs.get('model_version')
+        ml_id = ml_id
         if not cls._current_model or model_version != cls._current_model.model_version:
             jm = cls.get_job_manager()
             model_version = kwargs.get('model_version')
             job_result = jm.get_result(model_version)
             if job_result:
                 logger.debug(f'Found job result: {job_result}')
-                model = cls.model_class(label_config=label_config, train_output=job_result, **kwargs)
+                model = cls.model_class(ml_id=ml_id,label_config=label_config, train_output=job_result, **kwargs)
                 cls._current_model = ModelWrapper(model=model, model_version=job_result['job_id'])
             else:
                 logger.debug(f'Job result not found: create initial model')
-                model = cls.model_class(label_config=label_config, **kwargs)
+                model = cls.model_class(ml_id=ml_id,label_config=label_config, **kwargs)
                 cls._current_model = ModelWrapper(model=model, model_version='INITIAL')
         return cls._current_model
 
     @classmethod
     def job_status(cls, job_id):
         job = Job.fetch(job_id, connection=cls._redis)
         response = {
```

### Comparing `wow_ai_ml-0.2.6/wow_ai_ml/server.py` & `wow_ai_ml-0.2.7/wow_ai_ml/server.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.6/wow_ai_ml/utils.py` & `wow_ai_ml-0.2.7/wow_ai_ml/utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.6/PKG-INFO` & `wow_ai_ml-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ai-ml
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.inc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

