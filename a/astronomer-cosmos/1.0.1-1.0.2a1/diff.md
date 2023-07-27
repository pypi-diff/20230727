# Comparing `tmp/astronomer_cosmos-1.0.1.tar.gz` & `tmp/astronomer_cosmos-1.0.2a1.tar.gz`

## Comparing `astronomer_cosmos-1.0.1.tar` & `astronomer_cosmos-1.0.2a1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/__init__.py
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/config.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/constants.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/converter.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dataset.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/airflow/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/airflow/dag.py
--rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/airflow/graph.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/airflow/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/core/__init__.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/executable.py
--rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/graph.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/project.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/selector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/parser/__init__.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/parser/output.py
--rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/parser/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/hooks/__init__.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/hooks/subprocess.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/__init__.py
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/base.py
--rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/docker.py
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/kubernetes.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/lazy_load.py
--rw-r--r--   0        0        0    18147 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/local.py
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/virtualenv.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/__init__.py
--rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/base.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/bigquery/service_account_keyfile_dict.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/databricks/token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/snowflake/user_privatekey.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/spark/thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/trino/base.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/trino/ldap.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/LICENSE
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/README.rst
--rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/__init__.py
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/config.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/constants.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/converter.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dataset.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/airflow/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/airflow/dag.py
+-rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/airflow/graph.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/airflow/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/executable.py
+-rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/graph.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/project.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/parser/__init__.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/parser/output.py
+-rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/parser/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/hooks/__init__.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/hooks/subprocess.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/__init__.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/base.py
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/docker.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/kubernetes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/lazy_load.py
+-rw-r--r--   0        0        0    18147 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/local.py
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/virtualenv.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/__init__.py
+-rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/base.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/bigquery/service_account_keyfile_dict.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/snowflake/user_privatekey.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/base.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/ldap.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/LICENSE
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/README.rst
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/PKG-INFO
```

### Comparing `astronomer_cosmos-1.0.1/cosmos/__init__.py` & `astronomer_cosmos-1.0.2a1/cosmos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # type: ignore # ignores "Cannot assign to a type" MyPy error
 
 """
 Astronomer Cosmos is a library for rendering dbt workflows in Airflow.
 
 Contains dags, task groups, and operators.
 """
-__version__ = "1.0.1"
+__version__ = "1.0.2a1"
 
 from cosmos.airflow.dag import DbtDag
 from cosmos.airflow.task_group import DbtTaskGroup
 from cosmos.constants import LoadMode, TestBehavior, ExecutionMode
 from cosmos.dataset import get_dbt_dataset
 from cosmos.operators.lazy_load import MissingPackage
 from cosmos.config import (
```

### Comparing `astronomer_cosmos-1.0.1/cosmos/config.py` & `astronomer_cosmos-1.0.2a1/cosmos/config.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/constants.py` & `astronomer_cosmos-1.0.2a1/cosmos/constants.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/converter.py` & `astronomer_cosmos-1.0.2a1/cosmos/converter.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/dataset.py` & `astronomer_cosmos-1.0.2a1/cosmos/dataset.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/airflow/dag.py` & `astronomer_cosmos-1.0.2a1/cosmos/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/airflow/graph.py` & `astronomer_cosmos-1.0.2a1/cosmos/airflow/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/airflow/task_group.py` & `astronomer_cosmos-1.0.2a1/cosmos/airflow/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/core/airflow.py` & `astronomer_cosmos-1.0.2a1/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/core/graph/entities.py` & `astronomer_cosmos-1.0.2a1/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/dbt/graph.py` & `astronomer_cosmos-1.0.2a1/cosmos/dbt/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/dbt/project.py` & `astronomer_cosmos-1.0.2a1/cosmos/dbt/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/dbt/selector.py` & `astronomer_cosmos-1.0.2a1/cosmos/dbt/selector.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/dbt/parser/output.py` & `astronomer_cosmos-1.0.2a1/cosmos/dbt/parser/output.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/dbt/parser/project.py` & `astronomer_cosmos-1.0.2a1/cosmos/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/hooks/subprocess.py` & `astronomer_cosmos-1.0.2a1/cosmos/hooks/subprocess.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/operators/__init__.py` & `astronomer_cosmos-1.0.2a1/cosmos/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/operators/base.py` & `astronomer_cosmos-1.0.2a1/cosmos/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/operators/docker.py` & `astronomer_cosmos-1.0.2a1/cosmos/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/operators/kubernetes.py` & `astronomer_cosmos-1.0.2a1/cosmos/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/operators/local.py` & `astronomer_cosmos-1.0.2a1/cosmos/operators/local.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/operators/virtualenv.py` & `astronomer_cosmos-1.0.2a1/cosmos/operators/virtualenv.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/__init__.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/base.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,14 +157,21 @@
                 return value
 
         # otherwise, we don't have it - return None
         return None
 
     def __getattr__(self, name: str) -> Any:
         "If the attribute doesn't exist, try to get it from profile_args or the Airflow connection."
+        logger.info(
+            "Couldn't find attribute %s on %s. Trying to get it from `profile_args` or the Airflow connection.",
+            name,
+            self.__class__.__name__,
+        )
+
+        # if it doesn't exist, try to get it from profile_args or the Airflow connection
         attempted_value = self.get_dbt_value(name)
         if attempted_value is not None:
             return attempted_value
 
         raise AttributeError(
             f"{self.__class__.__name__} has no attribute {name}. If this is a dbt profile field, "
             f"ensure it's set either in the profile_args or the Airflow connection."
```

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/bigquery/service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/bigquery/service_account_keyfile_dict.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/bigquery/service_account_keyfile_dict.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/databricks/token.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/exasol/user_pass.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/postgres/user_pass.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/redshift/user_pass.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/snowflake/user_pass.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/snowflake/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/snowflake/user_privatekey.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/snowflake/user_privatekey.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/spark/thrift.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/trino/base.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/trino/certificate.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/trino/jwt.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/jwt.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/cosmos/profiles/trino/ldap.py` & `astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/.gitignore` & `astronomer_cosmos-1.0.2a1/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/LICENSE` & `astronomer_cosmos-1.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/README.rst` & `astronomer_cosmos-1.0.2a1/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/pyproject.toml` & `astronomer_cosmos-1.0.2a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.1/PKG-INFO` & `astronomer_cosmos-1.0.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 1.0.1
+Version: 1.0.2a1
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
```

