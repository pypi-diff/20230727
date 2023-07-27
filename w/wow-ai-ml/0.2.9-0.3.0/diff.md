# Comparing `tmp/wow_ai_ml-0.2.9.tar.gz` & `tmp/wow_ai_ml-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wow_ai_ml-0.2.9.tar", max compression
+gzip compressed data, was "wow_ai_ml-0.3.0.tar", max compression
```

## Comparing `wow_ai_ml-0.2.9.tar` & `wow_ai_ml-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.2.9/README.md
--rw-r--r--   0        0        0      261 2023-07-27 05:04:09.940002 wow_ai_ml-0.2.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.2.9/wow_ai_ml/__init__.py
--rw-r--r--   0        0        0     8994 2023-07-27 04:07:14.832928 wow_ai_ml-0.2.9/wow_ai_ml/api.py
--rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.2.9/wow_ai_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.2.9/wow_ai_ml/default_configs/README.md
--rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.2.9/wow_ai_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.2.9/wow_ai_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.2.9/wow_ai_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.2.9/wow_ai_ml/exceptions.py
--rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.2.9/wow_ai_ml/helpers.py
--rw-r--r--   0        0        0    34852 2023-07-27 05:03:25.508738 wow_ai_ml-0.2.9/wow_ai_ml/model.py
--rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.2.9/wow_ai_ml/server.py
--rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.2.9/wow_ai_ml/templates/preview.html
--rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.2.9/wow_ai_ml/utils.py
--rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     6415 2023-02-14 16:37:26.303084 wow_ai_ml-0.3.0/README.md
+-rw-r--r--   0        0        0      261 2023-07-27 05:59:47.460067 wow_ai_ml-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-30 05:04:46.921613 wow_ai_ml-0.3.0/wow_ai_ml/__init__.py
+-rw-r--r--   0        0        0     8994 2023-07-27 04:07:14.832928 wow_ai_ml-0.3.0/wow_ai_ml/api.py
+-rw-r--r--   0        0        0      267 2023-01-29 17:47:59.351874 wow_ai_ml-0.3.0/wow_ai_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2701 2023-01-29 17:47:59.457372 wow_ai_ml-0.3.0/wow_ai_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3861 2023-01-29 17:47:57.963857 wow_ai_ml-0.3.0/wow_ai_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      563 2023-01-29 17:47:59.127706 wow_ai_ml-0.3.0/wow_ai_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0       28 2023-01-29 17:47:59.904560 wow_ai_ml-0.3.0/wow_ai_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2023-01-29 17:47:56.017679 wow_ai_ml-0.3.0/wow_ai_ml/exceptions.py
+-rw-r--r--   0        0        0     2375 2023-01-29 17:48:02.301568 wow_ai_ml-0.3.0/wow_ai_ml/helpers.py
+-rw-r--r--   0        0        0    34792 2023-07-27 05:52:57.890563 wow_ai_ml-0.3.0/wow_ai_ml/model.py
+-rw-r--r--   0        0        0     7542 2023-01-29 17:48:02.879893 wow_ai_ml-0.3.0/wow_ai_ml/server.py
+-rw-r--r--   0        0        0        6 2023-02-01 14:28:47.129345 wow_ai_ml-0.3.0/wow_ai_ml/templates/preview.html
+-rw-r--r--   0        0        0     1999 2023-01-29 17:48:03.663323 wow_ai_ml-0.3.0/wow_ai_ml/utils.py
+-rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 wow_ai_ml-0.3.0/PKG-INFO
```

### Comparing `wow_ai_ml-0.2.9/README.md` & `wow_ai_ml-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.9/wow_ai_ml/api.py` & `wow_ai_ml-0.3.0/wow_ai_ml/api.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.9/wow_ai_ml/default_configs/README.md` & `wow_ai_ml-0.3.0/wow_ai_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.9/wow_ai_ml/default_configs/_wsgi.py.tmpl` & `wow_ai_ml-0.3.0/wow_ai_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.9/wow_ai_ml/default_configs/docker-compose.yml` & `wow_ai_ml-0.3.0/wow_ai_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.9/wow_ai_ml/exceptions.py` & `wow_ai_ml-0.3.0/wow_ai_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.9/wow_ai_ml/helpers.py` & `wow_ai_ml-0.3.0/wow_ai_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.9/wow_ai_ml/model.py` & `wow_ai_ml-0.3.0/wow_ai_ml/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,22 +486,20 @@
     def create(cls, project=None,ml_id=None, label_config=None, train_output=None, version=None, **kwargs):
         key = cls._key(project)
         logger.debug('Create project ' + str(key))
         kwargs.update(cls.init_kwargs)
         if not os.getenv('LABEL_STUDIO_ML_BACKEND_V2', default=LABEL_STUDIO_ML_BACKEND_V2_DEFAULT):
             # TODO: Deprecated branch since LS 1.5
             cls._current_model[key] = ModelWrapper(
-                ml_id=ml_id,
                 model=cls.model_class(ml_id=ml_id,label_config=label_config, train_output=train_output, **kwargs),
                 model_version=version or cls._generate_version()
             )
             return cls._current_model[key]
         else:
             cls._current_model = ModelWrapper(
-                ml_id=ml_id,
                 model=cls.model_class(ml_id=ml_id,label_config=label_config, train_output=train_output, **kwargs),
                 model_version=version or cls._generate_version()
             )
             return cls._current_model
 
     @classmethod
     def get_or_create(
```

### Comparing `wow_ai_ml-0.2.9/wow_ai_ml/server.py` & `wow_ai_ml-0.3.0/wow_ai_ml/server.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.9/wow_ai_ml/utils.py` & `wow_ai_ml-0.3.0/wow_ai_ml/utils.py`

 * *Files identical despite different names*

### Comparing `wow_ai_ml-0.2.9/PKG-INFO` & `wow_ai_ml-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wow-ai-ml
-Version: 0.2.9
+Version: 0.3.0
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.inc
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

