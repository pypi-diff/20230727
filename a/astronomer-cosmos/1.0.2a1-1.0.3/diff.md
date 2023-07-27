# Comparing `tmp/astronomer_cosmos-1.0.2a1.tar.gz` & `tmp/astronomer_cosmos-1.0.3.tar.gz`

## Comparing `astronomer_cosmos-1.0.2a1.tar` & `astronomer_cosmos-1.0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/__init__.py
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/config.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/constants.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/converter.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dataset.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/airflow/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/airflow/dag.py
--rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/airflow/graph.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/airflow/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/core/__init__.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/executable.py
--rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/graph.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/project.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/selector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/parser/__init__.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/parser/output.py
--rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/dbt/parser/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/hooks/__init__.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/hooks/subprocess.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/__init__.py
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/base.py
--rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/docker.py
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/kubernetes.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/lazy_load.py
--rw-r--r--   0        0        0    18147 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/local.py
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/operators/virtualenv.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/__init__.py
--rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/base.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/bigquery/service_account_keyfile_dict.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/databricks/token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/snowflake/user_privatekey.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/spark/thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/base.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/ldap.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/LICENSE
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/README.rst
--rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/pyproject.toml
--rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/__init__.py
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/config.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/constants.py
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/converter.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dataset.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/airflow/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/airflow/dag.py
+-rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/airflow/graph.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/airflow/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/executable.py
+-rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/graph.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/project.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/parser/__init__.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/parser/output.py
+-rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/parser/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/hooks/__init__.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/hooks/subprocess.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/__init__.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/base.py
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/docker.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/kubernetes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/lazy_load.py
+-rw-r--r--   0        0        0    18147 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/local.py
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/virtualenv.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/__init__.py
+-rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/base.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/bigquery/service_account_keyfile_dict.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/snowflake/user_privatekey.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/trino/base.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/trino/ldap.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/README.rst
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/PKG-INFO
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/__init__.py` & `astronomer_cosmos-1.0.3/cosmos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # type: ignore # ignores "Cannot assign to a type" MyPy error
 
 """
 Astronomer Cosmos is a library for rendering dbt workflows in Airflow.
 
 Contains dags, task groups, and operators.
 """
-__version__ = "1.0.2a1"
+__version__ = "1.0.3"
 
 from cosmos.airflow.dag import DbtDag
 from cosmos.airflow.task_group import DbtTaskGroup
 from cosmos.constants import LoadMode, TestBehavior, ExecutionMode
 from cosmos.dataset import get_dbt_dataset
 from cosmos.operators.lazy_load import MissingPackage
 from cosmos.config import (
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/config.py` & `astronomer_cosmos-1.0.3/cosmos/config.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/constants.py` & `astronomer_cosmos-1.0.3/cosmos/constants.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/converter.py` & `astronomer_cosmos-1.0.3/cosmos/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
         if dbt_executable_path:
             task_args["dbt_executable_path"] = dbt_executable_path
 
         validate_arguments(select, exclude, profile_args, task_args)
 
         build_airflow_graph(
-            nodes=dbt_graph.nodes,
+            nodes=dbt_graph.filtered_nodes,
             dag=dag or (task_group and task_group.dag),
             task_group=task_group,
             execution_mode=execution_mode,
             task_args=task_args,
             test_behavior=test_behavior,
             dbt_project_name=dbt_project.name,
             conn_id=conn_id,
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/dataset.py` & `astronomer_cosmos-1.0.3/cosmos/dataset.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/airflow/dag.py` & `astronomer_cosmos-1.0.3/cosmos/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/airflow/graph.py` & `astronomer_cosmos-1.0.3/cosmos/airflow/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/airflow/task_group.py` & `astronomer_cosmos-1.0.3/cosmos/airflow/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/core/airflow.py` & `astronomer_cosmos-1.0.3/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/core/graph/entities.py` & `astronomer_cosmos-1.0.3/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/dbt/graph.py` & `astronomer_cosmos-1.0.3/cosmos/dbt/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/dbt/project.py` & `astronomer_cosmos-1.0.3/cosmos/dbt/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/dbt/selector.py` & `astronomer_cosmos-1.0.3/cosmos/dbt/selector.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/dbt/parser/output.py` & `astronomer_cosmos-1.0.3/cosmos/dbt/parser/output.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/dbt/parser/project.py` & `astronomer_cosmos-1.0.3/cosmos/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/hooks/subprocess.py` & `astronomer_cosmos-1.0.3/cosmos/hooks/subprocess.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/operators/__init__.py` & `astronomer_cosmos-1.0.3/cosmos/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/operators/base.py` & `astronomer_cosmos-1.0.3/cosmos/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/operators/docker.py` & `astronomer_cosmos-1.0.3/cosmos/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/operators/kubernetes.py` & `astronomer_cosmos-1.0.3/cosmos/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/operators/local.py` & `astronomer_cosmos-1.0.3/cosmos/operators/local.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/operators/virtualenv.py` & `astronomer_cosmos-1.0.3/cosmos/operators/virtualenv.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/__init__.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/base.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,29 +54,31 @@
     def can_claim_connection(self) -> bool:
         """
         Return whether the connection is valid for this profile mapping.
         """
         if self.conn.conn_type != self.airflow_connection_type:
             return False
 
-        logger.info(dir(self.conn))
-        logger.info(self.conn.__dict__)
+        generated_profile = self.profile
 
         for field in self.required_fields:
-            try:
-                if not getattr(self, field):
+            # if it's a secret field, check if we can get it
+            if field in self.secret_fields:
+                if not self.get_dbt_value(field):
                     logger.info(
-                        "1 Not using mapping %s because %s is not set",
+                        "Not using mapping %s because %s is not set",
                         self.__class__.__name__,
                         field,
                     )
                     return False
-            except AttributeError:
+
+            # otherwise, check if it's in the generated profile
+            if not generated_profile.get(field):
                 logger.info(
-                    "2 Not using mapping %s because %s is not set",
+                    "Not using mapping %s because %s is not set",
                     self.__class__.__name__,
                     field,
                 )
                 return False
 
         return True
 
@@ -155,31 +157,23 @@
                     return getattr(self, f"transform_{name}")(value)
 
                 return value
 
         # otherwise, we don't have it - return None
         return None
 
-    def __getattr__(self, name: str) -> Any:
-        "If the attribute doesn't exist, try to get it from profile_args or the Airflow connection."
-        logger.info(
-            "Couldn't find attribute %s on %s. Trying to get it from `profile_args` or the Airflow connection.",
-            name,
-            self.__class__.__name__,
-        )
-
-        # if it doesn't exist, try to get it from profile_args or the Airflow connection
-        attempted_value = self.get_dbt_value(name)
-        if attempted_value is not None:
-            return attempted_value
-
-        raise AttributeError(
-            f"{self.__class__.__name__} has no attribute {name}. If this is a dbt profile field, "
-            f"ensure it's set either in the profile_args or the Airflow connection."
-        )
+    @property
+    def mapped_params(self) -> dict[str, Any]:
+        "Turns the self.airflow_param_mapping into a dictionary of dbt fields and their values."
+        mapped_params = {}
+
+        for dbt_field in self.airflow_param_mapping:
+            mapped_params[dbt_field] = self.get_dbt_value(dbt_field)
+
+        return mapped_params
 
     @classmethod
     def filter_null(cls, args: dict[str, Any]) -> dict[str, Any]:
         """
         Filters out null values from a dictionary.
         """
         return {k: v for k, v in args.items() if v is not None}
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/bigquery/service_account_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,13 @@
         "keyfile": "extra.key_path",
     }
 
     @property
     def profile(self) -> dict[str, Any | None]:
         "Generates profile. Defaults `threads` to 1."
         return {
+            **self.mapped_params,
             "type": "bigquery",
             "method": "service-account",
-            "project": self.project,
-            "dataset": self.dataset,
-            "threads": self.profile_args.get("threads") or 1,
-            "keyfile": self.keyfile,
+            "threads": 1,
             **self.profile_args,
         }
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/bigquery/service_account_keyfile_dict.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/bigquery/service_account_keyfile_dict.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,34 +15,32 @@
     """
 
     airflow_connection_type: str = "google_cloud_platform"
 
     required_fields = [
         "project",
         "dataset",
-        "keyfile_dict",
+        "keyfile_json",
     ]
 
     airflow_param_mapping = {
         "project": "extra.project",
         # multiple options for dataset because of older Airflow versions
-        "dataset": ["extra.dataset", "dataset"],
+        "dataset": "extra.dataset",
         # multiple options for keyfile_dict param name because of older Airflow versions
-        "keyfile_dict": ["extra.keyfile_dict", "keyfile_dict", "extra__google_cloud_platform__keyfile_dict"],
+        "keyfile_json": ["extra.keyfile_dict", "keyfile_dict", "extra__google_cloud_platform__keyfile_dict"],
     }
 
     @property
     def profile(self) -> dict[str, Any | None]:
         """
         Generates a GCP profile.
         Even though the Airflow connection contains hard-coded Service account credentials,
         we generate a temporary file and the DBT profile uses it.
         """
         return {
+            **self.mapped_params,
             "type": "bigquery",
             "method": "service-account-json",
-            "project": self.project,
-            "dataset": self.dataset,
-            "threads": self.profile_args.get("threads") or 1,
-            "keyfile_json": self.keyfile_dict,
+            "threads": 1,
             **self.profile_args,
         }
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/databricks/token.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/databricks/token.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,18 +34,16 @@
         "http_path": "extra.http_path",
     }
 
     @property
     def profile(self) -> dict[str, Any | None]:
         "Generates profile. The token is stored in an environment variable."
         return {
+            **self.mapped_params,
             "type": "databricks",
-            "schema": self.schema,
-            "host": self.host,
-            "http_path": self.http_path,
             **self.profile_args,
             # token should always get set as env var
             "token": self.get_env_var_format("token"),
         }
 
     def transform_host(self, host: str) -> str:
         "Removes the https:// prefix."
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/exasol/user_pass.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/postgres/user_pass.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,50 @@
-"Maps Airflow Exasol connections with a username and password to dbt profiles."
+"Maps Airflow Postgres connections using user + password authentication to dbt profiles."
 from __future__ import annotations
 
 from typing import Any
 
 from ..base import BaseProfileMapping
 
 
-class ExasolUserPasswordProfileMapping(BaseProfileMapping):
+class PostgresUserPasswordProfileMapping(BaseProfileMapping):
     """
-    Maps Airflow Exasol connections with a username and password to dbt profiles.
-    https://docs.getdbt.com/reference/warehouse-setups/exasol-setup
+    Maps Airflow Postgres connections using user + password authentication to dbt profiles.
+    https://docs.getdbt.com/reference/warehouse-setups/postgres-setup
+    https://airflow.apache.org/docs/apache-airflow-providers-postgres/stable/connections/postgres.html
     """
 
-    airflow_connection_type: str = "exasol"
-    is_community: bool = True
-
-    default_port: int = 8563
+    airflow_connection_type: str = "postgres"
 
     required_fields = [
-        "threads",
-        "dsn",
+        "host",
         "user",
         "password",
         "dbname",
         "schema",
     ]
-
     secret_fields = [
         "password",
     ]
-
     airflow_param_mapping = {
-        "dsn": "host",
+        "host": "host",
         "user": "login",
         "password": "password",
+        "port": "port",
         "dbname": "schema",
-        "encryption": "extra.encryption",
-        "compression": "extra.compression",
-        "connection_timeout": "extra.connection_timeout",
-        "socket_timeout": "extra.socket_timeout",
-        "protocol_version": "extra.protocol_version",
+        "keepalives_idle": "extra.keepalives_idle",
+        "sslmode": "extra.sslmode",
     }
 
     @property
     def profile(self) -> dict[str, Any | None]:
         "Gets profile. The password is stored in an environment variable."
-        profile_vars = {
-            "type": "exasol",
-            "threads": self.threads,
-            "dsn": self.dsn,
-            "user": self.user,
-            "dbname": self.dbname,
-            "schema": self.schema,
-            "encryption": self.conn.extra_dejson.get("encryption"),
-            "compression": self.conn.extra_dejson.get("compression"),
-            "connect_timeout": self.conn.extra_dejson.get("connection_timeout"),
-            "socket_timeout": self.conn.extra_dejson.get("socket_timeout"),
-            "protocol_version": self.conn.extra_dejson.get("protocol_version"),
+        profile = {
+            **self.mapped_params,
+            "type": "postgres",
+            "port": 5432,
             **self.profile_args,
             # password should always get set as env var
             "password": self.get_env_var_format("password"),
         }
 
-        # remove any null values
-        return self.filter_null(profile_vars)
-
-    def transform_dsn(self, host: str) -> str:
-        "Adds the port if it's not already there."
-        if ":" not in host:
-            port = self.conn.port or self.default_port
-            return f"{host}:{port}"
-
-        return host
+        return self.filter_null(profile)
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/postgres/user_pass.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/exasol/user_pass.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,65 @@
-"Maps Airflow Postgres connections using user + password authentication to dbt profiles."
+"Maps Airflow Exasol connections with a username and password to dbt profiles."
 from __future__ import annotations
 
 from typing import Any
 
 from ..base import BaseProfileMapping
 
 
-class PostgresUserPasswordProfileMapping(BaseProfileMapping):
+class ExasolUserPasswordProfileMapping(BaseProfileMapping):
     """
-    Maps Airflow Postgres connections using user + password authentication to dbt profiles.
-    https://docs.getdbt.com/reference/warehouse-setups/postgres-setup
-    https://airflow.apache.org/docs/apache-airflow-providers-postgres/stable/connections/postgres.html
+    Maps Airflow Exasol connections with a username and password to dbt profiles.
+    https://docs.getdbt.com/reference/warehouse-setups/exasol-setup
     """
 
-    airflow_connection_type: str = "postgres"
-    default_port = 5432
+    airflow_connection_type: str = "exasol"
+    is_community: bool = True
+
+    default_port: int = 8563
 
     required_fields = [
-        "host",
+        "threads",
+        "dsn",
         "user",
         "password",
-        "port",
         "dbname",
         "schema",
     ]
+
     secret_fields = [
         "password",
     ]
+
     airflow_param_mapping = {
-        "host": "host",
+        "dsn": "host",
         "user": "login",
         "password": "password",
-        "port": "port",
         "dbname": "schema",
-        "keepalives_idle": "extra.keepalives_idle",
-        "sslmode": "extra.sslmode",
+        "encryption": "extra.encryption",
+        "compression": "extra.compression",
+        "connection_timeout": "extra.connection_timeout",
+        "socket_timeout": "extra.socket_timeout",
+        "protocol_version": "extra.protocol_version",
     }
 
     @property
     def profile(self) -> dict[str, Any | None]:
         "Gets profile. The password is stored in an environment variable."
-        profile = {
-            "type": "postgres",
-            "host": self.conn.host,
-            "user": self.conn.login,
-            "port": self.conn.port or self.default_port,
-            "dbname": self.dbname,
-            "schema": self.schema,
-            "keepalives_idle": self.conn.extra_dejson.get("keepalives_idle"),
-            "sslmode": self.conn.extra_dejson.get("sslmode"),
+        profile_vars = {
+            **self.mapped_params,
+            "type": "exasol",
             **self.profile_args,
             # password should always get set as env var
             "password": self.get_env_var_format("password"),
         }
 
-        return self.filter_null(profile)
+        # remove any null values
+        return self.filter_null(profile_vars)
+
+    def transform_dsn(self, host: str) -> str:
+        "Adds the port if it's not already there."
+        if ":" not in host:
+            port = self.conn.port or self.default_port
+            return f"{host}:{port}"
+
+        return host
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/redshift/user_pass.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/redshift/user_pass.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     """
     Maps Airflow Redshift connections to dbt Redshift profiles if they use a username and password.
     https://docs.getdbt.com/reference/warehouse-setups/redshift-setup
     https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/connections/redshift.html
     """
 
     airflow_connection_type: str = "redshift"
-    default_port = 5432
 
     required_fields = [
         "host",
         "user",
         "password",
         "dbname",
         "schema",
@@ -37,21 +36,16 @@
         "region": "extra.region",
     }
 
     @property
     def profile(self) -> dict[str, Any | None]:
         "Gets profile."
         profile = {
+            **self.mapped_params,
             "type": "redshift",
-            "host": self.host,
-            "user": self.user,
-            "password": self.get_env_var_format("password"),
-            "port": self.port or self.default_port,
-            "dbname": self.dbname,
-            "schema": self.schema,
-            "connection_timeout": self.conn.extra_dejson.get("timeout"),
-            "sslmode": self.conn.extra_dejson.get("sslmode"),
-            "region": self.conn.extra_dejson.get("region"),
+            "port": 5439,
             **self.profile_args,
+            # password should always get set as env var
+            "password": self.get_env_var_format("password"),
         }
 
         return self.filter_null(profile)
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/snowflake/user_pass.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/snowflake/user_pass.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,21 +59,16 @@
 
         return conn
 
     @property
     def profile(self) -> dict[str, Any | None]:
         "Gets profile."
         profile_vars = {
+            **self.mapped_params,
             "type": "snowflake",
-            "account": self.account,
-            "user": self.user,
-            "schema": self.schema,
-            "database": self.database,
-            "role": self.conn.extra_dejson.get("role"),
-            "warehouse": self.conn.extra_dejson.get("warehouse"),
             **self.profile_args,
             # password should always get set as env var
             "password": self.get_env_var_format("password"),
         }
 
         # remove any null values
         return self.filter_null(profile_vars)
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/snowflake/user_privatekey.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/snowflake/user_privatekey.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,21 +60,16 @@
 
         return conn
 
     @property
     def profile(self) -> dict[str, Any | None]:
         "Gets profile."
         profile_vars = {
+            **self.mapped_params,
             "type": "snowflake",
-            "account": self.account,
-            "user": self.user,
-            "schema": self.schema,
-            "database": self.database,
-            "role": self.conn.extra_dejson.get("role"),
-            "warehouse": self.conn.extra_dejson.get("warehouse"),
             **self.profile_args,
             # private_key should always get set as env var
             "private_key_content": self.get_env_var_format("private_key_content"),
         }
 
         # remove any null values
         return self.filter_null(profile_vars)
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/spark/thrift.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/spark/thrift.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,25 +19,24 @@
     required_fields = [
         "schema",
         "host",
     ]
 
     airflow_param_mapping = {
         "host": "host",
+        "port": "port",
     }
 
     @property
     def profile(self) -> dict[str, Any | None]:
         """
         Return a dbt Spark profile based on the Airflow Spark connection.
         """
         profile_vars = {
+            **self.mapped_params,
             "type": "spark",
             "method": "thrift",
-            "schema": self.schema,
-            "host": self.host,
-            "port": self.conn.port,
             **self.profile_args,
         }
 
         # remove any null values
         return self.filter_null(profile_vars)
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/base.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/trino/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,23 +22,19 @@
     airflow_param_mapping = {
         "host": "host",
         "port": "port",
         "session_properties": "extra.session_properties",
     }
 
     @property
-    def profile(self) -> dict[str, Any | None]:
+    def profile(self) -> dict[str, Any]:
         "Gets profile."
         profile_vars = {
+            **self.mapped_params,
             "type": "trino",
-            "host": self.host,
-            "port": self.port,
-            "database": self.database,
-            "schema": self.schema,
-            "session_properties": self.conn.extra_dejson.get("session_properties"),
             **self.profile_args,
         }
 
         # remove any null values
         return self.filter_null(profile_vars)
 
     def transform_host(self, host: str) -> str:
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/certificate.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/trino/certificate.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     }
 
     @property
     def profile(self) -> dict[str, Any | None]:
         "Gets profile."
         common_profile_vars = super().profile
         profile_vars = {
+            **self.mapped_params,
             **common_profile_vars,
             "method": "certificate",
-            "client_certificate": self.client_certificate,
-            "client_private_key": self.client_private_key,
             **self.profile_args,
         }
 
         # remove any null values
         return self.filter_null(profile_vars)
```

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/jwt.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/trino/jwt.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/cosmos/profiles/trino/ldap.py` & `astronomer_cosmos-1.0.3/cosmos/profiles/trino/ldap.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,16 +30,17 @@
     @property
     def profile(self) -> dict[str, Any | None]:
         """
         Returns a dbt Trino profile based on the Airflow Trino connection.
         """
         common_profile_vars = super().profile
         profile_vars = {
+            **self.mapped_params,
             **common_profile_vars,
             "method": "ldap",
-            "user": self.user,
-            "password": self.get_env_var_format("password"),
             **self.profile_args,
+            # password should always get set as env var
+            "password": self.get_env_var_format("password"),
         }
 
         # remove any null values
         return self.filter_null(profile_vars)
```

### Comparing `astronomer_cosmos-1.0.2a1/.gitignore` & `astronomer_cosmos-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/LICENSE` & `astronomer_cosmos-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/README.rst` & `astronomer_cosmos-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/pyproject.toml` & `astronomer_cosmos-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.2a1/PKG-INFO` & `astronomer_cosmos-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 1.0.2a1
+Version: 1.0.3
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
```

