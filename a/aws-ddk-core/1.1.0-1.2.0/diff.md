# Comparing `tmp/aws-ddk-core-1.1.0.tar.gz` & `tmp/aws-ddk-core-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ddk-core-1.1.0.tar", last modified: Wed Jul  5 17:36:01 2023, max compression
+gzip compressed data, was "aws-ddk-core-1.2.0.tar", last modified: Thu Jul 27 15:40:58 2023, max compression
```

## Comparing `aws-ddk-core-1.1.0.tar` & `aws-ddk-core-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-05 17:36:01.329074 aws-ddk-core-1.1.0/
--rw-r--r--   0 hansonlu (569507325) 1896053708    11358 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/LICENSE
--rw-r--r--   0 hansonlu (569507325) 1896053708       23 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/MANIFEST.in
--rw-r--r--   0 hansonlu (569507325) 1896053708       67 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/NOTICE
--rw-r--r--   0 hansonlu (569507325) 1896053708     6364 2023-07-05 17:36:01.328621 aws-ddk-core-1.1.0/PKG-INFO
--rw-r--r--   0 hansonlu (569507325) 1896053708     5387 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/README.md
--rw-r--r--   0 hansonlu (569507325) 1896053708      234 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/pyproject.toml
--rw-r--r--   0 hansonlu (569507325) 1896053708       38 2023-07-05 17:36:01.329215 aws-ddk-core-1.1.0/setup.cfg
--rw-r--r--   0 hansonlu (569507325) 1896053708     2039 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/setup.py
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-05 17:36:01.289561 aws-ddk-core-1.1.0/src/
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-05 17:36:01.315267 aws-ddk-core-1.1.0/src/aws_ddk_core/
--rw-r--r--   0 hansonlu (569507325) 1896053708   646858 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/src/aws_ddk_core/__init__.py
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-05 17:36:01.318823 aws-ddk-core-1.1.0/src/aws_ddk_core/_jsii/
--rw-r--r--   0 hansonlu (569507325) 1896053708      573 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/src/aws_ddk_core/_jsii/__init__.py
--rw-r--r--   0 hansonlu (569507325) 1896053708  5062250 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/src/aws_ddk_core/_jsii/aws-ddk-core@1.1.0.jsii.tgz
--rw-r--r--   0 hansonlu (569507325) 1896053708        1 2023-07-05 17:35:42.000000 aws-ddk-core-1.1.0/src/aws_ddk_core/py.typed
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-05 17:36:01.317655 aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/
--rw-r--r--   0 hansonlu (569507325) 1896053708     6364 2023-07-05 17:36:01.000000 aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/PKG-INFO
--rw-r--r--   0 hansonlu (569507325) 1896053708      400 2023-07-05 17:36:01.000000 aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/SOURCES.txt
--rw-r--r--   0 hansonlu (569507325) 1896053708        1 2023-07-05 17:36:01.000000 aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/dependency_links.txt
--rw-r--r--   0 hansonlu (569507325) 1896053708      313 2023-07-05 17:36:01.000000 aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/requires.txt
--rw-r--r--   0 hansonlu (569507325) 1896053708       13 2023-07-05 17:36:01.000000 aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/top_level.txt
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-27 15:40:58.297214 aws-ddk-core-1.2.0/
+-rw-r--r--   0 hansonlu (569507325) 1896053708    11358 2023-07-27 15:40:42.000000 aws-ddk-core-1.2.0/LICENSE
+-rw-r--r--   0 hansonlu (569507325) 1896053708       23 2023-07-27 15:40:42.000000 aws-ddk-core-1.2.0/MANIFEST.in
+-rw-r--r--   0 hansonlu (569507325) 1896053708       67 2023-07-27 15:40:42.000000 aws-ddk-core-1.2.0/NOTICE
+-rw-r--r--   0 hansonlu (569507325) 1896053708     6485 2023-07-27 15:40:58.296903 aws-ddk-core-1.2.0/PKG-INFO
+-rw-r--r--   0 hansonlu (569507325) 1896053708     5387 2023-07-27 15:40:42.000000 aws-ddk-core-1.2.0/README.md
+-rw-r--r--   0 hansonlu (569507325) 1896053708      234 2023-07-27 15:40:42.000000 aws-ddk-core-1.2.0/pyproject.toml
+-rw-r--r--   0 hansonlu (569507325) 1896053708       38 2023-07-27 15:40:58.297307 aws-ddk-core-1.2.0/setup.cfg
+-rw-r--r--   0 hansonlu (569507325) 1896053708     2160 2023-07-27 15:40:42.000000 aws-ddk-core-1.2.0/setup.py
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-27 15:40:58.281875 aws-ddk-core-1.2.0/src/
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-27 15:40:58.286104 aws-ddk-core-1.2.0/src/aws_ddk_core/
+-rw-r--r--   0 hansonlu (569507325) 1896053708   702039 2023-07-27 15:40:42.000000 aws-ddk-core-1.2.0/src/aws_ddk_core/__init__.py
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-27 15:40:58.289189 aws-ddk-core-1.2.0/src/aws_ddk_core/_jsii/
+-rw-r--r--   0 hansonlu (569507325) 1896053708      573 2023-07-27 15:40:42.000000 aws-ddk-core-1.2.0/src/aws_ddk_core/_jsii/__init__.py
+-rw-r--r--   0 hansonlu (569507325) 1896053708  5077929 2023-07-27 15:40:42.000000 aws-ddk-core-1.2.0/src/aws_ddk_core/_jsii/aws-ddk-core@1.2.0.jsii.tgz
+-rw-r--r--   0 hansonlu (569507325) 1896053708        1 2023-07-27 15:40:42.000000 aws-ddk-core-1.2.0/src/aws_ddk_core/py.typed
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-07-27 15:40:58.288328 aws-ddk-core-1.2.0/src/aws_ddk_core.egg-info/
+-rw-r--r--   0 hansonlu (569507325) 1896053708     6485 2023-07-27 15:40:58.000000 aws-ddk-core-1.2.0/src/aws_ddk_core.egg-info/PKG-INFO
+-rw-r--r--   0 hansonlu (569507325) 1896053708      400 2023-07-27 15:40:58.000000 aws-ddk-core-1.2.0/src/aws_ddk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 hansonlu (569507325) 1896053708        1 2023-07-27 15:40:58.000000 aws-ddk-core-1.2.0/src/aws_ddk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 hansonlu (569507325) 1896053708      313 2023-07-27 15:40:58.000000 aws-ddk-core-1.2.0/src/aws_ddk_core.egg-info/requires.txt
+-rw-r--r--   0 hansonlu (569507325) 1896053708       13 2023-07-27 15:40:58.000000 aws-ddk-core-1.2.0/src/aws_ddk_core.egg-info/top_level.txt
```

### Comparing `aws-ddk-core-1.1.0/LICENSE` & `aws-ddk-core-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ddk-core-1.1.0/PKG-INFO` & `aws-ddk-core-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aws-ddk-core
-Version: 1.1.0
-Summary: AWS DataOps Development Kit
+Version: 1.2.0
+Summary: The AWS DataOps Development Kit is an open source development framework for customers that build data workflows and modern data architecture on AWS.
 Home-page: https://github.com/awslabs/aws-ddk/tree/main
 Author: AWS Professional Services<aws-proserve-orion-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-ddk/tree/main
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
```

### Comparing `aws-ddk-core-1.1.0/README.md` & `aws-ddk-core-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-ddk-core-1.1.0/setup.py` & `aws-ddk-core-1.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-ddk-core",
-    "version": "1.1.0",
-    "description": "AWS DataOps Development Kit",
+    "version": "1.2.0",
+    "description": "The AWS DataOps Development Kit is an open source development framework for customers that build data workflows and modern data architecture on AWS.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-ddk/tree/main",
     "long_description_content_type": "text/markdown",
     "author": "AWS Professional Services<aws-proserve-orion-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
     },
@@ -22,29 +22,29 @@
     },
     "packages": [
         "aws_ddk_core",
         "aws_ddk_core._jsii"
     ],
     "package_data": {
         "aws_ddk_core._jsii": [
-            "aws-ddk-core@1.1.0.jsii.tgz"
+            "aws-ddk-core@1.2.0.jsii.tgz"
         ],
         "aws_ddk_core": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.85.0, <3.0.0",
         "aws-cdk.aws-glue-alpha>=2.85.0.a0, <3.0.0",
         "aws-cdk.aws-kinesisfirehose-alpha>=2.85.0.a0, <3.0.0",
         "aws-cdk.aws-kinesisfirehose-destinations-alpha>=2.85.0.a0, <3.0.0",
         "aws-cdk.integ-tests-alpha>=2.85.0.a0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.84.0, <2.0.0",
+        "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `aws-ddk-core-1.1.0/src/aws_ddk_core/__init__.py` & `aws-ddk-core-1.2.0/src/aws_ddk_core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 import aws_cdk.aws_appflow as _aws_cdk_aws_appflow_ceddda9d
 import aws_cdk.aws_cloudwatch as _aws_cdk_aws_cloudwatch_ceddda9d
 import aws_cdk.aws_codeguruprofiler as _aws_cdk_aws_codeguruprofiler_ceddda9d
 import aws_cdk.aws_codepipeline as _aws_cdk_aws_codepipeline_ceddda9d
 import aws_cdk.aws_codestarnotifications as _aws_cdk_aws_codestarnotifications_ceddda9d
 import aws_cdk.aws_databrew as _aws_cdk_aws_databrew_ceddda9d
 import aws_cdk.aws_ec2 as _aws_cdk_aws_ec2_ceddda9d
+import aws_cdk.aws_emrserverless as _aws_cdk_aws_emrserverless_ceddda9d
 import aws_cdk.aws_events as _aws_cdk_aws_events_ceddda9d
 import aws_cdk.aws_glue as _aws_cdk_aws_glue_ceddda9d
 import aws_cdk.aws_glue_alpha as _aws_cdk_aws_glue_alpha_ce674d29
 import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
 import aws_cdk.aws_kinesis as _aws_cdk_aws_kinesis_ceddda9d
 import aws_cdk.aws_kinesisfirehose_alpha as _aws_cdk_aws_kinesisfirehose_alpha_30daaf29
 import aws_cdk.aws_kinesisfirehose_destinations_alpha as _aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc
@@ -3207,14 +3208,451 @@
 
     def __repr__(self) -> str:
         return "DeliveryStreamProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class EMRServerlessCluster(
+    _constructs_77d1e7e8.Construct,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="aws-ddk-core.EMRServerlessCluster",
+):
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        additional_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+        s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+        security_group: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SecurityGroup] = None,
+        vpc_cidr: typing.Optional[builtins.str] = None,
+        vpc_id: typing.Optional[builtins.str] = None,
+        release_label: builtins.str,
+        type: builtins.str,
+        architecture: typing.Optional[builtins.str] = None,
+        auto_start_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.AutoStartConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        auto_stop_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.AutoStopConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        image_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.ImageConfigurationInputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        initial_capacity: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Sequence[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.InitialCapacityConfigKeyValuePairProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+        maximum_capacity: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.MaximumAllowedResourcesProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        name: typing.Optional[builtins.str] = None,
+        network_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.NetworkConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_ceddda9d.CfnTag, typing.Dict[builtins.str, typing.Any]]]] = None,
+        worker_type_specifications: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Mapping[builtins.str, typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.WorkerTypeSpecificationInputProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+    ) -> None:
+        '''
+        :param scope: -
+        :param id: -
+        :param additional_policy_statements: Additional policy statements to add to the emr role.
+        :param s3_bucket: S3 Bucket.
+        :param security_group: Security Group.
+        :param vpc_cidr: The IP range (CIDR notation) for this VPC.
+        :param vpc_id: Existing vpc id.
+        :param release_label: The EMR release version associated with the application. *Minimum* : 1 *Maximum* : 64 *Pattern* : ``^[A-Za-z0-9._/-]+$``
+        :param type: The type of application, such as Spark or Hive.
+        :param architecture: The CPU architecture type of the application. Allowed values: ``X86_64`` or ``ARM64``
+        :param auto_start_configuration: The configuration for an application to automatically start on job submission.
+        :param auto_stop_configuration: The configuration for an application to automatically stop after a certain amount of time being idle.
+        :param image_configuration: ``AWS::EMRServerless::Application.ImageConfiguration``.
+        :param initial_capacity: The initial capacity of the application.
+        :param maximum_capacity: The maximum capacity of the application. This is cumulative across all workers at any given point in time during the lifespan of the application is created. No new resources will be created once any one of the defined limits is hit.
+        :param name: The name of the application. *Minimum* : 1 *Maximum* : 64 *Pattern* : ``^[A-Za-z0-9._\\\\/#-]+$``
+        :param network_configuration: The network configuration for customer VPC connectivity for the application.
+        :param tags: The tags assigned to the application.
+        :param worker_type_specifications: ``AWS::EMRServerless::Application.WorkerTypeSpecifications``.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__83d66a5f4ea6335b061a6877ac3664b7458c10cb62db78fcee7fdf475a19fee5)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = EMRServerlessClusterProps(
+            additional_policy_statements=additional_policy_statements,
+            s3_bucket=s3_bucket,
+            security_group=security_group,
+            vpc_cidr=vpc_cidr,
+            vpc_id=vpc_id,
+            release_label=release_label,
+            type=type,
+            architecture=architecture,
+            auto_start_configuration=auto_start_configuration,
+            auto_stop_configuration=auto_stop_configuration,
+            image_configuration=image_configuration,
+            initial_capacity=initial_capacity,
+            maximum_capacity=maximum_capacity,
+            name=name,
+            network_configuration=network_configuration,
+            tags=tags,
+            worker_type_specifications=worker_type_specifications,
+        )
+
+        jsii.create(self.__class__, self, [scope, id, props])
+
+    @jsii.member(jsii_name="createVpc")
+    def create_vpc(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        resource_name: builtins.str,
+        vpc_cidr: builtins.str,
+    ) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
+        '''
+        :param scope: -
+        :param resource_name: -
+        :param vpc_cidr: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__864be4d07f911163bb991815f5a8c0561cfd97d707e687ef07552b1d38bb82d2)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument resource_name", value=resource_name, expected_type=type_hints["resource_name"])
+            check_type(argname="argument vpc_cidr", value=vpc_cidr, expected_type=type_hints["vpc_cidr"])
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, jsii.invoke(self, "createVpc", [scope, resource_name, vpc_cidr]))
+
+    @builtins.property
+    @jsii.member(jsii_name="emrServerlessApplication")
+    def emr_serverless_application(
+        self,
+    ) -> _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication:
+        return typing.cast(_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication, jsii.get(self, "emrServerlessApplication"))
+
+    @builtins.property
+    @jsii.member(jsii_name="networkConfiguration")
+    def network_configuration(
+        self,
+    ) -> _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.NetworkConfigurationProperty:
+        return typing.cast(_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.NetworkConfigurationProperty, jsii.get(self, "networkConfiguration"))
+
+    @builtins.property
+    @jsii.member(jsii_name="role")
+    def role(self) -> _aws_cdk_aws_iam_ceddda9d.Role:
+        return typing.cast(_aws_cdk_aws_iam_ceddda9d.Role, jsii.get(self, "role"))
+
+    @builtins.property
+    @jsii.member(jsii_name="s3Bucket")
+    def s3_bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
+        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, jsii.get(self, "s3Bucket"))
+
+    @builtins.property
+    @jsii.member(jsii_name="securityGroup")
+    def security_group(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SecurityGroup]:
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SecurityGroup], jsii.get(self, "securityGroup"))
+
+    @builtins.property
+    @jsii.member(jsii_name="vpc")
+    def vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], jsii.get(self, "vpc"))
+
+
+@jsii.data_type(
+    jsii_type="aws-ddk-core.EMRServerlessClusterProps",
+    jsii_struct_bases=[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplicationProps],
+    name_mapping={
+        "release_label": "releaseLabel",
+        "type": "type",
+        "architecture": "architecture",
+        "auto_start_configuration": "autoStartConfiguration",
+        "auto_stop_configuration": "autoStopConfiguration",
+        "image_configuration": "imageConfiguration",
+        "initial_capacity": "initialCapacity",
+        "maximum_capacity": "maximumCapacity",
+        "name": "name",
+        "network_configuration": "networkConfiguration",
+        "tags": "tags",
+        "worker_type_specifications": "workerTypeSpecifications",
+        "additional_policy_statements": "additionalPolicyStatements",
+        "s3_bucket": "s3Bucket",
+        "security_group": "securityGroup",
+        "vpc_cidr": "vpcCidr",
+        "vpc_id": "vpcId",
+    },
+)
+class EMRServerlessClusterProps(
+    _aws_cdk_aws_emrserverless_ceddda9d.CfnApplicationProps,
+):
+    def __init__(
+        self,
+        *,
+        release_label: builtins.str,
+        type: builtins.str,
+        architecture: typing.Optional[builtins.str] = None,
+        auto_start_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.AutoStartConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        auto_stop_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.AutoStopConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        image_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.ImageConfigurationInputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        initial_capacity: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Sequence[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.InitialCapacityConfigKeyValuePairProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+        maximum_capacity: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.MaximumAllowedResourcesProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        name: typing.Optional[builtins.str] = None,
+        network_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.NetworkConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_ceddda9d.CfnTag, typing.Dict[builtins.str, typing.Any]]]] = None,
+        worker_type_specifications: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Mapping[builtins.str, typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.WorkerTypeSpecificationInputProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+        additional_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+        s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+        security_group: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SecurityGroup] = None,
+        vpc_cidr: typing.Optional[builtins.str] = None,
+        vpc_id: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param release_label: The EMR release version associated with the application. *Minimum* : 1 *Maximum* : 64 *Pattern* : ``^[A-Za-z0-9._/-]+$``
+        :param type: The type of application, such as Spark or Hive.
+        :param architecture: The CPU architecture type of the application. Allowed values: ``X86_64`` or ``ARM64``
+        :param auto_start_configuration: The configuration for an application to automatically start on job submission.
+        :param auto_stop_configuration: The configuration for an application to automatically stop after a certain amount of time being idle.
+        :param image_configuration: ``AWS::EMRServerless::Application.ImageConfiguration``.
+        :param initial_capacity: The initial capacity of the application.
+        :param maximum_capacity: The maximum capacity of the application. This is cumulative across all workers at any given point in time during the lifespan of the application is created. No new resources will be created once any one of the defined limits is hit.
+        :param name: The name of the application. *Minimum* : 1 *Maximum* : 64 *Pattern* : ``^[A-Za-z0-9._\\\\/#-]+$``
+        :param network_configuration: The network configuration for customer VPC connectivity for the application.
+        :param tags: The tags assigned to the application.
+        :param worker_type_specifications: ``AWS::EMRServerless::Application.WorkerTypeSpecifications``.
+        :param additional_policy_statements: Additional policy statements to add to the emr role.
+        :param s3_bucket: S3 Bucket.
+        :param security_group: Security Group.
+        :param vpc_cidr: The IP range (CIDR notation) for this VPC.
+        :param vpc_id: Existing vpc id.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__dff46b98beafa0af6fc125923b2225092c53114f275e10e2732de3f4d3cd2573)
+            check_type(argname="argument release_label", value=release_label, expected_type=type_hints["release_label"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument architecture", value=architecture, expected_type=type_hints["architecture"])
+            check_type(argname="argument auto_start_configuration", value=auto_start_configuration, expected_type=type_hints["auto_start_configuration"])
+            check_type(argname="argument auto_stop_configuration", value=auto_stop_configuration, expected_type=type_hints["auto_stop_configuration"])
+            check_type(argname="argument image_configuration", value=image_configuration, expected_type=type_hints["image_configuration"])
+            check_type(argname="argument initial_capacity", value=initial_capacity, expected_type=type_hints["initial_capacity"])
+            check_type(argname="argument maximum_capacity", value=maximum_capacity, expected_type=type_hints["maximum_capacity"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument network_configuration", value=network_configuration, expected_type=type_hints["network_configuration"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument worker_type_specifications", value=worker_type_specifications, expected_type=type_hints["worker_type_specifications"])
+            check_type(argname="argument additional_policy_statements", value=additional_policy_statements, expected_type=type_hints["additional_policy_statements"])
+            check_type(argname="argument s3_bucket", value=s3_bucket, expected_type=type_hints["s3_bucket"])
+            check_type(argname="argument security_group", value=security_group, expected_type=type_hints["security_group"])
+            check_type(argname="argument vpc_cidr", value=vpc_cidr, expected_type=type_hints["vpc_cidr"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "release_label": release_label,
+            "type": type,
+        }
+        if architecture is not None:
+            self._values["architecture"] = architecture
+        if auto_start_configuration is not None:
+            self._values["auto_start_configuration"] = auto_start_configuration
+        if auto_stop_configuration is not None:
+            self._values["auto_stop_configuration"] = auto_stop_configuration
+        if image_configuration is not None:
+            self._values["image_configuration"] = image_configuration
+        if initial_capacity is not None:
+            self._values["initial_capacity"] = initial_capacity
+        if maximum_capacity is not None:
+            self._values["maximum_capacity"] = maximum_capacity
+        if name is not None:
+            self._values["name"] = name
+        if network_configuration is not None:
+            self._values["network_configuration"] = network_configuration
+        if tags is not None:
+            self._values["tags"] = tags
+        if worker_type_specifications is not None:
+            self._values["worker_type_specifications"] = worker_type_specifications
+        if additional_policy_statements is not None:
+            self._values["additional_policy_statements"] = additional_policy_statements
+        if s3_bucket is not None:
+            self._values["s3_bucket"] = s3_bucket
+        if security_group is not None:
+            self._values["security_group"] = security_group
+        if vpc_cidr is not None:
+            self._values["vpc_cidr"] = vpc_cidr
+        if vpc_id is not None:
+            self._values["vpc_id"] = vpc_id
+
+    @builtins.property
+    def release_label(self) -> builtins.str:
+        '''The EMR release version associated with the application.
+
+        *Minimum* : 1
+
+        *Maximum* : 64
+
+        *Pattern* : ``^[A-Za-z0-9._/-]+$``
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-emrserverless-application.html#cfn-emrserverless-application-releaselabel
+        '''
+        result = self._values.get("release_label")
+        assert result is not None, "Required property 'release_label' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def type(self) -> builtins.str:
+        '''The type of application, such as Spark or Hive.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-emrserverless-application.html#cfn-emrserverless-application-type
+        '''
+        result = self._values.get("type")
+        assert result is not None, "Required property 'type' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def architecture(self) -> typing.Optional[builtins.str]:
+        '''The CPU architecture type of the application.
+
+        Allowed values: ``X86_64`` or ``ARM64``
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-emrserverless-application.html#cfn-emrserverless-application-architecture
+        '''
+        result = self._values.get("architecture")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def auto_start_configuration(
+        self,
+    ) -> typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.AutoStartConfigurationProperty]]:
+        '''The configuration for an application to automatically start on job submission.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-emrserverless-application.html#cfn-emrserverless-application-autostartconfiguration
+        '''
+        result = self._values.get("auto_start_configuration")
+        return typing.cast(typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.AutoStartConfigurationProperty]], result)
+
+    @builtins.property
+    def auto_stop_configuration(
+        self,
+    ) -> typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.AutoStopConfigurationProperty]]:
+        '''The configuration for an application to automatically stop after a certain amount of time being idle.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-emrserverless-application.html#cfn-emrserverless-application-autostopconfiguration
+        '''
+        result = self._values.get("auto_stop_configuration")
+        return typing.cast(typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.AutoStopConfigurationProperty]], result)
+
+    @builtins.property
+    def image_configuration(
+        self,
+    ) -> typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.ImageConfigurationInputProperty]]:
+        '''``AWS::EMRServerless::Application.ImageConfiguration``.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-emrserverless-application.html#cfn-emrserverless-application-imageconfiguration
+        '''
+        result = self._values.get("image_configuration")
+        return typing.cast(typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.ImageConfigurationInputProperty]], result)
+
+    @builtins.property
+    def initial_capacity(
+        self,
+    ) -> typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.List[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.InitialCapacityConfigKeyValuePairProperty]]]]:
+        '''The initial capacity of the application.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-emrserverless-application.html#cfn-emrserverless-application-initialcapacity
+        '''
+        result = self._values.get("initial_capacity")
+        return typing.cast(typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.List[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.InitialCapacityConfigKeyValuePairProperty]]]], result)
+
+    @builtins.property
+    def maximum_capacity(
+        self,
+    ) -> typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.MaximumAllowedResourcesProperty]]:
+        '''The maximum capacity of the application.
+
+        This is cumulative across all workers at any given point in time during the lifespan of the application is created. No new resources will be created once any one of the defined limits is hit.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-emrserverless-application.html#cfn-emrserverless-application-maximumcapacity
+        '''
+        result = self._values.get("maximum_capacity")
+        return typing.cast(typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.MaximumAllowedResourcesProperty]], result)
+
+    @builtins.property
+    def name(self) -> typing.Optional[builtins.str]:
+        '''The name of the application.
+
+        *Minimum* : 1
+
+        *Maximum* : 64
+
+        *Pattern* : ``^[A-Za-z0-9._\\\\/#-]+$``
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-emrserverless-application.html#cfn-emrserverless-application-name
+        '''
+        result = self._values.get("name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def network_configuration(
+        self,
+    ) -> typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.NetworkConfigurationProperty]]:
+        '''The network configuration for customer VPC connectivity for the application.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-emrserverless-application.html#cfn-emrserverless-application-networkconfiguration
+        '''
+        result = self._values.get("network_configuration")
+        return typing.cast(typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.NetworkConfigurationProperty]], result)
+
+    @builtins.property
+    def tags(self) -> typing.Optional[typing.List[_aws_cdk_ceddda9d.CfnTag]]:
+        '''The tags assigned to the application.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-emrserverless-application.html#cfn-emrserverless-application-tags
+        '''
+        result = self._values.get("tags")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_ceddda9d.CfnTag]], result)
+
+    @builtins.property
+    def worker_type_specifications(
+        self,
+    ) -> typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Mapping[builtins.str, typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.WorkerTypeSpecificationInputProperty]]]]:
+        '''``AWS::EMRServerless::Application.WorkerTypeSpecifications``.
+
+        :link: http://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-emrserverless-application.html#cfn-emrserverless-application-workertypespecifications
+        '''
+        result = self._values.get("worker_type_specifications")
+        return typing.cast(typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Mapping[builtins.str, typing.Union[_aws_cdk_ceddda9d.IResolvable, _aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.WorkerTypeSpecificationInputProperty]]]], result)
+
+    @builtins.property
+    def additional_policy_statements(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
+        '''Additional policy statements to add to the emr role.'''
+        result = self._values.get("additional_policy_statements")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
+
+    @builtins.property
+    def s3_bucket(self) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket]:
+        '''S3 Bucket.'''
+        result = self._values.get("s3_bucket")
+        return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket], result)
+
+    @builtins.property
+    def security_group(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SecurityGroup]:
+        '''Security Group.'''
+        result = self._values.get("security_group")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SecurityGroup], result)
+
+    @builtins.property
+    def vpc_cidr(self) -> typing.Optional[builtins.str]:
+        '''The IP range (CIDR notation) for this VPC.'''
+        result = self._values.get("vpc_cidr")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def vpc_id(self) -> typing.Optional[builtins.str]:
+        '''Existing vpc id.'''
+        result = self._values.get("vpc_id")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "EMRServerlessClusterProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 @jsii.data_type(
     jsii_type="aws-ddk-core.EnvironmentConfiguration",
     jsii_struct_bases=[],
     name_mapping={
         "account": "account",
         "bootstrap": "bootstrap",
         "props": "props",
@@ -7368,14 +7806,262 @@
 
     def __repr__(self) -> str:
         return "DataStageProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+@jsii.data_type(
+    jsii_type="aws-ddk-core.EMRServerlessJobStageProps",
+    jsii_struct_bases=[StateMachineStageProps],
+    name_mapping={
+        "description": "description",
+        "name": "name",
+        "additional_role_policy_statements": "additionalRolePolicyStatements",
+        "alarms_enabled": "alarmsEnabled",
+        "definition": "definition",
+        "definition_file": "definitionFile",
+        "state_machine_failed_executions_alarm_evaluation_periods": "stateMachineFailedExecutionsAlarmEvaluationPeriods",
+        "state_machine_failed_executions_alarm_threshold": "stateMachineFailedExecutionsAlarmThreshold",
+        "state_machine_input": "stateMachineInput",
+        "state_machine_name": "stateMachineName",
+        "application_id": "applicationId",
+        "execution_role_arn": "executionRoleArn",
+        "job_driver": "jobDriver",
+        "job_execution_status_check_period": "jobExecutionStatusCheckPeriod",
+        "start_job_run_props": "startJobRunProps",
+    },
+)
+class EMRServerlessJobStageProps(StateMachineStageProps):
+    def __init__(
+        self,
+        *,
+        description: typing.Optional[builtins.str] = None,
+        name: typing.Optional[builtins.str] = None,
+        additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+        alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
+        state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
+        state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
+        state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+        state_machine_name: typing.Optional[builtins.str] = None,
+        application_id: builtins.str,
+        execution_role_arn: builtins.str,
+        job_driver: typing.Mapping[builtins.str, typing.Any],
+        job_execution_status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        start_job_run_props: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+    ) -> None:
+        '''Properties of the EMR Serverless Job stage.
+
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param application_id: EMR Serverless Application Id.
+        :param execution_role_arn: EMR Execution Role Arn.
+        :param job_driver: The job driver for the job run. This is a Tagged Union structure. Only one of the following top level keys can be set: 'sparkSubmit', 'hive'
+        :param job_execution_status_check_period: Duration to wait between polling job status. Defaults to 30 seconds.
+        :param start_job_run_props: Additional properties to pass to 'emrserverless:StartJobRun'. https://docs.aws.amazon.com/emr-serverless/latest/APIReference/API_StartJobRun.html
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a74bc867d821b2a380e6cc61db61d700e291094dae87fe77909819ed40f25b02)
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument additional_role_policy_statements", value=additional_role_policy_statements, expected_type=type_hints["additional_role_policy_statements"])
+            check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
+            check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
+            check_type(argname="argument definition_file", value=definition_file, expected_type=type_hints["definition_file"])
+            check_type(argname="argument state_machine_failed_executions_alarm_evaluation_periods", value=state_machine_failed_executions_alarm_evaluation_periods, expected_type=type_hints["state_machine_failed_executions_alarm_evaluation_periods"])
+            check_type(argname="argument state_machine_failed_executions_alarm_threshold", value=state_machine_failed_executions_alarm_threshold, expected_type=type_hints["state_machine_failed_executions_alarm_threshold"])
+            check_type(argname="argument state_machine_input", value=state_machine_input, expected_type=type_hints["state_machine_input"])
+            check_type(argname="argument state_machine_name", value=state_machine_name, expected_type=type_hints["state_machine_name"])
+            check_type(argname="argument application_id", value=application_id, expected_type=type_hints["application_id"])
+            check_type(argname="argument execution_role_arn", value=execution_role_arn, expected_type=type_hints["execution_role_arn"])
+            check_type(argname="argument job_driver", value=job_driver, expected_type=type_hints["job_driver"])
+            check_type(argname="argument job_execution_status_check_period", value=job_execution_status_check_period, expected_type=type_hints["job_execution_status_check_period"])
+            check_type(argname="argument start_job_run_props", value=start_job_run_props, expected_type=type_hints["start_job_run_props"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "application_id": application_id,
+            "execution_role_arn": execution_role_arn,
+            "job_driver": job_driver,
+        }
+        if description is not None:
+            self._values["description"] = description
+        if name is not None:
+            self._values["name"] = name
+        if additional_role_policy_statements is not None:
+            self._values["additional_role_policy_statements"] = additional_role_policy_statements
+        if alarms_enabled is not None:
+            self._values["alarms_enabled"] = alarms_enabled
+        if definition is not None:
+            self._values["definition"] = definition
+        if definition_file is not None:
+            self._values["definition_file"] = definition_file
+        if state_machine_failed_executions_alarm_evaluation_periods is not None:
+            self._values["state_machine_failed_executions_alarm_evaluation_periods"] = state_machine_failed_executions_alarm_evaluation_periods
+        if state_machine_failed_executions_alarm_threshold is not None:
+            self._values["state_machine_failed_executions_alarm_threshold"] = state_machine_failed_executions_alarm_threshold
+        if state_machine_input is not None:
+            self._values["state_machine_input"] = state_machine_input
+        if state_machine_name is not None:
+            self._values["state_machine_name"] = state_machine_name
+        if job_execution_status_check_period is not None:
+            self._values["job_execution_status_check_period"] = job_execution_status_check_period
+        if start_job_run_props is not None:
+            self._values["start_job_run_props"] = start_job_run_props
+
+    @builtins.property
+    def description(self) -> typing.Optional[builtins.str]:
+        '''Description of the stage.'''
+        result = self._values.get("description")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def name(self) -> typing.Optional[builtins.str]:
+        '''Name of the stage.'''
+        result = self._values.get("name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def additional_role_policy_statements(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
+        '''Additional IAM policy statements to add to the state machine role.'''
+        result = self._values.get("additional_role_policy_statements")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
+
+    @builtins.property
+    def alarms_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enable/Disable all alarms in the stage.
+
+        :default: true
+        '''
+        result = self._values.get("alarms_enabled")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def definition(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]]:
+        '''Steps for the state machine.
+
+        Can either be provided as 'sfn.IChainable' or a JSON string.
+        '''
+        result = self._values.get("definition")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]], result)
+
+    @builtins.property
+    def definition_file(self) -> typing.Optional[builtins.str]:
+        '''File containing a JSON definition for the state machine.'''
+        result = self._values.get("definition_file")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def state_machine_failed_executions_alarm_evaluation_periods(
+        self,
+    ) -> typing.Optional[jsii.Number]:
+        '''The number of periods over which data is compared to the specified threshold.
+
+        :default: 1
+        '''
+        result = self._values.get("state_machine_failed_executions_alarm_evaluation_periods")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def state_machine_failed_executions_alarm_threshold(
+        self,
+    ) -> typing.Optional[jsii.Number]:
+        '''The number of failed state machine executions before triggering CW alarm.
+
+        :default: 1
+        '''
+        result = self._values.get("state_machine_failed_executions_alarm_threshold")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def state_machine_input(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''Input of the state machine.'''
+        result = self._values.get("state_machine_input")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
+
+    @builtins.property
+    def state_machine_name(self) -> typing.Optional[builtins.str]:
+        '''Name of the state machine.'''
+        result = self._values.get("state_machine_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def application_id(self) -> builtins.str:
+        '''EMR Serverless Application Id.'''
+        result = self._values.get("application_id")
+        assert result is not None, "Required property 'application_id' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def execution_role_arn(self) -> builtins.str:
+        '''EMR Execution Role Arn.'''
+        result = self._values.get("execution_role_arn")
+        assert result is not None, "Required property 'execution_role_arn' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def job_driver(self) -> typing.Mapping[builtins.str, typing.Any]:
+        '''The job driver for the job run.
+
+        This is a Tagged Union structure.
+        Only one of the following top level
+        keys can be set: 'sparkSubmit', 'hive'
+        '''
+        result = self._values.get("job_driver")
+        assert result is not None, "Required property 'job_driver' is missing"
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], result)
+
+    @builtins.property
+    def job_execution_status_check_period(
+        self,
+    ) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+        '''Duration to wait between polling job status.
+
+        Defaults to 30 seconds.
+        '''
+        result = self._values.get("job_execution_status_check_period")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+
+    @builtins.property
+    def start_job_run_props(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        '''Additional properties to pass to 'emrserverless:StartJobRun'.
+
+        https://docs.aws.amazon.com/emr-serverless/latest/APIReference/API_StartJobRun.html
+        '''
+        result = self._values.get("start_job_run_props")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "EMRServerlessJobStageProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class EventStage(
     Stage,
     metaclass=jsii.JSIIAbstractClass,
     jsii_type="aws-ddk-core.EventStage",
 ):
     '''Class that represents an event stage within a data pipeline.
 
@@ -9652,14 +10338,116 @@
         '''Input targets for the stage.
 
         Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
         '''
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
 
 
+class EMRServerlessJobStage(
+    StateMachineStage,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="aws-ddk-core.EMRServerlessJobStage",
+):
+    '''Stage that contains a step function that runs an EMR Job.'''
+
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        application_id: builtins.str,
+        execution_role_arn: builtins.str,
+        job_driver: typing.Mapping[builtins.str, typing.Any],
+        job_execution_status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        start_job_run_props: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+        additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+        alarms_enabled: typing.Optional[builtins.bool] = None,
+        definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+        definition_file: typing.Optional[builtins.str] = None,
+        state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
+        state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
+        state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+        state_machine_name: typing.Optional[builtins.str] = None,
+        description: typing.Optional[builtins.str] = None,
+        name: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''Constructs EMRServerlessJobStage.
+
+        :param scope: Scope within which this construct is defined.
+        :param id: Identifier of the stage.
+        :param application_id: EMR Serverless Application Id.
+        :param execution_role_arn: EMR Execution Role Arn.
+        :param job_driver: The job driver for the job run. This is a Tagged Union structure. Only one of the following top level keys can be set: 'sparkSubmit', 'hive'
+        :param job_execution_status_check_period: Duration to wait between polling job status. Defaults to 30 seconds.
+        :param start_job_run_props: Additional properties to pass to 'emrserverless:StartJobRun'. https://docs.aws.amazon.com/emr-serverless/latest/APIReference/API_StartJobRun.html
+        :param additional_role_policy_statements: Additional IAM policy statements to add to the state machine role.
+        :param alarms_enabled: Enable/Disable all alarms in the stage. Default: true
+        :param definition: Steps for the state machine. Can either be provided as 'sfn.IChainable' or a JSON string.
+        :param definition_file: File containing a JSON definition for the state machine.
+        :param state_machine_failed_executions_alarm_evaluation_periods: The number of periods over which data is compared to the specified threshold. Default: 1
+        :param state_machine_failed_executions_alarm_threshold: The number of failed state machine executions before triggering CW alarm. Default: 1
+        :param state_machine_input: Input of the state machine.
+        :param state_machine_name: Name of the state machine.
+        :param description: Description of the stage.
+        :param name: Name of the stage.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__9cbec3de2f6cc9565e6ad8777b9c24ec8039d2679d0b58ae0f8a78bb7c12d9c3)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = EMRServerlessJobStageProps(
+            application_id=application_id,
+            execution_role_arn=execution_role_arn,
+            job_driver=job_driver,
+            job_execution_status_check_period=job_execution_status_check_period,
+            start_job_run_props=start_job_run_props,
+            additional_role_policy_statements=additional_role_policy_statements,
+            alarms_enabled=alarms_enabled,
+            definition=definition,
+            definition_file=definition_file,
+            state_machine_failed_executions_alarm_evaluation_periods=state_machine_failed_executions_alarm_evaluation_periods,
+            state_machine_failed_executions_alarm_threshold=state_machine_failed_executions_alarm_threshold,
+            state_machine_input=state_machine_input,
+            state_machine_name=state_machine_name,
+            description=description,
+            name=name,
+        )
+
+        jsii.create(self.__class__, self, [scope, id, props])
+
+    @builtins.property
+    @jsii.member(jsii_name="stateMachine")
+    def state_machine(self) -> _aws_cdk_aws_stepfunctions_ceddda9d.StateMachine:
+        '''State machine.'''
+        return typing.cast(_aws_cdk_aws_stepfunctions_ceddda9d.StateMachine, jsii.get(self, "stateMachine"))
+
+    @builtins.property
+    @jsii.member(jsii_name="eventPattern")
+    def event_pattern(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern]:
+        '''Output event pattern of the stage.
+
+        Event pattern describes the structure of output event(s) produced by this stage.
+        Event Rules use event patterns to select events and route them to targets.
+        '''
+        return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventPattern], jsii.get(self, "eventPattern"))
+
+    @builtins.property
+    @jsii.member(jsii_name="targets")
+    def targets(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]]:
+        '''Input targets for the stage.
+
+        Targets are used by Event Rules to describe what should be invoked when a rule matches an event.
+        '''
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_events_ceddda9d.IRuleTarget]], jsii.get(self, "targets"))
+
+
 class GlueTransformStage(
     StateMachineStage,
     metaclass=jsii.JSIIMeta,
     jsii_type="aws-ddk-core.GlueTransformStage",
 ):
     '''Stage that contains a step function that runs Glue job, and a Glue crawler afterwards.
 
@@ -10465,14 +11253,18 @@
     "DataBrewTransformStage",
     "DataBrewTransformStageProps",
     "DataPipeline",
     "DataPipelineProps",
     "DataStage",
     "DataStageProps",
     "DeliveryStreamProps",
+    "EMRServerlessCluster",
+    "EMRServerlessClusterProps",
+    "EMRServerlessJobStage",
+    "EMRServerlessJobStageProps",
     "EnvironmentConfiguration",
     "EventStage",
     "EventStageProps",
     "FirehoseToS3Stage",
     "FirehoseToS3StageProps",
     "GetConfigProps",
     "GetEnvConfigProps",
@@ -10890,14 +11682,70 @@
     encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
     role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     source_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__83d66a5f4ea6335b061a6877ac3664b7458c10cb62db78fcee7fdf475a19fee5(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    additional_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+    s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+    security_group: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SecurityGroup] = None,
+    vpc_cidr: typing.Optional[builtins.str] = None,
+    vpc_id: typing.Optional[builtins.str] = None,
+    release_label: builtins.str,
+    type: builtins.str,
+    architecture: typing.Optional[builtins.str] = None,
+    auto_start_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.AutoStartConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    auto_stop_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.AutoStopConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    image_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.ImageConfigurationInputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    initial_capacity: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Sequence[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.InitialCapacityConfigKeyValuePairProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+    maximum_capacity: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.MaximumAllowedResourcesProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    name: typing.Optional[builtins.str] = None,
+    network_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.NetworkConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    tags: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_ceddda9d.CfnTag, typing.Dict[builtins.str, typing.Any]]]] = None,
+    worker_type_specifications: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Mapping[builtins.str, typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.WorkerTypeSpecificationInputProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__864be4d07f911163bb991815f5a8c0561cfd97d707e687ef07552b1d38bb82d2(
+    scope: _constructs_77d1e7e8.Construct,
+    resource_name: builtins.str,
+    vpc_cidr: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__dff46b98beafa0af6fc125923b2225092c53114f275e10e2732de3f4d3cd2573(
+    *,
+    release_label: builtins.str,
+    type: builtins.str,
+    architecture: typing.Optional[builtins.str] = None,
+    auto_start_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.AutoStartConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    auto_stop_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.AutoStopConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    image_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.ImageConfigurationInputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    initial_capacity: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Sequence[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.InitialCapacityConfigKeyValuePairProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+    maximum_capacity: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.MaximumAllowedResourcesProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    name: typing.Optional[builtins.str] = None,
+    network_configuration: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.NetworkConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    tags: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_ceddda9d.CfnTag, typing.Dict[builtins.str, typing.Any]]]] = None,
+    worker_type_specifications: typing.Optional[typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Mapping[builtins.str, typing.Union[_aws_cdk_ceddda9d.IResolvable, typing.Union[_aws_cdk_aws_emrserverless_ceddda9d.CfnApplication.WorkerTypeSpecificationInputProperty, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+    additional_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+    s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
+    security_group: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SecurityGroup] = None,
+    vpc_cidr: typing.Optional[builtins.str] = None,
+    vpc_id: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__cf306c436463dcb56197f32e9c4793604595ef2ca8f42b2d72de058d5806870c(
     *,
     account: typing.Optional[builtins.str] = None,
     bootstrap: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     props: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     region: typing.Optional[builtins.str] = None,
     resources: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
@@ -11364,14 +12212,35 @@
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__a74bc867d821b2a380e6cc61db61d700e291094dae87fe77909819ed40f25b02(
+    *,
+    description: typing.Optional[builtins.str] = None,
+    name: typing.Optional[builtins.str] = None,
+    additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+    alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
+    state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
+    state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
+    state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+    state_machine_name: typing.Optional[builtins.str] = None,
+    application_id: builtins.str,
+    execution_role_arn: builtins.str,
+    job_driver: typing.Mapping[builtins.str, typing.Any],
+    job_execution_status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    start_job_run_props: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__41f4bcf520b1f5e4739a71110428c14cbff5ea45be37a68ea1fe04dbffd91d83(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
 ) -> None:
@@ -11653,14 +12522,37 @@
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
     definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
     definition_file: typing.Optional[builtins.str] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+    state_machine_name: typing.Optional[builtins.str] = None,
+    description: typing.Optional[builtins.str] = None,
+    name: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9cbec3de2f6cc9565e6ad8777b9c24ec8039d2679d0b58ae0f8a78bb7c12d9c3(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    application_id: builtins.str,
+    execution_role_arn: builtins.str,
+    job_driver: typing.Mapping[builtins.str, typing.Any],
+    job_execution_status_check_period: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    start_job_run_props: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+    additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+    alarms_enabled: typing.Optional[builtins.bool] = None,
+    definition: typing.Optional[typing.Union[builtins.str, _aws_cdk_aws_stepfunctions_ceddda9d.IChainable]] = None,
+    definition_file: typing.Optional[builtins.str] = None,
+    state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
+    state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
+    state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `aws-ddk-core-1.1.0/src/aws_ddk_core/_jsii/__init__.py` & `aws-ddk-core-1.2.0/src/aws_ddk_core/_jsii/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import aws_cdk.aws_glue_alpha._jsii
 import aws_cdk.aws_kinesisfirehose_alpha._jsii
 import aws_cdk.aws_kinesisfirehose_destinations_alpha._jsii
 import aws_cdk.integ_tests_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
-    "aws-ddk-core", "1.1.0", __name__[0:-6], "aws-ddk-core@1.1.0.jsii.tgz"
+    "aws-ddk-core", "1.2.0", __name__[0:-6], "aws-ddk-core@1.2.0.jsii.tgz"
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-ddk-core-1.1.0/src/aws_ddk_core.egg-info/PKG-INFO` & `aws-ddk-core-1.2.0/src/aws_ddk_core.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aws-ddk-core
-Version: 1.1.0
-Summary: AWS DataOps Development Kit
+Version: 1.2.0
+Summary: The AWS DataOps Development Kit is an open source development framework for customers that build data workflows and modern data architecture on AWS.
 Home-page: https://github.com/awslabs/aws-ddk/tree/main
 Author: AWS Professional Services<aws-proserve-orion-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-ddk/tree/main
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
```

