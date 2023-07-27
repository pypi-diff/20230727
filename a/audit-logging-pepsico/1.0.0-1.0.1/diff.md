# Comparing `tmp/audit_logging_pepsico-1.0.0.tar.gz` & `tmp/audit_logging_pepsico-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audit_logging_pepsico-1.0.0.tar", last modified: Tue Jul 11 12:15:31 2023, max compression
+gzip compressed data, was "audit_logging_pepsico-1.0.1.tar", last modified: Thu Jul 27 14:18:08 2023, max compression
```

## Comparing `audit_logging_pepsico-1.0.0.tar` & `audit_logging_pepsico-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 12:15:31.585992 audit_logging_pepsico-1.0.0/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 audit_logging_pepsico-1.0.0/LICENSE
--rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-07-11 12:15:31.585702 audit_logging_pepsico-1.0.0/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 audit_logging_pepsico-1.0.0/README.md
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 12:15:31.580128 audit_logging_pepsico-1.0.0/audit_logging_pepsico/
--rw-rw-r--   0 jatintalati   (501) staff       (20)     2059 2023-05-21 21:09:26.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico/Kafka_log.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     3021 2023-05-17 06:47:52.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico/audit.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     2978 2023-05-17 06:46:50.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico/audit_config.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)      152 2023-05-02 11:42:24.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico/constants.py
--rw-rw-r--   0 jatintalati   (501) staff       (20)     5368 2023-06-09 13:25:10.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico/kafka_utilities.py
-drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-11 12:15:31.585085 audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/
--rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-07-11 12:15:31.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/PKG-INFO
--rw-r--r--   0 jatintalati   (501) staff       (20)      436 2023-07-11 12:15:31.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/SOURCES.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-07-11 12:15:31.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/dependency_links.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       35 2023-07-11 12:15:31.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/requires.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)       22 2023-07-11 12:15:31.000000 audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/top_level.txt
--rw-r--r--   0 jatintalati   (501) staff       (20)      669 2023-07-11 12:12:54.000000 audit_logging_pepsico-1.0.0/pyproject.toml
--rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-07-11 12:15:31.586109 audit_logging_pepsico-1.0.0/setup.cfg
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-27 14:18:08.229281 audit_logging_pepsico-1.0.1/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1070 2023-01-19 18:18:48.000000 audit_logging_pepsico-1.0.1/LICENSE
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-07-27 14:18:08.228990 audit_logging_pepsico-1.0.1/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1007 2023-01-19 18:54:02.000000 audit_logging_pepsico-1.0.1/README.md
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-27 14:18:08.224933 audit_logging_pepsico-1.0.1/audit_logging_pepsico/
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     2164 2023-07-27 13:57:28.000000 audit_logging_pepsico-1.0.1/audit_logging_pepsico/Kafka_log.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     3021 2023-05-17 06:47:52.000000 audit_logging_pepsico-1.0.1/audit_logging_pepsico/audit.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     2978 2023-05-17 06:46:50.000000 audit_logging_pepsico-1.0.1/audit_logging_pepsico/audit_config.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)      152 2023-05-02 11:42:24.000000 audit_logging_pepsico-1.0.1/audit_logging_pepsico/constants.py
+-rw-rw-r--   0 jatintalati   (501) staff       (20)     5368 2023-06-09 13:25:10.000000 audit_logging_pepsico-1.0.1/audit_logging_pepsico/kafka_utilities.py
+drwxr-xr-x   0 jatintalati   (501) staff       (20)        0 2023-07-27 14:18:08.228453 audit_logging_pepsico-1.0.1/audit_logging_pepsico.egg-info/
+-rw-r--r--   0 jatintalati   (501) staff       (20)     1516 2023-07-27 14:18:08.000000 audit_logging_pepsico-1.0.1/audit_logging_pepsico.egg-info/PKG-INFO
+-rw-r--r--   0 jatintalati   (501) staff       (20)      436 2023-07-27 14:18:08.000000 audit_logging_pepsico-1.0.1/audit_logging_pepsico.egg-info/SOURCES.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)        1 2023-07-27 14:18:08.000000 audit_logging_pepsico-1.0.1/audit_logging_pepsico.egg-info/dependency_links.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       35 2023-07-27 14:18:08.000000 audit_logging_pepsico-1.0.1/audit_logging_pepsico.egg-info/requires.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)       22 2023-07-27 14:18:08.000000 audit_logging_pepsico-1.0.1/audit_logging_pepsico.egg-info/top_level.txt
+-rw-r--r--   0 jatintalati   (501) staff       (20)      669 2023-07-27 14:16:39.000000 audit_logging_pepsico-1.0.1/pyproject.toml
+-rw-r--r--   0 jatintalati   (501) staff       (20)       38 2023-07-27 14:18:08.229379 audit_logging_pepsico-1.0.1/setup.cfg
```

### Comparing `audit_logging_pepsico-1.0.0/LICENSE` & `audit_logging_pepsico-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-1.0.0/PKG-INFO` & `audit_logging_pepsico-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audit_logging_pepsico
-Version: 1.0.0
+Version: 1.0.1
 Summary: A logging package which allows users to log in pepsico format. Specially write logs for request and response.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: logging,audit,pepsico,kafka,couchbase
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `audit_logging_pepsico-1.0.0/README.md` & `audit_logging_pepsico-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-1.0.0/audit_logging_pepsico/Kafka_log.py` & `audit_logging_pepsico-1.0.1/audit_logging_pepsico/Kafka_log.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 import json
 
 class KafkaAuditLog:
     def produce_log(self, logger, ip_address=None, channelId=None, systemId=None, customerId=None,
                     userId=None, url=None, operationName=None, orderId=None, coRelationId=None,
                     sourceOrderNumber=None, externalId=None, requestHeader=None, responseCode=None, documentType=None,
                     componentName=None, methodName=None, requestInput=None, responseOutput=None, gpid=None, route=None,
-                    kafka_producer=None, kafka_topic=None):
+                    kafka_producer=None, kafka_topic=None, interfaceName=None):
         try:
             ip_addr = ip_address
             id = con.AUDIT_PRIFIX + con.ID_DELIMITER + str(uuid.uuid4())
-            createdDate = str(datetime.now())
-            interfaceName = con.INTERFACE_NAME
+            createdDate = str(datetime.now().date()) + "T" + str(datetime.now().time())
+            if interfaceName is None:
+                interfaceName = con.INTERFACE_NAME
             log_type = con.AUDIT_SERVICE
             audit_obj = Audit(id, channelId, systemId, ip_addr,
                               userId, customerId, createdDate, url, interfaceName, operationName, orderId,
                               coRelationId, sourceOrderNumber,
                               externalId, requestHeader, responseCode, log_type, documentType, componentName,
                               methodName, requestInput, responseOutput, gpid, route)
             logs = audit_obj.__dict__
```

### Comparing `audit_logging_pepsico-1.0.0/audit_logging_pepsico/audit.py` & `audit_logging_pepsico-1.0.1/audit_logging_pepsico/audit.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-1.0.0/audit_logging_pepsico/audit_config.py` & `audit_logging_pepsico-1.0.1/audit_logging_pepsico/audit_config.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-1.0.0/audit_logging_pepsico/kafka_utilities.py` & `audit_logging_pepsico-1.0.1/audit_logging_pepsico/kafka_utilities.py`

 * *Files identical despite different names*

### Comparing `audit_logging_pepsico-1.0.0/audit_logging_pepsico.egg-info/PKG-INFO` & `audit_logging_pepsico-1.0.1/audit_logging_pepsico.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audit-logging-pepsico
-Version: 1.0.0
+Version: 1.0.1
 Summary: A logging package which allows users to log in pepsico format. Specially write logs for request and response.
 Author-email: Jatin Talati <jatalati@in.ibm.com>
 Keywords: logging,audit,pepsico,kafka,couchbase
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `audit_logging_pepsico-1.0.0/pyproject.toml` & `audit_logging_pepsico-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "audit_logging_pepsico"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Jatin Talati", email="jatalati@in.ibm.com" },
 ]
 description = "A logging package which allows users to log in pepsico format. Specially write logs for request and response."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["logging", "audit", "pepsico", "kafka", "couchbase"]
```

