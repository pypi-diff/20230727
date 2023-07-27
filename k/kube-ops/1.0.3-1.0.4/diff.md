# Comparing `tmp/kube_ops-1.0.3-py3-none-any.whl.zip` & `tmp/kube_ops-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 18992 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1310 b- defN 23-Jul-23 11:51 kube/__init__.py
--rw-r--r--  2.0 unx    32538 b- defN 23-Jul-23 05:31 kube/api.py
+Zip file size: 19825 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1664 b- defN 23-Jul-27 04:35 kube/__init__.py
+-rw-r--r--  2.0 unx    38925 b- defN 23-Jul-27 05:59 kube/api.py
 -rw-r--r--  2.0 unx     2611 b- defN 23-Jul-23 07:44 kube/common.py
--rw-r--r--  2.0 unx     5172 b- defN 23-Jul-26 11:55 kube/config.py
--rw-r--r--  2.0 unx     1197 b- defN 23-Jul-23 06:20 kube/enums.py
--rw-r--r--  2.0 unx    19115 b- defN 23-Jul-23 10:00 kube/manifests.py
--rw-r--r--  2.0 unx    10932 b- defN 23-Jul-23 10:00 kube/templates.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-27 01:27 kube_ops-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3425 b- defN 23-Jul-27 01:27 kube_ops-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 01:27 kube_ops-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-27 01:27 kube_ops-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      894 b- defN 23-Jul-27 01:27 kube_ops-1.0.3.dist-info/RECORD
-12 files, 78360 bytes uncompressed, 17526 bytes compressed:  77.6%
+-rw-r--r--  2.0 unx     5076 b- defN 23-Jul-27 04:49 kube/config.py
+-rw-r--r--  2.0 unx     1400 b- defN 23-Jul-27 02:32 kube/enums.py
+-rw-r--r--  2.0 unx    19771 b- defN 23-Jul-27 05:07 kube/manifests.py
+-rw-r--r--  2.0 unx    11913 b- defN 23-Jul-27 04:49 kube/templates.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-27 05:59 kube_ops-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3425 b- defN 23-Jul-27 05:59 kube_ops-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-27 05:59 kube_ops-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-27 05:59 kube_ops-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      894 b- defN 23-Jul-27 05:59 kube_ops-1.0.4.dist-info/RECORD
+12 files, 86845 bytes uncompressed, 18359 bytes compressed:  78.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kube/manifests.py
 Comment: 
 
 Filename: kube/templates.py
 Comment: 
 
-Filename: kube_ops-1.0.3.dist-info/LICENSE
+Filename: kube_ops-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: kube_ops-1.0.3.dist-info/METADATA
+Filename: kube_ops-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: kube_ops-1.0.3.dist-info/WHEEL
+Filename: kube_ops-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: kube_ops-1.0.3.dist-info/top_level.txt
+Filename: kube_ops-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: kube_ops-1.0.3.dist-info/RECORD
+Filename: kube_ops-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kube/__init__.py

```diff
@@ -1,34 +1,42 @@
 from .api import KubeApi, CustomObjectDef, dict_to_labels
 from .common import env_from_configmap, env_from_configmap_key_ref, env_from_secret, env_from_secret_key_ref, \
     env_from_field_ref, empty_dir, volume_from_configmap, volume_from_secret
 from .config import Kubeconfig
 from .enums import ImagePullPolicy, ServiceType, SecretType, PVCAccessMode, IngressRulePathType, MatchExprOperator, \
-    VolumeModes
-from .manifests import ConfigMap, CronJob, Job, Deployment, Ingress, Namespace, Pod, PersistentVolumeClaim, \
-    StatefulSet, Secret, SecretImagePull, SecretTLS, Service
-from .templates import Container
+    VolumeModes, UpdateStrategy, PodManagementPolicy
+from .manifests import ClusterRole, ClusterRoleBinding, ConfigMap, CronJob, Job, Deployment, Ingress, Namespace, Pod, \
+    PersistentVolumeClaim, Role, RoleBinding, StatefulSet, Secret, SecretImagePull, SecretTLS, Service, \
+    ServiceAccount, SecretServiceAccountToken
+from .templates import Container, LabelSelector
 
 __all__ = [
+    'ClusterRole',
+    'ClusterRoleBinding',
     'ConfigMap',
     'Container',
     'CronJob',
     'CustomObjectDef',
     'Deployment',
     'Ingress',
+    'LabelSelector',
     'Job',
     'KubeApi',
     'Kubeconfig',
     'Namespace',
     'Pod',
     'PersistentVolumeClaim',
+    'Role',
+    'RoleBinding',
     'Secret',
     'SecretImagePull',
     'SecretTLS',
     'Service',
+    'ServiceAccount',
+    'SecretServiceAccountToken',
     'StatefulSet',
     'env_from_configmap',
     'env_from_configmap_key_ref',
     'env_from_secret',
     'env_from_secret_key_ref',
     'env_from_field_ref',
     'empty_dir',
@@ -37,9 +45,11 @@
     'volume_from_secret',
     'ImagePullPolicy',
     'ServiceType',
     'SecretType',
     'PVCAccessMode',
     'IngressRulePathType',
     'MatchExprOperator',
-    'VolumeModes'
+    'VolumeModes',
+    'UpdateStrategy',
+    'PodManagementPolicy'
 ]
```

## kube/api.py

```diff
@@ -11,16 +11,14 @@
 import yaml
 from kubernetes import client, config as kube_config
 from kubernetes.client.rest import ApiException
 from kubernetes.config.incluster_config import SERVICE_HOST_ENV_NAME, \
     SERVICE_PORT_ENV_NAME, SERVICE_CERT_FILENAME
 from kubernetes.stream import stream, ws_client
 
-client.rest.logger.setLevel(logging.WARNING)
-
 
 class CustomObjectDef(typing.NamedTuple):
     """
     Class helper for custom resources definition in Kubernetes
 
     :example: For
               `apiVersion: route.openshift.io/v1
@@ -131,25 +129,29 @@
         else:
             s = 'Unknown'
 
         super().__init__(s)
 
 
 class KubeApi:
-    def __init__(self, namespace: str = None, conf: client.Configuration = None):
+    def __init__(
+            self, namespace: str = None, conf:
+            client.Configuration = None):
+
         self._ns = None
         self._conf = None
 
         if conf:
             client.Configuration().set_default(conf)
             self._conf = conf
         else:
             if self.is_use_in_cluster():
                 kube_config.load_incluster_config()
-                self._ns = Path(SERVICE_CERT_FILENAME).parent.joinpath('namespace').read_text()
+                self._ns = Path(SERVICE_CERT_FILENAME).parent \
+                    .joinpath('namespace').read_text()
             else:
                 kube_config.load_kube_config()
 
         if namespace:
             self._ns = namespace
         else:
             if self._ns is None:
@@ -201,14 +203,18 @@
     def networking_v1(self):
         return client.NetworkingV1Api(self._conf)
 
     @property
     def custom_object_api(self):
         return client.CustomObjectsApi(self._conf)
 
+    @property
+    def rbac_authorization_v1_api(self):
+        return client.RbacAuthorizationV1Api(self._conf)
+
     def _exec(self,
               pod_name: str,
               command: list,
               stdout: Writer,
               stderr: Writer,
               **kwargs) -> tuple[Writer, Writer, dict] | None:
         """
@@ -273,15 +279,16 @@
             stdout, stderr = ResponseDataCollector(), ResponseDataCollector()
         else:
             stdout, stderr = Logger(logging.info), Logger(logging.error)
 
         return self._exec(pod_name, command, stdout, stderr, **kwargs)
 
     def get_logs(self, pod_name: str, container: str = None,
-                 tail_lines: int = None, follow: bool = True, namespace: str = None):
+                 tail_lines: int = None, follow: bool = True,
+                 namespace: str = None):
         """
         Read logs from container.
 
         :param pod_name: Pod name.
         :param container: Print the logs of this container.
         :param tail_lines: Lines of recent log file to display.
         :param follow: Specify if the logs should be streamed.
@@ -320,29 +327,31 @@
         try:
             self._exec(name, cmd, f, Logger(logging.error), **kwargs)
         except Exception:
             raise
         finally:
             f.close()
 
-    def read_configmap(self, name: str, namespace: str = None) -> dict[str, str] | None:
+    def read_configmap(self, name: str,
+                       namespace: str = None) -> dict[str, str] | None:
         """
         Get ConfigMap's data
         :param name: ConfigMap name.
         :param namespace: Specific namespace.
         :return: dict[str, str] or None if secret not found.
         """
 
         cm = self.configmap_get(name, namespace=namespace)
         if not cm:
             return
 
         return cm.data
 
-    def read_secret(self, name: str, namespace: str = None) -> dict[str, str] | None:
+    def read_secret(self, name: str,
+                    namespace: str = None) -> dict[str, str] | None:
         """
         Get Secret's data
         :param name: Secret name.
         :param namespace: Specific namespace.
         :return: dict[str, str] or None if secret not found.
         """
 
@@ -376,42 +385,58 @@
 
         :return: Specific object for wrapped function
                  or None if resource not found.
         """
 
         ns = kwargs.pop('namespace', self._ns)
         try:
-            if custom_object_def is not None:
-                resp = func(
+            if custom_object_def:
+                args = [
                     custom_object_def.group,
                     custom_object_def.version,
-                    ns,
                     custom_object_def.plural,
-                    obj_name,
-                    **kwargs
-                )
+                    obj_name
+                ]
+                if namespaced:
+                    args.insert(2, ns)
             else:
+                args = [obj_name]
                 if namespaced:
-                    resp = func(obj_name, ns, **kwargs)
-                else:
-                    resp = func(obj_name, **kwargs)
+                    args.append(ns)
 
+            resp = func(*args, **kwargs)
             logging.debug('Kubernetes API Response: %s', resp)
 
             return resp
         except ApiException as e:
             if e.status == 404:
                 logging.debug(e)
                 return
 
             if check_err:
                 raise
 
             logging.error(e)
 
+    def _delete(self, func, name: str, **kwargs):
+        kwargs.setdefault('propagation_policy', "Foreground")
+        check_err = kwargs.pop('check_err', False)
+        namespaced = kwargs.pop('namespaced', True)
+        co = kwargs.pop('custom_object_def', None)
+
+        return self._wrapper(func, name, check_err,
+                             namespaced=namespaced,
+                             custom_object_def=co,
+                             **kwargs)
+
+    def _list(self, func, **kwargs):
+        ns = kwargs.pop('namespace', self._ns)
+
+        return func(ns, **kwargs)
+
     def _wrapper_create(self, func, obj, check_err: bool, *,
                         namespaced: bool = True, **kwargs):
         """
         The wrapper function used for the Kubernetes API request handle.
         Used only for create_* functions.
 
         :param func: Function for wrapping.
@@ -434,48 +459,129 @@
                 return
 
             if check_err:
                 raise
 
             logging.error(e)
 
+    def cluster_role_create(self, sec: client.V1ClusterRole, *,
+                            check_err: bool = True,
+                            **kwargs) -> client.V1ClusterRole:
+        """
+        Create ClusterRole.
+        """
+
+        return self._wrapper_create(
+            self.rbac_authorization_v1_api.create_cluster_role,
+            sec, check_err=check_err,
+            namespaced=False, **kwargs)
+
+    def cluster_role_delete(self, name: str,
+                            **kwargs) -> client.V1ClusterRole | None:
+        """
+        Delete ClusterRole by name.
+        """
+
+        return self._delete(self.rbac_authorization_v1_api.delete_cluster_role,
+                            name, namespaced=False, **kwargs)
+
+    def cluster_role_get(self, name: str, *, check_err: bool = True,
+                         **kwargs) -> client.V1ClusterRole | None:
+        """
+        Get ClusterRole.
+        """
+
+        return self._wrapper(self.rbac_authorization_v1_api.read_cluster_role,
+                             name, check_err, namespaced=False, **kwargs)
+
+    def cluster_role_list(self, **kwargs) -> client.V1ClusterRoleList:
+        """
+        List all ClusterRoles.
+        """
+
+        return self.rbac_authorization_v1_api.list_cluster_role(**kwargs)
+
+    def cluster_role_binding_create(self, sec: client.V1ClusterRoleBinding, *,
+                                    check_err: bool = True,
+                                    **kwargs) -> client.V1ClusterRoleBinding:
+        """
+        Create ClusterRoleBinding.
+        """
+
+        return self._wrapper_create(
+            self.rbac_authorization_v1_api.create_cluster_role_binding,
+            sec, check_err=check_err, namespaced=False, **kwargs)
+
+    def cluster_role_binding_delete(self, name: str,
+                                    **kwargs
+                                    ) -> client.V1ClusterRoleBinding | None:
+        """
+        Delete ClusterRoleBinding by name.
+        """
+
+        return self._delete(
+            self.rbac_authorization_v1_api.delete_cluster_role_binding,
+            name, namespaced=False, **kwargs)
+
+    def cluster_role_binding_get(self, name: str, *,
+                                 check_err: bool = True,
+                                 **kwargs
+                                 ) -> client.V1ClusterRoleBinding | None:
+        """
+        Get ClusterRoleBinding.
+        """
+
+        return self._wrapper(
+            self.rbac_authorization_v1_api.read_cluster_role_binding,
+            name, check_err, namespaced=False, **kwargs)
+
+    def cluster_role_binding_list(self,
+                                  **kwargs) -> client.V1ClusterRoleBindingList:
+        """
+        List all ClusterRoleBindings.
+        """
+
+        return self.rbac_authorization_v1_api.list_cluster_role_binding(
+            **kwargs)
+
     def configmap_create(self, sec: client.V1ConfigMap, *,
-                         check_err: bool = True, **kwargs) -> client.V1ConfigMap:
+                         check_err: bool = True,
+                         **kwargs) -> client.V1ConfigMap:
         """
-        Create CongMap in current namespace.
+        Create ConfigMap in current namespace.
         """
 
-        return self._wrapper_create(self.core_v1.create_namespaced_config_map,
-                                    sec, check_err=check_err, **kwargs)
+        return self._wrapper_create(
+            self.core_v1.create_namespaced_config_map,
+            sec, check_err=check_err, **kwargs)
 
-    def configmap_delete(self, name: str, **kwargs) -> client.V1ConfigMap | None:
+    def configmap_delete(self, name: str,
+                         **kwargs) -> client.V1ConfigMap | None:
         """
-        Delete Configmap by name in current namespace.
+        Delete ConfigMap by name in current namespace.
         """
 
-        kwargs.setdefault('propagation_policy', "Foreground")
-        return self._wrapper(self.core_v1.delete_namespaced_config_map,
-                             name, False, **kwargs)
+        return self._delete(self.core_v1.delete_namespaced_config_map,
+                            name, **kwargs)
 
     def configmap_get(self, name: str, *, check_err: bool = True,
                       **kwargs) -> client.V1ConfigMap | None:
         """
-        Get Configmap by name in current namespace.
+        Get ConfigMap by name in current namespace.
         """
 
         return self._wrapper(self.core_v1.read_namespaced_config_map,
                              name, check_err, **kwargs)
 
     def configmap_list(self, **kwargs) -> client.V1ConfigMapList:
         """
-        List all Configmaps in current namespace.
+        List all ConfigMaps in current namespace.
         """
 
-        ns = kwargs.pop('namespace', self._ns)
-        return self.core_v1.list_namespaced_config_map(ns, **kwargs)
+        return self._list(self.core_v1.list_namespaced_config_map, **kwargs)
 
     def cron_job_create(self, cronjob: client.V1CronJob, *,
                         check_err: bool = True, **kwargs) -> client.V1CronJob:
         """
         Create CronJob in current namespace.
         """
 
@@ -483,17 +589,16 @@
                                     cronjob, check_err=check_err, **kwargs)
 
     def cron_job_delete(self, name: str, **kwargs) -> client.V1CronJob | None:
         """
         Delete CronJob by name in current namespace.
         """
 
-        kwargs.setdefault('propagation_policy', "Foreground")
-        return self._wrapper(self.batch_v1.delete_namespaced_cron_job,
-                             name, False, **kwargs)
+        return self._delete(self.batch_v1.delete_namespaced_cron_job,
+                            name, **kwargs)
 
     def cron_job_get(self, name: str, *, check_err: bool = True,
                      **kwargs) -> client.V1CronJob | None:
         """
         Get CronJob by name in current namespace.
         """
 
@@ -501,16 +606,15 @@
                              name, check_err, **kwargs)
 
     def cron_job_list(self, **kwargs) -> client.V1CronJobList:
         """
         List all CronJobs in current namespace.
         """
 
-        ns = kwargs.pop('namespace', self._ns)
-        return self.batch_v1.list_namespaced_cron_job(ns, **kwargs)
+        return self._list(self.batch_v1.list_namespaced_cron_job, **kwargs)
 
     def custom_object_create(self, body, co: CustomObjectDef, *,
                              namespaced: bool = True,
                              check_err: bool = True,
                              **kwargs):
         """
         Create Custom Object API by name in current namespace.
@@ -548,36 +652,33 @@
         Delete Custom Object API by name in current namespace.
         """
 
         func = self.custom_object_api.delete_cluster_custom_object
         if namespaced:
             func = self.custom_object_api.delete_namespaced_custom_object
 
-        kwargs.setdefault('propagation_policy', "Foreground")
-        return self._wrapper(func, name, False,
-                             namespaced=namespaced,
-                             custom_object_def=co,
-                             **kwargs)
+        return self._delete(func, name,
+                            namespaced=namespaced,
+                            custom_object_def=co,
+                            **kwargs)
 
     def custom_object_list(self, co: CustomObjectDef, *,
                            namespaced: bool = True,
                            **kwargs):
         """
         List all Custom Object API in current namespace.
         """
 
         args = [co.group, co.version, co.plural]
+        func = self.custom_object_api.list_cluster_custom_object
         if namespaced:
             args.insert(2, kwargs.pop('namespace', self._ns))
+            func = self.custom_object_api.list_namespaced_custom_object
 
-            return self.custom_object_api.list_namespaced_custom_object(
-                *args, **kwargs)
-        else:
-            return self.custom_object_api.list_cluster_custom_object(
-                *args, **kwargs)
+        return func(*args, **kwargs)
 
     def job_create(self, job: client.V1Job, *, check_err: bool = True,
                    **kwargs) -> client.V1Job:
         """
         Create Job in current namespace.
         """
 
@@ -585,51 +686,50 @@
                                     job, check_err=check_err, **kwargs)
 
     def job_delete(self, name: str, **kwargs) -> client.V1Job | None:
         """
         Delete Job by name in current namespace.
         """
 
-        kwargs.setdefault('propagation_policy', "Foreground")
-        return self._wrapper(self.batch_v1.delete_namespaced_job,
-                             name, False, **kwargs)
+        return self._delete(self.batch_v1.delete_namespaced_job, name,
+                            **kwargs)
 
     def job_get(self, name: str, *, check_err: bool = True,
                 **kwargs) -> client.V1Job | None:
         """
         Get Job by name in current namespace.
         """
         return self._wrapper(self.batch_v1.read_namespaced_job,
                              name, check_err, **kwargs)
 
     def job_list(self, **kwargs) -> client.V1JobList:
         """
         List all Jobs in current namespace.
         """
 
-        ns = kwargs.pop('namespace', self._ns)
-        return self.batch_v1.list_namespaced_job(ns, **kwargs)
+        return self._list(self.batch_v1.list_namespaced_job, **kwargs)
 
-    def deployment_create(self, deploy: client.V1Deployment, *, check_err: bool = True,
+    def deployment_create(self, deploy: client.V1Deployment, *,
+                          check_err: bool = True,
                           **kwargs) -> client.V1Deployment | None:
         """
         Create Deployment in current namespace.
         """
 
         return self._wrapper_create(self.apps_v1.create_namespaced_deployment,
                                     deploy, check_err=check_err, **kwargs)
 
-    def deployment_delete(self, name: str, **kwargs) -> client.V1Deployment | None:
+    def deployment_delete(self, name: str,
+                          **kwargs) -> client.V1Deployment | None:
         """
         Delete Deployment in current namespace
         """
 
-        kwargs.setdefault('propagation_policy', "Foreground")
-        return self._wrapper(self.apps_v1.delete_namespaced_deployment,
-                             name, False, **kwargs)
+        return self._delete(self.apps_v1.delete_namespaced_deployment, name,
+                            **kwargs)
 
     def deployment_get(self, name: str, *, check_err: bool = True,
                        **kwargs) -> client.V1Deployment | None:
         """
         Get Deployment by name in current namespace.
         """
 
@@ -645,16 +745,17 @@
 
     def ingress_create(self, name: str, *, check_err: bool = True,
                        **kwargs) -> client.V1Ingress:
         """
         Get Ingres by name in current namespace.
         """
 
-        return self._wrapper_create(self.networking_v1.create_namespaced_ingress,
-                                    name, check_err, **kwargs)
+        return self._wrapper_create(
+            self.networking_v1.create_namespaced_ingress,
+            name, check_err, **kwargs)
 
     def ingress_delete(self, name: str, *, check_err: bool = True,
                        **kwargs) -> client.V1Ingress | None:
         """
         Get Ingresses by name in current namespace.
         """
 
@@ -666,39 +767,40 @@
         """
         Get Ingresses by name in current namespace.
         """
 
         return self._wrapper(self.networking_v1.read_namespaced_ingress,
                              name, check_err, **kwargs)
 
-    def ingress_list(self, **kwargs) -> client.V1Ingress:
+    def ingress_list(self, **kwargs) -> client.V1IngressList:
         """
         List all Ingresses in current namespace.
         """
 
-        ns = kwargs.pop('namespace', self._ns)
-        return self.networking_v1.list_namespaced_ingress(ns, **kwargs)
+        return self._list(self.networking_v1.list_namespaced_ingress,
+                          **kwargs)
 
     def namespace_create(self, ns: client.V1Namespace, *,
-                         check_err: bool = False, **kwargs) -> client.V1Namespace:
+                         check_err: bool = False,
+                         **kwargs) -> client.V1Namespace:
         """
         Create Namespace.
         """
 
         return self._wrapper_create(self.core_v1.create_namespace,
                                     ns, check_err, namespaced=False, **kwargs)
 
-    def namespace_delete(self, name: str, **kwargs) -> client.V1Namespace | None:
+    def namespace_delete(self, name: str,
+                         **kwargs) -> client.V1Namespace | None:
         """
         Delete Namespace by name.
         """
 
-        kwargs.setdefault('propagation_policy', "Foreground")
-        return self._wrapper(self.core_v1.delete_namespace,
-                             name, False, namespaced=False, **kwargs)
+        return self._delete(self.core_v1.delete_namespace,
+                            name, namespaced=False, **kwargs)
 
     def namespace_get(self, name: str, **kwargs) -> client.V1Namespace | None:
         """
         Get Namespace by name.
         """
 
         return self._wrapper(self.core_v1.read_namespace,
@@ -721,17 +823,15 @@
                                     pod, check_err=check_err, **kwargs)
 
     def pod_delete(self, name: str, **kwargs) -> client.V1Pod | None:
         """
         Delete Pod by name in current namespace.
         """
 
-        kwargs.setdefault('propagation_policy', "Foreground")
-        return self._wrapper(self.core_v1.delete_namespaced_pod,
-                             name, False, **kwargs)
+        return self._delete(self.core_v1.delete_namespaced_pod, name, **kwargs)
 
     def pod_get(self, name: str, *, check_err: bool = True,
                 **kwargs) -> client.V1Pod | None:
         """
         Get Pod by name in current namespace.
         """
 
@@ -739,52 +839,129 @@
                              name, check_err, **kwargs)
 
     def pod_list(self, **kwargs) -> client.V1PodList:
         """
         List all Pods in current namespace.
         """
 
-        ns = kwargs.pop('namespace', self._ns)
-        return self.core_v1.list_namespaced_pod(ns, **kwargs)
+        return self._list(self.core_v1.list_namespaced_pod, **kwargs)
 
     def pvc_create(self, pvc: client.V1PersistentVolumeClaim, *,
-                   check_err: bool = True, **kwargs) -> client.V1PersistentVolumeClaim:
+                   check_err: bool = True,
+                   **kwargs) -> client.V1PersistentVolumeClaim:
         """
         Create PersistentVolumeClaim in current namespace.
         """
 
         return self._wrapper_create(
             self.core_v1.create_namespaced_persistent_volume_claim,
             pvc, check_err=check_err, **kwargs)
 
-    def pvc_delete(self, name: str, **kwargs) -> client.V1PersistentVolumeClaim | None:
+    def pvc_delete(self, name: str,
+                   **kwargs) -> client.V1PersistentVolumeClaim | None:
         """
         Delete PersistentVolumeClaim by name in current namespace.
         """
 
-        kwargs.setdefault('propagation_policy', "Foreground")
-        return self._wrapper(self.core_v1.delete_namespaced_persistent_volume_claim,
-                             name, False, **kwargs)
+        return self._delete(
+            self.core_v1.delete_namespaced_persistent_volume_claim,
+            name, **kwargs)
 
     def pvc_get(self, name: str, *, check_err: bool = True,
                 **kwargs) -> client.V1PersistentVolumeClaim | None:
         """
         Get PersistentVolumeClaim by name in current namespace.
         """
 
-        return self._wrapper(self.core_v1.read_namespaced_persistent_volume_claim,
-                             name, check_err, **kwargs)
+        return self._wrapper(
+            self.core_v1.read_namespaced_persistent_volume_claim,
+            name, check_err, **kwargs)
 
     def pvc_list(self, **kwargs) -> client.V1PersistentVolumeClaimList:
         """
         List all PersistentVolumeClaims in current namespace.
         """
 
-        ns = kwargs.pop('namespace', self._ns)
-        return self.core_v1.list_namespaced_persistent_volume_claim(ns, **kwargs)
+        return self._list(self.core_v1.list_namespaced_persistent_volume_claim,
+                          **kwargs)
+
+    def role_create(self, sec: client.V1Role, *,
+                    check_err: bool = True, **kwargs) -> client.V1Role:
+        """
+        Create RoleBinding.
+        """
+
+        return self._wrapper_create(
+            self.rbac_authorization_v1_api.create_namespaced_role,
+            sec, check_err=check_err, namespaced=False, **kwargs)
+
+    def role_delete(self, name: str, **kwargs) -> client.V1Role | None:
+        """
+        Delete Role by name.
+        """
+
+        return self._delete(
+            self.rbac_authorization_v1_api.delete_namespaced_role,
+            name, **kwargs)
+
+    def role_get(self, name: str, *, check_err: bool = True,
+                 **kwargs) -> client.V1Role | None:
+        """
+        Get RoleBinding.
+        """
+
+        return self._wrapper(
+            self.rbac_authorization_v1_api.read_namespaced_role,
+            name, check_err, **kwargs)
+
+    def role_list(self, **kwargs) -> client.V1RoleList:
+        """
+        List all RoleBindings.
+        """
+
+        return self._list(self.rbac_authorization_v1_api.list_namespaced_role,
+                          **kwargs)
+
+    def role_binding_create(self, sec: client.V1RoleBinding, *,
+                            check_err: bool = True, **kwargs) -> client.V1RoleBinding:
+        """
+        Create RoleBinding.
+        """
+
+        return self._wrapper_create(
+            self.rbac_authorization_v1_api.create_namespaced_role_binding,
+            sec, check_err=check_err, namespaced=False, **kwargs)
+
+    def role_binding_delete(self, name: str, **kwargs) -> client.V1RoleBinding | None:
+        """
+        Delete RoleBinding by name.
+        """
+
+        return self._delete(
+            self.rbac_authorization_v1_api.delete_namespaced_role_binding,
+            name, **kwargs)
+
+    def role_binding_get(self, name: str, *, check_err: bool = True,
+                         **kwargs) -> client.V1RoleBinding | None:
+        """
+        Get RoleBinding.
+        """
+
+        return self._wrapper(
+            self.rbac_authorization_v1_api.read_namespaced_role_binding,
+            name, check_err, **kwargs)
+
+    def role_binding_list(self, **kwargs) -> client.V1RoleBindingList:
+        """
+        List all RoleBindings.
+        """
+
+        return self._list(
+            self.rbac_authorization_v1_api.list_namespaced_role_binding,
+            **kwargs)
 
     def secret_get(self, name: str, *, check_err: bool = True,
                    **kwargs) -> client.V1Secret | None:
         """
         Get Secret by name in current namespace.
         """
 
@@ -801,25 +978,23 @@
                                     sec, check_err=check_err, **kwargs)
 
     def secret_delete(self, name: str, **kwargs) -> client.V1Secret | None:
         """
         Delete Secret by name in current namespace.
         """
 
-        kwargs.setdefault('propagation_policy', "Foreground")
-        return self._wrapper(self.core_v1.delete_namespaced_secret,
-                             name, False, **kwargs)
+        return self._delete(self.core_v1.delete_namespaced_secret,
+                            name, **kwargs)
 
     def secret_list(self, **kwargs) -> client.V1SecretList:
         """
         List all Secrets in current namespace.
         """
 
-        ns = kwargs.pop('namespace', self._ns)
-        return self.core_v1.list_namespaced_secret(ns, **kwargs)
+        return self._list(self.core_v1.list_namespaced_secret, **kwargs)
 
     def service_get(self, name: str, *, check_err: bool = True,
                     **kwargs) -> client.V1Secret | None:
         """
         Get Service by name in current namespace.
         """
 
@@ -836,43 +1011,80 @@
                                     svc, check_err=check_err, **kwargs)
 
     def service_delete(self, name: str, **kwargs) -> client.V1Service | None:
         """
         Delete Service by name in current namespace.
         """
 
-        kwargs.setdefault('propagation_policy', "Foreground")
-        return self._wrapper(self.core_v1.delete_namespaced_service,
-                             name, False, **kwargs)
+        return self._delete(self.core_v1.delete_namespaced_service,
+                            name, **kwargs)
 
-    def service_list(self, **kwargs) -> client.V1Service:
+    def service_list(self, **kwargs) -> client.V1ServiceList:
         """
         List all Service in current namespace.
         """
 
-        ns = kwargs.pop('namespace', self._ns)
-        return self.core_v1.list_namespaced_service(ns, **kwargs)
+        return self._list(self.core_v1.list_namespaced_service, **kwargs)
+
+    def service_account_get(self, name: str, *, check_err: bool = True,
+                            **kwargs) -> client.V1Secret | None:
+        """
+        Get ServiceAccount by name in current namespace.
+        """
+
+        return self._wrapper(self.core_v1.read_namespaced_service_account,
+                             name, check_err, **kwargs)
 
-    def stateful_set_create(self, sts: client.V1StatefulSet, *, check_err: bool = True,
+    def service_account_create(self, svc: client.V1ServiceAccount, *,
+                               check_err: bool = True,
+                               **kwargs) -> client.V1ServiceAccount:
+        """
+        Create ServiceAccount in current namespace.
+        """
+
+        return self._wrapper_create(
+            self.core_v1.create_namespaced_service_account,
+            svc, check_err=check_err, **kwargs)
+
+    def service_account_delete(self, name: str,
+                               **kwargs) -> client.V1ServiceAccount | None:
+        """
+        Delete ServiceAccount by name in current namespace.
+        """
+
+        return self._delete(self.core_v1.delete_namespaced_service_account,
+                            name, **kwargs)
+
+    def service_account_list(self, **kwargs) -> client.V1ServiceAccountList:
+        """
+        List all ServiceAccount in current namespace.
+        """
+
+        return self._list(self.core_v1.list_namespaced_service_account,
+                          **kwargs)
+
+    def stateful_set_create(self, sts: client.V1StatefulSet, *,
+                            check_err: bool = True,
                             **kwargs) -> client.V1StatefulSet | None:
         """
         Create StatefulSet in current namespace.
         """
 
-        return self._wrapper_create(self.apps_v1.create_namespaced_stateful_set,
-                                    sts, check_err=check_err, **kwargs)
+        return self._wrapper_create(
+            self.apps_v1.create_namespaced_stateful_set,
+            sts, check_err=check_err, **kwargs)
 
-    def stateful_set_delete(self, name: str, **kwargs) -> client.V1StatefulSet | None:
+    def stateful_set_delete(self, name: str,
+                            **kwargs) -> client.V1StatefulSet | None:
         """
         Delete StatefulSet by name in current namespace.
         """
 
-        kwargs.setdefault('propagation_policy', "Foreground")
-        return self._wrapper(self.apps_v1.delete_namespaced_stateful_set,
-                             name, False, **kwargs)
+        return self._delete(self.apps_v1.delete_namespaced_stateful_set,
+                            name, **kwargs)
 
     def stateful_set_get(self, name: str, *, check_err: bool = True,
                          **kwargs) -> client.V1StatefulSet | None:
         """
         Get StatefulSet by name in current namespace.
         """
 
@@ -880,16 +1092,16 @@
                              name, check_err, **kwargs)
 
     def stateful_set_list(self, **kwargs) -> client.V1StatefulSetList:
         """
         List all StatefulSets in current namespace.
         """
 
-        ns = kwargs.pop('namespace', self._ns)
-        return self.apps_v1.list_namespaced_stateful_set(ns, **kwargs)
+        return self._list(self.apps_v1.list_namespaced_stateful_set,
+                          **kwargs)
 
     def scale_deployment(self, name: str, replicas: int, wait: bool = False,
                          **kwargs) -> client.V1Deployment:
         """
         Scale Deployment by name in current namespace.
 
         :param name: Deployment name.
```

## kube/config.py

```diff
@@ -1,20 +1,19 @@
 from __future__ import annotations
 
 import base64
 import hashlib
 import os
-import warnings
 from pathlib import Path
 from urllib.parse import urlparse
 
 import yaml
 from kubernetes import client
 from kubernetes.config.incluster_config import SERVICE_HOST_ENV_NAME, SERVICE_PORT_ENV_NAME, SERVICE_CERT_FILENAME
-from urllib3.exceptions import InsecureRequestWarning, MaxRetryError
+from urllib3.exceptions import MaxRetryError
 
 from .api import KubeApi
 
 
 class Kubeconfig:
     def __init__(self):
         self.__current_context = None
@@ -94,15 +93,14 @@
 
         if not insecure_skip_tls_verify and not ca_cert:
             raise ValueError('Add CA data or set `skip_tls_verify=True`')
 
         cluster = {"server": server}
         if insecure_skip_tls_verify:
             cluster['insecure-skip-tls-verify'] = insecure_skip_tls_verify
-            warnings.simplefilter(action="ignore", category=InsecureRequestWarning)
 
         if ca_cert:
             if ca_cert.startswith('-----BEGIN CERTIFICATE-----'):
                 ca_cert = base64.b64encode(ca_cert).decode()
             cluster['certificate-authority-data'] = ca_cert
 
         self.__clusters.setdefault(cluster_name, cluster)
@@ -122,18 +120,21 @@
             filepath = Path.home().joinpath('.kube/config')
         elif isinstance(filepath, str):
             filepath = Path(filepath)
 
         filepath.parent.mkdir(0o755, True, True)
 
         with open(filepath, 'w') as f:
-            yaml.safe_dump({
-                "apiVersion": "v1",
-                "kind": "Config",
-                "current-context": self.__current_context,
-                "preferences": {},
-                "clusters": [{"name": k, "cluster": v} for k, v in self.__clusters.items()],
-                "contexts": [{"name": k, "context": v} for k, v in self.__contexts.items()],
-                "users": [{"name": k, "user": v} for k, v in self.__users.items()]
-            }, f)
+            self.dump(f)
 
         os.chmod(filepath, 0o600)
+
+    def dump(self, stream=None):
+        yaml.safe_dump({
+            "apiVersion": "v1",
+            "kind": "Config",
+            "current-context": self.__current_context,
+            "preferences": {},
+            "clusters": [{"name": k, "cluster": v} for k, v in self.__clusters.items()],
+            "contexts": [{"name": k, "context": v} for k, v in self.__contexts.items()],
+            "users": [{"name": k, "user": v} for k, v in self.__users.items()]
+        }, stream)
```

## kube/enums.py

```diff
@@ -44,7 +44,17 @@
     Exists = 'Exists'
     DoesNotExist = 'DoesNotExist'
 
 
 class VolumeModes(enum.StrEnum):
     Filesystem = 'Filesystem'
     Block = 'Block'
+
+
+class UpdateStrategy(enum.StrEnum):
+    RollingUpdate = 'RollingUpdate'
+    Recreate = 'Recreate'
+
+
+class PodManagementPolicy(enum.StrEnum):
+    OrderedReady = 'OrderedReady'
+    Parallel = 'Parallel'
```

## kube/manifests.py

```diff
@@ -1,15 +1,16 @@
-import base64
 import json
 from copy import deepcopy
 
 from kubernetes import client
 
-from .enums import SecretType, ServiceType, IngressRulePathType, PVCAccessMode, MatchExprOperator, VolumeModes
-from .templates import PodSpec, PodTemplateSpec, JobTemplateSpec, Container, V1Primitive, ObjectMetadata, dict_str
+from .enums import SecretType, ServiceType, IngressRulePathType, PVCAccessMode, VolumeModes, UpdateStrategy, \
+    PodManagementPolicy
+from .templates import PodSpec, PodTemplateSpec, JobTemplateSpec, Container, V1Primitive, ObjectMetadata, \
+    LabelSelector, dict_str
 
 
 class Job(PodTemplateSpec, ObjectMetadata):
     def __init__(self, name: str, c: Container):
         super().__init__(c)
         ObjectMetadata.__init__(self, name)
 
@@ -113,33 +114,30 @@
     def set_annotations(self, **kwargs):
         self._pod.metadata.annotations = dict_str(**kwargs)
 
     def set_labels(self, **kwargs):
         self._pod.metadata.labels = dict_str(**kwargs)
 
 
-class Deployment(PodTemplateSpec, ObjectMetadata):
+class Deployment(PodTemplateSpec, ObjectMetadata, LabelSelector):
     def __init__(self, name: str, c: Container):
         super().__init__(c)
         ObjectMetadata.__init__(self, name)
 
         self._deploy = client.V1Deployment(
             spec=client.V1DeploymentSpec(
-                selector=client.V1LabelSelector(),
                 template=client.V1PodTemplateSpec()
             )
         )
 
     @property
     def manifest(self) -> client.V1Deployment:
         o = deepcopy(self._deploy)
-        if o.spec.selector.match_expressions is None and o.spec.selector.match_labels is None:
-            o.spec.selector = None
-
         o.metadata = self._metadata
+        o.spec.selector = self._selector
         o.spec.template = super().manifest
         return o
 
     @property
     def selector_match_labels(self) -> dict[str, str]:
         return self._deploy.spec.selector.match_labels.copy()
 
@@ -157,69 +155,39 @@
 
     def set_replicas(self, n: int):
         self._deploy.spec.replicas = n
 
     def set_revision_history_limit(self, n: int):
         self._deploy.spec.revision_history_limit = n
 
-    def set_selector_match_labels(self, **kwargs):
-        self._deploy.spec.selector.match_labels = dict_str(**kwargs)
-
-    def add_selector_match_expressions(self, key: str, operator: str, values: list[str]):
-        allow = ['In', 'NotIn', 'Exists', 'DoesNotExist']
-        if operator not in allow:
-            raise ValueError(f'Invalid operator value `{operator}`. Can be one of `{", ".join(allow)}`')
-
-        if self._deploy.spec.selector.match_expressions:
-            for e in self._deploy.spec.selector.match_expressions:
-                if e.key == key and e.operator == operator:
-                    return
-        else:
-            self._deploy.spec.selector.match_expression = []
-
-        self._deploy.spec.selector.match_expression.append(
-            client.V1LabelSelectorRequirement(key=key, operator=operator, values=values)
-        )
-
-    def set_strategy(self, typ: str, max_surge=None, max_unavailable=None):
-        allow = ['RollingUpdate', 'Recreate']
-        if typ not in allow:
-            raise ValueError(f'Invalid strategy type value `{typ}`. Can be one of `{", ".join(allow)}`')
-
+    def set_strategy(self, typ: UpdateStrategy, max_surge=None, max_unavailable=None):
         self._deploy.spec.strategy = client.V1DeploymentStrategy(
-            type=typ,
+            type=typ.value,
             rolling_update=client.V1RollingUpdateDeployment(max_surge=max_surge, max_unavailable=max_unavailable))
 
 
-class StatefulSet(PodTemplateSpec, ObjectMetadata):
+class StatefulSet(PodTemplateSpec, ObjectMetadata, LabelSelector):
     def __init__(self, name: str, c: Container):
         super().__init__(c)
         ObjectMetadata.__init__(self, name)
 
         self._sts = client.V1StatefulSet(
             api_version='v1',
             kind='StatefulSet',
             spec=client.V1StatefulSetSpec(
                 service_name='',
-                selector=client.V1LabelSelector(),
                 template=client.V1PodTemplateSpec()
             )
         )
 
     @property
     def manifest(self) -> client.V1StatefulSet:
         o = deepcopy(self._sts)
-
-        if not o.spec.service_name:
-            raise ValueError('Invalid value for `service_name`, must not be empty')
-
-        if o.spec.selector.match_expressions is None and o.spec.selector.match_labels is None:
-            raise ValueError('Invalid value for `selector`, must not be empty')
-
         o.metadata = self._metadata
+        o.spec.selector = self._selector
         o.spec.template = super().manifest
         return o
 
     def set_annotations(self, **kwargs):
         self._sts.metadata.annotations = dict_str(**kwargs)
 
     def set_labels(self, **kwargs):
@@ -233,53 +201,30 @@
 
     def set_replicas(self, n: int):
         self._sts.spec.replicas = n
 
     def set_revision_history_limit(self, n: int):
         self._sts.spec.revision_history_limit = n
 
-    def set_selector_match_labels(self, **kwargs):
-        self._sts.spec.selector.match_labels = dict_str(**kwargs)
-
-    def add_selector_match_expressions(self, key: str, operator: str, values: list[str]):
-        allow = ['In', 'NotIn', 'Exists', 'DoesNotExist']
-        if operator not in allow:
-            raise ValueError(f'Invalid operator value `{operator}`. Can be one of `{", ".join(allow)}`')
-
-        if self._sts.spec.selector.match_expressions:
-            for e in self._sts.spec.selector.match_expressions:
-                if e.key == key and e.operator == operator:
-                    return
-        else:
-            self._sts.spec.selector.match_expression = []
-
-        self._sts.spec.selector.match_expression.append(
-            client.V1LabelSelectorRequirement(key=key, operator=operator, values=values)
-        )
-
     def set_strategy(self, typ: str, max_unavailable=None, partition: int = None):
 
         self._sts.spec.update_strategy = client.V1StatefulSetUpdateStrategy(
             type=typ,
             rolling_update=client.V1RollingUpdateStatefulSetStrategy(
                 max_unavailable=max_unavailable, partition=partition))
 
     def set_service_name(self, name: str):
         self._sts.spec.service_name = name
 
     def set_persistent_volume_claim_retention_policy(self, when_deleted: str, when_scaled: str):
         o = client.V1StatefulSetPersistentVolumeClaimRetentionPolicy(when_deleted=when_deleted, when_scaled=when_scaled)
         self._sts.spec.persistent_volume_claim_retention_policy = o
 
-    def set_pod_management_policy(self, policy: str):
-        allow = ['OrderedReady', 'Parallel']
-        if policy not in allow:
-            raise ValueError(f'Invalid podManagementPolicy value `{policy}`. Can be one of `{", ".join(allow)}`')
-
-        self._sts.spec.pod_management_policy = policy
+    def set_pod_management_policy(self, policy: PodManagementPolicy):
+        self._sts.spec.pod_management_policy = policy.value
 
     def add_volume_claim_templates(self, pvc: client.V1PersistentVolumeClaim):
         if self._sts.spec.volume_claim_templates:
             for p in self._sts.spec.volume_claim_templates:
                 if p.metadata.name == pvc.metadata.name:
                     return
         else:
@@ -292,20 +237,17 @@
     def __init__(self, name: str, typ: SecretType):
         super().__init__(name)
         V1Primitive.__init__(self)
 
         self._secret = client.V1Secret(
             api_version="v1",
             kind="Secret",
-            type=typ.value,
+            type=typ.value
         )
 
-    def to_base64(self, v: str) -> str:
-        return base64.b64encode(v.encode()).decode()
-
     @property
     def manifest(self):
         sec = deepcopy(self._secret)
         sec.metadata = self._metadata
         sec.immutable = self._immutable
         if self._string_data:
             sec.string_data = self._string_data
@@ -331,31 +273,43 @@
             "email": email,
             "auth": self.to_base64(f"{username}:{password}")
         }
 
     @property
     def manifest(self):
         auth = json.dumps({"auths": self._registries})
-        self.set(".dockerconfigjson", self.to_base64(auth))
+        self.set(".dockerconfigjson", auth)
 
         return super().manifest
 
 
 class SecretTLS(Secret):
     def __init__(self, name: str):
         super().__init__(name, SecretType.TLS)
 
-    def set(self, tls_cert: str, tls_key: str, ca: str = None):
-        if ca:
-            super().set('ca.crt', ca)
+    def set(self, tls_cert: str, tls_key: str, ca_crt: str = None):
+        if ca_crt:
+            super().set('ca.crt', ca_crt)
 
         super().set('tls.crt', tls_cert)
         super().set('tls.key', tls_key)
 
 
+class SecretServiceAccountToken(Secret):
+    def __init__(self, name: str):
+        super().__init__(name, SecretType.ServiceAccountToken)
+
+    def set(self, namespace: str, token: str, ca_crt: str = None):
+        if ca_crt:
+            super().set('ca.crt', ca_crt)
+
+        super().set('namespace', namespace)
+        super().set('token', token)
+
+
 class ConfigMap(ObjectMetadata, V1Primitive):
     def __init__(self, name: str):
         super().__init__(name)
         V1Primitive.__init__(self)
 
         self._cm = client.V1ConfigMap(
             api_version="v1",
@@ -470,20 +424,14 @@
         else:
             self._ing.spec.tls = []
 
         self._ing.spec.tls.append(client.V1IngressTLS(hosts=hosts, secret_name=secret_name))
 
     def _ingress_backend(self, service_name: str = None, service_port: int | str = None,
                          ref: client.V1TypedLocalObjectReference = None) -> client.V1IngressBackend:
-        if not service_name and not ref:
-            raise ValueError('Required service_name and port or object reference')
-
-        if service_name and not service_port:
-            raise ValueError(f'Required both arguments service_name and port')
-
         backend = client.V1IngressBackend()
         if ref:
             backend.resource = ref
             return backend
 
         if isinstance(service_port, int):
             port_def = client.V1ServiceBackendPort(number=service_port)
@@ -507,15 +455,15 @@
     @property
     def manifest(self) -> client.V1Namespace:
         ns = deepcopy(self._ns)
         ns.metadata = self._metadata
         return ns
 
 
-class PersistentVolumeClaim(ObjectMetadata):
+class PersistentVolumeClaim(ObjectMetadata, LabelSelector):
     def __init__(self, name: str):
         super().__init__(name)
 
         self._pvc = client.V1PersistentVolumeClaim(
             api_version='v1',
             kind='PersistentVolumeClaim',
             spec=client.V1PersistentVolumeClaimSpec(
@@ -524,14 +472,15 @@
             )
         )
 
     @property
     def manifest(self) -> client.V1PersistentVolumeClaim:
         pvc = deepcopy(self._pvc)
         pvc.metadata = self._metadata
+        pvc.spec.selector = self._selector
         return pvc
 
     def set_access_modes(self, *args: PVCAccessMode):
         self._pvc.spec.access_modes = [a.value for a in args]
 
     def set_data_source(self, name: str, api_group: str, kind: str):
         self._pvc.spec.data_source = client.V1TypedLocalObjectReference(
@@ -539,44 +488,149 @@
         )
 
     def set_data_source_ref(self, name: str, namespace: str, api_group: str, kind: str):
         self._pvc.spec.data_source_ref = client.V1TypedObjectReference(
             api_group, kind, name, namespace
         )
 
-    def _check_selector(self):
-        if self._pvc.spec.selector is None:
-            self._pvc.spec.selector = client.V1LabelSelector()
-
-    def add_selector_match_expressions(self, key: str, operator: MatchExprOperator, *values: str):
-        self._check_selector()
-
-        if not self._pvc.spec.selector.match_expressions:
-            self._pvc.spec.selector.match_expressions = []
-
-        select = client.V1LabelSelectorRequirement(
-            key=key,
-            operator=operator.value
-        )
-        if values:
-            select.values = list(values)
-
-        self._pvc.spec.selector.match_expressions.append(select)
-
-    def set_match_labels(self, **kwargs: [str, str]):
-        self._check_selector()
-        self._pvc.spec.selector.match_labels = dict_str(**kwargs)
-
     def set_storage_class_name(self, name: str):
         self._pvc.spec.storage_class_name = name
 
     def set_volume_mode(self, mode: VolumeModes):
         self._pvc.spec.volume_mode = mode.value
 
     def set_volume_name(self, name: str):
         self._pvc.spec.volume_name = name
 
     def set_resources_requests(self, size: str):
         self._pvc.spec.resources.requests = {'storage': size}
 
     def set_resources_limits(self, size: str):
         self._pvc.spec.resources.limits = {'storage': size}
+
+
+class ServiceAccount(ObjectMetadata):
+    def __init__(self, name):
+        super().__init__(name)
+
+        self._sa = client.V1ServiceAccount(
+            api_version='v1',
+            kind='ServiceAccount'
+        )
+
+    @property
+    def manifest(self) -> client.V1ServiceAccount:
+        sa = deepcopy(self._sa)
+        sa.metadata = self._metadata
+        return sa
+
+    def set_automount_service_account_token(self, b: bool):
+        self._sa.automount_service_account_token = b
+
+    def add_image_pull_secrets(self, name: str):
+        self._sa.image_pull_secrets.append(
+            client.V1LocalObjectReference(name=name))
+
+    def add_secret(self, ref: client.V1ObjectReference):
+        self._sa.secrets.append(ref)
+
+    def add_secret_name(self, name: str):
+        self._sa.secrets.append(
+            client.V1ObjectReference(name=name))
+
+
+class Role(ObjectMetadata):
+    def __init__(self, name: str):
+        super().__init__(name)
+
+        self._role = client.V1Role(
+            api_version='rbac.authorization.k8s.io/v1',
+            kind='Role',
+            rules=[]
+        )
+
+    @property
+    def manifest(self) -> client.V1Role:
+        role = deepcopy(self._role)
+        role.metadata = self._metadata
+        return role
+
+    def add_rule(self, rule: client.V1PolicyRule):
+        self._role.rules.append(rule)
+
+
+class RoleBinding(ObjectMetadata):
+    def __init__(self, name: str):
+        super().__init__(name)
+
+        self._rb = client.V1RoleBinding(
+            api_version='rbac.authorization.k8s.io/v1',
+            kind='RoleBinding',
+            subjects=[]
+        )
+
+    @property
+    def manifest(self) -> client.V1RoleBinding:
+        rb = deepcopy(self._rb)
+        rb.metadata = self._metadata
+        return rb
+
+    def add_role_ref(self, api_group: str, kind: str, name: str):
+        self._rb.role_ref = client.V1RoleRef(
+            api_group=api_group, kind=kind, name=name)
+
+    def add_subject(self, kind: str, name: str, namespace: str, api_group: str = None):
+        self._rb.subjects.append(client.V1Subject(
+            api_group=api_group, kind=kind, name=name, namespace=namespace))
+
+
+class ClusterRole(ObjectMetadata):
+    def __init__(self, name: str):
+        super().__init__(name)
+
+        self._role = client.V1ClusterRole(
+            api_version='rbac.authorization.k8s.io/v1',
+            kind='ClusterRole',
+            rules=[]
+        )
+
+    @property
+    def manifest(self) -> client.V1ClusterRole:
+        role = deepcopy(self._role)
+        role.metadata = self._metadata
+        return role
+
+    def add_rule(self, rule: client.V1PolicyRule):
+        self._role.rules.append(rule)
+
+    def add_aggregation_rule(self, rule: client.V1LabelSelector):
+        if not self._role.aggregation_rule:
+            self._role.aggregation_rule = client.V1AggregationRule(
+                cluster_role_selectors=[]
+            )
+
+        self._role.aggregation_rule.cluster_role_selectors.append(rule)
+
+
+class ClusterRoleBinding(ObjectMetadata):
+    def __init__(self, name: str):
+        super().__init__(name)
+
+        self._crb = client.V1ClusterRoleBinding(
+            api_version='rbac.authorization.k8s.io/v1',
+            kind='ClusterRoleBinding',
+            subjects=[]
+        )
+
+    @property
+    def manifest(self) -> client.V1ClusterRoleBinding:
+        crb = deepcopy(self._crb)
+        crb.metadata = self._metadata
+        return crb
+
+    def add_role_ref(self, api_group: str, kind: str, name: str):
+        self._crb.role_ref = client.V1RoleRef(
+            api_group=api_group, kind=kind, name=name)
+
+    def add_subject(self, kind: str, name: str, namespace: str, api_group: str = None):
+        self._crb.subjects.append(client.V1Subject(
+            api_group=api_group, kind=kind, name=name, namespace=namespace))
```

## kube/templates.py

```diff
@@ -1,12 +1,13 @@
+import base64
 from copy import deepcopy
 
 from kubernetes import client
 
-from .enums import ImagePullPolicy
+from .enums import ImagePullPolicy, MatchExprOperator
 
 
 def dict_str(**kwargs):
     if not kwargs:
         return
 
     return dict(map(lambda kv: (kv[0], str(kv[1])), kwargs.items()))
@@ -47,33 +48,36 @@
         self._string_data = {}
         self._binary_data = {}
         self._immutable = None
 
     def set_immutable(self, b: bool):
         self._immutable = b
 
-    def set(self, k: str, v):
-        self._string_data[k] = v
+    def set(self, k: str, v: str):
+        self._binary_data[k] = self.to_base64(v)
 
     def set_default(self, k: str, v):
-        return self._string_data.setdefault(k, v)
+        return self._string_data.setdefault(k, self.to_base64(v))
 
-    # TODO: will be encoded twice if set to base64 encoded value
     def set_data(self, **kwargs):
-        self._string_data = dict_str(**kwargs)
+        self._string_data = dict_str(
+            **{k: self.to_base64(v) for k, v in kwargs.items()})
 
     def set_string(self, k: str, v: str):
         self._string_data[k] = v
 
     def set_default_string(self, k: str, v: str) -> str:
         return self._string_data.setdefault(k, v)
 
     def set_string_data(self, **kwargs):
         self._string_data = dict_str(**kwargs)
 
+    def to_base64(self, v: str) -> str:
+        return base64.b64encode(v.encode()).decode()
+
 
 class Container:
     def __init__(self, name: str):
         self._c = client.V1Container(name=name)
 
     @property
     def name(self):
@@ -343,7 +347,31 @@
     def __init__(self, c: Container):
         super().__init__(c, client.V1PodTemplateSpec())
 
 
 class JobTemplateSpec(_TemplateSpec):
     def __init__(self, c: Container):
         super().__init__(c, client.V1JobTemplateSpec())
+
+
+class LabelSelector:
+    def __init__(self):
+        self._selector = client.V1LabelSelector()
+
+    @property
+    def manifest(self) -> client.V1LabelSelector:
+        return deepcopy(self._selector)
+
+    def set_selector_match_labels(self, **kwargs):
+        self._selector.match_labels = dict_str(**kwargs)
+
+    def add_selector_match_expressions(self, key: str, operator: MatchExprOperator, values: list[str]):
+        if self._selector.match_expressions:
+            for e in self._selector.match_expressions:
+                if e.key == key and e.operator == operator.value:
+                    return
+        else:
+            self._selector.match_expression = []
+
+        self._selector.match_expression.append(
+            client.V1LabelSelectorRequirement(key=key, operator=operator.value, values=values)
+        )
```

## Comparing `kube_ops-1.0.3.dist-info/LICENSE` & `kube_ops-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kube_ops-1.0.3.dist-info/METADATA` & `kube_ops-1.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kube-ops
-Version: 1.0.3
+Version: 1.0.4
 Summary: Kubernetes OOP
 Author-email: myback <54638513+myback@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 myback.space
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

