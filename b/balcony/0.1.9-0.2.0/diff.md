# Comparing `tmp/balcony-0.1.9.tar.gz` & `tmp/balcony-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balcony-0.1.9.tar", max compression
+gzip compressed data, was "balcony-0.2.0.tar", max compression
```

## Comparing `balcony-0.1.9.tar` & `balcony-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,52 @@
--rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.9/LICENSE
--rw-r--r--   0        0        0     3965 2023-07-22 10:16:18.349371 balcony-0.1.9/README.md
--rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.9/balcony/__init__.py
--rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.9/balcony/__main__.py
--rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.9/balcony/aws.py
--rw-r--r--   0        0        0    15169 2023-06-27 10:41:54.525900 balcony-0.1.9/balcony/botocore_utils.py
--rw-r--r--   0        0        0    22612 2023-07-17 18:22:23.044112 balcony-0.1.9/balcony/cli.py
--rw-r--r--   0        0        0     3723 2023-06-27 12:34:24.543878 balcony-0.1.9/balcony/config.py
--rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.9/balcony/custom_nodes/__init__.py
--rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.9/balcony/custom_nodes/codebuild.py
--rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.9/balcony/custom_nodes/ecs.py
--rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.9/balcony/custom_nodes/iam.py
--rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.9/balcony/custom_nodes/lambda_functions.py
--rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.9/balcony/custom_nodes/s3.py
--rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.9/balcony/custom_nodes/ses.py
--rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.9/balcony/custom_nodes/ssm.py
--rw-r--r--   0        0        0     2306 2023-07-16 15:42:11.020304 balcony-0.1.9/balcony/custom_tf_import_configs/ec2.yaml
--rw-r--r--   0        0        0      935 2023-07-18 19:25:23.582721 balcony-0.1.9/balcony/custom_tf_import_configs/ecs.yaml
--rw-r--r--   0        0        0     4728 2023-07-22 11:34:28.352856 balcony-0.1.9/balcony/custom_tf_import_configs/iam.yaml
--rw-r--r--   0        0        0     2015 2023-07-22 14:31:51.087927 balcony-0.1.9/balcony/custom_tf_import_configs/lambda.yaml
--rw-r--r--   0        0        0     1845 2023-06-27 20:18:18.446771 balcony-0.1.9/balcony/custom_tf_import_configs/rds.yaml
--rw-r--r--   0        0        0     6175 2023-07-22 15:35:18.928011 balcony-0.1.9/balcony/custom_tf_import_configs/s3.yaml
--rw-r--r--   0        0        0     4257 2023-07-17 18:18:53.104515 balcony-0.1.9/balcony/custom_tf_import_configs/vpc.yaml
--rw-r--r--   0        0        0     3271 2023-07-18 18:28:06.436858 balcony-0.1.9/balcony/custom_yamls/_example_service.yaml
--rw-r--r--   0        0        0      842 2023-07-16 11:53:29.831094 balcony-0.1.9/balcony/custom_yamls/ec2.yaml
--rw-r--r--   0        0        0     2704 2023-07-18 19:10:24.404655 balcony-0.1.9/balcony/custom_yamls/ecs.yaml
--rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.9/balcony/custom_yamls/iam.yaml
--rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.9/balcony/custom_yamls/s3.yaml
--rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.9/balcony/errors.py
--rw-r--r--   0        0        0    49314 2023-07-22 10:13:58.426856 balcony-0.1.9/balcony/nodes.py
--rw-r--r--   0        0        0    17434 2023-07-22 10:14:21.080169 balcony-0.1.9/balcony/reader.py
--rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.9/balcony/registries.py
--rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.9/balcony/relations.py
--rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.9/balcony/terraform_import/__init__.py
--rw-r--r--   0        0        0    10761 2023-07-22 10:49:58.891484 balcony-0.1.9/balcony/terraform_import/importer.py
--rw-r--r--   0        0        0     1320 2023-07-17 16:45:25.594486 balcony-0.1.9/balcony/terraform_import/models.py
--rw-r--r--   0        0        0     3877 2023-07-17 16:46:47.909479 balcony-0.1.9/balcony/terraform_import/parsers.py
--rw-r--r--   0        0        0    16069 2023-06-27 13:47:03.229109 balcony-0.1.9/balcony/terraform_import/wizard.py
--rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.9/balcony/test.py
--rw-r--r--   0        0        0     6553 2023-07-07 16:07:51.678302 balcony-0.1.9/balcony/utils.py
--rw-r--r--   0        0        0     2344 2023-07-18 18:43:44.785613 balcony-0.1.9/balcony/yaml_config.py
--rw-r--r--   0        0        0     2124 2023-07-18 18:27:00.154209 balcony-0.1.9/balcony/yaml_validators.py
--rw-r--r--   0        0        0      748 2023-07-22 16:31:26.037712 balcony-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     5263 1970-01-01 00:00:00.000000 balcony-0.1.9/setup.py
--rw-r--r--   0        0        0     5071 1970-01-01 00:00:00.000000 balcony-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-22 17:45:55.086961 balcony-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4098 2023-07-22 19:18:33.704478 balcony-0.2.0/README.md
+-rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.2.0/balcony/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.2.0/balcony/__main__.py
+-rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.2.0/balcony/aws.py
+-rw-r--r--   0        0        0    15169 2023-06-27 10:41:54.525900 balcony-0.2.0/balcony/botocore_utils.py
+-rw-r--r--   0        0        0    23845 2023-07-23 07:10:40.500404 balcony-0.2.0/balcony/cli.py
+-rw-r--r--   0        0        0     3723 2023-06-27 12:34:24.543878 balcony-0.2.0/balcony/config.py
+-rw-r--r--   0        0        0      506 2023-07-23 07:02:11.796340 balcony-0.2.0/balcony/custom_nodes/__init__.py
+-rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.2.0/balcony/custom_nodes/codebuild.py
+-rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.2.0/balcony/custom_nodes/ecs.py
+-rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.2.0/balcony/custom_nodes/iam.py
+-rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.2.0/balcony/custom_nodes/lambda_functions.py
+-rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.2.0/balcony/custom_nodes/s3.py
+-rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.2.0/balcony/custom_nodes/ses.py
+-rw-r--r--   0        0        0     1841 2023-07-23 07:08:48.352822 balcony-0.2.0/balcony/custom_nodes/sqs.py
+-rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.2.0/balcony/custom_nodes/ssm.py
+-rw-r--r--   0        0        0      313 2023-07-23 10:20:47.461565 balcony-0.2.0/balcony/custom_tf_import_configs/dynamodb.yaml
+-rw-r--r--   0        0        0     2306 2023-07-16 15:42:11.020304 balcony-0.2.0/balcony/custom_tf_import_configs/ec2.yaml
+-rw-r--r--   0        0        0      935 2023-07-18 19:25:23.582721 balcony-0.2.0/balcony/custom_tf_import_configs/ecs.yaml
+-rw-r--r--   0        0        0     2060 2023-07-22 18:29:13.636554 balcony-0.2.0/balcony/custom_tf_import_configs/elbv2.yaml
+-rw-r--r--   0        0        0     4728 2023-07-22 11:34:28.352856 balcony-0.2.0/balcony/custom_tf_import_configs/iam.yaml
+-rw-r--r--   0        0        0     2015 2023-07-22 14:31:51.087927 balcony-0.2.0/balcony/custom_tf_import_configs/lambda.yaml
+-rw-r--r--   0        0        0     1845 2023-06-27 20:18:18.446771 balcony-0.2.0/balcony/custom_tf_import_configs/rds.yaml
+-rw-r--r--   0        0        0     6175 2023-07-22 15:35:18.928011 balcony-0.2.0/balcony/custom_tf_import_configs/s3.yaml
+-rw-r--r--   0        0        0     1471 2023-07-23 10:17:47.735155 balcony-0.2.0/balcony/custom_tf_import_configs/sns.yaml
+-rw-r--r--   0        0        0      555 2023-07-23 07:18:44.485172 balcony-0.2.0/balcony/custom_tf_import_configs/sqs.yaml
+-rw-r--r--   0        0        0     4257 2023-07-17 18:18:53.104515 balcony-0.2.0/balcony/custom_tf_import_configs/vpc.yaml
+-rw-r--r--   0        0        0     3271 2023-07-18 18:28:06.436858 balcony-0.2.0/balcony/custom_yamls/_example_service.yaml
+-rw-r--r--   0        0        0      842 2023-07-16 11:53:29.831094 balcony-0.2.0/balcony/custom_yamls/ec2.yaml
+-rw-r--r--   0        0        0     2704 2023-07-18 19:10:24.404655 balcony-0.2.0/balcony/custom_yamls/ecs.yaml
+-rw-r--r--   0        0        0     1047 2023-07-22 18:24:58.223256 balcony-0.2.0/balcony/custom_yamls/elbv2.yaml
+-rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.2.0/balcony/custom_yamls/iam.yaml
+-rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.2.0/balcony/custom_yamls/s3.yaml
+-rw-r--r--   0        0        0      612 2023-07-23 07:15:08.036683 balcony-0.2.0/balcony/custom_yamls/sqs.yaml
+-rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.2.0/balcony/errors.py
+-rw-r--r--   0        0        0    49415 2023-07-23 06:53:05.472848 balcony-0.2.0/balcony/nodes.py
+-rw-r--r--   0        0        0    17434 2023-07-22 10:14:21.080169 balcony-0.2.0/balcony/reader.py
+-rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.2.0/balcony/registries.py
+-rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.2.0/balcony/relations.py
+-rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.2.0/balcony/terraform_import/__init__.py
+-rw-r--r--   0        0        0    10761 2023-07-22 10:49:58.891484 balcony-0.2.0/balcony/terraform_import/importer.py
+-rw-r--r--   0        0        0     1320 2023-07-17 16:45:25.594486 balcony-0.2.0/balcony/terraform_import/models.py
+-rw-r--r--   0        0        0     3877 2023-07-17 16:46:47.909479 balcony-0.2.0/balcony/terraform_import/parsers.py
+-rw-r--r--   0        0        0    16075 2023-07-23 07:10:46.157322 balcony-0.2.0/balcony/terraform_import/wizard.py
+-rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.2.0/balcony/test.py
+-rw-r--r--   0        0        0     6553 2023-07-07 16:07:51.678302 balcony-0.2.0/balcony/utils.py
+-rw-r--r--   0        0        0     2344 2023-07-18 18:43:44.785613 balcony-0.2.0/balcony/yaml_config.py
+-rw-r--r--   0        0        0     2124 2023-07-18 18:27:00.154209 balcony-0.2.0/balcony/yaml_validators.py
+-rw-r--r--   0        0        0      742 2023-07-27 09:43:04.026970 balcony-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5399 1970-01-01 00:00:00.000000 balcony-0.2.0/setup.py
+-rw-r--r--   0        0        0     5174 1970-01-01 00:00:00.000000 balcony-0.2.0/PKG-INFO
```

### Comparing `balcony-0.1.9/README.md` & `balcony-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 Terraform v1.5 introduced [import blocks](https://developer.hashicorp.com/terraform/language/import) that allows users to define their imports as code.
 
 `balcony terraform-import <service> <resource-name>` command generates these import blocks for you.
 
 `balcony terraform-import --list` to see the list of supported resources.
 
 Related Docs: [Generate Terraform Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/)
+Related Docs: [Balcony Terraform Import Support Matrix](https://oguzhan-yilmaz.github.io/balcony/terraform-import-support-matrix/)
+
+
 
 ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif)
 
 
 ---
 
 ### Generate actual Terraform Resource Code
```

#### html2text {}

```diff
@@ -19,28 +19,29 @@
 yilmaz.github.io/balcony/quickstart/) ![](https://raw.githubusercontent.com/
 oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif) --- ### Generate
 Terraform Import Blocks Terraform v1.5 introduced [import blocks](https://
 developer.hashicorp.com/terraform/language/import) that allows users to define
 their imports as code. `balcony terraform-import  ` command generates these
 import blocks for you. `balcony terraform-import --list` to see the list of
 supported resources. Related Docs: [Generate Terraform Import Blocks](https://
-oguzhan-yilmaz.github.io/balcony/terraform-import/) ![](https://
-raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
-import-blocks-example.gif) --- ### Generate actual Terraform Resource Code If
-you have: - initialized terraform project - `import_blocks.tf` file that's
-generated with `balcony terraform-import` command you can run `terraform plan -
-generate-config-out=generated.tf` to generate actual `.tf` resource code. This
-feature is achieved with the [balcony-terraform-import Docker Image](https://
-github.com/oguzhan-yilmaz/balcony/pkgs/container/balcony-terraform-import).
-Related Docs: [Generate Terraform Code with Docker Image](https://oguzhan-
-yilmaz.github.io/balcony/terraform-import-docker/) ![](https://
-raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-
-tf-code-ec2-insances-example.gif) --- ### Interactive Wizard to create balcony
-import configurations Balcony doesn't know how to create terraform `import
-blocks` for all of the AWS resources. It can be taught how to do it by creating
-`import-configurations` yaml files, but it's a manual process. This is where
-the interactive wizard comes in. Interactive Wizards asks you required
-questions to automatically create the `import-configurations` yaml files.
-Related Docs: [Terraform Import Configuration Wizard](https://oguzhan-
-yilmaz.github.io/balcony/terraform-import-wizard/) ![](https://
-raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
-wizard-security-groups-example.gif)
+oguzhan-yilmaz.github.io/balcony/terraform-import/) Related Docs: [Balcony
+Terraform Import Support Matrix](https://oguzhan-yilmaz.github.io/balcony/
+terraform-import-support-matrix/) ![](https://raw.githubusercontent.com/
+oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif) --
+- ### Generate actual Terraform Resource Code If you have: - initialized
+terraform project - `import_blocks.tf` file that's generated with `balcony
+terraform-import` command you can run `terraform plan -generate-config-
+out=generated.tf` to generate actual `.tf` resource code. This feature is
+achieved with the [balcony-terraform-import Docker Image](https://github.com/
+oguzhan-yilmaz/balcony/pkgs/container/balcony-terraform-import). Related Docs:
+[Generate Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/
+balcony/terraform-import-docker/) ![](https://raw.githubusercontent.com/
+oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-
+example.gif) --- ### Interactive Wizard to create balcony import configurations
+Balcony doesn't know how to create terraform `import blocks` for all of the AWS
+resources. It can be taught how to do it by creating `import-configurations`
+yaml files, but it's a manual process. This is where the interactive wizard
+comes in. Interactive Wizards asks you required questions to automatically
+create the `import-configurations` yaml files. Related Docs: [Terraform Import
+Configuration Wizard](https://oguzhan-yilmaz.github.io/balcony/terraform-
+import-wizard/) ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-
+assets/main/gifs/terraform-wizard-security-groups-example.gif)
```

### Comparing `balcony-0.1.9/balcony/__init__.py` & `balcony-0.2.0/balcony/__init__.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/aws.py` & `balcony-0.2.0/balcony/aws.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/botocore_utils.py` & `balcony-0.2.0/balcony/botocore_utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/cli.py` & `balcony-0.2.0/balcony/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             )
             if similar_service_names:
                 console.print("[yellow]Found Similar Service Names:")
                 console.print(Columns(similar_service_names, equal=True, expand=True))
                 return
             else:
                 raise typer.Exit(
-                    f"Invalid service name: {service}. Please pick a proper one."
+                    f"Invalid service name: {service}. Please pick a proper one.", code=-1
                 )
 
         service_node = balcony_aws.get_service_node(service)
         resource_nodes = service_node.get_resource_nodes()
 
         resource_node_names = []
         for _rn in resource_nodes:
@@ -180,15 +180,16 @@
             )
             if similar_resource_names:
                 console.print("[yellow]Found Similar Resource Node Names:")
                 console.print(Columns(similar_resource_names, equal=True, expand=True))
                 return
             else:
                 raise typer.Exit(
-                    f"Invalid Resource Node name: [bold]{resource_node}[/] for Service: [bold]{service}[/]."
+                    f"Invalid Resource Node name: [bold]{resource_node}[/] for Service: [bold]{service}[/].",
+                    code=-1
                 )
         operations_panel = service_node._get_operation_details_panel(
             resource_node_obj.name
         )
         if screen_pager:
             with console.pager(styles=True):
                 console.print(operations_panel)
@@ -265,40 +266,40 @@
     ),
 ):
     if debug:
         set_log_level_at_runtime(logging.DEBUG)
 
     if list_contents:
         _list_service_or_resource(service, resource_node, screen_pager=screen)
-        raise typer.Exit()
+        raise typer.Exit(code=0)
 
     # warn user if pagination is not set
     if not follow_pagination:
         logger.debug(
             "[underline][yellow bold][WARNING][/] [bold][--paginate, -p][/] option [bold red]is NOT set[/]. You're likely to get incomplete data.[/]"
         )
     service_markup = f"[green]{service}[/]"
 
     if not service and not resource_node:
         # print out resource nodes of this service.
         _list_service_or_resource(service, resource_node, screen_pager=screen)
         console.print(
             Panel("[bold]Please pick one of the AWS Services", title="[red][bold]ERROR")
         )
-        raise typer.Exit()
+        raise typer.Exit(code=-1)
 
     if service and not resource_node:
         _list_service_or_resource(service, resource_node, screen_pager=screen)
         console.print(
             Panel(
                 f"[bold]Please pick one of the Resource Nodes from {service_markup} Service",
                 title="[red][bold]ERROR",
             )
         )
-        raise typer.Exit()
+        raise typer.Exit(code=-1)
 
     elif service and resource_node:
         service_node = balcony_aws.get_service_node(service)
         service_reader = service_node.get_service_reader()
 
         is_operation_selected = operation is not None
         read_data = None
@@ -348,34 +349,69 @@
                             f"Failed to format  [red]{str(e)}[/] with data: {r_data}"
                         )
 
                 if output_file:
                     output_filepath = Path(output_file).resolve()
                     logger.info(f"Saving output to: {output_filepath}")
                     save_str_list_to_output_file(output_filepath, formatted_output_list)
-                    raise typer.Exit()
+                    raise typer.Exit(code=0)
                 else:
                     # print to console
                     console.print("\n".join(formatted_output_list), overflow="ignore")
-                    raise typer.Exit()
+                    raise typer.Exit(code=0)
             else:
                 logger.debug(
                     f"[red]No data found.[/] Failed to use --format: '{formatter}'"
                 )
 
         if screen:
             with console.pager(styles=True):
                 console.print_json(data=read_data, default=str)
         elif output_file:
             output_filepath = Path(output_file).resolve()
             logger.info(f"Saving output to: {output_filepath}")
             save_dict_to_output_file(output_filepath, read_data)
         else:
             console.print_json(data=read_data, default=str)
-        raise typer.Exit()
+        raise typer.Exit(code=0)
+
+
+@app.command(
+    "terraform-import-support-matrix",
+    # no_args_is_help=True,
+    short_help="Show Terraform Import Support Matrix for AWS Services.",
+    help="""Show Terraform Import Support Matrix for AWS Services.""",
+)
+def terraform_import_support_matrix(
+    no_markdown_render: bool = typer.Option(
+        False,
+        "--no-md-render",
+        help="Doesn't renders the markdown table, instead prints the raw data.",
+    ),
+):
+    service_resource_list = get_importable_resources()
+
+    header = f"# Balcony Terraform Import Support Matrix\n".format()
+    header += f"| {'TerraformResourceType':<50} | {'Service':>15} | {'Resource':45} |\n".format()
+    header += f"| {'---':50} | {'---':15} | {'---':45} |\n".format()
+    result = header
+
+    for i, (terraform_type, service_name, resource_name) in enumerate(
+        service_resource_list
+    ):
+        cur_line = f"| {terraform_type:<50} | {service_name:>15} | {resource_name:45} |"
+        result += cur_line + "\n"
+
+    if no_markdown_render:
+        console.print(result)
+    else:
+        from rich.markdown import Markdown
+        console.print(Markdown(result))
+
+
 
 
 @app.command(
     "terraform-import",
     no_args_is_help=True,
     short_help="Generate Terraform import blocks for a given AWS Service and Resource Node.",
     help="""
@@ -492,21 +528,21 @@
                     Run     [bold]balcony aws {service_or_tf_resource_type}[/]      to see available resource nodes.
                 
                 - [underline]You may not have any resources in your AWS Account, check it first:[/]
                     Run     [bold]balcony aws {service_or_tf_resource_type} {resource_node} -d[/] 
             """
         ).strip()
         console.print(Padding(fail_msg, (1, 1)))
-        raise typer.Exit(-1)
+        raise typer.Exit(code=-1)
 
     if output_file:
         output_filepath = Path(output_file).resolve()
         logger.info(f"Saving output to: {output_filepath}")
         save_str_list_to_output_file(output_filepath, import_blocks)
-        raise typer.Exit()
+        raise typer.Exit(code=0)
 
     else:
         if screen:
             with console.pager(styles=True):
                 console.print("\n".join(import_blocks))
         else:            
             console.print("\n".join(import_blocks))
@@ -551,15 +587,15 @@
 ):
     # set debug level if enabled
     if debug:
         set_log_level_at_runtime(logging.DEBUG)
 
     if list_contents:
         _list_service_or_resource(service, resource_node, screen_pager=screen)
-        raise typer.Exit()
+        raise typer.Exit(code=0)
 
     if (not service) or (not resource_node):
         _list_service_or_resource(service, resource_node, screen_pager=screen)
 
         console.print(f"[red bold]Please pick a Service and Resource Node[/]")
         return
```

### Comparing `balcony-0.1.9/balcony/config.py` & `balcony-0.2.0/balcony/config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_nodes/codebuild.py` & `balcony-0.2.0/balcony/custom_nodes/codebuild.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_nodes/ecs.py` & `balcony-0.2.0/balcony/custom_nodes/ecs.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_nodes/iam.py` & `balcony-0.2.0/balcony/custom_nodes/iam.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_nodes/lambda_functions.py` & `balcony-0.2.0/balcony/custom_nodes/lambda_functions.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_nodes/s3.py` & `balcony-0.2.0/balcony/custom_nodes/s3.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_nodes/ses.py` & `balcony-0.2.0/balcony/custom_nodes/ses.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_nodes/ssm.py` & `balcony-0.2.0/balcony/custom_nodes/ssm.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_tf_import_configs/ec2.yaml` & `balcony-0.2.0/balcony/custom_tf_import_configs/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_tf_import_configs/ecs.yaml` & `balcony-0.2.0/balcony/custom_tf_import_configs/ecs.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_tf_import_configs/iam.yaml` & `balcony-0.2.0/balcony/custom_tf_import_configs/iam.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_tf_import_configs/lambda.yaml` & `balcony-0.2.0/balcony/custom_tf_import_configs/lambda.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_tf_import_configs/rds.yaml` & `balcony-0.2.0/balcony/custom_tf_import_configs/rds.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_tf_import_configs/s3.yaml` & `balcony-0.2.0/balcony/custom_tf_import_configs/s3.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_tf_import_configs/vpc.yaml` & `balcony-0.2.0/balcony/custom_tf_import_configs/vpc.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_yamls/_example_service.yaml` & `balcony-0.2.0/balcony/custom_yamls/_example_service.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_yamls/ec2.yaml` & `balcony-0.2.0/balcony/custom_yamls/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_yamls/ecs.yaml` & `balcony-0.2.0/balcony/custom_yamls/ecs.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/custom_yamls/iam.yaml` & `balcony-0.2.0/balcony/custom_yamls/iam.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/nodes.py` & `balcony-0.2.0/balcony/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1147,48 +1147,49 @@
             )
             if created_resource_node:
                 generated_resouce_nodes.append(created_resource_node)
 
         if len(generated_resouce_nodes) <= 1:
             return generated_resouce_nodes
 
-        # TODO: decide if this should be kept
-        # concat same names
-        combined_resource_nodes = []
-        _used_for_combining_resource_nodes = []
-
-        for i, gen_resource_node in enumerate(generated_resouce_nodes[:-1]):
-            if gen_resource_node in _used_for_combining_resource_nodes:
-                continue
-            for other_resource_node in generated_resouce_nodes[i + 1 :]:
-                # FIXME: IMPORTANT
-                if compare_two_camel_case_words(
-                    gen_resource_node.name, other_resource_node.name
-                ):
-                    # select the shortest name, meaning singular
-                    singular_named_resource_node = gen_resource_node
-                    plural_named_resource_node = other_resource_node
-                    if len(singular_named_resource_node.name) > len(
-                        plural_named_resource_node.name
-                    ):
-                        singular_named_resource_node, plural_named_resource_node = (
-                            plural_named_resource_node,
-                            singular_named_resource_node,
-                        )
-                    _used_for_combining_resource_nodes.append(
-                        plural_named_resource_node
-                    )
-                    singular_named_resource_node.operation_names.extend(
-                        plural_named_resource_node.operation_names
-                    )
+        # # TODO: decide if this should be kept
+        # # concat same names
+        # combined_resource_nodes = []
+        # _used_for_combining_resource_nodes = []
+
+        # for i, gen_resource_node in enumerate(generated_resouce_nodes[:-1]):
+        #     if gen_resource_node in _used_for_combining_resource_nodes:
+        #         continue
+        #     for other_resource_node in generated_resouce_nodes[i + 1 :]:
+        #         # FIXME: IMPORTANT
+        #         if compare_two_camel_case_words(
+        #             gen_resource_node.name, other_resource_node.name
+        #         ):
+        #             # select the shortest name, meaning singular
+        #             singular_named_resource_node = gen_resource_node
+        #             plural_named_resource_node = other_resource_node
+        #             if len(singular_named_resource_node.name) > len(
+        #                 plural_named_resource_node.name
+        #             ):
+        #                 singular_named_resource_node, plural_named_resource_node = (
+        #                     plural_named_resource_node,
+        #                     singular_named_resource_node,
+        #                 )
+        #             _used_for_combining_resource_nodes.append(
+        #                 plural_named_resource_node
+        #             )
+        #             singular_named_resource_node.operation_names.extend(
+        #                 plural_named_resource_node.operation_names
+        #             )
 
-            if gen_resource_node not in _used_for_combining_resource_nodes:
-                combined_resource_nodes.append(gen_resource_node)
+        #     if gen_resource_node not in _used_for_combining_resource_nodes:
+        #         combined_resource_nodes.append(gen_resource_node)
 
-        return combined_resource_nodes
+        # return combined_resource_nodes
+        return generated_resouce_nodes
 
     def get_read_operation_name_to_tokens_map(self) -> Dict:
         """Generate `operation name to word tokens` map for the
         available read operations in the ServiceNode.
 
         Caches the output in the class attr. `_read_operation_name_to_tokens_map`.
```

### Comparing `balcony-0.1.9/balcony/reader.py` & `balcony-0.2.0/balcony/reader.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/registries.py` & `balcony-0.2.0/balcony/registries.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/relations.py` & `balcony-0.2.0/balcony/relations.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/terraform_import/importer.py` & `balcony-0.2.0/balcony/terraform_import/importer.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/terraform_import/models.py` & `balcony-0.2.0/balcony/terraform_import/models.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/terraform_import/parsers.py` & `balcony-0.2.0/balcony/terraform_import/parsers.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/terraform_import/wizard.py` & `balcony-0.2.0/balcony/terraform_import/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     operation_names = get_operation_names_of_a_resource(
         balcony_aws, service, resource_name
     )
     if not operation_names:
         console.print(
             f"[red bold]No operations found for {service}.{resource_name}[/red bold]"
         )
-        raise typer.Exit(1)
+        raise typer.Exit(code=-1)
 
     console.print()
     console.rule("[bold cyan underline]Operation Selection")
     console.print()
     console.print("balcony may have multiple Operations for a Resource.")
     console.print(
         "Select which operation to use for generating the import configuration."
```

### Comparing `balcony-0.1.9/balcony/test.py` & `balcony-0.2.0/balcony/test.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/utils.py` & `balcony-0.2.0/balcony/utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/yaml_config.py` & `balcony-0.2.0/balcony/yaml_config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/balcony/yaml_validators.py` & `balcony-0.2.0/balcony/yaml_validators.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.9/pyproject.toml` & `balcony-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "balcony"
-version = "0.1.9"
+version = "0.2.0"
 description = "Read any resource in your AWS Account. You can generate terraform code for them, too."
 authors = ["Oguzhan Yilmaz <oguzhanylmz271@gmail.com>"]
-license = "GPL-3.0-or-later"
+license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 balcony = "balcony.cli:run_app"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `balcony-0.1.9/setup.py` & `balcony-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,17 +21,17 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['balcony = balcony.cli:run_app']}
 
 setup_kwargs = {
     'name': 'balcony',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': 'Read any resource in your AWS Account. You can generate terraform code for them, too.',
-    'long_description': '# balcony\n\n\n<div style="display: flex;">\n  <a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml/badge.svg" alt="Build and publish a Docker image to ghcr.io"></a>\n  <span style="width: 5px"></span>\n\n<a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment/badge.svg" alt="Build and Deploy Documentation website"></a>\n</div>\n\n\nbalcony is a modern CLI tool that with some killer features:\n\n- Auto-fill the required parameters for AWS API calls \n- Read the JSON data of any AWS resource in your account\n- Generate [Terraform Import Blocks](https://developer.hashicorp.com/terraform/language/import)\n- Generate actual `.tf` Terraform Resource code\n\nbalcony uses _read-only_ operations, it does not take any action on the used AWS account.\n\n\n### [Visit the Documentation Website](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n<!-- ### [**Go to QuickStart Page to get started using _balcony_**](quickstart.md) -->\n\n### Installation\n\n```bash\npip3 install balcony\n```\n\nVisit [**Installation & QuickStart Page**](https://oguzhan-yilmaz.github.io/balcony/quickstart/) to get started using _balcony_\n\n```bash  title="Basic usage"\n# see options\nbalcony\n\n# list available resources of ec2\nbalcony aws ec2 \n\n# read a resource\nbalcony aws s3 Buckets\n\n# show documentation\nbalcony aws iam Policy --list\n\n# generate terraform import blocks for a resource\nbalcony terraform-import s3 Buckets\n```\n\n\n## Features\n\n### Read any AWS Resource\n\n`balcony aws <service> <resource-name> --paginate` command reads all resources of a given type in your AWS account.\n\nRelated Docs: [QuickStart](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif)\n\n\n---\n\n### Generate Terraform Import Blocks\n\nTerraform v1.5 introduced [import blocks](https://developer.hashicorp.com/terraform/language/import) that allows users to define their imports as code.\n\n`balcony terraform-import <service> <resource-name>` command generates these import blocks for you.\n\n`balcony terraform-import --list` to see the list of supported resources.\n\nRelated Docs: [Generate Terraform Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif)\n\n\n---\n\n### Generate actual Terraform Resource Code \n\n\nIf you have:\n\n- initialized terraform project\n- `import_blocks.tf` file that\'s generated with `balcony terraform-import` command\n\nyou can run `terraform plan -generate-config-out=generated.tf` to generate actual `.tf` resource code.\n\nThis feature is achieved with the [balcony-terraform-import Docker Image](https://github.com/oguzhan-yilmaz/balcony/pkgs/container/balcony-terraform-import).\n\n\nRelated Docs: [Generate Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-docker/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-example.gif)\n\n\n---\n\n### Interactive Wizard to create balcony import configurations \n\nBalcony doesn\'t know how to create terraform `import blocks` for all of the AWS resources.\n\nIt can be taught how to do it by creating `import-configurations` yaml files, but it\'s a manual process. This is where the interactive wizard comes in.\n\nInteractive Wizards asks you required questions to automatically create the `import-configurations` yaml files.\n\nRelated Docs: [Terraform Import Configuration Wizard](https://oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-wizard-security-groups-example.gif)\n',
+    'long_description': '# balcony\n\n\n<div style="display: flex;">\n  <a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml/badge.svg" alt="Build and publish a Docker image to ghcr.io"></a>\n  <span style="width: 5px"></span>\n\n<a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment/badge.svg" alt="Build and Deploy Documentation website"></a>\n</div>\n\n\nbalcony is a modern CLI tool that with some killer features:\n\n- Auto-fill the required parameters for AWS API calls \n- Read the JSON data of any AWS resource in your account\n- Generate [Terraform Import Blocks](https://developer.hashicorp.com/terraform/language/import)\n- Generate actual `.tf` Terraform Resource code\n\nbalcony uses _read-only_ operations, it does not take any action on the used AWS account.\n\n\n### [Visit the Documentation Website](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n<!-- ### [**Go to QuickStart Page to get started using _balcony_**](quickstart.md) -->\n\n### Installation\n\n```bash\npip3 install balcony\n```\n\nVisit [**Installation & QuickStart Page**](https://oguzhan-yilmaz.github.io/balcony/quickstart/) to get started using _balcony_\n\n```bash  title="Basic usage"\n# see options\nbalcony\n\n# list available resources of ec2\nbalcony aws ec2 \n\n# read a resource\nbalcony aws s3 Buckets\n\n# show documentation\nbalcony aws iam Policy --list\n\n# generate terraform import blocks for a resource\nbalcony terraform-import s3 Buckets\n```\n\n\n## Features\n\n### Read any AWS Resource\n\n`balcony aws <service> <resource-name> --paginate` command reads all resources of a given type in your AWS account.\n\nRelated Docs: [QuickStart](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif)\n\n\n---\n\n### Generate Terraform Import Blocks\n\nTerraform v1.5 introduced [import blocks](https://developer.hashicorp.com/terraform/language/import) that allows users to define their imports as code.\n\n`balcony terraform-import <service> <resource-name>` command generates these import blocks for you.\n\n`balcony terraform-import --list` to see the list of supported resources.\n\nRelated Docs: [Generate Terraform Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/)\nRelated Docs: [Balcony Terraform Import Support Matrix](https://oguzhan-yilmaz.github.io/balcony/terraform-import-support-matrix/)\n\n\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif)\n\n\n---\n\n### Generate actual Terraform Resource Code \n\n\nIf you have:\n\n- initialized terraform project\n- `import_blocks.tf` file that\'s generated with `balcony terraform-import` command\n\nyou can run `terraform plan -generate-config-out=generated.tf` to generate actual `.tf` resource code.\n\nThis feature is achieved with the [balcony-terraform-import Docker Image](https://github.com/oguzhan-yilmaz/balcony/pkgs/container/balcony-terraform-import).\n\n\nRelated Docs: [Generate Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-docker/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-example.gif)\n\n\n---\n\n### Interactive Wizard to create balcony import configurations \n\nBalcony doesn\'t know how to create terraform `import blocks` for all of the AWS resources.\n\nIt can be taught how to do it by creating `import-configurations` yaml files, but it\'s a manual process. This is where the interactive wizard comes in.\n\nInteractive Wizards asks you required questions to automatically create the `import-configurations` yaml files.\n\nRelated Docs: [Terraform Import Configuration Wizard](https://oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-wizard-security-groups-example.gif)\n',
     'author': 'Oguzhan Yilmaz',
     'author_email': 'oguzhanylmz271@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 ['*'], 'balcony': ['custom_tf_import_configs/*', 'custom_yamls/*']}
 install_requires = \ ['Jinja2>=3.1.2,<4.0.0', 'PyYAML>=6.0,<7.0',
 'boto3>=1.24.80,<2.0.0', 'inflect>=6.0.0,<7.0.0', 'jmespath>=1.0.1,<2.0.0',
 'mkdocs-autorefs>=0.4.1,<0.5.0', 'mkdocs-material>=8.5.7,<10.0.0',
 'mkdocstrings[python]>=0.21.2,<0.22.0', 'pydantic>=1.10.7,<2.0.0',
 'rich>=13.3.4,<14.0.0', 'typer>=0.7.0,<0.8.0'] entry_points = \
 {'console_scripts': ['balcony = balcony.cli:run_app']} setup_kwargs = { 'name':
-'balcony', 'version': '0.1.9', 'description': 'Read any resource in your AWS
+'balcony', 'version': '0.2.0', 'description': 'Read any resource in your AWS
 Account. You can generate terraform code for them, too.', 'long_description':
 '# balcony\n\n\n
 \n [Build_and_publish_a_Docker_image_to_ghcr.io]\n \n\n[Build_and_Deploy
 Documentation_website]\n
 \n\n\nbalcony is a modern CLI tool that with some killer features:\n\n- Auto-
 fill the required parameters for AWS API calls \n- Read the JSON data of any
 AWS resource in your account\n- Generate [Terraform Import Blocks](https://
@@ -31,18 +31,20 @@
 yilmaz.github.io/balcony/quickstart/)\n\n![](https://raw.githubusercontent.com/
 oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif)\n\n\n---\n\n###
 Generate Terraform Import Blocks\n\nTerraform v1.5 introduced [import blocks]
 (https://developer.hashicorp.com/terraform/language/import) that allows users
 to define their imports as code.\n\n`balcony terraform-import  ` command
 generates these import blocks for you.\n\n`balcony terraform-import --list` to
 see the list of supported resources.\n\nRelated Docs: [Generate Terraform
-Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/)\n\n!
-[](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/
-terraform-import-blocks-example.gif)\n\n\n---\n\n### Generate actual Terraform
-Resource Code \n\n\nIf you have:\n\n- initialized terraform project\n-
+Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/
+)\nRelated Docs: [Balcony Terraform Import Support Matrix](https://oguzhan-
+yilmaz.github.io/balcony/terraform-import-support-matrix/)\n\n\n\n![](https://
+raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
+import-blocks-example.gif)\n\n\n---\n\n### Generate actual Terraform Resource
+Code \n\n\nIf you have:\n\n- initialized terraform project\n-
 `import_blocks.tf` file that\'s generated with `balcony terraform-import`
 command\n\nyou can run `terraform plan -generate-config-out=generated.tf` to
 generate actual `.tf` resource code.\n\nThis feature is achieved with the
 [balcony-terraform-import Docker Image](https://github.com/oguzhan-yilmaz/
 balcony/pkgs/container/balcony-terraform-import).\n\n\nRelated Docs: [Generate
 Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/balcony/
 terraform-import-docker/)\n\n![](https://raw.githubusercontent.com/oguzhan-
```

### Comparing `balcony-0.1.9/PKG-INFO` & `balcony-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: balcony
-Version: 0.1.9
+Version: 0.2.0
 Summary: Read any resource in your AWS Account. You can generate terraform code for them, too.
-License: GPL-3.0-or-later
+License: Apache-2.0
 Author: Oguzhan Yilmaz
 Author-email: oguzhanylmz271@gmail.com
 Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
@@ -93,14 +93,17 @@
 Terraform v1.5 introduced [import blocks](https://developer.hashicorp.com/terraform/language/import) that allows users to define their imports as code.
 
 `balcony terraform-import <service> <resource-name>` command generates these import blocks for you.
 
 `balcony terraform-import --list` to see the list of supported resources.
 
 Related Docs: [Generate Terraform Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/)
+Related Docs: [Balcony Terraform Import Support Matrix](https://oguzhan-yilmaz.github.io/balcony/terraform-import-support-matrix/)
+
+
 
 ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif)
 
 
 ---
 
 ### Generate actual Terraform Resource Code
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: balcony Version: 0.1.9 Summary: Read any resource
+Metadata-Version: 2.1 Name: balcony Version: 0.2.0 Summary: Read any resource
 in your AWS Account. You can generate terraform code for them, too. License:
-GPL-3.0-or-later Author: Oguzhan Yilmaz Author-email: oguzhanylmz271@gmail.com
-Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: GNU General
-Public License v3 or later (GPLv3+) Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Jinja2
-(>=3.1.2,<4.0.0) Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: boto3
-(>=1.24.80,<2.0.0) Requires-Dist: inflect (>=6.0.0,<7.0.0) Requires-Dist:
-jmespath (>=1.0.1,<2.0.0) Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0)
-Requires-Dist: mkdocs-material (>=8.5.7,<10.0.0) Requires-Dist: mkdocstrings
-[python] (>=0.21.2,<0.22.0) Requires-Dist: pydantic (>=1.10.7,<2.0.0) Requires-
-Dist: rich (>=13.3.4,<14.0.0) Requires-Dist: typer (>=0.7.0,<0.8.0)
-Description-Content-Type: text/markdown # balcony
+Apache-2.0 Author: Oguzhan Yilmaz Author-email: oguzhanylmz271@gmail.com
+Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: boto3 (>=1.24.80,<2.0.0)
+Requires-Dist: inflect (>=6.0.0,<7.0.0) Requires-Dist: jmespath
+(>=1.0.1,<2.0.0) Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) Requires-Dist:
+mkdocs-material (>=8.5.7,<10.0.0) Requires-Dist: mkdocstrings[python]
+(>=0.21.2,<0.22.0) Requires-Dist: pydantic (>=1.10.7,<2.0.0) Requires-Dist:
+rich (>=13.3.4,<14.0.0) Requires-Dist: typer (>=0.7.0,<0.8.0) Description-
+Content-Type: text/markdown # balcony
 [Build_and_publish_a_Docker_image_to_ghcr.io]  [Build_and_Deploy_Documentation
 website]
 balcony is a modern CLI tool that with some killer features: - Auto-fill the
 required parameters for AWS API calls - Read the JSON data of any AWS resource
 in your account - Generate [Terraform Import Blocks](https://
 developer.hashicorp.com/terraform/language/import) - Generate actual `.tf`
 Terraform Resource code balcony uses _read-only_ operations, it does not take
@@ -33,28 +33,29 @@
 yilmaz.github.io/balcony/quickstart/) ![](https://raw.githubusercontent.com/
 oguzhan-yilmaz/balcony-assets/main/gifs/aws-read-resource.gif) --- ### Generate
 Terraform Import Blocks Terraform v1.5 introduced [import blocks](https://
 developer.hashicorp.com/terraform/language/import) that allows users to define
 their imports as code. `balcony terraform-import  ` command generates these
 import blocks for you. `balcony terraform-import --list` to see the list of
 supported resources. Related Docs: [Generate Terraform Import Blocks](https://
-oguzhan-yilmaz.github.io/balcony/terraform-import/) ![](https://
-raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
-import-blocks-example.gif) --- ### Generate actual Terraform Resource Code If
-you have: - initialized terraform project - `import_blocks.tf` file that's
-generated with `balcony terraform-import` command you can run `terraform plan -
-generate-config-out=generated.tf` to generate actual `.tf` resource code. This
-feature is achieved with the [balcony-terraform-import Docker Image](https://
-github.com/oguzhan-yilmaz/balcony/pkgs/container/balcony-terraform-import).
-Related Docs: [Generate Terraform Code with Docker Image](https://oguzhan-
-yilmaz.github.io/balcony/terraform-import-docker/) ![](https://
-raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-
-tf-code-ec2-insances-example.gif) --- ### Interactive Wizard to create balcony
-import configurations Balcony doesn't know how to create terraform `import
-blocks` for all of the AWS resources. It can be taught how to do it by creating
-`import-configurations` yaml files, but it's a manual process. This is where
-the interactive wizard comes in. Interactive Wizards asks you required
-questions to automatically create the `import-configurations` yaml files.
-Related Docs: [Terraform Import Configuration Wizard](https://oguzhan-
-yilmaz.github.io/balcony/terraform-import-wizard/) ![](https://
-raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-
-wizard-security-groups-example.gif)
+oguzhan-yilmaz.github.io/balcony/terraform-import/) Related Docs: [Balcony
+Terraform Import Support Matrix](https://oguzhan-yilmaz.github.io/balcony/
+terraform-import-support-matrix/) ![](https://raw.githubusercontent.com/
+oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif) --
+- ### Generate actual Terraform Resource Code If you have: - initialized
+terraform project - `import_blocks.tf` file that's generated with `balcony
+terraform-import` command you can run `terraform plan -generate-config-
+out=generated.tf` to generate actual `.tf` resource code. This feature is
+achieved with the [balcony-terraform-import Docker Image](https://github.com/
+oguzhan-yilmaz/balcony/pkgs/container/balcony-terraform-import). Related Docs:
+[Generate Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/
+balcony/terraform-import-docker/) ![](https://raw.githubusercontent.com/
+oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-
+example.gif) --- ### Interactive Wizard to create balcony import configurations
+Balcony doesn't know how to create terraform `import blocks` for all of the AWS
+resources. It can be taught how to do it by creating `import-configurations`
+yaml files, but it's a manual process. This is where the interactive wizard
+comes in. Interactive Wizards asks you required questions to automatically
+create the `import-configurations` yaml files. Related Docs: [Terraform Import
+Configuration Wizard](https://oguzhan-yilmaz.github.io/balcony/terraform-
+import-wizard/) ![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-
+assets/main/gifs/terraform-wizard-security-groups-example.gif)
```

