# Comparing `tmp/astronomer_cosmos-1.0.0.tar.gz` & `tmp/astronomer_cosmos-1.0.1.tar.gz`

## Comparing `astronomer_cosmos-1.0.0.tar` & `astronomer_cosmos-1.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/__init__.py
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/config.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/constants.py
--rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/converter.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dataset.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/airflow/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/airflow/dag.py
--rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/airflow/graph.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/airflow/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/core/__init__.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/executable.py
--rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/graph.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/project.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/selector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/parser/__init__.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/parser/output.py
--rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/dbt/parser/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/hooks/__init__.py
--rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/hooks/subprocess.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/__init__.py
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/base.py
--rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/docker.py
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/kubernetes.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/lazy_load.py
--rw-r--r--   0        0        0    18067 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/local.py
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/operators/virtualenv.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/__init__.py
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/base.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/bigquery/service_account_keyfile_dict.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/databricks/token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/snowflake/user_privatekey.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/spark/thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/trino/base.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/cosmos/profiles/trino/ldap.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/LICENSE
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/README.rst
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7004 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/__init__.py
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/config.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/constants.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/converter.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dataset.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/airflow/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/airflow/dag.py
+-rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/airflow/graph.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/airflow/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/executable.py
+-rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/graph.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/project.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/parser/__init__.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/parser/output.py
+-rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/dbt/parser/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/hooks/__init__.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/hooks/subprocess.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/__init__.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/base.py
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/docker.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/kubernetes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/lazy_load.py
+-rw-r--r--   0        0        0    18147 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/local.py
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/operators/virtualenv.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/__init__.py
+-rw-r--r--   0        0        0     6355 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/base.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/bigquery/service_account_keyfile_dict.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/snowflake/user_privatekey.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/trino/base.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/cosmos/profiles/trino/ldap.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/README.rst
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.1/PKG-INFO
```

### Comparing `astronomer_cosmos-1.0.0/cosmos/__init__.py` & `astronomer_cosmos-1.0.1/cosmos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # type: ignore # ignores "Cannot assign to a type" MyPy error
 
 """
 Astronomer Cosmos is a library for rendering dbt workflows in Airflow.
 
 Contains dags, task groups, and operators.
 """
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from cosmos.airflow.dag import DbtDag
 from cosmos.airflow.task_group import DbtTaskGroup
 from cosmos.constants import LoadMode, TestBehavior, ExecutionMode
 from cosmos.dataset import get_dbt_dataset
 from cosmos.operators.lazy_load import MissingPackage
 from cosmos.config import (
```

### Comparing `astronomer_cosmos-1.0.0/cosmos/config.py` & `astronomer_cosmos-1.0.1/cosmos/config.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/constants.py` & `astronomer_cosmos-1.0.1/cosmos/constants.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/converter.py` & `astronomer_cosmos-1.0.1/cosmos/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,17 @@
         task_args = {
             **operator_args,
             # the following args may be only needed for local / venv:
             "project_dir": dbt_project.dir,
             "profile_config": profile_config,
         }
 
+        if dbt_executable_path:
+            task_args["dbt_executable_path"] = dbt_executable_path
+
         validate_arguments(select, exclude, profile_args, task_args)
 
         build_airflow_graph(
             nodes=dbt_graph.nodes,
             dag=dag or (task_group and task_group.dag),
             task_group=task_group,
             execution_mode=execution_mode,
```

### Comparing `astronomer_cosmos-1.0.0/cosmos/dataset.py` & `astronomer_cosmos-1.0.1/cosmos/dataset.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/airflow/dag.py` & `astronomer_cosmos-1.0.1/cosmos/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/airflow/graph.py` & `astronomer_cosmos-1.0.1/cosmos/airflow/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/core/airflow.py` & `astronomer_cosmos-1.0.1/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/core/graph/entities.py` & `astronomer_cosmos-1.0.1/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/dbt/graph.py` & `astronomer_cosmos-1.0.1/cosmos/dbt/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,18 +98,15 @@
             LoadMode.DBT_LS: self.load_via_dbt_ls,
             LoadMode.DBT_MANIFEST: self.load_from_dbt_manifest,
         }
         if method == LoadMode.AUTOMATIC:
             if self.project.is_manifest_available():
                 self.load_from_dbt_manifest()
                 return
-            elif (
-                execution_mode in (ExecutionMode.LOCAL, ExecutionMode.VIRTUALENV)
-                and self.project.is_profile_yml_available()
-            ):
+            elif execution_mode == ExecutionMode.LOCAL and self.project.is_profile_yml_available():
                 try:
                     self.load_via_dbt_ls()
                     return
                 except FileNotFoundError:
                     self.load_via_custom_parser()
                     return
             else:
@@ -126,15 +123,15 @@
         This is the most accurate way of loading `dbt` projects and filtering them out, since it uses the `dbt` command
         line for both parsing and filtering the nodes.
 
         Updates in-place:
         * self.nodes
         * self.filtered_nodes
         """
-        logger.info("Trying to parse the dbt project using dbt ls...")
+        logger.info("Trying to parse the dbt project `%s` using dbt ls...", self.project.name)
 
         if not self.profile_config:
             raise CosmosLoadDbtException("Unable to load dbt project without a profile config")
 
         if not shutil.which(self.dbt_cmd):
             raise CosmosLoadDbtException(f"Unable to find the dbt executable: {self.dbt_cmd}")
 
@@ -154,25 +151,26 @@
                     "--profile",
                     self.profile_config.profile_name,
                     "--target",
                     self.profile_config.target_name,
                 ]
             )
 
+            env = os.environ.copy()
+            env.update(env_vars)
+
             logger.info("Running command: `%s`", " ".join(command))
+            logger.info("Environment variable keys: %s", env.keys())
             process = Popen(
                 command,
                 stdout=PIPE,
                 stderr=PIPE,
                 cwd=self.project.dir,
                 universal_newlines=True,
-                env={
-                    **os.environ,
-                    **env_vars,
-                },
+                env=env,
             )
 
             stdout, stderr = process.communicate()
 
         logger.debug("Output: %s", stdout)
 
         if stderr or "Runtime Error" in stdout:
@@ -208,15 +206,15 @@
         Internally, it uses the legacy Cosmos DbtProject representation and converts it to the current
         nodes list representation.
 
         Updates in-place:
         * self.nodes
         * self.filtered_nodes
         """
-        logger.info("Trying to parse the dbt project using a custom Cosmos method...")
+        logger.info("Trying to parse the dbt project `%s` using a custom Cosmos method...", self.project.name)
 
         project = LegacyDbtProject(
             dbt_root_path=str(self.project.root_dir),
             dbt_models_dir=self.project.models_dir.stem if self.project.models_dir else None,
             dbt_seeds_dir=self.project.seeds_dir.stem if self.project.seeds_dir else None,
             project_name=self.project.name,
         )
@@ -247,15 +245,15 @@
         However, since the Manifest does not represent filters, it relies on the Custom Cosmos implementation
         to filter out the nodes relevant to the user (based on self.exclude and self.select).
 
         Updates in-place:
         * self.nodes
         * self.filtered_nodes
         """
-        logger.info("Trying to parse the dbt project using a dbt manifest...")
+        logger.info("Trying to parse the dbt project `%s` using a dbt manifest...", self.project.name)
         nodes = {}
         with open(self.project.manifest_path) as fp:  # type: ignore[arg-type]
             manifest = json.load(fp)
 
             for unique_id, node_dict in manifest.get("nodes", {}).items():
                 node = DbtNode(
                     name=node_dict["name"],
```

### Comparing `astronomer_cosmos-1.0.0/cosmos/dbt/project.py` & `astronomer_cosmos-1.0.1/cosmos/dbt/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/dbt/selector.py` & `astronomer_cosmos-1.0.1/cosmos/dbt/selector.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/dbt/parser/output.py` & `astronomer_cosmos-1.0.1/cosmos/dbt/parser/output.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/dbt/parser/project.py` & `astronomer_cosmos-1.0.1/cosmos/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/hooks/subprocess.py` & `astronomer_cosmos-1.0.1/cosmos/hooks/subprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,15 @@
         If ``cwd`` is None, execute the command in a temporary directory which will be cleaned afterwards.
         If ``env`` is not supplied, ``os.environ`` is passed
 
         :param command: the command to run
         :param env: Optional dict containing environment variables to be made available to the shell
             environment in which ``command`` will be executed.  If omitted, ``os.environ`` will be used.
             Note, that in case you have Sentry configured, original variables from the environment
-            will also be passed to the subprocess with ``SUBPROCESS_`` prefix. See
-            :doc:`/administration-and-deployment/logging-monitoring/errors` for details.
+            will also be passed to the subprocess with ``SUBPROCESS_`` prefix.
         :param output_encoding: encoding to use for decoding stdout
         :param cwd: Working directory to run the command in.
             If None (default), the command is run in a temporary directory.
         :return: :class:`namedtuple` containing:
                                     ``exit_code``
                                     ``output``: the last line from stderr or stdout
                                     ``full_output``: all lines from stderr or stdout.
```

### Comparing `astronomer_cosmos-1.0.0/cosmos/operators/__init__.py` & `astronomer_cosmos-1.0.1/cosmos/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/operators/base.py` & `astronomer_cosmos-1.0.1/cosmos/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/operators/docker.py` & `astronomer_cosmos-1.0.1/cosmos/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/operators/kubernetes.py` & `astronomer_cosmos-1.0.1/cosmos/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/operators/local.py` & `astronomer_cosmos-1.0.1/cosmos/operators/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,15 @@
                     "--profile",
                     self.profile_config.profile_name,
                     "--target",
                     self.profile_config.target_name,
                 ]
 
                 logger.info("Trying to run the command:\n %s\nFrom %s", full_cmd, tmp_project_dir)
+                logger.info("Using environment variables keys: %s", env.keys())
                 result = self.run_subprocess(
                     command=full_cmd,
                     env=env,
                     output_encoding=self.output_encoding,
                     cwd=tmp_project_dir,
                 )
```

### Comparing `astronomer_cosmos-1.0.0/cosmos/operators/virtualenv.py` & `astronomer_cosmos-1.0.1/cosmos/operators/virtualenv.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/__init__.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/base.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,19 @@
     def env_vars(self) -> dict[str, str]:
         "Returns a dictionary of environment variables that should be set based on self.secret_fields."
         env_vars = {}
 
         for field in self.secret_fields:
             env_var_name = self.get_env_var_name(field)
             value = self.get_dbt_value(field)
-            if value is not None:
-                env_vars[env_var_name] = str(value)
+
+            if value is None:
+                raise CosmosValueError(f"Could not find a value for secret field {field}.")
+
+            env_vars[env_var_name] = str(value)
 
         return env_vars
 
     def get_profile_file_contents(self, profile_name: str, target_name: str = "cosmos_target") -> str:
         """
         Translates the profile into a string that can be written to a profiles.yml file.
         """
@@ -158,15 +161,18 @@
 
     def __getattr__(self, name: str) -> Any:
         "If the attribute doesn't exist, try to get it from profile_args or the Airflow connection."
         attempted_value = self.get_dbt_value(name)
         if attempted_value is not None:
             return attempted_value
 
-        raise AttributeError
+        raise AttributeError(
+            f"{self.__class__.__name__} has no attribute {name}. If this is a dbt profile field, "
+            f"ensure it's set either in the profile_args or the Airflow connection."
+        )
 
     @classmethod
     def filter_null(cls, args: dict[str, Any]) -> dict[str, Any]:
         """
         Filters out null values from a dictionary.
         """
         return {k: v for k, v in args.items() if v is not None}
```

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/bigquery/service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/bigquery/service_account_keyfile_dict.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/bigquery/service_account_keyfile_dict.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/databricks/token.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/exasol/user_pass.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/postgres/user_pass.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/redshift/user_pass.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/snowflake/user_pass.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/snowflake/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/snowflake/user_privatekey.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/snowflake/user_privatekey.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/spark/thrift.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/trino/base.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/trino/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/trino/certificate.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/trino/certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/trino/jwt.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/trino/jwt.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/cosmos/profiles/trino/ldap.py` & `astronomer_cosmos-1.0.1/cosmos/profiles/trino/ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/.gitignore` & `astronomer_cosmos-1.0.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# cosmos-specific ignores
+# these files get autogenerated
+docs/profiles/*
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 .idea
 # C extensions
@@ -100,15 +104,14 @@
 celerybeat-schedule
 celerybeat.pid
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
-.env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
```

### Comparing `astronomer_cosmos-1.0.0/LICENSE` & `astronomer_cosmos-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.0/README.rst` & `astronomer_cosmos-1.0.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -35,45 +35,52 @@
 
 
 Example Usage
 ___________________
 
 You can render an Airflow Task Group using the ``DbtTaskGroup`` class. Here's an example with the jaffle_shop project:
 
+
 .. code-block:: python
 
     from pendulum import datetime
 
     from airflow import DAG
     from airflow.operators.empty import EmptyOperator
-    from cosmos.providers.dbt.task_group import DbtTaskGroup
+    from cosmos import DbtTaskGroup, ProfileConfig, ProjectConfig
+    from cosmos.profiles import PostgresUserPasswordProfileMapping
 
+    profile_config = ProfileConfig(
+        profile_name="default",
+        target_name="dev",
+        profile_mapping=PostgresUserPasswordProfileMapping(
+            conn_id="airflow_db",
+            profile_args={"schema": "public"},
+        ),
+    )
 
     with DAG(
         dag_id="extract_dag",
         start_date=datetime(2022, 11, 27),
         schedule="@daily",
     ):
         e1 = EmptyOperator(task_id="pre_dbt")
 
         dbt_tg = DbtTaskGroup(
-            dbt_project_name="jaffle_shop",
-            conn_id="airflow_db",
-            profile_args={
-                "schema": "public",
-            },
+            project_config=ProjectConfig("jaffle_shop"),
+            profile_config=profile_config,
         )
 
         e2 = EmptyOperator(task_id="post_dbt")
 
         e1 >> dbt_tg >> e2
 
 This will generate an Airflow Task Group that looks like this:
 
-.. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/jaffle_shop_task_group.png
+.. figure:: /docs/_static/jaffle_shop_task_group.png
 
 Community
 _________
 - Join us on the Airflow `Slack <https://join.slack.com/t/apache-airflow/shared_invite/zt-1zy8e8h85-es~fn19iMzUmkhPwnyRT6Q>`_ at #airflow-dbt
 
 Changelog
 _________
```

### Comparing `astronomer_cosmos-1.0.0/pyproject.toml` & `astronomer_cosmos-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 all = [
     "astronomer-cosmos[dbt-all]",
 ]
 docs =[
     "sphinx",
     "pydata-sphinx-theme",
     "sphinx-autobuild",
-    "sphinx-tabs",
     "sphinx-autoapi"
 ]
 tests = [
     "packaging",
     "pytest>=6.0",
     "pytest-split",
     "pytest-dotenv",
@@ -188,15 +187,14 @@
 ######################################
 
 [tool.hatch.envs.docs]
 dependencies = [
     "sphinx",
     "pydata-sphinx-theme",
     "sphinx-autobuild",
-    "sphinx-tabs",
     "sphinx-autoapi",
 ]
 
 [tool.hatch.envs.docs.scripts]
 build = "sphinx-build -b html docs docs/_build"
 serve = "sphinx-autobuild docs docs/_build"
```

### Comparing `astronomer_cosmos-1.0.0/PKG-INFO` & `astronomer_cosmos-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 1.0.0
+Version: 1.0.1
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
@@ -59,15 +59,14 @@
 Provides-Extra: docker
 Requires-Dist: apache-airflow-providers-docker>=3.5.0; extra == 'docker'
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autoapi; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
-Requires-Dist: sphinx-tabs; extra == 'docs'
 Provides-Extra: kubernetes
 Requires-Dist: apache-airflow-providers-cncf-kubernetes>=5.1.1; extra == 'kubernetes'
 Provides-Extra: tests
 Requires-Dist: mypy; extra == 'tests'
 Requires-Dist: packaging; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Requires-Dist: pytest-describe; extra == 'tests'
@@ -116,45 +115,52 @@
 
 
 Example Usage
 ___________________
 
 You can render an Airflow Task Group using the ``DbtTaskGroup`` class. Here's an example with the jaffle_shop project:
 
+
 .. code-block:: python
 
     from pendulum import datetime
 
     from airflow import DAG
     from airflow.operators.empty import EmptyOperator
-    from cosmos.providers.dbt.task_group import DbtTaskGroup
+    from cosmos import DbtTaskGroup, ProfileConfig, ProjectConfig
+    from cosmos.profiles import PostgresUserPasswordProfileMapping
 
+    profile_config = ProfileConfig(
+        profile_name="default",
+        target_name="dev",
+        profile_mapping=PostgresUserPasswordProfileMapping(
+            conn_id="airflow_db",
+            profile_args={"schema": "public"},
+        ),
+    )
 
     with DAG(
         dag_id="extract_dag",
         start_date=datetime(2022, 11, 27),
         schedule="@daily",
     ):
         e1 = EmptyOperator(task_id="pre_dbt")
 
         dbt_tg = DbtTaskGroup(
-            dbt_project_name="jaffle_shop",
-            conn_id="airflow_db",
-            profile_args={
-                "schema": "public",
-            },
+            project_config=ProjectConfig("jaffle_shop"),
+            profile_config=profile_config,
         )
 
         e2 = EmptyOperator(task_id="post_dbt")
 
         e1 >> dbt_tg >> e2
 
 This will generate an Airflow Task Group that looks like this:
 
-.. image:: https://raw.githubusercontent.com/astronomer/astronomer-cosmos/main/docs/jaffle_shop_task_group.png
+.. figure:: /docs/_static/jaffle_shop_task_group.png
 
 Community
 _________
 - Join us on the Airflow `Slack <https://join.slack.com/t/apache-airflow/shared_invite/zt-1zy8e8h85-es~fn19iMzUmkhPwnyRT6Q>`_ at #airflow-dbt
 
 Changelog
 _________
```

