# Comparing `tmp/dkist-service-configuration-1.0.0rc2.tar.gz` & `tmp/dkist-service-configuration-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-service-configuration-1.0.0rc2.tar", last modified: Wed Jul 26 21:52:30 2023, max compression
+gzip compressed data, was "dkist-service-configuration-1.0.0rc3.tar", last modified: Wed Jul 26 22:19:55 2023, max compression
```

## Comparing `dkist-service-configuration-1.0.0rc2.tar` & `dkist-service-configuration-1.0.0rc3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 21:52:30.982607 dkist-service-configuration-1.0.0rc2/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-26 21:52:30.982607 dkist-service-configuration-1.0.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1394 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 21:52:30.982607 dkist-service-configuration-1.0.0rc2/dkist_service_configuration/
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/dkist_service_configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/dkist_service_configuration/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1735 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/dkist_service_configuration/settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 21:52:30.982607 dkist-service-configuration-1.0.0rc2/dkist_service_configuration/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/dkist_service_configuration/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/dkist_service_configuration/tests/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/dkist_service_configuration/tests/test_settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 21:52:30.982607 dkist-service-configuration-1.0.0rc2/dkist_service_configuration.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-26 21:52:30.000000 dkist-service-configuration-1.0.0rc2/dkist_service_configuration.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-07-26 21:52:30.000000 dkist-service-configuration-1.0.0rc2/dkist_service_configuration.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 21:52:30.000000 dkist-service-configuration-1.0.0rc2/dkist_service_configuration.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-26 21:52:30.000000 dkist-service-configuration-1.0.0rc2/dkist_service_configuration.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-26 21:52:30.000000 dkist-service-configuration-1.0.0rc2/dkist_service_configuration.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-07-26 21:52:30.982607 dkist-service-configuration-1.0.0rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-26 21:52:15.000000 dkist-service-configuration-1.0.0rc2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 22:19:55.312128 dkist-service-configuration-1.0.0rc3/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-26 22:19:55.312128 dkist-service-configuration-1.0.0rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 22:19:55.308128 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 22:19:55.312128 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/tests/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration/tests/test_settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 22:19:55.312128 dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-26 22:19:55.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      631 2023-07-26 22:19:55.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 22:19:55.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-26 22:19:55.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-07-26 22:19:55.000000 dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-26 22:19:55.312128 dkist-service-configuration-1.0.0rc3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-26 22:19:39.000000 dkist-service-configuration-1.0.0rc3/setup.py
```

### Comparing `dkist-service-configuration-1.0.0rc2/.gitignore` & `dkist-service-configuration-1.0.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc2/.pre-commit-config.yaml` & `dkist-service-configuration-1.0.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc2/LICENSE` & `dkist-service-configuration-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc2/PKG-INFO` & `dkist-service-configuration-1.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-service-configuration
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Configuration support for DKIST services
 Home-page: https://bitbucket.org/dkistdc/dkist_service_configuration/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-service-configuration-1.0.0rc2/README.rst` & `dkist-service-configuration-1.0.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc2/bitbucket-pipelines.yml` & `dkist-service-configuration-1.0.0rc3/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc2/dkist_service_configuration/logging.py` & `dkist-service-configuration-1.0.0rc3/dkist_service_configuration/logging.py`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc2/dkist_service_configuration/settings.py` & `dkist-service-configuration-1.0.0rc3/dkist_service_configuration/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 """
 Wrapper for retrieving configurations and safely logging their retrieval
 """
 import re
 
 from pydantic import BaseModel
+from pydantic import BaseSettings
 from pydantic import Field
-from pydantic_settings import BaseSettings
-from pydantic_settings import SettingsConfigDict
 
 from dkist_service_configuration.logging import logger
 
 
 class ConfigurationBase(BaseSettings):
     """Settings base which logs configured settings while censoring secrets"""
 
-    log_level: str = Field("INFO", validation_alias="LOGURU_LEVEL")
+    log_level: str = Field("INFO", env="LOGURU_LEVEL")
+    # env -> validation_alias in pydantic 2.x
 
-    model_config = SettingsConfigDict(env_file=".env", env_file_encoding="utf-8")
+    class Config:
+        env_file = ".env"
+        env_file_encoding = "utf-8"
+
+    # model_config = SettingsConfigDict(env_file=".env", env_file_encoding="utf-8") in pydantic 2.x
 
     @staticmethod
     def _is_secret(field_name: str) -> bool:
         for pattern in ("pass", "secret", "token"):
             if re.search(pattern, field_name):
                 return True
         return False
 
     def log_configurations(self):
-        for field_name in self.model_fields:
+        for field_name in self.__fields__:  # __fields__ -> model_fields in pydantic 2.x
             if self._is_secret(field_name=field_name):
                 logger.info(f"{field_name}: <CENSORED>")
             logger.info(f"{field_name}: {getattr(self, field_name)}")
 
 
 class MeshService(BaseModel):
     """Model of the metadata for a node in the service mesh"""
@@ -44,12 +48,12 @@
     Settings base for services using a mesh configuration to define connections in the form
     {
         "upstream_service_name": {"mesh_address": "localhost", "mesh_port": 6742}
     }
     """
 
     service_mesh: dict[str, MeshService] = Field(
-        default_factory=dict, validation_alias="MESH_CONFIG"
-    )
+        default_factory=dict, env="MESH_CONFIG"
+    )  # env -> validation_alias when going to pydantic 2.x
 
     def service_mesh_detail(self, service_name) -> MeshService | None:
         return self.service_mesh.get(service_name)
```

### Comparing `dkist-service-configuration-1.0.0rc2/dkist_service_configuration/tests/test_settings.py` & `dkist-service-configuration-1.0.0rc3/dkist_service_configuration/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc2/dkist_service_configuration.egg-info/PKG-INFO` & `dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-service-configuration
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Configuration support for DKIST services
 Home-page: https://bitbucket.org/dkistdc/dkist_service_configuration/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-service-configuration-1.0.0rc2/dkist_service_configuration.egg-info/SOURCES.txt` & `dkist-service-configuration-1.0.0rc3/dkist_service_configuration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-service-configuration-1.0.0rc2/setup.cfg` & `dkist-service-configuration-1.0.0rc3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 [options]
 python_requires = >=3.10
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
 	loguru
-	pydantic-settings
+	pydantic < 2.0
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 
 [tool:pytest]
```

